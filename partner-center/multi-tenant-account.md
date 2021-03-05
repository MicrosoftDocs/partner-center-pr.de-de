---
title: Hinzufügen von Mandanten zu Ihrem Partner Center-Konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie mehrere Azure AD Mandanten in Ihrem Partner Center-Konto hinzufügen, konsolidieren oder verwalten, und erfahren Sie, warum Sie dies möglicherweise tun möchten.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124804"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="34168-103">Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="34168-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="34168-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="34168-104">**Appropriate roles**</span></span>

- <span data-ttu-id="34168-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="34168-105">Global admin</span></span>
- <span data-ttu-id="34168-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="34168-106">Account admin</span></span>

<span data-ttu-id="34168-107">In diesem Artikel wird erläutert, wie Sie mehrere Azure Active Directory Mandanten (Azure AD) für Ihr Unternehmen konsolidieren und diese dann in Ihrem Partner Center-Konto hinzufügen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="34168-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="34168-108">Hierfür gibt es viele Gründe.</span><span class="sxs-lookup"><span data-stu-id="34168-108">There are many reasons to do so.</span></span> <span data-ttu-id="34168-109">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="34168-109">For example:</span></span>

- <span data-ttu-id="34168-110">Nehmen wir beispielsweise an, dass Ihr Unternehmen, ".</span><span class="sxs-lookup"><span data-stu-id="34168-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="34168-111">Sie möchten, dass die beiden Unternehmen getrennt bleiben, aber Sie möchten, dass die neuen Mitarbeiter Partner Center verwenden können.</span><span class="sxs-lookup"><span data-stu-id="34168-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="34168-112">In diesem Fall ordnen Sie den Azure AD Mandanten des neuen Unternehmens Ihrem Partner-Global-Konto (PGA) zu.</span><span class="sxs-lookup"><span data-stu-id="34168-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="34168-113">Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="34168-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="34168-114">Wenn Sie Ihr Unternehmen mit mehr als einem Mandanten ausführen (z. b. *contoso.com*, *contoso.uk* und *contoso.in*), können Sie die mehr Instanzen Fähigkeit verwenden, um Sie im gleichen PC-Konto zu gruppieren.</span><span class="sxs-lookup"><span data-stu-id="34168-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="34168-115">Wenn die Richtlinien für Fusionen und Übernahmen Sie bei der Zusammenarbeit mit Mandanten beider Unternehmen benötigen, verwenden Sie die Mandanten *constoso.com* und *Fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="34168-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="34168-116">Benutzer eines beliebigen Mandanten müssen folgende Aktionen ausführen können:</span><span class="sxs-lookup"><span data-stu-id="34168-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="34168-117">Zugang zum Partner Center für Schulungen, digitale Downloads oder Microsoft Certified Professional-Zuordnungen (MCP).</span><span class="sxs-lookup"><span data-stu-id="34168-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="34168-118">Zugewiesenen Partner Center-Rollen wie Microsoft Partner Network (MPN) admin oder Incentive admin.</span><span class="sxs-lookup"><span data-stu-id="34168-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="34168-119">Fügen Sie Ihrem Konto einen Azure AD Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="34168-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="34168-120">Melden Sie sich als globaler Administrator bei [Microsoft Partner Center](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="34168-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="34168-121">Klicken Sie oben rechts auf **Einstellungen**, wählen Sie **Kontoeinstellungen** aus, und wählen Sie dann Mandanten **aus.**</span><span class="sxs-lookup"><span data-stu-id="34168-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot der Schaltfläche &quot;zuordnen&quot; im Bereich &quot;Azure AD Profil&quot;."::: 

1. <span data-ttu-id="34168-123">Wählen Sie **zuordnen** aus, und geben Sie dann den Mandanten an, den Sie zuordnen möchten.</span><span class="sxs-lookup"><span data-stu-id="34168-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="34168-124">Melden Sie sich an der Eingabeaufforderung als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und wählen Sie dann **bestätigen** aus.</span><span class="sxs-lookup"><span data-stu-id="34168-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot der Schaltfläche &quot;bestätigen&quot; im Bereich &quot;neue Azure AD Zuordnung bestätigen&quot;."::: 

   <span data-ttu-id="34168-126">Nachdem Sie die Zuordnung bestätigt haben, wird eine **alle festgelegte** Meldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34168-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="34168-127">Um den neu hinzugefügten Mandanten anzuzeigen, wählen Sie **zur Mandanten Verwaltung zurückkehren** aus.</span><span class="sxs-lookup"><span data-stu-id="34168-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="34168-128">Sie können einen Mandanten nicht mit einem Konto verknüpfen, wenn es bereits einem anderen Partner Center-Konto zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="34168-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="34168-129">Entfernen eines Mandanten aus Ihrem Konto</span><span class="sxs-lookup"><span data-stu-id="34168-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="34168-130">Melden Sie sich als globaler Administrator bei [Microsoft Partner Center](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="34168-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="34168-131">Klicken Sie in der oberen rechten Ecke auf das Symbol **Einstellungen** , und wählen Sie dann **Kontoeinstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="34168-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="34168-132">**Wählen Sie** im linken Bereich Mandanten aus.</span><span class="sxs-lookup"><span data-stu-id="34168-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="34168-133">Wählen Sie unter **Azure AD Mandanten verwalten** die Registerkarte **Partner** aus.</span><span class="sxs-lookup"><span data-stu-id="34168-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="34168-134">Wählen Sie neben dem Mandanten, dessen Zuordnung Sie entfernen möchten, die Option **Entfernen** aus.</span><span class="sxs-lookup"><span data-stu-id="34168-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot der aktuellen Mandanten Zuordnungen und ihrer Entfernungs Verknüpfungen.":::

   <span data-ttu-id="34168-136">Wie im obigen Screenshot gezeigt, sind die **Entfernungs Entfernungs** Links für alle zugeordneten Mandanten aktiviert, mit Ausnahme des primären Mandanten und des Mandanten, bei dem Sie zurzeit angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="34168-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="34168-137">Wenn Sie einen Mandanten entfernen, haben die Benutzer in diesem Mandanten keinen Zugriff mehr auf das Partner Center-Konto, und die Entfernung wirkt sich möglicherweise auf ihre Kompetenzen aus.</span><span class="sxs-lookup"><span data-stu-id="34168-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="34168-138">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="34168-138">Next steps</span></span>

- [<span data-ttu-id="34168-139">Erstellen von Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="34168-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






