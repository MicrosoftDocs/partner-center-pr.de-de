---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Jeder Mitarbeiter im Partner Center funktioniert muss, muss eine Rolle zugewiesen werden.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133900"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="51232-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="51232-104">Assign users roles and permissions</span></span>


<span data-ttu-id="51232-105">Sie haben Ihr Profil des Partners, einschließlich offizieller Name und Adresse, Informationen zum Support, Datei steuern Ausnahmen, Bankinformationen und der primäre Ansprechpartner für Ihr Unternehmen einrichten.</span><span class="sxs-lookup"><span data-stu-id="51232-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="51232-106">Nächster Schritt: erhalten Ihre Benutzer richten Sie mit Kennwörtern und Rollen, sodass sie im Partner Center mit Ihnen arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="51232-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="51232-107">Ihre Mitarbeiter arbeiten im Partner Center einrichten</span><span class="sxs-lookup"><span data-stu-id="51232-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="51232-108">Sie bestimmen die Zugriffsarten aufgeführt, die Ihre Benutzer müssen Partner Center durch die Rollen und Berechtigungen, die Sie ihnen geben.</span><span class="sxs-lookup"><span data-stu-id="51232-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="51232-109">Rollen beziehen sich auf die Programme, die, denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="51232-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="51232-110">Z. B. Wenn Ihr Unternehmen einen Cloud Solution Provider (CSP) ist, nicht nur müssen die standardmäßige Azure AD Mandanten Verwaltungsrollen z.B. globaler Administrator, allerdings benötigen Rollen spezifisch für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="51232-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="51232-111">Jedes Programm verfügt über Rollen, die speziell für sie.</span><span class="sxs-lookup"><span data-stu-id="51232-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="51232-112">Azure Active Directory (AAD) mandantenrollen enthalten globaler Administrator, Benutzeradministrator und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="51232-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="51232-113">Nicht-AAD-Rollen umfassen MPN Admin, Business-Profil-Admin, Verweis Admin, anreizprogramm Admin und anreizprogramm Benutzer.</span><span class="sxs-lookup"><span data-stu-id="51232-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="51232-114">Verwalten von kommerziellen Transaktionen im Partner Center (Azure AD und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="51232-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="51232-115">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="51232-115">**Role**</span></span>|<span data-ttu-id="51232-116">**Was sie tun können**</span><span class="sxs-lookup"><span data-stu-id="51232-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="51232-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="51232-117">Global admin</span></span>|<span data-ttu-id="51232-118">• Können auf alle Microsoft-Konto/Dienste mit vollständigen Berechtigungen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="51232-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="51232-119">• Erstellen von supporttickets im Partner Center</span><span class="sxs-lookup"><span data-stu-id="51232-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="51232-120">• Anzeigen Vereinbarungen, Preislisten und Angebote</span><span class="sxs-lookup"><span data-stu-id="51232-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="51232-121">• Anzeigen, erstellen und Verwalten von B2B-Zusammenarbeit</span><span class="sxs-lookup"><span data-stu-id="51232-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="51232-122">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="51232-122">User Admin</span></span>   | <span data-ttu-id="51232-123">• Anzeigen, erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="51232-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="51232-124">• Zeigen Sie alle aufgelisteten Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="51232-124">• View all partner profiles</span></span>
||<span data-ttu-id="51232-125">• Anzeigen, erstellen und Verwalten von B2B-Zusammenarbeit</span><span class="sxs-lookup"><span data-stu-id="51232-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="51232-126">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="51232-126">Billing admin</span></span> | <span data-ttu-id="51232-127">– Anzeigen, erstellen und Verwalten von abrechnungs-, Rechnungen und Abstimm Dateien</span><span class="sxs-lookup"><span data-stu-id="51232-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="51232-128">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="51232-128">Default user</span></span>|  <span data-ttu-id="51232-129">Mein Profil anzeigen</span><span class="sxs-lookup"><span data-stu-id="51232-129">View My profile</span></span>   |
|<span data-ttu-id="51232-130">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="51232-130">Admin agent</span></span> | <span data-ttu-id="51232-131">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="51232-131">•    Customer management</span></span>
||<span data-ttu-id="51232-132">• Hinzufügen von Geräteliste zu Partner Center <</span><span class="sxs-lookup"><span data-stu-id="51232-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="51232-133">• Erstellen und Anwenden von Profilen für Geräte</span><span class="sxs-lookup"><span data-stu-id="51232-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="51232-134">• Verwaltung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="51232-134">• Subscription management</span></span>
||<span data-ttu-id="51232-135">• Service Health und dienstanforderungen für Kunden</span><span class="sxs-lookup"><span data-stu-id="51232-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="51232-136">• Anforderung delegierte Administratorberechtigungen</span><span class="sxs-lookup"><span data-stu-id="51232-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="51232-137">• Die Preise und Angebote</span><span class="sxs-lookup"><span data-stu-id="51232-137">• View pricing and offers</span></span>
||<span data-ttu-id="51232-138">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="51232-138">• Billing</span></span>
||<span data-ttu-id="51232-139">• Im Auftrag eines Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="51232-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="51232-140">•, Registrieren Sie ein Wert hinzugefügt, reseller</span><span class="sxs-lookup"><span data-stu-id="51232-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="51232-141">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="51232-141">Sales agent</span></span> | <span data-ttu-id="51232-142">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="51232-142">•    Customer management</span></span>
||<span data-ttu-id="51232-143">• Das Partner Center Geräteliste hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="51232-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="51232-144">• Verwaltung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="51232-144">• Subscription management</span></span>
||<span data-ttu-id="51232-145">• Anzeigen-Support-tickets</span><span class="sxs-lookup"><span data-stu-id="51232-145">• View support tickets</span></span>
||<span data-ttu-id="51232-146">• Anforderung eine Beziehung mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="51232-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="51232-147">• Verwalten von kundenleads</span><span class="sxs-lookup"><span data-stu-id="51232-147">• Manage customer leads</span></span>
||<span data-ttu-id="51232-148">• Anzeigen, die Kunden-Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="51232-148">• View the customer agreement</span></span>
||<span data-ttu-id="51232-149">• Registrieren einen Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="51232-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="51232-150">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="51232-150">Helpdesk agent</span></span>| <span data-ttu-id="51232-151">• Suchen und anzeigen ein Kunden</span><span class="sxs-lookup"><span data-stu-id="51232-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="51232-152">• Kunden Bearbeiten von details</span><span class="sxs-lookup"><span data-stu-id="51232-152">• Edit customer details</span></span>
||<span data-ttu-id="51232-153">• Help Resolve-Kundenprobleme mit der Verwaltung von Abrechnung oder zum Abonnement</span><span class="sxs-lookup"><span data-stu-id="51232-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="51232-154">• Anforderung Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent zur Ausführung dieser Aufgabe für Office 365-Abonnements sein)</span><span class="sxs-lookup"><span data-stu-id="51232-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="51232-155">• Verwalten von Abonnements und Abrechnung Probleme im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent zur Ausführung dieser Aufgabe für Office 365-Abonnements sein)</span><span class="sxs-lookup"><span data-stu-id="51232-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="51232-156">Hersteller des Steuerelements Bereich (Vocabulary).</span><span class="sxs-lookup"><span data-stu-id="51232-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="51232-157">(CSP-Rolle und nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="51232-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="51232-158">CPVs entwickeln Sie apps für die Verwendung durch Partner (Cloud Solution Provider, CSP), damit sie ihre Systeme in Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="51232-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="51232-159">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="51232-159">**Role**</span></span>   |<span data-ttu-id="51232-160">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="51232-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="51232-161">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="51232-161">Global admin</span></span>| <span data-ttu-id="51232-162">Zeigen Sie an und verwalten Sie Ihr Profil CPV</span><span class="sxs-lookup"><span data-stu-id="51232-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="51232-163">Zeigen Sie an und verwalten Sie Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.</span><span class="sxs-lookup"><span data-stu-id="51232-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="51232-164">Verwalten von MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="51232-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="51232-165">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="51232-165">**Role**</span></span> | <span data-ttu-id="51232-166">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="51232-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="51232-167">Administrator für MPN-Partner</span><span class="sxs-lookup"><span data-stu-id="51232-167">MPN partner admin</span></span>|<span data-ttu-id="51232-168">•CAN hinzufügen, ohne Benutzer</span><span class="sxs-lookup"><span data-stu-id="51232-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="51232-169">• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner</span><span class="sxs-lookup"><span data-stu-id="51232-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="51232-170">• Anzeigen, die rechtlichen, Unternehmen, Unternehmen und MPN-Profile</span><span class="sxs-lookup"><span data-stu-id="51232-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="51232-171">• Details zum Benutzer und ihre Fähigkeiten-Daten</span><span class="sxs-lookup"><span data-stu-id="51232-171">• View user details and their skills data</span></span>
||<span data-ttu-id="51232-172">• Anzeigen Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="51232-172">• View competencies</span></span>
||<span data-ttu-id="51232-173">• Anzeigen und verwalten Sie die Vorteile</span><span class="sxs-lookup"><span data-stu-id="51232-173">• View and manage benefits</span></span>
||<span data-ttu-id="51232-174">• Anzeigen und erwerben von bietet MPN</span><span class="sxs-lookup"><span data-stu-id="51232-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="51232-175">• Anzeigen von MPN bietet, Bestellverlauf und Rechnungen</span><span class="sxs-lookup"><span data-stu-id="51232-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="51232-176">• Anzeigen Beitrag Partnerdaten</span><span class="sxs-lookup"><span data-stu-id="51232-176">• View partner contribution data</span></span>
||<span data-ttu-id="51232-177">• Können in den Gutschein Überprüfungstool arbeiten.</span><span class="sxs-lookup"><span data-stu-id="51232-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="51232-178">– Anzeigen von Datenanalysen für Kunden</span><span class="sxs-lookup"><span data-stu-id="51232-178">- View customer data analytics</span></span>
|<span data-ttu-id="51232-179">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="51232-179">Account admin</span></span>| <span data-ttu-id="51232-180">• Können nicht einem Mandanten Benutzer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="51232-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="51232-181">• Hinzufügen oder Löschen von Standorten</span><span class="sxs-lookup"><span data-stu-id="51232-181">• Add or delete locations</span></span>
||<span data-ttu-id="51232-182">– Verwalten von Profilen, die im Zusammenhang mit den Konten, die, denen Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="51232-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="51232-183">• Zuweisen von Rollen für Benutzer im Mandanten nicht AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="51232-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="51232-184">• Standorte in Programmen zu registrieren</span><span class="sxs-lookup"><span data-stu-id="51232-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="51232-185">Gastbenutzer (muss für den AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="51232-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="51232-186">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="51232-186">**Guest user**</span></span>   | <span data-ttu-id="51232-187">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="51232-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="51232-188">Administrator für MPN-Partner</span><span class="sxs-lookup"><span data-stu-id="51232-188">MPN partner admin</span></span>|
||<span data-ttu-id="51232-189">Konten-Administrator</span><span class="sxs-lookup"><span data-stu-id="51232-189">Accounts admin</span></span>|
||<span data-ttu-id="51232-190">Incentives-Administrator</span><span class="sxs-lookup"><span data-stu-id="51232-190">Incentives admin</span></span>|
||<span data-ttu-id="51232-191">Administrator für das Unternehmensprofil</span><span class="sxs-lookup"><span data-stu-id="51232-191">Business profile admin</span></span>|
||<span data-ttu-id="51232-192">Verweise auf admin</span><span class="sxs-lookup"><span data-stu-id="51232-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="51232-193">Verwalten von verweisen (nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="51232-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="51232-194">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="51232-194">**Role**</span></span>|<span data-ttu-id="51232-195">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="51232-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="51232-196">Verweise auf admin</span><span class="sxs-lookup"><span data-stu-id="51232-196">Referrals admin</span></span>       |<span data-ttu-id="51232-197">• Anzeigen, erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="51232-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="51232-198">• Empfangen und Verwalten von verweisen</span><span class="sxs-lookup"><span data-stu-id="51232-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="51232-199">• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner</span><span class="sxs-lookup"><span data-stu-id="51232-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="51232-200">Administrator für das Unternehmensprofil</span><span class="sxs-lookup"><span data-stu-id="51232-200">Business profile admin</span></span>   |<span data-ttu-id="51232-201">• Anzeigen, erstellen und Verwalten von Business-Profil</span><span class="sxs-lookup"><span data-stu-id="51232-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="51232-202">• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner</span><span class="sxs-lookup"><span data-stu-id="51232-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="51232-203">Verwalten von Incentives (nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="51232-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="51232-204">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="51232-204">**Role**</span></span> | <span data-ttu-id="51232-205">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="51232-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="51232-206">Incentives-Administrator</span><span class="sxs-lookup"><span data-stu-id="51232-206">Incentives admin</span></span>|<span data-ttu-id="51232-207">• Initiiert und Anreize verwaltet</span><span class="sxs-lookup"><span data-stu-id="51232-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="51232-208">• Anzeigen und bearbeiten alle Aspekte der Anreize für Programme</span><span class="sxs-lookup"><span data-stu-id="51232-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="51232-209">• Anzeigen und bearbeiten die Bank- und Steuerdaten-details</span><span class="sxs-lookup"><span data-stu-id="51232-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="51232-210">• Anzeigen Rebate und Co-op-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="51232-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="51232-211">• Unterstützung des Zugriffs</span><span class="sxs-lookup"><span data-stu-id="51232-211">• Access support</span></span>
||<span data-ttu-id="51232-212">• Im Fall von streitigkeiten Anreize für Zahlungen</span><span class="sxs-lookup"><span data-stu-id="51232-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="51232-213">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="51232-213">Incentives user</span></span>|<span data-ttu-id="51232-214">• Können Incentives sammeln, wenn Programme anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="51232-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="51232-215">• Anzeigen können, und starten Incentives sammeln, wenn Ansprüche</span><span class="sxs-lookup"><span data-stu-id="51232-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="51232-216">• Anzeigen Rebate und Co-op-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="51232-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="51232-217">• Anzeigen Rebate und Co-op-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="51232-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="51232-218">• Unterstützung des Zugriffs</span><span class="sxs-lookup"><span data-stu-id="51232-218">• Access support</span></span>












