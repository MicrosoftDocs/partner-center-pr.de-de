---
title: Zuweisen von Benutzerrollen und Berechtigungen | Partner Center
ms.topic: article
ms.date: 3/5/19
description: Jeder Mitarbeiter im Partner Center funktioniert muss, muss eine Rolle zugewiesen werden.
author: LauraBrenner
ms.author: labrenne
keywords: Rollen, Berechtigungen, Administrator, Agent
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682488"
---
# <a name="assign-users-roles-and-permissions"></a>Zuweisen von Rollen und Berechtigungen zu Benutzern


Sie haben Ihr Profil des Partners, einschließlich offizieller Name und Adresse, Informationen zum Support, Datei steuern Ausnahmen, Bankinformationen und der primäre Ansprechpartner für Ihr Unternehmen einrichten. Nächster Schritt: erhalten Ihre Benutzer richten Sie mit Kennwörtern und Rollen, sodass sie im Partner Center mit Ihnen arbeiten können.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Ihre Mitarbeiter arbeiten im Partner Center einrichten

Sie bestimmen die Zugriffsarten aufgeführt, die Ihre Benutzer müssen Partner Center durch die Rollen und Berechtigungen, die Sie ihnen geben. Rollen beziehen sich auf die Programme, die, denen Ihr Unternehmen beteiligt ist. Z. B. Wenn Ihr Unternehmen einen Cloud Solution Provider (CSP) ist, nicht nur müssen die standardmäßige Azure AD Mandanten Verwaltungsrollen z.B. globaler Administrator, allerdings benötigen Rollen spezifisch für das CSP-Programm. Jedes Programm verfügt über Rollen, die speziell für sie.

>[!Note]
> Azure Active Directory (AAD) mandantenrollen enthalten globaler Administrator, Benutzeradministrator und CSP-Rollen. Nicht-AAD-Rollen umfassen MPN Admin, Business-Profil-Admin, Verweis Admin, anreizprogramm Admin und anreizprogramm Benutzer. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Verwalten von kommerziellen Transaktionen im Partner Center (Azure AD und CSP-Rollen)

|**Rolle**|**Was sie tun können**|
|----------------------------------|:---------------------------------|
|Globaler Administrator|• Können auf alle Microsoft-Konto/Dienste mit vollständigen Berechtigungen zugreifen.
|      |• Erstellen von supporttickets im Partner Center
||• Anzeigen Vereinbarungen, Preislisten und Angebote
||• Anzeigen, erstellen und Verwalten von B2B-Zusammenarbeit|
|Benutzeradministrator   | • Anzeigen, erstellen und Verwalten von Benutzern
||• Zeigen Sie alle aufgelisteten Partnerprofile
||• Anzeigen, erstellen und Verwalten von B2B-Zusammenarbeit  |
|Abrechnungsadministrator | – Anzeigen, erstellen und Verwalten von abrechnungs-, Rechnungen und Abstimm Dateien|
|Standardbenutzer|  Mein Profil anzeigen   |
|Administratoragent | • Kundenverwaltung
||• Hinzufügen von Geräteliste zu Partner Center <
||• Erstellen und Anwenden von Profilen für Geräte
||• Verwaltung des Abonnements
||• Service Health und dienstanforderungen für Kunden
||• Anforderung delegierte Administratorberechtigungen
||• Die Preise und Angebote
||• Abrechnung
||• Im Auftrag eines Kunden verwalten
||•, Registrieren Sie ein Wert hinzugefügt, reseller|
|Vertriebsbeauftragter | • Kundenverwaltung
||• Das Partner Center Geräteliste hinzugefügt
||• Verwaltung des Abonnements
||• Anzeigen-Support-tickets
||• Anforderung eine Beziehung mit einem Kunden
||• Verwalten von kundenleads
||• Anzeigen, die Kunden-Vereinbarung
||• Registrieren einen Wiederverkäufer|
|Helpdesk-Agent| • Suchen und anzeigen ein Kunden
||• Kunden Bearbeiten von details
||• Help Resolve-Kundenprobleme mit der Verwaltung von Abrechnung oder zum Abonnement
||• Anforderung Support für Kunden (Hinweis: Sie müssen ein Administrator-Agent zur Ausführung dieser Aufgabe für Office 365-Abonnements sein)
||• Verwalten von Abonnements und Abrechnung Probleme im Namen von Kunden (Hinweis: Sie müssen ein Administrator-Agent zur Ausführung dieser Aufgabe für Office 365-Abonnements sein)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Hersteller des Steuerelements Bereich (Vocabulary). (CSP-Rolle und nicht-AAD-Rolle)
CPVs entwickeln Sie apps für die Verwendung durch Partner (Cloud Solution Provider, CSP), damit sie ihre Systeme in Partner Center-APIs integrieren können. 

|**Rolle**   |**Was Sie tun können**|
|------------------------------|:----------------------------|
|Globaler Administrator| Zeigen Sie an und verwalten Sie Ihr Profil CPV|
||Zeigen Sie an und verwalten Sie Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen.|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Verwalten von MPN-Mitgliedschaft und Ihres Unternehmens (nicht-AAD-Rollen)

|**Rolle** | **Was Sie tun können**|
|----------------------------|:----------------------------|
|Administrator für MPN-Partner|•CAN hinzufügen, ohne Benutzer
||• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner
||• Anzeigen, die rechtlichen, Unternehmen, Unternehmen und MPN-Profile
||• Details zum Benutzer und ihre Fähigkeiten-Daten
||• Anzeigen Kompetenzen
||• Anzeigen und verwalten Sie die Vorteile
||• Anzeigen und erwerben von bietet MPN
||• Anzeigen von MPN bietet, Bestellverlauf und Rechnungen
||• Anzeigen Beitrag Partnerdaten
||• Können in den Gutschein Überprüfungstool arbeiten.|
||– Anzeigen von Datenanalysen für Kunden
|Kontoadministrator| • Können nicht einem Mandanten Benutzer hinzufügen.
||• Hinzufügen oder Löschen von Standorten
||– Verwalten von Profilen, die im Zusammenhang mit den Konten, die, denen Sie Administrator sind 
||• Zuweisen von Rollen für Benutzer im Mandanten nicht AAD-Rollen 
||• Standorte in Programmen zu registrieren

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Gastbenutzer (muss für den AAD-Mandanten hinzugefügt werden)

|**Gastbenutzer**   | **Rollen**|
|---------------------------|:--------------------|
||Administrator für MPN-Partner|
||Konten-Administrator|
||Incentives-Administrator|
||Administrator für das Unternehmensprofil|
||Verweise auf admin|


## <a name="manage-referrals-non-aad-roles"></a>Verwalten von verweisen (nicht-AAD-Rollen)

|**Rolle**|**Was Sie tun können**|
|-----------------------------|:------------------------|
|Verweise auf admin       |• Anzeigen, erstellen und Verwalten von Geschäftsprofilen
||• Empfangen und Verwalten von verweisen
||• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner|
|Administrator für das Unternehmensprofil   |• Anzeigen, erstellen und Verwalten von Business-Profil 
||• Anzeigen, erstellen und Verwalten von Serviceanfragen für partner|

## <a name="manage-incentives--non-aad-roles"></a>Verwalten von Incentives (nicht-AAD-Rollen)

|**Rolle** | **Was Sie tun können**|
|------------------------------|:-------------------------|
|Incentives-Administrator|• Initiiert und Anreize verwaltet 
||• Anzeigen und bearbeiten alle Aspekte der Anreize für Programme
||• Anzeigen und bearbeiten die Bank- und Steuerdaten-details
||• Anzeigen Rebate und Co-op-Ergebnis
||• Unterstützung des Zugriffs
||• Im Fall von streitigkeiten Anreize für Zahlungen|
|Incentivebenutzer|• Können Incentives sammeln, wenn Programme anzuzeigen.
||• Anzeigen können, und starten Incentives sammeln, wenn Ansprüche
||• Anzeigen Rebate und Co-op-Ergebnis
||• Anzeigen Rebate und Co-op-Ergebnis
||• Unterstützung des Zugriffs












