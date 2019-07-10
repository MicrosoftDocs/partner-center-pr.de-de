---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Jedem Mitarbeiter, der im Partner Center arbeitet, muss eine Rolle zugewiesen werden.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 658106548596a5fa7d02d29c0065a23caeacb83d
ms.sourcegitcommit: 59825cb626e12dfe5eb2d28e836b4573368d705e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/09/2019
ms.locfileid: "67690840"
---
# <a name="assign-users-roles-and-permissions"></a>Zuweisen von Rollen und Berechtigungen zu Benutzern


Sie haben Ihr Partnerprofil mit gesetzlichem Namen und Adresse, Supportdetails, Steuerbefreiungen, Bankverbindung und dem Hauptansprechpartner für Ihr Unternehmen eingerichtet. Nächster Schritt: Einrichten der Benutzer mit Kennwörtern und Rollen, damit sie mit Ihnen gemeinsam im Partner Center arbeiten können.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Einrichten Ihrer Mitarbeiter für die Arbeit im Partner Center

Die Zugriffsarten Ihrer Benutzer auf das Partner Center bestimmen Sie durch die Rollen und Berechtigungen, die Sie ihnen erteilen. Rollen beziehen sich auf die Programme, an denen Ihr Unternehmen beteiligt ist. Wenn Ihr Unternehmen beispielsweise im CSP-Bereich (Cloud Solution Provider) tätig ist, verfügen Sie nicht nur über die Standard-Mandantenverwaltungsrollen von Azure AD (z.B. „Globaler Administrator“), sondern benötigen auch spezielle Rollen für das CSP-Programm. Jedes Programm verfügt über Rollen, die spezifisch für das jeweilige Programm sind.

>[!Note]
> AAD-Mandantenrollen (Azure Active Directory) enthalten globale Administrator-, Benutzeradministrator- und CSP-Rollen. Nicht-AAD-Rollen sind diese Rollen, die den Mandanten keine verwalten und MPN Admin, Administrator für Business-Profil, Verweis Verwaltungs-, anreizprogramm Admin und anreizprogramm Benutzer enthalten. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Verwalten kommerzieller Transaktionen im Partner Center (Azure AD- und CSP-Rollen)

|**Rolle**|**Funktionsumfang**|
|----------------------------------|:---------------------------------|
|Globaler Administrator|• Zugriff auf alle Microsoft-Konten/-Dienste mit allen Berechtigungen
|      |• Erstellen von Supportanfragen für das Partner Center
||• Anzeigen von Vereinbarungen, Preislisten und Angeboten
||• Anzeigen, Erstellen und Verwalten von Partnerbenutzern|
||  Anzeigen, erstellen und Verwalten von abrechnungs-, Rechnungen und Abstimm Dateien
|Benutzerverwaltungsadministrator   | • Anzeigen, erstellen und Verwalten von Benutzern
||• Anzeigen aller Partnerprofile
||• Anzeigen, Erstellen und Verwalten von Partnerbenutzern  |
|Abrechnungsadministrator | • Anzeigen, Erstellen und Verwalten der Abrechnung, von Rechnungen und Kontenabstimmungsdateien|
|Standardbenutzer|  Anzeigen des eigenen Profils   |
|Administratoragent | • Kundenverwaltung
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
||• Anzeigen Preis aufgelistet und bietet
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

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Gastbenutzer (muss dem AAD-Mandanten hinzugefügt werden)

|**Gastbenutzer**   | **Rollen**|
|---------------------------|:--------------------|
||MPN-Partneradministrator|
||Kontenadministrator|
||Incentiveadministrator|
||Geschäftsprofiladministrator|
||Empfehlungsadministrator|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Verwalten von MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen: Diese Rollen zu verwalten, die Geschäftstätigkeit Unternehmen statt des Mandanten)

|**Rolle** | **Funktionsumfang**|
|----------------------------|:----------------------------|
|Administrator für MPN-Partner|• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner||
||• Anzeigen, die rechtlichen, Unternehmen, Unternehmen und MPN-Profile
||• Anzeigen der Daten und Fähigkeiten von Benutzern
||• Anzeigen von Kompetenzen
||• Anzeigen und Verwalten von Vorteilen
||• Anzeigen und Kaufen von MPN-Angeboten
||• Anzeigen von Rechnungen und des Bestellverlaufs für MPN-Angebote
||• Anzeigen Partner Beitrag-Indikatordaten
||• Arbeiten im Gutscheinüberprüfungstool|
||• Anzeigen von Kundendatenanalysen
|| Anzeigen anderer Rollen in Unternehmen, aber können keine Rollen zuweisen
|Kontoadministrator| Hinzufügen von Standorten
|| Verwalten von Profilen, die im Zusammenhang mit den Konten, die, denen Sie Administrator sind 
||• Zuweisen von Rollen für Benutzer im Mandanten zu Nicht-AAD-Rollen 
||• Registrieren von Standorten in Programmen


## <a name="manage-referrals"></a>Verwalten von verweisen 

|**Rolle**|**Funktionsumfang**|
|-----------------------------|:------------------------|
|Empfehlungsadministrator       |• Anzeigen, Erstellen und Verwalten von Geschäftsprofilen
||• Empfangen und Verwalten von Empfehlungen
||• Anzeigen, erstellen und Verwalten von Co-Selling-Verweise|
||• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner
|Administrator für das Unternehmensprofil   |• Anzeigen, erstellen und Verwalten von Business-Profil 
||• Anzeigen, Erstellen und Verwalten von Serviceanfragen der Partner|

## <a name="manage-incentives"></a>Verwalten von incentives 

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
||• Zugreifen auf den Support












