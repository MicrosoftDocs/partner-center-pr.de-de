---
title: Sicherheitsanforderungen für Partner – FAQ | Partner Center
ms.topic: article
ms.date: 09/27/2019
description: Häufig gestellte Fragen zu den Sicherheitsanforderungen für Partner
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: high
ms.openlocfilehash: e9471ae8dd0e478540e30a879d010ffb0c1f1bc0
ms.sourcegitcommit: c388fae97437b727edeb0de3712bd2822010ecd6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/30/2019
ms.locfileid: "71678302"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Häufig gestellte Fragen zu den Sicherheitsanforderungen für Partner

Dieser Artikel enthält einige häufig gestellte Fragen zu den [Sicherheitsanforderungen für Partner](partner-security-requirements.md) sowie die entsprechenden Antworten.

## <a name="partner-security-requirements"></a>Sicherheitsanforderungen für Partner

### <a name="what-are-the-new-partner-security-requirements"></a>Welche neuen Sicherheitsanforderungen gelten für Partner?

Um unsere Partner und deine Kunden zu schützen, fordern wir Partner auf, sofort folgende Maßnahmen zu ergreifen:  

1. **Aktivieren der Multi-Factor Authentication (MFA) für alle Benutzer in Partnermandanten**. Alle Benutzer in Partnermandanten müssen die Multi-Factor Authentication (MFA) verwenden, wenn sie sich bei kommerziellen Microsoft-Clouddiensten anmelden oder im CSP (Cloud Solution Provider-Programm) Transaktionen über Partner Center oder APIs ausführen. Durch Aktivierung von Basisschutzrichtlinien ist die MFA kostenlos für alle Benutzer von Partnermandanten verfügbar.

2. **Übernehmen des Frameworks „Sicheres Anwendungsmodell“** . Alle Partner, die eine Integration in eine Microsoft-API wie Azure Resource Manager, Microsoft Graph und die Partner Center-API wünschen, müssen das Framework „Sicheres Anwendungsmodell“ übernehmen, um eine Unterbrechung der Integration zu vermeiden, wenn die Basisrichtlinien aktiviert werden.

Durch Aktivieren der Multi-Factor Authentication (MFA) und Übernehmen des Frameworks „Sicheres Anwendungsmodell“ kannst du deine Infrastruktur sowie die Daten deiner Kunden vor potenziellen Sicherheitsrisiken wie Identitätsdiebstahl oder anderen Betrugsversuchen schützen.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Welche Partner müssen die Anforderungen erfüllen?

Diese Anforderungen gelten für die folgenden Partnergruppen:

- Alle Partnerorganisationen, die am Cloud Solution Provider-Programm (CSP) teilnehmen und über die kommerziellen Clouddienste von Microsoft Transaktionen vornehmen
  - Alle Partner mit direkter Abrechnung
  - Indirekte Anbieter
  - Indirekte Vertriebspartner
- Alle Control Panel-Anbieter
- Alle Partner im Advisor-Programm  

Partner, die Transaktionen über eine unabhängige Cloud (21Vianet, US Government und Deutschland) ausführen, sind jedoch nicht verpflichtet, diese neuen Sicherheitsanforderungen zum 1. August zu erfüllen. Es wird jedoch allen Partnern, die über eine unabhängige Cloud handeln, dringend empfohlen, diese neuen Sicherheitsanforderungen sofort umzusetzen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

### <a name="what-are-the-key-timelines-and-milestones"></a>Welches sind die wichtigsten Zeitpläne und Meilensteine?

Die Bestimmungen in Bezug auf diese Sicherheitsanforderungen werden dem [Program Guide for Microsoft Cloud Solution Providers](https://go.microsoft.com/fwlink/p/?LinkId=617100) (Programmleitfaden für Cloud Solution Provider) sofort hinzugefügt. Du musst diese Sicherheitsanforderungen implementieren, um die Voraussetzungen für deine Teilnahme am CSP-Programm ab dem 1. August 2019 zu erfüllen.

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>Was geschieht, wenn ich nicht tätig werde?

Partner, die diese obligatorischen Sicherheitsverfahren nicht einhalten, werden nicht in der Lage sein, Transaktionen im Cloud Solution Provider-Programm auszuführen oder Kundenmandanten mit delegierten Administratorrechten zu verwalten, sobald diese Anforderungen in Kraft sind. Wir sind dabei, einen Termin festzulegen, ab dem diese Anforderungen verbindlich in Kraft treten, und werden den Partnern diesen Termin sowie detaillierte Informationen mitteilen.

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>Was passiert, wenn ich die MFA nicht gemäß diesen neuen Sicherheitsanforderungen bis 1. August 2019 implementiere?

Die Bestimmungen in Bezug auf diese Sicherheitsanforderungen im [Program Guide for Microsoft Cloud Solution Providers](https://go.microsoft.com/fwlink/p/?LinkId=617100) (Programmleitfaden für Cloud Solution Provider) sind am 1. August 2019 in Kraft getreten. Alle Partner im CSP-Programm müssen diese Anforderungen umsetzen, um die Programmbestimmungen zu erfüllen und ihr Geschäft zu schützen. Partner, die diese Sicherheitsverfahren nicht einhalten, werden möglicherweise nicht mehr in der Lage sein, Transaktionen im CSP-Programm auszuführen oder Kundenmandanten mit delegierten Administratorrechten zu verwalten, sobald wir mit der technischen Durchsetzung der Sicherheitsanforderungen für Partner begonnen haben (in naher Zukunft). Wir legen einen Termin für das Inkrafttreten der Anforderungen fest und werden unsere Partner in Kürze darüber informieren.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Warum setzt Microsoft diese neuen Anforderungen durch?

Sicherheit und Datenschutz von Kunden und Partnern haben für Microsoft oberste Priorität. Wir stellen immer mehr und immer ausgefeiltere Sicherheitsangriffe fest – insbesondere im Hinblick auf die Kompromittierung von Identitäten. Da präventive Maßnahmen in der Verteidigungsstrategie eine wichtige Rolle spielen, um Angriffe bereits im Vorfeld abzuwehren, beginnen wir damit, eine Reihe von obligatorischen Sicherheitsanforderungen durchzusetzen, die zum Schutz unserer Partner und deren Kunden beitragen.

### <a name="does-this-apply-to-all-geographies"></a>Gilt dies für alle geografischen Regionen?

Ja, dies gilt für alle geografischen Regionen. Es wird dringend empfohlen, dass alle Partner, die über eine unabhängige Cloud (21Vianet, US-Regierung und Deutschland) handeln, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner sind jedoch nicht verpflichtet, die neuen Sicherheitsanforderungen zum 1. August zu erfüllen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Sind Ausnahmen für ein Konto möglich?

Nein, kein Konto kann von der Anforderung ausgenommen werden, ein MFA-Verfahren einzurichten. Angesichts der umfassenden Privilegien, die mit dem Partnerstatus verbunden sind, müssen gemäß dem [Program Guide for Microsoft Cloud Solution Providers](https://go.microsoft.com/fwlink/p/?LinkId=617100) (Programmleitfaden für Cloud Solution Provider) MFA-Verfahren für jedes Konto in deinem Partnermandanten erzwungen werden.

## <a name="required-actions"></a>Erforderliche Aktionen

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Welches sind die wichtigsten Aktionen, die ich ausführen muss, um die Anforderungen zu erfüllen?

Alle Partner im CSP-Programm (Partner mit direkter Abrechnung, indirekte Anbieter und indirekte Handelspartner), Berater und Control Panel-Anbieter müssen die Anforderungen erfüllen.

1. **Durchsetzen der MFA für alle Benutzer**

    Alle Partner im CSP-Programm, Berater und Control Panel-Anbieter müssen die MFA für alle Benutzer in ihrem Partnermandanten erzwingen. Dies lässt sich durch Aktivieren der Basisrichtlinien [MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) sowie zukünftiger Basisrichtlinien erreichen. Die von den Basisrichtlinien bereitgestellte Funktionalität wird weiterentwickelt, um sicherzustellen, dass Partner und Kunden vor sich ständig ändernden Sicherheitsbedrohungen geschützt sind. Es ist also wichtig, die [Dokumentation zu den Basisrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) zu lesen, um mehr zu erfahren.

    - Unter [Basisrichtlinie: MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) findest du Informationen dazu, wie du diese Basisrichtlinie aktivierst.
    - Unter [Basisrichtlinie: Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) findest du Informationen dazu, wie du diese Basisrichtlinie aktivierst.
    - Grundlegendes zum Konzept der [Basisschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Weitere Überlegungen:

    - Indirekte Anbieter müssen für das Onboarding in Partner Center mit indirekten Handelspartnern zusammenarbeiten, sofern dies nicht bereits erfolgt ist, und ihre Handelspartner dazu anhalten, die Anforderungen zu erfüllen.
    - Die Azure MFA wird allen Benutzern im Partnermandanten über die Basisrichtlinien kostenlos zur Verfügung gestellt. Dabei ist die einzige Methode zur Verifizierung die [Microsoft Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Weitere Verifizierungsmethoden sind über die [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)-SKUs verfügbar, wenn andere Methoden wie ein Telefonanruf oder eine SMS erforderlich sind.
    - Beim Zugriff auf kommerzielle Clouddienste von Microsoft können Partner für jedes Konto auch die MFA-Lösung eines Drittanbieters nutzen.

2. **Übernehmen des Frameworks „Sicheres Anwendungsmodell“**

    Alle Partner, die eine benutzerdefinierte Integration über APIs (z. B. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) entwickelt oder mithilfe von PowerShell eine benutzerdefinierte Automatisierung implementiert haben, müssen das [Framework „Sicheres Anwendungsmodell“](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) übernehmen, um die Integration in Microsoft-Clouddienste zu ermöglichen. Eine Nichteinhaltung dieser Anforderung kann zu einer Unterbrechung aufgrund der MFA-Bereitstellung führen. Die folgenden Ressourcen bieten weitere Informationen sowie einen Leitfaden zur Übernahme des Modells.

    - [Übersicht über das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Partner Center: Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Dokumentation zur Authentifizierung in Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Dokumentation zur Multi-Factor Authentication (MFA) in Partner Center über PowerShell](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Wenn du eine Control Panel-Anwendung verwendest, musst du dich bezüglich der Übernahme des Frameworks „Sicheres Anwendungsmodell“ an den Hersteller wenden.

    Control Panel-Anbieter müssen das [Onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) in Partner Center als Control Panel-Anbieter durchführen und sofort mit der Umsetzung dieser Anforderung beginnen. Weitere Informationen findest du unter [Partner Center: Framework „Sicheres Anwendungsmodell“](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Control Panel-Anbieter müssen anstelle von Anmeldeinformationen die Zustimmung von CSP-Partnern akzeptieren und verwalten und alle vorhandenen Anmeldeinformationen von CSP-Partnern löschen.

## <a name="multi-factor-authentication"></a>Mehrstufige Authentifizierung

### <a name="what-is-multi-factor-authentication-mfa"></a>Was ist die Multi-Factor Authentication (MFA)?

Die MFA ist ein Sicherheitsmechanismus, mit dem Einzelpersonen über mehr als ein erforderliches Sicherheits- und Validierungsverfahren authentifiziert werden. Dabei sind mindestens zwei der folgenden Authentifizierungsmethoden erforderlich:

- Etwas, das Sie wissen (in der Regel ein Kennwort)
- Etwas, das Sie besitzen (ein vertrauenswürdiges Gerät, das sich nicht leicht duplizieren lässt, z. B. ein Telefon)
- Sie selbst (Biometrie)

### <a name="what-are-baseline-protection-policies"></a>Was sind Basisschutzrichtlinien?

[Microsoft-Basisschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (derzeit in der Vorschau) sind vordefinierte Richtlinien, die dabei helfen, Organisationen vor vielen gängigen Angriffen zu schützen. Diese allgemeinen Angriffe können Password Spray, Replay und Phishing einbeziehen. Basisrichtlinien sind in allen Editionen von Azure Active Directory verfügbar. Microsoft stellt diese Basisschutzrichtlinien allen Benutzern zur Verfügung, weil identitätsbasierte Angriffe seit einigen Jahren zunehmen. Ziel dieser Richtlinien ist es, sicherzustellen, dass alle Organisationen ohne zusätzliche Kosten über einen grundlegenden Schutz verfügen.

> [!NOTE]
> Die Basisrichtlinien von Microsoft und die zugehörigen Funktionen werden immer weiterentwickelt, um Partner und Kunden fortlaufend vor sich ständig ändernden Sicherheitsbedrohungen zu schützen. Möglicherweise treten in Kürze einige Änderungen hinsichtlich der Benennung und der Taxonomie der Basisschutzrichtlinien in Kraft. Microsoft empfiehlt dringend, regelmäßig die Seiten mit den Basisrichtlinien zu überprüfen, um die neuesten Informationen zu erhalten.

### <a name="what-baseline-policies-must-i-enable"></a>Welche Basisrichtlinien muss ich aktivieren?

Wenn du planst, die aktuellen Baselineschutzrichtlinien zu verwenden, um jedes Konto im Partnermandanten MFA-Verfahren zur Verfügung zu stellen, musst du auch die Baselinerichtlinien [MFA für Administratoren erfordern](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) aktivieren. Diese Basisschutzrichtlinien erfüllen die Anforderung eines kostenlosen MFA-Modells für jeden Benutzer im Partnermandanten nur für solche Partner, die Microsoft Authenticator-Apps über mobile Geräte verwenden.

Die Basisrichtlinie [MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) dient zum Schutz von Administratorbenutzern im Partnerverzeichnis, und mit der Basisrichtlinie [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) werden Nicht-Administratorbenutzer im Partnermandanten geschützt. Um diese Richtlinien zu aktivieren, müssen Benutzer sich für die MFA registrieren. Wenn die Benutzer nach der erfolgreichen Registrierung versuchen, sich anzumelden, werden sie basierend auf den Kriterien der Richtlinie zur Durchführung der entsprechenden MFA-Verfahren aufgefordert. Die von den Basisrichtlinien bereitgestellte Funktionalität wird weiterentwickelt, um sicherzustellen, dass Partner und Kunden vor sich ständig ändernden Sicherheitsbedrohungen geschützt sind. Es ist also wichtig, die [Dokumentation zu den Basisrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) zu lesen, um mehr zu erfahren.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Wie aktiviere ich die Richtlinie „MFA für Administratoren erforderlich“?

Die Basisrichtlinie „MFA für Administratoren erforderlich“ kann über das Azure-Verwaltungsportal aktiviert werden. Unter [Basisrichtlinie: MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) findest du Informationen dazu, wie du diese Basisrichtlinie aktivierst.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Wie aktiviere ich die Richtlinie „Endbenutzerschutz“?

Die Basisrichtlinie „Endbenutzerschutz“ kann über das Azure-Verwaltungsportal aktiviert werden. Unter [Basisrichtlinie: Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) findest du Informationen dazu, wie du diese Basisrichtlinie aktivierst.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>Werden die Basisrichtlinien automatisch aktiviert?

Nein. Zum Aktivieren dieser Richtlinien muss ein Benutzer, der Mitglied der Rolle „Globaler Administrator“, „Sicherheitsadministrator“ oder „Administrator für bedingten Zugriff“ ist, diese Richtlinien für die sofortige Verwendung konfigurieren.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Was kostet die Aktivierung der MFA?

Microsoft stellt die MFA über die Implementierung der Basisschutzrichtlinien [MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) kostenlos zur Verfügung. Die einzige Verifizierungsoption, die mit dieser Version der MFA zur Verfügung steht, ist die [Microsoft Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Wenn eine Verifizierung per Telefonanruf oder SMS erforderlich ist, muss eine Lizenz für [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) erworben werden. Alternativ dazu kannst du eine Drittanbieterlösung verwenden, um die MFA für jeden Benutzer in deinem Partnermandanten bereitzustellen. In diesem Fall liegt es in deiner Verantwortung, sicherzustellen, dass deine MFA-Lösung durchgesetzt wird und die Anforderungen erfüllt werden.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Wenn ich bereits über eine MFA-Lösung verfüge, welche Maßnahmen muss ich ergreifen?

Aufgrund dieser Sicherheitsanforderungen müssen Benutzer in einem Partnermandanten sich beim Zugriff auf kommerzielle Microsoft-Clouddienste mit MFA-Verfahren anmelden. Zur Erfüllung dieser Anforderungen kann auch eine Drittanbieterlösung eingesetzt werden. Microsoft stellt unabhängigen Identitätsanbietern keine Validierungstests mehr bereit, um die Kompatibilität mit Azure Active Directory zu überprüfen. Wenn du dein Produkt auf Interoperabilität testen möchtest, findest du weitere Informationen in diesen [Richtlinien](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Wenn Sie eine Drittanbieterlösung verwenden, muss überprüft werden, ob die Lösung den AMR-Anspruch (Authentication Method Reference) ausgibt, der den MFA-Wert enthält. Details zur Überprüfung, ob Ihre Drittanbieterlösung den erwarteten Anspruch ausgibt, finden Sie unter [Testing the Partner Security Requirements](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) (Testen der Partneranforderungen an die Sicherheit).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Welche Verifizierungsmethode kann ich für die Authentifizierung per MFA verwenden?

Microsoft stellt die MFA über die Implementierung der Basisschutzrichtlinien [MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) kostenlos zur Verfügung. Die einzige Verifizierungsoption, die mit dieser Version der MFA zur Verfügung steht, ist die [Microsoft Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Wenn eine Verifizierung per Telefonanruf oder SMS erforderlich ist, muss eine Lizenz für [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) erworben werden. Alternativ dazu kannst du eine Drittanbieterlösung verwenden, um die MFA für jeden Benutzer in deinem Partnermandanten bereitzustellen. In diesem Fall liegt es in deiner Verantwortung, sicherzustellen, dass deine MFA-Lösung durchgesetzt wird und die Anforderungen erfüllt werden.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Ich führe Transaktionen mit mehreren Partnermandanten aus. Muss ich die MFA für alle Mandanten implementieren?

Ja, du musst die MFA für jeden Azure Active Directory-Mandanten erzwingen, der dem CSP-Programm oder dem Advisor-Programm zugeordnet ist. Wenn du planst, eine Lizenz für Azure Active Directory Premium zu erwerben, muss auch für den Benutzer in jedem Azure Active Directory-Mandanten eine Lizenz erworben werden.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Muss für jeden meiner Partnermandanten die MFA erzwungen werden?*

Die Basisschutzrichtlinien [MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) erzwingen die MFA für jeden Mandanten in deinem Partnermandanten. Wenn du diese Richtlinien zum Bereitstellen der MFA nutzt und die [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)-Anwendung verwendest, musst du keine zusätzlichen Lizenzen erwerben. Andernfalls musst du eine geeignete Lösung erwerben, um jedem Benutzer in deinem Partnermandanten ein MFA-Verfahren bereitzustellen.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Ich bin Microsoft-Partner mit direkter Abrechnung. Wie muss ich vorgehen?

Cloud Solution Provider-Partner mit direkter Abrechnung müssen die MFA für jeden Benutzer in ihrem Partnermandanten erzwingen.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Ich bin indirekter Handelspartner und führe Transaktionen nur über einen Distributor durch. Muss ich trotzdem Maßnahmen ergreifen?

Alle indirekten Handelspartner müssen die MFA für jeden Benutzer in ihrem Partnermandanten erzwingen. Dies ist eine Maßnahme, die vom indirekten Handelspartner durchgeführt werden muss.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Ich verwende die Partner Center-API nicht. Muss ich die MFA dennoch implementieren?

Ja. Diese Sicherheitsanforderung gilt für alle Benutzer – einschließlich Administratorbenutzern von Partnern und Endbenutzern in einem Partnermandanten.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Welche Drittanbieter stellen MFA-Lösungen bereit, die mit Azure Active Directory kompatibel sind?

Online gibt es eine Vielzahl unabhängiger Bewertungen von MFA-Lösungen, z. B. von [Gartner](https://www.gartner.com/en/webinars/3881781). Bei der Überprüfung von MFA-Anbietern und -Lösungen müssen Partner sicherstellen, dass die ausgewählte Lösung mit Azure Active Directory kompatibel ist.

Microsoft stellt unabhängigen Identitätsanbietern keine Validierungstests mehr bereit, um die Kompatibilität mit Azure Active Directory zu überprüfen. Wenn du dein Produkt auf Interoperabilität testen möchtest, findest du weitere Informationen in diesen [Richtlinien](https://www.microsoft.com/download/details.aspx?id=56843).

Weitere Informationen findest du hier: [Azure AD-Verbund – Kompatibilitätsliste](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Wie kann ich die MFA in unserer Sandbox für die Integration testen?

Die Basisrichtlinien [MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) müssen für deinen Sandbox-Mandanten für die Integration aktiviert werden. Aufgrund dieser Richtlinien muss sich jeder Benutzer im Mandanten per MFA authentifizieren.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>Wirkt sich die Aktivierung der MFA darauf aus, wie ich mit dem Mandanten meines Kunden interagiere?

Nein. Die Erfüllung dieser Sicherheitsanforderungen wirkt sich nicht auf die Verwaltung der Kunden aus. Die Möglichkeit, delegierte administrative Vorgänge auszuführen, wird nicht beeinträchtigt.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Unterliegen meine Kunden den Sicherheitsanforderungen für Partner?

Nein. Die MFA muss nicht für jeden Benutzer in den Azure AD-Mandanten deiner Kunden erzwungen werden. Es empfiehlt sich allerdings, in Zusammenarbeit mit jedem Kunden zu ermitteln, wie die Benutzer der Kunden am besten geschützt werden können.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>Können bei den Basisschutzrichtlinien App-Kennwörter verwendet werden?

Ja, [App-Kennwörter](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) können verwendet werden. Du solltest die Überlegungen zur Verwendung von App-Kennwörtern überprüfen, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um zu ermitteln, ob sie für deine Anforderungen unterstützt werden.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Kann ein Benutzer von dieser Anforderung ausgenommen werden?

Nein. Jeder Benutzer im Partnermandanten, einschließlich aller Dienstkonten, muss sich per MFA authentifizieren.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Gelten die Sicherheitsanforderungen für Partner auch für die Sandbox zur Integration?

Ja. Die Sicherheitsanforderungen für Partner gelten auch für die Sandbox zur Integration. Das bedeutet, dass du für die Benutzer im Sandbox-Mandanten für die Integration eine geeignete MFA-Lösung implementieren musst. Es empfiehlt sich, die Basisschutzrichtlinien zu implementieren, um die MFA bereitzustellen.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Wie konfiguriere ich ein Konto für den Notfallzugriff?

Es hat sich bewährt, ein oder zwei Konten für den Notfallzugriff einzurichten, um eine versehentliche Aussperrung aus dem Azure AD-Mandanten zu verhindern. Aufgrund der Sicherheitsanforderungen für Partner muss sich jeder Benutzer per MFA authentifizieren. Das bedeutet, dass du die Definition eines Kontos für den Notfallzugriff ändern musst. Du könntest z. B. ein Konto verwenden, das eine Drittanbieterlösung für die MFA nutzt.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Wie wirken sich die Sicherheitsanforderungen für Partner auf Gastbenutzer aus?

Auch Gastbenutzer müssen sich per MFA authentifizieren, wenn sie auf Ressourcen in deinem Partnermandanten zugreifen. Die Sicherheitsanforderungen für Partner haben keine Auswirkungen darauf, wie Gastbenutzer auf Ressourcen in ihrem eigenen Mandanten zugreifen.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Wenn ich eine Drittanbieterlösung verwende, sind die Active Directory-Verbunddienste erforderlich?

Nein, bei Verwendung einer Drittanbieterlösung sind die Active Directory-Verbunddienste (AD FS) nicht erforderlich. Es empfiehlt sich, zusammen mit dem Lösungsanbieter zu ermitteln, welche Anforderungen für die Lösung bestehen.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>Ist die Aktivierung der Basisschutzrichtlinien erforderlich?

Nein, die Basisschutzrichtlinien müssen nicht aktiviert werden. Die einzige Anforderung besteht darin, die MFA für jeden Benutzer, einschließlich Dienstkonten, im Partnermandanten zu aktivieren.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kann der bedingte Zugriff zur Erfüllung der MFA-Anforderung verwendet werden?

Ja, du kannst den bedingten Zugriff verwenden, um die MFA für jeden Benutzer, einschließlich Dienstkonten, im Partnermandanten zu aktivieren. Angesichts der umfassenden Privilegien, die mit dem Partnerstatus verbunden sind, müssen wir jedoch sicherstellen, dass jeder Benutzer für jede einzelne Authentifizierung ein MFA-Captcha eingibt. Das bedeutet, dass der bedingte Zugriff nicht verwendet werden kann, um die MFA-Anforderung zu umgehen.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Welche Verifizierungsoptionen werden durch die Implementierung der Basisschutzrichtlinien bereitgestellt?

In Bezug auf die Version der MFA, die durch die Implementierung der Basisschutzrichtlinien zur Verfügung gestellt wird, ist eine Authentifikator-App die einzige Verifizierungsoption. Die Authentifizierung per Telefonanruf oder SMS gilt als weniger sicher. Daher sind diese Optionen mit dieser MFA-Version nicht verfügbar.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Wirken sich die Sicherheitsanforderungen für Partner auf das von Azure AD Connect verwendete Dienstkonto aus?

Nein. Die Sicherheitsanforderungen für Partner haben keine Auswirkungen auf das von Azure AD Connect verwendete Dienstkonto. Wenn bei Azure AD Connect aufgrund der Erzwingung der MFA ein Problem aufgrund, sende eine technische Supportanfrage an den Microsoft-Support.

## <a name="secure-application-model"></a>Sicheres Anwendungsmodell

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Wer sollte das sichere Anwendungsmodell übernehmen, um die Anforderungen zu erfüllen?

Microsoft führt ein sicheres, skalierbares Framework für die Authentifizierung von CSP-Partnern und Control Panel-Anbietern ein, das auf der Multi-Factor Authentication basiert. Weitere Informationen finden Sie im [Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Alle Partner, die eine benutzerdefinierte Integration über APIs (z. B. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) entwickelt oder mithilfe von PowerShell eine benutzerdefinierte Automatisierung implementiert haben, müssen das [Framework „Sicheres Anwendungsmodell“](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) übernehmen, um die Integration in Microsoft-Clouddienste zu ermöglichen.

### <a name="what-is-the-secure-application-model"></a>Was ist das sichere Anwendungsmodell?

Microsoft führt ein sicheres, skalierbares Framework für die Authentifizierung von CSP-Partnern und Control Panel-Anbietern ein, das auf der Multi-Factor Authentication basiert. Weitere Informationen finden Sie im [Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>Wie implementiere ich das sichere Anwendungsmodell?

Alle Partner, die eine benutzerdefinierte Integration über APIs (z. B. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) entwickelt oder mithilfe von PowerShell eine benutzerdefinierte Automatisierung implementiert haben, müssen das [Framework „Sicheres Anwendungsmodell“](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) übernehmen, um die Integration in Microsoft-Clouddienste zu ermöglichen. Eine Nichteinhaltung dieser Anforderung kann zu einer Unterbrechung aufgrund der MFA-Bereitstellung führen. Die folgenden Ressourcen bieten weitere Informationen sowie einen Leitfaden zur Übernahme des Modells.

- [Übersicht über das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokumentation zur Authentifizierung in Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Dokumentation zur Multi-Factor Authentication (MFA) in Partner Center über PowerShell](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Wenn du eine Control Panel-Anwendung verwendest, musst du dich bezüglich der Übernahme des Frameworks „Sicheres Anwendungsmodell“ an den Hersteller wenden.

Control Panel-Anbieter müssen das [Onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) in Partner Center als Control Panel-Anbieter durchführen und sofort mit der Umsetzung dieser Anforderung beginnen. Weitere Informationen findest du unter [Partner Center: Framework „Sicheres Anwendungsmodell“](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Control Panel-Anbieter müssen anstelle von Anmeldeinformationen die Zustimmung von CSP-Partnern akzeptieren und verwalten und alle vorhandenen Anmeldeinformationen von CSP-Partnern löschen.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Wer ist ein Control Panel-Anbieter?

Ein Control Panel-Anbieter ist ein unabhängiger Softwarehersteller, der Apps entwickelt, die von CSP-Partner zur Integration in Partner Center-APIs verwendet werden. Ein Control Panel-Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder die Partner Center-APIs. Eine detaillierte Beschreibung findest du unter [Partner Center: Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Muss das sichere Anwendungsmodell nur für die Partner Center-API bzw. das Partner Center SDK implementiert werden?

Sobald die Basisrichtlinien *MFA für Administratoren erforderlich* und *Endbenutzerschutz* aktiviert sind, muss sich jeder Benutzer per Multi-Factor Authentication authentifizieren. Das bedeutet, dass du das sichere Anwendungsmodell für jedes API-, Befehlszeilenschnittstellen- und PowerShell-Modul (z. B. Azure, Azure AD, MS Online, Partner Center usw.) implementieren musst, das nicht interaktiv ausgeführt werden soll und Benutzeranmeldeinformationen zur Authentifizierung verwendet.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Ich verwende Automatisierungstools wie z. B. PowerShell. Wie implementiere ich das sichere Anwendungsmodell?

Wenn deine Automatisierung nicht interaktiv ausgeführt werden soll und Benutzeranmeldeinformationen zur Authentifizierung verwendet, musst du das sichere Anwendungsmodell implementieren. Informationen zur Implementierung dieses Frameworks findest du unter [Sicheres Anwendungsmodell | Partner Center PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5).  Hinweis: Nicht alle Automatisierungstools bieten die Möglichkeit zur Authentifizierung mit Zugriffstoken. Wenn du genauere Informationen dazu benötigst, welche Änderungen erforderlich sind, sende eine Nachricht an die [Partner Center Security Guidance Group](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Welche Benutzeranmeldeinformationen sollte der Anwendungsadministrator beim Durchführen des Zustimmungsprozesses bereitstellen?

Es wird empfohlen, ein Dienstkonto zu verwenden, dem die geringstmöglichen Berechtigungen zugewiesen wurden. In Bezug auf die Partner Center-API bedeutet dies, dass du ein Konto verwenden solltest, dem die Rolle „Sales Agent“ oder „Admin Agents“ zugewiesen wurde.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Warum sollte der Anwendungsadministrator beim Durchführen des Zustimmungsprozesses keine Anmeldeinformationen eines globalen Administrators bereitstellen?

Um das Risiko so niedrig wie möglich zu halten, sollte ein Konto mit möglichst wenigen Berechtigungen verwendet werden. Es wird davon abgeraten, ein Konto mit globalen Administratorrechten zu verwenden, da dieses über weit mehr Berechtigungen verfügt, als für diesen Vorgang erforderlich sind.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Ich bin CSP-Partner. Woher weiß ich, ob mein Control Panel-Anbieter an der Implementierung der Lösung arbeitet oder nicht?

Partner, die eine Lösung eines Control Panel-Anbieters (Control Panel Vendor, CPV) für Transaktionen im CSP-Programm verwenden, müssen dies mit dem Control Panel-Anbieter selbst klären.

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Ich bin Control Panel-Anbieter. Wie registriere ich mich?

Informationen zum Registrieren als Control Panel-Anbieter (Control Panel Vendor, CPV) findest du in den [hier](https://docs.microsoft.com/partner-center/enroll-as-cpv) beschriebenen Richtlinien.

Um den Registrierungslink zu erhalten, müssen CPVs [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) kontaktieren und einen Microsoft-Mitarbeiter als Sponsor angeben, der eine geschäftliche Beziehung mit dem CPV unterhält oder dessen Geschäft kennt. Beispiel: ein Partner Development Manager (PDM).

Nachdem du dich bei Partner Center angemeldet und deine Anwendungen registriert hast, kannst du auf Partner Center-APIs zugreifen. Neue CPVs erhalten die Informationen zu ihrer Sandbox über eine Partner Center-Benachrichtigung. Nach der Registrierung als Control Panel-Anbieter für Microsoft und Zustimmung zur CPV-Vereinbarung stehen dir folgende Möglichkeiten zur Verfügung:

1. Verwalten von Mehrinstanzenanwendungen (Anwendungen im Azure-Portal hinzufügen, Anwendungen in Partner Center registrieren und deren Registrierung aufheben). Hinweis: CPVs müssen ihre Anwendungen in Partner Center registrieren, um die Autorisierung für Partner Center-APIs zu erhalten. Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.
2. Anzeigen und Verwalten deines CPV-Profils.
3. Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen. Die einzige Rolle, die ein CPV einnehmen kann, ist der globale Administrator.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Ich verwende das Partner Center SDK. Übernimmt das SDK automatisch das sichere Anwendungsmodell?

Nein. Du musst die Richtlinien im [Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) befolgen.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>Kann ich ein Aktualisierungstoken für das sichere Anwendungsmodell mit Konten generieren, die nicht für die MFA aktiviert sind?

Ja, ein Aktualisierungstoken kann mit einem Konto generiert werden, für das die MFA nicht erzwungen wird. Dies wird jedoch nicht empfohlen, weil ein Token, das mit einem nicht für die MFA aktivierten Konto generiert wurde, nicht auf Ressourcen zugreifen kann, denn dafür ist die MFA erforderlich.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Wie kann meine Anwendung ein Zugriffstoken abrufen, wenn ich die MFA aktiviere?

Im [Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) findest du detaillierte Informationen dazu, wie du dies einrichten kannst und gleichzeitig die neuen Sicherheitsanforderungen erfüllst. Beispielcode für .NET findest du [hier](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model), Java-Beispielcode [hier](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Erstelle ich als CPV eine Azure AD-Anwendung in meinem eigenen CPV-Mandanten oder im Mandanten des CSP-Partners?

Der CPV muss die Azure Active Directory-Anwendung in dem Mandanten erstellen, der mit seiner Registrierung als CPV verknüpft ist.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Ich bin Cloud Solution Provider und verwende eine reine App-Authentifizierung. Muss ich Änderungen vornehmen?

Die reine App-Authentifizierung ist nicht betroffen, weil keine Benutzeranmeldeinformationen verwendet werden, um ein Zugriffstoken anzufordern. Wenn Benutzeranmeldeinformationen freigegeben werden, müssen Control Panel-Anbieter das [Framework „Sicheres Anwendungsmodell“](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) übernehmen und alle vorhandenen Partneranmeldeinformationen löschen.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Kann ich als CPV die reine App-Authentifizierung verwenden, um Zugriffstoken zu erhalten?

Nein. Control Panel-Anbieter können nicht die reine App-Authentifizierung nutzen, um Zugriffstoken im Namen eines Partners anzufordern. Sie müssen das sichere Anwendungsmodell implementieren, bei dem alle Apps und Benutzer authentifiziert werden müssen.

## <a name="enforcement"></a>Erzwingen

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Ich verwende eine MFA-Lösung eines Drittanbieters und werde blockiert. Was soll ich tun?

Um zu überprüfen, ob das Konto, das den Zugriff auf die Ressourcen versucht hat, mit mehrstufiger Authentifizierung herausgefordert wurde, überprüfen wir den Anspruch [Verweis auf die Authentifizierungsmethode](https://tools.ietf.org/html/rfc8176), um festzustellen, ob MFA aufgelistet ist. Einige Drittanbieterlösungen geben diesen Anspruch nicht aus oder schließen den MFA-Wert nicht ein. Wenn der Anspruch fehlt oder der MFA-Wert nicht aufgelistet ist, gibt es keine Möglichkeit, herauszufinden, ob das authentifizierte Konto mit mehrstufiger Authentifizierung herausgefordert wurde. Sie müssen mit dem Anbieter Ihrer Drittanbieterlösung zusammenarbeiten, um zu bestimmen, welche Maßnahmen ergriffen werden müssen, damit die Lösung den Verweis auf die Authentifizierungsmethode-Anspruch ausgibt.

Wenn Sie nicht sicher sind, ob Ihre Drittanbieterlösung den erwarteten Anspruch ausgibt oder nicht, lesen Sie [Testing the Partner Security Requirements](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0) (Testen der Partneranforderungen an die Sicherheit).

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA blockiert meinen Support meines Kunden über AOBO. Wie kann ich vorgehen?

Bei der technischen Durchsetzung der Sicherheitsanforderungen für Partner wird überprüft, ob das authentifizierte Konto eine Herausforderung für mehrstufige Authentifizierung erhalten hat. Wenn keine Herausforderung erfolgt ist, werden Sie auf die Anmeldeseite umgeleitet und zur erneuten Authentifizierung aufgefordert. Wenn Ihre Domäne keine Verbunddomäne ist, werden Sie nach erfolgreicher Authentifizierung aufgefordert, die mehrstufige Authentifizierung einzurichten. Nach dem Abschluss dieses Vorgangs können Sie Ihre Kunden mithilfe von AOBO verwalten. Wenn Ihre Domäne eine Verbunddomäne ist, müssen Sie sicherstellen, dass das Konto eine Herausforderung zur mehrstufigen Authentifizierung empfängt.

## <a name="key-resources"></a>Wichtige Ressourcen

### <a name="how-to-get-started"></a>Erste Schritte

- [Sicherheitsanforderungen für Partner: Schrittanleitung](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Sende Fragen und Feedback an die [Partner Center Security Guidance Group](https://aka.ms/MPCSecurityGuidance).
- Nimm an Informationsveranstaltungen und Webinaren für Partner teil. [Hier findest du genaue Informationen und Ressourcen](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Ressourcen für die Aktivierung der MFA

- Grundlegendes zum Konzept der [Basisschutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Unter [Basisrichtlinie: MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) findest du Informationen dazu, wie du diese Basisrichtlinie aktivierst.
- Unter [Basisrichtlinie: Endbenutzerschutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) findest du Informationen dazu, wie du diese Basisrichtlinie aktivierst.

### <a name="resources-for-adopting-secure-application-model"></a>Ressourcen für die Übernahme des sicheren Anwendungsmodells

- [Übersicht über das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: Leitfaden für das sichere Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokumentation zur Authentifizierung in Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Dokumentation zur Multi-Factor Authentication (MFA) in Partner Center über PowerShell](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Support

### <a name="where-can-i-get-support"></a>Wo erhalte ich Support?

Unterstützende Ressourcen für die Erfüllung der Sicherheitsanforderungen findest du hier: Wenn du über Advanced Support for Partners (ASfP) verfügst, wende dich an deinen Service Account Manager. Wenn du über eine Premier Support for Partners-Vereinbarung (PSfP) verfügst, wende dich an den Service Account Manager und den Technical Account Manager.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Wie erhalte ich Hilfe beim Aktivieren der Basisrichtlinien?

- Partner können Beratungsstunden (in den MPN-Vorteilen) nutzen, um detaillierte Unterstützung bei der Implementierung der Sicherheitsanforderungen zu erhalten.
- Optionen für den technischen Produktsupport für Azure Active Directory sind über MPN-Vorteile verfügbar. Partner mit Zugriff auf aktive ASfP- oder PSfP-Vereinbarungen können sich an den entsprechenden Account Manager (SAM bzw. TAM) wenden, um die verfügbaren Optionen zu verstehen.
- Unterstützung bei der Implementierung von Basisrichtlinien über Partner Center erhältst du per [Serviceanforderung im Partner Center](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Wähle *MFA und sicheres Anwendungsmodell* als Thema aus.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Wie erhalte ich technische Informationen und Unterstützung bei der Übernahme des Frameworks „Sicheres Anwendungsmodell“?

Optionen für den technischen Produktsupport für Azure Active Directory sind über MPN-Vorteile verfügbar. Partner mit Zugriff auf ein aktives ASfP- oder PSfP-Abonnement können sich an den entsprechenden Account Manager (SAM bzw. TAM) wenden, um die verfügbaren Optionen zu verstehen.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Wie kann ich mich an den Support wenden, wenn ich den Zugriff auf Partner Center verloren habe?

Navigiere zu [Microsoft Partner-Support](https://partner.microsoft.com/support), und wähle dann **Alle Supportoptionen anzeigen** aus. Die verfügbaren Optionen zum Kontaktieren des Microsoft Partner-Supports werden angezeigt. Hierzu gehören eine Telefonnummer zum Anrufen des Supports und eine Option zum Chatten mit dem Support. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Wo finde ich Informationen zu häufigen technischen Problemen?

Informationen zu häufigen technischen Problemen sind [hier](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues) zu finden.
