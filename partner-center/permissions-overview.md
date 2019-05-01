---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Jedem Mitarbeiter, der im Partner Center arbeitet, muss eine Rolle zugewiesen werden.
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
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="c3bc5-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-104">Assign users roles and permissions</span></span>


<span data-ttu-id="c3bc5-105">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c3bc5-106">Nächster Schritt: Einrichten der Benutzer mit Kennwörtern und Rollen, damit sie mit Ihnen gemeinsam im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c3bc5-107">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="c3bc5-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c3bc5-108">Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c3bc5-109">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c3bc5-110">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c3bc5-111">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c3bc5-112">AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c3bc5-113">Zu den Nicht-AAD-Rollen gehören MPN-Administrator, Geschäftsprofiladministrator, Empfehlungsadministrator, Incentiveadministrator und Incentivebenutzer.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c3bc5-114">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c3bc5-115">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-115">**Role**</span></span>|<span data-ttu-id="c3bc5-116">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="c3bc5-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-117">Global admin</span></span>|<span data-ttu-id="c3bc5-118">• Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="c3bc5-119">• Erstellen von Supportanfragen für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="c3bc5-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c3bc5-120">• Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="c3bc5-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c3bc5-121">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="c3bc5-122">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-122">User Admin</span></span>   | <span data-ttu-id="c3bc5-123">• Anzeigen, Erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="c3bc5-124">• Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="c3bc5-124">• View all partner profiles</span></span>
||<span data-ttu-id="c3bc5-125">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="c3bc5-126">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-126">Billing admin</span></span> | <span data-ttu-id="c3bc5-127">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="c3bc5-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="c3bc5-128">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="c3bc5-128">Default user</span></span>|  <span data-ttu-id="c3bc5-129">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="c3bc5-129">View My profile</span></span>   |
|<span data-ttu-id="c3bc5-130">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="c3bc5-130">Admin agent</span></span> | <span data-ttu-id="c3bc5-131">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="c3bc5-131">•    Customer management</span></span>
||<span data-ttu-id="c3bc5-132">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="c3bc5-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="c3bc5-133">• Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="c3bc5-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="c3bc5-134">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="c3bc5-134">• Subscription management</span></span>
||<span data-ttu-id="c3bc5-135">• Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="c3bc5-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="c3bc5-136">• Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="c3bc5-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="c3bc5-137">• Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="c3bc5-137">• View pricing and offers</span></span>
||<span data-ttu-id="c3bc5-138">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="c3bc5-138">• Billing</span></span>
||<span data-ttu-id="c3bc5-139">• Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="c3bc5-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="c3bc5-140">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="c3bc5-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="c3bc5-141">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="c3bc5-141">Sales agent</span></span> | <span data-ttu-id="c3bc5-142">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="c3bc5-142">•    Customer management</span></span>
||<span data-ttu-id="c3bc5-143">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="c3bc5-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="c3bc5-144">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="c3bc5-144">• Subscription management</span></span>
||<span data-ttu-id="c3bc5-145">• Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="c3bc5-145">• View support tickets</span></span>
||<span data-ttu-id="c3bc5-146">• Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="c3bc5-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="c3bc5-147">• Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="c3bc5-147">• Manage customer leads</span></span>
||<span data-ttu-id="c3bc5-148">• Anzeigen des Kundenvertrags</span><span class="sxs-lookup"><span data-stu-id="c3bc5-148">• View the customer agreement</span></span>
||<span data-ttu-id="c3bc5-149">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="c3bc5-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="c3bc5-150">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="c3bc5-150">Helpdesk agent</span></span>| <span data-ttu-id="c3bc5-151">• Suchen nach und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="c3bc5-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="c3bc5-152">• Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="c3bc5-152">• Edit customer details</span></span>
||<span data-ttu-id="c3bc5-153">• Unterstützten von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="c3bc5-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c3bc5-154">• Anfordern von Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="c3bc5-155">• Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="c3bc5-156">CPV (Control Panel Vendor).</span><span class="sxs-lookup"><span data-stu-id="c3bc5-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c3bc5-157">(CSP-Rolle und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="c3bc5-158">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="c3bc5-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c3bc5-159">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-159">**Role**</span></span>   |<span data-ttu-id="c3bc5-160">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="c3bc5-161">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-161">Global admin</span></span>| <span data-ttu-id="c3bc5-162">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="c3bc5-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="c3bc5-163">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="c3bc5-164">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (Nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="c3bc5-165">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-165">**Role**</span></span> | <span data-ttu-id="c3bc5-166">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="c3bc5-167">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-167">MPN partner admin</span></span>|<span data-ttu-id="c3bc5-168">• Hinzufügen von Nicht-Mandantenbenutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="c3bc5-169">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="c3bc5-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="c3bc5-170">• Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="c3bc5-171">• Anzeigen der Daten und Fähigkeiten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-171">• View user details and their skills data</span></span>
||<span data-ttu-id="c3bc5-172">• Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-172">• View competencies</span></span>
||<span data-ttu-id="c3bc5-173">• Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-173">• View and manage benefits</span></span>
||<span data-ttu-id="c3bc5-174">• Anzeigen und Kaufen von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="c3bc5-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="c3bc5-175">• Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="c3bc5-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c3bc5-176">• Anzeigen von Partnerbeitragsdaten</span><span class="sxs-lookup"><span data-stu-id="c3bc5-176">• View partner contribution data</span></span>
||<span data-ttu-id="c3bc5-177">• Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="c3bc5-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c3bc5-178">• Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-178">- View customer data analytics</span></span>
|<span data-ttu-id="c3bc5-179">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-179">Account admin</span></span>| <span data-ttu-id="c3bc5-180">• Hinzufügen von Nicht-Mandantenbenutzern</span><span class="sxs-lookup"><span data-stu-id="c3bc5-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="c3bc5-181">• Hinzufügen oder Löschen von Standorten</span><span class="sxs-lookup"><span data-stu-id="c3bc5-181">• Add or delete locations</span></span>
||<span data-ttu-id="c3bc5-182">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="c3bc5-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c3bc5-183">• Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="c3bc5-184">• Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="c3bc5-185">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="c3bc5-186">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-186">**Guest user**</span></span>   | <span data-ttu-id="c3bc5-187">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="c3bc5-188">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-188">MPN partner admin</span></span>|
||<span data-ttu-id="c3bc5-189">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-189">Accounts admin</span></span>|
||<span data-ttu-id="c3bc5-190">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-190">Incentives admin</span></span>|
||<span data-ttu-id="c3bc5-191">Geschäftsprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-191">Business profile admin</span></span>|
||<span data-ttu-id="c3bc5-192">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="c3bc5-193">Verwalten von Empfehlungen (Nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="c3bc5-194">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-194">**Role**</span></span>|<span data-ttu-id="c3bc5-195">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="c3bc5-196">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-196">Referrals admin</span></span>       |<span data-ttu-id="c3bc5-197">• Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="c3bc5-198">• Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="c3bc5-199">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="c3bc5-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="c3bc5-200">Geschäftsprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-200">Business profile admin</span></span>   |<span data-ttu-id="c3bc5-201">• Anzeigen, Erstellen und Verwalten des Geschäftsprofils</span><span class="sxs-lookup"><span data-stu-id="c3bc5-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="c3bc5-202">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="c3bc5-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="c3bc5-203">Verwalten von Incentives (Nicht-AAD-Rollen)</span><span class="sxs-lookup"><span data-stu-id="c3bc5-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="c3bc5-204">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-204">**Role**</span></span> | <span data-ttu-id="c3bc5-205">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="c3bc5-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c3bc5-206">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="c3bc5-206">Incentives admin</span></span>|<span data-ttu-id="c3bc5-207">• Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="c3bc5-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="c3bc5-208">• Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c3bc5-209">• Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="c3bc5-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c3bc5-210">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c3bc5-211">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="c3bc5-211">• Access support</span></span>
||<span data-ttu-id="c3bc5-212">• Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="c3bc5-213">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="c3bc5-213">Incentives user</span></span>|<span data-ttu-id="c3bc5-214">• Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="c3bc5-215">• Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c3bc5-216">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c3bc5-217">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="c3bc5-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c3bc5-218">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="c3bc5-218">• Access support</span></span>












