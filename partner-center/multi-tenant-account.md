---
title: Fügen Sie Ihrem Partner Center-Konto weitere Mandanten hinzu.
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verwalten mehrerer Mandanten über Ihr Partner Center-Konto
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389515"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="ce3a6-103">Hinzufügen und Verwalten mehrerer Mandanten in Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="ce3a6-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="ce3a6-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="ce3a6-104">**Applies to**</span></span>

- <span data-ttu-id="ce3a6-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="ce3a6-105">Partner Center</span></span>

<span data-ttu-id="ce3a6-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="ce3a6-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ce3a6-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="ce3a6-107">Global admin</span></span>

<span data-ttu-id="ce3a6-108">Es gibt viele Gründe, warum Sie möglicherweise mehrere Azure AD Mandanten in Ihrem Partner Center-Konto verwalten müssen.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="ce3a6-109">Beispielsweise kann Ihr Unternehmen ein anderes Unternehmen erwerben und möchten, dass die Mitarbeiter des neuen Unternehmens Partner Center verwenden können.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="ce3a6-110">Sie möchten jedoch, dass die beiden Unternehmen getrennt bleiben.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="ce3a6-111">In diesem Fall würden Sie den Azure AD Mandanten des neuen Unternehmens Ihrem Partner-globalen Konto (PNG) zuordnen.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="ce3a6-112">Diese Zuordnung ermöglicht es Benutzern in beiden Unternehmen, in Partner Center zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="ce3a6-113">Fügen Sie Ihrem Konto einen weiteren Azure AD Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="ce3a6-114">Melden Sie sich als globaler Administrator beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="ce3a6-115">Wählen Sie auf dem Symbol " **Einstellungen** " die Option **Kontoeinstellungen** und dann Mandanten **aus.**</span><span class="sxs-lookup"><span data-stu-id="ce3a6-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="Mandanten zuordnen"::: 

3. <span data-ttu-id="ce3a6-117">Wählen Sie **anderen AD** -Mandanten zuordnen aus, und geben Sie den Mandanten an, den Sie zuordnen möchten</span><span class="sxs-lookup"><span data-stu-id="ce3a6-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="ce3a6-118">Melden Sie sich als globaler Administrator bei dem Mandanten an, den Sie zuordnen möchten, und bestätigen Sie die Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="Zuordnen von Mandanten bestätigen"::: 

5. <span data-ttu-id="ce3a6-120">Nachdem Sie sich vergewissert haben, wird eine Benachrichtigung über den Hinweis " **alle** " angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="ce3a6-121">Wählen Sie **zur Mandanten Verwaltung zurückkehren aus,** damit der neu hinzugefügte Mandant aufgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="ce3a6-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="ce3a6-122">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ce3a6-122">Next steps</span></span>

- [<span data-ttu-id="ce3a6-123">Hinzufügen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="ce3a6-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
