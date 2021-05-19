---
title: Auszahlungszeitpläne und -prozesse
description: Erfahren Sie mehr über Auszahlungen und Transaktionen, z. B. Zahlungszeitpläne und Recoupmentprozesse für den kommerziellen Marketplace und andere Transaktionen.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146951"
---
# <a name="payout-schedules-and-processes"></a>Auszahlungszeitpläne und -prozesse

**Geeignete Rollen:** Kontoadministrator-| Globaler Administrator

In diesem Artikel wird der Zahlungszeitplan von Microsoft erläutert, in dem der Status einer Auszahlung und der Prozess für nicht bezahlte Kunden zu finden sind.

## <a name="payment-schedules"></a>Zahlungspläne

In den folgenden Abschnitten wird der Auszahlungsprozess für **Enterprise Agreement-** und **Kreditkarten-/Rechnungstransaktionen** beschrieben.

### <a name="enterprise-agreement-transactions"></a>Enterprise Agreement Transaktionen

Wenn ein Kunde ein Produkt von Microsoft AppSource oder Azure Marketplace mithilfe seiner vorhandenen Microsoft Enterprise Agreement für Transaktionen erwirbt, geben wir Auszahlungen im nächsten Auszahlungszyklus 30 Tage nach der Kundenrechnung aus. Transaktionen, bei denen ein Kunde eine Kreditkarte verwendet, haben eine 30-tägige Haltefrist vor der Auszahlung.

Eine Auszahlung erfolgt häufig, bevor Microsoft die Zahlung vom Kunden einzahlt. Weitere [Informationen zu den Aktionen, die wir](#process-for-customer-non-payment) ergreifen, wenn der Kunde Microsoft nicht bezahlt, aber wir bereits eine Auszahlung ausgegeben haben, finden Sie weiter unten unter Prozess für nicht bezahlte Kunden.

| Ereignis | Beschreibung | Sichtbarkeit der Berichterstellung | Timing* |
| --- | --- | --- | --- |
| Nutzung oder Transaktionsmonat | Der Kunde verwendet oder kauft einen Dienst. | [Dashboard "Nutzung"](/azure/marketplace/partner-center-portal/usage-dashboard) [oder "Bestellung"](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 1** |
| Microsoft berechnet den Abrechnungsbetrag | Ermitteln der Gesamtnutzung und der Transaktionen insgesamt | [Dashboard "Nutzung"](/azure/marketplace/partner-center-portal/usage-dashboard) [oder "Bestellung"](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 2** |
| Gesendete Auszahlung | Ermitteln der Agenturgebühr und der Auszahlungseinnahmen | Im Transaktionsverlauf für den [Auszahlungsauszug](payout-statement.md) als Nicht verarbeitet markiert | **Monat 3 (1. Woche)** |
| Vorbereiten der Auszahlung | Einnahmen werden für die monatliche Zahlung vorbereitet. | Im Transaktionsverlauf im [Auszahlungsauszug](payout-statement.md) als "Anstehend" markiert | **Monat 3 (1. Woche)** |
| **Gesendete Auszahlung** | **Die Zahlung wird an den Herausgeber gesendet.** | **Markiert als Gesendet im Transaktionsverlauf und im Abschnitt "Zahlungen" des [Auszahlungsauszugs](payout-statement.md)** | **Monat 3 (nicht später als der 15.)** |
| Vom Kunden bezahlte Rechnung | Microsoft sammelt Zahlungen vom Kunden | Keine Änderung | **Monat 4 bis 12** |
|

\* Das Auszahlungsdatum befindet sich in Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Zeitachse für Zahlungen für Enterprise Agreement-Kunden.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transaktionen mit Kreditkarte oder Rechnung (Scheck/Überweisung)

Alle Käufe mit einer Kreditkarte oder einer monatlichen Rechnung haben einen 30-tägigen Zurückhaltungszeitraum, um sicherzustellen, dass Geld vom Kunden eingezogen wird.

| Ereignis | Beschreibung | Berichterstellungssichtbarkeit | Zeitliche Steuerung* |
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

Aufgrund des hier beschriebenen Auszahlungsprozesses wurden von Microsoft unter Umständen bereits Zahlungen an Herausgeber (Sie) geleistet, die letztendlich uneinbringlich sind. Für Beträge dieser Art gibt es daher einen Ausgleichsprozess. Wenn der Inkassoprozess für einen Kunden gestartet wurde und die Käufe voraussichtlich abgeschrieben werden müssen, erhalten Sie eine entsprechende Benachrichtigung, um Sie darüber zu informieren, dass Ihre (bereits erhaltene) Zahlung unter Umständen ausgeglichen werden muss.

Microsoft verwendet eine der folgenden Methoden, um bereits an Sie geleistete Zahlungen zurückzuerhalten: (1) Microsoft kann die unbezahlten Beträge mit zukünftigen Auszahlungen verrechnen. Wenn also beispielsweise Auszahlungen in Höhe von 1.000 USD als uneinbringlich eingestuft und abgeschrieben werden, werden Ihre zukünftigen Auszahlungen so lange zurückgehalten, bis die 1.000 USD ausgeglichen sind. (2) Alternativ kann Microsoft von Herausgebern eine Rückerstattung für nicht geleistete Zahlungen verlangen oder ihnen den entsprechenden Betrag in Rechnung stellen.

Der folgende Zeitplan ist ein Beispiel:

| Ereignis | Ungefähres Datum* | Partnersichtbarkeit |
| --- | --- | --- |
| Exemplarisches Auszahlungsdatum | 15.10.2020 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards |
| <font color="red">Ausbleibende Kundenzahlung an Microsoft</font> | 02.12.2020–05.12.2020 | Keine Änderung, wie oben |
| Kunde erhält erste E-Mail wegen Zahlungsverzug | 06.12.2020 | Keine |
| Kunde erhält regelmäßig E-Mails mit zunehmender Dringlichkeit | 07.12.2020–31.01.2021 | Keine |
| Herausgeber wird über voraussichtliche Abschreibung informiert | 07.01.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Kunde noch nicht bezahlt hat. Transaktions-ID und Dollarbetrag sind angegeben. |
| Kunde erhält Kündigungsbenachrichtigung | 01.02.2021 | Keine |
| Inkassoprozess endet/Betrag wird abgeschrieben | 15.02.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Betrag abgeschrieben wurde. Transaktions-ID und Dollarbetrag sind angegeben. |
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
