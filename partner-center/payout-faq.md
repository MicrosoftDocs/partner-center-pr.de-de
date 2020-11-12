---
title: Häufig gestellte Fragen zu Auszahlungs Informationen zum kommerziellen Marketplace von Microsoft
description: Hier erhalten Sie Antworten auf häufig gestellte Fragen zu den Zahlungen im kommerziellen Marketplace. Hier finden Sie Antworten zu den Gründen, aus denen sich Ihre Einnahmen unterscheiden.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532020"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Häufige Fragen zu kommerziellen Marketplace-Auszahlungen

In diesem Artikel werden häufig gestellte Fragen zu Zahlungen im kommerziellen Marketplace beantwortet.

## <a name="earnings-incorrect-or-missing"></a>Das Ergebnis ist falsch oder fehlt.

#### <a name="why-are-my-earnings-missing"></a>Warum fehlen meine Einnahmen?

- Die Kundenbestellung verfügt unter Umständen noch nicht über die Berechtigung zur Auszahlung. Für nicht von Unternehmen stammende Kundenbestellungen muss Microsoft die Kundenzahlung erhalten haben, bevor dem Herausgeber die Einnahmen ausgezahlt werden können. Bei Kundenbestellungen von Unternehmen sind Ihre Einnahmen ein bis zwei Tage nach dem Datum der Bestellung verfügbar. Überprüfen Sie den Bestellstatus unter [Auftragsberichte](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Einnahmen für Transaktionen, die vor Juli 2019 durchgeführt wurden, werden im Bericht zum Transaktionsverlauf ggf. nicht angezeigt. Überprüfen Sie den Verlauf der Auszüge auf der [Downloadseite für Auszahlungen](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Überprüfen Sie den [Zeitrahmen des Auszahlungs Zyklen](payment-thresholds-methods-timeframes.md) , und verstehen Sie, wann Ihre Einnahmen in der Auszahlungs Anweisung angezeigt werden sollten.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Warum unterscheidet sich mein Ergebnis Betrag von dem, was ich erwartet habe?

- Wenn die Bestellung von Ihrem Kunden teilweise bezahlt wurde, basiert Ihr Erwerbs Betrag auf dem teilweise bezahlten Betrag nach der deduktionsgebühr und der entsprechenden Steuer.
- Überprüfen Sie die Zuständigkeit für Steuern nach Land. Für Länder/Regionen, in denen Microsoft für die Steuerzahlung zuständig ist, wird der Steuerbetrag von Microsoft berechnet und von den Einnahmen des Herausgebers abgezogen. Der Transaktionsbetrag im Auszug ist der Betrag nach Abzug der Steuer. Weitere Informationen finden Sie unter [Steuerliche Aspekte für kommerzielle Marketplace-Herausgeber](tax-details-marketplace.md).
- SaaS-und IaaS-Angebote verfügen über eine reduzierte gebührengebühr von 10% anstelle der standardmäßigen 20%. Dies hat eine Gewinnquote von 90%. Dieses Angebot gilt bis zum 30. Juni 2021.

**Weitere** Informationen: [kommerzieller Marketplace-Herausgeber Vertrag](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details zu Auszahlungs Richtlinien](payout-policy-details.md), [Zahlungs Schwellenwert, Methode und Zeitrahmen](payment-thresholds-methods-timeframes.md), [kostenpflichtig im kommerziellen Marketplace](marketplace-get-paid.md), [Steuer Details](tax-details-marketplace.md), [Auszahlungs Anweisungen](payout-statement.md), [Bestell Dashboard in kommerziellen Marketplace Analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Einnahmenabgleich
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Wie kann ich Auszahlungsauszüge mit Auftrags- oder Nutzungsberichten in Analysen abgleichen?
Verwenden Sie assetid, OrderID und die Zeilen Element-ID, die im Bericht "Auszahlungs Transaktionsverlauf" mit analytischen Aufträgen und Verwendungs Berichten angezeigt werden. Verwenden Sie diese Zuordnung:

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Wann kann ich mit Zahlungen für meine Kundenbestellungen rechnen?
- Überprüfen Sie zunächst mithilfe ihrer assetid Kunden Bestellungen in [Auftrags Berichten](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Überprüfen Sie den kundenkanal für Ihr Kunden Abonnement im [Bericht "Kunden](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)".
- Für Unternehmenskunden wird der Verleger Gewinn in der Anweisung 1-2 Tage nach dem Bestelldatum angezeigt.
- Für Kunden, die keine Enterprise-Kunden sind, wird der Verleger Gewinn in der Anweisung 1-2 Tage nach Erhalt der Kundenzahlung angezeigt.

**Weitere** Informationen: [Auszahlungs Anweisungen](payout-statement.md), [Bestell Dashboard in kommerzieller Marketplace Analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Auszahlungsrichtlinien

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Wie kann ich die aktuelle Agenturgebühr und die Auszahlungsrate ermitteln?

- Sehen Sie in der Herausgebervereinbarung für den kommerziellen Marketplace nach. Standardmäßig hat die Agenturgebühr eine Höhe von 20 %. Die für SaaS Co-Sell berechtigten Transaktionen haben eine reduzierte Gebühr von 10%. Achten Sie auf Ankündigungen zu Angeboten in Bezug auf die Agenturgebühr.
- In ihrer Auszahlungs Anweisung gibt die Erwerbs Rate die tatsächliche Auszahlungsrate für eine bestimmte Transaktion an.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Wann kann ich eine Zahlung von Microsoft erwarten, nachdem in meinem Auszug Einnahmen angezeigt werden?
- Wenn Ihre Einnahmen den Status „Nicht verarbeitet“ aufweisen, können Sie das Datum der Auszahlungsbereitschaft für den Monat überprüfen, in dem Ihre Einnahmen für die Zahlung verarbeitet werden. Sobald Ihre Zahlung vorbereitet ist, ändert sich der Status ihres Erwerbs in "verarbeitet".  Microsoft gibt die Zahlungen jeweils am 15. des Monats frei, in dem diese die Auszahlungsbereitschaft erreichen.
- Bei Bestellungen, die per Kreditkarte gezahlt werden, hält Microsoft 30 Tage lang Zahlungen, bis der Erwerb ausgereift ist.

 **Weitere** Informationen: [kommerzielle Marketplace-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details zu Auszahlungs Richtlinien](payout-policy-details.md), [Steuer Details](tax-details-marketplace.md), [Zahlungs Schwellenwert, Methode und Zeitrahmen](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Zahlungen und Anpassungen

#### <a name="why-is-my-payment-missing"></a>Warum fehlt meine Zahlung?

- Stellen Sie sicher, dass der Auszahlungsstatus und der Status des Steuer Profils auf der [Übersichtsseite](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)als *gültig* angezeigt werden.
- Unter Umständen haben Sie den Mindestwert für eine Zahlung nicht erreicht. Einnahmen müssen mindestens eine Höhe von 50 US-Dollar haben, damit Sie eine Zahlung erhalten können.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Gewusst wie mein Konto so einrichten, dass es keine Zahlung erhält?
Sie können Zahlungen im [Auszahlungs Profil](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)speichern. Aktivieren Sie einfach **halten**. Microsoft hält sich an Sie, bis Sie den Halt freigeben.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Warum erhalte ich die Zahlung in einer anderen Währung als der beim Kauf verwendeten Währung?

Die Währung der Auszahlung basiert auf der Währung, die Sie im Auszahlungsprofil ausgewählt haben. Die Währung des Kaufs basiert auf der Währung, in der der Kunde die Zahlung geleistet hat.

#### <a name="how-do-i-reconcile-adjustments"></a>Wie kann ich Anpassungen abstimmen?

Bei Zahlungsanpassungen handelt es sich um Korrekturen von Zahlungen, um beispielsweise bei Systemproblemen einen Ausgleich vornehmen zu können. Im Auszahlungsauszug ist der Grund für die Anpassung (ReasonCode) angegeben. Dies ist nicht auf die direkte Abstimmung einzelner Transaktionen bezogen.

**Weitere** Informationen: [kommerzielle Marketplace-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details zu Auszahlungs Richtlinien](payout-policy-details.md), [Steuer Details](tax-details-marketplace.md), [Zahlungs Schwellenwert, Methode und Zeitrahmen](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Steuern

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Wie können wir anhand des Auszahlungsauszugs die Steuerzahlungszuständigkeit (Microsoft oder Herausgeber) ermitteln?

Suchen Sie im heruntergeladenen Transaktionsverlauf nach der Spalte für das Steuermodell. Dort sehen Sie, ob die Verwaltung durch Microsoft oder durch den unabhängigen Softwarehersteller erfolgt. Länderspezifische Steuerregeln und Auswirkungen auf die Auszahlung finden Sie in den [Steuerdetails](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Wie kann ich Formulare für die Steuer auf Servicegebühren herunterladen?

Navigieren Sie auf der Seite für die Auszahlungszahlung zum Bereich mit der Zahlungsliste.  Für Zahlungen mit Steuer auf Servicegebühren wird ein Link zum entsprechenden Steuerformular angezeigt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Wie kann ich ein Formular für die Quellensteuer als PDF herunterladen?

Navigieren Sie auf der Seite für die Auszahlungszahlung zum Bereich mit der Zahlungsliste.  Neben einer Zahlung wird ein Link zu einem Quellensteuerformular angezeigt.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Wo finde ich die Steuerformulare für das Jahresende?

Navigieren Sie zur [Profilseite](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage), um die Steuerformulare für das Jahresende anzuzeigen.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Wo finde ich die Quellensteuer für eine Transaktion?
Die Quellensteuer ist für US-amerikanische Herausgeber relevant, die ein W-9-Formular eingereicht haben. Die Quellensteuer wird für eine monatliche Zahlung berechnet.

**Weitere** Informationen: [kommerzielle Marketplace-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Auszahlungs Richtlinien Details](payout-policy-details.md)

## <a name="payout-statement-access"></a>Zugriff auf die Auszahlungs Anweisung

#### <a name="how-do-i-access-a-payout-statement"></a>Wie kann ich auf einen Auszahlungsauszug zugreifen?

1. Überprüfen Sie Ihre Rollen. Für den Zugriff auf den Auszahlungsauszug müssen Sie über die Rolle *Mitwirkender im Finanzbereich* oder *Kontobesitzer* verfügen.
2. Wählen Sie in der Navigationsleiste oben rechts das **Auszahlungs** Symbol aus, um Ihre Auszahlungs Anweisung anzuzeigen. Wählen Sie einen **Transaktionsverlauf** , eine **Zahlung** und einen **Download** aus.

**Weitere** Informationen: [Auszahlungs Rollen und-Berechtigungen](payout-statement.md#roles-and-permissions), [Auszahlungs Anweisungen](payout-statement.md) 

## <a name="payout-statement-report"></a>Bericht zur Auszahlungs Anweisung

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Was bedeuten die einzelnen Felder im Download des Transaktionsverlaufs?

Eine ausführliche Liste der Attribute und ihrer Bedeutungen finden Sie unter [Auszahlungs Anweisungen](payout-statement.md) .

#### <a name="what-is-earning-status"></a>Was ist der Einnahmenstatus?

Dadurch wird Ihr Ergebnis als nicht verarbeitet, verarbeitet oder gesendet angezeigt.

- **Nicht verarbeitete** –-Einnahmen liegen in einem Hinterlegungs Zeitraum bis zum Fälligkeitsdatum.
- **Verarbeitete** – Einnahmen sind gereift und werden auf eine monatliche Zahlung vorbereitet. Zahlungen werden jeweils 15. jeden Monats veröffentlicht.
- **Gesendet** – die Zahlung wurde basierend auf Ihrem Auszahlungs Profil erfolgreich auf Ihrer Bank veröffentlicht.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Wie kann ich Formulare für die Steuer auf Servicegebühren herunterladen?

Navigieren Sie auf der Seite für die Auszahlungszahlung zum Bereich mit der Zahlungsliste.  Für Zahlungen mit Steuer auf Servicegebühren wird ein Link zum entsprechenden Steuerformular angezeigt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Gewusst wie ein Steuerformular für die Zurückhaltung in PDF herunterladen?

Navigieren Sie auf der Seite für die Auszahlungszahlung zum Bereich mit der Zahlungsliste.  Neben einer Zahlung wird ein Link zu einem Quellensteuerformular angezeigt.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Wo finde ich die Steuerformulare für das Jahresende?

Navigieren Sie zur [Profilseite](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage), um die Steuerformulare für das Jahresende anzuzeigen.

**Weitere** Informationen: [Auszahlungs Anweisungen](payout-statement.md), [Download für den Transaktionsverlauf](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historische Auszüge

#### <a name="how-do-i-view-historical-information"></a>Gewusst wie Anzeigen von Verlaufs Informationen?

Der historische Auszug zeigt die Momentaufnahme der Auszahlungsdaten von Oktober 2019. Die hier aufgeführten Auszahlungs Informationen werden leider nicht aktualisiert. Um die neuesten Informationen zu erhalten, übermitteln Sie ein Support Ticket für die neuesten Daten.

**Weitere** Informationen: [Auszahlungs Anweisungen](payout-statement.md), [Download für den Transaktionsverlauf](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Auszahlungs Export-API

#### <a name="how-do-i-download-payout-data"></a>Wie lade ich Auszahlungsdaten herunter?

Verwenden Sie die [Partner-Auszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Nächste Schritte

- [Zahlungserhalt im kommerziellen Marketplace](marketplace-get-paid.md)
