---
title: Erstellen von Benutzerkonten und Zuweisen von Rollen
description: Jedem Mitarbeiter muss eine Rolle zugewiesen werden, bevor er auf das Partner Center zugreifen kann. Erfahren Sie, wie Sie Benutzerkonten erstellen, Rollen zuweisen und Berechtigungen festlegen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006769"
---
# <a name="create-user-accounts"></a><span data-ttu-id="b9526-104">Erstellen Sie Benutzerkonten</span><span class="sxs-lookup"><span data-stu-id="b9526-104">Create user accounts</span></span>  

<span data-ttu-id="b9526-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="b9526-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b9526-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="b9526-106">Account admin</span></span>
- <span data-ttu-id="b9526-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b9526-107">Global admin</span></span>
- <span data-ttu-id="b9526-108">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="b9526-108">User management admin</span></span>

<span data-ttu-id="b9526-109">Erstellen Sie Benutzerkonten für Mitarbeiter, die Zugriff auf das Partner Center benötigen.</span><span class="sxs-lookup"><span data-stu-id="b9526-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="b9526-110">Diese Aufgaben müssen von einem Administrator für die Benutzerverwaltung, Kontoadministrator oder vom globalen Administrator durchgeführt werden. Dem Benutzer, der diese Aufgaben ausführt, müssen auch die AAD-Rollen (Azure Active Directory) „Benutzeradministrator“ und „Globaler Administrator“ zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="b9526-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="b9526-111">Weitere Informationen zu AAD-Rollen findest du unter [Berechtigungen für Administratorrollen in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="b9526-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="b9526-112">Neuen Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="b9526-112">Add a new user</span></span>

1. <span data-ttu-id="b9526-113">Klicken Sie im Partner Center rechts oben auf das Symbol **Einstellungen**. Wählen Sie dann **Kontoeinstellungen** und anschließend **Benutzerverwaltung** aus.</span><span class="sxs-lookup"><span data-stu-id="b9526-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="b9526-114">Wählen Sie **Benutzer hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="b9526-114">Select **Add user**.</span></span>

3. <span data-ttu-id="b9526-115">Gib den vollständigen Namen und die eindeutige E-Mail-Adresse des Benutzers ein.</span><span class="sxs-lookup"><span data-stu-id="b9526-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="b9526-116">Wählen Sie den Agent- bzw. Administratortyp, den Sie dem Benutzer zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="b9526-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="b9526-117">Partner Center-Zugriff ist rollenbasiert. So können Sie Berechtigungen zum Anpassen der Benutzeransicht zuweisen, um nur die Funktionen anzuzeigen, die der Benutzer für bestimmte Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="b9526-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="b9526-118">Wenn Benutzer eine Rollenzuweisung wünschen, finden sie die zu kontaktierenden globalen Administratoren unter **Benutzerverwaltung** durch Filtern nach „globaler Administrator“.</span><span class="sxs-lookup"><span data-stu-id="b9526-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="b9526-119">Wählen Sie **Hinzufügen** aus, um das Benutzerkonto zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="b9526-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="b9526-120">Bestätigen Sie die Details des Benutzers auf der nächsten Seite.</span><span class="sxs-lookup"><span data-stu-id="b9526-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="b9526-121">Notieren Sie sich die Anmeldeinformationen des neuen Benutzers, die auf dieser Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b9526-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="b9526-122">Achten Sie darauf, diese Informationen zu kopieren und an den neuen Benutzer zu senden, da Sie später nicht erneut darauf zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="b9526-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="b9526-123">Der Benutzer muss sich bei Partner Center mit seinem Benutzernamen und einem temporären Kennwort anmelden.</span><span class="sxs-lookup"><span data-stu-id="b9526-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="b9526-124">Wenn sich der Benutzer zum ersten Mal bei Partner Center anmeldet, wird er aufgefordert, sein Kennwort zu ändern.</span><span class="sxs-lookup"><span data-stu-id="b9526-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="b9526-125">Zuweisen von Benutzerrollen</span><span class="sxs-lookup"><span data-stu-id="b9526-125">Assign user roles</span></span>

<span data-ttu-id="b9526-126">Um im Partner Center arbeiten zu können, muss Ihnen eine Rolle zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="b9526-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="b9526-127">Derzeit gibt es Rollen für Azure Active Directory-Mandanten, Cloud Solution Provider (CSP) und nicht auf AAD bezogene Rollen im Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="b9526-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="b9526-128">Ein einzelnes Unternehmen kann eine alle diese Rollen benötigen.</span><span class="sxs-lookup"><span data-stu-id="b9526-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="b9526-129">Benutzer müssen in Ihrem Mandanten aufgeführt sein, um auf das Partner Center zugreifen zu können.</span><span class="sxs-lookup"><span data-stu-id="b9526-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="b9526-130">Rollenzuweisungen gewähren zusätzliche Zugriffsrechte.</span><span class="sxs-lookup"><span data-stu-id="b9526-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9526-131">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="b9526-131">Next steps</span></span>

- [<span data-ttu-id="b9526-132">Zuweisen von Rollen und Berechtigungen für Mitarbeiter, die im Partner Center arbeiten müssen</span><span class="sxs-lookup"><span data-stu-id="b9526-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
