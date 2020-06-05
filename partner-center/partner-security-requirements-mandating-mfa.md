---
title: Festlegen von MFA für Ihren Partnermandanten
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie das Festlegen von MFA für Ihre Partnermandanten dazu beiträgt, Ihren Zugriff auf Kundenressourcen zu sichern. Enthält Beispielszenarien.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9454e9410e4110fdf3542bde3696d8447d4c90d0
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998306"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Festlegen von Multi-Factor Authentication (MFA) für Ihren Partnermandanten

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direktrechnung
  - Indirekter Anbieter
  - Indirekter Wiederverkäufer
- Alle Berater

**Betroffene Rollen**

- Administrator-Agent
- Vertriebsbeauftragter
- Helpdesk-Agent
- Rechnungsadministrator
- Globaler Administrator

Diese Funktion soll Partnern helfen, ihren Zugriff auf Kundenressourcen vor Kompromittierungen von Anmeldeinformationen zu schützen.
Partner müssen die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) für alle Benutzerkonten in ihrem Partnermandanten – einschließlich des Gastbenutzers – erzwingen. Mit diesem Feature werden diese Partnerrollen beauftragt, die MFA-Überprüfung für die folgenden Bereiche durchzuführen:

- [Partner Center Dashboard](#partner-center-dashboard) (Ab 1. Mai 2020)
- [Partner Center-API](#partner-center-api) (Ab 1. Mai 2020)
- [Vom Partner delegierte Verwaltung](#partner-delegated-administration)

Stärkere und laufende Sicherheits- und Datenschutzmaßnahmen gehören zu unseren wichtigsten Prioritäten, und wir unterstützen Partner weiterhin dabei, ihre Kunden und Mandanten zu schützen. Alle Partner, die am Cloud Solution Provider-Programm (CSP) teilnehmen, Control Panel Vendors (CPVs) und Berater sollten die [Sicherheitsanforderungen des Partners](partner-security-requirements.md) implementieren, um konform zu bleiben.

Microsoft hat mit der Aktivierung zusätzlicher Sicherheitsmaßnahmen für Partnermandanten begonnen. Mithilfe dieser Aktivierung können Partner ihre Mandanten und deren Kunden durch das Festlegen von MFA-Überprüfung (Multi-Factor Authentication) schützen, um einen nicht autorisierten Zugriff zu verhindern.

Wir haben die Aktivierung für vom Partner delegierte Verwaltungsfunktionen bei allen Partnermandanten erfolgreich abgeschlossen. Zur weiteren Unterstützung von Partnern und Kunden werden wir ab 1. Mai 2020 mit der Aktivierung für Partner Center-Transaktionen in CSP beginnen und so Partnern dabei helfen, ihre Unternehmen und Kunden vor Vorfällen im Zusammenhang mit Identitätsdiebstahl zu schützen.

Diese Dokumentation liefert Partnern detaillierte Informationen und Anleitungen zur Aktivierung von Sicherheitsmaßnahmen.

## <a name="partner-center-dashboard"></a>Partner Center-Dashboard

Bestimmte Seiten im Partner Center-Dashboard werden durch MFA geschützt, einschließlich:

* Alle Seiten auf der Registerkarte **Kunden**, z. B. alle Seiten, auf die über die folgende URL zugegriffen werden kann: https://partner.microsoft.com/commerce/*
* Alle Seiten auf der Registerkarte **Support > Kundenanforderungen**, z. B die Seite, auf die über https://partner.microsoft.com/dashboard/support/csp/customers/* zugegriffen wird
* Abrechnungsseite

Wenn Sie versuchen, auf eine dieser Seiten zuzugreifen und die MFA-Überprüfung zuvor nicht abgeschlossen haben, müssen Sie dies nun nachholen.

> [!NOTE]
> Andere Seiten im Partner Center, z. B. die Übersichtsseite oder die Seite zur Überprüfung der Dienstintegrität, werden nicht durch MFA geschützt.

Die folgenden Benutzertypen sind für den Zugriff auf diese durch MFA geschützten Seiten autorisiert und daher von diesem Feature betroffen:


| Durch MFA geschützte Seiten       | Administrator-Agents      |  Vertriebsbeauftragte     |   Helpdesk-Agents     | Globaler Administrator      |  Rechnungsadministrator     | 
|---    |---    |---    |---    |---    |---    |
| Alle Seiten auf der Registerkarte „Kunden“      |   x    |    x   |  x     |       |       |
| Alle Seiten auf der Registerkarte „Support“ > „Kundenanforderungen“     | x      |       |    x   |       |       |
| Abrechnungsseite     |   x    |       |       |    x   |   x    |

**Beispiele**

Um die Funktionsweise der Überprüfung zu veranschaulichen, sehen Sie sich die folgenden beiden Beispiele an.

**Beispiel 1: Partner hat Azure AD MFA implementiert**
1.    Jane arbeitet für CSP Contoso. Contoso hat MFA für alle Benutzer unter dem Contoso-Partnermandanten mit Azure Active Directory (Azure AD) MFA implementiert.
2.    Jane startet eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet Jane an Azure AD um, um sich anzumelden.
3.    Aufgrund der vorhandenen Azure AD MFA-Einrichtung durch Contoso muss Jane die MFA-Überprüfung durchführen. Nach erfolgreicher Anmeldung und MFA-Überprüfung wird Jane zurück zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4.    Jane versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da Jane die MFA-Überprüfung bei der Anmeldung bereits früher abgeschlossen hat, kann Jane auf die durch MFA geschützte Seite zugreifen, ohne die MFA-Überprüfung erneut durchlaufen zu müssen.

**Beispiel 2: Partner hat Drittanbieter-MFA mithilfe des Identitätsverbunds implementiert**
1. Trent arbeitet für CSP Wingtip. Wingtip hat Drittanbieter-MFA für alle Benutzer unter dem Wingtip-Partnermandanten mit Drittanbieter-MFA implementiert, die über einen Identitätsverbund in Azure AD integriert ist.
2. Trent startet eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet Trent an Azure AD um, um sich anzumelden.
3. Da Wingtip Identitätsverbund eingerichtet hat, leitet Azure AD Trent zum Verbundidentitätsanbieter um, um die Anmeldung und MFA-Überprüfung abzuschließen. Nach erfolgreicher Anmeldung und MFA-Überprüfung wird Trent zurück an Azure AD und dann zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4. Trent versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da Trent die MFA-Überprüfung bei der Anmeldung bereits früher abgeschlossen hat, kann Trent auf die durch MFA geschützte Seite zugreifen, ohne die MFA-Überprüfung erneut durchlaufen zu müssen.

**Beispiel 3: Partner hat MFA nicht implementiert**
1. John arbeitet für CSP Fabrikam. Fabrikam hat für keinen Benutzer unter dem Fabrikam-Partnermandanten MFA implementiert.
2. John startet eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet John an Azure AD um, um sich anzumelden.
3. Da Fabrikam MFA nicht implementiert hat, muss John die MFA-Überprüfung nicht durchführen. Nach erfolgreicher Anmeldung wird John zurück zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4. John versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da John die MFA-Überprüfung nicht abgeschlossen hat, leitet Partner Center John an Azure AD um, um die MFA-Überprüfung abzuschließen. Da John MFA jetzt zum ersten Mal durchführen muss, wird er außerdem aufgefordert, sich [für MFA zu registrieren](#mfa-registration-experience). Nach erfolgreicher MFA-Registrierung und MFA-Überprüfung kann John nun auf die durch MFA geschützte Seite zugreifen.
5. An einem weiteren Tag, bevor Fabrikam MFA für jeden Benutzer implementiert, startet John eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet John an Azure AD um, um sich ohne MFA-Eingabeaufforderung anzumelden. 
6. John versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da John die MFA-Überprüfung nicht abgeschlossen hat, leitet Partner Center John an Azure AD um, um die MFA-Überprüfung abzuschließen. Da John MFA registriert hat, wird er dieses Mal nur aufgefordert, die MFA-Überprüfung abzuschließen.

> [!NOTE]
>Aktion: Der Unternehmensadministrator sollte MFA jetzt über eine dieser [Optionen](partner-security-requirements.md#actions-that-you-need-to-take) implementieren, die von Partner Center vorgeschlagen werden.

## <a name="partner-center-api"></a>Partner Center-API

Die Partner Center-API unterstützt sowohl reine App-Authentifizierung als auch App- und Benutzerauthentifizierung. 

Wenn App- und Benutzerauthentifizierung verwendet wird, erfordert Partner Center eine MFA-Überprüfung. Genauer gesagt: Wenn eine Partneranwendung eine API-Anforderung an Partner Center senden möchte, muss sie ein Zugriffstoken in den Autorisierungsheader der Anforderung einschließen. 

> [!NOTE]
>[Sicheres Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) ist ein sicheres, skalierbares Framework zum Authentifizieren von CSP-Partnern und CPVS über die Microsoft Azure MFA-Architektur, wenn Sie die Partner Center-API aufrufen. Sie müssen sie implementieren, bevor Sie MFA für Ihren Mandanten aktivieren. 

Wenn Partner Center eine API-Anforderung mit einem Zugriffstoken empfängt, das mit App- und Benutzerauthentifizierung abgerufen wurde, prüft die Partner Center-API, ob der *MFA*-Wert im *AMR*-Anspruch (Authentication Method Reference) vorhanden ist. Sie können einen JWT-Decoder verwenden, um zu überprüfen, ob ein Zugriffstoken den erwarteten AMR-Wert enthält:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Wenn der Wert vorhanden ist, schließt Partner Center daraus, dass die MFA-Überprüfung abgeschlossen wurde, und verarbeitet die API-Anforderung. Wenn der Wert nicht vorhanden ist, lehnt die Partner Center-API die Anforderung mit der folgenden Antwort ab:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Wenn die reine App-Authentifizierung verwendet wird, funktionieren die APIs, die diese Authentifizierung unterstützen, kontinuierlich, ohne dass MFA erforderlich ist.

## <a name="partner-delegated-administration"></a>Vom Partner delegierte Verwaltung

### <a name="using-service-portals"></a>Verwenden von Dienstportalen

Partnerkonten, einschließlich Administrator-Agents und Helpdesk-Agents, können ihre vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen über Portale für Microsoft-Onlinedienste, die Befehlszeilenschnittstelle (CLI) und APIs (mit App- und Benutzerauthentifizierung) verwenden.

Beim Zugriff auf Portale für Microsoft-Onlinedienste mithilfe der vom Partner delegierten Verwaltungsberechtigungen (Admin-on-Behalf-Of, AOBO, Administrator im Auftrag von) zum Verwalten von Kundenressourcen erfordern viele dieser Portale, dass sich das Partnerkonto interaktiv authentifiziert, wobei der Azure Active Directory-Mandant des Kunden als Authentifizierungskontext festgelegt ist: Das Partnerkonto ist für die Anmeldung beim Kundenmandanten erforderlich.

Wenn Azure Active Directory solche Authentifizierungsanforderungen empfängt, muss das Partnerkonto eine MFA-Überprüfung durchführen. Je nachdem, ob es sich bei dem Partnerkonto um eine verwaltete oder eine Verbundidentität handelt, gibt es zwei Möglichkeiten:

- Wenn es sich bei dem Partnerkonto um eine **verwaltete** Identität handelt, wird der Benutzer direkt von Azure Active Directory aufgefordert, die MFA-Überprüfung abzuschließen. Wenn das Partnerkonto zuvor noch nicht für MFA mit Azure Active Directory registriert wurde, wird der Benutzer aufgefordert, zunächst die [MFA-Registrierung abzuschließen](#mfa-registration-experience).

- Wenn es sich bei dem Partnerkonto um eine **Verbundidentität** handelt, ist die Vorgehensweise davon abhängig, wie der Partneradministrator den Verbund in Azure Active Directory konfiguriert hat. Beim Einrichten eines Verbunds in Azure Active Directory kann der Partneradministrator Azure Active Directory informieren, ob der Verbundidentitätsanbieter MFA unterstützt. Wenn dies der Fall ist, leitet Azure Active Directory den Benutzer an den Verbundidentitätsanbieter weiter, um die MFA-Überprüfung abzuschließen. Andernfalls wird der Benutzer von Azure Active Directory direkt aufgefordert, die MFA-Überprüfung abzuschließen. Wenn das Partnerkonto zuvor noch nicht für MFA mit Azure Active Directory registriert wurde, wird der Benutzer aufgefordert, zunächst die [MFA-Registrierung abzuschließen](#mfa-registration-experience).

Die Benutzererfahrung ähnelt insgesamt dem Szenario, in dem ein Endkundenmandant MFA für seine Administratoren implementiert hat. Beispielsweise hat der Kundenmandant [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) aktiviert. Diese erfordern, dass sich alle Konten mit Administratorrechten mit MFA-Überprüfung beim Kundenmandanten anmelden, einschließlich Administrator-Agents und Helpdesk-Agents. Zu Testzwecken können Partner die [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) im Kundenmandanten aktivieren und dann versuchen, vom Partner delegierte Verwaltungsberechtigungen für den Zugriff auf den Kundenmandanten zu verwenden.

> [!NOTE]
> Nicht alle Portale für Microsoft-Onlinedienste erfordern, dass sich Partnerkonten beim Kundenmandanten beim Zugriff auf Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen anmelden. Stattdessen müssen sich die Partnerkonten nur beim Partnermandanten anmelden. Ein Beispiel hierfür ist das Exchange Admin Center. Im Laufe der Zeit erwarten wir, dass diese Portale erfordern, dass sich Partnerkonten beim Kundenmandanten anmelden, wenn vom Partner delegierte Verwaltungsberechtigungen verwendet werden.

### <a name="using-service-apis"></a>Verwenden von Dienst-APIs
Einige Microsoft-Onlinedienste-APIs (z. B. Azure Resource Manager, Azure AD Graph, Microsoft Graph usw.) unterstützen Partner durch vom Partner delegierte Verwaltungsberechtigungen, um Kundenressourcen programmgesteuert zu verwalten. Um vom Partner delegierte Verwaltungsberechtigungen mit diesen APIs zu nutzen, muss die Partneranwendung ein Zugriffstoken in den API-Anforderungsautorisierungsheader einschließen. Das Zugriffstoken wird abgerufen, indem sich ein Partnerbenutzerkonto bei Azure AD authentifiziert. Dabei wird das Azure AD des Kunden als Authentifizierungskontext festgelegt. Die Partneranwendung erfordert, dass sich ein Partnerbenutzerkonto beim Kundenmandanten anmeldet.

Wenn Azure AD eine solche Authentifizierungsanforderung empfängt, verlangt Azure AD, dass das Partnerbenutzerkonto eine MFA-Überprüfung durchführt. Wenn das Partnerbenutzerkonto noch nicht für MFA registriert wurde, wird das Benutzerkonto zunächst aufgefordert, die MFA-Registrierung abzuschließen.

Alle Partneranwendungen, die in diese APIs mit vom Partner delegierten Verwaltungsberechtigungen integriert sind, sind von diesem Feature betroffen. Um sicherzustellen, dass Partneranwendungen mit diesen APIs weiterhin ohne Unterbrechung zusammenarbeiten können:

- Der Partner muss die Verwendung einer nicht interaktiven Benutzerauthentifizierungsmethode mit Azure AD vermeiden, um das Zugriffstoken abzurufen. Bei Verwendung einer nicht interaktiven Benutzerauthentifizierungsmethode (etwa [Kennwortfluss](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)) kann Azure AD den Benutzer nicht auffordern, die MFA-Überprüfung abzuschließen. Der Partner muss stattdessen zu einer interaktiven Benutzerauthentifizierungsmethode wechseln, z. B. zum [OpenID Connect-Fluss](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code).
- Während der interaktiven Benutzerauthentifizierungsmethode sollte der Partner ein Partnerbenutzerkonto verwenden, das bereits für MFA aktiviert wurde. Wenn Sie von Azure AD dazu aufgefordert werden, können Partner alternativ die MFA-Registrierung und die MFA-Überprüfung während der Anmeldung abschließen.
- Dies ähnelt dem Szenario, in dem ein Endkundenmandant MFA für seine Administratoren implementiert hat. Beispielsweise hat der Kundenmandant [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) aktiviert. Diese erfordern, dass sich alle Benutzerkonten mit Administratorrechten mit MFA-Überprüfung beim Kundenmandanten anmelden, einschließlich Administrator-Agents und Helpdesk-Agents. Zu Testzwecken können Partner die [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) im Kundenmandanten aktivieren und dann versuchen, vom Partner delegierte Verwaltungsberechtigungen für den programmgesteuerten Zugriff auf den Kundenmandanten zu verwenden.

### <a name="mfa-registration-experience"></a>MFA-Registrierungsablauf
Wenn das Partnerbenutzerkonto noch nicht für MFA registriert wurde, wird der Benutzer während der MFA-Überprüfung zunächst von Azure AD aufgefordert, die MFA-Registrierung abzuschließen:

![MFA-Registrierung, Schritt 1](images/MfaRegistration1.png)

Nachdem der Benutzer auf **Weiter** geklickt hat, wird er aufgefordert, aus einer Liste von Überprüfungsmethoden auszuwählen.

![MFA-Registrierung, Schritt 2](images/MfaRegistration2.png)

Nach erfolgreicher Registrierung muss der Benutzer die MFA-Überprüfung basierend auf der vom Benutzer ausgewählten Überprüfungsmethode durchführen.



## <a name="request-for-technical-exception"></a>Anfrage einer technischen Ausnahme

Partner können eine technische Ausnahme beantragen, um die MFA-Überprüfung zu unterdrücken, wenn sie technische Probleme mit Microsoft-Onlinediensten haben und keine praktikable Lösung oder Problemumgehung verfügbar ist. Lesen Sie zuvor die folgenden Abschnitte:

 - [Liste der von Partnern gemeldeten häufigen Probleme](#list-of-common-issues-reported-by-partners)
 - [Einreichen einer Anfrage für eine technische Ausnahme](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Liste der von Partnern gemeldeten häufigen Probleme
Bevor Sie eine technische Ausnahme beantragen, überprüfen Sie die Liste der häufigen Probleme, die von anderen Partnern gemeldet wurden, um zu verstehen, ob es sich um gültige Gründe für eine technische Ausnahme handelt.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problem 1: Partner benötigt mehr Zeit für die Implementierung von MFA für seine Partner-Agents
Ein Partner hat noch nicht damit begonnen oder ist noch dabei, MFA für seine Partner-Agents zu implementieren, die Zugriff auf Portale für Microsoft-Onlinedienste benötigen, um Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen zu verwalten. Der Partner benötigt mehr Zeit, um die MFA-Implementierung abzuschließen. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein Der Partner muss planen, MFA für seine Benutzer zu implementieren, um Unterbrechungen zu vermeiden.

> [!NOTE]
> Auch wenn der Partner MFA für seine Partner-Agents nicht implementiert hat, können die Partner-Agents dennoch auf Portale für Microsoft-Onlinedienste mit vom Partner delegierten Verwaltungsberechtigungen zugreifen – vorausgesetzt, sie können die MFA-Registrierung und MFA-Überprüfung abschließen, wenn sie bei der Anmeldung beim Kundenmandanten dazu aufgefordert werden. Das Abschließen der MFA-Registrierung aktiviert den Benutzer nicht automatisch für MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problem 2: Partner hat MFA nicht für Benutzerkonten implementiert, die keine delegierten Verwaltungsberechtigungen verwenden
Ein Partner verfügt über einige Benutzer in seinen Partnermandanten, die keinen Zugriff auf Portale für Microsoft-Onlinedienste benötigen, um Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen zu verwalten. Der Partner ist gerade dabei, MFA für diese Benutzer zu implementieren, und benötigt mehr Zeit zum Abschließen des Vorgangs. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein Da diese Benutzerkonten keine vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen verwenden, müssen sie sich nicht beim Kundenmandanten anmelden. Sie sind nicht davon betroffen, dass Azure AD während der Anmeldung beim Kundenmandanten eine MFA-Überprüfung erfordert.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3: Partner hat MFA für Benutzerdienstkonten nicht implementiert
Ein Partner verfügt über einige Benutzerkonten in seinen Partnermandanten, die von Geräten als Dienstkonten verwendet werden. Dabei handelt es sich um Konten mit geringen Berechtigungen, die keinen Zugriff auf Partner Center oder Portale für Microsoft-Onlinedienste benötigen, um Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen zu verwalten. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein Da diese Benutzerkonten keine vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen verwenden, müssen sie sich nicht beim Kundenmandanten anmelden. Sie sind nicht davon betroffen, dass Azure AD während der Anmeldung beim Kundenmandanten eine MFA-Überprüfung erfordert.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4: Partner kann MFA nicht mithilfe der MS Authenticator-App implementieren
Ein Partner verfügt über eine „Clean Desk“-Richtlinie, die es Mitarbeitern nicht gestattet, ihre persönlichen mobilen Geräte in ihrem Arbeitsbereich zu verwenden. Ohne Zugriff auf ihre persönlichen mobilen Geräte können die Mitarbeiter die MS Authenticator-App nicht installieren, die die einzige MFA-Überprüfung ist, die von den Azure AD-Sicherheitsstandards unterstützt wird. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein, dies ist kein gültiger Grund für eine technische Ausnahme. Der Partner sollte die folgenden Alternativen berücksichtigen, damit seine Mitarbeiter beim Zugriff auf Partner Center die MFA-Überprüfung trotzdem durchführen können:
- Partner können sich auch für Azure AD Premium oder MFA-Lösungen von Drittanbietern registrieren (kompatibel mit Azure AD), die zusätzliche Überprüfungsmethoden bereitstellen können.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5: Partner kann MFA aufgrund der Verwendung von Legacyauthentifizierungsprotokollen nicht implementieren
Ein Partner arbeitet mit einigen Partner-Agents zusammen, die noch ältere Authentifizierungsprotokolle verwenden, die nicht mit MFA kompatibel sind. Beispielsweise verwenden die Benutzer noch Outlook 2010, das auf Legacyauthentifizierungsprotokollen basiert. Wenn MFA für diese Partner-Agents aktiviert wird, wird die Verwendung von Legacyauthentifizierungsprotokollen unterbrochen.

**Antwort**: Nein, dies ist kein gültiger Grund für eine technische Ausnahme. Es wird dringend empfohlen, dass Partner aufgrund potenzieller Sicherheitsrisiken von der Verwendung veralteter Authentifizierungsprotokolle Abstand nehmen, da diese Protokolle nicht durch MFA-Überprüfung geschützt werden können und für eine Gefährdung von Anmeldeinformationen weitaus anfälliger sind. Wenn der Wechsel von der Verwendung von Legacyauthentifizierungsprotokollen nicht möglich ist, sollten sich Partner für Azure AD Premium registrieren, das die Verwendung von Anwendungskennwörtern unterstützt. Anwendungskennwörter sind einmalige, vom System generierte Kennwörter, die in der Regel stärker als manuell vom Benutzer generierte Kennwörter sind. Mithilfe von Anwendungskennwörtern können Partner MFA für ihre Benutzer implementieren und dabei auf Anwendungskennwörter nur für ältere Authentifizierungsprotokolle zurückgreifen.

Lesen Sie den Beitrag zu [Standardauthentifizierung und Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282), um den neuesten Plan zur Unterstützung der Legacyauthentifizierung für Outlook zu verstehen, und folgen Sie dem [Teamblog zu Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange), um die bevorstehenden Neuerungen zu erfahren. 

> [!NOTE]
> Auch wenn der Partner MFA für seine Partner-Agents nicht implementiert hat, können die Partner-Agents dennoch auf Portale für Microsoft-Onlinedienste mit vom Partner delegierten Verwaltungsberechtigungen zugreifen – vorausgesetzt, sie können die MFA-Registrierung und MFA-Überprüfung abschließen, wenn sie bei der Anmeldung beim Kundenmandanten dazu aufgefordert werden. Das Abschließen der MFA-Registrierung aktiviert den Benutzer nicht automatisch für MFA.

#### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problem 6: Partner hat Drittanbieter-MFA implementiert, die von Azure AD nicht erkannt wird
Ein Partner hat MFA für seine Benutzer mit einer MFA-Lösung eines Drittanbieters implementiert. Der Partner kann jedoch die MFA-Lösung des Drittanbieters nicht ordnungsgemäß konfigurieren, um Azure AD zu vermitteln, dass die MFA-Überprüfung während der Benutzerauthentifizierung durchgeführt wurde. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Ja, dieses Problem kann als gültiger Grund für eine technische Ausnahme angesehen werden. Lassen Sie sich vor dem Einreichen einer Anfrage für eine technische Ausnahme durch den MFA-Lösungsdrittanbieter Folgendes bestätigen: Die MFA-Lösung kann nicht so konfiguriert werden, dass der Anspruch *authenticationmethodsreferences* (mit dem Wert *multipleauthn*) an Azure AD übermittelt wird, um anzugeben, dass die MFA-Überprüfung während der Benutzerauthentifizierung abgeschlossen wurde. Beim Einreichen einer Anfrage für eine technische Ausnahme müssen Sie Details zur verwendeten MFA-Lösung eines Drittanbieters mitteilen, die Integrationsmethode angeben (z. B. über einen Identitätsverbund oder die Verwendung eines benutzerdefinierten Azure AD-Steuerelements) und die folgenden Informationen als unterstützende Dokumente bereitstellen:
* Die Drittanbieter-MFA-Konfigurationen. 
* Das Ergebnis von [Testen der Sicherheitsanforderungen für Partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements), das vom Drittanbieter-MFA-fähigen Konto ausgeführt wird.
* Die Bestellung der Drittanbieter-MFA-Lösung, die Sie bereits verwenden oder verwenden möchten.


### <a name="how-to-submit-a-request-for-technical-exception"></a>Einreichen einer Anfrage für eine technische Ausnahme

So reichen Sie eine Anfrage für eine technische Ausnahme ein:

1. Melden Sie sich bei Partner Center als globaler Administrator oder Administrator-Agent an.
2. Erstellen Sie eine neue Partner-Serviceanfrage, indem Sie zu **Support** > **Partner-Supportanfragen** navigieren und auf **Neue Anfrage** klicken.
3. Suchen Sie im Suchfeld nach **MFA – Request for exception** (MFA – Anfrage einer Ausnahme), oder wählen Sie nacheinander **CSP** in „Kategorie“, **Konten, Onboarding, Zugriff** in „Thema“, **MFA – Request for exception** im Unterthema und **Nächster Schritt** aus.
4. Geben Sie die zum Einreichen einer Serviceanfrage erforderlichen Details an, und klicken Sie dann auf **Übermitteln**.

Es kann bis zu drei Arbeitstage dauern, bis Microsoft eine Antwort auf eine Anfrage für eine technische Ausnahme bereitstellt.
