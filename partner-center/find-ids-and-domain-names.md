---
title: Suchen nach Mandanten-ID, Domänenname, Benutzerobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie IDs im Azure-Portal finden– der Azure AD Mandanten-ID, des Domänennamens oder einer bestimmten Benutzerobjekt-ID einer Organisation. Einige Aufgaben benötigen diese Informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740283"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="34496-104">Suchen wichtiger IDs für einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="34496-104">Locate important IDs for a user</span></span>

<span data-ttu-id="34496-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="34496-105">**Appropriate roles**</span></span>

- <span data-ttu-id="34496-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="34496-106">Global admin</span></span>

<span data-ttu-id="34496-107">In diesem Artikel wird beschrieben, wie Sie die [Azure-Portal](https://portal.azure.com/) verwenden, um die folgenden Informationen für einen Benutzer zu finden:</span><span class="sxs-lookup"><span data-stu-id="34496-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="34496-108">Die Microsoft Azure Active Directory(Azure AD)-Mandanten-ID der Organisation oder des Unternehmens des Benutzers</span><span class="sxs-lookup"><span data-stu-id="34496-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="34496-109">Der primäre Domänenname der Organisation oder des Unternehmens, die dem Azure AD Mandanten zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="34496-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="34496-110">Die Benutzerobjekt-ID</span><span class="sxs-lookup"><span data-stu-id="34496-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="34496-111">Suchen der Microsoft Azure AD Mandanten-ID und des primären Domänennamens</span><span class="sxs-lookup"><span data-stu-id="34496-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="34496-112">Führen Sie diese Schritte aus, um die Azure AD Mandanten-ID oder den primären Domänennamen innerhalb des Azure-Portal zu suchen.</span><span class="sxs-lookup"><span data-stu-id="34496-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="34496-113">(Wenn Sie eine Mandanten-ID programmgesteuert suchen möchten, finden Sie weitere Informationen unter Suchen der [Mandanten-ID mit PowerShell oder der CLI.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="34496-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="34496-114">Die Mandanten-ID kann in verschiedenen Anwendungen oder Ressourcen als unterschiedliche Namen bezeichnet werden.</span><span class="sxs-lookup"><span data-stu-id="34496-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="34496-115">Die Mandanten-ID kann z. B. als Verzeichnis-ID, Azure Active Directory Mandant (Azure AD), Microsoft-ID oder für bestimmte Berichte bezeichnet werden, sogar als *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="34496-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="34496-116">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="34496-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="34496-117">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="34496-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zeigt Azure-Portal auswählen der option Azure Active Directory im Menü an.":::

3. <span data-ttu-id="34496-119">Eine Azure Active Directory **Seite Übersicht** wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34496-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="34496-120">Suchen Sie nach dem Feld Mandanten-ID und dem Feld Primäre **Domäne,** um die Azure AD **Mandanten-ID** oder den primären Domänennamen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="34496-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="34496-121">Diese Felder werden im Abschnitt Mandanteninformationen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34496-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zeigt die Seite Übersicht mit zwei hervorgehobenen Feldern an: Mandanten-ID und primärer Domänenname.":::

4. <span data-ttu-id="34496-123">Sie finden die Mandanten-ID im Azure-Portal auf andere Weise.</span><span class="sxs-lookup"><span data-stu-id="34496-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="34496-124">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="34496-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="34496-125">Navigieren Sie dann im Menü zum Abschnitt **Verwalten,** und wählen Sie **Eigenschaften** aus.</span><span class="sxs-lookup"><span data-stu-id="34496-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="34496-126">Auf der Seite Eigenschaften wird auch die zugeordnete Mandanten-ID des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34496-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Seite &quot;Eigenschaften&quot; mit hervorgehobenen Feld &quot;Mandanten-ID&quot;":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="34496-128">Suchen der Benutzerobjekt-ID</span><span class="sxs-lookup"><span data-stu-id="34496-128">Find the user object ID</span></span>

<span data-ttu-id="34496-129">Das Suchen des Domänennamens und der Mandanten-ID reicht möglicherweise nicht immer aus.</span><span class="sxs-lookup"><span data-stu-id="34496-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="34496-130">Möglicherweise müssen Sie auch die bestimmte Objekt-ID ermitteln, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="34496-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="34496-131">Führen Sie die folgenden Schritte aus, um die Objekt-ID eines Benutzers in der folgenden Azure-Portal:</span><span class="sxs-lookup"><span data-stu-id="34496-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="34496-132">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="34496-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="34496-133">Wählen Sie die Menüoption **Azure Active Directory** aus.</span><span class="sxs-lookup"><span data-stu-id="34496-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="34496-134">Suchen Sie **im Menü** nach dem Abschnitt Verwalten, und wählen Sie dann **Benutzer aus.**</span><span class="sxs-lookup"><span data-stu-id="34496-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zeigt Azure Active Directory mit hervorgehobener Option Benutzer an.":::

4. <span data-ttu-id="34496-136">Geben Sie auf der Seite Benutzer den Namen des Benutzers in das Suchfeld ein.</span><span class="sxs-lookup"><span data-stu-id="34496-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zeigt die Seite Benutzer mit Suchfeld an, um nach einem bestimmten Benutzer zu suchen.":::

5. <span data-ttu-id="34496-138">Wählen Sie den Namen des Benutzers aus, an dem er in der Liste angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="34496-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zeigt die Seite Benutzer an, auf der eine Zeile für den gesuchten Benutzer angezeigt wird.":::

6. <span data-ttu-id="34496-140">Suchen Sie auf der Seite Profil des Benutzers nach dem Abschnitt Identität.</span><span class="sxs-lookup"><span data-stu-id="34496-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="34496-141">Das Feld Objekt-ID wird hier mit der eindeutigen Objekt-ID des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="34496-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zeigt die Seite &quot;Benutzerprofil&quot; mit dem Abschnitt Identität und einem hervorgehobenen Feld für die Objekt-ID an.":::

## <a name="next-steps"></a><span data-ttu-id="34496-143">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="34496-143">Next steps</span></span>

- [<span data-ttu-id="34496-144">Programmgesteuertes Suchen Ihrer Mandanten-ID mit PowerShell oder cli</span><span class="sxs-lookup"><span data-stu-id="34496-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="34496-145">Weitere Informationen zu Benutzerprofilen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="34496-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="34496-146">Erfahren Sie, wie Partner Kundendetails in der Partner Center</span><span class="sxs-lookup"><span data-stu-id="34496-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

