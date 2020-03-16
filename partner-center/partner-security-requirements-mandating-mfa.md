---
title: Festlegen von MFA für Ihren Partnermandanten | Partner Center
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie das Festlegen von MFA für Ihre Partnermandanten dazu beiträgt, Ihren Zugriff auf Kundenressourcen zu sichern. Enthält Beispielszenarien.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: high
ms.openlocfilehash: bf57b489f84540e50e28df5568391818f50c79d4
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340188"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Festlegen von Multi-Factor Authentication (MFA) für Ihren Partnermandanten

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direktrechnung
  - Indirekter Anbieter
  - Indirekter Wiederverkäufer
- Alle Berater

**Geeignete Benutzer**
-    Alle aktivierten Benutzer einschließlich Gastbenutzer

Diese Partner müssen die MFA-Überprüfung für die folgenden Bereiche durchführen:

- [Partner Center-Dashboard](#partner-center-dashboard) (Ziel Q2 CY2020)
- [Partner Center-API](#partner-center-api) (Ziel Q2 CY2020)
- [Delegierte Partnerverwaltung](#partner-delegated-administration) (ab 18. November 2019)

Diese Funktion soll Partnern helfen, ihren Zugriff auf Kundenressourcen vor Kompromittierungen von Anmeldeinformationen zu schützen.

## <a name="partner-center-dashboard"></a>Partner Center-Dashboard
Bestimmte Seiten im Partner Center-Dashboard werden durch MFA geschützt, einschließlich:

* Alle Seiten auf der Registerkarte **Kunden**.
* Alle Seiten auf der Registerkarte **Support > Kundenanforderungen**.

Wenn Sie versuchen, auf eine dieser Seiten zuzugreifen und die MFA-Überprüfung zuvor nicht abgeschlossen haben, müssen Sie dies nun nachholen.

Die folgenden Benutzertypen sind beispielsweise für den Zugriff auf diese durch MFA geschützten Seiten autorisiert und daher von diesem Feature betroffen:

* Administrator-Agents
* Vertriebsbeauftragte
* Helpdesk-Agents

Um die Funktionsweise der Überprüfung zu veranschaulichen, sehen Sie sich die folgenden beiden Beispiele an.

**Beispiel 1: Partner hat Azure AD MFA implementiert**
1.    Jane arbeitet für CSP Contoso. Contoso hat MFA für alle Benutzer unter dem Contoso-Partnermandanten mit Azure AD MFA implementiert.
2.    Jane startet eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet Jane an Azure AD um, um sich anzumelden.
3.    Aufgrund der vorhandenen Azure AD MFA-Einrichtung durch Contoso muss Jane die MFA-Überprüfung durchführen. Nach erfolgreicher Anmeldung und MFA-Überprüfung wird Jane zurück zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4.    Jane versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da Jane die MFA-Überprüfung bei der Anmeldung bereits früher abgeschlossen hat, kann Jane auf die durch MFA geschützte Seite zugreifen, ohne die MFA-Überprüfung erneut durchlaufen zu müssen.

**Beispiel 2: Partner hat MFA von Drittanbietern mithilfe des Identitätsverbunds implementiert**
1. Trent arbeitet für CSP Wingtip. Wingtip hat Drittanbieter-MFA für alle Benutzer unter dem Wingtip-Partnermandanten implementiert, die über einen Identitätsverbund in Azure AD integriert ist.
2. Trent startet eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center Trent Jane an Azure AD um, um sich anzumelden.
3. Da Wingtip Identitätsverbund eingerichtet hat, leitet Azure AD Trent zum Verbundidentitätsanbieter um, um die Anmeldung und MFA-Überprüfung abzuschließen. Nach erfolgreicher Anmeldung und MFA-Überprüfung wird Trent zurück an Azure AD und dann zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4. Trent versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da Trent die MFA-Überprüfung bei der Anmeldung bereits früher abgeschlossen hat, kann Trent auf die durch MFA geschützte Seite zugreifen, ohne die MFA-Überprüfung erneut durchlaufen zu müssen.

**Beispiel 3: Partner hat MFA nicht implementiert**
1. John arbeitet für CSP Fabrikam. Fabrikam hat für keinen Benutzer unter dem Fabrikam-Partnermandanten MFA implementiert.
2. John startet eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet John an Azure AD um, um sich anzumelden.
3. Da Fabrikam MFA nicht implementiert hat, muss John die MFA-Überprüfung nicht durchführen. Nach erfolgreicher Anmeldung wird John zurück zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4. John versucht, auf eine der durch MFA geschützten Seiten im Partner Center zuzugreifen. Da John die MFA-Überprüfung nicht abgeschlossen hat, leitet Partner Center John an Azure AD um, um die MFA-Überprüfung abzuschließen. Da dies das erste Mal ist, dass John MFA ausführen muss, wird John außerdem aufgefordert, sich mit der Microsoft Authenticator-App für MFA zu registrieren. Nach erfolgreicher MFA-Registrierung und MFA-Überprüfung kann John nun auf die durch MFA geschützte Seite zugreifen.

## <a name="partner-center-api"></a>Partner Center-API

Die Partner Center-API unterstützt sowohl reine App-Authentifizierung als auch App- und Benutzerauthentifizierung. Wenn App- und Benutzerauthentifizierung verwendet wird, erfordert Partner Center eine MFA-Überprüfung. Genauer gesagt: Wenn eine Partneranwendung eine API-Anforderung an Partner Center senden möchte, muss sie ein Zugriffstoken in den Autorisierungsheader der Anforderung einschließen. Wenn Partner Center eine API-Anforderung mit einem Zugriffstoken empfängt, das mit App- und Benutzerauthentifizierung abgerufen wurde, prüft die Partner Center-API, ob der *MFA*-Wert im *AMR*-Anspruch (Authentication Method Reference) vorhanden ist. Sie können einen JWT-Decoder verwenden, um zu überprüfen, ob ein Zugriffstoken den erwarteten AMR-Wert enthält:

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
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
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

## <a name="partner-delegated-administration"></a>Vom Partner delegierte Verwaltung

### <a name="using-service-portals"></a>Verwenden von Dienstportalen

Partnerkonten, einschließlich Administrator-Agents und Helpdesk-Agents, können ihre vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen über Portale für Microsoft-Onlinedienste, die Befehlszeilenschnittstelle (CLI) und APIs (mit App- und Benutzerauthentifizierung) verwenden.

Beim Zugriff auf Portale für Microsoft-Onlinedienste mithilfe der vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen erfordern viele dieser Portale, dass sich das Partnerkonto interaktiv authentifiziert, wobei der Azure Active Directory-Mandant des Kunden als Authentifizierungskontext festgelegt ist: Das Partnerkonto ist für die Anmeldung beim Kundenmandanten erforderlich.

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

Nachdem er auf **Weiter** geklickt hat, wird der Benutzer aufgefordert, eine Auswahl aus einer Liste mit Überprüfungsmethoden (einschließlich Telefon, SMS und Authenticator-App) zu treffen.

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
Ein Partner verfügt über einige Benutzer in seinen Partnermandanten, die keinen Zugriff auf Portale für Microsoft-Onlinedienste benötigen, um Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen zu verwalten. Der Partner ist gerade dabei, MFA für diese Benutzer zu implementieren und benötigt mehr Zeit, um den Vorgang abzuschließen. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein Da diese Benutzerkonten keine vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen verwenden, müssen sie sich nicht beim Kundenmandanten anmelden. Sie sind nicht davon betroffen, dass Azure AD während der Anmeldung beim Kundenmandanten eine MFA-Überprüfung erfordert.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3: Partner hat MFA für Benutzerdienstkonten nicht implementiert
Ein Partner verfügt über einige Benutzerkonten in seinen Partnermandanten, die von Geräten als Dienstkonten verwendet werden. Dabei handelt es sich um Konten mit geringen Berechtigungen, die keinen Zugriff auf Partner Center oder Portale für Microsoft-Onlinedienste benötigen, um Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen zu verwalten. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein Da diese Benutzerkonten keine vom Partner delegierten Verwaltungsberechtigungen zum Verwalten von Kundenressourcen verwenden, müssen sie sich nicht beim Kundenmandanten anmelden. Sie sind nicht davon betroffen, dass Azure AD während der Anmeldung beim Kundenmandanten eine MFA-Überprüfung erfordert.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4: Partner kann MFA nicht mithilfe der MS Authenticator-App implementieren
Ein Partner verfügt über eine „Clean Desk“-Richtlinie, die es Mitarbeitern nicht gestattet, ihre persönlichen mobilen Geräte in ihrem Arbeitsbereich zu verwenden. Ohne Zugang zu ihren persönlichen mobilen Geräten können die Mitarbeiter die MS Authenticator-App nicht installieren, die die einzige MFA-Überprüfung ist, die von den Azure AD-Baselinerichtlinien unterstützt wird. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Nein, dies ist kein gültiger Grund für eine technische Ausnahme. Der Partner sollte die folgenden Alternativen berücksichtigen, damit seine Mitarbeiter beim Zugriff auf Partner Center die MFA-Überprüfung trotzdem durchführen können:
- Die Azure-Baselinerichtlinien können nicht nur mit der MS Authenticator-App, sondern auch mit einer kompatiblen Authenticator-App eines Drittanbieters verwendet werden. Dabei kann es sich um unterstützte Windows-Computer mit Microsoft Windows handeln.
- Partner können sich auch für Azure AD Premium oder MFA-Lösungen von Drittanbietern registrieren (kompatibel mit Azure AD), die zusätzliche Überprüfungsmethoden bereitstellen können.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5: Partner kann MFA aufgrund der Verwendung von Legacyauthentifizierungsprotokollen nicht implementieren
Ein Partner arbeitet mit einigen Partner-Agents zusammen, die noch ältere Authentifizierungsprotokolle verwenden, die nicht mit MFA kompatibel sind. Beispielsweise verwenden die Benutzer noch Outlook 2010, das auf Legacyauthentifizierungsprotokollen basiert. Wenn MFA für diese Partner-Agents aktiviert wird, wird die Verwendung von Legacyauthentifizierungsprotokollen unterbrochen.

**Antwort**: Nein, dies ist kein gültiger Grund für eine technische Ausnahme. Es wird dringend empfohlen, dass Partner aufgrund potenzieller Sicherheitsrisiken von der Verwendung veralteter Authentifizierungsprotokolle Abstand nehmen, da diese Protokolle nicht durch MFA-Überprüfung geschützt werden können und für eine Gefährdung von Anmeldeinformationen weitaus anfälliger sind. Wenn der Wechsel von der Verwendung von Legacyauthentifizierungsprotokollen nicht möglich ist, sollten sich Partner für Azure AD Premium registrieren, das die Verwendung von Anwendungskennwörtern unterstützt. Anwendungskennwörter sind einmalige, vom System generierte Kennwörter, die in der Regel stärker als manuell vom Benutzer generierte Kennwörter sind. Mithilfe von Anwendungskennwörtern können Partner MFA für ihre Benutzer implementieren und dabei auf Anwendungskennwörter nur für ältere Authentifizierungsprotokolle zurückgreifen.

> [!NOTE]
> Auch wenn der Partner MFA für seine Partner-Agents nicht implementiert hat, können die Partner-Agents dennoch auf Portale für Microsoft-Onlinedienste mit vom Partner delegierten Verwaltungsberechtigungen zugreifen – vorausgesetzt, sie können die MFA-Registrierung und MFA-Überprüfung abschließen, wenn sie bei der Anmeldung beim Kundenmandanten dazu aufgefordert werden. Das Abschließen der MFA-Registrierung aktiviert den Benutzer nicht automatisch für MFA.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-that-does-not-support-mfa"></a>Problem 6: Partner verwendet Exchange Online PowerShell ohne MFA-Unterstützung
Ein Partner verwendet Exchange Online PowerShell mit vom Partner delegierten Verwaltungsberechtigungen, um den Exchange Online-Dienst im Namen seiner Kunden zu verwalten. Exchange Online PowerShell bietet keine Unterstützung für MFA. Wenn der Partner MFA für seine Benutzer implementiert, können diese Benutzer nicht mehr auf Exchange Online PowerShell zugreifen. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Ja, dieses Problem kann als gültiger Grund für eine technische Ausnahme angesehen werden. Das vorhandene [Exchange Online PowerShell-Modul, das vom Partner delegierte Verwaltung](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) unterstützt, erfordert keinen Partnerbenutzer für die Anmeldung beim Kundenmandanten und ist daher von der Azure AD-Anforderung für MFA-Überprüfung nicht betroffen. Es ist jedoch nicht mit MFA kompatibel. Das Microsoft Exchange Online-Team entwickelt ein neues PowerShell-Modul, das sowohl vom Partner delegierte Verwaltungsberechtigungen als auch MFA unterstützt. Bis das neue PowerShell-Modul verfügbar ist, können Partner MFA nicht für Benutzer implementieren, die das vorhandene PowerShell-Modul verwenden müssen. Wenn diese Benutzer Schwierigkeiten beim Zugriff auf andere Microsoft-Onlinedienste haben, weil Azure AD MFA-Überprüfung während der mandantenübergreifenden Anmeldung erfordert, können Partner eine technische Ausnahme anfordern, um die MFA-Überprüfung zu unterdrücken.

> [!NOTE]
> Auch wenn der Partner MFA für Benutzer nicht implementieren kann, die Zugriff auf das Exchange Online PowerShell-Modul benötigen, können diese Benutzer dennoch auf Microsoft-Onlinedienste zugreifen, um Kundenressourcen mit vom Partner delegierten Verwaltungsberechtigungen zu verwalten – vorausgesetzt, sie können die MFA-Registrierung und MFA-Überprüfung abschließen, wenn sie bei der Anmeldung beim Kundenmandanten dazu aufgefordert werden. Das Abschließen der MFA-Registrierung aktiviert den Benutzer nicht automatisch für MFA und hat daher keinen Einfluss auf den Zugriff auf das Exchange Online PowerShell-Modul.

#### <a name="issue-7-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problem 7: Partner hat MFA von Drittanbietern implementiert, die von Azure AD nicht erkannt wird
Ein Partner hat MFA für seine Benutzer mit einer MFA-Lösung eines Drittanbieters implementiert. Der Partner kann jedoch die MFA-Lösung des Drittanbieters nicht ordnungsgemäß konfigurieren, um Azure AD zu vermitteln, dass die MFA-Überprüfung während der Benutzerauthentifizierung abgeschlossen wurde. Handelt es sich um einen gültigen Grund für eine technische Ausnahme?

**Antwort**: Ja, dieses Problem kann als gültiger Grund für eine technische Ausnahme angesehen werden. Lassen Sie sich vor dem Einreichen einer Anfrage für eine technische Ausnahme durch den MFA-Lösungsdrittanbieter bestätigen, dass die MFA-Lösung nicht so konfiguriert werden kann, dass der Anspruch *authenticationmethodsreferences* (mit dem Wert *multipleauthn*) an Azure AD übermittelt wird, um anzugeben, dass die MFA-Überprüfung während der Benutzerauthentifizierung abgeschlossen wurde. Wenn Sie eine Anfrage für eine technische Ausnahme einreichen, müssen Sie Einzelheiten zur verwendete MFA-Lösung des Drittanbieters und die Integrationsmethode (z. B. durch Identitätsverbund oder Verwendung von Azure AD Custom Control) angeben.

### <a name="how-to-submit-a-request-for-technical-exception"></a>Einreichen einer Anfrage für eine technische Ausnahme

So reichen Sie eine Anfrage für eine technische Ausnahme ein:

1. Melden Sie sich bei Partner Center als globaler Administrator oder Administrator-Agent an.
2. Erstellen Sie eine neue Partner-Serviceanfrage, indem Sie zu **Support** > **Partner-Supportanfragen** navigieren und auf **Neue Anfrage** klicken.
4. Im Thema **MFA und das sichere Anwendungsmodell** wählen Sie **Anfrage für technische Ausnahme einreichen** als Problemtyp aus.
6. Geben Sie die zum Einreichen einer Serviceanfrage erforderlichen Details an, und klicken Sie dann auf **Übermitteln**.

Es kann bis zu drei Arbeitstage dauern, bis Microsoft eine Antwort auf eine Anfrage für eine technische Ausnahme bereitstellt.
