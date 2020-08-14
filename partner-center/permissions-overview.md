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
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839185"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="835fe-103">Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen</span><span class="sxs-lookup"><span data-stu-id="835fe-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="835fe-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="835fe-104">**Appropriate roles**</span></span>

- <span data-ttu-id="835fe-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="835fe-105">Global admin</span></span>
- <span data-ttu-id="835fe-106">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-106">User admin</span></span>
- <span data-ttu-id="835fe-107">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-107">MPN partner admin</span></span>

<span data-ttu-id="835fe-108">Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="835fe-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="835fe-109">Der nächste Schritt besteht in der Einrichtung von Kennwörtern und Rollen für Ihre Benutzer, damit diese gemeinsam mit Ihnen im Partner Center arbeiten können.</span><span class="sxs-lookup"><span data-stu-id="835fe-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="835fe-110">Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center</span><span class="sxs-lookup"><span data-stu-id="835fe-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="835fe-111">Wie Ihre Benutzer auf das Partner Center zugreifen können, bestimmen Sie über die Rollen und Berechtigungen, die Sie ihnen erteilen.</span><span class="sxs-lookup"><span data-stu-id="835fe-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="835fe-112">Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist.</span><span class="sxs-lookup"><span data-stu-id="835fe-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="835fe-113">Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm.</span><span class="sxs-lookup"><span data-stu-id="835fe-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="835fe-114">Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.</span><span class="sxs-lookup"><span data-stu-id="835fe-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="835fe-115">Zu den AAD-Mandantenrollen (Azure Active Directory) gehören die Rollen „Globaler Administrator“, „Benutzeradministrator“ und „CSP“.</span><span class="sxs-lookup"><span data-stu-id="835fe-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="835fe-116">Nicht-AAD-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Zu ihnen gehören MPN-Administratoren, Geschäftsprofiladministratoren, Empfehlungsadministratoren, Prämienadministratoren und Prämienbenutzer.</span><span class="sxs-lookup"><span data-stu-id="835fe-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="835fe-117">Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)</span><span class="sxs-lookup"><span data-stu-id="835fe-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="835fe-118">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="835fe-118">**Role**</span></span>|<span data-ttu-id="835fe-119">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="835fe-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="835fe-120">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="835fe-120">Global admin</span></span>|<span data-ttu-id="835fe-121">\* Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="835fe-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="835fe-122">\* Erstellen von Supporttickets für das Partner Center</span><span class="sxs-lookup"><span data-stu-id="835fe-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="835fe-123">\* Anzeigen von Vereinbarungen, Preislisten und Angeboten</span><span class="sxs-lookup"><span data-stu-id="835fe-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="835fe-124">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="835fe-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="835fe-125">Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="835fe-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="835fe-126">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-126">User management admin</span></span>   | <span data-ttu-id="835fe-127">\* Anzeigen, Erstellen und Verwalten von Benutzern</span><span class="sxs-lookup"><span data-stu-id="835fe-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="835fe-128">\* Anzeigen aller Partnerprofile</span><span class="sxs-lookup"><span data-stu-id="835fe-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="835fe-129">\* Anzeigen, Erstellen und Verwalten von Partnerbenutzern</span><span class="sxs-lookup"><span data-stu-id="835fe-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="835fe-130">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-130">Billing admin</span></span> | <span data-ttu-id="835fe-131">• Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="835fe-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="835fe-132">\* Anzeigen von Preisen</span><span class="sxs-lookup"><span data-stu-id="835fe-132">\*    View pricing</span></span>
|<span data-ttu-id="835fe-133">Standardbenutzer</span><span class="sxs-lookup"><span data-stu-id="835fe-133">Default user</span></span>|  <span data-ttu-id="835fe-134">Anzeigen des eigenen Profils</span><span class="sxs-lookup"><span data-stu-id="835fe-134">View My profile</span></span>   |
|<span data-ttu-id="835fe-135">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="835fe-135">Admin agent</span></span> | <span data-ttu-id="835fe-136">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="835fe-136">\*    Customer management</span></span>
||<span data-ttu-id="835fe-137">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="835fe-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="835fe-138">\* Erstellen und Anwenden von Profilen auf Geräte</span><span class="sxs-lookup"><span data-stu-id="835fe-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="835fe-139">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="835fe-139">\*    Subscription management</span></span>
||<span data-ttu-id="835fe-140">\* Dienstintegrität und Serviceanfragen für Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="835fe-141">\* Anfordern delegierter Administratorrechte</span><span class="sxs-lookup"><span data-stu-id="835fe-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="835fe-142">\* Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="835fe-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="835fe-143">\* Abrechnung</span><span class="sxs-lookup"><span data-stu-id="835fe-143">\*    Billing</span></span>
||<span data-ttu-id="835fe-144">\* Verwalten im Auftrag eines Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="835fe-145">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="835fe-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="835fe-146">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="835fe-146">Sales agent</span></span> | <span data-ttu-id="835fe-147">\* Kundenverwaltung</span><span class="sxs-lookup"><span data-stu-id="835fe-147">\*    Customer management</span></span>
||<span data-ttu-id="835fe-148">\* Hinzufügen einer Geräteliste zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="835fe-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="835fe-149">\* Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="835fe-149">\*    Subscription management</span></span>
||<span data-ttu-id="835fe-150">\* Anzeigen von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="835fe-150">\*    View support tickets</span></span>
||<span data-ttu-id="835fe-151">\* Beantragen einer Partnerschaft mit einem Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="835fe-152">\* Anzeigen von Preisen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="835fe-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="835fe-153">\* Verwalten potenzieller Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="835fe-154">\* Anzeigen der Kundenvereinbarung</span><span class="sxs-lookup"><span data-stu-id="835fe-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="835fe-155">\* Registrieren eines Vertragshändlers</span><span class="sxs-lookup"><span data-stu-id="835fe-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="835fe-156">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="835fe-156">Helpdesk agent</span></span>| <span data-ttu-id="835fe-157">\* Suchen und Anzeigen von Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="835fe-158">\* Bearbeiten von Kundendetails</span><span class="sxs-lookup"><span data-stu-id="835fe-158">\*    Edit customer details</span></span>
||<span data-ttu-id="835fe-159">\* Unterstützen von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung</span><span class="sxs-lookup"><span data-stu-id="835fe-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="835fe-160">\* Anfordern von Support für Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="835fe-161">\* Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden</span><span class="sxs-lookup"><span data-stu-id="835fe-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="835fe-162">CPV (Control Panel Vendor,</span><span class="sxs-lookup"><span data-stu-id="835fe-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="835fe-163">CSP- und Nicht-AAD-Rolle)</span><span class="sxs-lookup"><span data-stu-id="835fe-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="835fe-164">CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können.</span><span class="sxs-lookup"><span data-stu-id="835fe-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="835fe-165">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="835fe-165">**Role**</span></span>   |<span data-ttu-id="835fe-166">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="835fe-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="835fe-167">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="835fe-167">Global admin</span></span>| <span data-ttu-id="835fe-168">Anzeigen und Verwalten Ihres CPV-Profils</span><span class="sxs-lookup"><span data-stu-id="835fe-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="835fe-169">Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen</span><span class="sxs-lookup"><span data-stu-id="835fe-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="835fe-170">Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)</span><span class="sxs-lookup"><span data-stu-id="835fe-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="835fe-171">**Gastbenutzer**</span><span class="sxs-lookup"><span data-stu-id="835fe-171">**Guest user**</span></span>   | <span data-ttu-id="835fe-172">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="835fe-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="835fe-173">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-173">MPN partner admin</span></span>|
||<span data-ttu-id="835fe-174">Kontenadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-174">Accounts admin</span></span>|
||<span data-ttu-id="835fe-175">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-175">Incentives admin</span></span>|
||<span data-ttu-id="835fe-176">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-176">Business profile admin</span></span>|
||<span data-ttu-id="835fe-177">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="835fe-178">Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (Nicht-AAD-Rollen, die zur Verwaltung auf Unternehmens- statt auf Mandantenebene verwendet werden)</span><span class="sxs-lookup"><span data-stu-id="835fe-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="835fe-179">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="835fe-179">**Role**</span></span> | <span data-ttu-id="835fe-180">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="835fe-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="835fe-181">MPN-Partneradministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-181">MPN partner admin</span></span>|<span data-ttu-id="835fe-182">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="835fe-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="835fe-183">\* Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen</span><span class="sxs-lookup"><span data-stu-id="835fe-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="835fe-184">\* Anzeigen der Daten und Qualifikationen von Benutzern</span><span class="sxs-lookup"><span data-stu-id="835fe-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="835fe-185">\* Anzeigen von Kompetenzen</span><span class="sxs-lookup"><span data-stu-id="835fe-185">\*    View competencies</span></span>
||<span data-ttu-id="835fe-186">\* Anzeigen und Verwalten von Vorteilen</span><span class="sxs-lookup"><span data-stu-id="835fe-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="835fe-187">\* Anzeigen und Erwerben von MPN-Angeboten</span><span class="sxs-lookup"><span data-stu-id="835fe-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="835fe-188">\* Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote</span><span class="sxs-lookup"><span data-stu-id="835fe-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="835fe-189">\* Anzeigen von Daten zu Partnerbeitragsindikatoren</span><span class="sxs-lookup"><span data-stu-id="835fe-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="835fe-190">\* Arbeiten im Gutscheinüberprüfungstool</span><span class="sxs-lookup"><span data-stu-id="835fe-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="835fe-191">\* Anzeigen von Kundendatenanalysen</span><span class="sxs-lookup"><span data-stu-id="835fe-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="835fe-192">\* Anzeigen der Rollen anderer Benutzer im Unternehmen, kann jedoch seinerseits keine Rollen zuweisen</span><span class="sxs-lookup"><span data-stu-id="835fe-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="835fe-193">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-193">Account admin</span></span>| <span data-ttu-id="835fe-194">Hinzufügen von Speicherorten</span><span class="sxs-lookup"><span data-stu-id="835fe-194">Add locations</span></span>
|| <span data-ttu-id="835fe-195">• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind</span><span class="sxs-lookup"><span data-stu-id="835fe-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="835fe-196">\* Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen</span><span class="sxs-lookup"><span data-stu-id="835fe-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="835fe-197">\* Registrieren von Standorten in Programmen</span><span class="sxs-lookup"><span data-stu-id="835fe-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="835fe-198">Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="835fe-198">Manage referrals</span></span> 

|<span data-ttu-id="835fe-199">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="835fe-199">**Role**</span></span>|<span data-ttu-id="835fe-200">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="835fe-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="835fe-201">Empfehlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-201">Referrals admin</span></span>       |<span data-ttu-id="835fe-202">\* Anzeigen, Erstellen und Verwalten von Geschäftsprofilen</span><span class="sxs-lookup"><span data-stu-id="835fe-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="835fe-203">\* Empfangen und Verwalten von Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="835fe-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="835fe-204">\* Anzeigen, Erstellen und Verwalten von Co-Selling-Empfehlungen</span><span class="sxs-lookup"><span data-stu-id="835fe-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="835fe-205">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="835fe-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="835fe-206">Unternehmensprofiladministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-206">Business profile admin</span></span>   |<span data-ttu-id="835fe-207">\* Anzeigen, Erstellen und Verwalten des Geschäftsprofils</span><span class="sxs-lookup"><span data-stu-id="835fe-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="835fe-208">\* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern</span><span class="sxs-lookup"><span data-stu-id="835fe-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="835fe-209">Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="835fe-209">Manage incentives</span></span> 

|<span data-ttu-id="835fe-210">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="835fe-210">**Role**</span></span> | <span data-ttu-id="835fe-211">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="835fe-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="835fe-212">Incentiveadministrator</span><span class="sxs-lookup"><span data-stu-id="835fe-212">Incentives admin</span></span>|<span data-ttu-id="835fe-213">\* Initiieren und Verwalten von Incentives</span><span class="sxs-lookup"><span data-stu-id="835fe-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="835fe-214">\* Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="835fe-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="835fe-215">\* Anzeigen und Bearbeiten von Bank- und Steuerdaten</span><span class="sxs-lookup"><span data-stu-id="835fe-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="835fe-216">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="835fe-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="835fe-217">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="835fe-217">\*    Access support</span></span>
||<span data-ttu-id="835fe-218">\* Konfliktlösung bei Incentivezahlungen</span><span class="sxs-lookup"><span data-stu-id="835fe-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="835fe-219">Incentivebenutzer</span><span class="sxs-lookup"><span data-stu-id="835fe-219">Incentives user</span></span>|<span data-ttu-id="835fe-220">\* Anzeigen von Incentiveprogrammen</span><span class="sxs-lookup"><span data-stu-id="835fe-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="835fe-221">\* Anzeigen und Initiieren von Incentiveansprüchen</span><span class="sxs-lookup"><span data-stu-id="835fe-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="835fe-222">\* Anzeigen von Rabatten und Co-Op-Erträgen</span><span class="sxs-lookup"><span data-stu-id="835fe-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="835fe-223">\* Zugreifen auf den Support</span><span class="sxs-lookup"><span data-stu-id="835fe-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="835fe-224">Anzeigen aussagekräftiger Daten zum Partner Center</span><span class="sxs-lookup"><span data-stu-id="835fe-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="835fe-225">**Rolle**</span><span class="sxs-lookup"><span data-stu-id="835fe-225">**Role**</span></span> | <span data-ttu-id="835fe-226">**Funktionsumfang**</span><span class="sxs-lookup"><span data-stu-id="835fe-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="835fe-227">Executive Report-Leser</span><span class="sxs-lookup"><span data-stu-id="835fe-227">Executive report viewer</span></span>|<span data-ttu-id="835fe-228">Zugriff auf alle Berichtsdatasets</span><span class="sxs-lookup"><span data-stu-id="835fe-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="835fe-229">Berichtleser</span><span class="sxs-lookup"><span data-stu-id="835fe-229">Report viewer</span></span>|<span data-ttu-id="835fe-230">Zugriff auf Datenberichte mit Ausnahme von Umsatz-, Kunden- und personenbezogenen Mitarbeiterdaten</span><span class="sxs-lookup"><span data-stu-id="835fe-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
