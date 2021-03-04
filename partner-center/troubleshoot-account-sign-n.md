---
title: Problembehandlung beim Einrichten Ihres Partner Center-Kontos oder der MPN-Erneuerungs Probleme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Beheben Sie Probleme bei der Registrierung beim Partner Center. Antworten behandeln Probleme mit Zahlungsmethoden, vergessen Kenn Wörter und vieles mehr.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9622f02039360e8ab39f459c9a2fe082ec70c854
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756737"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Behandeln von Problemen mit der Konto Einrichtung oder der MPN-Erneuerung


**Geeignete Rollen**

- Globaler Administrator
- MPN-Partneradministrator 
 
Hier finden Sie einige Vorschläge zur Problembehandlung bei häufigen Problemen, die beim Einrichten Ihres Partner Center-Kontos auftreten.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Was geschieht, wenn Sie vom Partner Mitgliedschafts Center migrieren und keine Firmen Informationsfelder bearbeiten können.

In Fällen, in denen Ihr Unternehmen bereits in Partner Center (z. –. CSP-Konto) vorhanden ist, wird Ihnen ein Schreib geschützter Bildschirm angezeigt. Auf diesem Bildschirm werden alle Informationen zu Ihrem Unternehmen angezeigt, so wie es im Partner Center vorhanden ist.

Die Details auf diesem Bildschirm können nicht geändert werden. Dies ist Entwurfs bedingt und kein Fehler.

Wählen Sie **annehmen** und **fort** fahren aus.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>, Wenn die IT-Abteilung die **Anmeldung für Partner Center** ausgeschaltet hat.

Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder wenn die virale Registrierung für den Azure AD Mandanten deaktiviert ist. Der globale Administrator für Ihr Azure AD Konto kann erforderliche Features aktivieren, indem Sie den folgenden PowerShell-Befehl ausführen:

**Set-msolcompanysettings-zustellwemailverifiedusers $true-allowadhocabonnements $true**

Weitere Informationen finden Sie [unter Self-Service](/azure/active-directory/users-groups-roles/directory-self-service-signup) -Registrierung.

## <a name="you-forgot-your-password"></a>Sie haben Ihr Kennwort vergessen.

Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link **kein Zugriff auf Ihr Konto?** aus. Mit dieser Option können Sie Ihr Kennwort zurücksetzen oder ihren globalen Administrator bitten, Ihnen neue Anmelde Informationen zuzuweisen.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Auf dem Bildschirm "erzählen Sie uns von Ihrem Unternehmen" erhalten Sie den Fehler "ein Fehler ist aufgetreten".

Diese Fehlermeldung wird normalerweise angezeigt, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercode in der Telefonnummer Ihres Unternehmens verwenden. Der im Feld für die Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Ihr Kreditkarten Erwerb erhält eine Fehlermeldung, die besagt, dass Ihre Bestellung abgelehnt wurde. Überprüfen Sie Ihre Informationen "


Verwenden Sie immer die Adresse, die Ihrer Kreditkarte entspricht, anstelle ihrer juristischen Person. Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Sie möchten von der Offline Zahlung zur Online Zahlungsmethode wechseln. 

Sie müssen die ursprüngliche Bestellung abbrechen und mithilfe der bevorzugten Zahlungsmethode erneut erwerben.

So brechen Sie eine Bestellung ab

1. Wählen Sie im Dashboard die Registerkarte **mitgliedschaftsangebote** aus.

2. Select- **Reihenfolge Abbrechen**

3. Es wird ein Bestätigungsfenster angezeigt, das Sie bestätigen müssen, um die anfängliche Reihenfolge abzubrechen.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten des Partner Center-Kontos](partner-center-account-setup.md)
- [So lesen Sie Ihre Rechnung und die Datei "Reconnaissance"](read-your-bill.md)
