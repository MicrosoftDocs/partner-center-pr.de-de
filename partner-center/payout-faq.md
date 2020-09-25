---
title: Häufig gestellte Fragen zu Auszahlungs Informationen zum kommerziellen Marketplace von Microsoft
description: Hier erhalten Sie Antworten auf häufig gestellte Fragen zu den Zahlungen im kommerziellen Marketplace.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335702"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Häufige Fragen zu kommerziellen Marketplace-Auszahlungen

In diesem Artikel werden häufig gestellte Fragen zu Zahlungen im kommerziellen Marketplace beantwortet.

## <a name="earnings-incorrect-or-missing"></a>Das Ergebnis ist falsch oder fehlt.

#### <a name="why-are-my-earnings-missing"></a>Warum fehlt mein Ergebnis?

- Die Kundenbestellung ist möglicherweise noch nicht für die Auszahlung berechtigt. Für nicht-Enterprise-Kunden Bestellungen muss Microsoft Kunden Zahlungen erhalten, bevor der Erwerb des Verlegers infrage kommt. Für Enterprise-Kunden Bestellungen ist Ihr Gewinn 1-2 Tage nach dem Bestelldatum verfügbar. Überprüfen Sie den Bestellstatus in [Auftrags Berichte](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Das Ergebnis der Transaktionen vor dem 2019. Juli kann im Transaktions Verlaufs Bericht nicht angezeigt werden. Überprüfen Sie die Verlaufs Anweisungen im [Auszahlungs Download](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Überprüfen Sie den [Zeitrahmen des Auszahlungs Zyklen](payment-thresholds-methods-timeframes.md) , und verstehen Sie, wann Ihre Einnahmen in der Auszahlungs Anweisung angezeigt werden sollten.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Warum unterscheidet sich mein Ergebnis Betrag von dem, was ich erwartet habe?

- Wenn die Bestellung von Ihrem Kunden teilweise bezahlt wurde, basiert Ihr Erwerbs Betrag auf dem teilweise bezahlten Betrag nach der deduktionsgebühr und der entsprechenden Steuer.
- Überprüfen Sie die Zuständigkeit für Steuern nach Land. Im Fall von Ländern, in denen die Steuern von Microsoft Verantwortlichkeit sind, sammelt und leitet Microsoft die Steuern der Erlöse des Herausgebers. Der in der Anweisung angezeigte Transaktionsbetrag liegt nach dem Steuerbetrag. Siehe [Steuer Details](tax-details-marketplace.md).
- SaaS-und IaaS-Angebote verfügen über eine reduzierte gebührengebühr von 10% anstelle der standardmäßigen 20%. Dies hat eine Gewinnquote von 90%. Diese herauf Stufung gilt bis zum 30. Juni 2021.

**Weitere**Informationen: [kommerzieller Marketplace-Herausgeber Vertrag](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details zu Auszahlungs Richtlinien](payout-policy-details.md), [Zahlungs Schwellenwert, Methode und Zeitrahmen](payment-thresholds-methods-timeframes.md), [kostenpflichtig im kommerziellen Marketplace](marketplace-get-paid.md), [Steuer Details](tax-details-marketplace.md), [Auszahlungs Anweisungen](payout-statement.md), [Bestell Dashboard in kommerziellen Marketplace Analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Einnahmenabgleich
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Gewusst wie abstimmen von Auszahlungs Anweisungen mit Bestell-oder Verwendungs Berichten in Analytics?
Verwenden Sie assetid, OrderID und die Zeilen Element-ID, die im Bericht "Auszahlungs Transaktionsverlauf" mit analytischen Aufträgen und Verwendungs Berichten angezeigt werden. Verwenden Sie diese Zuordnung:

- Auszahlungs Transaktionsverlauf. assetid = Order. OrderID
- Auszahlungs Transaktionsverlauf. OrderID & LineItem = Usage. Befehlszeilen-ID [OrderID: lineitemid]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Gewusst wie wissen, wann die Zahlungen für meine Kunden Bestellungen zu erwarten sind?
- Überprüfen Sie zunächst mithilfe ihrer assetid Kunden Bestellungen in [Auftrags Berichten](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Überprüfen Sie den kundenkanal für Ihr Kunden Abonnement im [Bericht "Kunden](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)".
- Für Unternehmenskunden wird der Verleger Gewinn in der Anweisung 1-2 Tage nach dem Bestelldatum angezeigt.
- Für Kunden, die keine Enterprise-Kunden sind, wird der Verleger Gewinn in der Anweisung 1-2 Tage nach Erhalt der Kundenzahlung angezeigt.

**Weitere**Informationen: [Auszahlungs Anweisungen](payout-statement.md), [Bestell Dashboard in kommerzieller Marketplace Analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Auszahlungs Richtlinien

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Gewusst wie die aktuelle Agenturgebühr und die Auszahlungsrate zu finden?

- Überprüfen Sie den kommerziellen Marketplace-Herausgeber Vertrag. Die Standard-Amt-Gebühr beträgt 20%. Der SaaS-Co-Selling für berechtigte Transaktionen hat eine reduzierte Gebühr von 10%. Überprüfen Sie, ob Ankündigungen zu den Gebühren einer Werbe Behörde vorliegen.
- In ihrer Auszahlungs Anweisung gibt die Erwerbs Rate die tatsächliche Auszahlungsrate für eine bestimmte Transaktion an.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Wann kann ich eine Zahlung von Microsoft erwarten, sobald die Einnahmen in meiner Erklärung angezeigt werden?
- Sobald Ihr Erwerb den Status "nicht verarbeitet" hat, können Sie das Fälligkeitsdatum für den Monat überprüfen, in dem Ihre Einnahmen für die Zahlung verarbeitet werden. Sobald Ihre Zahlung vorbereitet ist, ändert sich der Status ihres Erwerbs in "verarbeitet".  Microsoft gibt Zahlungen bis zum 15. Reife Monat frei.
- Bei Bestellungen, die per Kreditkarte gezahlt werden, hält Microsoft 30 Tage lang Zahlungen, bis der Erwerb ausgereift ist.

 **Weitere**Informationen: [kommerzielle Marketplace-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details zu Auszahlungs Richtlinien](payout-policy-details.md), [Steuer Details](tax-details-marketplace.md), [Zahlungs Schwellenwert, Methode und Zeitrahmen](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Zahlungen und Anpassungen

#### <a name="why-is-my-payment-missing"></a>Warum fehlt meine Zahlung?

- Stellen Sie sicher, dass der Auszahlungsstatus und der Status des Steuer Profils auf der [Übersichtsseite](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)als *gültig* angezeigt werden.
- Möglicherweise haben Sie den minimalen Schwellenwert für eine Zahlung nicht erreicht. Der Gewinn muss mindestens $50 USD betragen, um eine Zahlung zu erhalten.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Gewusst wie mein Konto so einrichten, dass es keine Zahlung erhält?
Sie können Zahlungen im [Auszahlungs Profil](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)speichern. Aktivieren Sie einfach **halten**. Microsoft hält sich an Sie, bis Sie den Halt freigeben.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Warum erhalte ich eine andere Währung als die Kauf Währung?

Die Auszahlungs Währung basiert auf der Währung, die Sie im Auszahlungs Profil ausgewählt haben. Die Erwerbs Währung basiert auf der Währung, die der Kunde bezahlt hat.

#### <a name="how-do-i-reconcile-adjustments"></a>Gewusst wie Anpassungen abstimmen?

Zahlungs Anpassungen sind Zahlungs Korrekturen, um ausgleichende Anpassungen wie z. b. System Probleme zu ermöglichen. In der Auszahlungs Anweisung gibt reasoncode den Grund für die Anpassung an. Diese sollen nicht direkt mit einzelnen Transaktionen abgestimmt werden.

**Weitere**Informationen: [kommerzielle Marketplace-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details zu Auszahlungs Richtlinien](payout-policy-details.md), [Steuer Details](tax-details-marketplace.md), [Zahlungs Schwellenwert, Methode und Zeitrahmen](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Steuern

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Wie identifizieren wir die Verantwortung für die Steueraufgaben zwischen Microsoft oder Publisher in der Auszahlungs Erklärung?

Suchen Sie unter Transaktionsverlauf herunterladen die Spalte Steuermodell. Dies zeigt, dass MS verwaltet oder ISV verwaltet wird. Siehe länderspezifische Steuerregeln und Auszahlungs Implikationen in den [Steuer Details](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Gewusst wie kostenpflichtige Steuerformulare für die Dienstgebühr herunterladen?

Wechseln Sie zur Seite **Auszahlungs Zahlung** , und klicken Sie dann auf die **Liste mit den Zahlungen** . Ein Link zum Steuerformular für die Dienstgebühr wird für eine Zahlung mit der Gebühr für die Dienstgebühr angezeigt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Gewusst wie ein Steuerformular für die Zurückhaltung in PDF herunterladen?

Wechseln Sie zur Seite *Auszahlungs Zahlung* , und klicken Sie dann auf die **Liste mit den Zahlungen** . Neben einer Zahlung wird ein Link zu einer Form vom Typ "zurück Haltungs Steuer" angezeigt.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Wo finde ich die Steuerformulare für das Ende des Jahres?

Wechseln Sie zur [Seite Profil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) , um die Steuerformulare für das Jahresende anzuzeigen.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Gewusst wie die Verweil Steuer für eine Transaktion zu finden?
Das zurückbehalten von Steuern gilt für US-Verleger, die ein W-9-Formular eingereicht haben. Das zurückbehalten von Steuern wird bei einer monatlichen Zahlung berechnet.

**Weitere**Informationen: [kommerzielle Marketplace-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Auszahlungs Richtlinien Details](payout-policy-details.md)

## <a name="payout-statement-access"></a>Zugriff auf die Auszahlungs Anweisung

#### <a name="how-do-i-access-a-payout-statement"></a>Gewusst wie auf eine Auszahlungs Anweisung zugreifen?

1. Überprüfen Sie Ihre Rollen. Für den Zugriff auf die Auszahlungs Anweisung müssen Sie über die Rolle " *Mitwirkender* " oder " *Konto Besitzer* " verfügen
2. Wählen Sie in der Navigationsleiste oben rechts das **Auszahlungs** Symbol aus, um Ihre Auszahlungs Anweisung anzuzeigen. Wählen Sie einen **Transaktionsverlauf**, eine **Zahlung**und einen **Download**aus.

**Weitere**Informationen: [Auszahlungs Rollen und-Berechtigungen](payout-statement.md#roles-and-permissions), [Auszahlungs Anweisungen](payout-statement.md) 

## <a name="payout-statement-report"></a>Bericht zur Auszahlungs Anweisung

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Was bedeuten die einzelnen Felder im Transaktions Download?

Eine ausführliche Liste der Attribute und ihrer Bedeutungen finden Sie unter [Auszahlungs Anweisungen](payout-statement.md) .

#### <a name="what-is-earning-status"></a>Was ist der Erwerbsstatus?

Dadurch wird Ihr Ergebnis als nicht verarbeitet, verarbeitet oder gesendet angezeigt.

- **Nicht verarbeitete** –-Einnahmen liegen in einem Hinterlegungs Zeitraum bis zum Fälligkeitsdatum.
- **Verarbeitete** – Einnahmen sind gereift und werden auf eine monatliche Zahlung vorbereitet. Zahlungen werden jeweils 15. jeden Monats veröffentlicht.
- **Gesendet** – die Zahlung wurde basierend auf Ihrem Auszahlungs Profil erfolgreich auf Ihrer Bank veröffentlicht.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Gewusst wie kostenpflichtige Steuerformulare für die Dienstgebühr herunterladen?

Wechseln Sie zur Seite **Auszahlungs Zahlung** , und klicken Sie dann auf die **Liste mit den Zahlungen** . Ein Link zum Steuerformular für die Dienstgebühr wird für eine Zahlung mit der Gebühr für die Dienstgebühr angezeigt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Gewusst wie ein Steuerformular für die Zurückhaltung in PDF herunterladen?

Wechseln Sie zur Seite **Auszahlungs Zahlung** , und klicken Sie dann auf die **Liste mit den Zahlungen** . Neben einer Zahlung wird ein Link zu einer Form vom Typ "zurück Haltungs Steuer" angezeigt.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Wo finde ich die Steuerformulare für das Ende des Jahres?

Wechseln Sie zur [Seite Profil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) , um die Steuerformulare für das Jahresende anzuzeigen.

**Weitere**Informationen: [Auszahlungs Anweisungen](payout-statement.md), [Download für den Transaktionsverlauf](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historische Auszüge

#### <a name="how-do-i-view-historical-information"></a>Gewusst wie Anzeigen von Verlaufs Informationen?

Die historische Anweisung zeigt die Momentaufnahme der Auszahlungs Daten ab dem Oktober 2019 an. Die hier aufgeführten Auszahlungs Informationen werden leider nicht aktualisiert. Um die neuesten Informationen zu erhalten, übermitteln Sie ein Support Ticket für die neuesten Daten.

**Weitere**Informationen: [Auszahlungs Anweisungen](payout-statement.md), [Download für den Transaktionsverlauf](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Auszahlungs Export-API

#### <a name="how-do-i-download-payout-data"></a>Gewusst wie Auszahlungs Daten herunterladen?

Verwenden Sie die [Partner-Auszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Nächste Schritte

- [Zahlungserhalt im kommerziellen Marketplace](marketplace-get-paid.md)
