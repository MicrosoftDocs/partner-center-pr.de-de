---
title: Zuweisen von Rollen und Berechtigungen zu Benutzern
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, welche Rollen am besten für Benutzer in Ihrem Unternehmen geeignet sind, die kommerzielle Transaktionen, Empfehlungen, Incentives oder MPN-Mitgliedschaften im Partner Center verwalten.
author: hemas
ms.author: hemas
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4f4ec3a1a14e6845f7b6079e286876d9bb1f3dd5
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948591"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Zuweisen von Rollen und Berechtigungen zu Benutzern im Unternehmen, die im Partner Center arbeiten müssen

**Geeignete Rollen**

- Globaler Administrator
- Benutzeradministrator
- MPN-Partneradministrator

Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet. Der nächste Schritt besteht in der Einrichtung von Kennwörtern und Rollen für Ihre Benutzer, damit diese gemeinsam mit Ihnen im Partner Center arbeiten können.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center

Wie Ihre Benutzer auf das Partner Center zugreifen können, bestimmen Sie über die Rollen und Berechtigungen, die Sie ihnen erteilen. Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist. Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm. Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.

>[!Note]
> Zu den AAD-Mandantenrollen (Azure Active Directory) gehören die Rollen „Globaler Administrator“, „Benutzeradministrator“ und „CSP“. Nicht-AAD-Rollen sind Rollen, die keine Verwaltung des Mandanten umfassen. Zu ihnen gehören MPN-Administratoren, Geschäftsprofiladministratoren, Empfehlungsadministratoren, Prämienadministratoren und Prämienbenutzer. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)

|**Rolle**|**Funktionsumfang**|
|----------------------------------|:---------------------------------|
|Globaler Administrator|* Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen
|      |* Erstellen von Supporttickets für das Partner Center
||* Anzeigen von Vereinbarungen, Preislisten und Angeboten
||* Anzeigen, Erstellen und Verwalten von Partnerbenutzern|
||  Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien
|Benutzerverwaltungsadministrator   | * Anzeigen, Erstellen und Verwalten von Benutzern
||* Anzeigen aller Partnerprofile
||* Anzeigen, Erstellen und Verwalten von Partnerbenutzern  |
|Abrechnungsadministrator | • Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien|
|Standardbenutzer|  Anzeigen des eigenen Profils   |
|Administrator-Agent | * Kundenverwaltung
||* Hinzufügen einer Geräteliste zum Partner Center
||* Erstellen und Anwenden von Profilen auf Geräte
||* Abonnementverwaltung
||* Dienstintegrität und Serviceanfragen für Kunden
||* Anfordern delegierter Administratorrechte
||* Anzeigen von Preisen und Angeboten
||* Abrechnung
||* Verwalten im Auftrag eines Kunden
||* Registrieren eines Vertragshändlers|
|Vertriebsbeauftragter | * Kundenverwaltung
||* Hinzufügen einer Geräteliste zum Partner Center
||* Abonnementverwaltung
||* Anzeigen von Supporttickets
||* Beantragen einer Partnerschaft mit einem Kunden
||* Verwalten potenzieller Kunden
||* Anzeigen der Kundenvereinbarung
||* Registrieren eines Vertragshändlers|
|Helpdesk-Agent| * Suchen und Anzeigen von Kunden
||* Bearbeiten von Kundendetails
||* Unterstützen von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung
||* Anfordern von Support für Kunden 
||* Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>CPV (Control Panel Vendor, CSP- und Nicht-AAD-Rolle)
CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können. 

|**Rolle**   |**Funktionsumfang**|
|------------------------------|:----------------------------|
|Globaler Administrator| Anzeigen und Verwalten Ihres CPV-Profils|
||Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)

|**Gastbenutzer**   | **Rollen**|
|---------------------------|:--------------------|
||MPN-Partneradministrator|
||Kontenadministrator|
||Incentiveadministrator|
||Unternehmensprofiladministrator|
||Empfehlungsadministrator|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (Nicht-AAD-Rollen, die zur Verwaltung auf Unternehmens- statt auf Mandantenebene verwendet werden)

|**Rolle** | **Funktionsumfang**|
|----------------------------|:----------------------------|
|MPN-Partneradministrator|* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern||
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
|Kontoadministrator| Hinzufügen von Speicherorten
|| • Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind 
||* Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen 
||* Registrieren von Standorten in Programmen


## <a name="manage-referrals"></a>Verwalten von Empfehlungen 

|**Rolle**|**Funktionsumfang**|
|-----------------------------|:------------------------|
|Empfehlungsadministrator       |* Anzeigen, Erstellen und Verwalten von Geschäftsprofilen
||* Empfangen und Verwalten von Empfehlungen
||* Anzeigen, Erstellen und Verwalten von Co-Selling-Empfehlungen|
||* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern
|Unternehmensprofiladministrator   |* Anzeigen, Erstellen und Verwalten des Geschäftsprofils 
||* Anzeigen, Erstellen und Verwalten von Serviceanfragen von Partnern|

## <a name="manage-incentives"></a>Verwalten von Incentives 

|**Rolle** | **Funktionsumfang**|
|------------------------------|:-------------------------|
|Incentiveadministrator|* Initiieren und Verwalten von Incentives 
||* Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen
||* Anzeigen und Bearbeiten von Bank- und Steuerdaten
||* Anzeigen von Rabatten und Co-Op-Erträgen
||* Zugreifen auf den Support
||* Konfliktlösung bei Incentivezahlungen|
|Incentivebenutzer|* Anzeigen von Incentiveprogrammen
||* Anzeigen und Initiieren von Incentiveansprüchen
||* Anzeigen von Rabatten und Co-Op-Erträgen
||* Zugreifen auf den Support

## <a name="view-partner-center-insights-data"></a>Anzeigen aussagekräftiger Daten zum Partner Center

|**Rolle** | **Funktionsumfang**|
|------------------------------|:-------------------------|
|Executive Report-Leser|Zugriff auf alle Berichtsdatasets|
|Berichtleser|Zugriff auf Datenberichte mit Ausnahme von Umsatz-, Kunden- und personenbezogenen Mitarbeiterdaten|












                                    