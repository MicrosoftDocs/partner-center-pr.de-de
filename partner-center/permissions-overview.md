---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Jedem Mitarbeiter, der im Partner Center arbeitet, muss eine Rolle zugewiesen werden.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 65a2f7f373fc57f86cfffa73aafd3b7095fe2c04
ms.sourcegitcommit: be8086534ec73937f2be9bcc495c2627423c50f6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/26/2019
ms.locfileid: "67396727"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="595cf-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-104">Assign users roles and permissions</span></span>


<span data-ttu-id="595cf-105">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="595cf-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="595cf-106">Nächster Schritt: Einrichten der Benutzer mit Kennwörtern und Rollen, damit sie mit Ihnen gemeinsam im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="595cf-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="595cf-107">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="595cf-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="595cf-108">Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="595cf-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="595cf-109">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="595cf-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="595cf-110">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="595cf-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="595cf-111">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="595cf-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="595cf-112">AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="595cf-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="595cf-113">Nicht-AAD-Rollen sind die Rollen, die keine Mandanten verwalten, und MPN Admin, Administrator für Business-Profil, Verweis Verwaltungs-, anreizprogramm Admin und anreizprogramm Benutzer enthalten.</span><span class="sxs-lookup"><span data-stu-id="595cf-113">Non-AAD roles are those roles that do not manage the tenant and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="595cf-114">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="595cf-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="595cf-115">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="595cf-115">**Role**</span></span>|<span data-ttu-id="595cf-116">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="595cf-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="595cf-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="595cf-117">Global admin</span></span>|<span data-ttu-id="595cf-118">• Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="595cf-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="595cf-119">• Erstellen von Supportanfragen für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="595cf-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="595cf-120">• Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="595cf-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="595cf-121">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="595cf-122">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-122">User Admin</span></span>   | <span data-ttu-id="595cf-123">• Anzeigen, Erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="595cf-124">• Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="595cf-124">• View all partner profiles</span></span>
||<span data-ttu-id="595cf-125">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="595cf-126">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-126">Billing admin</span></span> | <span data-ttu-id="595cf-127">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="595cf-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="595cf-128">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="595cf-128">Default user</span></span>|  <span data-ttu-id="595cf-129">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="595cf-129">View My profile</span></span>   |
|<span data-ttu-id="595cf-130">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="595cf-130">Admin agent</span></span> | <span data-ttu-id="595cf-131">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="595cf-131">•    Customer management</span></span>
||<span data-ttu-id="595cf-132">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="595cf-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="595cf-133">• Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="595cf-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="595cf-134">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="595cf-134">• Subscription management</span></span>
||<span data-ttu-id="595cf-135">• Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="595cf-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="595cf-136">• Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="595cf-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="595cf-137">• Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="595cf-137">• View pricing and offers</span></span>
||<span data-ttu-id="595cf-138">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="595cf-138">• Billing</span></span>
||<span data-ttu-id="595cf-139">• Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="595cf-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="595cf-140">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="595cf-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="595cf-141">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="595cf-141">Sales agent</span></span> | <span data-ttu-id="595cf-142">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="595cf-142">•    Customer management</span></span>
||<span data-ttu-id="595cf-143">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="595cf-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="595cf-144">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="595cf-144">• Subscription management</span></span>
||<span data-ttu-id="595cf-145">• Anzeigen Preis aufgelistet und bietet</span><span class="sxs-lookup"><span data-stu-id="595cf-145">• View price lists and offers</span></span>
||<span data-ttu-id="595cf-146">• Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="595cf-146">• View support tickets</span></span>
||<span data-ttu-id="595cf-147">• Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="595cf-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="595cf-148">• Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="595cf-148">• Manage customer leads</span></span>
||<span data-ttu-id="595cf-149">• Anzeigen des Kundenvertrags</span><span class="sxs-lookup"><span data-stu-id="595cf-149">• View the customer agreement</span></span>
||<span data-ttu-id="595cf-150">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="595cf-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="595cf-151">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="595cf-151">Helpdesk agent</span></span>| <span data-ttu-id="595cf-152">• Suchen nach und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="595cf-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="595cf-153">• Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="595cf-153">• Edit customer details</span></span>
||<span data-ttu-id="595cf-154">• Unterstützten von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="595cf-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="595cf-155">• Anfordern von Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="595cf-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="595cf-156">• Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="595cf-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="595cf-157">CPV (Control Panel Vendor).</span><span class="sxs-lookup"><span data-stu-id="595cf-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="595cf-158">(CSP-Rolle und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="595cf-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="595cf-159">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="595cf-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="595cf-160">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="595cf-160">**Role**</span></span>   |<span data-ttu-id="595cf-161">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="595cf-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="595cf-162">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="595cf-162">Global admin</span></span>| <span data-ttu-id="595cf-163">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="595cf-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="595cf-164">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="595cf-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="595cf-165">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="595cf-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="595cf-166">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="595cf-166">**Guest user**</span></span>   | <span data-ttu-id="595cf-167">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="595cf-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="595cf-168">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-168">MPN partner admin</span></span>|
||<span data-ttu-id="595cf-169">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-169">Accounts admin</span></span>|
||<span data-ttu-id="595cf-170">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-170">Incentives admin</span></span>|
||<span data-ttu-id="595cf-171">Geschäftsprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-171">Business profile admin</span></span>|
||<span data-ttu-id="595cf-172">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="595cf-173">Verwalten von MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen: Diese Rollen zu verwalten, die Geschäftstätigkeit Unternehmen statt des Mandanten)</span><span class="sxs-lookup"><span data-stu-id="595cf-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="595cf-174">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="595cf-174">**Role**</span></span> | <span data-ttu-id="595cf-175">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="595cf-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="595cf-176">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-176">MPN partner admin</span></span>|<span data-ttu-id="595cf-177">• Hinzufügen von Nicht-Mandantenbenutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-177">•Can add non-tenant users</span></span>
||<span data-ttu-id="595cf-178">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="595cf-178">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="595cf-179">• Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="595cf-179">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="595cf-180">• Anzeigen der Daten und Fähigkeiten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-180">• View user details and their skills data</span></span>
||<span data-ttu-id="595cf-181">• Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="595cf-181">• View competencies</span></span>
||<span data-ttu-id="595cf-182">• Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="595cf-182">• View and manage benefits</span></span>
||<span data-ttu-id="595cf-183">• Anzeigen und Kaufen von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="595cf-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="595cf-184">• Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="595cf-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="595cf-185">• Anzeigen von Partnerbeitragsdaten</span><span class="sxs-lookup"><span data-stu-id="595cf-185">• View partner contribution data</span></span>
||<span data-ttu-id="595cf-186">• Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="595cf-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="595cf-187">• Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="595cf-187">- View customer data analytics</span></span>
|<span data-ttu-id="595cf-188">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-188">Account admin</span></span>| <span data-ttu-id="595cf-189">• Hinzufügen von Nicht-Mandantenbenutzern</span><span class="sxs-lookup"><span data-stu-id="595cf-189">•   Can add non-tenant users</span></span>
||<span data-ttu-id="595cf-190">• Hinzufügen oder Löschen von Standorten</span><span class="sxs-lookup"><span data-stu-id="595cf-190">• Add or delete locations</span></span>
||<span data-ttu-id="595cf-191">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="595cf-191">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="595cf-192">• Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="595cf-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="595cf-193">• Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="595cf-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="595cf-194">Verwalten von verweisen</span><span class="sxs-lookup"><span data-stu-id="595cf-194">Manage referrals</span></span> 

|<span data-ttu-id="595cf-195">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="595cf-195">**Role**</span></span>|<span data-ttu-id="595cf-196">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="595cf-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="595cf-197">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-197">Referrals admin</span></span>       |<span data-ttu-id="595cf-198">• Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="595cf-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="595cf-199">• Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="595cf-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="595cf-200">• Anzeigen, erstellen und Verwalten von Co-Selling-Verweise</span><span class="sxs-lookup"><span data-stu-id="595cf-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="595cf-201">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="595cf-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="595cf-202">Administrator für das Unternehmensprofil</span><span class="sxs-lookup"><span data-stu-id="595cf-202">Business profile admin</span></span>   |<span data-ttu-id="595cf-203">• Anzeigen, erstellen und Verwalten von Business-Profil</span><span class="sxs-lookup"><span data-stu-id="595cf-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="595cf-204">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="595cf-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="595cf-205">Verwalten von incentives</span><span class="sxs-lookup"><span data-stu-id="595cf-205">Manage incentives</span></span> 

|<span data-ttu-id="595cf-206">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="595cf-206">**Role**</span></span> | <span data-ttu-id="595cf-207">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="595cf-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="595cf-208">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="595cf-208">Incentives admin</span></span>|<span data-ttu-id="595cf-209">• Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="595cf-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="595cf-210">• Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="595cf-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="595cf-211">• Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="595cf-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="595cf-212">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="595cf-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="595cf-213">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="595cf-213">• Access support</span></span>
||<span data-ttu-id="595cf-214">• Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="595cf-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="595cf-215">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="595cf-215">Incentives user</span></span>|<span data-ttu-id="595cf-216">• Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="595cf-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="595cf-217">• Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="595cf-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="595cf-218">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="595cf-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="595cf-219">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="595cf-219">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="595cf-220">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="595cf-220">• Access support</span></span>












