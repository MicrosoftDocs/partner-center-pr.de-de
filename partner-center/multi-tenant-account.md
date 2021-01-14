---
title: Fügen Sie Ihrem Partner Center-Konto weitere Mandanten hinzu.
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie mehrere Azure AD Mandanten in Ihrem Partner Center-Konto hinzufügen, konsolidieren oder verwalten. Informieren Sie sich auch über einige der Gründe, die Sie möglicherweise tun möchten.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182431"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="2261c-104">Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="2261c-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="2261c-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="2261c-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2261c-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2261c-106">Global admin</span></span>
- <span data-ttu-id="2261c-107">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="2261c-107">Account admin</span></span>

<span data-ttu-id="2261c-108">Mit diesem Feature können Sie mehrere Mandanten für Ihr Unternehmen verwalten und sie in Ihrem Partner Center-Konto konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="2261c-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="2261c-109">Es gibt viele Gründe, warum Sie möglicherweise mehrere Azure AD Mandanten in Ihrem Partner Center-Konto verwalten müssen.</span><span class="sxs-lookup"><span data-stu-id="2261c-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="2261c-110">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="2261c-110">For example:</span></span>

- <span data-ttu-id="2261c-111">Ihr Unternehmen kann ein anderes Unternehmen erwerben und möchten, dass die Mitarbeiter des neuen Unternehmens Partner Center verwenden können.</span><span class="sxs-lookup"><span data-stu-id="2261c-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="2261c-112">Sie möchten jedoch, dass die beiden Unternehmen getrennt bleiben.</span><span class="sxs-lookup"><span data-stu-id="2261c-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="2261c-113">In diesem Fall würden Sie den Azure AD Mandanten des neuen Unternehmens mit ihrem globalen Partner Konto (PGA) verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="2261c-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="2261c-114">Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="2261c-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="2261c-115">Wenn Sie über mehr als einen Mandanten verfügen, um Ihr Unternehmen auszuführen (z. b. contoso.com, contoso.uk, contoso.in), können Sie die mehr Instanzen Fähigkeit verwenden, um Sie mit dem gleichen PC-Konto zu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="2261c-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="2261c-116">Bei Fusionen und Übernahmen müssen Sie mit mehr als einem Mandanten arbeiten (Wenn Contoso beispielsweise Fabrikam übernimmt), müssen Sie in der Lage sein, sowohl constoso.com als auch fabrikam.com entsprechende Mandanten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="2261c-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="2261c-117">Benutzer von einem der Mandanten müssen folgende Aktionen ausführen können:</span><span class="sxs-lookup"><span data-stu-id="2261c-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="2261c-118">Access Partner Center für Schulungen, digitale Downloads, MCP-Zuordnung</span><span class="sxs-lookup"><span data-stu-id="2261c-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="2261c-119">Ihnen werden Partner Center-Rollen wie MPN admin, Incentive admin usw. zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="2261c-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="2261c-120">Fügen Sie Ihrem Konto einen weiteren Azure AD Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="2261c-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="2261c-121">Melden Sie sich als globaler Administrator beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="2261c-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="2261c-122">Wählen Sie auf dem Symbol " **Einstellungen** " die Option **Kontoeinstellungen** und dann Mandanten **aus.**</span><span class="sxs-lookup"><span data-stu-id="2261c-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Mandanten zuordnen"::: 

3. <span data-ttu-id="2261c-124">Wählen Sie **anderen AD** -Mandanten zuordnen aus, und geben Sie den Mandanten an, den Sie zuordnen möchten</span><span class="sxs-lookup"><span data-stu-id="2261c-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="2261c-125">Melden Sie sich als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und bestätigen Sie die Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="2261c-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zuordnen von Mandanten bestätigen"::: 

5. <span data-ttu-id="2261c-127">Nachdem Sie sich vergewissert haben, wird eine Benachrichtigung über den Hinweis " **alle** " angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2261c-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="2261c-128">Wählen Sie **zur Mandanten Verwaltung zurückkehren aus,** damit der neu hinzugefügte Mandant aufgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2261c-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="2261c-129">Sie können einem Konto keinen Mandanten zuordnen, wenn dieser bereits einem anderen Partner Center-Konto zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="2261c-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="2261c-130">Entfernen eines Mandanten aus Ihrem Konto</span><span class="sxs-lookup"><span data-stu-id="2261c-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="2261c-131">Melden Sie sich als globaler Administrator beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="2261c-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="2261c-132">Wählen Sie im Symbol " **Einstellungen** " die Option **Kontoeinstellungen** -> Mandanten aus, und klicken Sie auf die Registerkarte **Partner** .</span><span class="sxs-lookup"><span data-stu-id="2261c-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="2261c-133">Klicken Sie für den Mandanten, den Sie trennen möchten, auf **Entfernen** .</span><span class="sxs-lookup"><span data-stu-id="2261c-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="2261c-134">Das Aufheben der Zuordnung eines Mandanten bedeutet, dass die Benutzer in diesem Mandanten keinen Zugriff mehr auf das Partner Center-Konto haben. Dies kann sich auf ihre Kompetenzen auswirken.</span><span class="sxs-lookup"><span data-stu-id="2261c-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="2261c-135">Die Schaltfläche " **Entfernen** " ist für alle zugeordneten Mandanten aktiviert, mit Ausnahme des primären Mandanten und des Mandanten, bei dem Sie zurzeit angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="2261c-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="Mandanten mit der Schaltfläche &quot;entfernen&quot;":::
 

## <a name="next-steps"></a><span data-ttu-id="2261c-137">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2261c-137">Next steps</span></span>

- [<span data-ttu-id="2261c-138">Hinzufügen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="2261c-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






