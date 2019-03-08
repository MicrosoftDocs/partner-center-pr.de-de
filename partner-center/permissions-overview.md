---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Jeder Mitarbeiter im Partner Center funktioniert muss, muss eine Rolle zugewiesen werden.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587743"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="fe75b-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="fe75b-104">Assign users roles and permissions</span></span>


<span data-ttu-id="fe75b-105">Sie haben Ihr Profil des Partners, einschließlich offizieller Name und Adresse, Informationen zum Support, Datei steuern Ausnahmen, Bankinformationen und der primäre Ansprechpartner für Ihr Unternehmen einrichten.</span><span class="sxs-lookup"><span data-stu-id="fe75b-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="fe75b-106">Nächster Schritt: erhalten Ihre Benutzer richten Sie mit Kennwörtern und Rollen, sodass sie im Partner Center mit Ihnen arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="fe75b-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="fe75b-107">Ihre Mitarbeiter arbeiten im Partner Center einrichten</span><span class="sxs-lookup"><span data-stu-id="fe75b-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="fe75b-108">Sie bestimmen die Zugriffsarten aufgeführt, die Ihre Benutzer müssen Partner Center durch die Rollen und Berechtigungen, die Sie ihnen geben.</span><span class="sxs-lookup"><span data-stu-id="fe75b-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="fe75b-109">Rollen beziehen sich auf die Programme, die, denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="fe75b-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="fe75b-110">Z. B. Wenn Ihr Unternehmen einen Cloud Solution Provider (CSP) ist, nicht nur müssen die standardmäßige Azure AD Mandanten Verwaltungsrollen z.B. globaler Administrator, allerdings benötigen Rollen spezifisch für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="fe75b-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="fe75b-111">Jedes Programm verfügt über Rollen, die speziell für sie.</span><span class="sxs-lookup"><span data-stu-id="fe75b-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="fe75b-112">Azure Active Directory (AAD) mandantenrollen enthalten globaler Administrator, Benutzeradministrator und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="fe75b-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="fe75b-113">Nicht-AAD-Rollen umfassen MPN Admin, Business-Profil-Admin, Verweis Admin, anreizprogramm Admin und anreizprogramm Benutzer.</span><span class="sxs-lookup"><span data-stu-id="fe75b-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="fe75b-114">Verwalten von kommerziellen Transaktionen im Partner Center (Azure AD und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="fe75b-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="fe75b-115">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="fe75b-115">**Role**</span></span>|<span data-ttu-id="fe75b-116">**Was sie tun können**</span><span class="sxs-lookup"><span data-stu-id="fe75b-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="fe75b-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="fe75b-117">Global admin</span></span>|<span data-ttu-id="fe75b-118">• Können auf alle Microsoft-Konto/Dienste mit vollständigen Berechtigungen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="fe75b-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="fe75b-119">• Erstellen von supporttickets im Partner Center</span><span class="sxs-lookup"><span data-stu-id="fe75b-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="fe75b-120">• Anzeigen Vereinbarungen, Preislisten und Angebote</span><span class="sxs-lookup"><span data-stu-id="fe75b-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="fe75b-121">• Anzeigen, erstellen und Verwalten von B2B-Zusammenarbeit</span><span class="sxs-lookup"><span data-stu-id="fe75b-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="fe75b-122">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="fe75b-122">User Admin</span></span>   | <span data-ttu-id="fe75b-123">• Anzeigen, erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="fe75b-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="fe75b-124">• Zeigen Sie alle aufgelisteten Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="fe75b-124">• View all partner profiles</span></span>
||<span data-ttu-id="fe75b-125">• Anzeigen, erstellen und Verwalten von B2B-Zusammenarbeit</span><span class="sxs-lookup"><span data-stu-id="fe75b-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="fe75b-126">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="fe75b-126">Default user</span></span>|  <span data-ttu-id="fe75b-127">Mein Profil anzeigen</span><span class="sxs-lookup"><span data-stu-id="fe75b-127">View My profile</span></span>   |
|<span data-ttu-id="fe75b-128">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="fe75b-128">Admin agent</span></span> | <span data-ttu-id="fe75b-129">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="fe75b-129">•    Customer management</span></span>
||<span data-ttu-id="fe75b-130">• Hinzufügen von Geräteliste zu Partner Center <</span><span class="sxs-lookup"><span data-stu-id="fe75b-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="fe75b-131">• Erstellen und Anwenden von Profilen für Geräte</span><span class="sxs-lookup"><span data-stu-id="fe75b-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="fe75b-132">• Verwaltung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="fe75b-132">• Subscription management</span></span>
||<span data-ttu-id="fe75b-133">• Service Health und dienstanforderungen für Kunden</span><span class="sxs-lookup"><span data-stu-id="fe75b-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="fe75b-134">• Anforderung delegierte Administratorberechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe75b-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="fe75b-135">• Die Preise und Angebote</span><span class="sxs-lookup"><span data-stu-id="fe75b-135">• View pricing and offers</span></span>
||<span data-ttu-id="fe75b-136">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="fe75b-136">• Billing</span></span>
||<span data-ttu-id="fe75b-137">• Im Auftrag eines Kunden verwalten</span><span class="sxs-lookup"><span data-stu-id="fe75b-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="fe75b-138">•, Registrieren Sie ein Wert hinzugefügt, reseller</span><span class="sxs-lookup"><span data-stu-id="fe75b-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="fe75b-139">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="fe75b-139">Sales agent</span></span> | <span data-ttu-id="fe75b-140">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="fe75b-140">•    Customer management</span></span>
||<span data-ttu-id="fe75b-141">• Das Partner Center Geräteliste hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fe75b-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="fe75b-142">• Verwaltung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="fe75b-142">• Subscription management</span></span>
||<span data-ttu-id="fe75b-143">• Anzeigen-Support-tickets</span><span class="sxs-lookup"><span data-stu-id="fe75b-143">• View support tickets</span></span>
||<span data-ttu-id="fe75b-144">• Anforderung eine Beziehung mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="fe75b-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="fe75b-145">• Verwalten von kundenleads</span><span class="sxs-lookup"><span data-stu-id="fe75b-145">• Manage customer leads</span></span>
||<span data-ttu-id="fe75b-146">• Anzeigen, die Kunden-Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="fe75b-146">• View the customer agreement</span></span>
||<span data-ttu-id="fe75b-147">• Registrieren einen Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="fe75b-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="fe75b-148">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="fe75b-148">Helpdesk agent</span></span>| <span data-ttu-id="fe75b-149">• Suchen und anzeigen ein Kunden</span><span class="sxs-lookup"><span data-stu-id="fe75b-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="fe75b-150">• Kunden Bearbeiten von details</span><span class="sxs-lookup"><span data-stu-id="fe75b-150">• Edit customer details</span></span>
||<span data-ttu-id="fe75b-151">• Help Resolve-Kundenprobleme mit der Verwaltung von Abrechnung oder zum Abonnement</span><span class="sxs-lookup"><span data-stu-id="fe75b-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="fe75b-152">• Anforderung Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent zur Ausführung dieser Aufgabe für Office 365-Abonnements sein)</span><span class="sxs-lookup"><span data-stu-id="fe75b-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="fe75b-153">• Verwalten von Abonnements und Abrechnung Probleme im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent zur Ausführung dieser Aufgabe für Office 365-Abonnements sein)</span><span class="sxs-lookup"><span data-stu-id="fe75b-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="fe75b-154">Hersteller des Steuerelements Bereich (Vocabulary).</span><span class="sxs-lookup"><span data-stu-id="fe75b-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="fe75b-155">(CSP-Rolle und nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="fe75b-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="fe75b-156">CPVs entwickeln Sie apps für die Verwendung durch Partner (Cloud Solution Provider, CSP), damit sie ihre Systeme in Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="fe75b-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="fe75b-157">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="fe75b-157">**Role**</span></span>   |<span data-ttu-id="fe75b-158">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="fe75b-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="fe75b-159">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="fe75b-159">Global admin</span></span>| <span data-ttu-id="fe75b-160">Zeigen Sie an und verwalten Sie Ihr Profil CPV</span><span class="sxs-lookup"><span data-stu-id="fe75b-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="fe75b-161">Zeigen Sie an und verwalten Sie Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.</span><span class="sxs-lookup"><span data-stu-id="fe75b-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="fe75b-162">Verwalten von MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="fe75b-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="fe75b-163">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="fe75b-163">**Role**</span></span> | <span data-ttu-id="fe75b-164">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="fe75b-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="fe75b-165">Administrator für MPN-Partner</span><span class="sxs-lookup"><span data-stu-id="fe75b-165">MPN partner admin</span></span>|<span data-ttu-id="fe75b-166">•CAN hinzufügen, ohne Benutzer</span><span class="sxs-lookup"><span data-stu-id="fe75b-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="fe75b-167">• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner</span><span class="sxs-lookup"><span data-stu-id="fe75b-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="fe75b-168">• Anzeigen, die rechtlichen, Unternehmen, Unternehmen und MPN-Profile</span><span class="sxs-lookup"><span data-stu-id="fe75b-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="fe75b-169">• Details zum Benutzer und ihre Fähigkeiten-Daten</span><span class="sxs-lookup"><span data-stu-id="fe75b-169">• View user details and their skills data</span></span>
||<span data-ttu-id="fe75b-170">• Anzeigen Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="fe75b-170">• View competencies</span></span>
||<span data-ttu-id="fe75b-171">• Anzeigen und verwalten Sie die Vorteile</span><span class="sxs-lookup"><span data-stu-id="fe75b-171">• View and manage benefits</span></span>
||<span data-ttu-id="fe75b-172">• Anzeigen und erwerben von bietet MPN</span><span class="sxs-lookup"><span data-stu-id="fe75b-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="fe75b-173">• Anzeigen von MPN bietet, Bestellverlauf und Rechnungen</span><span class="sxs-lookup"><span data-stu-id="fe75b-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="fe75b-174">• Anzeigen Beitrag Partnerdaten</span><span class="sxs-lookup"><span data-stu-id="fe75b-174">• View partner contribution data</span></span>
||<span data-ttu-id="fe75b-175">• Können in den Gutschein Überprüfungstool arbeiten.</span><span class="sxs-lookup"><span data-stu-id="fe75b-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="fe75b-176">– Anzeigen von Datenanalysen für Kunden</span><span class="sxs-lookup"><span data-stu-id="fe75b-176">- View customer data analytics</span></span>
|<span data-ttu-id="fe75b-177">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="fe75b-177">Account admin</span></span>| <span data-ttu-id="fe75b-178">• Können nicht einem Mandanten Benutzer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="fe75b-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="fe75b-179">• Hinzufügen oder Löschen von Standorten</span><span class="sxs-lookup"><span data-stu-id="fe75b-179">• Add or delete locations</span></span>
||<span data-ttu-id="fe75b-180">– Verwalten von Profilen, die im Zusammenhang mit den Konten, die, denen Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="fe75b-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="fe75b-181">• Zuweisen von Rollen für Benutzer im Mandanten nicht AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="fe75b-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="fe75b-182">• Standorte in Programmen zu registrieren</span><span class="sxs-lookup"><span data-stu-id="fe75b-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="fe75b-183">Verwalten von verweisen (nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="fe75b-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="fe75b-184">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="fe75b-184">**Role**</span></span>|<span data-ttu-id="fe75b-185">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="fe75b-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="fe75b-186">Verweise auf admin</span><span class="sxs-lookup"><span data-stu-id="fe75b-186">Referrals admin</span></span>       |<span data-ttu-id="fe75b-187">• Anzeigen, erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="fe75b-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="fe75b-188">• Empfangen und Verwalten von verweisen</span><span class="sxs-lookup"><span data-stu-id="fe75b-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="fe75b-189">• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner</span><span class="sxs-lookup"><span data-stu-id="fe75b-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="fe75b-190">Administrator für das Unternehmensprofil</span><span class="sxs-lookup"><span data-stu-id="fe75b-190">Business profile admin</span></span>   |<span data-ttu-id="fe75b-191">• Anzeigen, erstellen und Verwalten von Business-Profil</span><span class="sxs-lookup"><span data-stu-id="fe75b-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="fe75b-192">• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner</span><span class="sxs-lookup"><span data-stu-id="fe75b-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="fe75b-193">Verwalten von Incentives (nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="fe75b-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="fe75b-194">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="fe75b-194">**Role**</span></span> | <span data-ttu-id="fe75b-195">**Was Sie tun können**</span><span class="sxs-lookup"><span data-stu-id="fe75b-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="fe75b-196">Incentives-Administrator</span><span class="sxs-lookup"><span data-stu-id="fe75b-196">Incentives admin</span></span>|<span data-ttu-id="fe75b-197">• Initiiert und Anreize verwaltet</span><span class="sxs-lookup"><span data-stu-id="fe75b-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="fe75b-198">• Anzeigen und bearbeiten alle Aspekte der Anreize für Programme</span><span class="sxs-lookup"><span data-stu-id="fe75b-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="fe75b-199">• Anzeigen und bearbeiten die Bank- und Steuerdaten-details</span><span class="sxs-lookup"><span data-stu-id="fe75b-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="fe75b-200">• Anzeigen Rebate und Co-op-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="fe75b-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="fe75b-201">• Unterstützung des Zugriffs</span><span class="sxs-lookup"><span data-stu-id="fe75b-201">• Access support</span></span>
||<span data-ttu-id="fe75b-202">• Im Fall von streitigkeiten Anreize für Zahlungen</span><span class="sxs-lookup"><span data-stu-id="fe75b-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="fe75b-203">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="fe75b-203">Incentives user</span></span>|<span data-ttu-id="fe75b-204">• Können Incentives sammeln, wenn Programme anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="fe75b-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="fe75b-205">• Anzeigen können, und starten Incentives sammeln, wenn Ansprüche</span><span class="sxs-lookup"><span data-stu-id="fe75b-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="fe75b-206">• Anzeigen Rebate und Co-op-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="fe75b-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="fe75b-207">• Anzeigen Rebate und Co-op-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="fe75b-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="fe75b-208">• Unterstützung des Zugriffs</span><span class="sxs-lookup"><span data-stu-id="fe75b-208">• Access support</span></span>












