---
title: FAQ zu den Sicherheitsanforderungen für Partner | Partner Center
ms.topic: article
ms.date: 07/18/2019
description: Häufig gestellte Fragen zu den Sicherheitsanforderungen des Partners
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider Program, CSP, System Steuerungs Hersteller, CPV, Multi-Factor Authentication, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820589"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Häufig gestellte Fragen zu den Sicherheitsanforderungen des Partners

Dieser Artikel enthält einige häufig gestellte Fragen zu den [Sicherheitsanforderungen des Partners](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Sicherheitsanforderungen für Partner

### <a name="what-are-the-new-partner-security-requirements"></a>Welche Sicherheitsanforderungen gelten für den neuen Partner?

Um unsere Partner und ihre Kunden zu schützen, fordern wir Partner auf, die folgenden Aktionen sofort durchführen zu können:  

1. **Aktivieren Sie die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) für alle Benutzer in Partner**Mandanten. Alle Benutzer in Partner Mandanten müssen die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) verwenden, wenn Sie sich bei kommerziellen Clouddiensten von Microsoft anmelden oder in CSP über Partner Center oder über APIs eine Transaktion durchführen. Durch die Aktivierung der baselineschutzrichtlinien ist MFA kostenlos für alle Benutzer von Partner Mandanten verfügbar.

2. Über **nehmen Sie das sichere Anwendungsmodell-Framework**. Alle Partner, die mit einer Microsoft-API, z. b. Azure Resource Manager, Microsoft Graph und der Partner Center-API, integrieren, müssen das sichere Anwendungsmodell Framework übernehmen, um eine Unterbrechung der Integration zu vermeiden, wenn die Basis Linien Richtlinien aktiviert sind 
 
Durch die Aktivierung der mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA) und die Übernahme des sicheren Anwendungsmodell-Frameworks können Sie Ihre Infrastruktur schützen und die Daten Ihrer Kunden vor potenziellen Sicherheitsrisiken schützen  

### <a name="which-partners-need-to-meet-the-requirements"></a>Welche Partner müssen die Anforderungen erfüllen?

Diese Anforderungen gelten für die folgenden Partnergruppen:
- Alle Partnerorganisationen, die am Cloud Solution Provider-Programm (CSP) teilnehmen, das mithilfe der kommerziellen Clouddienste von Microsoft transaagiert
  - Direkt Rechnungs Partner
  - Indirekte Anbieter
  - Indirekte Wiederverkäufer
- Alle System Steuerungs Anbieter
- Alle Advisor-Programmpartner  

Alle Partner, die eine Sovereign Cloud (21ViaNet, US Government und Deutschland) durchlaufen, müssen die neuen Sicherheitsanforderungen ab dem 1. August nicht erfüllen. Es wird jedoch dringend empfohlen, dass alle Partner einen Sovereign Cloud Act verwenden und diese neuen Sicherheitsanforderungen sofort übernehmen. Microsoft wird in Zukunft weitere Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

### <a name="what-are-the-key-timelines-and-milestones"></a>Was sind die wichtigsten Zeitachsen und Meilensteine?

Die Bedingungen, die diesen Sicherheitsanforderungen zugeordnet sind, werden sofort dem Leitfaden für das Cloud Solution Provider-Programm hinzugefügt. Diese Sicherheitsanforderungen müssen implementiert werden, damit Sie mit der Teilnahme am CSP-Programm gemäß dem 1. August 2019 kompatibel sind. 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>Was geschieht, wenn ich keine Aktionen nutze?

Partner, die diese Sicherheitspraktiken und Verpflichtungen nicht einhalten, können nicht in das Cloud Solution Provider-Programm eingreifen oder Kunden Mandanten verwalten, die delegierten Administratorrechte nutzen, sobald diese Sicherheitsanforderungen der Partner erzwungen werden. Wir werden gerade ein Erzwingungs Datum für die Anforderungen einrichten und die Partner des Datums mit detaillierten Informationen benachrichtigen.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Warum erzwingt Microsoft diese neuen Anforderungen?
Sicherheit und Datenschutz von Kunden und Partnern ist die höchste Priorität von Microsoft. Wir sehen weiterhin komplexere, zunehmende Anzahl von Sicherheitsangriffen, die in erster Linie mit Vorfällen bei der Identitäts Gefährdung in Zusammenhang stehen. Da vorbeugende Kontrollen eine wichtige Rolle bei der Gesamt Verteidigungsstrategie spielen, um Sicherheitsangriffe zu verhindern, werden wir mit der Erzwingung eines Satzes von obligatorischen Sicherheitsanforderungen beginnen, um Partner und ihre Kunden zu schützen.

### <a name="does-this-apply-to-all-geographies"></a>Gilt dies für alle geografischen Regionen?

Ja, dies gilt für alle geografischen Regionen. Es wird dringend empfohlen, dass alle Partner, die eine Sovereign Cloud (21ViaNet, US Government und Deutschland) durchlaufen, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner müssen jedoch nicht die neuen Sicherheitsanforderungen erfüllen, die ab dem 1. August gültig sind. Microsoft wird in Zukunft weitere Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

## <a name="required-actions"></a>Erforderliche Aktionen

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Welche wichtigen Aktionen muss ich durchführen, um die Anforderungen zu erfüllen?  
Alle Partner im CSP-Programm (direkt Rechnung, indirekter Anbieter und indirekter Händler), Berater und System Steuerungs Anbieter müssen die Anforderungen erfüllen.

1. **MFA für alle Benutzer erzwingen**

    Alle Partner im CSP-Programm, Berater und System Steuerungs Anbietern müssen die MFA für alle Benutzer in Ihrem Partner Mandanten erzwingen. Dies kann erreicht werden, indem die [MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), die [Endbenutzer-Schutz Basislinie](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)und alle zukünftigen Baseline-Richtlinien aktiviert werden. Die von den Baseline-Richtlinien bereitgestellte Funktionalität wird weiterentwickelt, um sicherzustellen, dass Partner und Kunden vor den sich ständig ändernden Sicherheitsbedrohungen geschützt werden. Daher ist es wichtig, dass Sie die Dokumentation zu den grundlegenden [Richtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) lesen, um mehr zu erfahren.

    - Siehe [Baseline-Richtlinie: Weitere Informationen zum Aktivieren der Richt](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) Linie für die MFA für Administratoren erforderlich für Administratoren anfordern von MFA für Administratoren.
    - Siehe [Baseline-Richtlinie: Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) ausführliche Informationen dazu, wie Sie die Baseline-Richtlinie für den Endbenutzer Schutz aktivieren.
    - Verstehen Sie das Konzept der grundlegenden [Schutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Weitere Überlegungen:

    - Indirekte Anbieter müssen mit indirekten Resellern zusammenarbeiten, um Sie in Partner Center zu integrieren, wenn Sie dies noch nicht getan haben, und ihre Händler ermutigen, die Anforderungen zu erfüllen.
    - Azure MFA wird für alle Benutzer im Partner Mandanten kostenlos über die Baseline-Richtlinien zur Verfügung gestellt, mit der einzigen Überprüfungs Methode, die die [Microsoft Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)verwendet.
    - Weitere Überprüfungsmethoden sind über die [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) SKUs verfügbar, wenn andere Methoden, z. b. SMS oder e-Mail, erforderlich sind.
    - Partner können auch für jeden Benutzer eine MFA-Lösung eines Drittanbieters nutzen, wenn Sie auf kommerzielle Clouddienste von Microsoft zugreifen.

2. **Übernehmen des sicheren Anwendungsmodell-Frameworks**

    Alle Partner, die eine benutzerdefinierte Integration mithilfe von APIs entwickelt haben (z. b. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) oder benutzerdefinierte Automation mit Tools wie PowerShell implementiert haben, müssen das [sichere Anwendungsmodell übernehmen. Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) , das in Microsoft Cloud Services integriert werden soll. Wenn dies nicht der Fall ist, kann dies aufgrund der MFA-Bereitstellung zu einer Unterbrechung führen. Die folgenden Ressourcen bieten eine Übersicht und Anleitungen zur Übernahme des Modells.

    - [Übersicht über das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Partner Center: Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungs Modells](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungs Modells](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [Partner Center-Authentifizierungs Dokument](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [MFA-Dokument (Partner Center PowerShell Multi-Factor Authentication)](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    Wenn Sie eine Systemsteuerung verwenden, müssen Sie sich bezüglich der Einführung des sicheren Anwendungsmodell-Frameworks an den Hersteller wenden.

    Systemsteuerungsanbieter müssen als solche in Partner Center [hinzugefügt](https://docs.microsoft.com/partner-center/enroll-as-cpv) werden, um sofort mit der Implementierung dieser Anforderung zu beginnen zu können. Weitere Informationen finden [Sie im Partner Center: Sicheres Anwendungsmodell-](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)Framework. System Steuerungs Anbieter müssen die Zustimmung von CSP-Partnern anstelle von Anmelde Informationen akzeptieren und verwalten und alle vorhandenen CSP-Partner Anmelde Informationen löschen.

## <a name="multi-factor-authentication"></a>Mehrstufige Authentifizierung

### <a name="what-is-mfa"></a>Was ist MFA?

Die mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) ist ein Sicherheitsmechanismus, bei dem Einzelpersonen durch mehr als eine erforderliche Sicherheits-und Validierungs Prozedur authentifiziert werden. Dies funktioniert, indem zwei oder mehr der folgenden Authentifizierungsmethoden erforderlich sind:

- Etwas, das Sie wissen (in der Regel ein Kennwort)
- Etwas, das Sie besitzen (ein vertrauenswürdiges Gerät, das sich nicht leicht duplizieren lässt, z. B. ein Telefon)
- Sie selbst (Biometrie)

### <a name="what-are-baseline-protection-policies"></a>Was sind Baseline-Schutzrichtlinien? 

Grund [Legende Schutzrichtlinien von Microsoft](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (derzeit ist die Vorschau) ein Satz vordefinierter Richtlinien, mit denen Organisationen vor vielen häufigen Angriffen geschützt werden. Diese häufigen Angriffe können Kenn Wort Spray, Wiedergabe und Phishing einschließen. Baseline-Richtlinien sind in allen Editionen von Azure Active Directory verfügbar. Microsoft stellt diese grundlegenden Schutzrichtlinien allen Benutzern zur Verfügung, da identitätsbasierte Angriffe in den letzten Jahren durchgeführt wurden. Ziel dieser Richtlinien ist es, sicherzustellen, dass für alle Organisationen ohne zusätzliche Kosten eine Baseline-Sicherheitsstufe aktiviert ist.

> [!NOTE]
> Microsoft Baseline-Richtlinien und zugehörige Funktionen werden weiterentwickelt, um Partner und Kunden vor sich ständig ändernden Sicherheitsbedrohungen besser zu schützen. In Kürze sind einige Benennungs-und Taxonomie-Änderungen mit den Baseline-Richtlinien möglich. Es wird dringend empfohlen, die Seite mit den Baseline-Richtlinien direkt zu besuchen, um die neuesten Informationen zu erhalten.

### <a name="what-baseline-policies-must-i-enable"></a>Welche Baseline-Richtlinien muss aktiviert werden?

Wenn Sie beabsichtigen, die aktuellen Baseline-Schutzrichtlinien zu verwenden, um für jeden Benutzer im Partner Mandanten MFA bereitzustellen, müssen Sie die Baseline-Richtlinien [MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) aktivieren aktivieren. Diese grundlegenden Schutzrichtlinien erfüllen die MFA-Anforderung für jeden Benutzer im Partner Mandanten kostenlos für die Partner, die Microsoft Authenticator-Apps über mobile Geräte verwenden.

Die [Baseline-Richtlinie MFA für Administratoren erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) wird für Administratoren im Partnerverzeichnis genutzt, und die Baseline-Richtlinie für den [Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) dient zum schützen nicht administrativer Benutzer im Partner Mandanten. Wenn Sie diese Richtlinien aktivieren, müssen Benutzer sich für MFA registrieren. Nachdem der Benutzer erfolgreich registriert wurde, wird er bei Anmelde versuchen basierend auf den Kriterien der Richtlinie zur Eingabe von MFA aufgefordert. Die von den Baseline-Richtlinien bereitgestellte Funktionalität wird weiterentwickelt, um sicherzustellen, dass Partner und Kunden vor den sich ständig ändernden Sicherheitsbedrohungen geschützt werden. Daher ist es wichtig, dass Sie die Dokumentation zu den grundlegenden [Richtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) lesen, um mehr zu erfahren.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Gewusst wie aktivieren Sie die Richtlinie MFA für Administratoren erforderlich? 

Die Baseline-Richtlinie MFA für Administratoren erforderlich kann über das Azure-Verwaltungs Portal aktiviert werden. Siehe [Baseline-Richtlinie: Weitere Informationen zum Aktivieren dieser Baseline](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) -Richtlinie finden Sie unter MFA für Administratoren.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Gewusst wie aktivieren Sie die Endbenutzer-Schutzrichtlinie?

Die Baseline-Richtlinie für den Endbenutzer Schutz kann über das Azure-Verwaltungs Portal aktiviert werden. Siehe [Baseline-Richtlinie: Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) ausführliche Informationen zum Aktivieren dieser Baseline-Richtlinie.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>Werden die Baseline-Richtlinien automatisch aktiviert? 

Nein, um diese Richtlinien zu aktivieren, muss ein Benutzer, der Mitglied der Rollen "globaler Administrator", "Sicherheitsadministrator" oder "bedingter Zugriffs Administrator" ist, die Richtlinien für die sofortige Verwendung der Richtlinie konfigurieren.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Welche Kosten fallen für die Aktivierung der MFA an?

Microsoft stellt MFA kostenlos durch die Implementierung der baselineschutz-Richtlinien [MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) bereit. Die einzige Überprüfungs Option, die über diese MFA-Version verfügbar ist, ist die [Microsoft Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Wenn ein Telefonanruf oder eine SMS-Nachricht erforderlich ist, muss eine [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) Lizenz erworben werden. Alternativ dazu können Sie eine Drittanbieter Lösung verwenden, um für jeden Benutzer in Ihrem Partner Mandanten MFA bereitzustellen – in diesem Fall ist es Ihre Aufgabe, sicherzustellen, dass Ihre MFA-Lösung erzwungen wird und Sie kompatibel sind.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Welche Aktionen benötige ich, wenn ich bereits über eine MFA-Lösung verfüge?

Über diese Sicherheitsanforderungen müssen sich Benutzer eines Partner Mandanten mit MFA authentifizieren, wenn Sie auf kommerzielle Clouddienste von Microsoft zugreifen. Die Lösung eines Drittanbieters kann verwendet werden, um diese Anforderungen zu erfüllen. Microsoft stellt keine Validierungstests mehr für unabhängige Identitäts Anbieter zur Kompatibilität mit Azure Active Directory bereit. Wenn Sie Ihr Produkt auf Interoperabilität testen möchten, lesen Sie diese [Richtlinien](https://www.microsoft.com/download/details.aspx?id=56843).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Welche Überprüfungs Methode kann ich verwenden, um MFA zu authentifizieren?

Microsoft stellt MFA kostenlos durch die Implementierung der baselineschutz-Richtlinien [MFA für Administratoren](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) bereit. Die einzige Überprüfungs Option, die über diese MFA-Version verfügbar ist, ist die [Microsoft Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Wenn ein Telefonanruf oder eine SMS-Nachricht erforderlich ist, muss eine [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) Lizenz erworben werden. Alternativ dazu können Sie eine Drittanbieter Lösung verwenden, um für jeden Benutzer in Ihrem Partner Mandanten MFA bereitzustellen – in diesem Fall ist es Ihre Aufgabe, sicherzustellen, dass Ihre MFA-Lösung erzwungen wird und Sie kompatibel sind.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Ich verwende mehrere Partner Mandanten für die Transaktion. Muss ich die MFA für alle implementieren?

Ja, Sie müssen die MFA für jeden Azure Active Directory Mandanten erzwingen, der dem CSP-Programm oder dem Advisor-Programm zugeordnet ist. Wenn Sie beabsichtigen, eine Azure Active Directory Premium Lizenz zu erwerben, muss eine Lizenz für den Benutzer in jedem Azure Active Directory Mandanten erworben werden.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Muss für jeden Benutzer in meinem Partner Mandanten MFA erzwungen werden? 

Die baselineschutz-Richtlinien [MFA für Administrator](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzer](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) erforderlich erzwingen die MFA für jeden Benutzer in Ihrem Partner Mandanten. Wenn Sie diese Richtlinien zur Bereitstellung von MFA nutzen und die [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) Anwendung verwenden, müssen Sie keine zusätzlichen Lizenzen erwerben. Andernfalls müssen Sie eine geeignete Lösung erwerben, um jedem Benutzer in Ihrem Partner Mandanten MFA zur Verfügung zu stellen.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Ich bin ein direkter Rechnungs Partner bei Microsoft. Was muss ich tun?

Die Partner von Direct Bill Cloud Solution Provider müssen die MFA für jeden Benutzer in Ihrem Partner Mandanten erzwingen.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Ich bin ein indirekter Reseller und führe nur einen Verteiler aus. Muss ich dies trotzdem tun?

Alle indirekten Reseller müssen die MFA für jeden Benutzer in Ihrem Partner Mandanten erzwingen. Dies ist eine Aktion, die der indirekte Reseller ausführen muss.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Ich verwende die Partner Center-API nicht. Muss ich trotzdem MFA implementieren?

Ja, diese Sicherheitsanforderung gilt für alle Benutzer, einschließlich Partner Administrator Benutzer und Endbenutzer in einem Partner Mandanten.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Welche Drittanbieter bieten MFA-Lösungen, die mit Azure Active Directory kompatibel sind?

Es gibt viele unabhängige Reviews von MFA-Lösungen, wie z. b. [Gartner](https://www.gartner.com/en/webinars/3881781). Bei der Überprüfung von MFA-Anbietern und-Lösungen müssen Partner sicherstellen, dass die von Ihnen gewählte Lösung mit Azure Active Directory kompatibel ist.

Microsoft stellt keine Validierungstests mehr für unabhängige Identitäts Anbieter zur Kompatibilität mit Azure Active Directory bereit. Wenn Sie Ihr Produkt auf Interoperabilität testen möchten, lesen Sie diese [Richtlinien](https://www.microsoft.com/download/details.aspx?id=56843).

Weitere Informationen finden Sie in der [Azure AD Verbund Kompatibilitätsliste](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Wie kann ich MFA in unserer Integrations Sandbox testen?

Die Baseline-Richtlinien [MFA für Administrator erforderlich](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) und [Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) sollten für Ihren Integration Sandbox-Mandanten aktiviert werden. Durch diese Richtlinie muss sich jeder Benutzer im Mandanten mit MFA authentifizieren.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>Wird der MFA-Effekt aktiviert, wie ich mit dem Mandanten meines Kunden interagiert? 

Nein. Die Erfüllung dieser Sicherheitsanforderungen wirkt sich nicht auf die Verwaltung Ihrer Kunden aus. Die Möglichkeit, Delegierte administrative Vorgänge auszuführen, wird nicht unterbrochen.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Unterliegen meine Kunden den Sicherheitsanforderungen des Partners?

Nein, es ist nicht erforderlich, dass Sie die MFA für jeden Benutzer in den Azure AD Mandanten Ihres Kunden erzwingen. Es wird jedoch empfohlen, dass Sie mit jedem Kunden zusammenarbeiten, um zu bestimmen, wie die Benutzer am besten geschützt werden.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>Können APP-Kenn Wörter mit den baselineschutzrichtlinien verwendet werden?

Ja, [App](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) -Kenn Wörter können verwendet werden. Lesen Sie die Überlegungen zur Verwendung von App-Kenn Wörtern, die [hier](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentiert sind, um zu ermitteln, ob Sie für Ihre Bedürfnisse unterstützt

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Kann jeder Benutzer von dieser Anforderung ausgeschlossen werden? 

Nein, jeder Benutzer, einschließlich Dienst Konten, muss sich mit MFA authentifizieren.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Gelten die Partner Sicherheitsanforderungen für die Integrations Sandbox?

Ja, die Sicherheitsanforderungen für Partner gelten für die Integrations Sandbox. Dies bedeutet, dass Sie die entsprechende MFA-Lösung für Benutzer im Integration Sandbox-Mandanten implementieren müssen. Es wird empfohlen, dass Sie die Baseline-Schutzrichtlinien implementieren, um MFA bereitzustellen.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Gewusst wie ein Konto für den Notfall Zugriff (Break Glass) konfigurieren?

Es hat sich als bewährte Vorgehensweise bewährt, ein oder zwei Notfall Zugriffs Konten zu erstellen, um zu verhindern, dass Sie versehentlich von Ihrem Azure AD Mandanten gesperrt werden. Hinsichtlich der Partner Sicherheitsanforderungen ist es erforderlich, dass sich jeder Benutzer mit MFA authentifiziert. Dies bedeutet, dass Sie die Definition eines Notfall Zugriffs Kontos ändern müssen. Dabei kann es sich um ein Konto handeln, das eine Drittanbieter Lösung für MFA nutzt.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Wie werden Gastbenutzer von den Sicherheitsanforderungen des Partners betroffen?

Gastbenutzer müssen sich mit MFA authentifizieren, wenn Sie auf Ressourcen in Ihrem Partner Mandanten zugreifen. Die Sicherheitsanforderungen des Partners haben keine Auswirkung darauf, dass der Gastbenutzer auf Ressourcen in seinem eigenen Mandanten zugreift.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Wenn ich eine Drittanbieter Lösung verwende, ist Active Directory Verbunddienst (ADFS) erforderlich? 

Nein, es ist nicht erforderlich, Active Directory Verbunddienst (ADFS) zu haben, wenn Sie eine Drittanbieter Lösung verwenden. Es wird empfohlen, dass Sie mit dem Anbieter der Lösung zusammenarbeiten, um zu bestimmen, welche Anforderungen für die Lösung erfüllt sind.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>Ist es erforderlich, die Baseline-Schutzrichtlinien zu aktivieren?

Nein, es ist nicht erforderlich, die baselineschutzrichtlinien zu aktivieren. Die einzige Voraussetzung besteht darin, dass Sie die MFA für jeden Benutzer, einschließlich der Dienst Konten, in Ihrem Partner Mandanten erzwingen.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kann der bedingte Zugriff verwendet werden, um die MFA-Anforderung zu erfüllen?

Ja, Sie können den bedingten Zugriff verwenden, um die MFA für jeden Benutzer, einschließlich der Dienst Konten, in Ihrem Partner Mandanten zu erzwingen. Angesichts der hohen privilegierten Natur eines Partners müssen wir jedoch sicherstellen, dass jeder Benutzer für jede einzelne Authentifizierung über eine MFA-Herausforderung verfügt. Dies bedeutet, dass Sie nicht in der Lage sind, die Funktion des bedingten Zugriffs zu nutzen, die die Anforderung für MFA umgehen.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Welche Überprüfungs Optionen werden durch die Implementierung der baselineschutzrichtlinien bereitgestellt? 

In Bezug auf die MFA-Version, die über die Implementierung der baselineschutzrichtlinien verfügbar ist, ist die einzige verfügbare Überprüfungs Option eine Authentifikator-app. Die Verwendung einer Telefonanruf-und SMS-Nachricht gilt als weniger sicher. Diese Optionen sind also in dieser MFA-Version nicht verfügbar.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Ist das Dienst Konto, das von verwendet wird, Azure AD Connect von den Sicherheitsanforderungen des Partners betroffen?

Nein, das von Azure AD Connect verwendete Dienst Konto wird von den Sicherheitsanforderungen des Partners nicht beeinträchtigt. Wenn Sie ein Problem mit Azure AD Connect aufgrund der Erzwingung von MFA haben, öffnen Sie eine technische Supportanfrage beim Microsoft-Support.

## <a name="secure-application-model"></a>Sicheres Anwendungsmodell

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Wer sollte das sichere Anwendungsmodell übernehmen, um die Anforderungen zu erfüllen?

Microsoft führt ein sicheres, skalierbares Framework für die Authentifizierung von Cloud Solution Provider (CSP)-Partnern und System Steuerungs Anbietern (CPV) ein, die die Multi-Factor Authentication nutzen. Weitere Informationen finden Sie im [Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) . Alle Partner, die eine benutzerdefinierte Integration mithilfe von APIs entwickelt haben (z. b. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) oder benutzerdefinierte Automation mit Tools wie PowerShell implementiert haben, müssen das [sichere Anwendungsmodell übernehmen. Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) , das in Microsoft Cloud Services integriert werden soll.

### <a name="what-is-the-secure-application-model"></a>Was ist das sichere Anwendungsmodell?

Microsoft führt ein sicheres, skalierbares Framework für die Authentifizierung von Cloud Solution Provider (CSP)-Partnern und System Steuerungs Anbietern (CPV) ein, die die Multi-Factor Authentication nutzen. Weitere Informationen finden Sie im [Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Gewusst wie das sichere Anwendungsmodell implementieren?

Alle Partner, die eine benutzerdefinierte Integration mithilfe von APIs entwickelt haben (z. b. Azure Resource Manager, Microsoft Graph, Partner Center-API usw.) oder benutzerdefinierte Automation mit Tools wie PowerShell implementiert haben, müssen das [sichere Anwendungsmodell übernehmen. Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) , das in Microsoft Cloud Services integriert werden soll. Wenn dies nicht der Fall ist, kann dies aufgrund der MFA-Bereitstellung zu einer Unterbrechung führen. Die folgenden Ressourcen bieten eine Übersicht und Anleitungen zur Übernahme des Modells.

- [Übersicht über das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungs Modells](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungs Modells](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Partner Center-Authentifizierungs Dokument](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [MFA-Dokument (Partner Center PowerShell Multi-Factor Authentication)](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

Wenn Sie eine Systemsteuerung verwenden, müssen Sie sich bezüglich der Einführung des sicheren Anwendungsmodell-Frameworks an den Hersteller wenden.

Systemsteuerungsanbieter müssen als solche in Partner Center [hinzugefügt](https://docs.microsoft.com/partner-center/enroll-as-cpv) werden, um sofort mit der Implementierung dieser Anforderung zu beginnen zu können. Weitere Informationen finden [Sie im Partner Center: Sicheres Anwendungsmodell-](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)Framework. System Steuerungs Anbieter müssen die Zustimmung von CSP-Partnern anstelle von Anmelde Informationen akzeptieren und verwalten und alle vorhandenen CSP-Partner Anmelde Informationen löschen.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Wer ist ein System Steuerungs Hersteller (System Steuerungs Vendor, CPV)? 
Ein System Steuerungs Anbieter ist ein unabhängiger Softwarehersteller, der apps entwickelt, die von CSP-Partnern für die Integration in Partner Center-APIs verwendet werden. Ein System Steuerungs Anbieter ist kein CSP-Partner mit direktem Zugriff auf das Partner Center-Dashboard oder APIs. Eine ausführliche Beschreibung finden Sie im [Partner Center: Leitfaden](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)zu sicheren Anwendungs Modellen.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Muss das sichere Anwendungsmodell nur für die Partner Center-API/das SDK implementiert werden? 

Wenn die Baseline-Richtlinien *MFA für Administratoren* und *Endbenutzer Schutz* erforderlich aktiviert sind, muss sich jeder Benutzer mit Multi-Factor Authentication authentifizieren. Dies bedeutet, dass Sie das sichere Anwendungsmodell für jede API, CLI und dieses PowerShell-Modul (z. b. Azure, Azure AD, MS Online, Partner Center usw.) implementieren müssen, das nicht interaktiv ausgeführt werden soll und die Verwendung von Benutzer Anmelde Informationen für die Authentifizierung benötigt.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Ich verwende Automatisierungstools wie PowerShell. Gewusst wie das sichere Anwendungsmodell implementieren?  

Wenn Ihre Automatisierung nicht interaktiv ausgeführt werden soll und Benutzer Anmelde Informationen für die Authentifizierung benötigt, müssen Sie das sichere Anwendungsmodell implementieren. Siehe [sicheres Anwendungsmodell | Partner Center PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) , um Anleitungen zur Implementierung dieses Frameworks zu erhalten.  Beachten Sie, dass nicht alle Automatisierungstools die Möglichkeit bieten, sich mit Zugriffs Token zu authentifizieren. Wenn Sie Hilfe benötigen, um zu verstehen, welche Änderungen vorgenommen werden müssen, senden Sie eine Nachricht in der [Partner Center-Sicherheits Leit Faden](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) Gruppe.

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Welche Benutzer Anmelde Informationen soll der Anwendungs Administrator beim Ausführen des Zustimmungs Prozesses bereitstellen? 

Es wird empfohlen, ein Dienst Konto zu verwenden, dem die geringsten Berechtigungen zugewiesen wurden. In Bezug auf die Partner Center-API bedeutet dies, dass Sie ein Konto verwenden sollten, dem entweder die Rolle "Sales Agent" oder "admin Agents" zugewiesen wurde.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Warum sollte der Anwendungs Administrator beim Ausführen des Zustimmungs Prozesses keine globalen Administrator Benutzer Anmelde Informationen bereitstellen?

Es wird empfohlen, den geringsten privilegierten Wert zu verwenden, um das Risiko zu verringern. Es wird nicht empfohlen, ein Konto zu verwenden, das über globale Administratorrechte verfügt, da dadurch mehr Berechtigungen bereitgestellt werden, als erforderlich sind.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Ich bin ein CSP-Partner. Gewusst wie wissen, ob der System Steuerungs Hersteller (CPV) an der Implementierung der Lösung arbeitet oder nicht? 

Für Partner, die eine CPV-Lösung (System Steuerungs Anbieter) verwenden, um das CSP-Programm (Cloud Solution Provider) zu verwenden, müssen Sie sich mit Ihrem CPV in zusammensetzen. 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Ich bin ein CPV. Gewusst wie registrieren? 

Befolgen Sie die [hier](https://docs.microsoft.com/partner-center/enroll-as-cpv)bereitgestellten Richtlinien, um sich als System Steuerungs Hersteller (CPV) anzumelden.

Damit der Registrierungs Link empfangen werden kann, muss er sich an den [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) Microsoft-Mitarbeiter Sponsor wenden, der über eine geschäftliche Beziehung mit der CPV verfügt oder sein Geschäft kennt. Beispielsweise ein Partner Development Manager (PDM).

Nachdem Sie sich bei Partner Center registriert und ihre Anwendungen registriert haben, haben Sie Zugriff auf die Partner Center-APIs. Wenn Sie ein neues CPV sind, erhalten Sie Ihre Sandbox-Informationen über eine Partner Center-Benachrichtigung. Nachdem Sie die Registrierung als Microsoft CPV abgeschlossen und die CPV-Vereinbarung akzeptiert haben, können Sie folgende Aktionen ausführen:

1. Verwalten einer mehr Instanzen fähigen Anwendung (Hinzufügen von Anwendungen zu Azure-Portal, registrieren und Aufheben der Registrierung von Anwendungen im Partner Center). Hinweis: CPVS müssen Ihre Anwendungen im Partner Center registrieren, um für Partner Center-APIs autorisiert zu werden. Das Hinzufügen von Anwendungen in das Azure-Portal allein reicht nicht aus, um CPV-Anwendungen für Partner Center-APIs zu autorisieren.
2. Sie können Ihr CPV-Profil anzeigen und verwalten.
3. Anzeigen und Verwalten Ihrer Benutzer, die Zugriff auf CPV Funktionen benötigen. Die einzige Rolle, die eine CPV aufweisen kann, ist der globale Administrator.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Ich verwende das Partner Center SDK. Übernimmt das SDK automatisch das sichere Anwendungsmodell? 

Nein, Sie müssen die Richtlinien befolgen, die im [Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)zur Verfügung stehen.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>Kann ich ein Aktualisierungs Token für das sichere Anwendungsmodell mit Konten generieren, für die MFA nicht aktiviert ist?

Ja, ein Aktualisierungs Token kann mit einem Konto generiert werden, für das MFA nicht erzwungen wird. Dies sollte jedoch nicht erfolgen, da jedes Token, das mit einem Konto generiert wird, für das MFA nicht aktiviert ist, aufgrund der MFA-Anforderung nicht auf Ressourcen zugreifen kann.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Wie sollte meine Anwendung ein Zugriffs Token erhalten, wenn wir die MFA aktivieren?

Sie müssen das Handbuch für den [sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) befolgen, das ausführliche Informationen dazu bereitstellt, während die neuen Sicherheitsanforderungen erfüllt werden. Hier finden Sie Beispielcode für [.NET](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) und [Java](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Erstellen Sie als CPV eine Azure AD-Anwendung in unserem CPV-Mandanten oder im Mandanten des CSP-Partners?

Die CPV muss die Azure Active Directory Anwendung in dem Mandanten erstellen, der mit Ihrer Registrierung als CPV verknüpft ist.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Ich bin ein CSP, der die reine App-Authentifizierung verwendet. Muss ich Änderungen vornehmen?

Die reine App-Authentifizierung wird nicht beeinträchtigt, weil keine Benutzer Anmelde Informationen verwendet werden, um ein Zugriffs Token anzufordern. Wenn die Benutzer Anmelde Informationen freigegeben werden, müssen System Steuerungs Anbieter (CPVS) das [sichere Anwendungsmodell Framework](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) übernehmen und vorhandene, vorhandene Partner Anmelde Informationen bereinigen.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Als CPV kann ich den Authentifizierungs Stil der app nur nutzen, um Zugriffs Token zu erhalten?

Nein, System Steuerungs Partner Partner können den Authentifizierungs Stil der app nur dann verwenden, wenn Sie im Namen des Partners Zugriffs Token anfordern. Sie sollten das sichere Anwendungsmodell implementieren, das den Stil der APP-und Benutzerauthentifizierung verwendet.

## <a name="key-resources"></a>Wichtige Ressourcen

### <a name="how-to-get-started"></a>Erste Schritte

- [Sicherheitsanforderungen für Partner: Schritt-für-Schritt-Anleitung](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Leiten Sie Ihre Fragen und Ihr Feedback an diese [Partner Center-Sicherheits Leit Faden Gruppe](https://aka.ms/MPCSecurityGuidance)weiter.
- Besuchen Sie anstehende Partner Bürostunden und Webinare. Überprüfen Sie [hier den detaillierten Zeitplan und die Ressourcen](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Ressourcen zum Aktivieren von MFA

- Verstehen Sie das Konzept der grundlegenden [Schutzrichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Siehe [Baseline-Richtlinie: Weitere Informationen zum Aktivieren der Richt](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) Linie für die MFA für Administratoren erforderlich für Administratoren anfordern von MFA für Administratoren.
- Siehe [Baseline-Richtlinie: Endbenutzer Schutz](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) ausführliche Informationen dazu, wie Sie die Baseline-Richtlinie für den Endbenutzer Schutz aktivieren.

### <a name="resources-for-adopting-secure-application-model"></a>Ressourcen für die Übernahme eines sicheren Anwendungs Modells

- [Übersicht über das sichere Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Partner Center: Handbuch zum sicheren Anwendungsmodell](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner im CSP-Programm: .NET-Beispielcode zum Aktivieren des sicheren Anwendungs Modells](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partner im CSP-Programm: Java-Beispielcode zum Aktivieren des sicheren Anwendungs Modells](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Partner Center-Authentifizierungs Dokument](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [MFA-Dokument (Partner Center PowerShell Multi-Factor Authentication)](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>Unterstützung

### <a name="where-can-i-ask-get-support"></a>Wo kann ich Support erhalten?

Wenn Sie über erweiterte Unterstützung für Partner (asfp) verfügen, wenden Sie sich außerdem an Ihren Dienst Konto-Manager, um die Unterstützung der Nutzung von Ressourcen zu erfüllen. wenden Sie sich für Premier Support for Partner Agreement (psfp) an Ihren Dienst Konto-Manager und den technischen Konto-Manager.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Wie erhalte ich Hilfe beim Aktivieren der Baseline-Richtlinien?

- Partner können die Beratungsstunden von MPN-Vorteilen nutzen, um ausführlichere Anleitungen zum Implementieren der Sicherheitsanforderungen zu erhalten.
- Technische Produktsupport Optionen für Azure Active Directory sind über Ihre MPN-Vorteile verfügbar. Partner mit Zugriff auf eine aktive asfp-oder psfp-Vereinbarung können mit ihrem zugehörigen Konto-Manager (Sam/TAM) zusammenarbeiten, um die verfügbaren Optionen optimal zu verstehen.
- Der Zugriff auf die Implementierung von Baselinerichtlinien mit Partner Center kann über [Partner Center Service Request](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)erfolgen. Wählen Sie *MFA & sicheres Anwendungsmodell* als Thema aus.

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>Gewusst wie Sie technische Informationen zur Übernahme eines sicheren Anwendungsmodell-Frameworks? 

Technische Produktsupport Optionen für Azure Active Directory sind über Ihre MPN-Vorteile verfügbar. Partner mit Zugang zu einem aktiven asfp-oder psfp-Abonnement können mit dem zugehörigen Konto-Manager (Sam/TAM) zusammenarbeiten, um die verfügbaren Optionen optimal zu verstehen.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Wo finde ich weitere Informationen zu technischen häufigen Problemen? 

Informationen zu den technischen häufigen Problemen finden Sie [hier](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
