---
title: Weisen Sie Benutzer Rollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Alle Mitarbeiter, die im Partner Center arbeiten muss eine Rolle zugewiesen werden.
author: labrenne
ms.author: labrenne
keywords: Rollen, Berechtigungen, Admin-agent
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086728"
---
# <a name="assign-users-roles-and-permissions"></a>Zuweisen von Rollen und Berechtigungen zu Benutzern


Sie haben Ihr Partnerprofil, einschließlich vollständiger Name und Adresse, Supportinformationen, steuerbefreiungen, Bankinformationen und der Hauptansprechpartner für Ihr Unternehmen einrichten. Nächster Schritt: fordern Sie die Benutzer einrichten mit Kennwörtern und Rollen, sodass sie im Partner Center mit Ihnen arbeiten können.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Richten Sie Ihre Mitarbeiter im Partner Center arbeiten

Sie bestimmen die Art des Zugriffs, die Ihre Benutzer über Partner Center die Rollen und Berechtigungen, die Sie ihnen zuweisen. Rollen beziehen sich auf die Programme, die, denen Ihr Unternehmen beteiligt ist. Beispielsweise, wenn Ihr Unternehmen ein Unternehmen Cloud Solution Provider (CSP) ist, nicht erhalten Sie nur das Azure AD-standard Mandanten-Management-Funktionen wie z. B. globaler Administrator, aber benötigen Rollen speziell für das CSP-Programm. Jedes Programm verfügt über Funktionen, die speziell für sie.

>[!Note]
> Azure Active Directory (AAD) Mandanten Rollen enthalten globaler Administrator, Admin Benutzer und CSP-Rollen. Nicht-AAD Rollen enthalten MPN Administrator, Administrator für das Unternehmensprofil, Administrator für Empfehlungen, Incentives-Administrator und Incentive-Benutzer. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Verwalten von kommerziellen Transaktionen im Partner Center (Azure AD und CSP Rollen)

|**Rolle**|**Berechtigungen dieser Rolle**|
|----------------------------------|:---------------------------------|
|Globaler Administrator|• Können alle Microsoft-Konten/-Dienste mit allen Berechtigungen zugreifen.
|      |• Supportanfragen für Partner Center erstellen
||• Ansicht Vereinbarungen, Preislisten und Angebote
||• Anzeigen, erstellen und Verwalten von Partnerbenutzer|
|Benutzeradministrator   | • Anzeigen, erstellen und Verwalten von Benutzern
||• Alle Partnerprofile anzeigen
||• Anzeigen, erstellen und Verwalten von Partnerbenutzer  |
|Standard-Benutzer|  Mein Profil anzeigen   |
|Administratoragent | • Kundenverwaltung
||• Liste der Geräte, die Partner Center< hinzufügen
||• Erstellen und Anwenden von Profilen auf Geräte
||• Abonnementverwaltung
||• Dienstintegrität und Serviceanfragen für Kunden
||• Anforderung delegierter Administratorrechte
||• Ansicht Preise und Angebote
||• Abrechnung
||• Im Auftrag eines Kunden verwalten
||• Registrieren einen Wert Vertragshändler|
|Vertriebsbeauftragter | • Kundenverwaltung
||• Geräteliste zum Partner Center hinzufügen
||• Abonnementverwaltung
||• Ansicht Supportanfragen
||• Anfordern einer Beziehung mit einem Kunden
||• Potenzielle Kunden verwalten
||• Ansicht Kundenvertrag
||• Registrieren einen Wiederverkäufer|
|Helpdesk-Agent| • Suchen und anzeigen ein Kunden
||• Bearbeiten Kundendetails
||• Hilfe Resolve Kunden bei Problemen mit Abrechnung oder der abonnementverwaltung
||• Anforderung Support im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office 365-Abonnements sein)
||• Verwalten von Abonnements und Diensten im Auftrag der Kunden (Hinweis: Sie müssen ein Administrator-Agent zum Ausführen dieser Aufgabe für Office 365-Abonnements sein)|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Control Panel-Anbieter (CPV). (CSP-Rolle und die nicht-AAD)
CPVs Entwickeln von apps für die Verwendung von Cloud Solution Provider (CSP) Partnern setzen, um ihre Systeme mit Partner Center-APIs zu integrieren. 

|**Rolle**   |**Was Sie tun können**|
|------------------------------|:----------------------------|
|Globaler Administrator| Zeigen Sie an und verwalten Sie Ihr Profil CPV|
||Zeigen Sie an und verwalten Sie alle Benutzer, die Zugriff auf CPV Funktionen benötigen|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Verwalten von MPN-Mitgliedschaft und Ihr Unternehmen (nicht-AAD Rollen)

|**Rolle** | **Was Sie tun können**|
|----------------------------|:----------------------------|
|MPN-Administrator|•CAN nicht-Mandanten Benutzer hinzufügen
||• Anzeigen, erstellen und Verwalten von Serviceanfragen der partner
||• Ansicht rechtliche, Organisation, geschäftlichen und MPN-Profilen
||• Ansicht Benutzerdetails Daten und Fähigkeiten
||• Anzeigen von Kompetenzen
||• Anzeigen und Verwalten von Vorteilen
||• Anzeigen und kaufen Sie MPN-Angebote
||Rechnungen und Bestellverlauf • Ansicht MPN-Angebote
||• Können Partner Beitrag Daten anzeigen.
||• Können im Beleg Überprüfung Tool arbeiten.|
|Administratorkonto| • Können Benutzer nicht-Mandanten hinzufügen.
||• Hinzufügen oder Löschen von Speicherorte
||-Verwalten Sie Profile, die im Zusammenhang mit der Konten, die Sie Administrator 
||• Zuweisung von Rollen für Benutzer im Mandanten nicht AAD-Rollen 
||• Speicherorte in Programme registrieren

## <a name="manage-referrals-non-aad-roles"></a>Verwalten von Empfehlungen (nicht-AAD Rollen)

|**Rolle**|**Was Sie tun können**|
|-----------------------------|:------------------------|
|Verweise auf admin       |• Anzeigen, erstellen und Verwalten von Unternehmensprofilen
||• Sie erhalten und Verwalten von Empfehlungen
||• Anzeigen, erstellen und Verwalten von Serviceanfragen der partner|
|Administrator für das Unternehmensprofil   |•View, erstellen und Verwalten des Unternehmensprofils 
||• Anzeigen, erstellen und Verwalten von Serviceanfragen der partner|

## <a name="manage-incentives--non-aad-roles"></a>Verwalten von Incentives (nicht-AAD Rollen)

|**Rolle** | **Was Sie tun können**|
|------------------------------|:-------------------------|
|Anreizadministrator|• Initiiert und Incentives verwaltet 
||• Kann anzeigen und bearbeiten alle Aspekte der Incentives-Programme
||• Kann anzeigen und Bearbeiten von Bank-und Steuerinformationen
||• Ansicht und gemeinschaftliche Einnahmen erhalten
||• Zugriff-Unterstützung
||• Fall Incentive-Zahlungen|
|Anreizbenutzer|• Können Anreizprogramme anzeigen.
||• Kann anzeigen und Initiieren eines incentiveanspruchs
||• Ansicht und gemeinschaftliche Einnahmen erhalten
||• Ansicht und gemeinschaftliche Einnahmen erhalten
||• Zugriff-Unterstützung












