---
title: Details zu Auszahlungs Richtlinien-Microsoft Commercial Marketplace
description: Details zu kommerziellen Marketplace-Auszahlungs Richtlinien, einschließlich Zeitpläne und neuausladung.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 04/24/2020
ms.openlocfilehash: 17fedcf4ef3d474eab679a03eecb221c90342a04
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335703"
---
# <a name="payout-policy-details"></a>Auszahlungsrichtliniendetails

Dieser Artikel erläutert den Auszahlungsprozess von Microsoft, den auszahlungszeitplan und die Richtlinie für die Wiederaufnahme sowie den Ort, an dem der Status einer Auszahlung zu finden ist.

## <a name="where-to-find-upcoming-payouts"></a>Ort für bevorstehende Auszahlungen

Wählen Sie in Partner Center das **Auszahlungs** Symbol in der oberen rechten Ecke des Bildschirms aus:

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Auszahlungssymbol rechts oben im Partner Center-Portal":::

> [!TIP]
> Nicht alle Kontorollen haben Zugriff auf Auszahlungsinformationen. Weitere Informationen finden Sie unter [Rollen und Berechtigungen](payout-statement.md#roles-and-permissions).

## <a name="payment-schedules"></a>Zahlungspläne

In den folgenden Abschnitten wird der Prozess für Auszahlungen beschrieben.

### <a name="enterprise-agreement-transactions-after-may-1-2020"></a>Enterprise Agreement-Transaktionen nach dem 1. Mai 2020

Wir haben das folgende Update für unser kommerzielles Marketplace-Herausgeber Auszahlungs Modell durchgeführt:

Ab dem 1. Mai 2020 aktualisieren wir unsere Auszahlungs Richtlinie im Zusammenhang mit Produkten, die in Microsoft AppSource erworben wurden oder von Kunden mit einem Microsoft-Konzernvertrag Azure Marketplace werden. Wenn ein Kunde ein Produkt von Azure Marketplace oder appsource mithilfe der vorhandenen Microsoft-Konzernvertrag für Transaktionen kauft, beginnen wir nach dem 1. Mai 2020, im nächsten Auszahlungs Zeitraum 30 Tage nach Kunden Rechnung Zahlungen auszugeben. Für Transaktionen, bei denen der Kunde eine Kreditkarte verwendet, gilt unverändert ein Einbehaltungszeitraum von 30 Tagen vor der Auszahlung. In dieser Tabelle werden Details zum auszahlungszeitplan angezeigt.

> [!NOTE]
> Unter [Prozess bei Nichtzahlung des Kunden](#process-for-customer-non-payment) erfahren Sie, welche Maßnahmen wir ergreifen, wenn der Kunde nicht bezahlt und wir bereits eine Auszahlung an Sie geleistet haben.

| Ereignis  | Datum (UTC) | Partnersichtbarkeit: Partner Center-Auszahlungsbericht  |  Partnersichtbarkeit: Partner Center-Analysen\* |
| --- | --- | --- | --- |
| Transaktion oder Nutzungsmonat | 01.08.2020–31.08.2020 | – | **Nutzungsbericht**: Anzeige des neuen Verbrauchs (wird alle vier Stunden aktualisiert)<br>**Auftragsbericht**: – |
| Laufzeitende (Monat) | 31.08.2020 | – | **Nutzungsbericht**: Anzeige des Verbrauchs am Monatsende<br>**Auftragsbericht**: – |
| Auftragsgenerierung | 03.09.2020–07.09.2020 | – | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Berechnung der erzielten Auszahlung | 04.09.2020–10.09.2020 | Kennzeichnung als **Nicht verarbeitet** im Transaktionsverlauf des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Monatliche Auszahlung | 10.05.2020 | Kennzeichnung als **Anstehend** im Transaktionsverlauf des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Auszahlungsdatum\** | 15.10.2020 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Begleichung der Kundenrechnung | 01.12.2020 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge  |
|  |  |  |  |

\* Auf Nutzungs- und Auftragsberichte kann im Analyseabschnitt in Partner Center zugegriffen werden.</br>\** Das Auszahlungsdatum ist in Pacific Standard Time (PST) angegeben.

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Kunden mit Kreditkarten- oder Rechnungszahlung

Für alle Käufe mit Kreditkarte oder monatlicher Rechnung gilt ein Einbehaltungszeitraum von 30 Tagen, um sicherzustellen, dass die Zahlung tatsächlich erfolgt und es zu keinen Rückbuchungen oder möglichen Betrugsfällen kommt.

| Ereignis  | Datum (UTC) | Partnersichtbarkeit: Partner Center-Auszahlungsbericht  |  Partnersichtbarkeit: Partner Center-Analysen\*  |
| --- | --- | --- | --- |
| Transaktion oder Nutzungsmonat | 01.08.2019–31.08.2019 | – | **Nutzungsbericht**: Anzeige des neuen Verbrauchs (wird alle vier Stunden aktualisiert)<br>**Auftragsbericht**: – |
| Laufzeitende (Monat) | 31.08.2019 | – | **Nutzungsbericht**: Anzeige des Verbrauchs am Monatsende<br>**Auftragsbericht**: – |
| Auftragsgenerierung | 03.09.2019–07.09.2019 | – | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Begleichung der Kundenrechnung | 07.09.2019–10.09.2019 | – | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Berechnung der Auszahlung | 08.09.2019–12.09.2019 | Kennzeichnung als **Nicht verarbeitet** im Transaktionsverlauf des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Monatliche Auszahlung | 05.11.2019\* | Kennzeichnung als **Anstehend** im Transaktionsverlauf des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Auszahlungsdatum\** | 15.11.2019 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
|  |  |  |  |

\* Auf Nutzungs- und Auftragsberichte kann im Analyseabschnitt in Partner Center zugegriffen werden.</br>\** Das Auszahlungsdatum ist in Pacific Standard Time (PST) angegeben.

### <a name="enterprise-agreement-transactions-prior-to-may-1-2020"></a>Enterprise Agreement-Transaktionen vor dem 1. Mai 2020

Alle Käufe vor diesem Datum werden gemäß dem folgenden Zeitplan verarbeitet und bezahlt, nachdem Microsoft die Zahlung von Kunden erhalten und die Marketplace-Gebühr verarbeitet hat.

| Ereignis  | Datum (UTC)  | Partnersichtbarkeit: Partner Center-Auszahlungsbericht  |  Partnersichtbarkeit: Partner Center-Analysen\*  |
| --- | --- | --- | --- |
| Transaktion oder Nutzungsmonat | 01.08.2019–31.08.2019 | – | **Nutzungsbericht**: Anzeige des neuen Verbrauchs (wird alle vier Stunden aktualisiert)<br>**Auftragsbericht**: – |
| Laufzeitende (Monat) | 31.08.2019 | – | **Nutzungsbericht**: Anzeige des Verbrauchs am Monatsende<br>**Auftragsbericht**: – |
| Auftragsgenerierung | 03.09.2019–07.09.2019 | – | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Begleichung der Kundenrechnung | 01.12.2019 | – | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Berechnung der Auszahlung | 05.12.2019–07.12.2019 | Kennzeichnung als **Nicht verarbeitet** im Transaktionsverlauf des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Monatliche Auszahlung | 05.01.2019 | Kennzeichnung als **Anstehend** im Transaktionsverlauf des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
| Auszahlungsdatum\** | 15.01.2019 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards | **Nutzungsbericht**: Anzeige des Verbrauchs mit Auftrags-ID/Auftragspositions-ID (OrderID/OrderLineItemID)<br>**Auftragsbericht**: Anzeige AKTIVER Kundenaufträge |
|  |  |  |  |

\* Auf Nutzungs- und Auftragsberichte kann im Analyseabschnitt in Partner Center zugegriffen werden.</br>\** Das Auszahlungsdatum ist in Pacific Standard Time (PST) angegeben.

## <a name="process-for-customer-non-payment"></a>Prozess bei Nichtzahlung des Kunden

In seltenen Fällen gelingt es Microsoft nicht, Kundenzahlungen für Käufe im kommerziellen Marketplace einzuziehen. Sollte ein Kunde seiner Zahlungsverpflichtung gegenüber Microsoft nicht gemäß dem entsprechenden Abrechnungszeitplan nachkommen, beginnt der Inkassoprozess. Dieser dauert ungefähr vier Monate und beinhaltet eine beharrliche Kommunikation durch Microsoft. Sollte die Zahlung bis zum Ende dieses Prozesses nicht eingehen, schreibt Microsoft den Betrag als uneinbringlich ab.

Aufgrund des hier beschriebenen Auszahlungsprozesses wurden von Microsoft unter Umständen bereits Zahlungen an Herausgeber (Sie) geleistet, die letztendlich uneinbringlich sind. Für Beträge dieser Art gibt es daher einen Ausgleichsprozess. Wenn der Inkassoprozess für einen Kunden gestartet wurde und die Käufe voraussichtlich abgeschrieben werden müssen, erhalten Sie eine entsprechende Benachrichtigung, um Sie darüber zu informieren, dass Ihre (bereits erhaltene) Zahlung unter Umständen ausgeglichen werden muss.

Microsoft verwendet eine der folgenden Methoden, um bereits an Sie geleistete Zahlungen zurückzuerhalten: (1) Microsoft kann die unbezahlten Beträge mit zukünftigen Auszahlungen verrechnen. Wenn also beispielsweise Auszahlungen in Höhe von 1.000 USD als uneinbringlich eingestuft und abgeschrieben werden, werden Ihre zukünftigen Auszahlungen so lange zurückgehalten, bis die 1.000 USD ausgeglichen sind. (2) Alternativ kann Microsoft von Herausgebern eine Rückerstattung für nicht geleistete Zahlungen verlangen oder ihnen den entsprechenden Betrag in Rechnung stellen.

In der folgenden Tabelle wird ein Beispiel für einen Zeitplan angezeigt:

| Ereignis | Ungefähres Datum | Partnersichtbarkeit |
| --- | --- | --- |
| Exemplarisches Auszahlungsdatum | 15.10.2020 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards |
| Ausbleibende Kundenzahlung an Microsoft | 02.12.2020–05.12.2020 | Keine Änderung, wie oben |
| Kunde erhält erste E-Mail wegen Zahlungsverzug | 06.12.2020 | Keine |
| Kunde erhält regelmäßig E-Mails mit zunehmender Dringlichkeit | 07.12.2020–31.01.2021 | Keine |
| Herausgeber wird über voraussichtliche Abschreibung informiert | 07.01.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Kunde noch nicht bezahlt hat. Transaktions-ID und Dollarbetrag sind angegeben. |
| Kunde erhält Kündigungsbenachrichtigung | 01.02.2021 | Keine |
| Inkassoprozess endet/Betrag wird abgeschrieben | 15.02.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Betrag abgeschrieben wurde. Transaktions-ID und Dollarbetrag sind angegeben. |
| Auszahlung wird abgezogen | 01.03.2021 | Partner Center-Auszahlungsauszug des Herausgebers enthält negative Transaktion |
| Auszahlung wird einbehalten | 15.03.2021 | Partner Center-Auszahlungsauszug enthält zukünftige Auszahlungen. Zahlungen an den Herausgeber werden erst wieder geleistet, wenn der Saldo nicht mehr negativ ist.  |
|||

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Anzahl der Tage bis zum Eingang von Zahlungen auf einem Auszahlungskonto

In der Regel senden wir die in einem Monat fälligen Zahlungen am 15. des Monats, es dauert jedoch einige Zeit, bis die Zahlung auf Ihrem Konto eingeht. Die Anzahl der Tage hängt von der Zahlungsmethode ab, die wir für Ihr Konto verwenden, wie unten beschrieben.

> [!NOTE]
> Die unten gezeigten Tage sind ungefähre Angaben. Es kann länger oder kürzer dauern, bis eine Auszahlung auf Ihrem Konto eingeht.

| Payment Method     | Anzahl der Tage bis zum Eingang auf dem Auszahlungskonto     |
|--------------------|--------------------------------------------|
| PayPal             | 1 Werktag                             |
| ACH/SEPA-Überweisungen           | 2-3 Werktage                          |
| Telegrafische Geldüberweisung      | 7-10 Werktage                         |

## <a name="next-step"></a>Nächster Schritt

- [Steuerliche Aspekte für kommerzielle Marketplace-Herausgeber](tax-details-marketplace.md)
