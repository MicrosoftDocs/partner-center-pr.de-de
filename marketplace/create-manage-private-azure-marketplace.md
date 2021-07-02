---
title: Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal
description: Erfahren Sie mehr über das Erstellen und Verwalten von privaten Azure Marketplace (Vorschauversion) im Azure-Portal. Mit privatem Azure Marketplace (Vorschau) können Administratoren steuern, welche Drittanbieterlösungen ihre Benutzer verwenden können.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173702"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="f95ff-104">Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="f95ff-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="f95ff-105">Mit privatem Azure Marketplace können Administratoren steuern, welche Drittanbieterlösungen ihre Benutzer verwenden können.</span><span class="sxs-lookup"><span data-stu-id="f95ff-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="f95ff-106">Hierzu kann der Benutzer nur Angebote bereitstellen, die vom Administrator genehmigt wurden und den Richtlinien Ihres Unternehmens entsprechen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="f95ff-107">Mit privatem Azure Marketplace können Benutzer im Onlineshop nach kompatiblen Angeboten suchen, die erworben und bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="f95ff-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="f95ff-108">Als Marketplace-Administrator (zugewiesene Rolle) beginnen Sie mit einem deaktivierten und leeren privaten Store, in dem Sie Ihre genehmigten Angebote und Pläne hinzufügen können.</span><span class="sxs-lookup"><span data-stu-id="f95ff-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="f95ff-109">In diesem Artikel wird erläutert, wie Sie die erforderliche Rolle zuweisen, einen privaten Speicher erstellen, Elemente verwalten, Benutzeranforderungen genehmigen und private Azure Marketplace für Ihre Benutzer aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f95ff-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="f95ff-110">Private Azure Marketplace befindet sich auf Mandantenebene, sodass allen Benutzern unter dem Mandanten die gleiche zusammengestellte Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f95ff-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="f95ff-111">Alle Microsoft-Lösungen (einschließlich [unterstützter Linux-Distributionen)](/azure/virtual-machines/linux/endorsed-distros)werden automatisch privaten Azure Marketplace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f95ff-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="f95ff-112">Zuweisen der Marketplace-Administratorrolle</span><span class="sxs-lookup"><span data-stu-id="f95ff-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="f95ff-113">Der Globaler Administrator des Mandanten muss die **Marketplace-Administratorrolle** dem Privaten Azure Marketplace Administrator zuweisen, der den privaten Speicher verwaltet.</span><span class="sxs-lookup"><span data-stu-id="f95ff-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f95ff-114">Der Zugriff auf private Azure Marketplace-Verwaltung ist nur für IT-Administratoren verfügbar, deren Marketplace-Administratorrolle zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="f95ff-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="f95ff-115">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f95ff-115">Prerequisites</span></span>

<span data-ttu-id="f95ff-116">Diese Voraussetzungen sind erforderlich, bevor Sie einem Benutzer im Mandantenbereich die Rolle "Marketplace-Administrator" zuweisen können:</span><span class="sxs-lookup"><span data-stu-id="f95ff-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="f95ff-117">Sie haben Zugriff auf einen **globaler Administrator** Benutzer.</span><span class="sxs-lookup"><span data-stu-id="f95ff-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="f95ff-118">Der Mandant verfügt über mindestens ein Abonnement (kann ein beliebiger Typ sein).</span><span class="sxs-lookup"><span data-stu-id="f95ff-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="f95ff-119">Dem globaler Administrator Benutzer wird die Rolle **Mitwirkender** oder höher für das ausgewählte Abonnement zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="f95ff-120">Zuweisen der Marketplace-Administratorrolle mit Zugriffssteuerung (IAM)</span><span class="sxs-lookup"><span data-stu-id="f95ff-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="f95ff-121">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="f95ff-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="f95ff-122">Wählen Sie **Alle Dienste** und dann **Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="f95ff-123">Wählen  Sie im Menü auf der linken Seite Private Marketplace aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Zeigt die Menüoption &quot;Privater Marketplace&quot; auf der linken Seite des Marketplace an.":::

1. <span data-ttu-id="f95ff-125">Wählen Sie **Zugriffssteuerung (IAM)** aus, um die Marketplace-Administratorrolle zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zeigt den I A M-Bildschirm für die Zugriffssteuerung an.":::

1. <span data-ttu-id="f95ff-127">Wählen Sie **+Hinzufügen** > **Rollenzuweisung hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="f95ff-128">Wählen Sie unter **Rolle** die Option **Marketplace-Administrator** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zeigt das Menü Rollenzuweisung an.":::

1. <span data-ttu-id="f95ff-130">Wählen Sie in der Dropdownliste den gewünschten Benutzer und dann **Fertig** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="f95ff-131">Zuweisen der Marketplace-Administratorrolle mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="f95ff-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="f95ff-132">Verwenden Sie das folgende PowerShell-Skript, um die Rolle "Marketplace-Administrator" zuzuweisen. es sind die folgenden Parameter erforderlich:</span><span class="sxs-lookup"><span data-stu-id="f95ff-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="f95ff-133">**TenantId:** Die ID des Mandanten im Bereich (Die Marketplace-Administratorrolle kann für den Mandantenbereich zugewiesen werden).</span><span class="sxs-lookup"><span data-stu-id="f95ff-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="f95ff-134">**SubscriptionId:** Ein Abonnement, dem der globale Administrator die Rolle **Mitwirkender** oder höher zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="f95ff-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="f95ff-135">**GlobalAdminUsername:** Der Benutzername des globalen Administrators.</span><span class="sxs-lookup"><span data-stu-id="f95ff-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="f95ff-136">**UsernameToAssignRoleFor:** Der Benutzername, dem die Marketplace-Administratorrolle zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="f95ff-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="f95ff-137">Für Gastbenutzer, die zum Mandanten eingeladen werden, kann es bis zu 48 Stunden dauern, bis ihr Konto für die Zuweisung der Marketplace-Administratorrolle verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="f95ff-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="f95ff-138">Weitere Informationen finden Sie unter [Eigenschaften eines Azure Active Directory B2B-Zusammenarbeitsbenutzers.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="f95ff-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="f95ff-139">Weitere Informationen zu den Im PowerShell-Modul "Az.Portal" enthaltenen Cmdlets finden Sie unter [Microsoft Azure PowerShell: Portaldashboard-Cmdlets.](/powershell/module/az.portal/)</span><span class="sxs-lookup"><span data-stu-id="f95ff-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="f95ff-140">Erstellen eines privaten Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f95ff-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="f95ff-141">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="f95ff-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f95ff-142">Wählen Sie **Alle Dienste** und dann **Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zeigt das Azure-Portal Hauptfenster an.":::

3. <span data-ttu-id="f95ff-144">Wählen  Sie im Menü auf der linken Seite Private Marketplace aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="f95ff-145">Wählen Sie **Erste Schritte** aus, um private Azure Marketplace zu erstellen (sie müssen dies nur einmal tun).</span><span class="sxs-lookup"><span data-stu-id="f95ff-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Zeigt, wie Sie im Hauptfenster des Azure-Portal die Erste Schritte auswählen.":::

    <span data-ttu-id="f95ff-147">Wenn private Azure Marketplace für diesen Mandanten bereits vorhanden ist, wird Marketplace **verwalten** standardmäßig ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="f95ff-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="f95ff-148">Nach Abschluss des Abschlusses verfügen Sie über eine leere und deaktivierte private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f95ff-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zeigt den leeren Bildschirm private Azure Marketplace an.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="f95ff-150">Hinzufügen von Elementen aus dem Katalog</span><span class="sxs-lookup"><span data-stu-id="f95ff-150">Add items from gallery</span></span>

<span data-ttu-id="f95ff-151">Ein Element ist eine Kombination aus einem Angebot und einem Plan.</span><span class="sxs-lookup"><span data-stu-id="f95ff-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="f95ff-152">Sie können auf der Seite Marketplace verwalten nach Elementen suchen und elemente hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f95ff-153">Wählen Sie **Elemente hinzufügen aus.**</span><span class="sxs-lookup"><span data-stu-id="f95ff-153">Select **Add items**.</span></span>

2. <span data-ttu-id="f95ff-154">Durchsuchen Sie den **Katalog,** oder verwenden Sie das Suchfeld, um das gewünschte Element zu suchen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Zeigt, wie Sie den Katalog durchsuchen oder das Suchfeld verwenden.":::

3. <span data-ttu-id="f95ff-156">Standardmäßig werden beim Hinzufügen eines neuen Angebots alle aktuellen Pläne der genehmigten Liste hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f95ff-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="f95ff-157">Um die Planauswahl vor dem Hinzufügen der ausgewählten Elemente zu ändern, wählen Sie das Dropdownmenü auf der Kachel des Angebots aus, und aktualisieren Sie die erforderlichen Pläne.</span><span class="sxs-lookup"><span data-stu-id="f95ff-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Zeigt, wie erforderliche Pläne aktualisiert werden.":::

4. <span data-ttu-id="f95ff-159">Wählen Sie unten links **Fertig** aus, nachdem Sie Ihre Auswahl getroffen haben.</span><span class="sxs-lookup"><span data-stu-id="f95ff-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="f95ff-160">**Das Hinzufügen von Elementen** zum Marketplace ist nur für Nicht-Microsoft-Angebote verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f95ff-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="f95ff-161">Microsoft-Lösungen (einschließlich [unterstützter Linux-Distributionen)](/azure/virtual-machines/linux/endorsed-distros)werden als "Standardmäßig genehmigt" gekennzeichnet und können nicht im privaten Marketplace verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="f95ff-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="f95ff-162">Bearbeiten von Elementplänen</span><span class="sxs-lookup"><span data-stu-id="f95ff-162">Edit item's plans</span></span>

<span data-ttu-id="f95ff-163">Sie können die Pläne eines Elements auf der Seite Marketplace verwalten bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="f95ff-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f95ff-164">Überprüfen Sie in der Spalte **Pläne** die verfügbaren Pläne im Dropdownmenü für dieses Element.</span><span class="sxs-lookup"><span data-stu-id="f95ff-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="f95ff-165">Aktivieren oder deaktivieren Sie die Kontrollkästchen, um auszuwählen, welche Pläne Ihren Benutzern zur Verfügung gestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zeigt, wie sie das Kontrollkästchen für das erforderliche Element aktivieren oder deaktivieren.":::

   > [!NOTE]
   > <span data-ttu-id="f95ff-167">Für jedes Angebot muss mindestens ein Plan ausgewählt sein, damit das Update durchgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="f95ff-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="f95ff-168">Um alle Pläne im Zusammenhang mit einem Angebot zu entfernen, löschen Sie das gesamte Angebot (siehe nächster Abschnitt).</span><span class="sxs-lookup"><span data-stu-id="f95ff-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="f95ff-169">Löschen von Angeboten</span><span class="sxs-lookup"><span data-stu-id="f95ff-169">Delete offers</span></span>

<span data-ttu-id="f95ff-170">Aktivieren Sie auf der Seite Marketplace verwalten das Kontrollkästchen neben dem Angebotsnamen (siehe Bildschirm oben), und wählen Sie **Elemente löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="f95ff-171">Aktivieren/Deaktivieren von privaten Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f95ff-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="f95ff-172">Auf der Seite Marketplace verwalten sehen Sie eines dieser Banner, das den aktuellen Status von Private Azure Marketplace zeigt:</span><span class="sxs-lookup"><span data-stu-id="f95ff-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zeigt das Banner &quot;Status deaktivieren&quot; an.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zeigt das Banner &quot;Status aktivieren&quot; an.":::

<span data-ttu-id="f95ff-175">Sie können private Azure Marketplace nach Bedarf aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f95ff-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="f95ff-176">Wenn diese Option deaktiviert ist, wählen **Sie Privaten Marketplace** aktivieren aus, um dies zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f95ff-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="f95ff-177">Wenn diese Option aktiviert ist, wählen **Sie Privaten Marketplace** deaktivieren aus, um den Marketplace zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f95ff-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="f95ff-178">Private Azure Marketplace Notification Center</span><span class="sxs-lookup"><span data-stu-id="f95ff-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="f95ff-179">Notification Center besteht aus drei Arten von Benachrichtigungen und ermöglicht dem Marketplace-Administrator das Ausführen von Aktionen basierend auf der Benachrichtigung:</span><span class="sxs-lookup"><span data-stu-id="f95ff-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="f95ff-180">Genehmigungsanforderungen von Benutzern für Elemente, die nicht in der genehmigten Liste enthalten sind (siehe [Anforderung zum Hinzufügen von Angeboten oder Plänen](#request-to-add-offers-or-plans) weiter unten).</span><span class="sxs-lookup"><span data-stu-id="f95ff-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="f95ff-181">Neue Planbenachrichtigungen für Angebote, die bereits einen oder mehrere Pläne in der genehmigten Liste enthalten.</span><span class="sxs-lookup"><span data-stu-id="f95ff-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="f95ff-182">Planbenachrichtigungen für Elemente, die sich in der Genehmigten Liste befinden, aber aus der globalen Azure Marketplace entfernt wurden, wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="f95ff-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="f95ff-183">So greifen Sie auf die Mitteilungszentrale zu</span><span class="sxs-lookup"><span data-stu-id="f95ff-183">To access the notification center:</span></span>

1. <span data-ttu-id="f95ff-184">Wählen Sie im Menü auf der linken Seite die Option **Benachrichtigungen** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Zeigt das Menü Benachrichtigungen an.":::

1. <span data-ttu-id="f95ff-186">Wählen Sie das Menü mit den Auslassungszeichen aus, um weitere Aktionen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zeigt die Ergebnisse des Menüs Weitere Optionen an.":::

1. <span data-ttu-id="f95ff-188">Bei Plananforderungen wird unter Anforderungen anzeigen das Formular für **genehmigungsanforderung** geöffnet, in dem Sie alle Benutzeranforderungen für das jeweilige Angebot überprüfen können.</span><span class="sxs-lookup"><span data-stu-id="f95ff-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="f95ff-189">Wählen Sie **Genehmigen** oder **Ablehnen aus.**</span><span class="sxs-lookup"><span data-stu-id="f95ff-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Zeigt die Optionen zum Genehmigen und Ablehnen an.":::

1. <span data-ttu-id="f95ff-191">Wählen Sie im Dropdownmenü den zu genehmigenden Plan aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="f95ff-192">Fügen Sie einen Kommentar hinzu, und wählen **Sie Senden** aus.</span><span class="sxs-lookup"><span data-stu-id="f95ff-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="f95ff-193">Durchsuchen privater Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f95ff-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="f95ff-194">Wenn private Azure Marketplace aktiviert ist, sehen Benutzer, welche Pläne der Marketplace-Administrator genehmigt hat.</span><span class="sxs-lookup"><span data-stu-id="f95ff-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="f95ff-195">Ein grünes **Genehmigtes** Benachrichtigungsmerkmal zeigt ein Partnerangebot (nicht von Microsoft) an, das genehmigt wurde.</span><span class="sxs-lookup"><span data-stu-id="f95ff-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="f95ff-196">Ein blauer **Genehmigter** Hinweis weist auf ein Microsoft-Angebot (einschließlich [unterstützter Linux-Distributionen)](/azure/virtual-machines/linux/endorsed-distros)hin, das genehmigt wurde.</span><span class="sxs-lookup"><span data-stu-id="f95ff-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="f95ff-197">Benutzer können zwischen Angeboten filtern, die genehmigt sind und nicht genehmigt sind:</span><span class="sxs-lookup"><span data-stu-id="f95ff-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Zeigt die Filteroption an.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="f95ff-199">Kaufen oder Bereitstellen in privatem Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f95ff-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="f95ff-200">Die Seite mit den Produktdetails ähnelt der globalen Azure Marketplace, es gibt jedoch drei private Azure Marketplace spezifischen Szenarien.</span><span class="sxs-lookup"><span data-stu-id="f95ff-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="f95ff-201">Wenn ein Benutzer einen genehmigten Plan auswählt, wird die **Schaltfläche** Erstellen aktiviert:</span><span class="sxs-lookup"><span data-stu-id="f95ff-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Zeigt das Angebotsbanner an, auf dem sie angezeigt wird, dass ein Plan erstellt werden kann.":::

- <span data-ttu-id="f95ff-203">Wenn eine Produktplanauswahl nicht auf der Produktdetailseseite angezeigt wird, der Administrator jedoch einen  oder mehrere Pläne genehmigt hat, wird auf einem Banner angezeigt, welche Pläne genehmigt und die Schaltfläche Erstellen aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="f95ff-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Zeigt das Angebotsbanner an, das darauf hindellt, dass ein Plan erstellt werden kann und verfügbare Pläne angezeigt werden.":::

- <span data-ttu-id="f95ff-205">Wenn ein Benutzer einen nicht genehmigten Plan auswählt, wird der Plan in einem Banner als nicht genehmigt angezeigt, und die **Schaltfläche** Erstellen ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="f95ff-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="f95ff-206">Der Benutzer kann weiterhin anfordern, den Plan der Genehmigten Liste hinzuzufügen (siehe nächster Abschnitt).</span><span class="sxs-lookup"><span data-stu-id="f95ff-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="f95ff-207">Anforderung zum Hinzufügen von Angeboten oder Plänen</span><span class="sxs-lookup"><span data-stu-id="f95ff-207">Request to add offers or plans</span></span>

<span data-ttu-id="f95ff-208">Sie können anfordern, ein öffentliches Angebot oder einen Plan hinzuzufügen, der bzw. der derzeit nicht in der privaten Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f95ff-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="f95ff-209">Wählen **Sie Anforderung aus, um** im Banner hinzuzufügen, um das Formular **Zugriffsanforderung zu öffnen.**</span><span class="sxs-lookup"><span data-stu-id="f95ff-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Zeigt das Banner mit dem Link &quot;Anforderung zum Hinzufügen&quot; an.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Zeigt das Formular für Die Zugriffsanforderung für Angebote oder Pläne an.":::

1. <span data-ttu-id="f95ff-212">Wählen Sie aus, welche Pläne der Anforderung hinzugefügt werden sollen (**Jeder** Plan teilt dem Marketplace-Administrator mit, dass Sie keinen Plan innerhalb eines Angebots bevorzugen).</span><span class="sxs-lookup"><span data-stu-id="f95ff-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="f95ff-213">Fügen Sie eine **Begründung hinzu,** und wählen **Sie Anforderung aus,** um Ihre Anforderung zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="f95ff-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Zeigt das Formular für Zugriffsanforderungen für Angebote oder Pläne mit Beispieleinträgen an.":::

1. <span data-ttu-id="f95ff-215">Ein Hinweis auf eine ausstehende Anforderung wird im Formular Zugriffsanforderung mit der Option Anforderung widerrufen **angezeigt.**</span><span class="sxs-lookup"><span data-stu-id="f95ff-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Zeigt eine Liste mit genehmigten oder ausstehenden Plänen mit dem Link &quot;Anforderung widerrufen&quot; an.":::

> [!NOTE]
> <span data-ttu-id="f95ff-217">Nach dem Senden wird das Genehmigungsanforderungsformular an die [Mitteilungszentrale](#private-azure-marketplace-notification-center) gesendet, damit der Marketplace-Administrator die Anforderung überprüfen und Maßnahmen ergreifen kann.</span><span class="sxs-lookup"><span data-stu-id="f95ff-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="f95ff-218">Die Genehmigung im privaten Marketplace gibt keine Beschaffung einer Lösung an.</span><span class="sxs-lookup"><span data-stu-id="f95ff-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="f95ff-219">Häufig gestellte Fragen (FAQs)</span><span class="sxs-lookup"><span data-stu-id="f95ff-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="f95ff-220">Ich blockiere bereits Marketplace-Drittanbieteranwendung über Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="f95ff-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="f95ff-221">Wie ist das anders?</span><span class="sxs-lookup"><span data-stu-id="f95ff-221">How is this different?</span></span>

<span data-ttu-id="f95ff-222">Es gibt derzeit zwei Möglichkeiten, Drittanbieterdienste im Marketplace einzuschränken:</span><span class="sxs-lookup"><span data-stu-id="f95ff-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="f95ff-223">Deaktivieren Sie über das EA-Portal oder Azure-Portal Dienste von Drittanbietern, oder beschränken Sie sie auf "Nur Free- oder BYOL-SKUs".</span><span class="sxs-lookup"><span data-stu-id="f95ff-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Zeigt, wie Dienste in der -Azure-Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Zeigt, wie Dienste im E A-Portal beschränkt werden.":::

2. <span data-ttu-id="f95ff-226">Erstellen Sie eine Azure-Richtlinie, um nur bestimmte VMs zu erlauben.</span><span class="sxs-lookup"><span data-stu-id="f95ff-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="f95ff-227">Weitere Informationen zum Erzwingen von Richtlinien für Windows VMs finden Sie unter Anwenden von Richtlinien auf Windows [VMs mit Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="f95ff-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="f95ff-228">Private Azure Marketplace ermöglicht mehr Flexibilität beim Einschränken und Zulassen bestimmter Angebote und Pläne.</span><span class="sxs-lookup"><span data-stu-id="f95ff-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="f95ff-229">Endbenutzer werden über die Verfügbarkeit für die Bereitstellung im Marketplace-Katalog informiert, noch bevor sie versuchen, Dienste von Drittanbietern bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="f95ff-230">Um die Bereitstellung von Diensten von Drittanbietern zu ermöglichen, legen Sie Azure Marketplace in der EA Portal auf Ein/Aktiviert fest, und Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="f95ff-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="f95ff-231">Private Azure Marketplace können Partnerlösungen zusammengestellt werden, die nicht auf virtuelle Computer beschränkt sind.</span><span class="sxs-lookup"><span data-stu-id="f95ff-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="f95ff-232">Private Azure Marketplace können auf Planebene zusammengestellt werden und auch "Aktueller und zukünftiger Plan" festlegen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="f95ff-233">Private Azure Marketplace können die Endbenutzer im Vor-/Nach-Vor-Ort darüber informieren, was bereitgestellt werden kann und was nicht.</span><span class="sxs-lookup"><span data-stu-id="f95ff-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="f95ff-234">Worin besteht der Unterschied zwischen einem privaten Angebot und einem Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="f95ff-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="f95ff-235">Mit **einem privaten Angebot** können Herausgeber Pläne erstellen, die nur für Zielkunden sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="f95ff-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="f95ff-236">Auf diese Weise können sie angepasste Lösungen privat mit ausgehandelten Preisen, privaten Geschäftsbedingungen und speziellen Konfigurationen teilen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="f95ff-237">Weitere Informationen finden Sie unter [Private Angebote im kommerziellen Marketplace.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="f95ff-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="f95ff-238">**Private Azure Marketplace** im Azure-Portal können Administratoren vorab genehmigen, welche Drittanbieterlösungen ihre Benutzer bereitstellen können.</span><span class="sxs-lookup"><span data-stu-id="f95ff-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="f95ff-239">Mit einem privaten Azure Marketplace können Benutzer die Vorteile der Azure Marketplace, indem sie konforme Angebote finden, kaufen und bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="f95ff-240">Zum Verwalten abonnementbasierter privater Angebote im privaten Marketplace muss der Marketplace-Administrator mindestens über die Rolle "Lesen" für das spezifische Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="f95ff-241">Ich habe dem Private Azure Marketplace ein privates Angebot hinzugefügt. Warum wird es nicht auf der Registerkarte "Marketplace verwalten" angezeigt?</span><span class="sxs-lookup"><span data-stu-id="f95ff-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="f95ff-242">Abonnementbasierte private Angebote sind nur für die aufgelisteten Abonnements in den Einstellungen für private Angebote sichtbar.</span><span class="sxs-lookup"><span data-stu-id="f95ff-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="f95ff-243">Stellen Sie zum Anzeigen des privaten Angebots sicher, dass im globalen Abonnementfilter alle Abonnements angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f95ff-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Zeigt den Filter für den privaten Marketplace an.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="f95ff-245">Können benutzerdefinierte Images in private Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="f95ff-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="f95ff-246">Nein.</span><span class="sxs-lookup"><span data-stu-id="f95ff-246">No.</span></span> <span data-ttu-id="f95ff-247">Private Azure Marketplace ermöglicht jedem IT-Administrator das Verwalten und Zusammengestellt von Drittanbieterlösungen von globalen Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f95ff-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="f95ff-248">Da benutzerdefinierte Images nicht auf globalen Azure Marketplace sind, kann der IT-Administrator Ihre benutzerdefinierten Images nicht auswählen und auswählen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="f95ff-249">Wenn Sie benutzerdefinierte Images freigeben möchten, verwenden Sie [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="f95ff-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="f95ff-250">Schritt-für-Schritt-Anleitung: Erstellen eines Shared Image Gallery (SIG) ([CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="f95ff-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="f95ff-251">Erstellen Sie eine Imagedefinition innerhalb einer SIG.</span><span class="sxs-lookup"><span data-stu-id="f95ff-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="f95ff-252">Der Kunde sollte **generalisiert für** das Feld Betriebssystemstatus auswählen.</span><span class="sxs-lookup"><span data-stu-id="f95ff-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="f95ff-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="f95ff-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="f95ff-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="f95ff-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="f95ff-255">Die SIG-VM-Images befinden sich in einem Abonnement.</span><span class="sxs-lookup"><span data-stu-id="f95ff-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="f95ff-256">Um sie für andere Abonnements verfügbar zu machen, verwenden Sie eine App-Registrierung ([CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="f95ff-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="f95ff-257">Warum werden einige Angebote standardmäßig genehmigt **angezeigt,** obwohl der Herausgeber nicht Microsoft ist?</span><span class="sxs-lookup"><span data-stu-id="f95ff-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="f95ff-258">Microsoft unterstützt Linux- und Open-Source-Technologie in Azure.</span><span class="sxs-lookup"><span data-stu-id="f95ff-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="f95ff-259">[Unterstützte Linux-Distributionen](/azure/virtual-machines/linux/endorsed-distros) werden in Azure unterstützt, und der Preis ist in virtuelle Computer integriert.</span><span class="sxs-lookup"><span data-stu-id="f95ff-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="f95ff-260">Da der Azure Linux-Agent bereits auf der Azure Marketplace vorinstalliert ist, wird er wie ein Microsoft-Angebot behandelt.</span><span class="sxs-lookup"><span data-stu-id="f95ff-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="f95ff-261">Da Microsoft-Angebote standardmäßig genehmigt sind, können unterstützte Linux-Distributionen nicht in Private Azure Marketplace verwaltet und standardmäßig genehmigt werden.</span><span class="sxs-lookup"><span data-stu-id="f95ff-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="f95ff-262">Support kontaktieren</span><span class="sxs-lookup"><span data-stu-id="f95ff-262">Contact support</span></span>

- <span data-ttu-id="f95ff-263">Weitere Azure Marketplace sie unter [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="f95ff-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>