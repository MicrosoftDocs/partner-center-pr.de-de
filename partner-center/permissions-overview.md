---
title: Zuweisen von Rollen und Berechtigungen zu Benutzern
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, welche Rollen am besten für Benutzer in Ihrem Unternehmen geeignet sind, die kommerzielle Transaktionen, Empfehlungen, Incentives oder MPN-Mitgliedschaften im Partner Center verwalten.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 964c0e6be3003c2b3c9da8828d6e896e2fff82f9
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756461"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen

**Geeignete Rollen**

- Globaler Administrator
- Benutzeradministrator
- MPN-Partneradministrator

Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet. Der nächste Schritt besteht in der Einrichtung von Kennwörtern und Rollen für Ihre Benutzer, damit diese gemeinsam mit Ihnen im Partner Center arbeiten können.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center

Wie Ihre Benutzer auf das Partner Center zugreifen können, bestimmen Sie über die Rollen und Berechtigungen, die Sie ihnen erteilen. Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist. Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die standardmäßigen Azure Active Directory-Rollen für die Mandantenverwaltung (z. B. „Globaler Administrator“), sondern benötigen auch spezifische Rollen für das CSP-Programm. Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.

>[!Note]
> Zu den Azure Active Directory-Mandantenrollen gehören die Rollen „Globaler Administrator“, „Benutzeradministrator“ und „CSP“. Nicht-Azure Active Directory-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Dazu zählen MPN-Administratoren, Geschäftsprofiladministratoren, Administratoren für Empfehlungen sowie Incentives-Administratoren und -Benutzer. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)

|**Rolle**|**Funktionsumfang**|**Weitere Informationen**|
|----------------------------------|---|:---------------------------------|
|Globaler Administrator|* Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen|[Verwalten des Partner Center-Kontos](partner-center-account-setup.md)
|      |* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets
||* Anzeigen von Vereinbarungen, Preislisten und Angeboten
||* Anzeigen, Erstellen und Verwalten von Partnerbenutzern|
||  Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien
|Benutzerverwaltungsadministrator   | * Anzeigen, Erstellen und Verwalten von Benutzern|[Verwalten von Microsoft Partner Network-Mitgliedschaftsvorteilen und -Angeboten im Partner Center](manage-your-partner-network-benefits.md)
||* Anzeigen aller Partnerprofile
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets
|Abrechnungsadministrator | • Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien|[Lesen Ihrer Rechnung](billing.md)
||* Anzeigen von Preisen
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets
|Standardbenutzer|  Anzeigen des eigenen Profils   |[Zurücksetzen Ihres Kennworts](reset-my-pasword.md)
|Administrator-Agent | * Kundenverwaltung|[Kontakt zu Ihren Kunden](connect-with-your-customers.md)
||* Hinzufügen einer Geräteliste zum Partner Center
||* Erstellen und Anwenden von Profilen auf Geräte
||* Abonnementverwaltung
||* Dienstintegrität und Serviceanfragen für Kunden
||* Anfordern delegierter Administratorrechte
||* Anzeigen von Preisen und Angeboten
||* Abrechnung
||* Verwalten im Auftrag eines Kunden
||* Registrieren eines Vertragshändlers
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets|
|Vertriebsbeauftragter | * Kundenverwaltung|[Bereitstellen von Abrechnungssupport für Kunden und Beantworten von Fragen zur Abrechnung](provide-billing-support.md)
||* Hinzufügen einer Geräteliste zum Partner Center
||* Abonnementverwaltung
||* Anzeigen von Supporttickets
||* Beantragen einer Partnerschaft mit einem Kunden
||* Anzeigen von Preisen und Angeboten
||* Verwalten potenzieller Kunden
||* Anzeigen der Kundenvereinbarung
||* Registrieren eines Vertragshändlers
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets|
|Helpdesk-Agent| * Suchen und Anzeigen von Kunden|[Eskalieren von Problemen an Microsoft und Bestimmen, welche Probleme besser für die Eskalation an Microsoft geeignet sind](escalate-problems-to-microsoft.md)
||* Bearbeiten von Kundendetails
||* Unterstützen von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung
||* Anfordern von Support für Kunden 
||* Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>CPV (Control Panel Vendor, (CSP-Rolle und Nicht-Azure AD-Rolle)

CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können. 

|**Rolle**   |**Funktionsumfang**|**Weitere Informationen**|
|------------------------------|:----------------------------|----|
|Globaler Administrator| Anzeigen und Verwalten Ihres CPV-Profils|[Registrieren als Control Panel Vendor, um die Integration von CSP-Partnersystemen in Partner Center-APIs zu unterstützen](enroll-as-cpv.md)
||Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Gastbenutzer (muss dem Azure Active Directory-Mandanten hinzugefügt werden)

|**Gastbenutzer**   | **Rollen**|
|---------------------------|:--------------------|
||MPN-Partneradministrator|
||Unternehmensprofiladministrator|
||Empfehlungsadministrator|


## <a name="manage-mpn-membership-and-your-company"></a>Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens 

Diese Rollen sind keine Azure Active Directory-Rollen. Mit diesen Rollen werden geschäftliche Aspekte und keine Mandanten verwaltet.

|**Rolle** | **Funktionsumfang**|**Weitere Informationen**|
|----------------------------|:----------------------------|-----|
|MPN-Partneradministrator|* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern|[Erwerben oder Verlängern eines Microsoft Action Pack-Abonnements oder der Silver- und Gold-Kompetenzen](mpn-get-action-pack.md)
||* Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen
||* Anzeigen der Daten und Qualifikationen von Benutzern
||* Anzeigen von Kompetenzen
||* Anzeigen und Verwalten von Vorteilen
||* Anzeigen und Erwerben von MPN-Angeboten
||* Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote
||* Anzeigen von Daten zu Partnerbeitragsindikatoren
||* Arbeiten im Gutscheinüberprüfungstool|
||* Anzeigen von Kundendatenanalysen
||* Anzeigen der Rollen anderer Benutzer im Unternehmen, kann jedoch seinerseits keine Rollen zuweisen
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets
|Kontoadministrator| Hinzufügen von Speicherorten|[Standorte verwalten](manage-locations.md)
|| • Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind 
||* Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-Azure Active Directory-Rollen 
||* Registrieren von Standorten in Programmen
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets

## <a name="manage-referrals"></a>Verwalten von Empfehlungen

|**Rolle** | **Funktionsumfang**|**Weitere Informationen**
|------------------------------|:-------------------------|---|
|Empfehlungsadministrator|Erstellen und Verwalten aller Einträge auf der Registerkarte „Empfehlungen“ im Partner Center|[Verwalten von Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
||    Anzeigen und Bearbeiten aller Co-Selling-Verkaufschancen und Leads
||    Zuweisen von Teammitgliedern für einen Deal
||    Anzeigen und Bearbeiten von Geschäftsprofilen
||    Anzeigen und Registrieren von Deals für Verkaufschancen, die als gewonnen markiert und für die Dealregistrierung zugelassen sind
||    Erstellen und Anzeigen von Supporttickets
|Empfehlungsbenutzer|Erstellen und Verwalten von Co-Selling-Verkaufschancen nur, wenn sie Teil des Teams sind |[Verwalten von Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
||    Erstellen von Co-Selling-Verkaufschancen für die Standorte, an denen ihnen die Rolle zugewiesen ist
||    Anzeigen und Registrieren von Deals für Verkaufschancen, die als gewonnen markiert und für die Dealregistrierung zugelassen sind, wenn sie Teammitglieder sind
||    Erstellen und Anzeigen von Supporttickets
|Unternehmensprofiladministrator|Erstellen und Verwalten von Geschäftsprofilen | [Verwalten von Geschäftsprofilen](create-a-marketing-profile.md)
||    Erstellen und Anzeigen von Supporttickets

Zusammen mit der neuen Benutzerrolle für Empfehlungen wird auch der Standortbereich für Deals eingeführt. In der folgenden Tabelle wird der Zugriff auf Deals basierend auf dem Standort erläutert.

|**Scope** | **Funktionsumfang** |
|------------------------------|:-------------------------|
|Gesamtes Unternehmen | Sowohl Administratoren als auch Benutzer haben Zugriff zum Erstellen von Deals für jeden Standort in Ihrem Unternehmen.|
|| Der Empfehlungsadministrator hat Zugriff zum Anzeigen und Bearbeiten aller Deals. |
|| Empfehlungsbenutzer haben nur dann Zugriff zum Anzeigen und Bearbeiten aller Deals, wenn Sie Teil des Teams sind. |
|Ein oder mehrere Standorte | Sowohl Administratoren als auch Benutzer haben Zugriff zum Erstellen von Deals für den zugewiesenen Standort in Ihrem Unternehmen.|
|| Der Empfehlungsadministrator hat Zugriff zum Anzeigen und Bearbeiten aller Deals, die zu den zugewiesenen Standorten gehören.|
|| Empfehlungsbenutzer haben Zugriff zum Anzeigen und Bearbeiten aller Deals, die zu den zugewiesenen Standorten gehören, wenn Sie Teil des Teams sind.|

## <a name="manage-incentives"></a>Verwalten von Incentives

|**Rolle** | **Funktionsumfang**|**Weitere Informationen**
|------------------------------|:-------------------------|---|
|Incentiveadministrator|* Initiieren und Verwalten von Incentives |[Hilfreiche Ressourcen für den Einstieg in Incentives](incentives-get-started-intro.md)
||* Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen
||* Anzeigen und Bearbeiten von Bank- und Steuerdaten
||* Anzeigen von Rabatten und Co-Op-Erträgen
||* Zugreifen auf den Support
||* Konfliktlösung bei Incentivezahlungen|
|Incentivebenutzer|* Anzeigen von Incentiveprogrammen
||* Anzeigen und Initiieren von Incentiveansprüchen
||* Anzeigen von Rabatten und Co-Op-Erträgen
||* Erstellen von Supporttickets für das Partner Center
||* Anzeigen erstellter Partnersupporttickets

## <a name="view-partner-center-insights-data"></a>Anzeigen aussagekräftiger Daten zum Partner Center

|**Rolle** | **Funktionsumfang**|**Weitere Informationen**|
|------------------------------|:-------------------------|---|
|Executive Report-Leser|Zugriff auf alle Berichtsdatasets, Erstellen von Partnersupporttickets, Anzeigen erstellter Partnersupporttickets|[Partner Center-Einblicke – Berichte im Dashboard „Übersicht“](pci-overview-report.md)
|Berichtleser|Zugriff auf Datenberichte mit Ausnahme von Umsatz-, Kunden- und personenbezogenen Mitarbeiterdaten, Erstellen von Partnersupporttickets, Anzeigen erstellter Partnersupporttickets|

## <a name="next-steps"></a>Nächste Schritte

- [Erstellen von Benutzerkonten und Zuweisen von Rollen und Berechtigungen](create-user-accounts-and-set-permissions.md)
- [Überprüfen der Kontoinformationen bei der Registrierung für ein neues Partner Center-Programm](verification-responses.md)
