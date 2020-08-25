---
title: Problembehandlung beim Einrichten Ihres Partner Center-Kontos oder der MPN-Erneuerungs Probleme
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Beheben von Problemen bei der Anmeldung in Partner Center
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848934"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Behandeln von Problemen mit der Konto Einrichtung oder der MPN-Erneuerung

### <a name="applies-to"></a>Gilt für:

- Partner Center
 
### <a name="appropriate-roles"></a>Geeignete Rollen

- Globaler Administrator
- MPN-Partneradministrator 
 

Hier finden Sie einige Vorschläge zur Problembehandlung bei häufigen Problemen, die beim Einrichten Ihres Partner Center-Kontos auftreten.

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Was geschieht, wenn Sie vom Partner Mitgliedschafts Center migrieren und keine Firmen Informationsfelder bearbeiten können.

Dies tritt auf, wenn Ihr Unternehmen bereits in Partner Center (z. –. CSP-Konto) vorhanden ist Ihnen wird ein Schreib geschützter Bildschirm angezeigt, auf dem alle Informationen zu Ihrem Unternehmen angezeigt werden, wie es im Partner Center vorhanden ist.

Die Details auf diesem Bildschirm können nicht geändert werden. Dies ist Entwurfs bedingt und kein Fehler.

Wählen Sie **annehmen** und **fort** fahren aus.

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Sie versuchen, sich zu registrieren oder aus dem Partner Membership Center zu migrieren, und Sie erhalten eine Fehlermeldung, die besagt, dass die IT-Abteilung die Registrierung **für Partner Center**ausgeschaltet hat. 

Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder die virale Registrierung für den Azure AD Mandanten deaktiviert ist. Der globale Administrator für Ihr Azure AD Konto kann erforderliche Features aktivieren, indem Sie den folgenden PowerShell-Befehl ausführen:

**Set-msolcompanysettings-zustellwemailverifiedusers $true-allowadhocabonnements $true**

Weitere Informationen finden Sie [unter Self-Service](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) -Registrierung.

### <a name="you-forgot-your-password"></a>Sie haben Ihr Kennwort vergessen.

Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link **kein Zugriff auf Ihr Konto?** aus, um Ihr Kennwort zurückzusetzen, oder bitten Sie Ihren globalen Administrator, Ihnen neue Anmelde Informationen zuzuweisen.

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Auf dem Bildschirm "erzählen Sie uns von Ihrem Unternehmen" erhalten Sie den Fehler "ein Fehler ist aufgetreten".

Dies geschieht normalerweise, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercode in der Telefonnummer Ihres Unternehmens verwenden. Der im Feld für die Telefonnummer eingegebene Wert darf maximal 10 Zeichen enthalten.

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Sie versuchen, den Kauf über die Kreditkarte abzuschließen, aber Sie erhalten eine Fehlermeldung mit dem Hinweis, dass die Bestellung abgelehnt wurde. Überprüfen Sie Ihre Informationen "

Sie sollten immer die Adresse Ihrer Kreditkarte einfügen, die ihrer juristischen Person nicht entspricht. Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Sie möchten von der Offline Zahlung zur Online Zahlungsmethode wechseln. 

Sie müssen die ursprüngliche Bestellung abbrechen und mithilfe der bevorzugten Zahlungsmethode erneut erwerben.

So brechen Sie eine Bestellung ab

1. Wählen Sie im Dashboard die Registerkarte **mitgliedschaftsangebote** aus.

2. Select- **Reihenfolge Abbrechen**

3. Es wird ein Bestätigungsfenster angezeigt, das Sie bestätigen müssen, um die anfängliche Reihenfolge abzubrechen.
