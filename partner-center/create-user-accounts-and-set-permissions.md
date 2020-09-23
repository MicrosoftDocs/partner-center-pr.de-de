---
title: Erstellen von Benutzerkonten und Zuweisen von Rollen
description: Jedem Mitarbeiter muss eine Rolle zugewiesen werden, bevor er auf das Partner Center zugreifen kann. Erfahren Sie, wie Sie Benutzerkonten erstellen, Rollen zuweisen und Berechtigungen festlegen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 637e88205d9944f7220e227b5101220d94ed42db
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000434"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="8bf64-104">Erstellen von Benutzerkonten und Zuweisen von Rollen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8bf64-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="8bf64-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="8bf64-105">**Appropriate roles**</span></span>

- <span data-ttu-id="8bf64-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-106">Account admin</span></span>
- <span data-ttu-id="8bf64-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-107">Global admin</span></span>
- <span data-ttu-id="8bf64-108">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-108">User management admin</span></span>

<span data-ttu-id="8bf64-109">Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf das Partner Center benötigen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="8bf64-110">Diese Aufgaben müssen von einem Administrator für die Benutzerverwaltung, Kontoadministrator oder vom globalen Administrator durchgeführt werden. Dem Benutzer, der diese Aufgaben ausführt, müssen auch die AAD-Rollen (Azure Active Directory) „Benutzeradministrator“ und „Globaler Administrator“ zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="8bf64-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="8bf64-111">Weitere Informationen zu AAD-Rollen findest du unter [Berechtigungen für Administratorrollen in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="8bf64-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="8bf64-112">Neuen Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8bf64-112">Add a new user</span></span>

1. <span data-ttu-id="8bf64-113">Klicken Sie im Partner Center rechts oben auf das Symbol **Einstellungen** und dann auf **Benutzerverwaltung**.</span><span class="sxs-lookup"><span data-stu-id="8bf64-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="8bf64-114">Wählen Sie **Benutzer hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="8bf64-114">Select **Add user**.</span></span>

3. <span data-ttu-id="8bf64-115">Gib den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.</span><span class="sxs-lookup"><span data-stu-id="8bf64-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="8bf64-116">Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="8bf64-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="8bf64-117">Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="8bf64-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="8bf64-118">Wenn Benutzer eine Rollenzuweisung wünschen, finden sie die zu kontaktierenden globalen Administratoren unter **Benutzerverwaltung** durch Filtern nach „globaler Administrator“.</span><span class="sxs-lookup"><span data-stu-id="8bf64-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="8bf64-119">Wählen Sie **Hinzufügen** aus, um das Benutzerkonto zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="8bf64-120">Bestätigen Sie die Details des Benutzers auf der nächsten Seite.</span><span class="sxs-lookup"><span data-stu-id="8bf64-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="8bf64-121">Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8bf64-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="8bf64-122">Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="8bf64-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="8bf64-123">Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden.</span><span class="sxs-lookup"><span data-stu-id="8bf64-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="8bf64-124">Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern.</span><span class="sxs-lookup"><span data-stu-id="8bf64-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="8bf64-125">Finden der Rolle, die Ihnen zugewiesen wurde</span><span class="sxs-lookup"><span data-stu-id="8bf64-125">Find the role you've been assigned</span></span>

<span data-ttu-id="8bf64-126">Wenn Ihr globaler Administrator Sie nicht informiert hat, können Sie wie folgt herausfinden, welche Rolle Sie in Partner Center innehaben:</span><span class="sxs-lookup"><span data-stu-id="8bf64-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="8bf64-127">Melden Sie sich beim Partner Center-[dashboard]https://partner.microsoft.com/dashboard/home) an.</span><span class="sxs-lookup"><span data-stu-id="8bf64-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="8bf64-128">Wählen Sie das Symbol **Kontoeinstellungen** und dann **Mein Profil** aus.</span><span class="sxs-lookup"><span data-stu-id="8bf64-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="8bf64-129">Wählen Sie die Registerkarte **Rollen und Berechtigungen** aus. Ihre Rollen und Berechtigungen werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8bf64-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="8bf64-130">Wenn Sie nach dem Anmelden ein Programm nicht sehen können, bedeutet dies in der Regel, dass Sie nicht über die erforderlichen Berechtigungen verfügen, um in diesem Programm arbeiten zu können.</span><span class="sxs-lookup"><span data-stu-id="8bf64-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="8bf64-131">Wenn Sie beispielsweise nach dem Anmelden die Seite „Incentives“ nicht sehen, besitzen Sie keine Berechtigungen für Incentives.</span><span class="sxs-lookup"><span data-stu-id="8bf64-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="8bf64-132">Ihr globaler Administrator kann Ihnen die erforderlichen Berechtigungen erteilen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="8bf64-133">Finden des globalen Administrators</span><span class="sxs-lookup"><span data-stu-id="8bf64-133">Find your global admin</span></span>

<span data-ttu-id="8bf64-134">Es kann vorkommen, dass ein Benutzer seine Rolle ändern lassen muss oder ein neuer Benutzer eine Zuweisung zu einer bestimmten Rolle wünscht.</span><span class="sxs-lookup"><span data-stu-id="8bf64-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="8bf64-135">Wenn Sie einen globalen Administrator suchen, der Rollenänderungen vornehmen oder einem Benutzer neue Rollen zuweisen kann, wählen Sie oben rechts in Partner Center über das **Kontoeinstellungen-Symbol** den Eintrag **Benutzerverwaltung** aus, und filtern Sie nach „Globaler Administrator“. Alternativ können Sie zu **Mein Profil** navigieren, dort **Rollen und Berechtigungen** auswählen und eine Liste der verschiedenen Administratoren anzeigen, die Ihnen beim Erhöhen Ihrer Berechtigungen helfen können.</span><span class="sxs-lookup"><span data-stu-id="8bf64-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="8bf64-136">Neuer globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-136">New global admin</span></span>

<span data-ttu-id="8bf64-137">Wenn Ihr globaler Administrator aus dem Unternehmen ausscheidet und diese Aufgabe von jemand anderem übernommen wird, können Sie ein Ticket an das Azure-Team oder an das Office 365-Team senden.</span><span class="sxs-lookup"><span data-stu-id="8bf64-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="8bf64-138">Wählen Sie eine der folgenden Optionen aus, um zu erfahren, wie Sie dazu vorgehen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="8bf64-139">Neuer globaler Administrator für Azure</span><span class="sxs-lookup"><span data-stu-id="8bf64-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="8bf64-140">Neuer globaler Administrator für Office 365</span><span class="sxs-lookup"><span data-stu-id="8bf64-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="8bf64-141">Zuweisen von Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="8bf64-141">Assign user roles</span></span>

<span data-ttu-id="8bf64-142">Um im Partner Center arbeiten zu können, muss Ihnen eine Rolle zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="8bf64-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="8bf64-143">Derzeit gibt es Rollen für Azure Active Directory-Mandanten, Cloud Solution Provider (CSP) und nicht auf AAD bezogene Rollen im Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="8bf64-144">Ein einzelnes Unternehmen kann eine alle diese Rollen benötigen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="8bf64-145">Benutzer müssen in Ihrem Mandanten aufgeführt sein, um auf das Partner Center zugreifen zu können.</span><span class="sxs-lookup"><span data-stu-id="8bf64-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="8bf64-146">Rollenzuweisungen gewähren zusätzliche Zugriffsrechte.</span><span class="sxs-lookup"><span data-stu-id="8bf64-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="8bf64-147">**AAD-Mandantenrollen**:</span><span class="sxs-lookup"><span data-stu-id="8bf64-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="8bf64-148">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-148">Global admin</span></span>
- <span data-ttu-id="8bf64-149">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-149">User admin</span></span>

<span data-ttu-id="8bf64-150">**CSP-Rollen**:</span><span class="sxs-lookup"><span data-stu-id="8bf64-150">**CSP roles include**:</span></span>
- <span data-ttu-id="8bf64-151">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="8bf64-151">Admin agent</span></span>
- <span data-ttu-id="8bf64-152">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-152">Billing admin</span></span>
- <span data-ttu-id="8bf64-153">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="8bf64-153">Sales agent</span></span>
- <span data-ttu-id="8bf64-154">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="8bf64-154">Helpdesk agent</span></span>

<span data-ttu-id="8bf64-155">**Rollen für die Verwaltung der MPN-Mitgliedschaft und des Unternehmens (außerhalb von AAD)**</span><span class="sxs-lookup"><span data-stu-id="8bf64-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="8bf64-156">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-156">MPN partner admin</span></span>
- <span data-ttu-id="8bf64-157">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-157">Account admin</span></span>
- <span data-ttu-id="8bf64-158">Administrator für Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="8bf64-158">Referral admin</span></span>
- <span data-ttu-id="8bf64-159">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-159">Business profile admin</span></span>
- <span data-ttu-id="8bf64-160">Incentives-Administrator und -Benutzer</span><span class="sxs-lookup"><span data-stu-id="8bf64-160">Incentives admin and user</span></span>

<span data-ttu-id="8bf64-161">**Control Panel Vendor ist eine CSP- und keine AAD-Rolle**.</span><span class="sxs-lookup"><span data-stu-id="8bf64-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="8bf64-162">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8bf64-162">Global admin</span></span>

<span data-ttu-id="8bf64-163">**Gastbenutzer** muss Teil des AAD-Mandanten sein und eine beliebige AAD-externe Rolle haben.</span><span class="sxs-lookup"><span data-stu-id="8bf64-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="8bf64-164">Spezifische Informationen zu den Rollen und ihren Möglichkeiten finden Sie unter [Zuweisen von Benutzerberechtigungen](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8bf64-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="8bf64-165">Zuordnen des Microsoft Learn Kontos eines Benutzers im Partner Center</span><span class="sxs-lookup"><span data-stu-id="8bf64-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="8bf64-166">Damit Sie die Schulungs- und Lernpfade anzeigen können, die Ihre Benutzer für Kompetenzen verwenden, müssen sie Ihre MCP-ID ihrem Partner Center-Konto zuordnen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="8bf64-167">Wenn Sie als globaler Administrator neue Benutzer hinzufügen, müssen Sie sie daran erinnern, ihre MCP-ID ihrem Konto zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="8bf64-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="8bf64-168">Zuordnen Ihrer MCP-ID zu Ihrem Partner Center-Konto</span><span class="sxs-lookup"><span data-stu-id="8bf64-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="8bf64-169">Wähle im Partner Center-Dashboard das Symbol für **Dein Konto** in der rechten Ecke des Dashboards aus, und wähle dann **Mein Profil** aus.</span><span class="sxs-lookup"><span data-stu-id="8bf64-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="8bf64-170">Unter **Dein Learning** kannst du dein Microsoft Learning-Konto zuordnen und auch dein Microsoft-Konto mit Partner University verbinden.</span><span class="sxs-lookup"><span data-stu-id="8bf64-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8bf64-171">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="8bf64-171">Next steps</span></span>

- [<span data-ttu-id="8bf64-172">Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen</span><span class="sxs-lookup"><span data-stu-id="8bf64-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)