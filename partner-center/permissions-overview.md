---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 3/5/2019
description: Jedem Mitarbeiter, der im Partner Center arbeitet, muss eine Rolle zugewiesen werden.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708870"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="32617-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="32617-104">Assign users roles and permissions</span></span>


<span data-ttu-id="32617-105">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="32617-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="32617-106">Nächster Schritt: Einrichten der Benutzer mit Kennwörtern und Rollen, damit sie mit Ihnen gemeinsam im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="32617-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="32617-107">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="32617-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="32617-108">Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="32617-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="32617-109">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="32617-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="32617-110">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="32617-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="32617-111">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="32617-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="32617-112">AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="32617-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="32617-113">Nicht-Aad-Rollen sind die Rollen, die den Mandanten nicht verwalten. dazu gehören MPN admin, Business profile admin, referadmin, Incentive admin und Incentive User.</span><span class="sxs-lookup"><span data-stu-id="32617-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="32617-114">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="32617-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="32617-115">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="32617-115">**Role**</span></span>|<span data-ttu-id="32617-116">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="32617-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="32617-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="32617-117">Global admin</span></span>|<span data-ttu-id="32617-118">• Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32617-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="32617-119">• Erstellen von Supportanfragen für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="32617-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="32617-120">• Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="32617-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="32617-121">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="32617-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="32617-122">Anzeigen, erstellen und Verwalten von Abrechnungs-, Rechnungen-und Reconnaissance-Dateien</span><span class="sxs-lookup"><span data-stu-id="32617-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="32617-123">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-123">User management admin</span></span>   | <span data-ttu-id="32617-124">• Anzeigen, erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="32617-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="32617-125">• Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="32617-125">• View all partner profiles</span></span>
||<span data-ttu-id="32617-126">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="32617-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="32617-127">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-127">Billing admin</span></span> | <span data-ttu-id="32617-128">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="32617-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="32617-129">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="32617-129">Default user</span></span>|  <span data-ttu-id="32617-130">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="32617-130">View My profile</span></span>   |
|<span data-ttu-id="32617-131">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="32617-131">Admin agent</span></span> | <span data-ttu-id="32617-132">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="32617-132">•    Customer management</span></span>
||<span data-ttu-id="32617-133">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="32617-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="32617-134">• Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="32617-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="32617-135">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="32617-135">• Subscription management</span></span>
||<span data-ttu-id="32617-136">• Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="32617-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="32617-137">• Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="32617-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="32617-138">• Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="32617-138">• View pricing and offers</span></span>
||<span data-ttu-id="32617-139">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="32617-139">• Billing</span></span>
||<span data-ttu-id="32617-140">• Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="32617-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="32617-141">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="32617-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="32617-142">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="32617-142">Sales agent</span></span> | <span data-ttu-id="32617-143">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="32617-143">•    Customer management</span></span>
||<span data-ttu-id="32617-144">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="32617-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="32617-145">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="32617-145">• Subscription management</span></span>
||<span data-ttu-id="32617-146">• Preislisten und Angebote anzeigen</span><span class="sxs-lookup"><span data-stu-id="32617-146">• View price lists and offers</span></span>
||<span data-ttu-id="32617-147">• Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="32617-147">• View support tickets</span></span>
||<span data-ttu-id="32617-148">• Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="32617-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="32617-149">• Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="32617-149">• Manage customer leads</span></span>
||<span data-ttu-id="32617-150">• Anzeigen des Kundenvertrags</span><span class="sxs-lookup"><span data-stu-id="32617-150">• View the customer agreement</span></span>
||<span data-ttu-id="32617-151">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="32617-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="32617-152">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="32617-152">Helpdesk agent</span></span>| <span data-ttu-id="32617-153">• Suchen nach und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="32617-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="32617-154">• Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="32617-154">• Edit customer details</span></span>
||<span data-ttu-id="32617-155">• Unterstützten von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="32617-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="32617-156">• Anfordern von Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="32617-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="32617-157">• Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="32617-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="32617-158">CPV (Control Panel Vendor).</span><span class="sxs-lookup"><span data-stu-id="32617-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="32617-159">(CSP-Rolle und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="32617-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="32617-160">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="32617-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="32617-161">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="32617-161">**Role**</span></span>   |<span data-ttu-id="32617-162">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="32617-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="32617-163">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="32617-163">Global admin</span></span>| <span data-ttu-id="32617-164">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="32617-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="32617-165">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="32617-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="32617-166">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="32617-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="32617-167">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="32617-167">**Guest user**</span></span>   | <span data-ttu-id="32617-168">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="32617-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="32617-169">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="32617-169">MPN partner admin</span></span>|
||<span data-ttu-id="32617-170">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-170">Accounts admin</span></span>|
||<span data-ttu-id="32617-171">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-171">Incentives admin</span></span>|
||<span data-ttu-id="32617-172">Geschäftsprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="32617-172">Business profile admin</span></span>|
||<span data-ttu-id="32617-173">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="32617-174">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (nicht-Aad-Rollen: Diese Rollen verwalten das Unternehmensgeschäft und nicht den Mandanten)</span><span class="sxs-lookup"><span data-stu-id="32617-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="32617-175">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="32617-175">**Role**</span></span> | <span data-ttu-id="32617-176">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="32617-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="32617-177">Administrator für MPN-Partner</span><span class="sxs-lookup"><span data-stu-id="32617-177">MPN partner admin</span></span>|<span data-ttu-id="32617-178">• Anzeigen, erstellen und Verwalten von Partner Dienst Anforderungen</span><span class="sxs-lookup"><span data-stu-id="32617-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="32617-179">• Anzeigen von rechtlichen, Firmen-, Geschäfts-und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="32617-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="32617-180">• Anzeigen der Daten und Fähigkeiten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="32617-180">• View user details and their skills data</span></span>
||<span data-ttu-id="32617-181">• Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="32617-181">• View competencies</span></span>
||<span data-ttu-id="32617-182">• Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="32617-182">• View and manage benefits</span></span>
||<span data-ttu-id="32617-183">• Anzeigen und Kaufen von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="32617-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="32617-184">• Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="32617-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="32617-185">• Anzeigen von Partner Beitrag-Indikator Daten</span><span class="sxs-lookup"><span data-stu-id="32617-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="32617-186">• Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="32617-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="32617-187">• Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="32617-187">- View customer data analytics</span></span>
|| <span data-ttu-id="32617-188">Anzeigen anderer Benutzer Rollen innerhalb des Unternehmens, aber keine Zuweisung von Rollen</span><span class="sxs-lookup"><span data-stu-id="32617-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="32617-189">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-189">Account admin</span></span>| <span data-ttu-id="32617-190">Speicherorte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="32617-190">Add locations</span></span>
|| <span data-ttu-id="32617-191">Verwalten von Profilen in Bezug auf die Konten, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="32617-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="32617-192">• Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="32617-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="32617-193">• Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="32617-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="32617-194">Verwalten von verweisen</span><span class="sxs-lookup"><span data-stu-id="32617-194">Manage referrals</span></span> 

|<span data-ttu-id="32617-195">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="32617-195">**Role**</span></span>|<span data-ttu-id="32617-196">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="32617-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="32617-197">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-197">Referrals admin</span></span>       |<span data-ttu-id="32617-198">• Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="32617-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="32617-199">• Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="32617-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="32617-200">• Anzeigen, erstellen und Verwalten von Co-Selling-Referenzen</span><span class="sxs-lookup"><span data-stu-id="32617-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="32617-201">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="32617-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="32617-202">Administrator für das Unternehmensprofil</span><span class="sxs-lookup"><span data-stu-id="32617-202">Business profile admin</span></span>   |<span data-ttu-id="32617-203">• Anzeigen, erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="32617-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="32617-204">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="32617-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="32617-205">Verwalten von Anreizen</span><span class="sxs-lookup"><span data-stu-id="32617-205">Manage incentives</span></span> 

|<span data-ttu-id="32617-206">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="32617-206">**Role**</span></span> | <span data-ttu-id="32617-207">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="32617-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="32617-208">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="32617-208">Incentives admin</span></span>|<span data-ttu-id="32617-209">• Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="32617-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="32617-210">• Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="32617-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="32617-211">• Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="32617-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="32617-212">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="32617-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="32617-213">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="32617-213">• Access support</span></span>
||<span data-ttu-id="32617-214">• Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="32617-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="32617-215">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="32617-215">Incentives user</span></span>|<span data-ttu-id="32617-216">• Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="32617-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="32617-217">• Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="32617-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="32617-218">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="32617-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="32617-219">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="32617-219">• Access support</span></span>












