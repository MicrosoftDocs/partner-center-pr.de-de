---
title: Zuweisen von Rollen und Berechtigungen zu Benutzern
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, welche Rollen am besten für Benutzer in Ihrem Unternehmen geeignet sind, die kommerzielle Transaktionen, Empfehlungen, Incentives oder MPN-Mitgliedschaften im Partner Center verwalten.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434319"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="2869a-103">Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen</span><span class="sxs-lookup"><span data-stu-id="2869a-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="2869a-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="2869a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2869a-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2869a-105">Global admin</span></span>
- <span data-ttu-id="2869a-106">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-106">User admin</span></span>
- <span data-ttu-id="2869a-107">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-107">MPN partner admin</span></span>

<span data-ttu-id="2869a-108">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="2869a-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="2869a-109">Der nächste Schritt besteht in der Einrichtung von Kennwörtern und Rollen für Ihre Benutzer, damit diese gemeinsam mit Ihnen im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="2869a-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="2869a-110">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="2869a-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="2869a-111">Wie Ihre Benutzer auf das Partner Center zugreifen können, bestimmen Sie über die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="2869a-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="2869a-112">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="2869a-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="2869a-113">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="2869a-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="2869a-114">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="2869a-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="2869a-115">Zu den AAD-Mandantenrollen (Azure Active Directory) gehören die Rollen „Globaler Administrator“, „Benutzeradministrator“ und „CSP“.</span><span class="sxs-lookup"><span data-stu-id="2869a-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="2869a-116">Nicht-AAD-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Zu ihnen gehören MPN-Administratoren, Geschäftsprofiladministratoren, Empfehlungsadministratoren, Prämienadministratoren und Prämienbenutzer.</span><span class="sxs-lookup"><span data-stu-id="2869a-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="2869a-117">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="2869a-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="2869a-118">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="2869a-118">**Role**</span></span>|<span data-ttu-id="2869a-119">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="2869a-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="2869a-120">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2869a-120">Global admin</span></span>|<span data-ttu-id="2869a-121">\* Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2869a-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="2869a-122">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="2869a-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="2869a-123">\* Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="2869a-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="2869a-124">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="2869a-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="2869a-125">Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="2869a-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="2869a-126">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-126">User management admin</span></span>   | <span data-ttu-id="2869a-127">\* Anzeigen, Erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="2869a-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="2869a-128">\* Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="2869a-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="2869a-129">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="2869a-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="2869a-130">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-130">Billing admin</span></span> | <span data-ttu-id="2869a-131">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="2869a-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="2869a-132">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="2869a-132">Default user</span></span>|  <span data-ttu-id="2869a-133">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="2869a-133">View My profile</span></span>   |
|<span data-ttu-id="2869a-134">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="2869a-134">Admin agent</span></span> | <span data-ttu-id="2869a-135">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="2869a-135">\*    Customer management</span></span>
||<span data-ttu-id="2869a-136">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="2869a-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="2869a-137">\* Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="2869a-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="2869a-138">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="2869a-138">\*    Subscription management</span></span>
||<span data-ttu-id="2869a-139">\* Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="2869a-140">\* Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="2869a-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="2869a-141">\* Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="2869a-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="2869a-142">\* Abrechnung</span><span class="sxs-lookup"><span data-stu-id="2869a-142">\*    Billing</span></span>
||<span data-ttu-id="2869a-143">\* Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="2869a-144">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="2869a-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="2869a-145">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="2869a-145">Sales agent</span></span> | <span data-ttu-id="2869a-146">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="2869a-146">\*    Customer management</span></span>
||<span data-ttu-id="2869a-147">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="2869a-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="2869a-148">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="2869a-148">\*    Subscription management</span></span>
||<span data-ttu-id="2869a-149">\* Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="2869a-149">\*    View support tickets</span></span>
||<span data-ttu-id="2869a-150">\* Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="2869a-151">\* Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="2869a-152">\* Anzeigen der Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="2869a-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="2869a-153">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="2869a-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="2869a-154">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="2869a-154">Helpdesk agent</span></span>| <span data-ttu-id="2869a-155">\* Suchen und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="2869a-156">\* Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="2869a-156">\*    Edit customer details</span></span>
||<span data-ttu-id="2869a-157">\* Unterstützen von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="2869a-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="2869a-158">\* Anfordern von Support für Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="2869a-159">\* Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden</span><span class="sxs-lookup"><span data-stu-id="2869a-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="2869a-160">CPV (Control Panel Vendor,</span><span class="sxs-lookup"><span data-stu-id="2869a-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="2869a-161">CSP- und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="2869a-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="2869a-162">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="2869a-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="2869a-163">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="2869a-163">**Role**</span></span>   |<span data-ttu-id="2869a-164">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="2869a-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="2869a-165">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2869a-165">Global admin</span></span>| <span data-ttu-id="2869a-166">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="2869a-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="2869a-167">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="2869a-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="2869a-168">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="2869a-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="2869a-169">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="2869a-169">**Guest user**</span></span>   | <span data-ttu-id="2869a-170">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="2869a-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="2869a-171">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-171">MPN partner admin</span></span>|
||<span data-ttu-id="2869a-172">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-172">Accounts admin</span></span>|
||<span data-ttu-id="2869a-173">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-173">Incentives admin</span></span>|
||<span data-ttu-id="2869a-174">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-174">Business profile admin</span></span>|
||<span data-ttu-id="2869a-175">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="2869a-176">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (Nicht-AAD-Rollen, die zur Verwaltung auf Unternehmens- statt auf Mandantenebene verwendet werden)</span><span class="sxs-lookup"><span data-stu-id="2869a-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="2869a-177">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="2869a-177">**Role**</span></span> | <span data-ttu-id="2869a-178">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="2869a-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="2869a-179">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-179">MPN partner admin</span></span>|<span data-ttu-id="2869a-180">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="2869a-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="2869a-181">\* Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="2869a-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="2869a-182">\* Anzeigen der Daten und Qualifikationen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="2869a-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="2869a-183">\* Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="2869a-183">\*    View competencies</span></span>
||<span data-ttu-id="2869a-184">\* Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="2869a-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="2869a-185">\* Anzeigen und Erwerben von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="2869a-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="2869a-186">\* Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="2869a-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="2869a-187">\* Anzeigen von Daten zu Partnerbeitragsindikatoren</span><span class="sxs-lookup"><span data-stu-id="2869a-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="2869a-188">\* Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="2869a-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="2869a-189">\* Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="2869a-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="2869a-190">\* Anzeigen der Rollen anderer Benutzer im Unternehmen, kann jedoch seinerseits keine Rollen zuweisen</span><span class="sxs-lookup"><span data-stu-id="2869a-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="2869a-191">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-191">Account admin</span></span>| <span data-ttu-id="2869a-192">Hinzufügen von Speicherorten</span><span class="sxs-lookup"><span data-stu-id="2869a-192">Add locations</span></span>
|| <span data-ttu-id="2869a-193">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="2869a-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="2869a-194">\* Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="2869a-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="2869a-195">\* Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="2869a-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="2869a-196">Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="2869a-196">Manage referrals</span></span> 

|<span data-ttu-id="2869a-197">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="2869a-197">**Role**</span></span>|<span data-ttu-id="2869a-198">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="2869a-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="2869a-199">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-199">Referrals admin</span></span>       |<span data-ttu-id="2869a-200">\* Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="2869a-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="2869a-201">\* Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="2869a-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="2869a-202">\* Anzeigen, Erstellen und Verwalten von Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="2869a-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="2869a-203">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="2869a-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="2869a-204">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-204">Business profile admin</span></span>   |<span data-ttu-id="2869a-205">\* Anzeigen, Erstellen und Verwalten des Geschäftsprofils</span><span class="sxs-lookup"><span data-stu-id="2869a-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="2869a-206">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="2869a-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="2869a-207">Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="2869a-207">Manage incentives</span></span> 

|<span data-ttu-id="2869a-208">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="2869a-208">**Role**</span></span> | <span data-ttu-id="2869a-209">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="2869a-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="2869a-210">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="2869a-210">Incentives admin</span></span>|<span data-ttu-id="2869a-211">\* Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="2869a-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="2869a-212">\* Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="2869a-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="2869a-213">\* Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="2869a-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="2869a-214">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="2869a-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="2869a-215">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="2869a-215">\*    Access support</span></span>
||<span data-ttu-id="2869a-216">\* Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="2869a-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="2869a-217">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="2869a-217">Incentives user</span></span>|<span data-ttu-id="2869a-218">\* Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="2869a-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="2869a-219">\* Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="2869a-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="2869a-220">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="2869a-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="2869a-221">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="2869a-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="2869a-222">Anzeigen aussagekräftiger Daten zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="2869a-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="2869a-223">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="2869a-223">**Role**</span></span> | <span data-ttu-id="2869a-224">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="2869a-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="2869a-225">Executive Report-Leser</span><span class="sxs-lookup"><span data-stu-id="2869a-225">Executive report viewer</span></span>|<span data-ttu-id="2869a-226">Zugriff auf alle Berichtsdatasets</span><span class="sxs-lookup"><span data-stu-id="2869a-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="2869a-227">Berichtleser</span><span class="sxs-lookup"><span data-stu-id="2869a-227">Report viewer</span></span>|<span data-ttu-id="2869a-228">Zugriff auf Datenberichte mit Ausnahme von Umsatz-, Kunden- und personenbezogenen Mitarbeiterdaten</span><span class="sxs-lookup"><span data-stu-id="2869a-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    