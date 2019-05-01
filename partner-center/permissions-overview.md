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
# <a name="assign-users-roles-and-permissions"></a>Zuweisen von Rollen und Berechtigungen zu Benutzern


Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet. Nächster Schritt: Einrichten der Benutzer mit Kennwörtern und Rollen, damit sie mit Ihnen gemeinsam im Partner Center arbeiten können.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center

Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen. Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist. Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm. Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.

>[!Note]
> AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen. Zu den Nicht-AAD-Rollen gehören MPN-Administrator, Geschäftsprofiladministrator, Empfehlungsadministrator, Incentiveadministrator und Incentivebenutzer. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)

|**Rolle**|**Funktionsumfang**|
|----------------------------------|:---------------------------------|
|Globaler Administrator|• Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen
|      |• Erstellen von Supportanfragen für das Partner Center
||• Anzeigen von Vereinbarungen, Preislisten und Angeboten
||• Anzeigen, Erstellen und Verwalten von Partnerbenutzern|
|Benutzeradministrator   | • Anzeigen, Erstellen und Verwalten von Benutzern
||• Anzeigen aller Partnerprofile
||• Anzeigen, Erstellen und Verwalten von Partnerbenutzern  |
|Abrechnungsadministrator | • Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien|
|Standardbenutzer|  Anzeigen des eigenen Profils   |
|Administrator-Agent | • Kundenverwaltung
||• Hinzufügen einer Geräteliste zum Partner Center
||• Erstellen und Anwenden von Profilen auf Geräte
||• Abonnementverwaltung
||• Dienstintegrität und Serviceanfragen für Kunden
||• Anfordern delegierter Administratorrechte
||• Anzeigen von Preisen und Angeboten
||• Abrechnung
||• Verwalten im Auftrag eines Kunden
||• Registrieren eines Vertragshändlers|
|Vertriebsbeauftragter | • Kundenverwaltung
||• Hinzufügen einer Geräteliste zum Partner Center
||• Abonnementverwaltung
||• Anzeigen von Supporttickets
||• Beantragen einer Partnerschaft mit einem Kunden
||• Verwalten potenzieller Kunden
||• Anzeigen des Kundenvertrags
||• Registrieren eines Vertragshändlers|
|Helpdesk-Agent| • Suchen nach und Anzeigen von Kunden
||• Bearbeiten von Kundendetails
||• Unterstützten von Kunden beim Lösen von Problemen mit der Abrechnung oder der Abonnementverwaltung
||• Anfordern von Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)
||• Verwalten von Abonnements und Abrechnungsproblemen im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent sein, um diese Aufgabe für Office 365-Abonnements ausführen zu können)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>CPV (Control Panel Vendor). (CSP-Rolle und Nicht-AAD-Rolle)
CPVs entwickeln Apps für die Verwendung durch CSP-Partner (Cloud Solution Provider), damit diese ihre Systeme mit Partner Center-APIs integrieren können. 

|**Rolle**   |**Funktionsumfang**|
|------------------------------|:----------------------------|
|Globaler Administrator| Anzeigen und Verwalten Ihres CPV-Profils|
||Anzeigen und Verwalten der Benutzer, die Zugriff auf CPV Funktionen benötigen|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Verwalten der MPN-Mitgliedschaft und Ihres Unternehmens (Nicht-AAD-Rollen)

|**Rolle** | **Funktionsumfang**|
|----------------------------|:----------------------------|
|MPN-Partneradministrator|• Hinzufügen von Nicht-Mandantenbenutzern
||• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner
||• Anzeigen von rechtlichen, unternehmerischen, geschäftlichen und MPN-Profilen
||• Anzeigen der Daten und Fähigkeiten von Benutzern
||• Anzeigen von Kompetenzen
||• Anzeigen und Verwalten von Vorteilen
||• Anzeigen und Kaufen von MPN-Angeboten
||• Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote
||• Anzeigen von Partnerbeitragsdaten
||• Arbeiten im Gutscheinüberprüfungstool|
||• Anzeigen von Kundendatenanalysen
|Kontoadministrator| • Hinzufügen von Nicht-Mandantenbenutzern
||• Hinzufügen oder Löschen von Standorten
||• Verwalten von Profilen, die im Zusammenhang mit den Konten stehen, für die Sie Administrator sind 
||• Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen 
||• Registrieren von Standorten in Programmen

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)

|**Gastbenutzer**   | **Rollen**|
|---------------------------|:--------------------|
||MPN-Partneradministrator|
||Kontenadministrator|
||Incentiveadministrator|
||Geschäftsprofiladministrator|
||Empfehlungsadministrator|


## <a name="manage-referrals-non-aad-roles"></a>Verwalten von Empfehlungen (Nicht-AAD-Rollen)

|**Rolle**|**Funktionsumfang**|
|-----------------------------|:------------------------|
|Empfehlungsadministrator       |• Anzeigen, Erstellen und Verwalten von Geschäftsprofilen
||• Empfangen und Verwalten von Empfehlungen
||• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner|
|Geschäftsprofiladministrator   |• Anzeigen, Erstellen und Verwalten des Geschäftsprofils 
||• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner|

## <a name="manage-incentives--non-aad-roles"></a>Verwalten von Incentives (Nicht-AAD-Rollen)

|**Rolle** | **Funktionsumfang**|
|------------------------------|:-------------------------|
|Incentiveadministrator|• Initiieren und Verwalten von Incentives 
||• Anzeigen und Bearbeiten aller Aspekte von Incentiveprogrammen
||• Anzeigen und Bearbeiten von Bank- und Steuerdaten
||• Anzeigen von Rabatt- und Co-Op-Einnahmen
||• Zugreifen auf den Support
||• Konfliktlösung bei Incentivezahlungen|
|Incentivebenutzer|• Anzeigen von Incentiveprogrammen
||• Anzeigen und Initiieren von Incentiveansprüchen
||• Anzeigen von Rabatt- und Co-Op-Einnahmen
||• Anzeigen von Rabatt- und Co-Op-Einnahmen
||• Zugreifen auf den Support












