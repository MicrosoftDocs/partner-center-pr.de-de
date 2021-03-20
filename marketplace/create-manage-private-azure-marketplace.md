---
title: Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal
description: Erfahren Sie mehr über das Erstellen und Verwalten von privaten Azure Marketplace (Vorschau) im Azure-Portal. Mit der privaten Azure Marketplace (Vorschauversion) können Administratoren steuern, welche Lösungen von Drittanbietern Ihre Benutzer verwenden können.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712765"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal

Mit der privaten Azure Marketplace können Administratoren bestimmen, welche Lösungen von Drittanbietern Ihre Benutzer verwenden können. Dies bewirkt, dass der Benutzer nur Angebote bereitstellen kann, die vom Administrator genehmigt werden und den Richtlinien Ihres Unternehmens entsprechen. Mit dem privaten Azure Marketplace können Benutzer im Online Store nach kompatiblen angeboten zum Erwerb und Bereitstellen suchen.

Als Marketplace-Administrator (zugewiesene Rolle) beginnen Sie mit einem deaktivierten und leeren privaten Speicher, in dem Sie Ihre genehmigten Angebote und Pläne hinzufügen können. In diesem Artikel wird erläutert, wie Sie die erforderliche Rolle zuweisen, einen privaten Speicher erstellen, Elemente verwalten, Benutzer Anforderungen genehmigen und private Azure Marketplace für Ihre Benutzer aktivieren.

> [!NOTE]
> - Private Azure Marketplace befinden sich auf Mandanten Ebene, sodass allen Benutzern unter dem Mandanten dieselbe Liste angezeigt wird.
> - Alle Microsoft-Lösungen (einschließlich unterstütztes [Linux-Verteilungen](/azure/virtual-machines/linux/endorsed-distros)) werden automatisch privaten Azure Marketplace hinzugefügt.

## <a name="assign-the-marketplace-admin-role"></a>Zuweisen der Marketplace-Administrator Rolle

Der globale Administrator des Mandanten muss die **Marketplace-Administrator** Rolle dem privaten Azure Marketplace-Administrator zuweisen, der den privaten Speicher verwalten wird.

>[!IMPORTANT]
> Der Zugriff auf die private Azure Marketplace Verwaltung ist nur für IT-Administratoren mit zugewiesener Marketplace-Administrator Rolle verfügbar.

### <a name="prerequisites"></a>Voraussetzungen

Diese Voraussetzungen sind erforderlich, bevor Sie die Marketplace-Administrator Rolle einem Benutzer im Mandanten Bereich zuweisen können:

- Sie haben Zugriff auf einen **globalen Administrator** Benutzer.
- Der Mandant verfügt über mindestens ein Abonnement (kann ein beliebiger Typ sein).
- Dem globalen Administrator Benutzer wird die Rolle " **Mitwirkender** " oder höher für das ausgewählte Abonnement zugewiesen.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Zuweisen der Marketplace-Administrator Rolle mit Access Control (IAM)

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
1. Wählen Sie **alle Dienste** und dann **Marketplace** aus.
1. Wählen Sie im Menü auf der linken Seite **privater Marketplace** aus.

    [![Zeigt die Menüoption für den privaten Marketplace auf der linken Seite des Marketplace an.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Wählen Sie **Zugriffs Steuerung (IAM)** , um die Rolle Marketplace-Administrator zuzuweisen.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zeigt den Bildschirm I A M Access Control an.":::

1. Wählen Sie **+Hinzufügen** > **Rollenzuweisung hinzufügen** aus.
1. Wählen Sie unter **Rolle** die Option **Marketplace-Administrator** aus.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zeigt das Rollen Zuweisungs Menü an.":::

1. Wählen Sie in der Dropdown Liste den gewünschten Benutzer aus, und wählen Sie dann **abgeschlossen** aus.

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

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

Weitere Informationen zu den im AZ. Portal PowerShell-Modul enthaltenen Cmdlets finden Sie unter [Microsoft Azure PowerShell: Portal-Dashboard-Cmdlets](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Private Azure Marketplace erstellen

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
2. Wählen Sie **alle Dienste** und dann **Marketplace** aus.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zeigt das Azure-Portal Hauptfenster an.":::

3. Wählen Sie im Menü auf der linken Seite **privater Marketplace** aus.

4. Wählen Sie " **starten** ", um eine private Azure Marketplace zu erstellen (Dies ist nur einmal erforderlich).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Zeigt, wie das Hauptfenster &quot;get started on the Azure-Portal&quot; ausgewählt wird.":::

    Wenn für diesen Mandanten bereits private Azure Marketplace vorhanden sind, wird standardmäßig die Option " **Marketplace verwalten** " ausgewählt.

5. Nach Abschluss des Vorgangs verfügen Sie über eine leere und deaktivierte private Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zeigt den leeren privaten Azure Marketplace Bildschirm an.":::

## <a name="add-items-from-gallery"></a>Elemente aus Katalog hinzufügen

Ein Element ist eine Kombination aus einem Angebot und einem Plan. Sie können auf der Seite Marketplace verwalten nach Elementen suchen und diese hinzufügen.

1. Wählen Sie **Elemente hinzufügen** aus.

2. Durchsuchen **Sie den Katalog, oder verwenden** Sie das Suchfeld, um das gewünschte Element zu finden.

    [![Zeigt, wie Sie den Katalog durchsuchen oder das Suchfeld verwenden.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Beim Hinzufügen eines neuen Angebots werden standardmäßig alle aktuellen Pläne der genehmigten Liste hinzugefügt. Um die Plan Auswahl vor dem Hinzufügen der ausgewählten Elemente zu ändern, wählen Sie das Dropdown Menü in der Kachel des Angebots aus, und aktualisieren Sie die erforderlichen Pläne.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Zeigt, wie die erforderlichen Pläne aktualisiert werden.":::

4. Klicken Sie unten links auf **Done (abgeschlossen** ), nachdem Sie Ihre Auswahl getroffen haben.

>[!Note]
> Das **Hinzufügen von Elementen** zum Marketplace ist nur für Angebote verfügbar, die nicht von Microsoft unterstützt werden. Microsoft-Lösungen (einschließlich unterstützter [Linux-Verteilungen](/azure/virtual-machines/linux/endorsed-distros)) werden als "standardmäßig genehmigt" gekennzeichnet und können nicht im privaten Marketplace verwaltet werden.

## <a name="edit-items-plans"></a>Element Pläne bearbeiten

Sie können die Pläne eines Elements auf der Seite "Marketplace verwalten" bearbeiten.

1. Überprüfen Sie die verfügbaren Pläne in der Spalte **Pläne** im Dropdown Menü für dieses Element.
2. Aktivieren bzw. deaktivieren Sie die Kontrollkästchen, um auszuwählen, welche Pläne Ihren Benutzern zur Verfügung gestellt werden sollen.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zeigt, wie das Kontrollkästchen für das erforderliche Element aktiviert oder deaktiviert wird.":::

> [!NOTE]
> Jedes Angebot benötigt mindestens einen Plan, der für das Update ausgewählt ist. Löschen Sie das gesamte Angebot (siehe nächster Abschnitt), um alle Pläne im Zusammenhang mit einem Angebot zu entfernen.

## <a name="delete-offers"></a>Löschen von Angeboten

Aktivieren Sie auf der Seite Marketplace verwalten das Kontrollkästchen neben dem Angebots Namen (siehe Bildschirm oben), und wählen Sie **Elemente löschen** aus.

## <a name="enabledisable-private-azure-marketplace"></a>Private Azure Marketplace aktivieren/deaktivieren

Auf der Seite "Marketplace verwalten" finden Sie einen dieser Banner, der den aktuellen Status privater Azure Marketplace anzeigt:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zeigt das Banner &quot;Zustand deaktivieren&quot; an.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zeigt das Banner &quot;Enable State&quot; an.":::

Sie können private Azure Marketplace nach Bedarf aktivieren oder deaktivieren.

- Wenn diese Option deaktiviert ist, aktivieren Sie die Option **privaten Marketplace aktivieren** aktivieren.
- Wenn diese Option aktiviert ist, wählen Sie den **privaten Marketplace deaktivieren** aus

## <a name="private-azure-marketplace-notification-center"></a>Benachrichtigungs Center für private Azure Marketplace

Das Benachrichtigungs Center besteht aus drei Arten von Benachrichtigungen und ermöglicht dem Marketplace-Administrator, basierend auf der Benachrichtigung Aktionen durchführen zu können:

- Genehmigungsanforderungen von Benutzern für Elemente, die sich nicht in der genehmigten Liste befinden (siehe [Anforderung zum Hinzufügen von angeboten oder Plänen](#request-to-add-offers-or-plans) unten).
- Neue Plan Benachrichtigungen für Angebote, die bereits über einen oder mehrere Pläne in der genehmigten Liste verfügen.
- Die Plan Benachrichtigungen für Elemente, die sich in der genehmigten Liste befinden, aber aus der globalen Azure Marketplace entfernt wurden, wurden entfernt.

So greifen Sie auf das Benachrichtigungs Center zu:

1. Wählen Sie im Menü auf der linken Seite die Option **Benachrichtigungen** aus.

    [![Zeigt das Menü Benachrichtigungen an.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Wählen Sie das Menü mit den Auslassungs Punkten für weitere Aktionen aus.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zeigt die Menü Ergebnisse der weiteren Optionen an.":::

1. Bei Plan Anforderungen wird durch **Anzeigen von Anforderungen** das Formular Genehmigungs Anforderung geöffnet, in dem Sie alle Benutzer Anforderungen für das jeweilige Angebot überprüfen können.
1. Wählen Sie **genehmigen** oder **ablehnen** aus.

    [![Zeigt die Optionen "genehmigen" und "ablehnen" an.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Wählen Sie im Dropdown Menü den Plan aus, der genehmigt werden soll.
1. Fügen Sie einen Kommentar hinzu, und wählen Sie **senden** aus.

## <a name="browsing-private-azure-marketplace"></a>Private Azure Marketplace durchsuchen

Wenn private Azure Marketplace aktiviert ist, sehen Benutzer, welche Pläne der Marketplace-Administrator genehmigt hat.

- Ein grünes **genehmigter** Hinweis gibt an, dass ein von ihnen genehmigtes Partner Angebot (nicht von Microsoft) genehmigt wird.
- Ein blauer **genehmigter** Hinweis gibt an, dass ein Microsoft-Angebot (einschließlich unterstütztes [Linux-Verteilungen](/azure/virtual-machines/linux/endorsed-distros)) genehmigt ist.

Benutzer können zwischen angeboten filtern, die nicht genehmigt sind und nicht genehmigt sind:

[![Zeigt die Filteroption an.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>In privatem Azure Marketplace kaufen oder bereitstellen

Während die Produktdetailseite dem globalen Azure Marketplace ähnelt, gibt es drei private Azure Marketplace spezifische Szenarien.

- Wenn ein Benutzer einen genehmigten Plan auswählt, wird die Schaltfläche " **Erstellen** " aktiviert:

    [![Zeigt das Angebots Banner an, das anzeigt, dass ein Plan erstellt werden kann.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Wenn eine Produkt Plan Auswahl nicht auf der Seite Produktdetails angezeigt wird, aber der Administrator einen oder mehrere Pläne genehmigt hat, wird in einem Banner festgestellt, welche Pläne genehmigt und die Schaltfläche **Erstellen** aktiviert ist:

    [![Zeigt das Angebots Banner an, das darauf hinweist, dass ein Plan erstellt und verfügbare Pläne angezeigt werden kann.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Wenn ein Benutzer einen nicht genehmigten Plan auswählt, wird in einem Banner der Plan als nicht genehmigt festgestellt, und die Schaltfläche **Erstellen** ist deaktiviert. Der Benutzer kann weiterhin anfordern, den Plan der genehmigten Liste hinzuzufügen (siehe nächster Abschnitt).

## <a name="request-to-add-offers-or-plans"></a>Anforderung zum Hinzufügen von angeboten oder Plänen

Sie können anfordern, ein öffentliches Angebot oder einen Plan hinzuzufügen, der im privaten Azure Marketplace derzeit nicht genehmigt ist.

1. Wählen Sie **Anforderung zum Hinzufügen** im Banner aus, um das Formular für die **Zugriffs Anforderung** zu öffnen.

    [![Zeigt das Banner mit dem Link "Anforderung zum Hinzufügen" an.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Zeigt das Zugriffs Anforderungs Formular für Angebote oder Pläne an.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Wählen Sie aus, welche Pläne der Anforderung hinzugefügt werden sollen (**Jeder Plan** weist den Marketplace-Administrator an, dass Sie keinen Plan innerhalb eines Angebots bevorzugen).

1. Fügen Sie eine **Begründung** und eine **Anforderung** zum Übermitteln Ihrer Anforderung hinzu.
  
    [![Zeigt das Zugriffs Anforderungs Formular für Angebote oder Pläne mit Beispieleinträgen an.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Eine Angabe für eine ausstehende Anforderung wird im Zugriffs Anforderungs Formular mit einer Option zum **zurückziehen der Anforderung** angezeigt.

    [![Zeigt eine Liste mit genehmigten oder ausstehenden Plänen mit einem Link zum Widerrufen der Anforderung an.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Nachdem die Anforderung gesendet wurde, wird das Genehmigungs Anforderungs Formular an das [Benachrichtigungs Center](#private-azure-marketplace-notification-center) für den Marketplace-Administrator gesendet, um die Anforderung zu überprüfen und Maßnahmen zu ergreifen.

## <a name="frequently-asked-questions-faqs"></a>Häufig gestellte Fragen (FAQs)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Ich blockiere die Marketplace-Drittanbieter Anwendung bereits über Azure Policy. Wie sieht das anders aus?

Es gibt derzeit zwei Möglichkeiten, Dienste von Drittanbietern im Marketplace einzuschränken:

1. Deaktivieren Sie über das EA-Portal oder das Azure-Portal Dienste von Drittanbietern, oder beschränken Sie diese auf "kostenlose oder byol-SKUs".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Zeigt, wie Dienste im Azure-Portal eingeschränkt werden.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Zeigt, wie Dienste im E-A-Portal eingeschränkt werden.":::

2. Erstellen Sie eine Azure-Richtlinie, um nur bestimmte VMS zuzulassen. Ausführliche Informationen zum Erzwingen von Richtlinien für virtuelle Windows-Computer finden Sie unter [Anwenden von Richtlinien auf Windows-VMS mit Azure Resource Manager](/azure/virtual-machines/windows/policy).

Die private Azure Marketplace ermöglicht mehr Flexibilität bei der Einschränkung und bei der Ermöglichung spezifischer Angebote und Pläne. Er informiert Endbenutzer über die Verfügbarkeit für die Bereitstellung im Marketplace-Katalog, auch wenn Sie versuchen, Drittanbieter Dienste bereitzustellen. Um die Bereitstellung von Diensten von Drittanbietern zuzulassen, legen Sie im EA-Portal und im Azure-Portal Azure Marketplace auf ein/aktivieren fest.

- Private Azure Marketplace können Partner Lösungen, die nicht auf virtuelle Computer beschränkt sind, mit anderen Werten
- Private Azure Marketplace können auf Planebene einen Cursor einrichten und können auch "aktueller und zukünftiger Plan" festlegen.
- Der private Azure Marketplace kann die Endbenutzer darüber informieren, was bereitgestellt werden kann und was nicht.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Worin besteht der Unterschied zwischen einem privaten Angebot und einem privaten Azure Marketplace?

Ein **privates Angebot** ermöglicht Verlegern das Erstellen von Plänen, die nur für Zielkunden sichtbar sind. Dies ermöglicht es Ihnen, angepasste Lösungen privat mit ausgehandelten Preisen, privaten Geschäftsbedingungen und spezialisierten Konfigurationen gemeinsam zu nutzen. Weitere Informationen finden Sie unter [private Angebote im kommerziellen Marketplace](/azure/marketplace/private-offers).

Mit dem **privaten Azure Marketplace** in der Azure-Portal können Administratoren vorab genehmigen, welche Lösungen von Drittanbietern Ihre Benutzer bereitstellen können. Bei einer privaten Azure Marketplace können die Benutzer die Vorteile der Azure Marketplace nutzen, indem Sie kompatible Angebote finden, kaufen und bereitstellen. Zum Verwalten von Abonnement basierten privaten angeboten im privaten Marketplace muss der Marketplace-Administrator mindestens über die Rolle "lesen" für das jeweilige Abonnement verfügen.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Ich habe dem privaten Azure Marketplace ein privates Angebot hinzugefügt. Warum wird es nicht auf der Registerkarte "Marketplace verwalten" angezeigt?

Abonnement basierte private Angebote sind nur für die aufgeführten Abonnements in den Einstellungen des privaten Angebots sichtbar. Um das private Angebot anzuzeigen, stellen Sie sicher, dass der globale Abonnement Filter alle Abonnements anzeigt.

[![Zeigt den privaten Marketplace-Filter an.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Können wir benutzerdefinierte Images in private Azure Marketplace einschließen?

Nein. Die private Azure Marketplace ermöglicht IT-Administratoren, Lösungen von Drittanbietern von globalen Azure Marketplace zu verwalten und zu betreiben. Da benutzerdefinierte Images sich nicht auf globalen Azure Marketplace befinden, kann der IT-Administrator die benutzerdefinierten Images nicht auswählen und auswählen. Wenn Sie benutzerdefinierte Images freigeben möchten, verwenden Sie die frei [gegebene Image Galerie](/azure/virtual-machines/shared-image-galleries).

1. Schritt-für-Schritt-Anleitung Erstellen eines freigegebenen Image Katalogs (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Erstellen Sie eine Image Definition innerhalb von SIG. Der Kunde sollte für das Feld "OS-State" **generalisiert** auswählen. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Bringen Sie ein verwaltetes Image in den freigegebenen Image Katalog ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. Die SIG-VM-Images befinden sich in einem Abonnement. Verwenden Sie eine APP-Registrierung ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)), um Sie für andere Abonnements verfügbar zu machen.

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Warum werden einige Angebote **standardmäßig genehmigt** , auch wenn der Verleger nicht Microsoft ist?

Microsoft unterstützt Linux-und Open-Source-Technologie in Azure. Unterstützte [Linux-Distributionen](/azure/virtual-machines/linux/endorsed-distros) werden in Azure unterstützt, und der Preis ist in virtuelle Computer integriert. Da der Azure Linux-Agent bereits auf Azure Marketplace vorinstalliert ist, wird er wie ein Microsoft-Angebot behandelt. Da Microsoft-Angebote standardmäßig genehmigt werden, können unterstützte Linux-Distributionen nicht in privaten Azure Marketplace verwaltet werden und sind standardmäßig genehmigt.

## <a name="contact-support"></a>Kontaktieren des Supports

- Azure Marketplace Unterstützung finden Sie unter [Microsoft Q&A](/answers/products/).