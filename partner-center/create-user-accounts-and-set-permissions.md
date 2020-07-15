---
title: Erstellen von Benutzerkonten und Zuweisen von Rollen
description: Jedem Mitarbeiter muss eine Rolle zugewiesen werden, bevor er auf das Partner Center zugreifen kann. Erfahren Sie, wie Sie Benutzerkonten erstellen, Rollen zuweisen und Berechtigungen festlegen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
Keywords: Rollen, Berechtigungen, Benutzer hinzufügen, Rolle zuweisen, Administrator, Agent
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 9ec8e98f77d49e34b6747b0f580502e9df25a950
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265197"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="93062-105">Erstellen von Benutzerkonten und Zuweisen von Rollen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93062-105">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="93062-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="93062-106">**Appropriate roles**</span></span>

- <span data-ttu-id="93062-107">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="93062-107">Account admin</span></span>
- <span data-ttu-id="93062-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="93062-108">Global admin</span></span>
- <span data-ttu-id="93062-109">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="93062-109">User management admin</span></span>

<span data-ttu-id="93062-110">Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf das Partner Center benötigen.</span><span class="sxs-lookup"><span data-stu-id="93062-110">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="93062-111">Diese Aufgaben müssen von einem Administrator für die Benutzerverwaltung, Kontoadministrator oder vom globalen Administrator durchgeführt werden. Dem Benutzer, der diese Aufgaben ausführt, müssen auch die AAD-Rollen (Azure Active Directory) „Benutzeradministrator“ und „Globaler Administrator“ zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="93062-111">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="93062-112">Weitere Informationen zu AAD-Rollen findest du unter [Berechtigungen für Administratorrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="93062-112">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="93062-113">Neuen Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="93062-113">Add a new user</span></span>

1. <span data-ttu-id="93062-114">Klicken Sie im Partner Center rechts oben auf das Symbol **Einstellungen** und dann auf **Benutzerverwaltung**.</span><span class="sxs-lookup"><span data-stu-id="93062-114">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="93062-115">Wählen Sie **Benutzer hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="93062-115">Select **Add user**.</span></span>

3. <span data-ttu-id="93062-116">Gib den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.</span><span class="sxs-lookup"><span data-stu-id="93062-116">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="93062-117">Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="93062-117">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="93062-118">Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="93062-118">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="93062-119">Wenn Benutzer eine Rollenzuweisung wünschen, finden sie die zu kontaktierenden globalen Administratoren unter **Benutzerverwaltung** durch Filtern nach „globaler Administrator“.</span><span class="sxs-lookup"><span data-stu-id="93062-119">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="93062-120">Wählen Sie **Hinzufügen** aus, um das Benutzerkonto zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="93062-120">Select **Add** to create the user account.</span></span> <span data-ttu-id="93062-121">Bestätigen Sie die Details des Benutzers auf der nächsten Seite.</span><span class="sxs-lookup"><span data-stu-id="93062-121">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="93062-122">Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="93062-122">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="93062-123">Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="93062-123">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="93062-124">Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden.</span><span class="sxs-lookup"><span data-stu-id="93062-124">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="93062-125">Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern.</span><span class="sxs-lookup"><span data-stu-id="93062-125">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="93062-126">Finden des globalen Administrators</span><span class="sxs-lookup"><span data-stu-id="93062-126">Find your global admin</span></span>

<span data-ttu-id="93062-127">Es kann vorkommen, dass ein Benutzer seine Rolle ändern lassen muss oder ein neuer Benutzer eine Zuweisung zu einer bestimmten Rolle wünscht.</span><span class="sxs-lookup"><span data-stu-id="93062-127">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="93062-128">Um einen globalen Administrator zu finden, der Rollenänderungen vornehmen oder einem neuen Benutzer Rollen zuweisen kann, klicken Sie rechts oben im Partner Center auf das Symbol **Einstellungen**, wählen Sie **Benutzerverwaltung** aus, und filtern Sie nach „Globaler Administrator“.</span><span class="sxs-lookup"><span data-stu-id="93062-128">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="93062-129">Neuer globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="93062-129">New global admin</span></span>

<span data-ttu-id="93062-130">Wenn Ihr globaler Administrator aus dem Unternehmen ausscheidet und diese Aufgabe von jemand anderem übernommen wird, können Sie ein Ticket an das Azure-Team oder an das Office 365-Team senden.</span><span class="sxs-lookup"><span data-stu-id="93062-130">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="93062-131">Wählen Sie eine der folgenden Optionen aus, um zu erfahren, wie Sie dazu vorgehen.</span><span class="sxs-lookup"><span data-stu-id="93062-131">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="93062-132">Neuer globaler Administrator für Azure</span><span class="sxs-lookup"><span data-stu-id="93062-132">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="93062-133">Neuer globaler Administrator für Office 365</span><span class="sxs-lookup"><span data-stu-id="93062-133">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="93062-134">Zuweisen von Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="93062-134">Assign user roles</span></span>

<span data-ttu-id="93062-135">Um im Partner Center arbeiten zu können, muss Ihnen eine Rolle zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="93062-135">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="93062-136">Derzeit gibt es Rollen für Azure Active Directory-Mandanten, Cloud Solution Provider (CSP) und nicht auf AAD bezogene Rollen im Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="93062-136">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="93062-137">Ein einzelnes Unternehmen kann eine alle diese Rollen benötigen.</span><span class="sxs-lookup"><span data-stu-id="93062-137">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="93062-138">Benutzer müssen in Ihrem Mandanten aufgeführt sein, um auf das Partner Center zugreifen zu können.</span><span class="sxs-lookup"><span data-stu-id="93062-138">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="93062-139">Rollenzuweisungen gewähren zusätzliche Zugriffsrechte.</span><span class="sxs-lookup"><span data-stu-id="93062-139">Role assignments provide additional access.</span></span>


<span data-ttu-id="93062-140">**AAD-Mandantenrollen**:</span><span class="sxs-lookup"><span data-stu-id="93062-140">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="93062-141">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="93062-141">Global admin</span></span>
- <span data-ttu-id="93062-142">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="93062-142">User admin</span></span>

<span data-ttu-id="93062-143">**CSP-Rollen**:</span><span class="sxs-lookup"><span data-stu-id="93062-143">**CSP roles include**:</span></span>
- <span data-ttu-id="93062-144">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="93062-144">Admin agent</span></span>
- <span data-ttu-id="93062-145">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="93062-145">Billing admin</span></span>
- <span data-ttu-id="93062-146">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="93062-146">Sales agent</span></span>
- <span data-ttu-id="93062-147">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="93062-147">Helpdesk agent</span></span>

<span data-ttu-id="93062-148">**Rollen für die Verwaltung der MPN-Mitgliedschaft und des Unternehmens (außerhalb von AAD)**</span><span class="sxs-lookup"><span data-stu-id="93062-148">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="93062-149">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="93062-149">MPN partner admin</span></span>
- <span data-ttu-id="93062-150">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="93062-150">Account admin</span></span>
- <span data-ttu-id="93062-151">Administrator für Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="93062-151">Referral admin</span></span>
- <span data-ttu-id="93062-152">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="93062-152">Business profile admin</span></span>
- <span data-ttu-id="93062-153">Incentives-Administrator und -Benutzer</span><span class="sxs-lookup"><span data-stu-id="93062-153">Incentives admin and user</span></span>

<span data-ttu-id="93062-154">**Control Panel Vendor ist eine CSP- und keine AAD-Rolle**.</span><span class="sxs-lookup"><span data-stu-id="93062-154">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="93062-155">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="93062-155">Global admin</span></span>

<span data-ttu-id="93062-156">**Gastbenutzer** muss Teil des AAD-Mandanten sein und eine beliebige AAD-externe Rolle haben.</span><span class="sxs-lookup"><span data-stu-id="93062-156">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="93062-157">Spezifische Informationen zu den Rollen und ihren Möglichkeiten finden Sie unter [Zuweisen von Benutzerberechtigungen](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="93062-157">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="93062-158">Zuordnen des Microsoft Learn Kontos eines Benutzers im Partner Center</span><span class="sxs-lookup"><span data-stu-id="93062-158">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="93062-159">Damit Sie die Schulungs- und Lernpfade anzeigen können, die Ihre Benutzer für Kompetenzen verwenden, müssen sie Ihre MCP-ID ihrem Partner Center-Konto zuordnen.</span><span class="sxs-lookup"><span data-stu-id="93062-159">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="93062-160">Wenn Sie als globaler Administrator neue Benutzer hinzufügen, müssen Sie sie daran erinnern, ihre MCP-ID ihrem Konto zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="93062-160">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="93062-161">Zuordnen Ihrer MCP-ID zu Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="93062-161">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="93062-162">Wähle im Partner Center-Dashboard das Symbol für **Dein Konto** in der rechten Ecke des Dashboards aus, und wähle dann **Mein Profil** aus.</span><span class="sxs-lookup"><span data-stu-id="93062-162">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="93062-163">Unter **Dein Learning** kannst du dein Microsoft Learning-Konto zuordnen und auch dein Microsoft-Konto mit Partner University verbinden.</span><span class="sxs-lookup"><span data-stu-id="93062-163">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
