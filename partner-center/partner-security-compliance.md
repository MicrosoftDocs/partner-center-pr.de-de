---
title: Bericht zum Status der Sicherheitsanforderungen
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die Einhaltung der Sicherheitsanforderungen mit dem Bericht zum Status der Sicherheitsanforderungen und dem MFA-Bericht im Partner Center überprüfen.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: d56b9675ea405b29190f68420037ea9a92f3d831
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086548"
---
# <a name="security-requirements-status-report"></a>Bericht zum Status der Sicherheitsanforderungen

**Geeignete Rollen**
- CPV-Administrator
- Globaler Administrator

In diesem Artikel wird der Bericht zum Status der Sicherheitsanforderungen im Partner Center erläutert. Dieser Bericht enthält Metriken zur Einhaltung von [Sicherheitsanforderungen für Partner](partner-security-requirements.md) hinsichtlich der mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA) für Benutzer in Ihrem Partnermandanten.

Um auf diesen Bericht im [Partner Center](https://partner.microsoft.com/dashboard) zuzugreifen, wechseln Sie zu **Einstellungen** > **Kontoeinstellungen** > **Status der Sicherheitsanforderungen**. Der Bericht wird täglich aktualisiert und stellt die Anmeldedaten der letzten sieben Tage dar.

>[!NOTE]
>Der Bericht zum Status der Sicherheitsanforderungen wird nur im Partner Center unterstützt. Er steht in der Microsoft Cloud for US Government oder der Microsoft Cloud Deutschland nicht zur Verfügung. Es wird dringend empfohlen, dass alle Partner, die Transaktionen über eine unabhängige Cloud (US Government und Deutschland) ausführen, diese neuen Sicherheitsanforderungen sofort umsetzen. Diese Partner sind derzeit jedoch nicht verpflichtet, die neuen Sicherheitsanforderungen zu erfüllen. Microsoft wird in Zukunft zusätzliche Details zur Durchsetzung dieser Sicherheitsanforderungen für unabhängige Clouds bereitstellen.

## <a name="security-status-metrics"></a>Metriken für den Sicherheitsstatus

Der Bericht zum Status der Sicherheitsanforderungen bietet Erkenntnisse über die MFA-Implementierung von Partnern und stellt Metriken für die MFA-Konfiguration und Partner Center-Aktivitäten in Partnermandanten bereit. In den folgenden Abschnitten werden diese Metriken genauer erläutert.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-Konfiguration für einen Partnermandanten

Die Metrik **Prozentsatz der aktivierten Benutzerkonten, bei denen MFA mithilfe der hier aufgeführten Optionen erzwungen wird:** zeigt den Prozentsatz der aktivierten Benutzerkonten in Ihrem Partnermandanten, für die MFA erzwungen wird. Sie können eine dieser [MFA-Optionen](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) verwenden, um Konformität zu erreichen. Diese Daten werden täglich erfasst und gemeldet. Beispiel:

- Contoso ist ein CSP-Partner mit 110 Benutzerkonten im Mandanten. 10 Benutzerkonten sind deaktiviert. 
- Für 90 von den übrigen 100 Benutzerkonten wird mithilfe der bereitgestellten [MFA-Optionen](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) MFA erzwungen. Daher zeigt die Metrik 90 % an. 

### <a name="partner-center-requests-with-mfa"></a>Partner Center-Anforderungen mit MFA

Bei jeder Anmeldung Ihrer Mitarbeiter beim Partner Center, um zu arbeiten oder mithilfe von APIs Daten über das Partner Center abzurufen oder zu senden, wird der Sicherheitsstatus Ihrer Mitarbeiter herausgefordert und nachverfolgt. Ebenfalls in der Nachverfolgung des Sicherheitsstatus enthalten sind Ihre Anwendungen und alle Control Panel Vendor-Anwendungen. Diese Daten werden in Metriken unter **Prozentsatz der Anforderungen an Partner Center mit MFA** angezeigt und stellen die letzten sieben Tage dar.

#### <a name="dashboard-mfa-verification"></a>MFA-Überprüfung für das Dashboard

Die Metrik **Über das Partner Center-Portal** bezieht sich auf Aktivitäten im Partner Center-Dashboard. Sie misst den Prozentsatz der Vorgänge, die von Benutzern ausgeführt wurden, die die MFA-Überprüfung abgeschlossen haben. Beispiel:

- Contoso ist ein CSP-Partner mit zwei Administratormitarbeitern Jane und John.
- Am ersten Tag hat sich Jane beim Partner Center-Dashboard ohne MFA-Überprüfung angemeldet und drei Vorgänge ausgeführt.
- Am zweiten Tag hat sich John beim Partner Center-Dashboard ohne MFA-Überprüfung angemeldet und fünf Vorgänge ausgeführt.
- Am dritten Tag hat sich Jane beim Partner Center-Dashboard mit MFA-Überprüfung angemeldet und zwei Vorgänge ausgeführt.
- An den verbleibenden vier Tagen wurden von keinem der Mitarbeiter Vorgänge ausgeführt.
- Von den zehn Vorgängen, die innerhalb des Sieben-Tage-Zeitraums stattgefunden haben, wurden zwei von Benutzern mit MFA-Überprüfung vorgenommen. Daher zeigt die Metrik 20 % an.

Verwenden Sie die Datei für **Portalanforderungen ohne MFA**, um zu ermitteln, welcher Benutzer sich ohne MFA-Überprüfung beim Partner Center-Dashboard angemeldet hat, und wann der letzte Besuch innerhalb des Berichterstellungszeitfensters stattgefunden hat.

#### <a name="appuser-mfa-verification"></a>MFA-Überprüfung für Anwendung und Benutzer

Die Metrik **Über API oder SDK** bezieht sich auf die Anwendungs- und Benutzerauthentifizierung über API-Anforderungen im Partner Center. Sie misst den Prozentsatz der API-Anforderungen, die mithilfe eines Zugriffstokens mit MFA-Anspruch erfolgt sind. Beispiel:

- Fabrikam ist ein CSP-Partner und verfügt über eine CSP-Anwendung, die eine Mischung aus Anwendungs- und Benutzerauthentifizierung und rein auf die Anwendung beschränkten Authentifizierungsmethoden verwendet.
- Am ersten Tag hat die Anwendung drei API-Anforderungen unter Verwendung eines Zugriffstokens ausgeführt, das mit App- und Benutzerauthentifizierung ohne MFA-Überprüfung abgerufen wurde.
- Am zweiten Tag hat die Anwendung fünf API-Anforderungen unter Verwendung eines Zugriffstokens ausgeführt, das mit einer reinen App-Authentifizierung abgerufen wurde.
- Am dritten Tag hat die Anwendung zwei API-Anforderungen unter Verwendung eines Zugriffstokens ausgeführt, das mit App- und Benutzerauthentifizierung einschließlich MFA-Überprüfung abgerufen wurde.
- An den verbleibenden vier Tagen wurden von keinem der Mitarbeiter Vorgänge ausgeführt.
- Die fünf API-Anforderungen am zweiten Tag, die unter Verwendung eines Zugriffstokens ausgeführt wurden, das mit einer reinen App-Authentifizierung abgerufen wurde, werden von der Metrik nicht berücksichtigt, da keine Benutzeranmeldeinformationen verwendet werden. Von den verbleibenden fünf Vorgängen wurden zwei unter Verwendung eines Zugriffstokens ausgeführt, das mit MFA-Überprüfung abgerufen wurde. Daher zeigt die Metrik 40 % an.

Wenn Sie wissen möchten, welche App- und Benutzeraktivitäten diese Metrik nicht zu 100 % erfüllen, verwenden Sie die folgenden Dateien:

- **Zusammenfassung der API-Anforderungen**: Bietet Informationen zum allgemeinen MFA-Status nach Anwendung.
- **Alle API-Anforderungen**: Enthält Details zu den einzelnen API-Anforderungen von Benutzern Ihres Mandanten. Das Ergebnis ist auf die letzten 10.000 Anforderungen beschränkt, um die Downloaderfahrung zu verbessern.

## <a name="actions-for-mfa-status-below-100"></a>Aktionen für MFA-Status unter 100 %

Einigen Partnern, die MFA implementiert haben, werden möglicherweise Berichtsmetriken unter 100 % angezeigt. Dies wird leicht verständlich, wenn die zu berücksichtigenden Faktoren bekannt sind.

> [!NOTE]
> Sie müssen mit jemandem aus Ihrer Organisation zusammenarbeiten, der/die mit Identitätsverwaltung und MFA-Implementierung für Ihren Partnermandanten vertraut ist.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementierte MFA für den Partnermandanten

Sie müssen MFA für Ihren Partnermandanten implementieren, um Konformität zu erreichen. Ausführliche Informationen zur Implementierung von MFA finden Sie unter [Sicherheitsanforderungen für die Verwendung von Partner Center oder Partner Center-APIs](partner-security-requirements.md).

>[!NOTE]
> MFA-Metriken werden täglich berechnet und berücksichtigen Vorgänge, die in den letzten sieben Tagen ausgeführt wurden. Wenn Sie die MFA-Implementierung für Ihren Partnermandanten erst vor Kurzem abgeschlossen haben, erreichen die Metriken möglicherweise noch nicht 100 %.

### <a name="verify-mfa-on-all-user-accounts"></a>Überprüfen der MFA für alle Benutzerkonten

Verstehen Sie, ob Ihre aktuelle MFA-Implementierung alle Benutzerkonten oder nur einige abdeckt. Einige MFA-Lösungen sind richtlinienbasiert und unterstützen den Ausschluss von Benutzern. Bei anderen müssen Sie MFA u. U. explizit auf Benutzerbasis aktivieren. Vergewissern Sie sich, dass Sie keine Benutzer aus Ihrer aktuellen MFA-Implementierung ausgeschlossen haben. Jedes ausgeschlossene Benutzerkonto, über das sich ein Benutzer beim Partner Center anmeldet, um CSP-, CPV- oder beraterbezogene Aktivitäten auszuführen, kann bewirken, dass die Metriken keine 100 % erreichen.

### <a name="review-your-mfa-conditions"></a>Überprüfen der MFA-Bedingungen

Sie sollten wissen, ob MFA von Ihrer aktuellen Implementierung nur unter bestimmten Bedingungen erzwungen wird. Einige MFA-Lösungen bieten Flexibilität und erzwingen MFA nur, wenn bestimmte Bedingungen erfüllt sind. Beispielsweise, wenn der Benutzer von einem unbekannten Gerät oder einem unbekannten Standort zugreift. Ein Benutzer, der für MFA aktiviert ist, aber für den der Abschluss der MFA-Überprüfung beim Zugriff auf das Partner Center nicht vorgeschrieben ist, kann bewirken, dass die Metriken 100 % nicht erreichen.

>[!NOTE]
>Partner, die MFA mithilfe von Azure AD-Sicherheitsstandards implementiert haben, müssen beachten, dass die mehrstufige Authentifizierung für Nicht-Administrator-Benutzerkonten risikobasiert erzwungen wird. Benutzer werden nur bei Anmeldeversuchen mit erhöhtem Risiko zur MFA aufgefordert (beispielsweise, wenn sich der Benutzer von einem anderen Standort aus anmeldet). Außerdem bleiben Benutzern 14 Tage Zeit für die Registrierung bei MFA. Benutzer, die die MFA-Registrierung nicht abgeschlossen haben, werden während des 14-Tages-Zeitraums nicht zur MFA-Überprüfung aufgefordert. Daher ist bei Partnern, die MFA mithilfe der Azure AD-Sicherheitsstandards implementiert haben, damit zu rechnen, dass die Metriken die 100 % nicht erreichen.

### <a name="review-third-party-mfa-configurations"></a>Überprüfen der MFA-Konfigurationen von Drittanbietern

Wenn Sie eine MFA-Lösung eines Drittanbieters verwenden, bestimmen Sie, wie Sie diese in Azure AD integrieren. Im Allgemeinen gibt es zwei Methoden, einschließlich Partnerverbund und benutzerdefinierter Steuerelemente:

* **Identitätsverbund**: Wenn Azure AD eine Authentifizierungsanforderung empfängt, leitet Azure AD den Benutzer zur Authentifizierung an den Verbundidentitätsanbieter um. Bei erfolgreicher Authentifizierung leitet der Verbundidentitätsanbieter den Benutzer zusammen mit einem SAML-Token wieder an Azure AD weiter. Damit Azure AD erkennen kann, dass der Benutzer die MFA-Überprüfung bei seiner Authentifizierung beim Verbundidentitätsanbieter abgeschlossen hat, muss das SAML-Token den Anspruch *authenticationmethodsreferences* (mit dem Wert *multipleauthn*) enthalten. Überprüfen Sie, ob der Verbundidentitätsanbieter die Ausstellung eines solchen Anspruchs unterstützt. Ist dies der Fall, überprüfen Sie, ob der Verbundidentitätsanbieter entsprechend konfiguriert wurde. Wenn der Anspruch fehlt, liegen in Azure AD (und entsprechend auch im Partner Center) keine Informationen vor, dass der Benutzer die MFA-Überprüfung abgeschlossen hat, was dazu führen kann, dass die Metrik keine 100 % erreicht.

* **Benutzerdefiniertes Steuerelement**: Ein benutzerdefiniertes Azure AD-Steuerelement kann nicht verwendet werden, um zu ermitteln, ob ein Benutzer die MFA-Überprüfung über eine MFA-Lösung eines Drittanbieters abgeschlossen hat. Daher erscheint jeder Benutzer, der die MFA-Überprüfung mithilfe eines benutzerdefinierten Steuerelements abgeschlossen hat, für Azure AD (und in der Folge auch für das Partner Center) als mit nicht abgeschlossener MFA-Überprüfung angemeldet. Es empfiehlt sich, wo immer möglich dem Identitätsverbund bei der Integration in Azure Ad gegenüber benutzerdefinierten Steuerelementen den Vorzug zu geben.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifizieren der Benutzer, die sich ohne MFA beim Partner Center angemeldet haben

Es kann sinnvoll sein, zu identifizieren, welche Benutzer sich ohne MFA-Überprüfung beim Partner Center anmelden und sie mithilfe Ihrer aktuellen MFA-Implementierung zu überprüfen. Sie können den [Azure AD-Anmeldebericht](/azure/active-directory/reports-monitoring/concept-sign-ins) verwenden, um herauszufinden, ob ein Benutzer die MFA-Überprüfung abgeschlossen hat oder nicht. Der Azure AD-Anmeldebericht steht zurzeit nur Partnern zur Verfügung, die Azure AD Premium oder eine andere O365-SKU abonniert haben, die Azure AD Premium umfasst (beispielsweise EMS).

## <a name="next-steps"></a>Nächste Schritte

- [Partner Center security guidance group community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Sicherheitsanforderungen für Partner](partner-security-requirements.md)
- [Häufig gestellte Fragen (FAQ) zu den Sicherheitsanforderungen für Partner](partner-security-requirements-faq.md)
