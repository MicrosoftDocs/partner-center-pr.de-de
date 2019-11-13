---
title: Überprüfen der MFA für Ihren Partner Mandanten | Partner Center
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Details zum Überprüfen der mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA) für die Sicherheitsanforderungen Ihres Partner Mandanten
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: medium
ms.openlocfilehash: 9241e7fd7f9812e2c456eac70065e185a9cf8d61
ms.sourcegitcommit: 0f14e29540c6814f01395924223b495cc5299954
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/13/2019
ms.locfileid: "73983351"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) für Ihren Partner Mandanten

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direktrechnung
  - Indirekter Anbieter
  - Indirekter Händler
- Alle Berater

Diese Partner müssen die MFA-Überprüfung für die folgenden Bereiche durchführen:

- [Partner Center-Dashboard](#partner-center-dashboard) (Ausrichtung auf H1 CY2020)
- [Partner Center-API](#partner-center-api) (Ausrichtung auf H1 CY2020)
- [Partner delegierte Administration](#partner-delegated-administration) (ab dem 18. November 2019)

Diese Funktion soll Partnern helfen, Ihren Zugriff auf Kunden Ressourcen vor Kompromittierungen von Anmelde Informationen zu schützen.

## <a name="partner-center-dashboard"></a>Partner Center-Dashboard
Bestimmte Seiten im Partner Center-Dashboard werden MFA-geschützt, einschließlich:

* Alle Seiten auf der Registerkarte **Customers** .
* Alle Seiten auf der Registerkarte " **Support > Kundenanforderungen** ".

Wenn Sie versuchen, auf eine dieser Seiten zuzugreifen, und Sie die MFA-Überprüfung noch nicht abgeschlossen haben, müssen Sie dies tun.

Die folgenden Benutzer Typen sind für den Zugriff auf diese MFA-geschützten Seiten autorisiert und sind daher von diesem Feature betroffen, einschließlich:

* Administrator-Agents
* Vertriebs-Agents
* Helpdesk-Agents

Um zu veranschaulichen, wie dies funktioniert, sollten Sie die folgenden beiden Beispiele in Erwägung gezogen.

**Beispiel 1: Partner hat Azure AD MFA implementiert**
1.  Jane arbeitet für CSP. Die MFA für alle Benutzer unter dem Partner Mandanten von "MFA" wurde von "MFA" mithilfe von Azure AD MFA implementiert.
2.  Andrea startet von Ihrer Arbeitsstation aus eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet Jane an Azure AD um sich anzumelden.
3.  Aufgrund der vorhandenen Azure AD MFA-Einrichtung durch "Configuration Manager" muss Andrea die MFA-Überprüfung durchführen. Nach erfolgreicher Anmeldung und MFA-Überprüfung wird Andrea zurück zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4.  Andrea versucht, auf eine der MFA-geschützten Seiten im Partner Center zuzugreifen. Andrea hat die MFA-Überprüfung bereits während der Anmeldung bereits abgeschlossen, kann Andrea auf die MFA-geschützte Seite zugreifen, ohne die MFA-Überprüfung erneut durchlaufen zu müssen.

**Beispiel 2: Partner hat MFA von Drittanbietern mithilfe des Identitäts Verbunds implementiert.**
1. Trent funktioniert für CSP Wingtip. Wingtip hat MFA für alle Benutzer unter dem Wingtip-Partner Mandanten mithilfe von MFA von Drittanbietern implementiert, die mit Azure AD über den Identitäts Verbund integriert ist.
2. Auf seiner Arbeitsstation startet Trent eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet Justin an Azure AD an, um sich anzumelden.
3. Da Wingtip den Identitäts Verbund eingerichtet hat, leitet Azure AD Trent zum Verbund Identitäts Anbieter um, um die Anmeldung und MFA-Überprüfung abzuschließen. Nach erfolgreicher Anmeldung und MFA-Überprüfung wird Trent zurück an Azure AD und dann auf die Übersichtsseite des Partner Center-Dashboards umgeleitet.
4. Justin versucht, auf eine der MFA-geschützten Seiten im Partner Center zuzugreifen. Da bei der früheren Anmeldung bereits die MFA-Überprüfung durch die MFA-Überprüfung abgeschlossen wurde, kann der Zugriff auf die MFA-geschützte Seite durch die MFA-Überprüfung nicht mehr erforderlich sein.

**Beispiel 3: der Partner hat MFA nicht implementiert.**
1. John arbeitet für CSP fabrikam. Fabrikam hat MFA für keinen Benutzer unter dem Fabrikam-Partner Mandanten implementiert.
2. John startet von seiner Arbeitsstation aus eine neue Browsersitzung und navigiert zur Übersichtsseite des Partner Center-Dashboards (die nicht durch MFA geschützt ist). Partner Center leitet John an Azure AD um sich anzumelden.
3. Da Fabrikam MFA noch nicht implementiert hat, muss John die MFA-Überprüfung nicht durchführen. Nach erfolgreicher Anmeldung wird John zurück zur Übersichtsseite für das Partner Center-Dashboard umgeleitet.
4. John versucht, auf eine der MFA-geschützten Seiten im Partner Center zuzugreifen. Da John die MFA-Überprüfung nicht abgeschlossen hat, leitet Partner Center John an Azure AD um, um die MFA-Überprüfung abzuschließen. Da dies das erste Mal ist, dass John die MFA durchführen muss, wird John außerdem aufgefordert, sich mit Microsoft Authenticator App für MFA zu registrieren. Bei erfolgreicher MFA-Registrierung und MFA-Überprüfung kann John nun auf die MFA-geschützte Seite zugreifen.

## <a name="partner-center-api"></a>Partner Center-API

Die Partner Center-API unterstützt sowohl reine App-Authentifizierung als auch APP-und Benutzerauthentifizierung. Wenn die APP-und Benutzerauthentifizierung verwendet wird, benötigt Partner Center die MFA-Überprüfung. Genauer gesagt, wenn eine Partner Anwendung eine API-Anforderung an das Partner Center senden möchte, muss Sie ein Zugriffs Token im Autorisierungs Header der Anforderung enthalten. Wenn Partner Center eine API-Anforderung mit einem Zugriffs Token empfängt, das mit der APP-und Benutzerauthentifizierung abgerufen wurde, prüft die Partner Center-API, ob der *MFA* -Wert im *Authentifizierungsmethoden Verweis (AMR)* -Anspruch vorhanden ist. Sie können einen JWT-Decoder verwenden, um zu überprüfen, ob ein Zugriffs Token den erwarteten Wert für Authentifizierungsmethoden Verweis (AMR) enthält.

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

Wenn der Wert vorhanden ist, schließt Partner Center ab, dass die MFA-Überprüfung abgeschlossen wurde, und verarbeitet die API-Anforderung. Wenn der Wert nicht vorhanden ist, lehnt die Partner Center-API die Anforderung mit der folgenden Antwort ab:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>Partner delegierte Administration

### <a name="using-service-portals"></a>Verwenden von Dienst Portalen

Partnerkonten, einschließlich Administrator-Agents und helpdeskagents, können Ihre Partner delegierten Administratorrechte zum Verwalten von Kunden Ressourcen über Microsoft Online Services-Portale, Befehlszeilenschnittstelle (CLI) und APIs (mit App-und Benutzerauthentifizierung) verwenden.

Beim Zugriff auf Microsoft Online Services-Portale mithilfe der Partner delegierten Administratorrechte zum Verwalten von Kunden Ressourcen erfordern viele dieser Portale, dass sich das Partner Konto interaktiv authentifiziert, wobei der Kunde Azure Active Directory Mandanten als der Authentifizierungs Kontext: das Partnerkonto ist für die Anmeldung beim Kunden Mandanten erforderlich.

Wenn Azure Active Directory solche Authentifizierungsanforderungen empfängt, muss das Partnerkonto die MFA-Überprüfung durchführen. Je nachdem, ob es sich bei dem Partnerkonto um eine verwaltete oder eine Verbund Identität handelt, gibt es zwei Möglichkeiten:

- Wenn das Partnerkonto eine **verwaltete** Identität ist, fordert Azure Active Directory den Benutzer direkt auf, die MFA-Überprüfung abzuschließen. Wenn das Partnerkonto noch nicht für die mAzure Active Directory FA registriert ist, wird der Benutzer zuerst aufgefordert, die [MFA-Registrierung abzuschließen](#mfa-registration-experience) .

- Wenn es sich bei dem Partnerkonto um eine Verbund Identität handelt, ist die Vorgehensweise davon abhängig, wie der Partner Administrator den **Verbund** in Azure Active Directory konfiguriert hat. Beim Einrichten eines Verbunds in Azure Active Directory kann der Partner Administrator Azure Active Directory, ob der Verbund Identitäts Anbieter MFA unterstützt. Wenn dies der Fall ist, leitet Azure Active Directory den Benutzer an den Verbund Identitäts Anbieter weiter, um die MFA-Überprüfung abzuschließen. Andernfalls wird der Benutzer von Azure Active Directory direkt aufgefordert, die MFA-Überprüfung abzuschließen. Wenn das Partnerkonto noch nicht für die mAzure Active Directory FA registriert ist, wird der Benutzer zuerst aufgefordert, die [MFA-Registrierung abzuschließen](#mfa-registration-experience) .

Die gesamte Benutzerfreundlichkeit ähnelt dem Szenario, in dem ein Endkunden Mandant MFA für seine Administratoren implementiert hat. Beispielsweise hat der Kunden Mandant [Azure AD Baseline-Richtlinie aktiviert: MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), bei der alle Konten mit Administratorrechten bei der MFA-Überprüfung, einschließlich Administrator-Agents und helpdeskagents, beim Kunden Mandanten angemeldet werden müssen. Zu Testzwecken können Partner die [Richtlinie MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) im Kunden Mandanten aktivieren und dann versuchen, Delegierte Administratorrechte für den Zugriff auf den Kunden Mandanten zu verwenden.

> [!NOTE]
> Nicht alle Microsoft Online Service-Portale erfordern, dass sich Partnerkonten beim Kunden Mandanten beim Zugriff auf Kunden Ressourcen mit Delegierten Administratorrechten für Partner anmelden. Stattdessen müssen sich nur die Partnerkonten beim Partner Mandanten anmelden. Ein Beispiel hierfür ist das Exchange Admin Center. Im Laufe der Zeit erwarten wir, dass diese Portale Partnerkonten benötigen, um sich beim Kunden Mandanten anzumelden, wenn Partner delegierte Administratorrechte verwenden.

### <a name="using-service-apis"></a>Verwenden von Dienst-APIs
Einige Microsoft Online Services-APIs (z. b. Azure Resource Manager, Azure AD Graph, Microsoft Graph usw.) unterstützen Partner, die Delegierte Administratorrechte für Partner verwenden, um die Kunden Ressourcen Programm gesteuert zu verwalten. Um Partner delegierte Administratorrechte mit diesen APIs zu nutzen, muss die Partner Anwendung ein Zugriffs Token in den API-Anforderungs Autorisierungs Header einschließen, bei dem das Zugriffs Token durch ein Partner Benutzerkonto für die Authentifizierung mit Azure AD abgerufen wird. Customer Azure AD als Authentifizierungs Kontext festgelegt. Die Partner Anwendung muss über ein Partner Benutzerkonto beim Kunden Mandanten angemeldet sein.

Wenn Azure AD z. b. Authentifizierungsanforderungen empfängt, benötigt Azure AD das Partner Benutzerkonto, um die MFA-Überprüfung abzuschließen. Wenn das Partner Benutzerkonto noch nicht für MFA registriert wurde, wird das Benutzerkonto zuerst aufgefordert, die MFA-Registrierung abzuschließen.

Alle Partneranwendungen, die in diese APIs mit Delegierten Administratorrechten für Partner integriert sind, sind von diesem Feature betroffen. Um sicherzustellen, dass Partneranwendungen mit diesen APIs weiterhin ohne Unterbrechung arbeiten können:

- Der Partner muss die Verwendung einer nicht interaktiven Benutzer Authentifizierungsmethode mit Azure AD vermeiden, um das Zugriffs Token abzurufen. Bei Verwendung einer nicht interaktiven Benutzer Authentifizierungsmethode, wie z. b. des Kenn [Wort Flusses](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), kann Azure AD den Benutzer nicht auffordern, die MFA-Überprüfung abzuschließen. Der Partner muss stattdessen zur Verwendung interaktiver Benutzer Authentifizierungsmethoden wie [OpenID Connect Flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) wechseln.
- Während der interaktiven Benutzer Authentifizierungsmethode sollte der Partner ein Partner Benutzerkonto verwenden, das bereits für MFA aktiviert ist. Wenn Sie von Azure AD aufgefordert werden, können Partner die MFA-Registrierung und die MFA-Überprüfung während der Anmeldung abschließen.
- Dies ähnelt dem Szenario, in dem ein Endkunden Mandant MFA für seine Administratoren implementiert hat. Beispielsweise hat der Kunden Mandant [Azure AD Basis Richtlinien-MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)aktiviert, bei der alle Benutzerkonten mit Administratorrechten bei der MFA-Überprüfung, einschließlich Administrator-Agents und helpdeskagents, beim Kunden Mandanten angemeldet werden müssen. Zu Testzwecken können Partner die [Richtlinie für die MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) im Kunden Mandanten aktivieren und dann versuchen, die delegierten Administratorrechte für Partner für den programmgesteuerten Zugriff auf den Kunden Mandanten zu verwenden.

### <a name="mfa-registration-experience"></a>MFA-Registrierung
Wenn das Partnerkonto bei der MFA-Überprüfung noch nicht für MFA registriert ist, fordert Azure AD den Benutzer auf, zuerst die MFA-Registrierung abzuschließen:

![MFA-Registrierung, Schritt 1](images/MfaRegistration1.png)

Nachdem Sie auf **weiter**geklickt haben, wird der Benutzer zur Auswahl aus einer Liste mit Überprüfungsmethoden (einschließlich Telefon, SMS und Authentifikator-APP) aufgefordert.

![MFA-Registrierung, Schritt 2](images/MfaRegistration2.png)

Nach erfolgreicher Registrierung muss der Benutzer die MFA-Überprüfung basierend auf der vom Benutzer ausgewählten Überprüfung durchführen.



## <a name="request-for-technical-exception"></a>Technische Ausnahme anfordern

Partner können eine technische Ausnahme anwenden, um die MFA-Überprüfung zu unterdrücken, wenn Sie technische Probleme mit Microsoft Online Services haben und keine mögliche Lösung oder Problem Umgehung vorliegt. Lesen Sie hierzu die folgenden Abschnitte:

 - [Liste der von Partnern gemeldeten häufigen Probleme](#list-of-common-issues-reported-by-partners)
 - [Übermitteln einer Anforderung für eine technische Ausnahme](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Liste der von Partnern gemeldeten häufigen Probleme
Bevor Sie eine technische Ausnahme anwenden, überprüfen Sie die Liste der häufigen Probleme, die von anderen Partnern gemeldet wurden, um zu verstehen, ob es sich um gültige Gründe für eine technische Ausnahme handelt.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problem 1: der Partner benötigt mehr Zeit, um MFA für die Partner-Agents zu implementieren
Ein Partner wurde noch nicht gestartet oder ist noch nicht im Prozess der Implementierung von MFA für die Partner-Agents, die Zugriff auf Microsoft Online Services-Portale mit Delegierten Administratorrechten für die Verwaltung von Kunden Ressourcen benötigen. Der Partner benötigt mehr Zeit, um die MFA-Implementierung abzuschließen. Ist dies ein gültiger Grund für eine technische Ausnahme?

**Antwort**: Nein. Der Partner muss planen, die MFA für Ihre Benutzer zu implementieren, um Unterbrechungen zu vermeiden.

> [!NOTE]
> Obwohl der Partner die MFA für seine Partner-Agents nicht implementiert hat, können die Partner Agenten weiterhin mithilfe der delegierten Administratorrechte von Partner auf Microsoft Online Services-Portale zugreifen, sofern Sie die MFA-Registrierung und MFA-Überprüfung durchführen können Wenn Sie während der Anmeldung beim Kunden Mandanten aufgefordert werden. Durch das Abschließen der MFA-Registrierung wird der Benutzer nicht automatisch für MFA aktiviert.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problem 2: der Partner hat die MFA nicht für Benutzerkonten implementiert, die keine delegierten Administratorrechte verwenden.
Ein Partner verfügt über einige Benutzer in seinen Partner Mandanten, die keinen Zugriff auf Microsoft Online Services-Portale benötigen, um Kunden Ressourcen mit delegierten Administrator Berechtigungen von Partnern zu verwalten. Der Partner ist gerade dabei, MFA für diese Benutzer zu implementieren und benötigt mehr Zeit, um den Vorgang abzuschließen. Ist dies ein gültiger Grund für eine technische Ausnahme?

**Antwort**: Nein. Da diese Benutzerkonten keine Partner delegierten Administratorrechte zum Verwalten von Kunden Ressourcen verwenden, müssen Sie sich nicht beim Kunden Mandanten anmelden. Sie werden von Azure AD, die während der Anmeldung beim Kunden Mandanten die MFA-Überprüfung erfordern, nicht beeinträchtigt.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3: der Partner hat die MFA für Benutzer Dienst Konten nicht implementiert.
Ein Partner verfügt über einige Benutzerkonten in seinen Partner Mandanten, die von Geräten als Dienst Konten verwendet werden. Dabei handelt es sich im Allgemeinen um Konten mit geringen Rechten, die keinen Zugriff auf Partner Center-oder Microsoft Online Services-Portale benötigen, um Kunden Ressourcen mit delegierten Administrator Berechtigungen von Partnern zu verwalten Ist dies ein gültiger Grund für eine technische Ausnahme?

**Antwort**: Nein. Da diese Benutzerkonten keine Partner delegierten Administratorrechte zum Verwalten von Kunden Ressourcen verwenden, müssen Sie sich nicht beim Kunden Mandanten anmelden. Sie werden von Azure AD, die während der Anmeldung beim Kunden Mandanten die MFA-Überprüfung erfordern, nicht beeinträchtigt.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4: der Partner kann MFA nicht mithilfe der MS Authenticator-App implementieren.
Ein Partner verfügt über eine "Clean Desk"-Richtlinie, die es Mitarbeitern nicht gestattet, Ihre persönlichen mobilen Geräte in Ihren Arbeitsbereich zu bringen. Ohne Zugriff auf Ihre persönlichen mobilen Geräte können die Mitarbeiter die MS Authenticator-APP nicht installieren. Dies ist die einzige MFA-Überprüfung, die von Azure AD Basis Richtlinien unterstützt wird. Ist dies ein gültiger Grund für eine technische Ausnahme?

**Antwort**: Nein, dies ist kein gültiger Grund für eine technische Ausnahme. Der Partner sollte die folgenden alternativen berücksichtigen, damit Ihre Mitarbeiter beim Zugriff auf Partner Center weiterhin die MFA-Überprüfung durchführen können:
- Mit Ausnahme der MS Authenticator-App können Azure AD Baseline-Richtlinien auch mit einer von Drittanbietern kompatiblen Authentifikator-App verwendet werden, bei der es sich unter Umständen um Windows-Computer mit Microsoft Windows handelt.
- Partner können sich auch für Azure AD Premium-oder Drittanbieter-MFA-Lösungen registrieren (kompatibel mit Azure AD), die zusätzliche Überprüfungsmethoden bereitstellen können.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5: der Partner kann die MFA aufgrund der Verwendung von Legacy Authentifizierungs Protokollen nicht implementieren
Ein Partner verfügt über einige Partner-Agents, die weiterhin ältere Authentifizierungsprotokolle verwenden, die nicht mit MFA kompatibel sind. Beispielsweise verwenden die Benutzer weiterhin Outlook 2010, das auf Legacy Authentifizierungs Protokollen basiert. Wenn Sie die MFA für diese Partner-Agents aktivieren, wird die Verwendung von Legacy Authentifizierungs Protokollen unterbrochen.

**Antwort**: Nein, dies ist kein gültiger Grund für eine technische Ausnahme. Es wird dringend empfohlen, dass Partner aufgrund potenzieller Sicherheitsrisiken von der Verwendung veralteter Authentifizierungsprotokolle Weg gehen, da diese Protokolle nicht mit der MFA-Überprüfung geschützt werden können und für die Gefährdung von Anmelde Informationen weitaus anfälliger sind. Wenn der Wechsel von der Verwendung von Legacy Authentifizierungs Protokollen nicht möglich ist, sollten sich die Partner für Azure AD Premium registrieren, die die Verwendung von Anwendungs Kennwörtern unterstützt. Anwendungs Kennwörter sind einmalig vom systemgenerierte Kenn Wörter, die in der Regel stärker als von Menschen generierte Kenn Wörter sind. Mithilfe von Anwendungs Kennwörtern können Partner MFA für Ihre Benutzer implementieren und dabei nur auf Anwendungs Kennwörter für ältere Authentifizierungsprotokolle zurückgreifen.

> [!NOTE]
> Obwohl der Partner die MFA für seine Partner-Agents nicht implementiert hat, können die Partner Agenten weiterhin mithilfe der delegierten Administratorrechte von Partner auf Microsoft Online Services-Portale zugreifen, sofern Sie die MFA-Registrierung und MFA-Überprüfung durchführen können Wenn Sie während der Anmeldung beim Kunden Mandanten aufgefordert werden. Durch das Abschließen der MFA-Registrierung wird der Benutzer nicht automatisch für MFA aktiviert.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>Problem 6: der Partner verwendet Exchange Online PowerShell, die MFA nicht unterstützt.
Ein Partner verwendet Exchange Online-PowerShell mit Delegierten Administratorrechten für Partner, um den Exchange Online-Dienst im Namen Ihrer Kunden zu verwalten. Exchange Online PowerShell bietet keine Unterstützung für MFA. Wenn Partner MFA für Ihre Benutzer implementiert, können diese Benutzer nicht mehr auf Exchange Online-PowerShell zugreifen. Ist dies ein gültiger Grund für eine technische Ausnahme?

**Antwort**: Ja, dies kann als gültiger Grund für eine technische Ausnahme angesehen werden. Das vorhandene [Exchange Online-PowerShell-Modul, das Partner delegierte Administration unterstützt](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , erfordert nicht, dass sich Partner Benutzer beim Kunden Mandanten anmelden und daher nicht von Azure AD, die die MFA-Überprüfung benötigen, beeinträchtigt werden. Es ist jedoch nicht MFA-kompatibel. Das Microsoft Exchange Online-Team entwickelt ein neues PowerShell-Modul, das sowohl Delegierte Administratorrechte für Partner als auch MFA unterstützt. Bis das neue PowerShell-Modul verfügbar ist, können Partner MFA nicht für Benutzer implementieren, die das vorhandene PowerShell-Modul verwenden müssen. Wenn diese Benutzer Schwierigkeiten beim Zugriff auf andere Microsoft Online Services haben, weil Azure Ad die MFA-Überprüfung während der Mandanten übergreifenden Anmeldung erfordert, können Partner eine technische Ausnahme anfordern, um die MFA-Überprüfung zu unterdrücken.

> [!NOTE]
> Obwohl der Partner MFA für Benutzer, die Zugriff auf das Exchange Online-PowerShell-Modul benötigen, nicht implementieren kann, können diese Benutzer weiterhin auf Microsoft Online Services zugreifen, um Kunden Ressourcen mit delegierten Administrator Berechtigungen für Partner zu verwalten. Sie können die MFA-Registrierung und die MFA-Überprüfung durchführen, wenn Sie während der Anmeldung beim Kunden Mandanten aufgefordert werden. Durch das Abschließen der MFA-Registrierung wird der Benutzer nicht automatisch für die MFA aktiviert und hat daher keinen Einfluss auf den Zugriff auf das Exchange Online-PowerShell-Modul

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>Problem 7: Partner hat MFA von Drittanbietern implementiert, die von Azure AD nicht erkannt wird.
Ein Partner hat MFA für Ihre Benutzer mithilfe einer MFA-Lösung eines Drittanbieters implementiert. Der Partner kann jedoch die MFA-Lösung eines Drittanbieters nicht ordnungsgemäß konfigurieren, um zu Azure AD, dass die MFA-Überprüfung während der Benutzerauthentifizierung abgeschlossen wurde. Ist dies ein gültiger Grund für eine technische Ausnahme?

**Antwort**: Ja, dies kann als gültiger Grund für eine technische Ausnahme angesehen werden. Vergewissern Sie sich vor dem Übermitteln einer technischen Ausnahme, dass die MFA-Lösung mit dem MFA-Lösungsanbieter eines Drittanbieters nicht so konfiguriert werden kann, dass der *authenticationmethodsreferences* -Anspruch (mit dem Wert *multipleauthn*) an Azure AD , um anzugeben, dass die MFA-Überprüfung während der Benutzerauthentifizierung abgeschlossen wurde. Wenn Sie eine technische Ausnahme Anfrage einreichen, geben Sie Details zur verwendeten MFA-Lösung eines Drittanbieters an, und geben Sie die Integrationsmethode (z. b. über einen Identitäts Verbund oder die Verwendung von Azure AD benutzerdefiniertem Steuerelement) an.

### <a name="how-to-submit-a-request-for-technical-exception"></a>Übermitteln einer Anforderung für eine technische Ausnahme

So senden Sie eine technische Ausnahme Anforderung:

1. Melden Sie sich bei Partner Center als globaler Administrator oder Administrator-Agent an.
2. Erstellen Sie einen neuen Partner Service Request, indem Sie zur **Unterstützung** > **Partner Supportanfragen** navigieren und auf **neue Anforderung**klicken.
4. Im Thema **MFA und sicheres Anwendungsmodell** sendet Gül **eine technische Ausnahme** als Problemtyp.
6. Geben Sie die zum Senden einer Service Request erforderlichen Details an, und klicken Sie auf **senden**.

Microsoft kann bis zu drei Arbeitstage in Anspruch nehmen, um eine Antwort auf eine technische Ausnahme anzufordern.
