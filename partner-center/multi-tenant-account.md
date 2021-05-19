---
title: Hinzufügen von Mandanten zu Ihrem Partner Center-Konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie mehrere Azure AD Mandanten in Ihrem Partner Center-Konto hinzufügen, konsolidieren oder verwalten und warum Sie dies tun möchten.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151201"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="24936-103">Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="24936-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="24936-104">**Geeignete Rollen:** globale | Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="24936-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="24936-105">In diesem Artikel wird erläutert, wie Sie mehrere Azure Active Directory -Mandanten (Azure AD) für Ihr Unternehmen konsolidieren und diese dann ihrem Partner Center-Konto hinzufügen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="24936-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="24936-106">Dafür gibt es viele Gründe.</span><span class="sxs-lookup"><span data-stu-id="24936-106">There are many reasons to do so.</span></span> <span data-ttu-id="24936-107">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="24936-107">For example:</span></span>

- <span data-ttu-id="24936-108">Angenommen, Ihr Unternehmen Contoso hat ein anderes Unternehmen erworben: Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="24936-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="24936-109">Sie möchten, dass die beiden Unternehmen getrennt bleiben, aber die neuen Mitarbeiter in der Lage sein sollen, Partner Center zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="24936-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="24936-110">In diesem Fall ordnen Sie den Azure AD Mandanten des neuen Unternehmens Ihrem globalen Partnerkonto (PGA) zu.</span><span class="sxs-lookup"><span data-stu-id="24936-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="24936-111">Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="24936-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="24936-112">Wenn Sie Ihr Unternehmen mit mehr als einem Mandanten (z. *B. contoso.com*, *contoso.uk* und *contoso.in*) ausführen, können Sie diese mithilfe von Mehrinstanzenfähigkeit im gleichen PC-Konto gruppieren.</span><span class="sxs-lookup"><span data-stu-id="24936-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="24936-113">Wenn Die Richtlinien für Fusionen und Übernahmen erfordern, dass Sie mit Mandanten beider Unternehmen zusammenarbeiten, verwenden Sie sowohl die *constoso.com* als auch *fabrikam.com* Mandanten.</span><span class="sxs-lookup"><span data-stu-id="24936-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="24936-114">Benutzer eines beliebigen Mandanten müssen in der Lage sein, Folgendes zu ermöglichen:</span><span class="sxs-lookup"><span data-stu-id="24936-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="24936-115">Greifen Sie auf Partner Center für Schulungen, digitale Downloads oder die McP-Zuordnung (Microsoft Certified Professional) zu.</span><span class="sxs-lookup"><span data-stu-id="24936-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="24936-116">Ihnen werden Partner Center Rollen zugewiesen, z. B. Microsoft Partner Network-Administrator (MPN) oder Incentives-Administrator.</span><span class="sxs-lookup"><span data-stu-id="24936-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="24936-117">Hinzufügen eines Azure AD Mandanten zu Ihrem Konto</span><span class="sxs-lookup"><span data-stu-id="24936-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="24936-118">Melden Sie sich als globaler Administrator bei [Microsoft Partner Center](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="24936-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="24936-119">Wählen Sie oben rechts **Einstellungen** aus, wählen Sie **Kontoeinstellungen** und dann **Mandanten aus.**</span><span class="sxs-lookup"><span data-stu-id="24936-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot der Schaltfläche &quot;Zuordnen&quot; im Bereich &quot;profil&quot; Azure AD"::: 

1. <span data-ttu-id="24936-121">Wählen Sie **Zuordnen** aus, und geben Sie dann den Mandanten an, den Sie zuordnen möchten.</span><span class="sxs-lookup"><span data-stu-id="24936-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="24936-122">Melden Sie sich an der Eingabeaufforderung als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und wählen Sie dann **Bestätigen aus.**</span><span class="sxs-lookup"><span data-stu-id="24936-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot der Schaltfläche &quot;Bestätigen&quot; im Bereich &quot;Neue Azure AD bestätigen&quot;."::: 

   <span data-ttu-id="24936-124">Nachdem Sie die Zuordnung bestätigt haben, wird die Meldung **Alle** festgelegt angezeigt.</span><span class="sxs-lookup"><span data-stu-id="24936-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="24936-125">Um den neu hinzugefügten Mandanten anzeigen zu können, wählen **Sie Zur Mandantenverwaltung zurückkehren aus.**</span><span class="sxs-lookup"><span data-stu-id="24936-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="24936-126">Sie können einen Mandanten nicht einem Konto zuordnen, wenn er bereits einem anderen Konto Partner Center ist.</span><span class="sxs-lookup"><span data-stu-id="24936-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="24936-127">Entfernen eines Mandanten aus Ihrem Konto</span><span class="sxs-lookup"><span data-stu-id="24936-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="24936-128">Melden Sie sich als globaler Administrator bei [Microsoft Partner Center an.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="24936-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="24936-129">Wählen Sie oben rechts das Symbol **Einstellungen** und dann **Kontoeinstellungen aus.**</span><span class="sxs-lookup"><span data-stu-id="24936-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="24936-130">Wählen Sie im linken Bereich **Mandanten aus.**</span><span class="sxs-lookup"><span data-stu-id="24936-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="24936-131">Wählen **Sie unter Azure AD Mandanten verwalten** die Registerkarte **Partner** aus.</span><span class="sxs-lookup"><span data-stu-id="24936-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="24936-132">Klicken **Sie neben** dem Mandanten, dessen Zuordnung Sie entfernen möchten, auf Entfernen.</span><span class="sxs-lookup"><span data-stu-id="24936-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot der aktuellen Mandantenzuordnungen und deren Links zum Entfernen":::

   <span data-ttu-id="24936-134">Wie im vorherigen Screenshot  gezeigt, sind die Links entfernen für alle zugeordneten Mandanten aktiviert, mit Ausnahme des primären Mandanten und des Mandanten, bei dem Sie derzeit angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="24936-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="24936-135">Wenn Sie einen Mandanten entfernen, haben die Benutzer in diesem Mandanten keinen Zugriff mehr auf das Partner Center-Konto, und die Entfernung hat möglicherweise Auswirkungen auf Ihre Kompetenzen.</span><span class="sxs-lookup"><span data-stu-id="24936-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="24936-136">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="24936-136">Next steps</span></span>

- [<span data-ttu-id="24936-137">Erstellen von Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="24936-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






