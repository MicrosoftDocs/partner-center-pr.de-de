---
title: Behandeln von Problemen beim Einrichten Ihres Partner Center kontos oder der MPN-Verlängerung
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Behandeln von Problemen beim Versuch, sich bei einem Partner Center. Antworten auf Herausforderungen bei Zahlungsmethoden, das Vergessen von Kennwörtern und mehr.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854688"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Behandeln von Problemen bei der Kontoeinrichtung oder MPN-Verlängerung

**Geeignete Rollen:** Globale Administratorrechte | MPN-Partneradministrator
 
Hier finden Sie einige Vorschläge zur Behandlung häufiger Probleme, die beim Einrichten Ihres Kontos Partner Center auftreten.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Was geschieht, wenn Sie von einem Partner Membership Center und keine Felder für Unternehmensinformationen bearbeiten können?

In Fällen, in denen Ihr Unternehmen bereits in Partner Center ist (z. B. ein CSP-Konto), wird ein schreibgeschützter Bildschirm angezeigt. Auf diesem Bildschirm werden alle Informationen zu Ihrem Unternehmen angezeigt, wie es in der Partner Center.

Sie können die Details auf diesem Bildschirm nicht ändern. Dies ist entwurfsweise und kein Fehler.

Wählen Sie **Akzeptieren** und **Fortfahren aus,** um fortzufahren.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Wenn die IT-Abteilung die Anmeldung für die **Partner Center**

Diese Meldung wird angezeigt, weil virale Benutzer deaktiviert sind oder weil die virale Anmeldung auf dem Azure AD ist. Der globale Administrator für Ihr Azure AD-Konto kann erforderliche Features aktivieren, indem er den folgenden PowerShell-Befehl ausführen:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Weitere Informationen finden Sie unter [Self-Service-Anmeldung.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Sie haben Ihr Kennwort vergessen.

Wenn Sie Ihr Kennwort vergessen haben, wählen Sie auf der Anmeldeseite den Link Kann nicht auf Ihr Konto **zugreifen?** aus. Mit dieser Option können Sie Ihr Kennwort zurücksetzen oder Ihren globalen Administrator bitten, Ihnen neue Anmeldeinformationen zu zuweisen.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Auf dem Bildschirm "Informieren Sie uns über Ihr Unternehmen" wird der Fehler "Es ist etwas schief gelaufen" angezeigt.

Diese Fehlermeldung wird in der Regel angezeigt, wenn Sie versehentlich Sonderzeichen, Leerzeichen oder Ländercode in der Telefonnummer Ihres Unternehmens verwenden. Der im Feld Telefonnummer eingegebene Wert darf nur maximal 10 Zeichen enthalten.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Ihr Kreditkartenkauf erhält eine Fehlermeldung mit dem Hinweis, dass Ihre Bestellung abgelehnt wurde. Überprüfen Sie Ihre Informationen."


Verwenden Sie immer die Adresse, die Ihrer Kreditkarte und nicht Ihrer juristischen Person entspricht. Stellen Sie außerdem sicher, dass die Postleitzahl korrekt ist und der von Ihnen verwendeten Adresse entspricht.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Sie möchten von der Offlinezahlung zur Onlinezahlungsmethode wechseln. 

Sie müssen die ursprüngliche Bestellung stornieren und mit der bevorzugten Zahlungsmethode erneut ankaufen.

So brechen Sie einen Auftrag ab:

1. Wählen Sie im Dashboard die Registerkarte **Mitgliedschaftsangebote** aus.

2. Wählen Sie **Auftrag stornieren aus.**

3. Ein Bestätigungsfenster wird angezeigt, und Sie müssen dies bestätigen, um die ursprüngliche Bestellung abzubrechen.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten des Partner Center-Kontos](partner-center-account-setup.md)
- [Lesen Ihrer Rechnung und Abstimmungsdatei](read-your-bill.md)
