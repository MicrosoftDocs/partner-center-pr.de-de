---
title: Suchen von Mandanten-ID, Domänen Name, Benutzerobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie IDs in der Azure-Portal Azure AD Mandanten-ID, Domänen Name oder bestimmte Benutzerobjekt-ID des Unternehmens finden. Einige Aufgaben benötigen diese Informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360070"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="e4b42-104">Wichtige IDs für einen Benutzer suchen</span><span class="sxs-lookup"><span data-stu-id="e4b42-104">Locate important IDs for a user</span></span>

<span data-ttu-id="e4b42-105">In diesem Artikel wird beschrieben, wie Sie den [Azure-Portal](https://portal.azure.com/) verwenden, um die folgenden Informationen für einen Benutzer zu suchen:</span><span class="sxs-lookup"><span data-stu-id="e4b42-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="e4b42-106">Die Microsoft Azure Active Directory-Mandanten-ID (Azure AD) der Organisation oder des Unternehmens des Benutzers</span><span class="sxs-lookup"><span data-stu-id="e4b42-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="e4b42-107">Der primäre Domänen Name der Organisation oder des Unternehmens, die mit dem Azure AD Mandanten verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="e4b42-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="e4b42-108">Die Benutzerobjekt-ID</span><span class="sxs-lookup"><span data-stu-id="e4b42-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="e4b42-109">Suchen der Microsoft Azure AD Mandanten-ID und des primären Domänen Namens</span><span class="sxs-lookup"><span data-stu-id="e4b42-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="e4b42-110">Führen Sie diese Schritte aus, um die Azure AD Mandanten-ID oder den primären Domänen Namen innerhalb des Azure-Portal zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="e4b42-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="e4b42-111">(Wenn Sie eine Mandanten-ID Programm gesteuert finden möchten, finden Sie weitere Informationen untersuchen der Mandanten- [ID mit PowerShell oder der CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="e4b42-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="e4b42-112">Die Mandanten-ID kann in verschiedenen Anwendungen oder Ressourcen als unterschiedliche Namen bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="e4b42-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="e4b42-113">Beispielsweise kann die Mandanten-ID als Verzeichnis-ID, der Azure Active Directory (Azure AD)-Mandant, Microsoft-ID oder für bestimmte Berichte (auch *tenantguid* ) bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="e4b42-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="e4b42-114">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="e4b42-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e4b42-115">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="e4b42-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zeigt, Azure-Portal die Azure Active Directory-Option im Menü ausgewählt wird.":::

3. <span data-ttu-id="e4b42-117">Eine Azure Active Directory **Übersichts** Seite wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e4b42-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="e4b42-118">Wenn Sie die Azure AD Mandanten-ID oder den primären Domänen Namen ermitteln möchten, suchen Sie nach dem Feld Mandanten- **ID** und dem Feld **primäre Domäne** .</span><span class="sxs-lookup"><span data-stu-id="e4b42-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="e4b42-119">Diese Felder werden im Abschnitt Mandanten Informationen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e4b42-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zeigt eine Übersichtsseite mit zwei markierten Feldern, der Mandanten-ID und dem primären Domänen Namen an.":::

4. <span data-ttu-id="e4b42-121">Sie finden die Mandanten-ID in der Azure-Portal auf andere Weise.</span><span class="sxs-lookup"><span data-stu-id="e4b42-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="e4b42-122">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="e4b42-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="e4b42-123">Suchen Sie anschließend im Menü den Abschnitt **Verwalten** , und wählen Sie **Eigenschaften** aus.</span><span class="sxs-lookup"><span data-stu-id="e4b42-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="e4b42-124">Auf der Seite "Eigenschaften" wird auch die zugehörige Mandanten-ID des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e4b42-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zeigt die Eigenschaften Seite mit hervorgehobenem Feld für Mandanten-ID.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="e4b42-126">Suchen der Benutzerobjekt-ID</span><span class="sxs-lookup"><span data-stu-id="e4b42-126">Find the user object ID</span></span>

<span data-ttu-id="e4b42-127">Das Auffinden des Domänen Namens und der Mandanten-ID ist möglicherweise nicht immer ausreichend.</span><span class="sxs-lookup"><span data-stu-id="e4b42-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="e4b42-128">Möglicherweise müssen Sie auch die spezifische Objekt-ID suchen, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="e4b42-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="e4b42-129">Führen Sie die folgenden Schritte aus, um die Objekt-ID eines Benutzers in der Azure-Portal zu finden:</span><span class="sxs-lookup"><span data-stu-id="e4b42-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="e4b42-130">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="e4b42-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e4b42-131">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="e4b42-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="e4b42-132">Suchen Sie im Menü den Abschnitt **Verwalten** , und wählen Sie dann **Benutzer** aus.</span><span class="sxs-lookup"><span data-stu-id="e4b42-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zeigt Azure Active Directory Menü mit hervorgehobener Option _OL_QUOTE_PLACEHOLDER_Benutzer_OL_QUOTE_PLACEHOLDER_ an.":::

4. <span data-ttu-id="e4b42-134">Geben Sie auf der Seite Benutzer den Namen des Benutzers in das Suchfeld ein.</span><span class="sxs-lookup"><span data-stu-id="e4b42-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zeigt die Seite _OL_QUOTE_PLACEHOLDER_Benutzer_OL_QUOTE_PLACEHOLDER_ mit Suchfeld an, um nach einem bestimmten Benutzer zu suchen.":::

5. <span data-ttu-id="e4b42-136">Wählen Sie den Namen des Benutzers aus, in dem er in der Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e4b42-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zeigt die Benutzerseite an, die eine Zeile für den gesuchten Benutzer anzeigt.":::

6. <span data-ttu-id="e4b42-138">Suchen Sie auf der Profilseite des Benutzers den Abschnitt "Identität".</span><span class="sxs-lookup"><span data-stu-id="e4b42-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="e4b42-139">Das Feld Objekt-ID wird hier mit der eindeutigen Objekt-ID des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e4b42-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zeigt die Seite _OL_QUOTE_PLACEHOLDER_Benutzerprofil_OL_QUOTE_PLACEHOLDER_ mit dem Identitäts Abschnitt und einem markierten Feld für die Objekt-ID an.":::

## <a name="next-steps"></a><span data-ttu-id="e4b42-141">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="e4b42-141">Next steps</span></span>

- [<span data-ttu-id="e4b42-142">Programm gesteuertes ermitteln Ihrer Mandanten-ID mit PowerShell oder der CLI</span><span class="sxs-lookup"><span data-stu-id="e4b42-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="e4b42-143">Weitere Informationen zu Benutzerprofilen finden Sie unter Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e4b42-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="e4b42-144">Erfahren Sie, wie Partner Kunden Details in Partner Center sehen oder exportieren können.</span><span class="sxs-lookup"><span data-stu-id="e4b42-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)
