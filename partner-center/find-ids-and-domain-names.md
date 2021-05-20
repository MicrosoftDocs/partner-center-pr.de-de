---
title: Suchen der Mandanten-ID, des Domänennamens, der Benutzerobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie IDs im Azure-Portal suchen– die Azure AD Mandanten-ID, den Domänennamen oder die spezifische Benutzerobjekt-ID einer Organisation. Einige Aufgaben benötigen diese Informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150861"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="b0e8a-104">Suchen wichtiger IDs für einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="b0e8a-104">Locate important IDs for a user</span></span>

<span data-ttu-id="b0e8a-105">**Geeignete Rollen**: Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b0e8a-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="b0e8a-106">In diesem Artikel wird beschrieben, wie Sie [die](https://portal.azure.com/) Azure-Portal verwenden, um die folgenden Informationen für einen Benutzer zu finden:</span><span class="sxs-lookup"><span data-stu-id="b0e8a-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="b0e8a-107">Die Microsoft Azure Active Directory (Azure AD) Mandanten-ID der Organisation oder des Unternehmens des Benutzers</span><span class="sxs-lookup"><span data-stu-id="b0e8a-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="b0e8a-108">Der primäre Domänenname der Organisation oder des Unternehmens, die dem Azure AD zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="b0e8a-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="b0e8a-109">Die Benutzerobjekt-ID</span><span class="sxs-lookup"><span data-stu-id="b0e8a-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="b0e8a-110">Suchen der Microsoft Azure AD Mandanten-ID und des primären Domänennamens</span><span class="sxs-lookup"><span data-stu-id="b0e8a-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="b0e8a-111">Führen Sie die folgenden Schritte aus, um die Azure AD Mandanten-ID oder den primären Domänennamen in der Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="b0e8a-112">(Wenn Sie eine Mandanten-ID programmgesteuert suchen möchten, finden Sie weitere Informationen unter Suchen der [Mandanten-ID mit PowerShell oder cli.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="b0e8a-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="b0e8a-113">Die Mandanten-ID kann in verschiedenen Anwendungen oder Ressourcen als unterschiedliche Namen bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="b0e8a-114">Beispielsweise kann die Mandanten-ID als Verzeichnis-ID, der Azure Active Directory-Mandant (Azure AD), die Microsoft-ID oder für bestimmte Berichte, sogar *als tenantguid,* bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="b0e8a-115">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="b0e8a-116">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zeigt Azure-Portal, wie Sie die Azure Active Directory im Menü auswählen.":::

3. <span data-ttu-id="b0e8a-118">Eine Azure Active Directory **Seite Übersicht** wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="b0e8a-119">Um die Azure AD Mandanten-ID oder den primären Domänennamen zu finden, suchen Sie nach dem Feld **Mandanten-ID** und dem Feld **Primäre** Domäne.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="b0e8a-120">Diese Felder werden im Abschnitt Mandanteninformationen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zeigt die Seite Übersicht mit zwei hervorgehobenen Feldern an: Mandanten-ID und primärer Domänenname.":::

4. <span data-ttu-id="b0e8a-122">Sie können die Mandanten-ID in der Azure-Portal auf einige andere Arten finden.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="b0e8a-123">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="b0e8a-124">Suchen Sie dann im Menü **nach dem** Abschnitt Verwalten, und wählen Sie **Eigenschaften aus.**</span><span class="sxs-lookup"><span data-stu-id="b0e8a-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="b0e8a-125">Auf der Seite Eigenschaften wird auch die zugeordnete Mandanten-ID des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zeigt die Seite Eigenschaften mit hervorgehobenen Feld Mandanten-ID an.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="b0e8a-127">Suchen der Benutzerobjekt-ID</span><span class="sxs-lookup"><span data-stu-id="b0e8a-127">Find the user object ID</span></span>

<span data-ttu-id="b0e8a-128">Es reicht möglicherweise nicht immer aus, nur den Domänennamen und die Mandanten-ID zu finden.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="b0e8a-129">Möglicherweise müssen Sie auch die bestimmte Objekt-ID suchen, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="b0e8a-130">Führen Sie die folgenden Schritte aus, um die Objekt-ID eines Benutzers im Azure-Portal zu suchen:</span><span class="sxs-lookup"><span data-stu-id="b0e8a-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="b0e8a-131">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="b0e8a-132">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="b0e8a-133">Suchen Sie im Menü den Abschnitt **Verwalten,** und wählen Sie dann **Benutzer** aus.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zeigt Azure Active Directory Menü mit hervorgehobener Option Benutzer an.":::

4. <span data-ttu-id="b0e8a-135">Geben Sie auf der Seite Benutzer den Namen des Benutzers in das Suchfeld ein.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zeigt die Seite Benutzer mit suchfeld an, um nach einem bestimmten Benutzer zu suchen.":::

5. <span data-ttu-id="b0e8a-137">Wählen Sie den Namen des Benutzers aus, an dem er in der Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zeigt die Seite Benutzer an, auf der eine Zeile für den gesuchten Benutzer angezeigt wird.":::

6. <span data-ttu-id="b0e8a-139">Suchen Sie den Abschnitt Identität auf der Seite Profil des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="b0e8a-140">Das Feld Objekt-ID wird hier mit der eindeutigen Objekt-ID des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zeigt die Seite Benutzerprofil mit dem Abschnitt Identität und einem hervorgehobenen Feld für Objekt-ID an.":::

## <a name="next-steps"></a><span data-ttu-id="b0e8a-142">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="b0e8a-142">Next steps</span></span>

- [<span data-ttu-id="b0e8a-143">Programmgesteuertes Suchen Ihrer Mandanten-ID mit PowerShell oder cli</span><span class="sxs-lookup"><span data-stu-id="b0e8a-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="b0e8a-144">Weitere Informationen zu Benutzerprofilen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b0e8a-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="b0e8a-145">Erfahren Sie, wie Partner Kundendetails in Partner Center anzeigen oder exportieren können.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

