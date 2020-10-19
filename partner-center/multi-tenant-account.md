---
title: Fügen Sie Ihrem Partner Center-Konto weitere Mandanten hinzu.
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie mehrere Azure AD Mandanten in Ihrem Partner Center-Konto hinzufügen, konsolidieren oder verwalten. Informieren Sie sich auch über einige der Gründe, die Sie möglicherweise tun möchten.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175158"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="d776c-104">Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="d776c-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="d776c-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="d776c-105">**Applies to**</span></span>

- <span data-ttu-id="d776c-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="d776c-106">Partner Center</span></span>

<span data-ttu-id="d776c-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="d776c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d776c-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="d776c-108">Global admin</span></span>

<span data-ttu-id="d776c-109">Mit diesem Feature können Sie mehrere Mandanten für Ihr Unternehmen verwalten und sie in Ihrem Partner Center-Konto konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="d776c-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="d776c-110">Es gibt viele Gründe, warum Sie möglicherweise mehrere Azure AD Mandanten in Ihrem Partner Center-Konto verwalten müssen.</span><span class="sxs-lookup"><span data-stu-id="d776c-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="d776c-111">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d776c-111">For example:</span></span>

- <span data-ttu-id="d776c-112">Ihr Unternehmen kann ein anderes Unternehmen erwerben und möchten, dass die Mitarbeiter des neuen Unternehmens Partner Center verwenden können.</span><span class="sxs-lookup"><span data-stu-id="d776c-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="d776c-113">Sie möchten jedoch, dass die beiden Unternehmen getrennt bleiben.</span><span class="sxs-lookup"><span data-stu-id="d776c-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="d776c-114">In diesem Fall würden Sie den Azure AD Mandanten des neuen Unternehmens mit ihrem globalen Partner Konto (PGA) verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="d776c-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="d776c-115">Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="d776c-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="d776c-116">Wenn Sie über mehr als einen Mandanten verfügen, um Ihr Unternehmen auszuführen (z. b. contoso.com, contoso.uk, contoso.in), können Sie die mehr Instanzen Fähigkeit verwenden, um Sie mit dem gleichen PC-Konto zu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="d776c-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="d776c-117">Bei Fusionen und Übernahmen müssen Sie mit mehr als einem Mandanten arbeiten (Wenn Contoso beispielsweise Fabrikam übernimmt), müssen Sie in der Lage sein, sowohl constoso.com als auch fabrikam.com entsprechende Mandanten zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d776c-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="d776c-118">Benutzer von einem der Mandanten müssen folgende Aktionen ausführen können:</span><span class="sxs-lookup"><span data-stu-id="d776c-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="d776c-119">Access Partner Center für Schulungen, digitale Downloads, MCP-Zuordnung</span><span class="sxs-lookup"><span data-stu-id="d776c-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="d776c-120">Ihnen werden Partner Center-Rollen wie MPN admin, Incentive admin usw. zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="d776c-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="d776c-121">Fügen Sie Ihrem Konto einen weiteren Azure AD Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="d776c-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="d776c-122">Melden Sie sich als globaler Administrator beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="d776c-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="d776c-123">Wählen Sie auf dem Symbol " **Einstellungen** " die Option **Kontoeinstellungen** und dann Mandanten **aus.**</span><span class="sxs-lookup"><span data-stu-id="d776c-123">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Mandanten zuordnen"::: 

3. <span data-ttu-id="d776c-125">Wählen Sie **anderen AD** -Mandanten zuordnen aus, und geben Sie den Mandanten an, den Sie zuordnen möchten</span><span class="sxs-lookup"><span data-stu-id="d776c-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="d776c-126">Melden Sie sich als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und bestätigen Sie die Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="d776c-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Mandanten zuordnen"::: 

5. <span data-ttu-id="d776c-128">Nachdem Sie sich vergewissert haben, wird eine Benachrichtigung über den Hinweis " **alle** " angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d776c-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="d776c-129">Wählen Sie **zur Mandanten Verwaltung zurückkehren aus,** damit der neu hinzugefügte Mandant aufgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d776c-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="d776c-130">Sie können einem Konto keinen Mandanten zuordnen, wenn dieser bereits einem anderen Partner Center-Konto zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="d776c-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="d776c-131">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d776c-131">Next steps</span></span>

- [<span data-ttu-id="d776c-132">Hinzufügen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="d776c-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
