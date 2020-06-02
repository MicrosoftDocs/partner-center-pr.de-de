---
title: Zuweisen von Rollen und Berechtigungen zu Benutzern
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, welche Rollen am besten für Benutzer in Ihrem Unternehmen geeignet sind, die kommerzielle Transaktionen, Empfehlungen, Incentives oder MPN-Mitgliedschaften im Partner Center verwalten.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 0858340c6965ac932f0d4694f6f21be89ca5f817
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795887"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="7472b-104">Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen</span><span class="sxs-lookup"><span data-stu-id="7472b-104">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="7472b-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="7472b-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7472b-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7472b-106">Global admin</span></span>
- <span data-ttu-id="7472b-107">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-107">User admin</span></span>
- <span data-ttu-id="7472b-108">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-108">MPN partner admin</span></span>

<span data-ttu-id="7472b-109">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="7472b-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7472b-110">Nächster Schritt: Richten Sie Kennwörter und Rollen für Ihre Benutzer ein, damit sie gemeinsam mit Ihnen im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="7472b-110">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7472b-111">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="7472b-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7472b-112">Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="7472b-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7472b-113">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="7472b-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7472b-114">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="7472b-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7472b-115">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="7472b-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7472b-116">AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen.</span><span class="sxs-lookup"><span data-stu-id="7472b-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7472b-117">Nicht-AAD-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Zu ihnen gehören MPN-Administrator, Geschäftsprofiladministrator, Empfehlungsadministrator, Incentiveadministrator und Incentivebenutzer.</span><span class="sxs-lookup"><span data-stu-id="7472b-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7472b-118">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="7472b-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7472b-119">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="7472b-119">**Role**</span></span>|<span data-ttu-id="7472b-120">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="7472b-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7472b-121">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7472b-121">Global admin</span></span>|<span data-ttu-id="7472b-122">\* Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7472b-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7472b-123">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="7472b-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7472b-124">\* Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="7472b-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7472b-125">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="7472b-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7472b-126">Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="7472b-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7472b-127">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-127">User management admin</span></span>   | <span data-ttu-id="7472b-128">\* Anzeigen, Erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="7472b-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="7472b-129">\* Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="7472b-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="7472b-130">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="7472b-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="7472b-131">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-131">Billing admin</span></span> | <span data-ttu-id="7472b-132">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="7472b-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="7472b-133">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="7472b-133">Default user</span></span>|  <span data-ttu-id="7472b-134">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="7472b-134">View My profile</span></span>   |
|<span data-ttu-id="7472b-135">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="7472b-135">Admin agent</span></span> | <span data-ttu-id="7472b-136">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="7472b-136">\*    Customer management</span></span>
||<span data-ttu-id="7472b-137">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="7472b-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7472b-138">\* Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="7472b-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="7472b-139">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="7472b-139">\*    Subscription management</span></span>
||<span data-ttu-id="7472b-140">\* Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="7472b-141">\* Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="7472b-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="7472b-142">\* Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="7472b-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="7472b-143">\* Abrechnung</span><span class="sxs-lookup"><span data-stu-id="7472b-143">\*    Billing</span></span>
||<span data-ttu-id="7472b-144">\* Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="7472b-145">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="7472b-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="7472b-146">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="7472b-146">Sales agent</span></span> | <span data-ttu-id="7472b-147">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="7472b-147">\*    Customer management</span></span>
||<span data-ttu-id="7472b-148">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="7472b-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7472b-149">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="7472b-149">\*    Subscription management</span></span>
||<span data-ttu-id="7472b-150">\* Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="7472b-150">\*    View support tickets</span></span>
||<span data-ttu-id="7472b-151">\* Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="7472b-152">\* Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="7472b-153">\* Anzeigen der Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="7472b-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="7472b-154">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="7472b-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="7472b-155">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="7472b-155">Helpdesk agent</span></span>| <span data-ttu-id="7472b-156">\* Suchen und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="7472b-157">\* Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="7472b-157">\*    Edit customer details</span></span>
||<span data-ttu-id="7472b-158">\* Unterstützen von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="7472b-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7472b-159">\* Anfordern von Support für Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="7472b-160">\* Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden</span><span class="sxs-lookup"><span data-stu-id="7472b-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7472b-161">CPV (Control Panel Vendor).</span><span class="sxs-lookup"><span data-stu-id="7472b-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7472b-162">(CSP-Rolle und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="7472b-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7472b-163">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="7472b-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7472b-164">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="7472b-164">**Role**</span></span>   |<span data-ttu-id="7472b-165">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="7472b-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7472b-166">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7472b-166">Global admin</span></span>| <span data-ttu-id="7472b-167">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="7472b-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7472b-168">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="7472b-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7472b-169">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="7472b-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7472b-170">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="7472b-170">**Guest user**</span></span>   | <span data-ttu-id="7472b-171">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="7472b-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7472b-172">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-172">MPN partner admin</span></span>|
||<span data-ttu-id="7472b-173">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-173">Accounts admin</span></span>|
||<span data-ttu-id="7472b-174">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-174">Incentives admin</span></span>|
||<span data-ttu-id="7472b-175">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-175">Business profile admin</span></span>|
||<span data-ttu-id="7472b-176">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7472b-177">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen: diese Rollen sind auf das Unternehmen bezogen, nicht auf den Mandanten)</span><span class="sxs-lookup"><span data-stu-id="7472b-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7472b-178">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="7472b-178">**Role**</span></span> | <span data-ttu-id="7472b-179">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="7472b-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7472b-180">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-180">MPN partner admin</span></span>|<span data-ttu-id="7472b-181">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="7472b-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7472b-182">\* Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="7472b-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7472b-183">\* Anzeigen der Daten und Qualifikationen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="7472b-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="7472b-184">\* Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="7472b-184">\*    View competencies</span></span>
||<span data-ttu-id="7472b-185">\* Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="7472b-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="7472b-186">\* Anzeigen und Erwerben von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="7472b-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="7472b-187">\* Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="7472b-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7472b-188">\* Anzeigen von Daten zu Partnerbeitragsindikatoren</span><span class="sxs-lookup"><span data-stu-id="7472b-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="7472b-189">\* Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="7472b-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7472b-190">\* Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="7472b-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="7472b-191">\* Anzeigen der Rollen anderer Benutzer im Unternehmen, kann jedoch seinerseits keine Rollen zuweisen</span><span class="sxs-lookup"><span data-stu-id="7472b-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="7472b-192">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-192">Account admin</span></span>| <span data-ttu-id="7472b-193">Hinzufügen von Speicherorten</span><span class="sxs-lookup"><span data-stu-id="7472b-193">Add locations</span></span>
|| <span data-ttu-id="7472b-194">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="7472b-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7472b-195">\* Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="7472b-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7472b-196">\* Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="7472b-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7472b-197">Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="7472b-197">Manage referrals</span></span> 

|<span data-ttu-id="7472b-198">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="7472b-198">**Role**</span></span>|<span data-ttu-id="7472b-199">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="7472b-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7472b-200">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-200">Referrals admin</span></span>       |<span data-ttu-id="7472b-201">\* Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="7472b-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="7472b-202">\* Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="7472b-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="7472b-203">\* Anzeigen, Erstellen und Verwalten von Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="7472b-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7472b-204">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="7472b-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7472b-205">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-205">Business profile admin</span></span>   |<span data-ttu-id="7472b-206">\* Anzeigen, Erstellen und Verwalten des Geschäftsprofils</span><span class="sxs-lookup"><span data-stu-id="7472b-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="7472b-207">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="7472b-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7472b-208">Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="7472b-208">Manage incentives</span></span> 

|<span data-ttu-id="7472b-209">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="7472b-209">**Role**</span></span> | <span data-ttu-id="7472b-210">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="7472b-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7472b-211">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="7472b-211">Incentives admin</span></span>|<span data-ttu-id="7472b-212">\* Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="7472b-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="7472b-213">\* Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="7472b-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7472b-214">\* Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="7472b-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7472b-215">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="7472b-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7472b-216">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="7472b-216">\*    Access support</span></span>
||<span data-ttu-id="7472b-217">\* Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="7472b-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="7472b-218">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="7472b-218">Incentives user</span></span>|<span data-ttu-id="7472b-219">\* Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="7472b-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="7472b-220">\* Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="7472b-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7472b-221">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="7472b-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7472b-222">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="7472b-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="7472b-223">Partner Center-Einblicke – Daten anzeigen</span><span class="sxs-lookup"><span data-stu-id="7472b-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="7472b-224">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="7472b-224">**Role**</span></span> | <span data-ttu-id="7472b-225">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="7472b-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7472b-226">Bericht-Viewer für leitende Mitarbeiter</span><span class="sxs-lookup"><span data-stu-id="7472b-226">Executive report viewer</span></span>|<span data-ttu-id="7472b-227">Zugriff auf alle Berichtsdatasets</span><span class="sxs-lookup"><span data-stu-id="7472b-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="7472b-228">Berichts-Viewer</span><span class="sxs-lookup"><span data-stu-id="7472b-228">Report viewer</span></span>|<span data-ttu-id="7472b-229">Zugriff auf Datenberichte mit Ausnahme von Umsatz-, Kunden- und personenbezogenen Mitarbeiterdaten</span><span class="sxs-lookup"><span data-stu-id="7472b-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    