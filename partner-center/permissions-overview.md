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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040766"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="cfbc0-103">Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="cfbc0-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="cfbc0-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-105">Global admin</span></span>
- <span data-ttu-id="cfbc0-106">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-106">User admin</span></span>
- <span data-ttu-id="cfbc0-107">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-107">MPN partner admin</span></span>

<span data-ttu-id="cfbc0-108">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="cfbc0-109">Der nächste Schritt besteht in der Einrichtung von Kennwörtern und Rollen für Ihre Benutzer, damit diese gemeinsam mit Ihnen im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="cfbc0-110">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="cfbc0-111">Wie Ihre Benutzer auf das Partner Center zugreifen können, bestimmen Sie über die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="cfbc0-112">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="cfbc0-113">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="cfbc0-114">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="cfbc0-115">Zu den AAD-Mandantenrollen (Azure Active Directory) gehören die Rollen „Globaler Administrator“, „Benutzeradministrator“ und „CSP“.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="cfbc0-116">Nicht-AAD-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Zu ihnen gehören MPN-Administratoren, Geschäftsprofiladministratoren, Empfehlungsadministratoren, Prämienadministratoren und Prämienbenutzer.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="cfbc0-117">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="cfbc0-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="cfbc0-118">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-118">**Role**</span></span>|<span data-ttu-id="cfbc0-119">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="cfbc0-120">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-120">Global admin</span></span>|<span data-ttu-id="cfbc0-121">\* Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="cfbc0-122">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-123">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="cfbc0-124">\* Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="cfbc0-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="cfbc0-125">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="cfbc0-126">Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="cfbc0-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="cfbc0-127">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-127">User management admin</span></span>   | <span data-ttu-id="cfbc0-128">\* Anzeigen, Erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="cfbc0-129">\* Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="cfbc0-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="cfbc0-130">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="cfbc0-131">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-132">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="cfbc0-133">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-133">Billing admin</span></span> | <span data-ttu-id="cfbc0-134">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="cfbc0-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="cfbc0-135">\* Anzeigen von Preisen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-135">\*    View pricing</span></span>
||<span data-ttu-id="cfbc0-136">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-137">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="cfbc0-138">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="cfbc0-138">Default user</span></span>|  <span data-ttu-id="cfbc0-139">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="cfbc0-139">View My profile</span></span>   |
|<span data-ttu-id="cfbc0-140">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="cfbc0-140">Admin agent</span></span> | <span data-ttu-id="cfbc0-141">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-141">\*    Customer management</span></span>
||<span data-ttu-id="cfbc0-142">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="cfbc0-143">\* Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="cfbc0-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="cfbc0-144">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-144">\*    Subscription management</span></span>
||<span data-ttu-id="cfbc0-145">\* Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="cfbc0-146">\* Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="cfbc0-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="cfbc0-147">\* Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="cfbc0-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="cfbc0-148">\* Abrechnung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-148">\*    Billing</span></span>
||<span data-ttu-id="cfbc0-149">\* Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="cfbc0-150">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="cfbc0-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="cfbc0-151">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-152">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="cfbc0-153">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="cfbc0-153">Sales agent</span></span> | <span data-ttu-id="cfbc0-154">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-154">\*    Customer management</span></span>
||<span data-ttu-id="cfbc0-155">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="cfbc0-156">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-156">\*    Subscription management</span></span>
||<span data-ttu-id="cfbc0-157">\* Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-157">\*    View support tickets</span></span>
||<span data-ttu-id="cfbc0-158">\* Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="cfbc0-159">\* Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="cfbc0-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="cfbc0-160">\* Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="cfbc0-161">\* Anzeigen der Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="cfbc0-162">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="cfbc0-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="cfbc0-163">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-164">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="cfbc0-165">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="cfbc0-165">Helpdesk agent</span></span>| <span data-ttu-id="cfbc0-166">\* Suchen und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="cfbc0-167">\* Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="cfbc0-167">\*    Edit customer details</span></span>
||<span data-ttu-id="cfbc0-168">\* Unterstützen von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="cfbc0-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="cfbc0-169">\* Anfordern von Support für Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="cfbc0-170">\* Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden</span><span class="sxs-lookup"><span data-stu-id="cfbc0-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="cfbc0-171">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-172">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="cfbc0-173">CPV (Control Panel Vendor,</span><span class="sxs-lookup"><span data-stu-id="cfbc0-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="cfbc0-174">CSP- und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="cfbc0-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="cfbc0-175">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="cfbc0-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="cfbc0-176">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-176">**Role**</span></span>   |<span data-ttu-id="cfbc0-177">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="cfbc0-178">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-178">Global admin</span></span>| <span data-ttu-id="cfbc0-179">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="cfbc0-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="cfbc0-180">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="cfbc0-181">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="cfbc0-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="cfbc0-182">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-182">**Guest user**</span></span>   | <span data-ttu-id="cfbc0-183">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="cfbc0-184">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-184">MPN partner admin</span></span>|
||<span data-ttu-id="cfbc0-185">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-185">Accounts admin</span></span>|
||<span data-ttu-id="cfbc0-186">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-186">Incentives admin</span></span>|
||<span data-ttu-id="cfbc0-187">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-187">Business profile admin</span></span>|
||<span data-ttu-id="cfbc0-188">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="cfbc0-189">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (Nicht-AAD-Rollen, die zur Verwaltung auf Unternehmens- statt auf Mandantenebene verwendet werden)</span><span class="sxs-lookup"><span data-stu-id="cfbc0-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="cfbc0-190">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-190">**Role**</span></span> | <span data-ttu-id="cfbc0-191">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="cfbc0-192">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-192">MPN partner admin</span></span>|<span data-ttu-id="cfbc0-193">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="cfbc0-194">\* Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="cfbc0-195">\* Anzeigen der Daten und Qualifikationen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="cfbc0-196">\* Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-196">\*    View competencies</span></span>
||<span data-ttu-id="cfbc0-197">\* Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="cfbc0-198">\* Anzeigen und Erwerben von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="cfbc0-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="cfbc0-199">\* Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="cfbc0-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="cfbc0-200">\* Anzeigen von Daten zu Partnerbeitragsindikatoren</span><span class="sxs-lookup"><span data-stu-id="cfbc0-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="cfbc0-201">\* Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="cfbc0-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="cfbc0-202">\* Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="cfbc0-203">\* Anzeigen der Rollen anderer Benutzer im Unternehmen, kann jedoch seinerseits keine Rollen zuweisen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="cfbc0-204">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-205">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="cfbc0-206">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-206">Account admin</span></span>| <span data-ttu-id="cfbc0-207">Hinzufügen von Speicherorten</span><span class="sxs-lookup"><span data-stu-id="cfbc0-207">Add locations</span></span>
|| <span data-ttu-id="cfbc0-208">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="cfbc0-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="cfbc0-209">\* Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="cfbc0-210">\* Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="cfbc0-211">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-212">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="cfbc0-213">Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-213">Manage referrals</span></span> 

|<span data-ttu-id="cfbc0-214">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-214">**Role**</span></span>|<span data-ttu-id="cfbc0-215">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="cfbc0-216">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-216">Referrals admin</span></span>       |<span data-ttu-id="cfbc0-217">\* Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="cfbc0-218">\* Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="cfbc0-219">\* Anzeigen, Erstellen und Verwalten von Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="cfbc0-220">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="cfbc0-221">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-221">Business profile admin</span></span>   |<span data-ttu-id="cfbc0-222">\* Anzeigen, Erstellen und Verwalten des Geschäftsprofils</span><span class="sxs-lookup"><span data-stu-id="cfbc0-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="cfbc0-223">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="cfbc0-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="cfbc0-224">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-225">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="cfbc0-226">Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="cfbc0-226">Manage incentives</span></span> 

|<span data-ttu-id="cfbc0-227">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-227">**Role**</span></span> | <span data-ttu-id="cfbc0-228">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="cfbc0-229">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="cfbc0-229">Incentives admin</span></span>|<span data-ttu-id="cfbc0-230">\* Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="cfbc0-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="cfbc0-231">\* Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="cfbc0-232">\* Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="cfbc0-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="cfbc0-233">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="cfbc0-234">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="cfbc0-234">\*    Access support</span></span>
||<span data-ttu-id="cfbc0-235">\* Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="cfbc0-236">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="cfbc0-236">Incentives user</span></span>|<span data-ttu-id="cfbc0-237">\* Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="cfbc0-238">\* Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="cfbc0-239">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="cfbc0-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="cfbc0-240">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cfbc0-241">\* Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="cfbc0-242">Anzeigen aussagekräftiger Daten zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbc0-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="cfbc0-243">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-243">**Role**</span></span> | <span data-ttu-id="cfbc0-244">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="cfbc0-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="cfbc0-245">Executive Report-Leser</span><span class="sxs-lookup"><span data-stu-id="cfbc0-245">Executive report viewer</span></span>|<span data-ttu-id="cfbc0-246">Zugriff auf alle Berichtsdatasets, Erstellen von Partnersupporttickets, Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="cfbc0-247">Berichtleser</span><span class="sxs-lookup"><span data-stu-id="cfbc0-247">Report viewer</span></span>|<span data-ttu-id="cfbc0-248">Zugriff auf Datenberichte mit Ausnahme von Umsatz-, Kunden- und personenbezogenen Mitarbeiterdaten, Erstellen von Partnersupporttickets, Anzeigen erstellter Partnersupporttickets</span><span class="sxs-lookup"><span data-stu-id="cfbc0-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
