---
title: Erstellen und Verwalten von privaten Azure Marketplace in Azure-Portal
description: Erfahren Sie mehr über das Erstellen und Verwalten von privaten Azure Marketplace (Vorschau) im Azure-Portal.
ms.prod: marketplace-customer
ms.topic: article
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 1333bb2c8830cec83d7b7f05890af818d5c0ce5b
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94487702"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Erstellen und Verwalten von privaten Azure Marketplace (Vorschau) im Azure-Portal

Mit der privaten Azure Marketplace (Vorschauversion) können Administratoren steuern, welche Lösungen von Drittanbietern Ihre Benutzer verwenden können. Dies ermöglicht es Ihnen, nur Angebote bereitzustellen, die Sie genehmigen und die den Richtlinien Ihres Unternehmens entsprechen. Mit dem privaten Azure Marketplace können Ihre Benutzer im Online Store nach kompatiblen angeboten zum Erwerb und Bereitstellen suchen. 

Als Marketplace-Administrator (zugewiesene Rolle) beginnen Sie mit einem deaktivierten und leeren privaten Speicher, in dem Sie Ihre genehmigten Angebote und Pläne hinzufügen können. In diesem Artikel wird erläutert, wie Sie private Azure Marketplace für Ihre Benutzer erstellen, verwalten und aktivieren.

Hinweise:

- Private Azure Marketplace befinden sich auf Mandanten Ebene, sodass allen Benutzern unter dem Mandanten dieselbe Liste angezeigt wird.
- Alle Microsoft-Lösungen werden automatisch privaten Azure Marketplace hinzugefügt.

## <a name="assign-the-marketplace-admin-role"></a>Zuweisen der Marketplace-Administrator Rolle

Der globale Administrator des Mandanten muss die **Marketplace-Administrator** Rolle dem privaten Azure Marketplace-Administrator zuweisen, der den privaten Speicher verwalten wird.

>[!IMPORTANT]
> Der Zugriff auf die private Azure Marketplace Verwaltung ist nur für IT-Administratoren mit zugewiesener Marketplace-Administrator Rolle verfügbar.

### <a name="prerequisites"></a>Voraussetzungen

Sie müssen diese Voraussetzungen erfüllen, bevor Sie die Marketplace-Administrator Rolle einem Benutzer im Mandanten Bereich zuweisen können:

- Sie haben Zugriff auf einen **globalen Administrator** Benutzer.
- Der Mandant verfügt über mindestens ein Abonnement (kann ein beliebiger Typ sein).
- Dem globalen Administrator Benutzer wird die Rolle " **Mitwirkender** " oder höher für das Abonnement zugewiesen, das Sie in Schritt 2 ausgewählt haben.
- Für den Benutzer des globalen Administrators ist der Zugriff auf **Ja** festgelegt (siehe [Elevate-Access-Global-admin](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Zuweisen der Marketplace-Administrator Rolle mithilfe von PowerShell

Verwenden Sie das folgende PowerShell-Skript, um die Marketplace-Administrator Rolle zuzuweisen. hierfür sind die folgenden Parameter erforderlich:

- **Tenantid:** Die ID des Mandanten im Bereich (Marketplace-Administrator Rolle kann im Mandanten Bereich zugewiesen werden).
- **Abonnement-ID:** Ein Abonnement, für das dem globalen Administrator die Rolle " **Mitwirkender** " oder höher zugewiesen ist.
- **Globaladminusername:** Der Benutzername des globalen Administrators.
- **Usernametozuzuzutragrolefor:** Der Benutzername, dem die Marketplace-Administrator Rolle zugewiesen wird.

> [!NOTE]
> Für Gastbenutzer, die an den Mandanten eingeladen wurden, kann es bis zu 48 Stunden dauern, bis Ihr Konto zum Zuweisen der Marketplace-Administrator Rolle verfügbar ist. Weitere Informationen finden Sie unter [Eigenschaften eines Azure Active Directory B2B-Kollaborations Benutzers](/azure/active-directory/b2b/user-properties).

```PowerShell
function Assign-MarketplaceAdminRole {
[CmdletBinding()]
param(
[Parameter(Mandatory)]
[string]$TenantId,

[Parameter(Mandatory)]
[string]$SubscriptionId,

[Parameter(Mandatory)]
[string]$GlobalAdminUsername,

[Parameter(Mandatory)]
[string]$UsernameToAssignRoleFor
)

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin"

Write-Output "TenantId = $TenantId"
Write-Output "SubscriptionId = $SubscriptionId"
Write-Output "GlobalAdminUsername = $GlobalAdminUsername"
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor"

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)"

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

if($profile -eq $null)
{
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop
}
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername)
{
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)"
}
else
{
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)"
}

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

Weitere Informationen zu den im AZ. Portal PowerShell-Modul enthaltenen Cmdlets finden Sie unter [Microsoft Azure PowerShell: Portal-Dashboard-Cmdlets](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Private Azure Marketplace erstellen

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
2. Wählen Sie **alle Dienste** und dann **Marketplace** aus.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure-Portal Hauptfenster.":::

3. Wählen Sie den **privaten Marketplace** aus den Optionen auf der linken Seite aus.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Wählen Sie im Hauptfenster des Azure-Portal den privaten Marketplace aus.":::

4. Wählen Sie " **starten** ", um eine private Azure Marketplace zu erstellen (Dies ist nur einmal erforderlich).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Klicken Sie im Azure-Portal Hauptfenster auf &quot;starten&quot;.":::

    Wenn für diesen Mandanten bereits private Azure Marketplace vorhanden sind, wird standardmäßig die Option " **Marketplace verwalten** " ausgewählt.

5. Nach Abschluss des Vorgangs verfügen Sie über eine leere und deaktivierte private Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Der leere private Azure Marketplace Bildschirm.":::

## <a name="add-items-from-gallery"></a>Elemente aus Katalog hinzufügen

Ein Element ist eine Kombination aus einem Angebot und einem Plan. Sie können auf der Seite Marketplace verwalten nach Elementen suchen und Elemente hinzufügen.

1. Wählen Sie **Elemente hinzufügen** aus.

2. Durchsuchen **Sie den Katalog, oder verwenden** Sie das Suchfeld, um das gewünschte Element zu finden.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Durchsuchen des Katalogs oder Verwenden des Suchfelds.":::

3. Beim Hinzufügen eines neuen Angebots werden standardmäßig alle aktuellen Pläne der Zulassungsliste hinzugefügt. Um die Plan Auswahl vor dem Hinzufügen der ausgewählten Elemente zu ändern, wählen Sie das Dropdown Menü in der Kachel des Angebots aus, und aktualisieren Sie die erforderlichen Pläne.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualisieren Sie die erforderlichen Pläne.":::

4. Klicken Sie unten links auf **Done (abgeschlossen** ), nachdem Sie Ihre Auswahl getroffen haben.

>[!Note]
> Das **Hinzufügen von Elementen** zum Marketplace ist nur für Angebote verfügbar, die nicht von Microsoft unterstützt werden. Microsoft-Angebote sind standardmäßig zulässig.

## <a name="edit-item-plans"></a>Element Pläne bearbeiten

Sie können die Pläne eines Elements auf der Seite "Marketplace verwalten" bearbeiten.

1. Überprüfen Sie die verfügbaren Pläne in der Spalte **Pläne** im Dropdown Menü für dieses Element.
2. Aktivieren bzw. deaktivieren Sie die Kontrollkästchen, um auszuwählen, welche Pläne Ihren Benutzern zur Verfügung gestellt werden sollen.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Aktivieren oder Deaktivieren des Kontrollkästchens für das erforderliche Element":::

> [!NOTE]
> Für jedes Angebot muss mindestens ein Plan ausgewählt sein, damit das Update ausgeführt wird. Löschen Sie das gesamte Angebot (siehe nächster Abschnitt), um alle Pläne im Zusammenhang mit einem Angebot zu entfernen.

## <a name="delete-offers"></a>Löschen von Angeboten

Aktivieren Sie auf der Seite Marketplace verwalten das Kontrollkästchen neben dem Angebots Namen (siehe Bildschirm oben), und wählen Sie **Elemente löschen** aus.

## <a name="enabledisable-private-azure-marketplace"></a>Private Azure Marketplace aktivieren/deaktivieren

Auf der Seite "Marketplace verwalten" finden Sie einen dieser Banner, der den aktuellen Status privater Azure Marketplace anzeigt:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zustands Banner deaktivieren":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Status Banner aktivieren":::

Sie können private Azure Marketplace nach Bedarf aktivieren oder deaktivieren.

1. Wenn diese Option deaktiviert ist, aktivieren Sie die Option **privaten Marketplace aktivieren** aktivieren.
2. Wenn diese Option aktiviert ist, wählen Sie den **privaten Marketplace deaktivieren** aus

## <a name="browsing-private-azure-marketplace"></a>Private Azure Marketplace durchsuchen

Wenn private Azure Marketplace aktiviert ist, wird Benutzern angezeigt, welche Pläne der Marketplace-Administrator zugelassen hat.

- Ein grüner **Allowed** zulässiger Hinweis gibt an, dass es sich um ein Angebot eines Partners (nicht-Microsoft) handelt.
- Ein blauer **Allowed** zulässiger Hinweis gibt ein zulässiges Microsoft-Angebot an.

Benutzer können zwischen angeboten filtern, die nicht zulässig sind und nicht zulässig sind:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filteroption.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>In privatem Azure Marketplace kaufen oder bereitstellen

Während die Produktdetailseite dem öffentlichen Azure Marketplace ähnelt, gibt es drei private Azure Marketplace spezifische Szenarien.

- Wenn ein Benutzer einen zulässigen Plan auswählt, wird die Schaltfläche **Erstellen** aktiviert:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Angebots Banner mit dem Hinweis, dass ein Plan erstellt werden kann.":::

- Wenn ein Benutzer einen nicht zulässigen Plan auswählt, wird in einem Banner darauf hingewiesen, dass der Plan nicht zulässig ist und die Schaltfläche **Erstellen** deaktiviert ist.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Angebots Banner mit einem Plan können nicht erstellt werden.":::

- Wenn eine Produkt Plan Auswahl nicht auf der Seite Produktdetails angezeigt wird, aber der Administrator einen oder mehrere Pläne genehmigt hat, wird in einem Banner festgestellt, welche Pläne zulässig sind und wie die Schaltfläche **Erstellen** aktiviert ist:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Angebots Banner mit dem Hinweis, dass ein Plan erstellt und verfügbare Pläne angezeigt werden können.":::

## <a name="contact-support"></a>Kontaktieren Sie den Support.

Azure Marketplace Unterstützung finden Sie unter [Microsoft Q&A](/answers/products/). 
