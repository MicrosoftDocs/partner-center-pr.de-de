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
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="46091-103">Erstellen und Verwalten von privaten Azure Marketplace (Vorschau) im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="46091-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="46091-104">Mit der privaten Azure Marketplace (Vorschauversion) können Administratoren steuern, welche Lösungen von Drittanbietern Ihre Benutzer verwenden können.</span><span class="sxs-lookup"><span data-stu-id="46091-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="46091-105">Dies ermöglicht es Ihnen, nur Angebote bereitzustellen, die Sie genehmigen und die den Richtlinien Ihres Unternehmens entsprechen.</span><span class="sxs-lookup"><span data-stu-id="46091-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="46091-106">Mit dem privaten Azure Marketplace können Ihre Benutzer im Online Store nach kompatiblen angeboten zum Erwerb und Bereitstellen suchen.</span><span class="sxs-lookup"><span data-stu-id="46091-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="46091-107">Als Marketplace-Administrator (zugewiesene Rolle) beginnen Sie mit einem deaktivierten und leeren privaten Speicher, in dem Sie Ihre genehmigten Angebote und Pläne hinzufügen können.</span><span class="sxs-lookup"><span data-stu-id="46091-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="46091-108">In diesem Artikel wird erläutert, wie Sie private Azure Marketplace für Ihre Benutzer erstellen, verwalten und aktivieren.</span><span class="sxs-lookup"><span data-stu-id="46091-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="46091-109">Hinweise:</span><span class="sxs-lookup"><span data-stu-id="46091-109">Notes:</span></span>

- <span data-ttu-id="46091-110">Private Azure Marketplace befinden sich auf Mandanten Ebene, sodass allen Benutzern unter dem Mandanten dieselbe Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="46091-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="46091-111">Alle Microsoft-Lösungen werden automatisch privaten Azure Marketplace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="46091-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="46091-112">Zuweisen der Marketplace-Administrator Rolle</span><span class="sxs-lookup"><span data-stu-id="46091-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="46091-113">Der globale Administrator des Mandanten muss die **Marketplace-Administrator** Rolle dem privaten Azure Marketplace-Administrator zuweisen, der den privaten Speicher verwalten wird.</span><span class="sxs-lookup"><span data-stu-id="46091-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="46091-114">Der Zugriff auf die private Azure Marketplace Verwaltung ist nur für IT-Administratoren mit zugewiesener Marketplace-Administrator Rolle verfügbar.</span><span class="sxs-lookup"><span data-stu-id="46091-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="46091-115">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46091-115">Prerequisites</span></span>

<span data-ttu-id="46091-116">Sie müssen diese Voraussetzungen erfüllen, bevor Sie die Marketplace-Administrator Rolle einem Benutzer im Mandanten Bereich zuweisen können:</span><span class="sxs-lookup"><span data-stu-id="46091-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="46091-117">Sie haben Zugriff auf einen **globalen Administrator** Benutzer.</span><span class="sxs-lookup"><span data-stu-id="46091-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="46091-118">Der Mandant verfügt über mindestens ein Abonnement (kann ein beliebiger Typ sein).</span><span class="sxs-lookup"><span data-stu-id="46091-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="46091-119">Dem globalen Administrator Benutzer wird die Rolle " **Mitwirkender** " oder höher für das Abonnement zugewiesen, das Sie in Schritt 2 ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="46091-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="46091-120">Für den Benutzer des globalen Administrators ist der Zugriff auf **Ja** festgelegt (siehe [Elevate-Access-Global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="46091-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="46091-121">Zuweisen der Marketplace-Administrator Rolle mithilfe von PowerShell</span><span class="sxs-lookup"><span data-stu-id="46091-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="46091-122">Verwenden Sie das folgende PowerShell-Skript, um die Marketplace-Administrator Rolle zuzuweisen. hierfür sind die folgenden Parameter erforderlich:</span><span class="sxs-lookup"><span data-stu-id="46091-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="46091-123">**Tenantid:** Die ID des Mandanten im Bereich (Marketplace-Administrator Rolle kann im Mandanten Bereich zugewiesen werden).</span><span class="sxs-lookup"><span data-stu-id="46091-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="46091-124">**Abonnement-ID:** Ein Abonnement, für das dem globalen Administrator die Rolle " **Mitwirkender** " oder höher zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="46091-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="46091-125">**Globaladminusername:** Der Benutzername des globalen Administrators.</span><span class="sxs-lookup"><span data-stu-id="46091-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="46091-126">**Usernametozuzuzutragrolefor:** Der Benutzername, dem die Marketplace-Administrator Rolle zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="46091-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="46091-127">Für Gastbenutzer, die an den Mandanten eingeladen wurden, kann es bis zu 48 Stunden dauern, bis Ihr Konto zum Zuweisen der Marketplace-Administrator Rolle verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="46091-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="46091-128">Weitere Informationen finden Sie unter [Eigenschaften eines Azure Active Directory B2B-Kollaborations Benutzers](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="46091-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="46091-129">Weitere Informationen zu den im AZ. Portal PowerShell-Modul enthaltenen Cmdlets finden Sie unter [Microsoft Azure PowerShell: Portal-Dashboard-Cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="46091-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="46091-130">Private Azure Marketplace erstellen</span><span class="sxs-lookup"><span data-stu-id="46091-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="46091-131">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="46091-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="46091-132">Wählen Sie **alle Dienste** und dann **Marketplace** aus.</span><span class="sxs-lookup"><span data-stu-id="46091-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure-Portal Hauptfenster.":::

3. <span data-ttu-id="46091-134">Wählen Sie den **privaten Marketplace** aus den Optionen auf der linken Seite aus.</span><span class="sxs-lookup"><span data-stu-id="46091-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Wählen Sie im Hauptfenster des Azure-Portal den privaten Marketplace aus.":::

4. <span data-ttu-id="46091-136">Wählen Sie " **starten** ", um eine private Azure Marketplace zu erstellen (Dies ist nur einmal erforderlich).</span><span class="sxs-lookup"><span data-stu-id="46091-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Klicken Sie im Azure-Portal Hauptfenster auf _OL_QUOTE_PLACEHOLDER_starten_OL_QUOTE_PLACEHOLDER_.":::

    <span data-ttu-id="46091-138">Wenn für diesen Mandanten bereits private Azure Marketplace vorhanden sind, wird standardmäßig die Option " **Marketplace verwalten** " ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="46091-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="46091-139">Nach Abschluss des Vorgangs verfügen Sie über eine leere und deaktivierte private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="46091-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Der leere private Azure Marketplace Bildschirm.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="46091-141">Elemente aus Katalog hinzufügen</span><span class="sxs-lookup"><span data-stu-id="46091-141">Add items from gallery</span></span>

<span data-ttu-id="46091-142">Ein Element ist eine Kombination aus einem Angebot und einem Plan.</span><span class="sxs-lookup"><span data-stu-id="46091-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="46091-143">Sie können auf der Seite Marketplace verwalten nach Elementen suchen und Elemente hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="46091-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="46091-144">Wählen Sie **Elemente hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="46091-144">Select **Add items**.</span></span>

2. <span data-ttu-id="46091-145">Durchsuchen **Sie den Katalog, oder verwenden** Sie das Suchfeld, um das gewünschte Element zu finden.</span><span class="sxs-lookup"><span data-stu-id="46091-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Durchsuchen des Katalogs oder Verwenden des Suchfelds.":::

3. <span data-ttu-id="46091-147">Beim Hinzufügen eines neuen Angebots werden standardmäßig alle aktuellen Pläne der Zulassungsliste hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="46091-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="46091-148">Um die Plan Auswahl vor dem Hinzufügen der ausgewählten Elemente zu ändern, wählen Sie das Dropdown Menü in der Kachel des Angebots aus, und aktualisieren Sie die erforderlichen Pläne.</span><span class="sxs-lookup"><span data-stu-id="46091-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualisieren Sie die erforderlichen Pläne.":::

4. <span data-ttu-id="46091-150">Klicken Sie unten links auf **Done (abgeschlossen** ), nachdem Sie Ihre Auswahl getroffen haben.</span><span class="sxs-lookup"><span data-stu-id="46091-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="46091-151">Das **Hinzufügen von Elementen** zum Marketplace ist nur für Angebote verfügbar, die nicht von Microsoft unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="46091-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="46091-152">Microsoft-Angebote sind standardmäßig zulässig.</span><span class="sxs-lookup"><span data-stu-id="46091-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="46091-153">Element Pläne bearbeiten</span><span class="sxs-lookup"><span data-stu-id="46091-153">Edit item plans</span></span>

<span data-ttu-id="46091-154">Sie können die Pläne eines Elements auf der Seite "Marketplace verwalten" bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="46091-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="46091-155">Überprüfen Sie die verfügbaren Pläne in der Spalte **Pläne** im Dropdown Menü für dieses Element.</span><span class="sxs-lookup"><span data-stu-id="46091-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="46091-156">Aktivieren bzw. deaktivieren Sie die Kontrollkästchen, um auszuwählen, welche Pläne Ihren Benutzern zur Verfügung gestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="46091-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Aktivieren oder Deaktivieren des Kontrollkästchens für das erforderliche Element":::

> [!NOTE]
> <span data-ttu-id="46091-158">Für jedes Angebot muss mindestens ein Plan ausgewählt sein, damit das Update ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="46091-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="46091-159">Löschen Sie das gesamte Angebot (siehe nächster Abschnitt), um alle Pläne im Zusammenhang mit einem Angebot zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="46091-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="46091-160">Löschen von Angeboten</span><span class="sxs-lookup"><span data-stu-id="46091-160">Delete offers</span></span>

<span data-ttu-id="46091-161">Aktivieren Sie auf der Seite Marketplace verwalten das Kontrollkästchen neben dem Angebots Namen (siehe Bildschirm oben), und wählen Sie **Elemente löschen** aus.</span><span class="sxs-lookup"><span data-stu-id="46091-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="46091-162">Private Azure Marketplace aktivieren/deaktivieren</span><span class="sxs-lookup"><span data-stu-id="46091-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="46091-163">Auf der Seite "Marketplace verwalten" finden Sie einen dieser Banner, der den aktuellen Status privater Azure Marketplace anzeigt:</span><span class="sxs-lookup"><span data-stu-id="46091-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zustands Banner deaktivieren":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Status Banner aktivieren":::

<span data-ttu-id="46091-166">Sie können private Azure Marketplace nach Bedarf aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="46091-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="46091-167">Wenn diese Option deaktiviert ist, aktivieren Sie die Option **privaten Marketplace aktivieren** aktivieren.</span><span class="sxs-lookup"><span data-stu-id="46091-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="46091-168">Wenn diese Option aktiviert ist, wählen Sie den **privaten Marketplace deaktivieren** aus</span><span class="sxs-lookup"><span data-stu-id="46091-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="46091-169">Private Azure Marketplace durchsuchen</span><span class="sxs-lookup"><span data-stu-id="46091-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="46091-170">Wenn private Azure Marketplace aktiviert ist, wird Benutzern angezeigt, welche Pläne der Marketplace-Administrator zugelassen hat.</span><span class="sxs-lookup"><span data-stu-id="46091-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="46091-171">Ein grüner **Allowed** zulässiger Hinweis gibt an, dass es sich um ein Angebot eines Partners (nicht-Microsoft) handelt.</span><span class="sxs-lookup"><span data-stu-id="46091-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="46091-172">Ein blauer **Allowed** zulässiger Hinweis gibt ein zulässiges Microsoft-Angebot an.</span><span class="sxs-lookup"><span data-stu-id="46091-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="46091-173">Benutzer können zwischen angeboten filtern, die nicht zulässig sind und nicht zulässig sind:</span><span class="sxs-lookup"><span data-stu-id="46091-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filteroption.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="46091-175">In privatem Azure Marketplace kaufen oder bereitstellen</span><span class="sxs-lookup"><span data-stu-id="46091-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="46091-176">Während die Produktdetailseite dem öffentlichen Azure Marketplace ähnelt, gibt es drei private Azure Marketplace spezifische Szenarien.</span><span class="sxs-lookup"><span data-stu-id="46091-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="46091-177">Wenn ein Benutzer einen zulässigen Plan auswählt, wird die Schaltfläche **Erstellen** aktiviert:</span><span class="sxs-lookup"><span data-stu-id="46091-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Angebots Banner mit dem Hinweis, dass ein Plan erstellt werden kann.":::

- <span data-ttu-id="46091-179">Wenn ein Benutzer einen nicht zulässigen Plan auswählt, wird in einem Banner darauf hingewiesen, dass der Plan nicht zulässig ist und die Schaltfläche **Erstellen** deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="46091-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Angebots Banner mit einem Plan können nicht erstellt werden.":::

- <span data-ttu-id="46091-181">Wenn eine Produkt Plan Auswahl nicht auf der Seite Produktdetails angezeigt wird, aber der Administrator einen oder mehrere Pläne genehmigt hat, wird in einem Banner festgestellt, welche Pläne zulässig sind und wie die Schaltfläche **Erstellen** aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="46091-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Angebots Banner mit dem Hinweis, dass ein Plan erstellt und verfügbare Pläne angezeigt werden können.":::

## <a name="contact-support"></a><span data-ttu-id="46091-183">Kontaktieren Sie den Support.</span><span class="sxs-lookup"><span data-stu-id="46091-183">Contact support</span></span>

<span data-ttu-id="46091-184">Azure Marketplace Unterstützung finden Sie unter [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="46091-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
