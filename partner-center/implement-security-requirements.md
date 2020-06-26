---
title: Implementieren der Sicherheitsanforderungen für Partner
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die erforderlichen Sicherheitsanforderungen für Benutzer implementieren.
author: LauraBrenner
ms.author: labrenne
keywords: security
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133265"
---
# <a name="implement-the-partner-security-requirements"></a>Implementieren der Sicherheitsanforderungen für Partner

**Geeignete Rollen**

- Globaler Administrator

Sicherheit und Datenschutz von Kunden und Partnern besitzen für Microsoft oberste Priorität. Wir stellen immer mehr und immer ausgefeiltere Sicherheitsangriffe fest, insbesondere im Hinblick auf die Kompromittierung von Identitäten. Da präventive Maßnahmen in der Verteidigungsstrategie eine wichtige Rolle spielen, um Angriffe bereits im Vorfeld abzuwehren, beginnen wir damit, eine Reihe von obligatorischen Sicherheitsanforderungen durchzusetzen, die zum Schutz unserer Partner und deren Kunden beitragen.

In diesem Tutorial erfahren Sie mehr über die Sicherheitsanforderungen für Partner, deren Erfüllung und die Auswirkungen auf die Benutzer in Ihrem Partnerverzeichnis.

Alle Partner, die am Cloud Solution Provider-Programm teilnehmen, Systemsteuerungsanbieter oder Advisor-Partner sind verpflichtet, mehrstufige Authentifizierung (Multi-Factor Authentication, MFA) für jeden Benutzer in ihrem Partnermandanten durchzusetzen. Diese kann durch Aktivieren von zwei [Azure Active Directory-Baselinerichtlinien](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) erzwungen werden. Baselinerichtlinien sind eine Reihe von vordefinierten Richtlinien, die dabei helfen, Unternehmen vor vielen allgemeinen Angriffen zu schützen. Diese allgemeinen Angriffe können Password Spray, Replay und Phishing einbeziehen. Basisrichtlinien sind in allen Editionen von Azure Active Directory verfügbar. Microsoft stellt diese Basisschutzrichtlinien allen Benutzern zur Verfügung, weil identitätsbasierte Angriffe seit einigen Jahren zunehmen.

In den folgenden Verfahren wird beschrieben, wie Sie die beiden erforderlichen Basisrichtlinien aktivieren:

- **MFA für Administratoren erfordern** – Wenn Sie die Richtlinie „MFA für Administratoren erfordern“ aktivieren, müssen sich Benutzer in den Administratorrollen über die Authentifikator-App für MFA registrieren. Nachdem die MFA-Registrierung abgeschlossen ist, müssen Administratoren MFA bei jeder Anmeldung durchführen.

- **Endbenutzerschutz** – Der Endbenutzerschutz ist eine risikobasierte MFA-Baselinerichtlinie, die alle Benutzer in einem Verzeichnis schützt. Wenn Sie diese Richtlinie aktivieren, müssen sich alle Benutzer über die Authentifikator-App für MFA registrieren. Benutzer können die MFA-Registrierungsaufforderung 14 Tage lang ignorieren. Danach wird ihnen die Anmeldung verwehrt, bis sie sich für MFA registriert haben. Nach der Registrierung für MFA werden die Benutzer nur noch während risikobehafteter Anmeldeversuche zur MFA aufgefordert. Kompromittierte Benutzerkonten werden gesperrt, bis ihr Kennwort zurückgesetzt und Risikoereignisse abgewiesen wurden.

Sobald diese Richtlinien aktiviert sind, kann jeder Benutzer Azure MFA ohne zusätzliche Kosten nutzen. Wenn Sie eine Drittanbieterlösung verwenden, müssen Sie beim Zugriff auf kommerzielle Microsoft-Clouddienste MFA für jeden Benutzer erzwingen.

>[!NOTE]
>Da MFA für jeden Benutzer im Partnerverzeichnis erzwungen wird, hat dies Auswirkungen auf jede Automatisierung oder Integration, die Benutzeranmeldeinformationen verwendet. Um diese Auswirkungen zu berücksichtigen, müssen Sie die Methode ändern, durch die die Automatisierung oder Integration mit kommerziellen Clouddiensten von Microsoft verbunden wird. Wenn der Dienst, mit dem Sie eine Verbindung herstellen, die tokenbasierte Authentifizierung unterstützt, wird empfohlen, das Framework [Sicheres Anwendungsmodell](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) zu implementieren.

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>Schritt 1: Sperren aller vorhandenen Legacy-Authentifizierungsprotokolle

Bevor Sie die Richtlinien „MFA für Administratoren erfordern“ und „Endbenutzerschutz“ aktivieren, sollten Sie sicherstellen, dass die Benutzer keine Legacy-Authentifizierungsprotokolle verwenden. Weitere Informationen finden Sie im Artikel [Vorgehensweise: Blockieren der Legacyauthentifizierung bei Azure AD durch bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use).

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>Schritt 2: Aktivieren der Baselinerichtlinie „MFA für Administratoren erfordern“

Durch die Baselinerichtlinie „MFA für Administratoren erfordern“ wird MFA für die folgenden Verzeichnisrollen verpflichtend, die als die Azure AD-Rollen mit den höchsten Berechtigungen betrachtet werden:

- Globaler Administrator
- SharePoint-Administrator
- Exchange-Administrator
- Administrator für bedingten Zugriff
- Sicherheitsadministrator
- Helpdeskadministrator/Kennwortadministrator
- Rechnungsadministrator
- Benutzeradministrator

Beim Aktivieren der Richtlinie „MFA für Administratoren erfordern“ sind die obigen neun Administratorrollen für die Registrierung über die Authentifikator-App für MFA erforderlich. Nachdem die MFA-Registrierung abgeschlossen ist, müssen Administratoren bei jeder Anmeldung eine MFA durchführen.

Wenn diese Konten in Ihrem Unternehmen in Skripts oder Code verwendet werden, sollten Sie sie durch [verwaltete Identitäten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) ersetzen.

So aktivieren Sie diese Richtlinie und schützen Ihre Administratoren

1. Melden Sie sich beim  **Azure-Portal** als globaler Administrator, Sicherheitsadministrator oder Administrator für bedingten Zugriff an.

2. Navigieren Sie zu **Azure Active Directory** > **Bedingter Zugriff**.

3. Wählen Sie in der Liste der Richtlinien die Option **Baselinerichtlinie: MFA für Administratoren erfordern** aus.

4. Legen Sie **Richtlinie aktivieren** auf **Richtline sofort verwenden** fest.

5. Wählen Sie  **Speichern** aus.

Nachdem Sie diese Richtlinie aktiviert haben, werden Benutzer in den oben aufgeführten Administratorrollen bei der Anmeldung aufgefordert, zusätzliche Sicherheitsinformationen anzugeben und die mobile App zu konfigurieren. Danach können sie sich beim entsprechenden Clouddienst anmelden.

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>Schritt 3: Aktivieren der Baselinerichtlinie „Endbenutzerschutz“

Die Baselinerichtlinie für den Endbenutzerschutz schützt alle Benutzer in einem Verzeichnis. Wenn Sie diese Richtlinie aktivieren, müssen sich alle Benutzer innerhalb von 14 Tagen für Azure MFA registrieren. Nachdem Benutzer registriert sind, werden sie nur noch bei riskanten Anmeldeversuchen aufgefordert, MFA durchzuführen. Dieses Verhalten wird sich für Partnermandanten in Zukunft ändern. Kompromittierte Benutzerkonten werden bis zum Zurücksetzen des Kennworts gesperrt und riskieren eine Ablehnung.

Die Richtlinie „Baselinerichtlinie: Endbenutzerschutz“ ist vorkonfiguriert und wird ganz oben angezeigt, wenn Sie zum Blatt „Bedingter Zugriff“ im Azure-Portal navigieren.

So aktivieren Sie diese Richtlinie und schützen Ihre Benutzer

1. Melden Sie sich beim  **Azure-Portal** als globaler Administrator, Sicherheitsadministrator oder Administrator für bedingten Zugriff an.

2. Navigieren Sie zu **Azure Active Directory** > **Bedingter Zugriff**.

3. Wählen Sie in der Liste der Richtlinien die Option **Baselinerichtlinie: Endbenutzerschutz (Vorschau)** aus.

4. Legen Sie **Richtlinie aktivieren** auf **Richtline sofort verwenden** fest.

5. Wählen Sie  **Speichern** aus.

Nachdem Sie diese Richtlinie aktiviert haben, werden alle Benutzer bei der Anmeldung aufgefordert, zusätzliche Sicherheitsinformationen anzugeben und die mobile App zu konfigurieren. Danach können sie sich beim entsprechenden Clouddienst anmelden.

>[!NOTE]
>Bis die Sicherheitsanforderungen des Partners durchgesetzt werden, werden Benutzer, die nicht unter die Baselinerichtlinie „MFA für Administratoren erfordern“ fallen, nur im Falle eines Risikos aufgefordert, die MFA durchzuführen.