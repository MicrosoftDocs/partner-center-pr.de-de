---
title: Auszahlungszeitpläne und -prozesse
description: Erfahren Sie mehr über Auszahlungen und Transaktionen, z. B. Zahlungszeitpläne und Recoupmentprozesse für Azure Marketplace und andere Transaktionen.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582420"
---
# <a name="payout-schedules-and-processes"></a>Auszahlungszeitpläne und -prozesse

**Geeignete Rollen:** Kontoadministrator-| Globaler Administrator

In diesem Artikel werden der Zahlungszeitplan von Microsoft, der Ort, an dem der Status einer Auszahlung zu finden ist, und der Prozess für die Nichtzahlung des Kunden erläutert.

## <a name="payment-schedules"></a>Zahlungspläne

In den folgenden Abschnitten wird der Auszahlungsprozess für **Enterprise Agreement-** und **Microsoft-Kundenvereinbarung- oder CSP-Transaktionen** beschrieben.

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Transaktionen, wenn der Kunde über eine Enterprise Agreement

Wenn ein Kunde ein Produkt von Microsoft AppSource oder Azure Marketplace mithilfe seiner vorhandenen Microsoft-Enterprise Agreement für Transaktionen erwirbt, geben wir Auszahlungen im nächsten Auszahlungszyklus 30 Tage nach der Kundenrechnung aus. Transaktionen, bei denen ein Kunde eine Kreditkarte verwendet, verfügen über einen 30-tägigen Zurückhaltungszeitraum vor der Auszahlung.

Häufig erfolgt eine Auszahlung, bevor Microsoft die Zahlung vom Kunden einsackt. Die Aktionen, die wir ergreifen, wenn der Kunde Microsoft nicht bezahlt, aber bereits eine Auszahlung ausgestellt hat, finden Sie weiter unten unter Verarbeiten der Nichtzahlung durch den [Kunden.](#process-for-customer-non-payment)

| Ereignis | Beschreibung | Berichtssichtbarkeit | Zeitliche Steuerung* |
| --- | --- | --- | --- |
| Nutzung oder Monat der Transaktion | Der Kunde verwendet oder kauft einen Dienst. | [Nutzungs-](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestelldashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 1** |
| Microsoft berechnet den Abrechnungsbetrag. | Ermitteln der Gesamtnutzung, der Gesamtanzahl der Transaktionen | [Nutzungs-](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestelldashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 2** |
| Bereitgestellte Auszahlung | Ermitteln der Agenturgebühr und der Auszahlungserlöse | Im Transaktionsverlauf für den Auszahlungsauszug als Nicht verarbeitet [markiert](payout-statement.md) | **Monat 3 (1. Woche)** |
| Vorbereiten der Auszahlung | Einnahmen sind auf monatliche Zahlungen vorbereitet | Im Transaktionsverlauf im Auszahlungsauszug als Anstehende [markiert](payout-statement.md) | **Monat 3 (1. Woche)** |
| **Gesendete Auszahlung** | **Die Zahlung wird an den Herausgeber gesendet.** | **Gekennzeichnet als Gesendet im Transaktionsverlauf und im Abschnitt "Zahlungen" des [Auszahlungsauszugs](payout-statement.md)** | **Monat 3 (nicht später als der 15.)** |
| Vom Kunden bezahlte Rechnung | Microsoft erfasst Die Zahlung vom Kunden | Keine Änderung | **Monat 4 bis 12** |
|

\* Das Auszahlungsdatum ist Pacific Normalzeit (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Zahlungszeitachse für Enterprise Agreement-Kunden.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Transaktionen, wenn der Kunde über einen Microsoft-Kundenvereinbarung oder CSP verfügt

Alle Käufe mit einer Kreditkarte oder monatlichen Rechnung verfügen über eine 30-tägige Haltefrist, um sicherzustellen, dass die Mittel vom Kunden einsammelt werden.

| Ereignis | Beschreibung | Sichtbarkeit der Berichterstellung | Timing* |
| --- | --- | --- | --- |
| Nutzung oder Monat der Transaktion | Der Kunde verwendet oder kauft einen Dienst. | [Nutzungs-](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestelldashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 1** |
| Vom Kunden bezahlte Rechnung | Ermitteln der Gesamtnutzung, des Transaktionswerts und der Vom Kunden bezahlten Rechnung | [Nutzungs-](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestelldashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 2** |
| Bereitgestellte Auszahlung | Ermitteln der Agenturgebühr und der Auszahlungseinnahmen | Im Transaktionsverlauf für den [Auszahlungsauszug](payout-statement.md) als Nicht verarbeitet markiert | **Monat 2** |
| 30-Tage-Haltedauer | Sicherstellen der Sammlung von Guthaben, möglicher Rückbelastungen und Rückerstattungsanforderungen | Im Transaktionsverlauf für den [Auszahlungsauszug](payout-statement.md) als Nicht verarbeitet markiert | **Monat 3** |
| Vorbereiten der Auszahlung | Einnahmen werden für die monatliche Zahlung vorbereitet. | Im Transaktionsverlauf im [Auszahlungsauszug](payout-statement.md) als "Anstehend" markiert | **Monat 4 (1. Woche)** |
| **Gesendete Auszahlung** | **Die Zahlung wird an den Herausgeber gesendet.** | **Gekennzeichnet als Gesendet im Transaktionsverlauf und im Abschnitt "Zahlungen" des [Auszahlungsauszugs](payout-statement.md)** | **Monat 4 (nicht später als der 15.)** |
|

\* Das Auszahlungsdatum ist Pacific Normalzeit (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Zeitachse der Zahlungen für Kreditkarten- und Rechnungskunden.":::

## <a name="process-for-customer-non-payment"></a>Prozess bei Nichtzahlung des Kunden

In seltenen Fällen gelingt es Microsoft nicht, Kundenzahlungen für Käufe im kommerziellen Marketplace einzuziehen. Sollte ein Kunde seiner Zahlungsverpflichtung gegenüber Microsoft nicht gemäß dem entsprechenden Abrechnungszeitplan nachkommen, beginnt der Inkassoprozess. Dieser dauert ungefähr vier Monate und beinhaltet eine beharrliche Kommunikation durch Microsoft. Wenn die Zahlung am Ende dieses Prozesses nicht eingegangen ist, schreibt Microsoft die Mittel als nicht einsetzbar ab.

Aufgrund des hier beschriebenen Auszahlungsprozesses wurden von Microsoft unter Umständen bereits Zahlungen an Herausgeber (Sie) geleistet, die letztendlich uneinbringlich sind. Für Beträge dieser Art gibt es daher einen Ausgleichsprozess.

Microsoft verwendet eine der folgenden Methoden, um bereits an Sie geleistete Zahlungen zurückzuerhalten: (1) Microsoft kann die unbezahlten Beträge mit zukünftigen Auszahlungen verrechnen. Wenn also beispielsweise Auszahlungen in Höhe von 1.000 USD als uneinbringlich eingestuft und abgeschrieben werden, werden Ihre zukünftigen Auszahlungen so lange zurückgehalten, bis die 1.000 USD ausgeglichen sind. (2) Alternativ kann Microsoft von Herausgebern eine Rückerstattung für nicht geleistete Zahlungen verlangen oder ihnen den entsprechenden Betrag in Rechnung stellen.

Der folgende Zeitplan ist ein Beispiel:

| Ereignis | Ungefähres Datum* | Partnersichtbarkeit |
| --- | --- | --- |
| Exemplarisches Auszahlungsdatum | 15.10.2020 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards |
| <font color="red">Ausbleibende Kundenzahlung an Microsoft</font> | 02.12.2020–05.12.2020 | Keine Änderung, wie oben |
| Kunde erhält erste E-Mail wegen Zahlungsverzug | 06.12.2020 | Keine |
| Kunde erhält regelmäßig E-Mails mit zunehmender Dringlichkeit | 07.12.2020–31.01.2021 | Keine |
| Herausgeber wird über voraussichtliche Abschreibung informiert | 07.01.2021 | - |
| Kunde erhält Kündigungsbenachrichtigung | 01.02.2021 | Keine |
| Inkassoprozess endet/Betrag wird abgeschrieben | 15.02.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Betrag abgeschrieben wurde. |
| Auszahlung wird abgezogen | 01.03.2021 | Der Herausgeber sieht eine negative Transaktion in Partner Center Auszahlungsauszug. |
| Auszahlung wird einbehalten | 15.03.2021 | Zukünftige Auszahlungen werden in Partner Center Auszahlungsauszug angezeigt. Zahlungen an den Herausgeber werden erst wieder geleistet, wenn der Saldo nicht mehr negativ ist.  |
|||

\* Das Auszahlungsdatum ist Pacific Normalzeit (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Anzahl der Tage bis zum Eingang von Zahlungen auf einem Auszahlungskonto

Wir senden in der Regel alle fälligen Zahlungen in einem bestimmten Monat am 15. Tag dieses Monats, aber es dauert eine weitere Zeit, bis die Zahlung Ihr Konto erreicht. Die Anzahl der Tage hängt von der Zahlungsmethode ab, die wir für Ihr Konto verwenden, wie unten beschrieben.

> [!NOTE]
> Die unten gezeigten Tage sind ungefähr. Bei jeder Zahlung kann es mehr oder weniger Zeit dauern, ihr Konto zu erreichen.

| Payment Method     | Anzahl der Tage bis zum Eingang auf dem Auszahlungskonto     |
|--------------------|--------------------------------------------|
| PayPal             | 1 Werktag                             |
| ACH/SEPA-Überweisungen           | 2-3 Werktage                          |
| Telegrafische Geldüberweisung      | 7-10 Werktage                         |
|

## <a name="next-steps"></a>Nächste Schritte

- [Steuerliche Aspekte für kommerzielle Marketplace-Herausgeber](tax-details-marketplace.md)
