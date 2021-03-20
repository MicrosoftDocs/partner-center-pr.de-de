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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="d8737-104">Erstellen und Verwalten von privaten Azure Marketplace im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="d8737-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="d8737-105">Mit der privaten Azure Marketplace können Administratoren bestimmen, welche Lösungen von Drittanbietern Ihre Benutzer verwenden können.</span><span class="sxs-lookup"><span data-stu-id="d8737-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="d8737-106">Dies bewirkt, dass der Benutzer nur Angebote bereitstellen kann, die vom Administrator genehmigt werden und den Richtlinien Ihres Unternehmens entsprechen.</span><span class="sxs-lookup"><span data-stu-id="d8737-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="d8737-107">Mit dem privaten Azure Marketplace können Benutzer im Online Store nach kompatiblen angeboten zum Erwerb und Bereitstellen suchen.</span><span class="sxs-lookup"><span data-stu-id="d8737-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="d8737-108">Als Marketplace-Administrator (zugewiesene Rolle) beginnen Sie mit einem deaktivierten und leeren privaten Speicher, in dem Sie Ihre genehmigten Angebote und Pläne hinzufügen können.</span><span class="sxs-lookup"><span data-stu-id="d8737-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="d8737-109">In diesem Artikel wird erläutert, wie Sie die erforderliche Rolle zuweisen, einen privaten Speicher erstellen, Elemente verwalten, Benutzer Anforderungen genehmigen und private Azure Marketplace für Ihre Benutzer aktivieren.</span><span class="sxs-lookup"><span data-stu-id="d8737-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="d8737-110">Private Azure Marketplace befinden sich auf Mandanten Ebene, sodass allen Benutzern unter dem Mandanten dieselbe Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d8737-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="d8737-111">Alle Microsoft-Lösungen (einschließlich unterstütztes [Linux-Verteilungen](/azure/virtual-machines/linux/endorsed-distros)) werden automatisch privaten Azure Marketplace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8737-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="d8737-112">Zuweisen der Marketplace-Administrator Rolle</span><span class="sxs-lookup"><span data-stu-id="d8737-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="d8737-113">Der globale Administrator des Mandanten muss die **Marketplace-Administrator** Rolle dem privaten Azure Marketplace-Administrator zuweisen, der den privaten Speicher verwalten wird.</span><span class="sxs-lookup"><span data-stu-id="d8737-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d8737-114">Der Zugriff auf die private Azure Marketplace Verwaltung ist nur für IT-Administratoren mit zugewiesener Marketplace-Administrator Rolle verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d8737-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="d8737-115">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d8737-115">Prerequisites</span></span>

<span data-ttu-id="d8737-116">Diese Voraussetzungen sind erforderlich, bevor Sie die Marketplace-Administrator Rolle einem Benutzer im Mandanten Bereich zuweisen können:</span><span class="sxs-lookup"><span data-stu-id="d8737-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="d8737-117">Sie haben Zugriff auf einen **globalen Administrator** Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d8737-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="d8737-118">Der Mandant verfügt über mindestens ein Abonnement (kann ein beliebiger Typ sein).</span><span class="sxs-lookup"><span data-stu-id="d8737-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="d8737-119">Dem globalen Administrator Benutzer wird die Rolle " **Mitwirkender** " oder höher für das ausgewählte Abonnement zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="d8737-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="d8737-120">Zuweisen der Marketplace-Administrator Rolle mit Access Control (IAM)</span><span class="sxs-lookup"><span data-stu-id="d8737-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="d8737-121">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="d8737-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="d8737-122">Wählen Sie **alle Dienste** und dann **Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="d8737-123">Wählen Sie im Menü auf der linken Seite **privater Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="d8737-124">[![Zeigt die Menüoption für den privaten Marketplace auf der linken Seite des Marketplace an.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="d8737-125">Wählen Sie **Zugriffs Steuerung (IAM)** , um die Rolle Marketplace-Administrator zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="d8737-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zeigt den Bildschirm I A M Access Control an.":::

1. <span data-ttu-id="d8737-127">Wählen Sie **+Hinzufügen** > **Rollenzuweisung hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="d8737-128">Wählen Sie unter **Rolle** die Option **Marketplace-Administrator** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zeigt das Rollen Zuweisungs Menü an.":::

1. <span data-ttu-id="d8737-130">Wählen Sie in der Dropdown Liste den gewünschten Benutzer aus, und wählen Sie dann **abgeschlossen** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="d8737-131">Zuweisen der Marketplace-Administrator Rolle mithilfe von PowerShell</span><span class="sxs-lookup"><span data-stu-id="d8737-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="d8737-132">Verwenden Sie das folgende PowerShell-Skript, um die Marketplace-Administrator Rolle zuzuweisen. hierfür sind die folgenden Parameter erforderlich:</span><span class="sxs-lookup"><span data-stu-id="d8737-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="d8737-133">**Tenantid:** Die ID des Mandanten im Bereich (Marketplace-Administrator Rolle kann im Mandanten Bereich zugewiesen werden).</span><span class="sxs-lookup"><span data-stu-id="d8737-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="d8737-134">**Abonnement-ID:** Ein Abonnement, für das dem globalen Administrator die Rolle " **Mitwirkender** " oder höher zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="d8737-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="d8737-135">**Globaladminusername:** Der Benutzername des globalen Administrators.</span><span class="sxs-lookup"><span data-stu-id="d8737-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="d8737-136">**Usernametozuzuzutragrolefor:** Der Benutzername, dem die Marketplace-Administrator Rolle zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="d8737-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="d8737-137">Für Gastbenutzer, die an den Mandanten eingeladen wurden, kann es bis zu 48 Stunden dauern, bis Ihr Konto zum Zuweisen der Marketplace-Administrator Rolle verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="d8737-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="d8737-138">Weitere Informationen finden Sie unter [Eigenschaften eines Azure Active Directory B2B-Kollaborations Benutzers](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="d8737-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="d8737-139">Weitere Informationen zu den im AZ. Portal PowerShell-Modul enthaltenen Cmdlets finden Sie unter [Microsoft Azure PowerShell: Portal-Dashboard-Cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="d8737-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="d8737-140">Private Azure Marketplace erstellen</span><span class="sxs-lookup"><span data-stu-id="d8737-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="d8737-141">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="d8737-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="d8737-142">Wählen Sie **alle Dienste** und dann **Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zeigt das Azure-Portal Hauptfenster an.":::

3. <span data-ttu-id="d8737-144">Wählen Sie im Menü auf der linken Seite **privater Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="d8737-145">Wählen Sie " **starten** ", um eine private Azure Marketplace zu erstellen (Dies ist nur einmal erforderlich).</span><span class="sxs-lookup"><span data-stu-id="d8737-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Zeigt, wie das Hauptfenster &quot;get started on the Azure-Portal&quot; ausgewählt wird.":::

    <span data-ttu-id="d8737-147">Wenn für diesen Mandanten bereits private Azure Marketplace vorhanden sind, wird standardmäßig die Option " **Marketplace verwalten** " ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="d8737-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="d8737-148">Nach Abschluss des Vorgangs verfügen Sie über eine leere und deaktivierte private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d8737-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zeigt den leeren privaten Azure Marketplace Bildschirm an.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="d8737-150">Elemente aus Katalog hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d8737-150">Add items from gallery</span></span>

<span data-ttu-id="d8737-151">Ein Element ist eine Kombination aus einem Angebot und einem Plan.</span><span class="sxs-lookup"><span data-stu-id="d8737-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="d8737-152">Sie können auf der Seite Marketplace verwalten nach Elementen suchen und diese hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d8737-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="d8737-153">Wählen Sie **Elemente hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-153">Select **Add items**.</span></span>

2. <span data-ttu-id="d8737-154">Durchsuchen **Sie den Katalog, oder verwenden** Sie das Suchfeld, um das gewünschte Element zu finden.</span><span class="sxs-lookup"><span data-stu-id="d8737-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="d8737-155">[![Zeigt, wie Sie den Katalog durchsuchen oder das Suchfeld verwenden.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="d8737-156">Beim Hinzufügen eines neuen Angebots werden standardmäßig alle aktuellen Pläne der genehmigten Liste hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8737-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="d8737-157">Um die Plan Auswahl vor dem Hinzufügen der ausgewählten Elemente zu ändern, wählen Sie das Dropdown Menü in der Kachel des Angebots aus, und aktualisieren Sie die erforderlichen Pläne.</span><span class="sxs-lookup"><span data-stu-id="d8737-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Zeigt, wie die erforderlichen Pläne aktualisiert werden.":::

4. <span data-ttu-id="d8737-159">Klicken Sie unten links auf **Done (abgeschlossen** ), nachdem Sie Ihre Auswahl getroffen haben.</span><span class="sxs-lookup"><span data-stu-id="d8737-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="d8737-160">Das **Hinzufügen von Elementen** zum Marketplace ist nur für Angebote verfügbar, die nicht von Microsoft unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="d8737-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="d8737-161">Microsoft-Lösungen (einschließlich unterstützter [Linux-Verteilungen](/azure/virtual-machines/linux/endorsed-distros)) werden als "standardmäßig genehmigt" gekennzeichnet und können nicht im privaten Marketplace verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="d8737-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="d8737-162">Element Pläne bearbeiten</span><span class="sxs-lookup"><span data-stu-id="d8737-162">Edit item's plans</span></span>

<span data-ttu-id="d8737-163">Sie können die Pläne eines Elements auf der Seite "Marketplace verwalten" bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="d8737-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="d8737-164">Überprüfen Sie die verfügbaren Pläne in der Spalte **Pläne** im Dropdown Menü für dieses Element.</span><span class="sxs-lookup"><span data-stu-id="d8737-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="d8737-165">Aktivieren bzw. deaktivieren Sie die Kontrollkästchen, um auszuwählen, welche Pläne Ihren Benutzern zur Verfügung gestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d8737-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zeigt, wie das Kontrollkästchen für das erforderliche Element aktiviert oder deaktiviert wird.":::

> [!NOTE]
> <span data-ttu-id="d8737-167">Jedes Angebot benötigt mindestens einen Plan, der für das Update ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="d8737-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="d8737-168">Löschen Sie das gesamte Angebot (siehe nächster Abschnitt), um alle Pläne im Zusammenhang mit einem Angebot zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="d8737-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="d8737-169">Löschen von Angeboten</span><span class="sxs-lookup"><span data-stu-id="d8737-169">Delete offers</span></span>

<span data-ttu-id="d8737-170">Aktivieren Sie auf der Seite Marketplace verwalten das Kontrollkästchen neben dem Angebots Namen (siehe Bildschirm oben), und wählen Sie **Elemente löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="d8737-171">Private Azure Marketplace aktivieren/deaktivieren</span><span class="sxs-lookup"><span data-stu-id="d8737-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="d8737-172">Auf der Seite "Marketplace verwalten" finden Sie einen dieser Banner, der den aktuellen Status privater Azure Marketplace anzeigt:</span><span class="sxs-lookup"><span data-stu-id="d8737-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zeigt das Banner &quot;Zustand deaktivieren&quot; an.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zeigt das Banner &quot;Enable State&quot; an.":::

<span data-ttu-id="d8737-175">Sie können private Azure Marketplace nach Bedarf aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="d8737-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="d8737-176">Wenn diese Option deaktiviert ist, aktivieren Sie die Option **privaten Marketplace aktivieren** aktivieren.</span><span class="sxs-lookup"><span data-stu-id="d8737-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="d8737-177">Wenn diese Option aktiviert ist, wählen Sie den **privaten Marketplace deaktivieren** aus</span><span class="sxs-lookup"><span data-stu-id="d8737-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="d8737-178">Benachrichtigungs Center für private Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d8737-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="d8737-179">Das Benachrichtigungs Center besteht aus drei Arten von Benachrichtigungen und ermöglicht dem Marketplace-Administrator, basierend auf der Benachrichtigung Aktionen durchführen zu können:</span><span class="sxs-lookup"><span data-stu-id="d8737-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="d8737-180">Genehmigungsanforderungen von Benutzern für Elemente, die sich nicht in der genehmigten Liste befinden (siehe [Anforderung zum Hinzufügen von angeboten oder Plänen](#request-to-add-offers-or-plans) unten).</span><span class="sxs-lookup"><span data-stu-id="d8737-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="d8737-181">Neue Plan Benachrichtigungen für Angebote, die bereits über einen oder mehrere Pläne in der genehmigten Liste verfügen.</span><span class="sxs-lookup"><span data-stu-id="d8737-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="d8737-182">Die Plan Benachrichtigungen für Elemente, die sich in der genehmigten Liste befinden, aber aus der globalen Azure Marketplace entfernt wurden, wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="d8737-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="d8737-183">So greifen Sie auf das Benachrichtigungs Center zu:</span><span class="sxs-lookup"><span data-stu-id="d8737-183">To access the notification center:</span></span>

1. <span data-ttu-id="d8737-184">Wählen Sie im Menü auf der linken Seite die Option **Benachrichtigungen** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="d8737-185">[![Zeigt das Menü Benachrichtigungen an.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="d8737-186">Wählen Sie das Menü mit den Auslassungs Punkten für weitere Aktionen aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zeigt die Menü Ergebnisse der weiteren Optionen an.":::

1. <span data-ttu-id="d8737-188">Bei Plan Anforderungen wird durch **Anzeigen von Anforderungen** das Formular Genehmigungs Anforderung geöffnet, in dem Sie alle Benutzer Anforderungen für das jeweilige Angebot überprüfen können.</span><span class="sxs-lookup"><span data-stu-id="d8737-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="d8737-189">Wählen Sie **genehmigen** oder **ablehnen** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="d8737-190">[![Zeigt die Optionen "genehmigen" und "ablehnen" an.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="d8737-191">Wählen Sie im Dropdown Menü den Plan aus, der genehmigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8737-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="d8737-192">Fügen Sie einen Kommentar hinzu, und wählen Sie **senden** aus.</span><span class="sxs-lookup"><span data-stu-id="d8737-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="d8737-193">Private Azure Marketplace durchsuchen</span><span class="sxs-lookup"><span data-stu-id="d8737-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="d8737-194">Wenn private Azure Marketplace aktiviert ist, sehen Benutzer, welche Pläne der Marketplace-Administrator genehmigt hat.</span><span class="sxs-lookup"><span data-stu-id="d8737-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="d8737-195">Ein grünes **genehmigter** Hinweis gibt an, dass ein von ihnen genehmigtes Partner Angebot (nicht von Microsoft) genehmigt wird.</span><span class="sxs-lookup"><span data-stu-id="d8737-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="d8737-196">Ein blauer **genehmigter** Hinweis gibt an, dass ein Microsoft-Angebot (einschließlich unterstütztes [Linux-Verteilungen](/azure/virtual-machines/linux/endorsed-distros)) genehmigt ist.</span><span class="sxs-lookup"><span data-stu-id="d8737-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="d8737-197">Benutzer können zwischen angeboten filtern, die nicht genehmigt sind und nicht genehmigt sind:</span><span class="sxs-lookup"><span data-stu-id="d8737-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="d8737-198">[![Zeigt die Filteroption an.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="d8737-199">In privatem Azure Marketplace kaufen oder bereitstellen</span><span class="sxs-lookup"><span data-stu-id="d8737-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="d8737-200">Während die Produktdetailseite dem globalen Azure Marketplace ähnelt, gibt es drei private Azure Marketplace spezifische Szenarien.</span><span class="sxs-lookup"><span data-stu-id="d8737-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="d8737-201">Wenn ein Benutzer einen genehmigten Plan auswählt, wird die Schaltfläche " **Erstellen** " aktiviert:</span><span class="sxs-lookup"><span data-stu-id="d8737-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="d8737-202">[![Zeigt das Angebots Banner an, das anzeigt, dass ein Plan erstellt werden kann.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="d8737-203">Wenn eine Produkt Plan Auswahl nicht auf der Seite Produktdetails angezeigt wird, aber der Administrator einen oder mehrere Pläne genehmigt hat, wird in einem Banner festgestellt, welche Pläne genehmigt und die Schaltfläche **Erstellen** aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="d8737-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="d8737-204">[![Zeigt das Angebots Banner an, das darauf hinweist, dass ein Plan erstellt und verfügbare Pläne angezeigt werden kann.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="d8737-205">Wenn ein Benutzer einen nicht genehmigten Plan auswählt, wird in einem Banner der Plan als nicht genehmigt festgestellt, und die Schaltfläche **Erstellen** ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="d8737-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="d8737-206">Der Benutzer kann weiterhin anfordern, den Plan der genehmigten Liste hinzuzufügen (siehe nächster Abschnitt).</span><span class="sxs-lookup"><span data-stu-id="d8737-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="d8737-207">Anforderung zum Hinzufügen von angeboten oder Plänen</span><span class="sxs-lookup"><span data-stu-id="d8737-207">Request to add offers or plans</span></span>

<span data-ttu-id="d8737-208">Sie können anfordern, ein öffentliches Angebot oder einen Plan hinzuzufügen, der im privaten Azure Marketplace derzeit nicht genehmigt ist.</span><span class="sxs-lookup"><span data-stu-id="d8737-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="d8737-209">Wählen Sie **Anforderung zum Hinzufügen** im Banner aus, um das Formular für die **Zugriffs Anforderung** zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="d8737-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="d8737-210">[![Zeigt das Banner mit dem Link "Anforderung zum Hinzufügen" an.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="d8737-211">[![Zeigt das Zugriffs Anforderungs Formular für Angebote oder Pläne an.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="d8737-212">Wählen Sie aus, welche Pläne der Anforderung hinzugefügt werden sollen (**Jeder Plan** weist den Marketplace-Administrator an, dass Sie keinen Plan innerhalb eines Angebots bevorzugen).</span><span class="sxs-lookup"><span data-stu-id="d8737-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="d8737-213">Fügen Sie eine **Begründung** und eine **Anforderung** zum Übermitteln Ihrer Anforderung hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8737-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="d8737-214">[![Zeigt das Zugriffs Anforderungs Formular für Angebote oder Pläne mit Beispieleinträgen an.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="d8737-215">Eine Angabe für eine ausstehende Anforderung wird im Zugriffs Anforderungs Formular mit einer Option zum **zurückziehen der Anforderung** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d8737-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="d8737-216">[![Zeigt eine Liste mit genehmigten oder ausstehenden Plänen mit einem Link zum Widerrufen der Anforderung an.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="d8737-217">Nachdem die Anforderung gesendet wurde, wird das Genehmigungs Anforderungs Formular an das [Benachrichtigungs Center](#private-azure-marketplace-notification-center) für den Marketplace-Administrator gesendet, um die Anforderung zu überprüfen und Maßnahmen zu ergreifen.</span><span class="sxs-lookup"><span data-stu-id="d8737-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="d8737-218">Häufig gestellte Fragen (FAQs)</span><span class="sxs-lookup"><span data-stu-id="d8737-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="d8737-219">Ich blockiere die Marketplace-Drittanbieter Anwendung bereits über Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="d8737-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="d8737-220">Wie sieht das anders aus?</span><span class="sxs-lookup"><span data-stu-id="d8737-220">How is this different?</span></span>

<span data-ttu-id="d8737-221">Es gibt derzeit zwei Möglichkeiten, Dienste von Drittanbietern im Marketplace einzuschränken:</span><span class="sxs-lookup"><span data-stu-id="d8737-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="d8737-222">Deaktivieren Sie über das EA-Portal oder das Azure-Portal Dienste von Drittanbietern, oder beschränken Sie diese auf "kostenlose oder byol-SKUs".</span><span class="sxs-lookup"><span data-stu-id="d8737-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Zeigt, wie Dienste im Azure-Portal eingeschränkt werden.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Zeigt, wie Dienste im E-A-Portal eingeschränkt werden.":::

2. <span data-ttu-id="d8737-225">Erstellen Sie eine Azure-Richtlinie, um nur bestimmte VMS zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="d8737-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="d8737-226">Ausführliche Informationen zum Erzwingen von Richtlinien für virtuelle Windows-Computer finden Sie unter [Anwenden von Richtlinien auf Windows-VMS mit Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="d8737-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="d8737-227">Die private Azure Marketplace ermöglicht mehr Flexibilität bei der Einschränkung und bei der Ermöglichung spezifischer Angebote und Pläne.</span><span class="sxs-lookup"><span data-stu-id="d8737-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="d8737-228">Er informiert Endbenutzer über die Verfügbarkeit für die Bereitstellung im Marketplace-Katalog, auch wenn Sie versuchen, Drittanbieter Dienste bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="d8737-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="d8737-229">Um die Bereitstellung von Diensten von Drittanbietern zuzulassen, legen Sie im EA-Portal und im Azure-Portal Azure Marketplace auf ein/aktivieren fest.</span><span class="sxs-lookup"><span data-stu-id="d8737-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="d8737-230">Private Azure Marketplace können Partner Lösungen, die nicht auf virtuelle Computer beschränkt sind, mit anderen Werten</span><span class="sxs-lookup"><span data-stu-id="d8737-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="d8737-231">Private Azure Marketplace können auf Planebene einen Cursor einrichten und können auch "aktueller und zukünftiger Plan" festlegen.</span><span class="sxs-lookup"><span data-stu-id="d8737-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="d8737-232">Der private Azure Marketplace kann die Endbenutzer darüber informieren, was bereitgestellt werden kann und was nicht.</span><span class="sxs-lookup"><span data-stu-id="d8737-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="d8737-233">Worin besteht der Unterschied zwischen einem privaten Angebot und einem privaten Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="d8737-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="d8737-234">Ein **privates Angebot** ermöglicht Verlegern das Erstellen von Plänen, die nur für Zielkunden sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d8737-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="d8737-235">Dies ermöglicht es Ihnen, angepasste Lösungen privat mit ausgehandelten Preisen, privaten Geschäftsbedingungen und spezialisierten Konfigurationen gemeinsam zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="d8737-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="d8737-236">Weitere Informationen finden Sie unter [private Angebote im kommerziellen Marketplace](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="d8737-236">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="d8737-237">Mit dem **privaten Azure Marketplace** in der Azure-Portal können Administratoren vorab genehmigen, welche Lösungen von Drittanbietern Ihre Benutzer bereitstellen können.</span><span class="sxs-lookup"><span data-stu-id="d8737-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="d8737-238">Bei einer privaten Azure Marketplace können die Benutzer die Vorteile der Azure Marketplace nutzen, indem Sie kompatible Angebote finden, kaufen und bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="d8737-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="d8737-239">Zum Verwalten von Abonnement basierten privaten angeboten im privaten Marketplace muss der Marketplace-Administrator mindestens über die Rolle "lesen" für das jeweilige Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="d8737-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="d8737-240">Ich habe dem privaten Azure Marketplace ein privates Angebot hinzugefügt. Warum wird es nicht auf der Registerkarte "Marketplace verwalten" angezeigt?</span><span class="sxs-lookup"><span data-stu-id="d8737-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="d8737-241">Abonnement basierte private Angebote sind nur für die aufgeführten Abonnements in den Einstellungen des privaten Angebots sichtbar.</span><span class="sxs-lookup"><span data-stu-id="d8737-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="d8737-242">Um das private Angebot anzuzeigen, stellen Sie sicher, dass der globale Abonnement Filter alle Abonnements anzeigt.</span><span class="sxs-lookup"><span data-stu-id="d8737-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="d8737-243">[![Zeigt den privaten Marketplace-Filter an.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="d8737-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="d8737-244">Können wir benutzerdefinierte Images in private Azure Marketplace einschließen?</span><span class="sxs-lookup"><span data-stu-id="d8737-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="d8737-245">Nein.</span><span class="sxs-lookup"><span data-stu-id="d8737-245">No.</span></span> <span data-ttu-id="d8737-246">Die private Azure Marketplace ermöglicht IT-Administratoren, Lösungen von Drittanbietern von globalen Azure Marketplace zu verwalten und zu betreiben.</span><span class="sxs-lookup"><span data-stu-id="d8737-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="d8737-247">Da benutzerdefinierte Images sich nicht auf globalen Azure Marketplace befinden, kann der IT-Administrator die benutzerdefinierten Images nicht auswählen und auswählen.</span><span class="sxs-lookup"><span data-stu-id="d8737-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="d8737-248">Wenn Sie benutzerdefinierte Images freigeben möchten, verwenden Sie die frei [gegebene Image Galerie](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="d8737-248">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="d8737-249">Schritt-für-Schritt-Anleitung Erstellen eines freigegebenen Image Katalogs (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="d8737-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="d8737-250">Erstellen Sie eine Image Definition innerhalb von SIG.</span><span class="sxs-lookup"><span data-stu-id="d8737-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="d8737-251">Der Kunde sollte für das Feld "OS-State" **generalisiert** auswählen.</span><span class="sxs-lookup"><span data-stu-id="d8737-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="d8737-252">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="d8737-252">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="d8737-253">Bringen Sie ein verwaltetes Image in den freigegebenen Image Katalog ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="d8737-253">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="d8737-254">Die SIG-VM-Images befinden sich in einem Abonnement.</span><span class="sxs-lookup"><span data-stu-id="d8737-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="d8737-255">Verwenden Sie eine APP-Registrierung ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)), um Sie für andere Abonnements verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="d8737-255">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="d8737-256">Warum werden einige Angebote **standardmäßig genehmigt** , auch wenn der Verleger nicht Microsoft ist?</span><span class="sxs-lookup"><span data-stu-id="d8737-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="d8737-257">Microsoft unterstützt Linux-und Open-Source-Technologie in Azure.</span><span class="sxs-lookup"><span data-stu-id="d8737-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="d8737-258">Unterstützte [Linux-Distributionen](/azure/virtual-machines/linux/endorsed-distros) werden in Azure unterstützt, und der Preis ist in virtuelle Computer integriert.</span><span class="sxs-lookup"><span data-stu-id="d8737-258">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="d8737-259">Da der Azure Linux-Agent bereits auf Azure Marketplace vorinstalliert ist, wird er wie ein Microsoft-Angebot behandelt.</span><span class="sxs-lookup"><span data-stu-id="d8737-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="d8737-260">Da Microsoft-Angebote standardmäßig genehmigt werden, können unterstützte Linux-Distributionen nicht in privaten Azure Marketplace verwaltet werden und sind standardmäßig genehmigt.</span><span class="sxs-lookup"><span data-stu-id="d8737-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="d8737-261">Kontaktieren des Supports</span><span class="sxs-lookup"><span data-stu-id="d8737-261">Contact support</span></span>

- <span data-ttu-id="d8737-262">Azure Marketplace Unterstützung finden Sie unter [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="d8737-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>