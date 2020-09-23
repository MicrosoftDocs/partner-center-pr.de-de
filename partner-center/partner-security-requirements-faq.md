---
title: Sicherheitsanforderungen für Partner – häufig gestellte Fragen
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Häufig gestellte Fragen zu den Sicherheitsanforderungen für Partner – was sie beinhalten, wie sie von Partnern umgesetzt werden sollten und woher Sie wissen, ob Sie sie erfüllen.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5695a5478f1fdb9d16c395bb3ea87240fc2cf6f3
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999804"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Häufig gestellte Fragen zu den Sicherheitsanforderungen für Partner

**Geeignete Benutzer**

- Alle aktivierten Benutzer einschließlich Gastbenutzer

Dieser Artikel enthält einige häufig gestellte Fragen zu den [Sicherheitsanforderungen für Partner](partner-security-requirements.md) sowie die entsprechenden Antworten.

## <a name="partner-security-requirements"></a>Sicherheitsanforderungen für Partner

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>Was sind die Sicherheitsanforderungen für Partner, und warum sollten Partner sie implementieren?

Stärkere und laufende Sicherheits- und Datenschutzmaßnahmen gehören zu unseren wichtigsten Prioritäten, und wir unterstützen Partner weiterhin dabei, ihre Kunden und Mandanten zu schützen. Wir stellen immer mehr und immer ausgefeiltere Sicherheitsangriffe fest – insbesondere im Hinblick auf die Kompromittierung von Identitäten. Da vorbeugende Maßnahmen eine Schlüsselrolle bei der Gesamtverteidigungsstrategie spielen, um Sicherheitsangriffe abzuwehren, haben wir in 2019 [obligatorische Sicherheitsanforderungen](partner-security-requirements.md) eingeführt. Alle Partner, die am Cloud Solution Provider-Programm (CSP) teilnehmen, Control Panel Vendors und Berater sollten die Anforderungen implementieren, um konform zu bleiben.

### <a name="what-are-the-key-timelines-and-milestones"></a>Welches sind die wichtigsten Zeitpläne und Meilensteine?

Die mit den Sicherheitsanforderungen verbundenen Bestimmungen wurden der Microsoft Partner-Vereinbarung in 2019 hinzugefügt. Sie müssen diese Sicherheitsanforderungen baldmöglichst implementieren, um die Voraussetzungen für Ihre Teilnahme am CSP-Programm zu erfüllen.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Was geschieht, wenn ich diese Sicherheitsanforderungen für Partner nicht implementiere?

Die Microsoft Partner-Vereinbarung setzt voraus, dass Sie die mehrstufige Authentifizierung für Benutzerkonten erzwingen und das sichere Anwendungsmodell für die Interaktion mit der Partner Center-API übernehmen. 

Partner, die diese Sicherheitsverfahren nicht einhalten, können dann möglicherweise keine Transaktionen im CSP-Programm mehr ausführen oder Kundenmandanten mit delegierten Administratorrechten verwalten.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Gelten die Sicherheitsanforderungen für alle geografischen Regionen?

Ja, die Sicherheitsanforderungen gelten für alle geografischen Regionen. Es wird dringend empfohlen, dass alle Partner, die über eine unabhängige Cloud (21Vianet, US-Regierung und Deutschland) handeln, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner müssen jedoch nicht die neuen Sicherheitsanforderungen zum 1. August erfüllen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Sind Ausnahmen für ein Konto möglich?

Nein, kein Benutzerkonto kann davon ausgenommen werden, ein MFA-Verfahren durchzusetzen. Angesichts der umfassenden Privilegien, die mit dem Partnerstatus verbunden sind, muss die mehrstufige Authentifizierung gemäß der Microsoft Partner-Vereinbarung für jedes Benutzerkonto im Partnermandanten erzwungen werden.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Woher weiß ich, ob ich die Sicherheitsanforderungen für Partner erfüllt habe?

Führen Sie die folgenden Schritte aus.

- Sie müssen alle Anforderungen erfüllen, die in den [Sicherheitsanforderungen für Partner](partner-security-requirements.md) beschrieben werden.
- Sie müssen sicherstellen, dass für alle Benutzerkonten in Ihrem Partnermandanten die mehrstufige Authentifizierung erzwungen wird.

Um die wichtigsten Bereiche zu identifizieren, in denen Sie Maßnahmen ergreifen können, nutzen Sie den Bericht [Status der Sicherheitsanforderungen](https://partner.microsoft.com/commerce/security/compliance), der über das Partner Center verfügbar ist.

Weitere Informationen zum Statusbericht finden Sie unter [Status der Sicherheitsanforderungen für Partner](partner-security-compliance.md).

## <a name="required-actions"></a>Erforderliche Aktionen

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Welches sind die wichtigsten Aktionen, die ich ausführen muss, um die Anforderungen zu erfüllen?

Alle Partner im CSP-Programm (Partner mit direkter Abrechnung, indirekte Anbieter und indirekte Handelspartner), Berater und Control Panel-Anbieter müssen die Anforderungen erfüllen.

1. **Durchsetzen der MFA für alle Benutzer**

    Alle Partner im CSP-Programm, Berater und Control Panel-Anbieter müssen die MFA für alle Benutzer in ihrem Partnermandanten erzwingen.

    Weitere Überlegungen:

    - Indirekte Anbieter müssen für das Onboarding in Partner Center mit indirekten Handelspartnern zusammenarbeiten, sofern dies nicht bereits erfolgt ist, und ihre Handelspartner dazu anhalten, die Anforderungen zu erfüllen.
    - Azure MFA wird allen Benutzern im Partnermandanten über Azure AD-Sicherheitsstandards kostenlos zur Verfügung gestellt. Dabei wird nur die Überprüfungsmethode einer Authenticator-Anwendung verwendet, die zeitbasierte Einmalkennwörter (Time Based One Time, TOTP) unterstützt.
    - Weitere Verifizierungsmethoden sind über die [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium)-SKUs verfügbar, wenn andere Methoden wie ein Telefonanruf oder eine SMS erforderlich sind.
    - Beim Zugriff auf kommerzielle Clouddienste von Microsoft können Partner für jedes Konto auch die MFA-Lösung eines Drittanbieters nutzen.

2. **Übernehmen des Frameworks „Sicheres Anwendungsmodell“**

    Alle Partner, die eine benutzerdefinierte Integration über APIs (z. B. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) entwickelt oder mithilfe von PowerShell eine benutzerdefinierte Automatisierung implementiert haben, müssen das [Framework „Sicheres Anwendungsmodell“](/partner-center/develop/enable-secure-app-model) übernehmen, um die Integration in Microsoft-Clouddienste zu ermöglichen. Eine Nichteinhaltung dieser Anforderung kann zu einer Unterbrechung aufgrund der MFA-Bereitstellung führen. Die folgenden Ressourcen bieten weitere Informationen sowie einen Leitfaden zur Übernahme des Modells.

    - [Übersicht über das sichere Anwendungsmodell](/partner-center/develop/enable-secure-app-model)
    - [Partner Center: Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Dokumentation zur Authentifizierung in Partner Center](/partner-center/develop/partner-center-authentication)
    - [Dokumentation zur Multi-Factor Authentication (MFA) in Partner Center über PowerShell](/powershell/partnercenter/multi-factor-auth)

    Wenn Sie einen Control Panel verwenden, wenden Sie sich im Hinblick auf die Übernahme des Frameworks „Sicheres Anwendungsmodell“ an den Hersteller.

    Control Panel-Anbieter müssen das [Onboarding](enroll-as-cpv.md) in Partner Center als Control Panel-Anbieter durchführen und sofort mit der Umsetzung dieser Anforderung beginnen. Weitere Informationen findest du unter [Partner Center: Framework „Sicheres Anwendungsmodell“](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Control Panel-Anbieter müssen anstelle von Anmeldeinformationen die Zustimmung von CSP-Partnern akzeptieren und verwalten und alle vorhandenen Anmeldeinformationen von CSP-Partnern löschen.

## <a name="multi-factor-authentication"></a>Mehrstufige Authentifizierung

### <a name="what-is-multi-factor-authentication-mfa"></a>Was ist die Multi-Factor Authentication (MFA)?

Die MFA ist ein Sicherheitsmechanismus, mit dem Einzelpersonen über mehr als ein erforderliches Sicherheits- und Validierungsverfahren authentifiziert werden. Dabei sind mindestens zwei der folgenden Authentifizierungsmethoden erforderlich:

- Etwas, das Sie wissen (in der Regel ein Kennwort)
- Etwas, das Sie besitzen (ein vertrauenswürdiges Gerät, das sich nicht leicht duplizieren lässt, z. B. ein Telefon)
- Etwas, das Sie sind (Biometrie)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Was kostet die Aktivierung der MFA?

Microsoft stellt MFA kostenlos durch die Implementierung von Azure AD Sicherheitsstandards bereit. Die einzige Überprüfungsoption, die bei dieser Version der MFA zur Verfügung steht, ist eine Authenticator-App. Wenn eine Verifizierung per Telefonanruf oder SMS erforderlich ist, muss eine Lizenz für [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) erworben werden. Alternativ können Sie eine Drittanbieterlösung verwenden, um MFA für jeden Benutzer in Ihrem Partnermandanten bereitzustellen. In diesem Fall müssen Sie selbst sicherstellen, dass Ihre MFA-Lösung erzwungen wird und die Anforderungen erfüllt werden.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Welche Maßnahmen muss ich ergreifen, wenn ich bereits über eine MFA-Lösung verfüge?

Aufgrund dieser Sicherheitsanforderungen müssen Benutzer in einem Partnermandanten sich beim Zugriff auf kommerzielle Microsoft-Clouddienste mit MFA-Verfahren anmelden. Zur Erfüllung dieser Anforderungen können Drittanbieterlösungen verwendet werden. Microsoft stellt unabhängigen Identitätsanbietern keine Validierungstests mehr bereit, um die Kompatibilität mit Azure Active Directory zu überprüfen. Wenn Sie Ihr Produkt auf Interoperabilität testen möchten, lesen Sie diese [Richtlinien](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Wenn Sie eine Drittanbieterlösung verwenden, muss unbedingt überprüft werden, ob sie den AMR-Anspruch (Authentication Method Reference) mit dem MFA-Wert ausgibt. Ausführliche Informationen zur Überprüfung, ob Ihre Drittanbieterlösung den erwarteten Anspruch ausgibt, finden Sie unter [Testing the Partner Security Requirements](/powershell/partnercenter/test-partner-security-requirements) (Testen der Partneranforderungen an die Sicherheit).

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Ich führe Transaktionen mit mehreren Partnermandanten aus. Muss ich die MFA für alle Mandanten implementieren?

Ja, Sie müssen die MFA für jeden Azure Active Directory-Mandanten erzwingen, der dem CSP-Programm oder dem Beraterprogramm zugeordnet ist. Wenn Sie eine Lizenz für Azure Active Directory Premium erwerben möchten, müssen Sie auch für den Benutzer in jedem Azure Active Directory-Mandanten eine Lizenz erwerben.

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Muss MFA für jedes Benutzerkonto in meinem Partnermandanten erzwungen werden?

Ja, jeder Benutzer muss MFA erzwingen. Wenn Sie aber Azure AD-Sicherheitsstandards verwenden, ist keine zusätzliche Maßnahme erforderlich, weil MFA durch dieses Feature für alle Benutzerkonten erzwungen wird. Das Aktivieren von Sicherheitsstandards ist eine kostenlose und einfache Möglichkeit, um sicherzustellen, dass Ihre Benutzerkonten MFA-konform sind und durch die Erzwingung von MFA nicht beeinträchtigt werden.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Ich bin Microsoft-Partner mit direkter Abrechnung. Wie muss ich vorgehen?

Cloud Solution Provider-Partner mit direkter Abrechnung müssen die MFA für jeden Benutzer in ihrem Partnermandanten erzwingen.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Ich bin indirekter Handelspartner und führe Transaktionen nur über einen Distributor durch. Muss ich trotzdem MFA aktivieren?

Alle indirekten Handelspartner müssen die MFA für jeden Benutzer in ihrem Partnermandanten erzwingen. Der indirekte Wiederverkäufer muss MFA aktivieren.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Ich verwende die Partner Center-API nicht. Muss ich die MFA dennoch implementieren?

Ja. Diese Sicherheitsanforderung gilt für alle Benutzer – einschließlich Administratorbenutzern von Partnern und Endbenutzern in einem Partnermandanten.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Welche Drittanbieter stellen MFA-Lösungen bereit, die mit Azure Active Directory kompatibel sind?

Bei der Überprüfung von MFA-Anbietern und -Lösungen müssen Partner sicherstellen, dass die ausgewählte Lösung mit Azure Active Directory kompatibel ist.

Microsoft stellt unabhängigen Identitätsanbietern keine Validierungstests mehr bereit, um die Kompatibilität mit Azure Active Directory zu überprüfen. Wenn Sie Ihr Produkt auf Interoperabilität testen möchten, lesen Sie diese [Richtlinien](https://www.microsoft.com/download/details.aspx?id=56843).

Weitere Informationen Sie in [Azure AD-Verbund – Kompatibilitätsliste](/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Wie kann ich die MFA in unserer Sandbox für die Integration testen?

Das Feature für die Azure AD-Sicherheitsstandards sollte aktiviert sein. Alternativ kannst du auch Drittanbieterlösungen verwenden, die den Verbund nutzen.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Wirkt sich die Aktivierung der MFA darauf aus, wie ich mit meinem Kundenmandanten interagiere?

Nein Die Erfüllung dieser Sicherheitsanforderungen wirkt sich nicht auf die Verwaltung der Kunden aus. Die Möglichkeit, delegierte administrative Vorgänge auszuführen, wird nicht beeinträchtigt.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Unterliegen meine Kunden den Sicherheitsanforderungen für Partner?

Nein. Die MFA muss nicht für jeden Benutzer in den Azure AD-Mandanten deiner Kunden erzwungen werden. Es empfiehlt sich allerdings, in Zusammenarbeit mit jedem Kunden zu ermitteln, wie die Benutzer der Kunden am besten geschützt werden können.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kann ein Benutzer von der MFA-Anforderung ausgenommen werden?

Nein. Jeder Benutzer im Partnermandanten, einschließlich aller Dienstkonten, muss sich per MFA authentifizieren.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Gelten die Sicherheitsanforderungen für Partner auch für die Sandbox zur Integration?

Ja. Die Sicherheitsanforderungen für Partner gelten auch für die Sandbox zur Integration. Dies bedeutet, dass du für die Benutzer im Sandbox-Mandanten für die Integration die geeignete MFA-Lösung implementieren musst. Es wird empfohlen, dass du die Azure AD-Sicherheitsstandards implementierst, um MFA bereitzustellen.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Wie konfiguriere ich ein Konto für den Notfallzugriff?

Es hat sich bewährt, ein oder zwei Konten für den Notfallzugriff einzurichten, um eine versehentliche Aussperrung aus dem Azure AD-Mandanten zu verhindern. Aufgrund der Sicherheitsanforderungen für Partner muss sich jeder Benutzer per MFA authentifizieren. Diese Anforderung bedeutet, dass Sie die Definition eines Kontos für den Notfallzugriff ändern müssen. Du könntest z. B. ein Konto verwenden, das eine Drittanbieterlösung für die MFA nutzt.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Ist der Active Directory-Verbunddienst (Active Directory Federation Service, ADFS) erforderlich, wenn ich eine Drittanbieterlösung verwende?

Nein, bei Verwendung einer Drittanbieterlösung ist der Active Directory-Verbunddienst (ADFS) nicht erforderlich. Es empfiehlt sich, zusammen mit dem Lösungsanbieter zu ermitteln, welche Anforderungen für die Lösung bestehen.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Ist es erforderlich, Azure AD Sicherheitsstandards zu aktivieren?

Nein, Azure AD-Sicherheitsstandards müssen nicht zwingend aktiviert werden.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kann der bedingte Zugriff zur Erfüllung der MFA-Anforderung verwendet werden?

Ja, du kannst den bedingten Zugriff verwenden, um die MFA für jeden Benutzer, einschließlich Dienstkonten, im Partnermandanten zu aktivieren. Angesichts der umfassenden Privilegien, die mit dem Partnerstatus verbunden sind, müssen wir jedoch sicherstellen, dass jeder Benutzer für jede einzelne Authentifizierung ein MFA-Captcha eingibt. Dies bedeutet, dass der bedingte Zugriff nicht verwendet werden kann, um die MFA-Anforderung zu umgehen.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Wirken sich die Sicherheitsanforderungen für Partner auf das von Azure AD Connect verwendete Dienstkonto aus?

Nein. Die Sicherheitsanforderungen für Partner haben keine Auswirkungen auf das von Azure AD Connect verwendete Dienstkonto. Wenn bei Azure AD Connect aufgrund der Erzwingung der MFA ein Problem aufgrund, sende eine technische Supportanfrage an den Microsoft-Support.

## <a name="secure-application-model"></a>Sicheres Anwendungsmodell

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Wer sollte das sichere Anwendungsmodell übernehmen, um die Anforderungen zu erfüllen?

Microsoft führt ein sicheres, skalierbares Framework für die Authentifizierung von CSP-Partnern und Control Panel-Anbietern ein, das auf der Multi-Factor Authentication basiert. Weitere Informationen finden Sie im [Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Alle Partner, die eine benutzerdefinierte Integration über APIs (z. B. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) entwickelt oder mithilfe von PowerShell eine benutzerdefinierte Automatisierung implementiert haben, müssen das [Framework „Sicheres Anwendungsmodell“](/partner-center/develop/enable-secure-app-model) übernehmen, um die Integration in Microsoft-Clouddienste zu ermöglichen.

### <a name="what-is-the-secure-application-model"></a>Was ist das sichere Anwendungsmodell?

Microsoft führt ein sicheres, skalierbares Framework für die Authentifizierung von CSP-Partnern und Control Panel-Anbietern ein, das auf der Multi-Factor Authentication basiert. Weitere Informationen finden Sie im [Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>Wie implementiere ich das sichere Anwendungsmodell?

Alle Partner, die eine benutzerdefinierte Integration über APIs (z. B. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) entwickelt oder mithilfe von PowerShell eine benutzerdefinierte Automatisierung implementiert haben, müssen das [Framework „Sicheres Anwendungsmodell“](/partner-center/develop/enable-secure-app-model) übernehmen, um die Integration in Microsoft-Clouddienste zu ermöglichen. Eine Nichteinhaltung dieser Anforderung kann zu einer Unterbrechung aufgrund der MFA-Bereitstellung führen. Die folgenden Ressourcen bieten weitere Informationen sowie einen Leitfaden zur Übernahme des Modells.

- [Übersicht über das sichere Anwendungsmodell](/partner-center/develop/enable-secure-app-model)
- [Partner Center: Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokumentation zur Authentifizierung in Partner Center](/partner-center/develop/partner-center-authentication)
- [Dokumentation zur Multi-Factor Authentication (MFA) in Partner Center über PowerShell](/powershell/partnercenter/multi-factor-auth)

Wenn Sie einen Control Panel verwenden, müssen Sie sich im Hinblick auf die Übernahme des Frameworks „Sicheres Anwendungsmodell“ an den Hersteller wenden.

Control Panel-Anbieter müssen das [Onboarding](enroll-as-cpv.md) in Partner Center als Control Panel-Anbieter durchführen und sofort mit der Umsetzung dieser Anforderung beginnen. Weitere Informationen findest du unter [Partner Center: Framework „Sicheres Anwendungsmodell“](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Control Panel-Anbieter müssen anstelle von Anmeldeinformationen die Zustimmung von CSP-Partnern akzeptieren und verwalten und alle vorhandenen Anmeldeinformationen von CSP-Partnern löschen.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Muss das sichere Anwendungsmodell nur für die Partner Center-API bzw. das Partner Center SDK implementiert werden?

Das Erzwingen der mehrstufigen Authentifizierung für alle Benutzerkonten wirkt sich auf jede Automatisierung oder Integration aus, die für die nicht interaktive Ausführung vorgesehen ist. Gemäß den Partnersicherheitsanforderungen muss das sichere Anwendungsmodell für die Partner Center API aktiviert werden. Das Modell kann aber auch genutzt werden, um eine Zwei-Faktor-Authentifizierung mit Automatisierung und Integration einzurichten.

>[!Note] 
>Ressourcen, auf die zugegriffen wird, müssen die zugriffstokenbasierte Authentifizierung unterstützen.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Ich verwende Automatisierungstools wie z. B. PowerShell. Wie implementiere ich das sichere Anwendungsmodell?

Wenn deine Automatisierung nicht interaktiv ausgeführt werden soll und sie Benutzeranmeldeinformationen zur Authentifizierung verwendet, musst du das sichere Anwendungsmodell implementieren. Informationen zur Implementierung dieses Frameworks findest du unter [Sicheres Anwendungsmodell | Partner Center PowerShell](/powershell/partnercenter/multi-factor-auth).  

>[!Note] 
>Nicht alle Automatisierungstools ermöglichen die Authentifizierung mit Zugriffstoken. Wenn du genauere Informationen dazu benötigst, welche Änderungen erforderlich sind, sende eine Nachricht an die Gruppe [Partner Center Security Guidance](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance). 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Welche Benutzeranmeldeinformationen sollte der Anwendungsadministrator beim Durchführen des Zustimmungsprozesses bereitstellen?

Es wird empfohlen, ein Dienstkonto zu verwenden, dem die geringstmöglichen Berechtigungen zugewiesen wurden. Hinsichtlich der Partner Center-API sollten Sie ein Konto verwenden, dem die Rolle „Sales Agent“ oder „Admin Agents“ zugewiesen wurde.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Warum sollte der Anwendungsadministrator beim Durchführen des Zustimmungsprozesses keine Anmeldeinformationen eines globalen Administrators bereitstellen?

Um das Risiko so gering wie möglich zu halten, empfiehlt sich die Verwendung eines Kontos mit möglichst wenigen Berechtigungen. Es wird davon abgeraten, ein Konto mit globalen Administratorrechten zu verwenden, weil dadurch mehr Berechtigungen bereitgestellt würden, als für diesen Vorgang erforderlich sind.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Ich bin CSP-Partner. Woher weiß ich, ob mein Control Panel-Anbieter an der Implementierung der Lösung arbeitet oder nicht?

Partner, die eine Lösung eines Control Panel-Anbieters (Control Panel Vendor, CPV) für Transaktionen im CSP-Programm verwenden, müssen dies mit dem Control Panel-Anbieter selbst klären.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Wer ist ein Control Panel-Anbieter?

Ein Control Panel-Anbieter ist ein unabhängiger Softwarehersteller, der Apps entwickelt, die von CSP-Partner zur Integration in Partner Center-APIs verwendet werden. Ein Control Panel-Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder die Partner Center-APIs. Eine detaillierte Beschreibung findest du unter [Partner Center: Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Ich bin Control Panel-Anbieter. Wie registriere ich mich?

Informationen zum Registrieren als Control Panel-Anbieter (Control Panel Vendor, CPV) findest du in den [hier](enroll-as-cpv.md) beschriebenen Richtlinien.

Wenn CPVs den Registrierungslink erhalten möchten, müssen sie [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) kontaktieren und einen Microsoft-Mitarbeiter als Sponsor angeben, der eine geschäftliche Beziehung mit dem CPV unterhält oder dessen Geschäft kennt. Beispiel: ein Partner Development Manager (PDM).

Nachdem du dich bei Partner Center angemeldet und deine Anwendungen registriert hast, kannst du auf Partner Center-APIs zugreifen. Neue CPVs erhalten die Informationen zu ihrer Sandbox über eine Partner Center-Benachrichtigung. Nach der Registrierung als Control Panel-Anbieter für Microsoft und Zustimmung zur CPV-Vereinbarung stehen dir folgende Möglichkeiten zur Verfügung:

1. Verwalten von mehrinstanzenfähigen Anwendungen (Anwendungen im Azure-Portal hinzufügen, Anwendungen in Partner Center registrieren und deren Registrierung aufheben).

   >[!Note]
   >CPVs müssen ihre Anwendungen in Partner Center registrieren, um die Autorisierung für Partner Center-APIs zu erhalten. Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.

1. Anzeigen und Verwalten deines CPV-Profils.

1. Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen. Ein CPV kann nur über die Rolle „Globaler Administrator“ verfügen.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Ich verwende das Partner Center SDK. Übernimmt das SDK automatisch das sichere Anwendungsmodell?

Nein, du musst die Richtlinien im [Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) befolgen.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Kann ich ein Aktualisierungstoken für das sichere Anwendungsmodell mit Konten generieren, die nicht für die MFA aktiviert wurden?

Ja, ein Aktualisierungstoken kann mit einem Konto generiert werden, für das die MFA nicht erzwungen wird. Dies sollte jedoch vermieden werden. Jedes Token, das mit einem Konto ohne aktivierte MFA generiert wurde, kann nicht auf Ressourcen zugreifen, das MFA hierfür erforderlich ist.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Wie kann meine Anwendung ein Zugriffstoken abrufen, wenn ich die MFA aktiviere?

Im [Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) findest du detaillierte Informationen dazu, wie du dies einrichten kannst und gleichzeitig die neuen Sicherheitsanforderungen erfüllst. Beispielcode für .NET findest du [hier](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model), Java-Beispielcode [hier](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Erstelle ich als CPV eine Azure AD-Anwendung in meinem eigenen CPV-Mandanten oder im Mandanten des CSP-Partners?

Der CPV muss die Azure Active Directory-Anwendung in dem Mandanten erstellen, der mit seiner Registrierung als CPV verknüpft ist.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Ich bin Cloud Solution Provider und verwende eine reine App-Authentifizierung. Muss ich Änderungen vornehmen?

Die reine App-Authentifizierung ist nicht betroffen, weil zum Anfordern eines Zugriffstokens keine Benutzeranmeldeinformationen verwendet werden. Wenn Benutzeranmeldeinformationen freigegeben werden, müssen Control Panel-Anbieter das [Framework „Sicheres Anwendungsmodell“](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) übernehmen und alle vorhandenen Partneranmeldeinformationen löschen.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Kann ich als CPV die reine App-Authentifizierung verwenden, um Zugriffstoken zu erhalten?

Nein. Control Panel-Anbieter können nicht die reine App-Authentifizierung nutzen, um Zugriffstoken im Namen eines Partners anzufordern. Sie müssen das sichere Anwendungsmodell implementieren, bei dem alle Apps und Benutzer authentifiziert werden müssen.

## <a name="technical-enforcement"></a>Technische Erzwingung

### <a name="what-is-the-activation-of-security-safeguards"></a>Was ist die Aktivierung von Sicherheitsmaßnahmen?

Alle Partner, die am Cloud Solution Provider-Programm (CSP) teilnehmen, Control Panel Vendors (CPVs) und Berater sollten die obligatorischen Sicherheitsanforderungen implementieren, um konform zu bleiben.

Um zusätzlichen Schutz zu bieten, hat Microsoft mit der Aktivierung von Sicherheitsmaßnahmen begonnen, die Partnern dabei helfen, ihre Mandanten und ihre Kunden zu schützen, indem sie die MFA-Überprüfung (Multi-Factor Authentication, mehrstufige Authentifizierung) festlegen, durch die ein nicht autorisierter Zugriff verhindert wird.  

Wir haben die Aktivierung der AOBO-Funktionen (Admin-on-Behalf-Of, Administrator im Auftrag von) für alle Partnermandanten erfolgreich abgeschlossen. Zur weiteren Unterstützung von Partnern und Kunden werden wir (Ziel Q2 CY2020) mit der Aktivierung für Partner Center-Transaktionen in CSP beginnen und so Partnern dabei helfen, ihre Unternehmen und Kunden vor Vorfällen im Zusammenhang mit Identitätsdiebstahl zu schützen.

Weitere Informationen finden Sie unter [Festlegen von Multi-Factor Authentication (MFA) für Ihren Partnermandanten](partner-security-requirements-mandating-mfa.md).

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Ich verwende eine MFA-Lösung eines Drittanbieters und werde blockiert. Was soll ich tun?

Zur Überprüfung, ob das Konto, das den Zugriff auf die Ressourcen versucht hat, mit mehrstufiger Authentifizierung herausgefordert wurde, überprüfen wir den Anspruch [Verweis auf die Authentifizierungsmethode](https://tools.ietf.org/html/rfc8176), um festzustellen, ob MFA aufgelistet ist. Einige Drittanbieterlösungen geben diesen Anspruch nicht aus oder beziehen den MFA-Wert nicht mit ein. Wenn der Anspruch fehlt oder der MFA-Wert nicht aufgelistet ist, gibt es keine Möglichkeit, herauszufinden, ob das authentifizierte Konto mit mehrstufiger Authentifizierung herausgefordert wurde. Sie müssen mit dem Anbieter Ihrer Drittanbieterlösung zusammenarbeiten, um zu bestimmen, welche Maßnahmen ergriffen werden müssen, damit die Lösung den Verweis auf die Authentifizierungsmethode-Anspruch ausgibt.

Wenn Sie nicht genau wissen, ob Ihre Drittanbieterlösung den erwarteten Anspruch ausgibt oder nicht, lesen Sie [Testing the Partner Security Requirements](/powershell/partnercenter/test-partner-security-requirements) (Testen der Partneranforderungen an die Sicherheit).

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA blockiert meinen Support meines Kunden über AOBO. Wie kann ich vorgehen?

Bei der technischen Durchsetzung der Sicherheitsanforderungen für Partner wird überprüft, ob das authentifizierte Konto eine Herausforderung für mehrstufige Authentifizierung erhalten hat. Wenn dies nicht geschehen ist, werden Sie auf die Anmeldeseite umgeleitet und zur erneuten Authentifizierung aufgefordert. Ausführlichere Informationen und Anleitungen finden Sie in dieser Dokumentation zu [Festlegen von Multi-Factor Authentication (MFA) für Ihren Partnermandanten](partner-security-requirements-mandating-mfa.md#partner-delegated-administration). In dem Fall, in dem Ihre Domäne keine Verbunddomäne ist, werden Sie nach erfolgreicher Authentifizierung aufgefordert, die mehrstufige Authentifizierung einzurichten. Nach Abschluss dieses Vorgangs können Sie Ihre Kunden mithilfe von AOBO verwalten. In dem Fall, in dem Ihre Domäne eine Verbunddomäne ist, müssen Sie sicherstellen, dass das Konto zur mehrstufigen Authentifizierung aufgefordert wird.

## <a name="security-defaults-transition"></a>Umstellung von Sicherheitsstandards

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Wie kann ich von Basisrichtlinien auf Sicherheitsstandards oder andere MFA-Lösungen umstellen?

Die Azure Active Directory (Azure AD)-[„Basisrichtlinien“ werden demnächst entfernt und ersetzt](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) durch „Sicherheitsstandards“, einen umfassenderen Satz von Schutzrichtlinien für Sie und Ihre Kunden. [Sicherheitsstandards](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) können dazu beitragen, Ihre Organisation vor Sicherheitsangriffen im Zusammenhang mit Identitätsdiebstahl zu schützen.

Ihre Implementierung der mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA) wird infolge der Deaktivierung der Basisrichtlinien entfernt, wenn Sie nicht von den Basisrichtlinien auf die Richtlinie für Sicherheitsstandards oder [andere MFA-Implementierungsoptionen](partner-security-requirements.md#actions-that-you-need-to-take) umgestellt haben. Alle Benutzer in Ihren Partnermandanten, die durch MFA geschützte Vorgänge ausführen, werden aufgefordert, die MFA-Überprüfung abzuschließen. Ausführlichere Informationen dazu finden Sie [hier](partner-security-requirements-mandating-mfa.md).
Führen Sie eine der folgenden Aktionen aus, damit Ihre Konformität gewahrt bleibt und Unterbrechungen so gering wie möglich sind:

- Umstellung auf Sicherheitsstandards
    - Die Richtlinie für Sicherheitsstandards ist eine der Optionen, die Partner zur Implementierung von MFA wählen können. Sie bietet eine grundlegende Sicherheitsstufe, die ohne Zusatzkosten bereitgestellt wird.
    - Informieren Sie sich, wie Sie MFA für Ihre Organisation mit Azure AD aktivieren, und lesen Sie die [wichtigsten Überlegungen zu Sicherheitsstandards](partner-security-requirements.md#security-defaults).
    - Aktivieren Sie die Richtlinie für Sicherheitsstandards, wenn Sie Ihren Geschäftsanforderungen entspricht.
- Umstellung auf bedingten Zugriff
    - Wenn die Richtlinie für Sicherheitsstandards Ihren Anforderungen nicht entspricht, aktivieren Sie „Bedingter Zugriff“. Weitere Informationen finden Sie in der Azure AD-Dokumentation zum bedingten Zugriff.

## <a name="key-resources"></a>Wichtige Ressourcen

### <a name="how-to-get-started"></a>Erste Schritte

- [Sicherheitsanforderungen für Partner: Schrittanleitung](partner-security-requirements.md).
- Sende Fragen und Feedback an die [Partner Center Security Guidance Group](https://aka.ms/MPCSecurityGuidance).
- Nimm an Informationsveranstaltungen und Webinaren für Partner teil. [Hier findest du den detaillierten Zeitplan und Ressourcen](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Ressourcen für die Übernahme des sicheren Anwendungsmodells

- [Übersicht über das sichere Anwendungsmodell](/partner-center/develop/enable-secure-app-model)
- [Partner Center: Leitfaden für das sichere Anwendungsmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungsmodells](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokumentation zur Authentifizierung in Partner Center](/partner-center/develop/partner-center-authentication)
- [Dokumentation zur Multi-Factor Authentication (MFA) in Partner Center über PowerShell](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Support

### <a name="where-can-i-get-support"></a>Wo erhalte ich Support?

Unterstützende Ressourcen für die Erfüllung der Sicherheitsanforderungen findest du hier: Wenn du über Advanced Support for Partners (ASfP) verfügst, wende dich an deinen Service Account Manager. Wenn du über eine Premier Support for Partners-Vereinbarung (PSfP) verfügst, wende dich an den Service Account Manager und den Technical Account Manager.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Wie erhalte ich technische Informationen und Unterstützung bei der Übernahme des Frameworks „Sicheres Anwendungsmodell“?

Optionen für den technischen Produktsupport für Azure Active Directory sind über MPN-Vorteile verfügbar. Partner mit Zugriff auf ein aktives ASfP- oder PSfP-Abonnement können sich an den entsprechenden Account Manager (SAM bzw. TAM) wenden, um die verfügbaren Optionen zu verstehen.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Wie kann ich mich an den Support wenden, wenn ich den Zugriff auf Partner Center verloren habe?

Navigiere zu [Microsoft Partner-Support](https://partner.microsoft.com/support), und wähle dann **Alle Supportoptionen anzeigen** aus. Ihnen werden die verfügbaren Optionen für die Kontaktaufnahme mit dem Microsoft Partner-Support angezeigt, einschließlich einer Telefonnummer, um den Support anzurufen, und einer Option, um mit dem Support zu chatten.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Wo finde ich Informationen zu häufigen technischen Problemen?

Informationen zu häufigen technischen Problemen finden Sie unter [Sicherheitsanforderungen für Partner, die das Partner Center oder Partner Center-APIs verwenden](partner-security-requirements.md).