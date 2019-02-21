---
title: Weisen Sie Benutzer Rollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Alle Mitarbeiter, die im Partner Center arbeiten muss eine Rolle zugewiesen werden.
author: labrenne
ms.author: labrenne
keywords: Rollen, Berechtigungen, Admin-agent
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086728"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="8e4c3-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="8e4c3-104">Assign users roles and permissions</span></span>


<span data-ttu-id="8e4c3-105">Sie haben Ihr Partnerprofil, einschließlich vollständiger Name und Adresse, Supportinformationen, steuerbefreiungen, Bankinformationen und der Hauptansprechpartner für Ihr Unternehmen einrichten.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="8e4c3-106">Nächster Schritt: fordern Sie die Benutzer einrichten mit Kennwörtern und Rollen, sodass sie im Partner Center mit Ihnen arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="8e4c3-107">Richten Sie Ihre Mitarbeiter im Partner Center arbeiten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="8e4c3-108">Sie bestimmen die Art des Zugriffs, die Ihre Benutzer über Partner Center die Rollen und Berechtigungen, die Sie ihnen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="8e4c3-109">Rollen beziehen sich auf die Programme, die, denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="8e4c3-110">Beispielsweise, wenn Ihr Unternehmen ein Unternehmen Cloud Solution Provider (CSP) ist, nicht erhalten Sie nur das Azure AD-standard Mandanten-Management-Funktionen wie z. B. globaler Administrator, aber benötigen Rollen speziell für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="8e4c3-111">Jedes Programm verfügt über Funktionen, die speziell für sie.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="8e4c3-112">Azure Active Directory (AAD) Mandanten Rollen enthalten globaler Administrator, Admin Benutzer und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="8e4c3-113">Nicht-AAD Rollen enthalten MPN Administrator, Administrator für das Unternehmensprofil, Administrator für Empfehlungen, Incentives-Administrator und Incentive-Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="8e4c3-114">Verwalten von kommerziellen Transaktionen im Partner Center (Azure AD und CSP Rollen)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|**<span data-ttu-id="8e4c3-115">Rolle</span><span class="sxs-lookup"><span data-stu-id="8e4c3-115">Role</span></span>**|**<span data-ttu-id="8e4c3-116">Berechtigungen dieser Rolle</span><span class="sxs-lookup"><span data-stu-id="8e4c3-116">What they can do</span></span>**|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="8e4c3-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8e4c3-117">Global admin</span></span>|<span data-ttu-id="8e4c3-118">• Können alle Microsoft-Konten/-Dienste mit allen Berechtigungen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="8e4c3-119">• Supportanfragen für Partner Center erstellen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8e4c3-120">• Ansicht Vereinbarungen, Preislisten und Angebote</span><span class="sxs-lookup"><span data-stu-id="8e4c3-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="8e4c3-121">• Anzeigen, erstellen und Verwalten von Partnerbenutzer</span><span class="sxs-lookup"><span data-stu-id="8e4c3-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="8e4c3-122">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="8e4c3-122">User Admin</span></span>   | <span data-ttu-id="8e4c3-123">• Anzeigen, erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="8e4c3-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="8e4c3-124">• Alle Partnerprofile anzeigen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-124">• View all partner profiles</span></span>
||<span data-ttu-id="8e4c3-125">• Anzeigen, erstellen und Verwalten von Partnerbenutzer</span><span class="sxs-lookup"><span data-stu-id="8e4c3-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="8e4c3-126">Standard-Benutzer</span><span class="sxs-lookup"><span data-stu-id="8e4c3-126">Default user</span></span>|  <span data-ttu-id="8e4c3-127">Mein Profil anzeigen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-127">View My profile</span></span>   |
|<span data-ttu-id="8e4c3-128">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="8e4c3-128">Admin agent</span></span> | <span data-ttu-id="8e4c3-129">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-129">•    Customer management</span></span>
||<span data-ttu-id="8e4c3-130">• Liste der Geräte, die Partner Center< hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="8e4c3-131">• Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="8e4c3-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="8e4c3-132">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-132">• Subscription management</span></span>
||<span data-ttu-id="8e4c3-133">• Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="8e4c3-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="8e4c3-134">• Anforderung delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="8e4c3-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="8e4c3-135">• Ansicht Preise und Angebote</span><span class="sxs-lookup"><span data-stu-id="8e4c3-135">• View pricing and offers</span></span>
||<span data-ttu-id="8e4c3-136">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-136">• Billing</span></span>
||<span data-ttu-id="8e4c3-137">• Im Auftrag eines Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="8e4c3-138">• Registrieren einen Wert Vertragshändler</span><span class="sxs-lookup"><span data-stu-id="8e4c3-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="8e4c3-139">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="8e4c3-139">Sales agent</span></span> | <span data-ttu-id="8e4c3-140">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-140">•    Customer management</span></span>
||<span data-ttu-id="8e4c3-141">• Geräteliste zum Partner Center hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="8e4c3-142">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-142">• Subscription management</span></span>
||<span data-ttu-id="8e4c3-143">• Ansicht Supportanfragen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-143">• View support tickets</span></span>
||<span data-ttu-id="8e4c3-144">• Anfordern einer Beziehung mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="8e4c3-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="8e4c3-145">• Potenzielle Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-145">• Manage customer leads</span></span>
||<span data-ttu-id="8e4c3-146">• Ansicht Kundenvertrag</span><span class="sxs-lookup"><span data-stu-id="8e4c3-146">• View the customer agreement</span></span>
||<span data-ttu-id="8e4c3-147">• Registrieren einen Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="8e4c3-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="8e4c3-148">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="8e4c3-148">Helpdesk agent</span></span>| <span data-ttu-id="8e4c3-149">• Suchen und anzeigen ein Kunden</span><span class="sxs-lookup"><span data-stu-id="8e4c3-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="8e4c3-150">• Bearbeiten Kundendetails</span><span class="sxs-lookup"><span data-stu-id="8e4c3-150">• Edit customer details</span></span>
||<span data-ttu-id="8e4c3-151">• Hilfe Resolve Kunden bei Problemen mit Abrechnung oder der abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="8e4c3-152">• Anforderung Support im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office 365-Abonnements sein)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="8e4c3-153">• Verwalten von Abonnements und Diensten im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office 365-Abonnements sein)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="8e4c3-154">Control Panel-Anbieter (CPV).</span><span class="sxs-lookup"><span data-stu-id="8e4c3-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="8e4c3-155">(CSP-Rolle und die nicht-AAD)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="8e4c3-156">CPVs Entwickeln von apps für die Verwendung von Cloud Solution Provider (CSP) Partnern setzen, um ihre Systeme mit Partner Center-APIs zu integrieren.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|**<span data-ttu-id="8e4c3-157">Rolle</span><span class="sxs-lookup"><span data-stu-id="8e4c3-157">Role</span></span>**   |**<span data-ttu-id="8e4c3-158">Was Sie tun können</span><span class="sxs-lookup"><span data-stu-id="8e4c3-158">What you can do</span></span>**|
|------------------------------|:----------------------------|
|<span data-ttu-id="8e4c3-159">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8e4c3-159">Global admin</span></span>| <span data-ttu-id="8e4c3-160">Zeigen Sie an und verwalten Sie Ihr Profil CPV</span><span class="sxs-lookup"><span data-stu-id="8e4c3-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="8e4c3-161">Zeigen Sie an und verwalten Sie alle Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="8e4c3-162">Verwalten von MPN-Mitgliedschaft und Ihr Unternehmen (nicht-AAD Rollen)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|**<span data-ttu-id="8e4c3-163">Rolle</span><span class="sxs-lookup"><span data-stu-id="8e4c3-163">Role</span></span>** | **<span data-ttu-id="8e4c3-164">Was Sie tun können</span><span class="sxs-lookup"><span data-stu-id="8e4c3-164">What you can do</span></span>**|
|----------------------------|:----------------------------|
|<span data-ttu-id="8e4c3-165">MPN-Administrator</span><span class="sxs-lookup"><span data-stu-id="8e4c3-165">MPN admin</span></span>|<span data-ttu-id="8e4c3-166">•CAN nicht-Mandanten Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="8e4c3-167">• Anzeigen, erstellen und Verwalten von Serviceanfragen der partner</span><span class="sxs-lookup"><span data-stu-id="8e4c3-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="8e4c3-168">• Ansicht rechtliche, Organisation, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="8e4c3-169">• Ansicht Benutzerdetails Daten und Fähigkeiten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-169">• View user details and their skills data</span></span>
||<span data-ttu-id="8e4c3-170">• Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-170">• View competencies</span></span>
||<span data-ttu-id="8e4c3-171">• Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-171">• View and manage benefits</span></span>
||<span data-ttu-id="8e4c3-172">• Anzeigen und kaufen Sie MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="8e4c3-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="8e4c3-173">Rechnungen und Bestellverlauf • Ansicht MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="8e4c3-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="8e4c3-174">• Können Partner Beitrag Daten anzeigen.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-174">• Can view partner contribution data</span></span>
||<span data-ttu-id="8e4c3-175">• Können im Beleg Überprüfung Tool arbeiten.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-175">• Can work in the Voucher Validation tool</span></span>|
|<span data-ttu-id="8e4c3-176">Administratorkonto</span><span class="sxs-lookup"><span data-stu-id="8e4c3-176">Account admin</span></span>| <span data-ttu-id="8e4c3-177">• Können Benutzer nicht-Mandanten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-177">•   Can add non-tenant users</span></span>
||<span data-ttu-id="8e4c3-178">• Hinzufügen oder Löschen von Speicherorte</span><span class="sxs-lookup"><span data-stu-id="8e4c3-178">• Add or delete locations</span></span>
||<span data-ttu-id="8e4c3-179">-Verwalten Sie Profile, die im Zusammenhang mit der Konten, die Sie Administrator</span><span class="sxs-lookup"><span data-stu-id="8e4c3-179">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="8e4c3-180">• Zuweisung von Rollen für Benutzer im Mandanten nicht AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-180">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="8e4c3-181">• Speicherorte in Programme registrieren</span><span class="sxs-lookup"><span data-stu-id="8e4c3-181">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="8e4c3-182">Verwalten von Empfehlungen (nicht-AAD Rollen)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-182">Manage referrals (non-AAD roles)</span></span>

|**<span data-ttu-id="8e4c3-183">Rolle</span><span class="sxs-lookup"><span data-stu-id="8e4c3-183">Role</span></span>**|**<span data-ttu-id="8e4c3-184">Was Sie tun können</span><span class="sxs-lookup"><span data-stu-id="8e4c3-184">What you can do</span></span>**|
|-----------------------------|:------------------------|
|<span data-ttu-id="8e4c3-185">Verweise auf admin</span><span class="sxs-lookup"><span data-stu-id="8e4c3-185">Referrals admin</span></span>       |<span data-ttu-id="8e4c3-186">• Anzeigen, erstellen und Verwalten von Unternehmensprofilen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-186">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="8e4c3-187">• Sie erhalten und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-187">• Receive and manage referrals</span></span>
||<span data-ttu-id="8e4c3-188">• Anzeigen, erstellen und Verwalten von Serviceanfragen der partner</span><span class="sxs-lookup"><span data-stu-id="8e4c3-188">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="8e4c3-189">Administrator für das Unternehmensprofil</span><span class="sxs-lookup"><span data-stu-id="8e4c3-189">Business profile admin</span></span>   |<span data-ttu-id="8e4c3-190">•View, erstellen und Verwalten des Unternehmensprofils</span><span class="sxs-lookup"><span data-stu-id="8e4c3-190">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="8e4c3-191">• Anzeigen, erstellen und Verwalten von Serviceanfragen der partner</span><span class="sxs-lookup"><span data-stu-id="8e4c3-191">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="8e4c3-192">Verwalten von Incentives (nicht-AAD Rollen)</span><span class="sxs-lookup"><span data-stu-id="8e4c3-192">Manage Incentives  (non-AAD roles)</span></span>

|**<span data-ttu-id="8e4c3-193">Rolle</span><span class="sxs-lookup"><span data-stu-id="8e4c3-193">Role</span></span>** | **<span data-ttu-id="8e4c3-194">Was Sie tun können</span><span class="sxs-lookup"><span data-stu-id="8e4c3-194">What you can do</span></span>**|
|------------------------------|:-------------------------|
|<span data-ttu-id="8e4c3-195">Anreizadministrator</span><span class="sxs-lookup"><span data-stu-id="8e4c3-195">Incentives admin</span></span>|<span data-ttu-id="8e4c3-196">• Initiiert und Incentives verwaltet</span><span class="sxs-lookup"><span data-stu-id="8e4c3-196">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="8e4c3-197">• Kann anzeigen und bearbeiten alle Aspekte der Incentives-Programme</span><span class="sxs-lookup"><span data-stu-id="8e4c3-197">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="8e4c3-198">• Kann anzeigen und Bearbeiten von Bank-und Steuerinformationen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-198">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="8e4c3-199">• Ansicht und gemeinschaftliche Einnahmen erhalten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-199">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8e4c3-200">• Zugriff-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-200">• Access support</span></span>
||<span data-ttu-id="8e4c3-201">• Fall Incentive-Zahlungen</span><span class="sxs-lookup"><span data-stu-id="8e4c3-201">• Dispute incentives payments</span></span>|
|<span data-ttu-id="8e4c3-202">Anreizbenutzer</span><span class="sxs-lookup"><span data-stu-id="8e4c3-202">Incentives user</span></span>|<span data-ttu-id="8e4c3-203">• Können Anreizprogramme anzeigen.</span><span class="sxs-lookup"><span data-stu-id="8e4c3-203">•  Can view incentives programs</span></span>
||<span data-ttu-id="8e4c3-204">• Kann anzeigen und Initiieren eines incentiveanspruchs</span><span class="sxs-lookup"><span data-stu-id="8e4c3-204">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="8e4c3-205">• Ansicht und gemeinschaftliche Einnahmen erhalten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-205">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8e4c3-206">• Ansicht und gemeinschaftliche Einnahmen erhalten</span><span class="sxs-lookup"><span data-stu-id="8e4c3-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8e4c3-207">• Zugriff-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="8e4c3-207">• Access support</span></span>












