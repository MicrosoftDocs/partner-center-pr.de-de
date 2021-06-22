---
title: Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal
description: Erfahren Sie mehr über das Erstellen und Verwalten von privaten Azure Marketplace (Vorschauversion) im Azure-Portal. Mit privatem Azure Marketplace (Vorschau) können Administratoren steuern, welche Drittanbieterlösungen ihre Benutzer verwenden können.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431670"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal

Mit privatem Azure Marketplace können Administratoren steuern, welche Drittanbieterlösungen ihre Benutzer verwenden können. Hierzu kann der Benutzer nur Angebote bereitstellen, die vom Administrator genehmigt wurden und den Richtlinien Ihres Unternehmens entsprechen. Mit privatem Azure Marketplace können Benutzer im Onlineshop nach kompatiblen Angeboten suchen, die erworben und bereitgestellt werden können.

Als Marketplace-Administrator (zugewiesene Rolle) beginnen Sie mit einem deaktivierten und leeren privaten Store, in dem Sie Ihre genehmigten Angebote und Pläne hinzufügen können. In diesem Artikel wird erläutert, wie Sie die erforderliche Rolle zuweisen, einen privaten Speicher erstellen, Elemente verwalten, Benutzeranforderungen genehmigen und private Azure Marketplace für Ihre Benutzer aktivieren.

> [!NOTE]
> - Private Azure Marketplace befindet sich auf Mandantenebene, sodass allen Benutzern unter dem Mandanten die gleiche zusammengestellte Liste angezeigt wird.
> - Alle Microsoft-Lösungen (einschließlich [unterstützter Linux-Distributionen)](/azure/virtual-machines/linux/endorsed-distros)werden automatisch privaten Azure Marketplace hinzugefügt.

## <a name="assign-the-marketplace-admin-role"></a>Zuweisen der Marketplace-Administratorrolle

Der Globaler Administrator des Mandanten muss die **Marketplace-Administratorrolle** dem Privaten Azure Marketplace Administrator zuweisen, der den privaten Speicher verwaltet.

>[!IMPORTANT]
> Der Zugriff auf private Azure Marketplace-Verwaltung ist nur für IT-Administratoren verfügbar, deren Marketplace-Administratorrolle zugewiesen ist.

### <a name="prerequisites"></a>Voraussetzungen

Diese Voraussetzungen sind erforderlich, bevor Sie einem Benutzer im Mandantenbereich die Rolle "Marketplace-Administrator" zuweisen können:

- Sie haben Zugriff auf einen **globaler Administrator** Benutzer.
- Der Mandant verfügt über mindestens ein Abonnement (kann ein beliebiger Typ sein).
- Dem globaler Administrator Benutzer wird die Rolle **Mitwirkender** oder höher für das ausgewählte Abonnement zugewiesen.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Zuweisen der Marketplace-Administratorrolle mit Zugriffssteuerung (IAM)

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
1. Wählen Sie **Alle Dienste** und dann **Marketplace** aus.
1. Wählen  Sie im Menü auf der linken Seite Private Marketplace aus.

    [![Zeigt die Menüoption "Privater Marketplace" auf der linken Seite des Marketplace an.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Wählen Sie **Zugriffssteuerung (IAM)** aus, um die Marketplace-Administratorrolle zuzuweisen.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zeigt den I A M-Bildschirm für die Zugriffssteuerung an.":::

1. Wählen Sie **+Hinzufügen** > **Rollenzuweisung hinzufügen** aus.
1. Wählen Sie unter **Rolle** die Option **Marketplace-Administrator** aus.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zeigt das Menü Rollenzuweisung an.":::

1. Wählen Sie in der Dropdownliste den gewünschten Benutzer und dann **Fertig** aus.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Zuweisen der Marketplace-Administratorrolle mit PowerShell

Verwenden Sie das folgende PowerShell-Skript, um die Rolle "Marketplace-Administrator" zuzuweisen. es sind die folgenden Parameter erforderlich:

- **TenantId:** Die ID des Mandanten im Bereich (Die Marketplace-Administratorrolle kann für den Mandantenbereich zugewiesen werden).
- **SubscriptionId:** Ein Abonnement, dem der globale Administrator die Rolle **Mitwirkender** oder höher zugewiesen hat.
- **GlobalAdminUsername:** Der Benutzername des globalen Administrators.
- **UsernameToAssignRoleFor:** Der Benutzername, dem die Marketplace-Administratorrolle zugewiesen wird.

> [!NOTE]
> Für Gastbenutzer, die zum Mandanten eingeladen werden, kann es bis zu 48 Stunden dauern, bis ihr Konto für die Zuweisung der Marketplace-Administratorrolle verfügbar ist. Weitere Informationen finden Sie unter [Eigenschaften eines Azure Active Directory B2B-Zusammenarbeitsbenutzers.](/azure/active-directory/b2b/user-properties)

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

Weitere Informationen zu den Cmdlets, die im Az.Portal PowerShell-Modul enthalten sind, finden Sie unter [Microsoft Azure PowerShell: Portaldashboard-Cmdlets.](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>Erstellen eines privaten Azure Marketplace

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
2. Wählen Sie **Alle Dienste** und dann **Marketplace** aus.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zeigt das Azure-Portal Hauptfenster an.":::

3. Wählen  Sie im Menü auf der linken Seite Private Marketplace aus.

4. Wählen Sie **Los geht's** aus, um private Azure Marketplace zu erstellen (sie müssen dies nur einmal tun).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Zeigt, wie Sie im Hauptfenster des Azure-Portal die Los geht's auswählen.":::

    Wenn private Azure Marketplace für diesen Mandanten bereits vorhanden ist, wird Marketplace **verwalten** standardmäßig ausgewählt.

5. Nach Abschluss des Abschlusses verfügen Sie über eine leere und deaktivierte private Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zeigt den leeren Bildschirm private Azure Marketplace an.":::

## <a name="add-items-from-gallery"></a>Hinzufügen von Elementen aus dem Katalog

Ein Element ist eine Kombination aus einem Angebot und einem Plan. Sie können auf der Seite Marketplace verwalten nach Elementen suchen und elemente hinzufügen.

1. Wählen Sie **Elemente hinzufügen aus.**

2. Durchsuchen Sie den **Katalog,** oder verwenden Sie das Suchfeld, um das gewünschte Element zu suchen.

    [![Zeigt, wie Sie den Katalog durchsuchen oder das Suchfeld verwenden.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Standardmäßig werden beim Hinzufügen eines neuen Angebots alle aktuellen Pläne der genehmigten Liste hinzugefügt. Um die Planauswahl vor dem Hinzufügen der ausgewählten Elemente zu ändern, wählen Sie das Dropdownmenü auf der Kachel des Angebots aus, und aktualisieren Sie die erforderlichen Pläne.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Zeigt, wie erforderliche Pläne aktualisiert werden.":::

4. Wählen Sie unten links **Fertig** aus, nachdem Sie Ihre Auswahl getroffen haben.

>[!Note]
> **Das Hinzufügen von Elementen** zum Marketplace ist nur für Nicht-Microsoft-Angebote verfügbar. Microsoft-Lösungen (einschließlich [unterstützter Linux-Distributionen)](/azure/virtual-machines/linux/endorsed-distros)werden als "Standardmäßig genehmigt" gekennzeichnet und können nicht im privaten Marketplace verwaltet werden.

## <a name="edit-items-plans"></a>Bearbeiten von Elementplänen

Sie können die Pläne eines Elements auf der Seite Marketplace verwalten bearbeiten.

1. Überprüfen Sie in der Spalte **Pläne** die verfügbaren Pläne im Dropdownmenü für dieses Element.
2. Aktivieren oder deaktivieren Sie die Kontrollkästchen, um auszuwählen, welche Pläne Ihren Benutzern zur Verfügung gestellt werden sollen.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zeigt, wie sie das Kontrollkästchen für das erforderliche Element aktivieren oder deaktivieren.":::

> [!NOTE]
> Für jedes Angebot muss mindestens ein Plan ausgewählt sein, damit das Update durchgeführt werden kann. Um alle Pläne im Zusammenhang mit einem Angebot zu entfernen, löschen Sie das gesamte Angebot (siehe nächster Abschnitt).

## <a name="delete-offers"></a>Löschen von Angeboten

Aktivieren Sie auf der Seite Marketplace verwalten das Kontrollkästchen neben dem Angebotsnamen (siehe Bildschirm oben), und wählen Sie **Elemente löschen** aus.

## <a name="enabledisable-private-azure-marketplace"></a>Aktivieren/Deaktivieren von privaten Azure Marketplace

Auf der Seite Marketplace verwalten sehen Sie eines dieser Banner, das den aktuellen Status von Private Azure Marketplace zeigt:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zeigt das Banner &quot;Status deaktivieren&quot; an.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zeigt das Banner &quot;Status aktivieren&quot; an.":::

Sie können private Azure Marketplace nach Bedarf aktivieren oder deaktivieren.

- Wenn diese Option deaktiviert ist, wählen **Sie Privaten Marketplace** aktivieren aus, um dies zu aktivieren.
- Wenn diese Option aktiviert ist, wählen **Sie Privaten Marketplace** deaktivieren aus, um den Marketplace zu deaktivieren.

## <a name="private-azure-marketplace-notification-center"></a>Private Azure Marketplace Notification Center

Notification Center besteht aus drei Arten von Benachrichtigungen und ermöglicht dem Marketplace-Administrator das Ausführen von Aktionen basierend auf der Benachrichtigung:

- Genehmigungsanforderungen von Benutzern für Elemente, die nicht in der genehmigten Liste enthalten sind (siehe [Anforderung zum Hinzufügen von Angeboten oder Plänen](#request-to-add-offers-or-plans) weiter unten).
- Neue Planbenachrichtigungen für Angebote, die bereits einen oder mehrere Pläne in der genehmigten Liste enthalten.
- Planbenachrichtigungen für Elemente, die sich in der Genehmigten Liste befinden, aber aus der globalen Azure Marketplace entfernt wurden, wurden entfernt.

So greifen Sie auf die Mitteilungszentrale zu

1. Wählen Sie im Menü auf der linken Seite die Option **Benachrichtigungen** aus.

    [![Zeigt das Menü Benachrichtigungen an.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Wählen Sie das Menü mit den Auslassungszeichen aus, um weitere Aktionen anzuzeigen.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zeigt die Ergebnisse des Menüs Weitere Optionen an.":::

1. Bei Plananforderungen wird unter Anforderungen anzeigen das Formular für **genehmigungsanforderung** geöffnet, in dem Sie alle Benutzeranforderungen für das jeweilige Angebot überprüfen können.
1. Wählen Sie **Genehmigen** oder **Ablehnen aus.**

    [![Zeigt die Optionen zum Genehmigen und Ablehnen an.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Wählen Sie im Dropdownmenü den zu genehmigenden Plan aus.
1. Fügen Sie einen Kommentar hinzu, und wählen **Sie Senden** aus.

## <a name="browsing-private-azure-marketplace"></a>Durchsuchen privater Azure Marketplace

Wenn private Azure Marketplace aktiviert ist, sehen Benutzer, welche Pläne der Marketplace-Administrator genehmigt hat.

- Ein grünes **Genehmigtes** Benachrichtigungsmerkmal zeigt ein Partnerangebot (nicht von Microsoft) an, das genehmigt wurde.
- Ein blauer **Genehmigter** Hinweis weist auf ein Microsoft-Angebot (einschließlich [unterstützter Linux-Distributionen)](/azure/virtual-machines/linux/endorsed-distros)hin, das genehmigt wurde.

Benutzer können zwischen Angeboten filtern, die genehmigt sind und nicht genehmigt sind:

[![Zeigt die Filteroption an.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kaufen oder Bereitstellen in privatem Azure Marketplace

Die Seite mit den Produktdetails ähnelt der globalen Azure Marketplace, es gibt jedoch drei private Azure Marketplace spezifischen Szenarien.

- Wenn ein Benutzer einen genehmigten Plan auswählt, ist die Schaltfläche **Erstellen** aktiviert:

    [![Zeigt das Angebotsbanner an, in dem ein Plan erstellt werden kann.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Wenn eine Produktplanauswahl nicht auf der Seite mit den Produktdetails angezeigt wird, der Administrator jedoch mindestens einen Plan genehmigt hat, wird in einem Banner angegeben, welche Pläne genehmigt wurden und die Schaltfläche **Erstellen** aktiviert ist:

    [![Zeigt das Angebotsbanner an, das anzeigt, dass ein Plan erstellt werden kann, und zeigt verfügbare Pläne an.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Wenn ein Benutzer einen nicht genehmigten Plan auswählt, wird der Plan in einem Banner als nicht genehmigt markiert, und die Schaltfläche **Erstellen** ist deaktiviert. Der Benutzer kann weiterhin anfordern, den Plan der genehmigten Liste hinzuzufügen (siehe nächster Abschnitt).

## <a name="request-to-add-offers-or-plans"></a>Anforderung zum Hinzufügen von Angeboten oder Plänen

Sie können anfordern, ein öffentliches Angebot oder einen Plan hinzuzufügen, das bzw. der derzeit nicht im privaten Azure Marketplace genehmigt ist.

1. Wählen Sie **Anforderung aus, um** das Banner hinzuzufügen, um das Formular **Zugriffsanforderung** zu öffnen.

    [![Zeigt das Banner mit dem Link "Anforderung zum Hinzufügen" an.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Zeigt das Zugriffsanforderungsformular für Angebote oder Pläne an.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Wählen Sie aus, welche Pläne der Anforderung hinzugefügt werden sollen (**Jeder Plan** teilt dem Marketplace-Administrator mit, dass Sie keinen Plan innerhalb eines Angebots bevorzugen).

1. Fügen Sie eine **Begründung** hinzu, und wählen Sie **Anforderung** aus, um Ihre Anforderung zu übermitteln.
  
    [![Zeigt das Zugriffsanforderungsformular für Angebote oder Pläne mit Beispieleinträgen an.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Ein Hinweis auf eine ausstehende Anforderung wird im Formular Zugriffsanforderung mit einer Option zum **Abheben** der Anforderung angezeigt.

    [![Zeigt eine Liste mit genehmigten oder ausstehenden Plänen mit dem Link Zum Widerrufen einer Anforderung an.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Nach der Übermittlung wird das Genehmigungsanforderungsformular an das [Notification Center](#private-azure-marketplace-notification-center) gesendet, damit der Marketplace-Administrator die Anforderung überprüfen und Maßnahmen ergreifen kann.

> [!CAUTION]
> Die Genehmigung im privaten Marketplace weist nicht auf die Beschaffung einer Lösung hin.

## <a name="frequently-asked-questions-faqs"></a>Häufig gestellte Fragen (FAQs)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Ich blockiere bereits Marketplace-Drittanbieteranwendungen über Azure Policy. Wie unterscheidet sich dies?

Es gibt derzeit zwei Möglichkeiten, Dienste von Drittanbietern im Marketplace einzuschränken:

1. Deaktivieren Sie über das EA-Portal oder die Azure-Portal Drittanbieterdienste, oder beschränken Sie sie auf "Nur kostenlose oder BYOL-SKUs".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Zeigt, wie Dienste im Azure-Portal eingeschränkt werden.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Zeigt, wie Dienste im E A-Portal eingeschränkt werden.":::

2. Erstellen Sie eine Azure-Richtlinie, um nur bestimmte VMs zuzulassen. Ausführliche Informationen zum Erzwingen von Richtlinien auf virtuelle Windows-Computer finden Sie unter Anwenden von [Richtlinien auf virtuelle Windows-Computer mit Azure Resource Manager](/azure/virtual-machines/windows/policy).

Private Azure Marketplace ermöglicht mehr Flexibilität beim Einschränken und Zulassen bestimmter Angebote und Pläne. Endbenutzer werden über die Verfügbarkeit für die Bereitstellung im Marketplace-Katalog informiert, noch bevor sie versuchen, Drittanbieterdienste bereitzustellen. Um die Bereitstellung von Drittanbieterdiensten zu ermöglichen, legen Sie Azure Marketplace in EA Portal und der Azure-Portal auf Ein/Aktiviert fest.

- Private Azure Marketplace können Partnerlösungen zusammenbauen, die nicht auf virtuelle Computer beschränkt sind.
- Private Azure Marketplace können auf Planebene zusammenstellen und auch "Aktueller und zukünftiger Plan" festlegen.
- Private Azure Marketplace können endbenutzer vorab darüber informieren, was bereitgestellt werden kann und was nicht.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Was ist der Unterschied zwischen einem privaten Angebot und einem privaten Azure Marketplace?

Mit einem **privaten Angebot** können Herausgeber Pläne erstellen, die nur für Zielkunden sichtbar sind. Dadurch können sie benutzerdefinierte Lösungen mit ausgehandelten Preisen, privaten Geschäftsbedingungen und speziellen Konfigurationen privat freigeben. Weitere Informationen finden Sie unter [Private Angebote im kommerziellen Marketplace.](/azure/marketplace/private-offers)

**Mit privaten Azure Marketplace** im Azure-Portal können Administratoren vorab genehmigen, welche Drittanbieterlösungen ihre Benutzer bereitstellen können. Mit einem privaten Azure Marketplace können Benutzer die Vorteile der Azure Marketplace nutzen, indem sie konforme Angebote suchen, kaufen und bereitstellen. Zum Verwalten abonnementbasierter privater Angebote im privaten Marketplace muss der Marketplace-Administrator mindestens über die Rolle "Lesen" für das jeweilige Abonnement verfügen.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Ich habe dem privaten Azure Marketplace ein privates Angebot hinzugefügt. Warum wird es nicht auf der Registerkarte "Marketplace verwalten" angezeigt?

Abonnementbasierte private Angebote sind nur für die aufgelisteten Abonnements in den Einstellungen für private Angebote sichtbar. Um das private Angebot anzuzeigen, stellen Sie sicher, dass der globale Abonnementfilter alle Abonnements anzeigt.

[![Zeigt den Filter für den privaten Marketplace an.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Können benutzerdefinierte Images in private Azure Marketplace aufgenommen werden?

Nein. Private Azure Marketplace ermöglicht es jedem IT-Administrator, Lösungen von Drittanbietern aus globalen Azure Marketplace zu verwalten und zu cursieren. Da sich benutzerdefinierte Images nicht auf globalen Azure Marketplace befinden, kann der IT-Administrator Ihre benutzerdefinierten Images nicht auswählen und auswählen. Wenn Sie benutzerdefinierte Images freigeben möchten, verwenden Sie [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Schritt-für-Schritt-Anleitung Erstellen eines Shared Image Gallery (SIG) ([CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Erstellen Sie eine Imagedefinition innerhalb einer SIG. Der Kunde sollte **generalisiert** als Feld für den Betriebssystemzustand auswählen. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Verwaltetes Image in die Shared Image Gallery ([CLI,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell))
4. Die SIG-VM-Images befinden sich in einem Abonnement. Um sie für andere Abonnements verfügbar zu machen, verwenden Sie eine App-Registrierung ([CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Warum werden einige Angebote **standardmäßig genehmigt** angezeigt, obwohl der Herausgeber nicht Microsoft ist?

Microsoft unterstützt Linux- und Open-Source-Technologie in Azure. [Unterstützte Linux-Distributionen](/azure/virtual-machines/linux/endorsed-distros) werden in Azure unterstützt, und der Preis ist in virtuelle Computer integriert. Da der Azure Linux-Agent bereits auf Azure Marketplace vorinstalliert ist, wird er wie ein Microsoft-Angebot behandelt. Da Microsoft-Angebote standardmäßig genehmigt werden, können unterstützte Linux-Distributionen nicht in privaten Azure Marketplace verwaltet werden und sind standardmäßig genehmigt.

## <a name="contact-support"></a>Support kontaktieren

- Unterstützung für Azure Marketplace finden Sie unter [Microsoft Q&A](/answers/products/).