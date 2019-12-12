---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 10/10/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfährst du, welche Rollen für Benutzer am besten geeignet sind, die kommerzielle Transaktionen, Empfehlungen, Anreize oder die MPN-Mitgliedschaften deines Unternehmens verwalten.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: high
ms.openlocfilehash: f49417eea3a2d8b06713cd53355eef68c81d179e
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943133"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="e594d-104">Zuweisen von Rollen und Berechtigungen zu Benutzern</span><span class="sxs-lookup"><span data-stu-id="e594d-104">Assign users roles and permissions</span></span>


<span data-ttu-id="e594d-105">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="e594d-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="e594d-106">Nächster Schritt: Einrichten der Benutzer mit Kennwörtern und Rollen, damit sie mit Ihnen gemeinsam im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="e594d-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="e594d-107">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="e594d-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="e594d-108">Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="e594d-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="e594d-109">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="e594d-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="e594d-110">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="e594d-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="e594d-111">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="e594d-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="e594d-112">AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="e594d-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="e594d-113">Nicht-AAD-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Zu ihnen gehören MPN-Administrator, Geschäftsprofiladministrator, Empfehlungsadministrator, Incentiveadministrator und Incentivebenutzer.</span><span class="sxs-lookup"><span data-stu-id="e594d-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="e594d-114">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="e594d-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="e594d-115">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="e594d-115">**Role**</span></span>|<span data-ttu-id="e594d-116">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="e594d-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="e594d-117">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="e594d-117">Global admin</span></span>|<span data-ttu-id="e594d-118">• Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e594d-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="e594d-119">• Erstellen von Supportanfragen für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="e594d-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="e594d-120">• Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="e594d-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="e594d-121">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="e594d-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="e594d-122">Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="e594d-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="e594d-123">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-123">User management admin</span></span>   | <span data-ttu-id="e594d-124">•    Benutzer anzeigen, erstellen und verwalten</span><span class="sxs-lookup"><span data-stu-id="e594d-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="e594d-125">• Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="e594d-125">• View all partner profiles</span></span>
||<span data-ttu-id="e594d-126">• Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="e594d-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="e594d-127">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-127">Billing admin</span></span> | <span data-ttu-id="e594d-128">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="e594d-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="e594d-129">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="e594d-129">Default user</span></span>|  <span data-ttu-id="e594d-130">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="e594d-130">View My profile</span></span>   |
|<span data-ttu-id="e594d-131">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="e594d-131">Admin agent</span></span> | <span data-ttu-id="e594d-132">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="e594d-132">•    Customer management</span></span>
||<span data-ttu-id="e594d-133">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="e594d-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="e594d-134">• Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="e594d-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="e594d-135">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="e594d-135">• Subscription management</span></span>
||<span data-ttu-id="e594d-136">• Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="e594d-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="e594d-137">• Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="e594d-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="e594d-138">• Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="e594d-138">• View pricing and offers</span></span>
||<span data-ttu-id="e594d-139">• Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e594d-139">• Billing</span></span>
||<span data-ttu-id="e594d-140">• Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="e594d-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="e594d-141">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="e594d-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="e594d-142">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="e594d-142">Sales agent</span></span> | <span data-ttu-id="e594d-143">• Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="e594d-143">•    Customer management</span></span>
||<span data-ttu-id="e594d-144">• Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="e594d-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="e594d-145">• Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="e594d-145">• Subscription management</span></span>
||<span data-ttu-id="e594d-146">• Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="e594d-146">• View support tickets</span></span>
||<span data-ttu-id="e594d-147">• Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="e594d-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="e594d-148">• Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="e594d-148">• Manage customer leads</span></span>
||<span data-ttu-id="e594d-149">• Anzeigen des Kundenvertrags</span><span class="sxs-lookup"><span data-stu-id="e594d-149">• View the customer agreement</span></span>
||<span data-ttu-id="e594d-150">• Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="e594d-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="e594d-151">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="e594d-151">Helpdesk agent</span></span>| <span data-ttu-id="e594d-152">• Suchen nach und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="e594d-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="e594d-153">• Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="e594d-153">• Edit customer details</span></span>
||<span data-ttu-id="e594d-154">• Unterstützten von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="e594d-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="e594d-155">• Anfordern von Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="e594d-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="e594d-156">• Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)</span><span class="sxs-lookup"><span data-stu-id="e594d-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="e594d-157">CPV (Control Panel Vendor).</span><span class="sxs-lookup"><span data-stu-id="e594d-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="e594d-158">(CSP-Rolle und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="e594d-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="e594d-159">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="e594d-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="e594d-160">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="e594d-160">**Role**</span></span>   |<span data-ttu-id="e594d-161">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="e594d-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="e594d-162">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="e594d-162">Global admin</span></span>| <span data-ttu-id="e594d-163">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="e594d-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="e594d-164">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="e594d-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="e594d-165">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="e594d-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="e594d-166">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="e594d-166">**Guest user**</span></span>   | <span data-ttu-id="e594d-167">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="e594d-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="e594d-168">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-168">MPN partner admin</span></span>|
||<span data-ttu-id="e594d-169">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-169">Accounts admin</span></span>|
||<span data-ttu-id="e594d-170">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-170">Incentives admin</span></span>|
||<span data-ttu-id="e594d-171">Geschäftsprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-171">Business profile admin</span></span>|
||<span data-ttu-id="e594d-172">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="e594d-173">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen: diese Rollen sind auf das Unternehmen bezogen, nicht auf den Mandanten)</span><span class="sxs-lookup"><span data-stu-id="e594d-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="e594d-174">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="e594d-174">**Role**</span></span> | <span data-ttu-id="e594d-175">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="e594d-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="e594d-176">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-176">MPN partner admin</span></span>|<span data-ttu-id="e594d-177">•    Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="e594d-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="e594d-178">• Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="e594d-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="e594d-179">• Anzeigen der Daten und Fähigkeiten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="e594d-179">• View user details and their skills data</span></span>
||<span data-ttu-id="e594d-180">• Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="e594d-180">• View competencies</span></span>
||<span data-ttu-id="e594d-181">• Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="e594d-181">• View and manage benefits</span></span>
||<span data-ttu-id="e594d-182">• Anzeigen und Kaufen von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="e594d-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="e594d-183">• Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="e594d-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="e594d-184">• Anzeigen von Daten der Partnerbeitragsindikatoren</span><span class="sxs-lookup"><span data-stu-id="e594d-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="e594d-185">• Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="e594d-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="e594d-186">• Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="e594d-186">- View customer data analytics</span></span>
|| <span data-ttu-id="e594d-187">Anzeigen der Rollen anderer Benutzer im Unternehmen, kann jedoch seinerseits keine Rollen zuweisen</span><span class="sxs-lookup"><span data-stu-id="e594d-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="e594d-188">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-188">Account admin</span></span>| <span data-ttu-id="e594d-189">Hinzufügen von Speicherorten</span><span class="sxs-lookup"><span data-stu-id="e594d-189">Add locations</span></span>
|| <span data-ttu-id="e594d-190">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="e594d-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="e594d-191">• Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="e594d-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="e594d-192">• Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="e594d-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="e594d-193">Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="e594d-193">Manage referrals</span></span> 

|<span data-ttu-id="e594d-194">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="e594d-194">**Role**</span></span>|<span data-ttu-id="e594d-195">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="e594d-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="e594d-196">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-196">Referrals admin</span></span>       |<span data-ttu-id="e594d-197">• Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="e594d-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="e594d-198">• Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="e594d-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="e594d-199">• Anzeigen, Erstellen und Verwalten von Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="e594d-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="e594d-200">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="e594d-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="e594d-201">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-201">Business profile admin</span></span>   |<span data-ttu-id="e594d-202">• Anzeigen, Erstellen und Verwalten des Geschäftsprofils</span><span class="sxs-lookup"><span data-stu-id="e594d-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="e594d-203">• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner</span><span class="sxs-lookup"><span data-stu-id="e594d-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="e594d-204">Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="e594d-204">Manage incentives</span></span> 

|<span data-ttu-id="e594d-205">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="e594d-205">**Role**</span></span> | <span data-ttu-id="e594d-206">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="e594d-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="e594d-207">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="e594d-207">Incentives admin</span></span>|<span data-ttu-id="e594d-208">• Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="e594d-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="e594d-209">• Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="e594d-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="e594d-210">• Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="e594d-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="e594d-211">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="e594d-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e594d-212">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="e594d-212">• Access support</span></span>
||<span data-ttu-id="e594d-213">• Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="e594d-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="e594d-214">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="e594d-214">Incentives user</span></span>|<span data-ttu-id="e594d-215">• Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="e594d-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="e594d-216">• Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="e594d-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="e594d-217">• Anzeigen von Rabatt- und Co-Op-Einnahmen</span><span class="sxs-lookup"><span data-stu-id="e594d-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e594d-218">• Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="e594d-218">• Access support</span></span>












