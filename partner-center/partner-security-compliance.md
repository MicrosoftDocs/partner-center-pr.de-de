---
title: Status der Sicherheitsanforderungen für Partner | Partner Center
ms.date: 10/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bleiben Sie bei der Compliance Ihres Unternehmens mit MFA-Anforderungen auf dem aktuellen Stand.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider-Programm, CSP, Control Panel-Anbieter, CPV, mehrstufige Authentifizierung, MFA, sicheres Anwendungsmodell, sicheres App-Modell, Sicherheit
ms.localizationpriority: high
ms.openlocfilehash: 52a87b80c68ec44263a7e402ea458b918aa952df
ms.sourcegitcommit: 9612a02407b8f18f825e1433adc4e6b0b62c9034
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73661116"
---
# <a name="partner-security-requirements-status"></a>Status der Sicherheitsanforderungen für Partner

**Zielgruppe**

- Alle Partner im Cloud Solution Provider-Programm
  - Direktrechnung
  - Indirekter Anbieter
  - Indirekter Wiederverkäufer
- Alle Control Panel-Anbieter
- Alle Berater

Mehr Sicherheitsmaßnahmen für den Datenschutz und eine höhere Sicherheit gehören zu unseren obersten Prioritäten. Wir wissen, dass die beste Verteidigung die Prävention ist und dass wir nur so stark sind wie unser schwächstes Glied. Deshalb müssen alle in unserem Ökosystem handeln und sicherstellen, dass sie über angemessene Sicherheitsvorkehrungen verfügen. Zum Schutz von Partnern und Kunden führen wir eine Reihe von verbindlichen Sicherheitsanforderungen für Berater, Control Panel-Anbieter und Partner ein, die am Cloud Solution Provider-Programm teilnehmen.

Seit dem 1. August 2019 sind alle Partner verpflichtet, die mehrstufige Authentifizierung für alle Benutzer, einschließlich Dienstkonten, in ihrem Partnermandanten durchzusetzen. Ausführlichere Informationen zu den neuen Sicherheitsrichtlinien finden Sie unter [Sicherheitsanforderungen für Partner](partner-security-requirements.md).

Wir möchten sicherstellen, dass jeder Benutzer für jede einzelne Authentifizierung über eine MFA-Herausforderung verfügt. Dies kann auf eine der folgenden Arten erreicht werden:

- Implementieren von Azure AD Premium zum Sicherstellen, dass MFA für jeden Benutzer erzwungen wird
- Implementieren der [Azure AD-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementieren der Lösung eines Drittanbieters zum Sicherstellen, dass MFA für jeden Benutzer erzwungen wird

## <a name="partner-security-requirements-status"></a>Status der Sicherheitsanforderungen für Partner

Mithilfe dieses Berichts können Sie den Status der Sicherheitsanforderungen überprüfen, da er Ihnen die Möglichkeit gibt, zu sehen, wo Sie möglicherweise zurückbleiben. Die Nachverfolgung wird regelmäßig aktualisiert.

>[!NOTE]
>Der Bericht zum Status der Sicherheitsanforderungen für Partner wird nur im Partner Center unterstützt. Er steht in der Microsoft Cloud for US Government oder der Microsoft Cloud Deutschland nicht zur Verfügung. Es wird dringend empfohlen, dass alle Partner, die über eine unabhängige Cloud (21Vianet, US-Regierung und Deutschland) handeln, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner sind jedoch nicht verpflichtet, die neuen Sicherheitsanforderungen zum 1. August 2019 zu erfüllen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

Bei jeder Anmeldung Ihrer Mitarbeiter beim Partner Center, um zu arbeiten oder mithilfe von APIs Daten über das Partner Center abzurufen oder zu senden, wird der Sicherheitsstatus Ihrer Mitarbeiter herausgefordert und nachverfolgt. Ebenfalls in der Nachverfolgung des Sicherheitsstatus enthalten sind Ihre Anwendungen und alle Anwendungen von Anbietern in der Systemsteuerung. Der angezeigte Status bezieht sich auf die vergangenen 7 Tage.

## <a name="multi-factor-authentication-mfa-report"></a>Bericht zur mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA)

Der Partner Center-MFA-Bericht bietet Erkenntnisse über die MFA-Partnerimplementierung, indem er zwei Metriken auf der Grundlage von Aktivitäten im Partner Center bereitstellt:

**Von Benutzern abgeschlossene MFA-Überprüfung**

Diese Metrik bezieht sich auf Aktivitäten im Partner Center-Dashboard. Sie misst den Prozentsatz der Vorgänge, die von Benutzern ausgeführt wurden, die die MFA-Überprüfung abgeschlossen haben. Zum Beispiel:

- Contoso ist ein CSP-Partner mit zwei Administratormitarbeitern Jane und John.
- Am ersten Tag hat Jane sich beim Partner Center-Dashboard ohne MFA-Überprüfung angemeldet und 3 Vorgänge ausgeführt.
- Am zweiten Tag hat John sich beim Partner Center-Dashboard ohne MFA-Überprüfung angemeldet und 5 Vorgänge ausgeführt.
- Am dritten Tag hat Jane sich beim Partner Center-Dashboard mit MFA-Überprüfung angemeldet und 2 Vorgänge ausgeführt.
- An den verbleibenden 4 Tagen wurden von keinem der Mitarbeiter Vorgänge ausgeführt.
- Von den 10 Vorgängen, die innerhalb des 7-Tage-Zeitraums ausgeführt wurden, sind 2 von Benutzern mit MFA-Überprüfung vorgenommen worden. Daher zeigt die Metrik 20 % an.

**Anwendungs- und Benutzerauthentifizierung**

Diese Metrik bezieht sich auf die Verwendung von API-Anforderungen im Partner Center, die mithilfe von Anwendungs- und Benutzerauthentifizierung erfolgt sind. Sie misst den Prozentsatz der API-Anforderungen, die mithilfe eines Zugriffstokens mit MFA-Anspruch erfolgt sind. Zum Beispiel:

- Fabrikam ist ein CSP-Partner und verfügt über eine CSP-Anwendung, die eine Mischung aus Anwendungs- und Benutzerauthentifizierung und rein auf die Anwendung beschränkten Authentifizierungsmethoden verwendet.
- Am ersten Tag hat die Anwendung 3 API-Anforderungen vorgenommen, die auf ein Zugriffstoken gestützt waren, das ohne MFA-Überprüfung bei der Methode zur Anwendungs- und Benutzerauthentifizierung abgerufen wurde.
- Am zweiten Tag hat die Anwendung 5 API-Anforderungen vorgenommen, die sich auf ein Zugriffstoken stützten, das nur mithilfe reiner Anwendungsauthentifizierung abgerufen wurde.
- Am dritten Tag hat die Anwendung 2 API-Anforderungen vorgenommen, die auf ein Zugriffstoken gestützt waren, das mit MFA-Überprüfung bei der Methode zur Anwendungs- und Benutzerauthentifizierung abgerufen wurde.
- An den verbleibenden 4 Tagen wurden von keinem der Mitarbeiter Vorgänge ausgeführt.
- Die 5 API-Anforderungen am zweiten Tag, die von einem Zugriffstoken gestützt waren, das über reine Anwendungsauthentifizierung abgerufen wurde, werden von der Metrik ausgelassen, da sie keine Benutzeranmeldeinformationen verwendeten. Von den verbleibenden 5 Vorgängen waren 2 durch ein Zugriffstoken gestützt, das mithilfe von MFA-Überprüfung abgerufen wurde. Daher zeigt die Metrik 40 % an.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Vorgehen, wenn die im MFA-Bericht ausgewiesenen Metriken keine 100 % erreichen

Es ist möglich, dass die im MFA-Bericht im Partner Center ausgewiesenen Metriken für Partner, die MFA implementiert haben, keine 100 % erreichen. Dies wird leicht verständlich, wenn die zu berücksichtigenden Faktoren bekannt sind.

> [!NOTE]
> Sie müssen mit jemandem aus Ihrer Organisation zusammenarbeiten, der/die mit Identitätsverwaltung und MFA-Implementierung für Ihren Partnermandanten vertraut ist.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Haben Sie MFA für Ihren Partnermandanten implementiert?

Andernfalls müssen Sie zunächst MFA für Ihren Partnermandanten implementieren. Ausführliche Informationen zur Implementierung von MFA finden Sie im Artikel [Sicherheitsanforderungen für Partner](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Haben Sie die MFA-Implementierung erst vor kurzem abgeschlossen?

Die Metriken werden täglich errechnet und berücksichtigen Vorgänge, die im Verlauf der letzten 7 Tage ausgeführt wurden. Wenn Sie die MFA-Implementierung für Ihren Partnermandanten erst vor kurzem abgeschlossen haben, erreichen die Metriken möglicherweise keine 100 %.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Wurden einige Benutzerkonten aus der MFA-Implementierung ausgeschlossen?

Verstehen Sie, ob Ihre aktuelle MFA-Implementierung alle Benutzerkonten oder nur einige abdeckt. Einige MFA-Lösungen sind richtlinienbasiert und unterstützen den Ausschluss von Benutzern, während Sie möglicherweise für andere die MFA auf Benutzerbasis explizit aktivieren müssen. Vergewissern Sie sich, dass Sie keine Benutzer aus Ihrer aktuellen MFA-Implementierung ausgeschlossen haben. Jedes Benutzerkonto, das ausgeschlossen wurde und sich beim Partner Center anmeldet, um mit CSP zusammenhängende Aktivitäten auszuführen, kann bewirken, dass die Metriken nicht 100 % erreichen.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>Ist MFA nur erforderlich, wenn bestimmte Bedingungen erfüllt sind?

Verstehen Sie, ob die aktuelle Implementierung MFA nur unter bestimmten Bedingungen erzwingt. Einige MFA-Lösungen bieten Flexibilität und erzwingen MFA nur, wenn bestimmte Bedingungen erfüllt sind. Beispielsweise, wenn der Benutzer von einem unbekannten Gerät oder einem unbekannten Standort zugreift. Ein Benutzer, der für MFA aktiviert ist, aber für den der Abschluss der MFA-Überprüfung beim Zugriff auf das Partner Center nicht vorgeschrieben ist, kann bewirken, dass die Metriken 100 % nicht erreichen.

>[!NOTE]
>Partner, die MFA mithilfe von Azure AD-Sicherheitsstandards implementiert haben, müssen beachten, dass die mehrstufige Authentifizierung für Nicht-Administrator-Benutzerkonten risikobasiert erzwungen wird. Benutzer werden nur bei Anmeldeversuchen mit erhöhtem Risiko zur MFA aufgefordert (beispielsweise, wenn sich der Benutzer von einem anderen Standort aus anmeldet). Außerdem bleiben Benutzern 14 Tage Zeit für die Registrierung bei MFA. Benutzer, die die MFA-Registrierung nicht abgeschlossen haben, werden während des 14-Tages-Zeitraums nicht zur MFA-Überprüfung aufgefordert. Daher ist bei Partnern, die MFA mithilfe der Azure AD-Sicherheitsstandards implementiert haben, damit zu rechnen, dass die Metriken die 100 % nicht erreichen.

### <a name="are-you-using-3rd-party-mfa-solution"></a>Verwenden Sie eine MFA-Lösung eines Drittanbieters?

Wenn Sie eine Drittanbieter-MFA-Lösung verwenden, bestimmen Sie, wie Sie diese in Azure AD integrieren. Im Allgemeinen gibt es zwei Methoden, einschließlich Partnerverbund und benutzerdefinierter Steuerelemente:

* **Identitätsverbund**: Wenn Azure AD eine Authentifizierungsanforderung empfängt, leitet Azure AD den Benutzer zur Authentifizierung an den Verbundidentitätsanbieter um. Bei erfolgreicher Authentifizierung leitet der Verbundidentitätsanbieter den Benutzer zusammen mit einem SAML-Token wieder an Azure AD weiter. Damit Azure AD erkennen kann, dass der Benutzer die MFA-Überprüfung bei seiner Authentifizierung beim Verbundidentitätsanbieter abgeschlossen hat, muss das SAML-Token den Anspruch *authenticationmethodsreferences* (mit dem Wert *multipleauthn*) enthalten. Überprüfen Sie, ob der Verbundidentitätsanbieter die Ausstellung eines solchen Anspruchs unterstützt. Ist dies der Fall, überprüfen Sie, ob der Verbundidentitätsanbieter entsprechend konfiguriert wurde. Wenn der Anspruch fehlt, weiß Azure AD (und entsprechend auch das Partner Center) nicht, dass der Benutzer die MFA-Überprüfung abgeschlossen hat, was dazu führen kann, dass die Metrik nicht die 100 % erreicht.

* **Benutzerdefiniertes Steuerelement**: Ein benutzerdefiniertes Azure AD-Steuerelement kann nicht verwendet werden, um zu ermitteln, ob ein Benutzer die MFA-Überprüfung über eine MFA-Drittanbieterlösung abgeschlossen hat. Daher erscheint jeder Benutzer, der die MFA-Überprüfung mithilfe eines benutzerdefinierten Steuerelements abgeschlossen hat, für Azure AD (und in der Folge auch für das Partner Center) als mit nicht abgeschlossener MFA-Überprüfung angemeldet. Es empfiehlt sich, wo immer möglich dem Identitätsverbund bei der Integration in Azure Ad gegenüber benutzerdefinierten Steuerelementen den Vorzug zu geben.

### <a name="identity-which-users-have-logged-into-partner-center-without-mfa"></a>Bestimmen der Benutzer, die sich ohne MFA beim Partner Center angemeldet haben

Es kann sinnvoll sein, zu identifizieren, welche Benutzer sich ohne MFA-Überprüfung beim Partner Center anmelden und sie mithilfe Ihrer aktuellen MFA-Implementierung zu überprüfen. Sie können den [Azure AD-Anmeldebericht](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) verwenden, um herauszufinden, ob ein Benutzer die MFA-Überprüfung abgeschlossen hat oder nicht. Der Azure AD-Anmeldebericht steht zurzeit nur Partnern zur Verfügung, die Azure AD Premium oder eine andere O365-SKU abonniert haben, die Azure AD Premium enthält (beispielsweise EMS).

**Weitere Informationen**

- [Partner Center security guidance group community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Sicherheitsanforderungen für Partner](partner-security-requirements.md)
- [Häufig gestellte Fragen (FAQ) zu den Sicherheitsanforderungen für Partner](partner-security-requirements-faq.md)
