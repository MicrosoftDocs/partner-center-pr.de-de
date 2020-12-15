---
title: Auszahlungs Zeitpläne und-Prozesse
description: Erfahren Sie mehr über Auszahlungen und Transaktionen, z. b. Zahlungs Zeitpläne und Wiederholungsprozesse für den kommerziellen Marketplace und andere Transaktionen.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/25/2020
ms.openlocfilehash: bb7a6673d2dee5a35f1c5be96f354451633eecf5
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492669"
---
# <a name="payout-schedules-and-processes"></a>Auszahlungs Zeitpläne und-Prozesse

**Geeignete Rollen:**

- Kontoadministrator
- Globaler Administrator

In diesem Artikel wird der Zahlungsplan von Microsoft erläutert, in dem der Status einer Auszahlung zu finden ist, und der Prozess für die Nichtzahlung von Kunden.

## <a name="payment-schedules"></a>Zahlungspläne

In den folgenden Abschnitten wird der Auszahlungsprozess für **Konzernvertrag** -und **Kreditkarten-/Rechnung-** Transaktionen beschrieben.

### <a name="enterprise-agreement-transactions"></a>Transaktionen Konzernvertrag

Wenn ein Kunde ein Produkt von Microsoft AppSource oder Azure Marketplace mit vorhandenem Microsoft-Konzernvertrag für Transaktionen kauft, werden im nächsten Auszahlungs Zeitraum 30 Tage nach Kunden Rechnung Zahlungen ausgegeben. Transaktionen, bei denen ein Kunde eine Kreditkarte verwendet, haben eine 30-tägige Beibehaltungsdauer vor der Auszahlung.

Es kommt häufig vor, dass Microsoft die Zahlung vom Kunden sammelt. Weitere Informationen zu den Aktionen, die wir durchführen, wenn der Kunde [Microsoft nicht bezahlt](#process-for-customer-non-payment) , aber wir haben bereits eine Auszahlung ausgegeben.

| Ereignis | Beschreibung | Sichtbarkeit von Berichten | Zeit Steuerungs |
| --- | --- | --- | --- |
| Verwendung oder Monat der Transaktion | Der Kunde verwendet oder kauft einen Dienst. | Dashboard für [Nutzung](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestellung](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 1** |
| Microsoft berechnet Abrechnungsbetrag | Bestimmen der Gesamtauslastung, Transaktionen gesamt | Dashboard für [Nutzung](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestellung](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 2** |
| Auszahlungs Veröffentlichung | Bestimmen der Gebühren und Auszahlungs Einnahmen der Agentur | Im Transaktionsverlauf in der [Auszahlungs Anweisung](payout-statement.md) als nicht verarbeitet markiert | **Monat 3 (1. Woche)** |
| Auszahlung vorbereiten | Der Gewinn ist für die monatliche Zahlung vorbereitet. | Im Transaktionsverlauf in der [Auszahlungs Anweisung](payout-statement.md) als demnächst markiert | **Monat 3 (1. Woche)** |
| **Auszahlung gesendet** | **Die Zahlung wird an den Verleger gesendet.** | **Gekennzeichnet als in Transaktionsverlauf gesendet und im Abschnitt "Zahlungen" der [Auszahlungs Anweisung](payout-statement.md)** | **Monat 3 (nicht später als der 15.)** |
| Von Kunde bezahlte Rechnung | Microsoft sammelt die Zahlung von Kunden | Keine Änderung | **Monat 4 bis 12** |
|

\* Das Auszahlungsdatum liegt in der Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Die Zeitachse für Enterprise Agreement-Kunden.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transaktionen mit Kreditkarte oder Rechnung (Überprüfung/Netzwerk)

Alle Käufe mit einer Kreditkarte oder einer monatlichen Rechnung verfügen über einen Zeitraum von 30 Tagen, um sicherzustellen, dass die Geldbeträge vom Kunden gesammelt werden.

| Ereignis | Beschreibung | Sichtbarkeit von Berichten | Zeit Steuerungs |
| --- | --- | --- | --- |
| Verwendung oder Monat der Transaktion | Der Kunde verwendet oder kauft einen Dienst. | Dashboard für [Nutzung](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestellung](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 1** |
| Von Kunde bezahlte Rechnung | Ermitteln der Gesamtauslastung, des gesamten Transaktionswerts und der Kunden zahlungsrechnung | Dashboard für [Nutzung](/azure/marketplace/partner-center-portal/usage-dashboard) oder [Bestellung](/azure/marketplace/partner-center-portal/orders-dashboard) | **Monat 2** |
| Auszahlungs Veröffentlichung | Bestimmen der Gebühren und Auszahlungs Einnahmen der Agentur | Im Transaktionsverlauf in der [Auszahlungs Anweisung](payout-statement.md) als nicht verarbeitet markiert | **Monat 2** |
| 30-tägige Beibehaltungszeitraum | Stellen Sie die Erfassung von Kosten, möglichen Rück Belastungs-und Erstattungs Anforderungen sicher. | Im Transaktionsverlauf in der [Auszahlungs Anweisung](payout-statement.md) als nicht verarbeitet markiert | **Monat 3** |
| Auszahlung vorbereiten | Der Gewinn ist für die monatliche Zahlung vorbereitet. | Im Transaktionsverlauf in der [Auszahlungs Anweisung](payout-statement.md) als demnächst markiert | **Monat 4 (1. Woche)** |
| **Auszahlung gesendet** | **Die Zahlung wird an den Verleger gesendet.** | **Gekennzeichnet als in Transaktionsverlauf gesendet und im Abschnitt "Zahlungen" der [Auszahlungs Anweisung](payout-statement.md)** | **Monat 4 (spätestens 15.)** |
|

\* Das Auszahlungsdatum liegt in der Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Zeitachsen der Zahlungen für Kreditkarten-und Rechnungs Kunden.":::

## <a name="process-for-customer-non-payment"></a>Prozess bei Nichtzahlung des Kunden

In seltenen Fällen gelingt es Microsoft nicht, Kundenzahlungen für Käufe im kommerziellen Marketplace einzuziehen. Sollte ein Kunde seiner Zahlungsverpflichtung gegenüber Microsoft nicht gemäß dem entsprechenden Abrechnungszeitplan nachkommen, beginnt der Inkassoprozess. Dieser dauert ungefähr vier Monate und beinhaltet eine beharrliche Kommunikation durch Microsoft. Sollte die Zahlung bis zum Ende dieses Prozesses nicht eingehen, schreibt Microsoft den Betrag als uneinbringlich ab.

Aufgrund des hier beschriebenen Auszahlungsprozesses wurden von Microsoft unter Umständen bereits Zahlungen an Herausgeber (Sie) geleistet, die letztendlich uneinbringlich sind. Für Beträge dieser Art gibt es daher einen Ausgleichsprozess. Wenn der Inkassoprozess für einen Kunden gestartet wurde und die Käufe voraussichtlich abgeschrieben werden müssen, erhalten Sie eine entsprechende Benachrichtigung, um Sie darüber zu informieren, dass Ihre (bereits erhaltene) Zahlung unter Umständen ausgeglichen werden muss.

Microsoft verwendet eine der folgenden Methoden, um bereits an Sie geleistete Zahlungen zurückzuerhalten: (1) Microsoft kann die unbezahlten Beträge mit zukünftigen Auszahlungen verrechnen. Wenn also beispielsweise Auszahlungen in Höhe von 1.000 USD als uneinbringlich eingestuft und abgeschrieben werden, werden Ihre zukünftigen Auszahlungen so lange zurückgehalten, bis die 1.000 USD ausgeglichen sind. (2) Alternativ kann Microsoft von Herausgebern eine Rückerstattung für nicht geleistete Zahlungen verlangen oder ihnen den entsprechenden Betrag in Rechnung stellen.

Im Anschluss finden Sie einen Beispielzeitplan:

| Ereignis | Ungefähre Datumsangabe * | Partnersichtbarkeit |
| --- | --- | --- |
| Exemplarisches Auszahlungsdatum | 15.10.2020 | Kennzeichnung als **Gesendet** im Transaktionsverlauf und im Auszahlungsabschnitt des Auszahlungsdashboards |
| <font color="red">Ausbleibende Kundenzahlung an Microsoft</font> | 02.12.2020–05.12.2020 | Keine Änderung, wie oben |
| Kunde erhält erste E-Mail wegen Zahlungsverzug | 06.12.2020 | Keine |
| Kunde erhält regelmäßig E-Mails mit zunehmender Dringlichkeit | 07.12.2020–31.01.2021 | Keine |
| Herausgeber wird über voraussichtliche Abschreibung informiert | 07.01.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Kunde noch nicht bezahlt hat. Transaktions-ID und Dollarbetrag sind angegeben. |
| Kunde erhält Kündigungsbenachrichtigung | 01.02.2021 | Keine |
| Inkassoprozess endet/Betrag wird abgeschrieben | 15.02.2021 | Herausgeber erhält eine E-Mail-Benachrichtigung mit der Information, dass der Betrag abgeschrieben wurde. Transaktions-ID und Dollarbetrag sind angegeben. |
| Auszahlung wird abgezogen | 01.03.2021 | Dem Verleger wird eine negative Transaktion in der Partner Center-Auszahlungs Anweisung angezeigt. |
| Auszahlung wird einbehalten | 15.03.2021 | Zukünftige Auszahlungen werden in der Partner Center-Auszahlungs Anweisung angezeigt. Zahlungen an den Herausgeber werden erst wieder geleistet, wenn der Saldo nicht mehr negativ ist.  |
|||

\* Das Auszahlungsdatum liegt in der Pacific Standard Time (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Anzahl der Tage bis zum Eingang von Zahlungen auf einem Auszahlungskonto

In der Regel senden wir die in einem Monat fälligen Zahlungen am 15. des Monats, es dauert jedoch einige Zeit, bis die Zahlung auf Ihrem Konto eingeht. Die Anzahl der Tage hängt von der Zahlungsmethode ab, die wir für Ihr Konto verwenden, wie unten beschrieben.

> [!NOTE]
> Die unten gezeigten Tage sind ungefähre Werte. das Erreichen Ihres Kontos kann mehr oder weniger Zeit in Anspruch nehmen.

| Payment Method     | Anzahl der Tage bis zum Eingang auf dem Auszahlungskonto     |
|--------------------|--------------------------------------------|
| PayPal             | 1 Werktag                             |
| ACH/SEPA-Überweisungen           | 2-3 Werktage                          |
| Telegrafische Geldüberweisung      | 7-10 Werktage                         |
|

## <a name="next-steps"></a>Nächste Schritte

- [Steuerliche Aspekte für kommerzielle Marketplace-Herausgeber](tax-details-marketplace.md)
