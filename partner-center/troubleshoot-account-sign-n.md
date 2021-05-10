---
title: Behandeln von Problemen beim Einrichten Ihres Partner Center-Kontos oder der MPN-Verlängerung
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Behandeln von Problemen beim Versuch, sich bei Partner Center zu registrieren. Antworten behandeln Herausforderungen bei Zahlungsmethoden, vergessenen Kennwörtern und mehr.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686261"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Behandeln von Problemen mit der Kontoeinrichtung oder MPN-Verlängerung


**Geeignete Rollen**

- Globaler Administrator
- MPN-Partneradministrator
 
Hier finden Sie einige Vorschläge zur Behandlung häufiger Probleme, die beim Einrichten Ihres Partner Center-Kontos auftreten.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Was geschieht, wenn Sie von Partner Membership Center migrieren und keine Unternehmensinformationsfelder bearbeiten können?

In Fällen, in denen Ihr Unternehmen bereits in Partner Center (z. B. einem CSP-Konto) vorhanden ist, wird ihnen ein schreibgeschützter Bildschirm angezeigt. Auf diesem Bildschirm werden alle Informationen zu Ihrem Unternehmen angezeigt, die in Partner Center vorhanden sind.

Sie können die Details auf diesem Bildschirm nicht ändern. Dies ist entwurfshalber und kein Fehler.

Wählen Sie **Akzeptieren** und **Fortfahren** aus, um den Vorgang fortzusetzen.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Wenn die IT-Abteilung die **Registrierung für Partner Center** deaktiviert hat

Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder die virale Registrierung auf dem Azure AD Mandanten deaktiviert ist. Der globale Administrator für Ihr Azure AD-Konto kann die erforderlichen Features aktivieren, indem er den folgenden PowerShell-Befehl ausführt:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Weitere Informationen finden Sie unter [Self-Service-Registrierung.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Sie haben Ihr Kennwort vergessen.

Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link Kann nicht auf **Ihr Konto zugreifen?** aus. Mit dieser Option können Sie Ihr Kennwort zurücksetzen oder Ihren globalen Administrator bitten, Ihnen neue Anmeldeinformationen zuzuweisen.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Auf dem Bildschirm "Informieren Sie uns über Ihr Unternehmen" wird der Fehler "Es ist etwas schief gelaufen" angezeigt.

Diese Fehlermeldung wird normalerweise angezeigt, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercodes in Ihrer Unternehmenstelefonnummer verwenden. Der im Feld Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Für Ihren Kreditkartenkauf wird eine Fehlermeldung mit dem Hinweis angezeigt, dass Ihre Bestellung abgelehnt wurde. Überprüfen Sie Ihre Informationen."


Verwenden Sie immer die Adresse, die Ihrer Kreditkarte und nicht Ihrer juristischen Person entspricht. Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Sie möchten von der Offlinezahlung zur Onlinezahlungsmethode wechseln. 

Sie müssen die ursprüngliche Bestellung und den ursprünglichen Wiederkauf mithilfe der bevorzugten Zahlungsmethode stornieren.

So stornieren Sie einen Auftrag:

1. Wählen Sie **im Dashboard die** Registerkarte Mitgliedschaftsangebote aus.

2. Wählen Sie **Bestellung stornieren aus.**

3. Ein Bestätigungsfenster wird angezeigt, und Sie müssen bestätigen, um die erste Bestellung zu stornieren.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten des Partner Center-Kontos](partner-center-account-setup.md)
- [Lesen Ihrer Rechnung und Abstimmungsdatei](read-your-bill.md)
