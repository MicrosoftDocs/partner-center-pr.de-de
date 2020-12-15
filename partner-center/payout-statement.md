---
title: Auszahlungsaufstellungen
description: Informieren Sie sich über Auszahlungs Anweisungen und-Zusammenfassungen sowie über das Anzeigen und Exportieren von Zahlungsdaten aus dem Microsoft Partner Center.
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 10/29/2020
ms.openlocfilehash: f74dcdc240553cea2c9d226364a8bd6242acc200
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492635"
---
# <a name="payout-statements"></a>Auszahlungsaufstellungen

**Geeignete Rollen:**

- Kontoadministrator
- Globaler Administrator

Die **Auszahlungs Erklärung** bietet einen Überblick über Ihre Auszahlungen von angeboten, die über den kommerziellen Marketplace verkauft werden. Es zeigt den Transaktionsverlauf Ihres Ergebnisses, schätzt Ihre nächste Zahlung und zeigt Zahlungs Trends an. Sie können auch den Transaktionsverlauf und die Zahlungsanweisungen herunterladen. In diesem Artikel wird erläutert, wie Sie auf Ihre Auszahlungs Erklärung und die unterschiedlichen Auszahlungs Seiten und Downloads zugreifen können, die Ihnen im Partner Center zur Verfügung stehen.

>[!NOTE]
>Es werden nur Daten für MPN-IDs und Programme angezeigt, denen Sie zugeordnet sind. Wenn Sie zusätzliche Daten anzeigen möchten, wenden Sie sich an Ihren Konto Administrator, um Berechtigungen zu erhalten. 

## <a name="roles-and-permissions"></a>Rollen und Berechtigungen

Für den Zugriff auf eine Auszahlungs Anweisung müssen Sie der Rolle " **Konto Besitzer** " oder " **Mitwirkender Mitwirkender** " zugewiesen sein.

| Berichte/Seiten | Kontobesitzer | Manager | Entwickler | Mitwirkender im Geschäftsbereich | Mitwirkender im Finanzbereich | Vermarkter |
| --- | --- | --- | --- | --- | --- | --- |
| Kaufbericht (einschließlich Daten in Quasi-Echtzeit) | Kann anzeigen | Kann anzeigen | Kein Zugriff | Kein Zugriff | Kann anzeigen | Kein Zugriff |
| Feedback – Berichte/Antworten | Kann Feedback anzeigen und senden | Kann Feedback anzeigen und senden | Kann Feedback anzeigen und senden | Kein Zugriff | Kein Zugriff | Kann Feedback anzeigen und senden |
| Integritätsbericht (einschließlich Daten in Quasi-Echtzeit) | Kann anzeigen | Kann anzeigen | Kann anzeigen | Kann anzeigen | Kein Zugriff | Kein Zugriff |
| Nutzungsbericht | Kann anzeigen | Kann anzeigen | Kann anzeigen | Kann anzeigen | Kein Zugriff | Kein Zugriff |
| Auszahlungskonto | Kann aktualisieren | Kein Zugriff | Kein Zugriff | Kein Zugriff | Kann aktualisieren | Kein Zugriff |
| Steuerprofil | Kann aktualisieren | Kein Zugriff | Kein Zugriff | Kein Zugriff | Kann aktualisieren | Kein Zugriff |
| Auszahlungszusammenfassung | Kann anzeigen | Kein Zugriff | Kein Zugriff | Kein Zugriff | Kann anzeigen | Kein Zugriff |
|

## <a name="access-your-payout-statement"></a>Zugriff auf Ihre Auszahlungs Anweisung

Melden Sie sich bei [Partner Center](https://partner.microsoft.com/dashboard/home) an, und wählen Sie das Auszahlungs Symbol in der oberen rechten Ecke des Bildschirms aus, um auf diese unterschiedlichen Zusammenfassungen zuzugreifen:

- Transaktionsverlauf
- Zahlungen
- Exportieren von Daten

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Veranschaulicht das Auszahlungs Symbol in der oberen rechten Ecke des Partner Center-Portals.":::

Sie können auch die [Partner-Auszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts) verwenden, um eine Verbindung zu Auszahlungs Transaktionen und Zahlungsdaten direkt herzustellen und diese zu erhalten.


## <a name="transaction-history"></a>Transaktionsverlauf

Die Seite **Transaktionsverlauf** zeigt die Zusammenfassung ihres Ergebnisses, die geschätzte nächste Zahlung und ihren Gewinn-und Zahlungs Trend in den letzten 36 Monaten an. Sie können auch Transaktionsdetails aus diesem Abschnitt herunterladen.


:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Transaktions Übersicht.":::

- **Das in diesem Jahr gesendete Ergebnis** – Gesamtgewinn und Aufschlüsselung der Einnahmen, die im kommenden Monat gezahlt werden.
- **Geschätzter Zahlungs Monat** – Gesamtgewinn in den kommenden Monaten erwartet.
- **Gewinn-und Zahlungs Trend** – monatliche Erwerbs-und Zahlungsbeträge in den letzten 36 Monaten.
- **Download** – laden Sie Transaktionsdetails im CSV-oder TSV-Format herunter.

Verwenden Sie die Auswahl Datumsbereich in der oberen rechten Ecke der Seite, um die Ausgabe der Seite so zu filtern, dass die letzten 3, 6, 12 oder 36 Monate angezeigt werden. Oder wählen Sie einen benutzerdefinierten Datumsbereich von bis zu 36 Monaten aus. Der Standard Datumsbereich ist 12 Monate. Sie können auch nach Registrierungs-ID, Programm, Zahlungs-ID, Erwerbs Wert, Hebel und Status filtern. Daten sind für das aktuelle Geschäftsjahr (1. Juni 30. Juli) und die letzten beiden Geschäftsjahre verfügbar.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Der Suchfilter in der oberen rechten Ecke der Seite.":::

Zum Anzeigen weiterer Details zu einer Einnahme klicken Sie rechts auf der Seite auf den Pfeil nach unten. Auf diese Weise werden der Hebel, der Umsatz Betrag, das Produkt und der Kunde angezeigt. Wenn eine dieser Daten aus irgendeinem Grund nicht verfügbar ist, Sie aber darauf zugreifen müssen, wenden Sie sich an den Support. Wenn das Ergebnis einer Anpassung und nicht einer Transaktion entspricht, werden die Felder Product und Customer nicht angezeigt.

### <a name="transaction-history-summary"></a>Transaktionsverlauf-Zusammenfassung

Dies zeigt Details zum Erwerb, einschließlich des Ursprungs der ergaben aus dem Produkt, das die ergaben Datumsangaben, den Status und den geschätzten Zahlungs Monat verkauft.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Transaktionsverlauf.":::

- Erstellungs **Datum** – das Datum des Kaufs.
- **Ermittungstyp** – der Typ des Erwerbs, z. b. Sell, Rabatt oder Co-op.
- **Gesamtbetrag** – der Netto Erwerbs Betrag. Im kommerziellen Marketplace bedeutet dies, dass die Standard-Marketplace-Gebühr abgezogen wird.
- **Status** – bietet drei Optionen:
    - **Anstehende** –-Einnahmen liegen in einem ausstehenden kühl Zeitraum.
    - **Verarbeitete** –-Einnahmen werden für die nächste Zahlung vorbereitet.
    - **Gesendete** –-Einnahmen wurden bezahlt.
- **Geschätzter Zahlungs Monat** – der Monat, in dem der Gewinn gezahlt werden soll. Weitere Informationen finden Sie im [nächsten Abschnitt](#estimated-payment-month) .

Das Sammeln von Transaktionen wird angezeigt, sobald die Transaktion die Auszahlungs Berechtigung erfüllt. Informationen dazu, warum Sie möglicherweise fehlende oder unerwartete Einnahmen haben, finden Sie unter [häufig gestellte Fragen zu kommerziellen Marketplace-Auszahlungen](payout-faq.md#why-are-my-earnings-missing).

#### <a name="estimated-payment-month"></a>Geschätzter Zahlungs Monat

Die Seite Transaktionsverlauf enthält jetzt eine Tabelle mit ihren geschätzten Zahlungs Summen in den nächsten Monaten. Sie können diese Informationen auch in den Exporten Transaktionsverlauf und Zusammenfassungs Bericht anzeigen und herunterladen. Diese Informationen erleichtern das verbessern von reversationen und Zahlungs Projektionen.

Der geschätzte Zahlungs Monat wird basierend auf Programm Konfigurations Regeln und Zeitachsen berechnet und im nächsten/bevorstehenden Zahlungszeitraum verarbeitet.

Der geschätzte Zahlungs Monat ist zurzeit für alle Erwerbs Typen mit Ausnahme von Co-op verfügbar, die als **nicht zutreffend** angezeigt werden. Für den Gewinn vor dem 1. Juli 2020 wird der geschätzte Zahlungs Monat als **nicht verfügbar** angezeigt.

In der folgenden Tabelle wird ein Beispiel für einen geschätzten Zahlungs Monat angezeigt.

| Month (Monat) | Amount |
| ------ | :-----------: |
|  Sep-2020 |  $7.273,99   |
|  Oct-2020 | $8.692,30  |
|  November-2020 | $107,89  |

Der geschätzte Betrag kann aus einer Vielzahl von Gründen von der tatsächlichen Menge abweichen:

- Restatement wird generiert: Wenn die Einnahmen neu berechnet werden, ist der tatsächliche Betrag anders.
- Anpassungen: der tatsächliche Betrag variiert abhängig von den erfolgten oder gesendeten Anpassungen.
- Regeln ändern: eine Änderung der Regeln kann die Neuberechnung in tatsächlichem Betrag widerspiegeln.
- Zahlbar: Wenn ein Zahlungs Fehler auftritt, kann der tatsächliche Betrag abweichen.

Beachten Sie, dass Ihre Zahlung nur im projizierten Monat freigegeben wird, wenn die Regeln für Schwellenwert und Zahlungs Berechtigungen Ihres Programms erfüllt sind. Diese Regeln enthalten, sind jedoch nicht auf die unten stehende Liste beschränkt:

- Ihr Steuer Profil muss auf dem neuesten Stand sein.
- Ihre Einnahmen müssen den minimalen Erstellungs Schwellenwert, der in Ihrem Programmhandbuch definiert ist, erfüllen oder überschreiten.
- Auszahlung bei Halt: Wenn Sie auf der Seite "Profil Zuweisung" die Option "meine Zahlung aufbewahren" auswählen.
- Auszahlungs Instrument nicht verfügbar: Zahlungs-oder/oder Steuer Profil ist nicht abgeschlossen.

### <a name="transaction-history-download"></a>Download von Transaktionsverläufen

Klicken Sie oben auf der Seite auf " **herunterladen** ", um weitere Details zu einem Erwerbs Bereich anzuzeigen. In der folgenden Tabelle werden die einzelnen Spalten im Bericht erläutert.

>[!NOTE]
>Der Export für den Transaktions Verlaufs Download enthält zwei neue Felder ab August 2020:
>
>- **lastpaymentcurrency**  Die Währung, in der die letzte Zahlung über alle mpns eingegangen ist, an die der derzeit angemeldete Partner Zugriff hat. Wenn keine Zahlung eingegangen ist, ist die letzte Zahlungswährung US-Dollar.
>- **earningamountinlastpaymentcurrency**  Der Erwerbs Betrag in der letzten Zahlungswährung.

| Spaltenname | Beschreibung | Anwendbarkeit für Incentive-Programme/marketplaces |
| --- | --- | --- |
| agreementEndDate | Enddatum der Vereinbarung | Incentives – nur einige Programme |
| agreementNumber | Vereinbarungsnummer | Incentives – nur einige Programme |
| agreementStartDate | Startdatum der Vereinbarung | Incentives – nur einige Programme |
| calculationDate | Datum der Berechnung der Einnahme im System | All |
| claimId | Eindeutiger Bezeichner für den Anspruch | Incentives – nur einige Programme |
| customerCountry | Land/Region des Kunden | marketplaces |
| CustomerEmail |  |  |
| customerName | Ist immer leer | Nur Incentive-Programme (Ausnahme: OEM) und marketplaces |
| customertenantid |  |  |
| distributorId | Verteiler-ID | Incentives – nur einige Programme |
| distributorName | Verteilername | Incentives – nur einige Programme |
| earningamount | Einnahmebetrag in der ursprünglichen Transaktionswährung | All |
| earningAmountInLastPaymentCurrency | Einnahmebetrag in der Währung der letzten Zahlung (leer, wenn noch keine Zahlungen geleistet wurden) |  |
| earningAmountUSD | Einnahmebetrag in US-Dollar | All |
| earningDate | Datum der Einnahme | All |
| earningExchangeRate | Wechselkurs zum Anzeigen des entsprechenden Betrags in US-Dollar | All |
| earningId | Eindeutiger Bezeichner für jede Einnahme | All |
| earningrate | Auf Transaktionsbetrag angewendete Incentive-Rate zum Generieren eines Erwerbs | All |
| earningType | Gibt an, ob es sich um eine Gebühr, einen Rabatt, Co-Op, Verkauf usw. handelt | All |
| exchangeRateDate | Datum des Wechselkurses, der zum Berechnen des Einnahmebetrags in US-Dollar verwendet wurde | All |
| externalReferenceId | Eindeutige ID für das Programm | Direkt Zahlungs Programme (Incentives und marketplaces) |
| externalReferenceIdLabel | Beschriftung der eindeutigen ID | Direkt Zahlungs Programme (Incentives und marketplaces) |
| instantrebateamount |  |  |
| "invoicedate" |  |  |
| InvoiceNumber | Rechnungsnummer (gilt nur für Enterprise) | Incentives und marketplaces-einige Programme |
| lastPaymentCurrency | Währung der letzten Zahlung (leer, wenn noch keine Zahlungen geleistet wurden) |  |
| lever | Geschäftsregel für die Einnahme | All |
| LicensingProgramName | Name des Lizenzierungsprogramms |  |
| LineItemId | Einzelne Position in der Rechnung eines Kunden |  |
| localProviderSeller | Lokaler Anbieter/Seller of Record |  |
| Reife Monat | Der geschätzte Zahlungs Monat | Alle |
| OrderId | Bezieht sich auf die Rechnung eines Kunden  | marketplaces |
| parentProductId | Eindeutige ID des übergeordneten Produkts. Wenn kein übergeordnetes Produkt für die Transaktion vorhanden ist, entspricht die ID des übergeordneten Produkts der Produkt-ID. | marketplaces |
| parentProductName | Name des übergeordneten Produkts. Wenn kein übergeordnetes Produkt für die Transaktion vorhanden ist, entspricht der Name des übergeordneten Produkts dem Produktnamen. | marketplaces |
| participantID | Primäre Identität des Partners, der unter dem Programm die Einnahme erzielt | All |
| participantIdType | Hauptsächlich Programm-ID für Incentive-Programme und Verkäufer, wenn für marketplaces | All |
| participantName | Name des Partners, der die Einnahme erzielt | All |
| partnerCountryCode | Standort/Land/Region des Partners, der die Einnahme erzielt | All |
| partNumber | Ist immer leer | Einige Incentive-Programme und-Markt Orte |
| paymentId | Eindeutige ID für die Zahlung. Diese Nummer ist normalerweise auf Ihrem Kontoauszug zu sehen | Nur SAP-Zahlungen |
| paymentStatus | Zahlungsstatus | All |
| paymentStatusDescription | Benutzerfreundliche Beschreibung des Zahlungsstatus | All |
| productId | Eindeutige Produkt-ID | marketplaces |
| ProductName | Mit der Transaktion verknüpfter Produktname | Alle |
| productType | Produkttyp, z. B. App, Add-On oder Spiel | marketplaces |
| Programmcode | Dem Programmnamen zuzuordnende Zeichenfolge |  |
| programName | Name des Incentive-/Store-Programms | All |
| purchaseOrderCoverageEndDate | Ist immer leer | Incentive-Programm – CRI |
| purchaseOrderCoverageStartDate | Ist immer leer | Incentive-Programm – CRI |
| purchaseOrderType | Ist immer leer | Incentive-Programm – CRI |
| purchaseTypeCode | Ist immer leer | Incentive-Programm – CRI |
| quantity | Abhängig vom Programm. Gibt die in Rechnung gestellte Menge für Transaktionsprogramme an | All |
| reasoncode |  |  |
| resellercountry |  |  |
| resellerId | ID des Handelspartners | Incentives – nur einige Programme |
| resellerName | Name des Handelspartners |  |
| SkuId | Die bei Veröffentlichung definierte SKU-ID. Ein Angebot kann mehrere SKUs enthalten, aber eine SKU kann nur einem einzigen Angebot zugeordnet werden. Incentives – nur einige Programme |  |
| storeFee | Der von Microsoft als Gebühr für die Bereitstellung der App oder des Add-Ons im Store einbehaltene Betrag | marketplaces |
| subscriptionEndDate | Enddatum des Abonnements | Incentives – nur einige Programme |
| subscriptionId | Abonnement-ID, die dem Kunden zugeordnet ist | Incentives – nur einige Programme |
| subscriptionStartDate | Startdatum des Abonnements | Incentives – nur einige Programme |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Partei, die für das Abführen von Steuern (Verkaufssteuer, Nutzungssteuer oder Mehrwertsteuer/Waren- und Dienstleistungssteuer) verantwortlich ist | marketplaces |
| taxRemitted | Betrag der abgeführten Steuern (Verkaufssteuer, Nutzungssteuer oder Mehrwertsteuer/Waren- und Dienstleistungssteuer) | marketplaces |
| taxState | Bundesland/Kanton des Kunden |  |
| taxzipcode | Postleitzahl des Kunden |  |
| tpan | Gibt das Ad Network (Werbenetzwerk) des Drittanbieters an | marketplaces nur anzeigen |
| transactionAmount | Transaktionsbetrag in der ursprünglichen Transaktionswährung, auf deren Basis die Einnahme generiert wird | All |
| transactionAmountUSD | Transaktionsbetrag in US-Dollar | All |
| transactionCountryCode | Code des Landes/der Region, in dem/der die Transaktion erfolgt ist |  |
| transactionCurrency | Währung, in der die ursprüngliche Kundentransaktion ausgeführt wurde (dies ist nicht die Währung für den Partnerstandort) | All |
| transactionDate | Datum der Transaktion. Nützlich für Programme, bei denen viele Transaktionen zu einer Einnahme beitragen | All |
| transactionExchangeRate | Datum des Wechselkurses zum Anzeigen des entsprechenden Transaktionsbetrags in US-Dollar | All |
| transactionId | Eindeutige ID für die Transaktion | All |
| transactionPaymentMethod | Vom Kunden für die Transaktion verwendetes Zahlungsmittel, z. B. Kreditkarte, Abrechnung des Mobilfunkanbieters oder PayPal | marketplaces |
| transactionType | Transaktionstyp, z. B. Kauf, Erstattung, Stornierung oder Rückbelastung | marketplaces |
| workload | Workload | Incentives – nur einige Programme |
|

### <a name="transaction-adjustment-codes"></a>Transaktions Anpassungs Codes

In der folgenden Tabelle werden die Ursachen Codes für Anpassungen und deren Beschreibungen aufgelistet.

|**Ursachen Code**   |**Beschreibung**   |
|------------------|:-------------------------------------|
| AR-Konformität | Anpassung, bei der die Einnahmen reduziert werden, wenn Microsoft-Rechnungen nicht rechtzeitig vom Partner bezahlt werden. |
| Co-op-Rollover | Anpassung, bei der die Zusammenführung von Co-op-Ergebnissen in einen anderen Zeitraum übertragen wird |
| OPS-Anpassung | Anpassung, die Fehler bei der Microsoft-System Berechnung korrigiert. |
| OPS-Anpassung Microsoft falsche Calc | Anpassung, mit der falsch Skalierungen korrigiert werden. |
| OPS-Anpassung Microsoft falsche Registrierung | Anpassung der in die Registrierung bezogenen falsch Skalierungen. |
| Partner Zuordnung (Abonnement) MCI/CSP | Anpassung, mit der die Abonnement falsche Ausrichtung korrigiert wird. |
| Richtlinien Ausnahme | Anpassung, die eine Programm Regel überschreibt.  |
| Ergebnis des vorherigen Zeitraums | Anpassung für das Ergebnis außerhalb des aktuellen Erwerbs Zeitraums. |

## <a name="payments"></a>Zahlungen

Auf der Seite **Zahlungen** finden Sie Informationen zu den Kosten, die Sie mit Microsoft erworben haben. Außerdem wird gezeigt, wann und wie viel Sie bezahlt werden.

>[!Note]
> Qualifiziert für eine Auszahlung sind Beträge, die den [Zahlungsschwellenwert](payment-thresholds-methods-timeframes.md) von 50 US-Dollar erreichen. Weitere Informationen finden Sie in der [Microsoft-Herausgeber Vereinbarung](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Übersichtsseite &quot;Zahlungen&quot;.":::

- **Summe bezahlt in diesem Jahr** – die kombinierte Summe, die Sie in diesem Jahr in US-Dollar für alle Programme bezahlt haben.
- **Nächste geschätzte Zahlung** – die nächste nächste Zahlung an Sie (auch wenn in Kürze andere vorhanden sind), in US-Dollar.
- **Letzte Zahlung** – der Betrag (in US-Dollar), der Programmname und das Programm Ihrer letzten Zahlung.
- **Zahlung nach Quelle** – Betrag der Zahlungen (in US-Dollar) pro Programm in den letzten 12 Monaten.

### <a name="payments-list"></a>Zahlungs Liste

**In der Liste mit den Zahlungs** Tabellen werden kostenpflichtige und ausstehende Zahlungen angezeigt. Sie können die Steuerinformationen für die Dienstgebühr im PDF-Format herunterladen und die Details zu den Details für eine bestimmte Zahlung anzeigen.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Transaktionsverlauf exportieren":::

- **Bezahlt** – alle Zahlungen wurden erfolgreich gesendet. Wählen Sie das Jahr im Dropdown Menü aus, um die in diesem Jahr veröffentlichten Zahlungen zu filtern.
- **Ausstehende** – bevorstehende Zahlungen.
- **Service Payment Tax (PDF-Format)** – verfügbar für die Zahlungen, die für die Gebühr für die Dienstgebühr unterliegen. Die Gebühren für die Dienstgebühr werden in **anderen Steuern** angezeigt.
- **View** – leitet eine Umleitung zum Transaktionsverlauf mit einer Liste der in die Zahlung enthaltenen Einnahmen um.

Informationen dazu, warum Sie möglicherweise fehlende oder unerwartete Einnahmen haben, finden Sie unter [häufig gestellte Fragen zu kommerziellen Marketplace-Auszahlungen](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Zahlungsstatus

In der folgenden Tabelle werden die verschiedenen Erwerbsstatus erläutert.

| Einnahmenstatus | `Reason` | Partneraktion erforderlich? |
| --- | --- | --- |
| Nicht verarbeitet | Die Einnahme ist für eine Auszahlung qualifiziert. Sie verbleibt in diesem Zustand für einen kühl Zeitraum, wie im Programmhandbuch für das Incentives-Programm definiert. | Nein |
| Anstehend | Der Zahlungsauftrag hat ausstehende interne Überprüfungen generiert, bevor die Zahlung verarbeitet wird. | Nein |
| Ausstehende Steuerrechnung | Ihre Steuerrechnung ist unvollständig oder ungültig. | Sie müssen Ihre Steuerrechnung aktualisieren, bevor Sie bezahlt werden können. |
| Bei Überprüfung abgelehnt | Die Zahlung wurde während der Überprüfung abgelehnt. | Wenden Sie sich an den Microsoft-Support, um weitere Informationen zu erhalten. |
| Fehler | Die Zahlung ist aufgrund eines Microsoft-Systemfehlers fehlgeschlagen. | Weitere Informationen erhalten Sie vom Microsoft Support. |
| In Bearbeitung | Die Zahlung wird ausgeführt. | Nein |
| Falsche Zahlung | Der Zahlungsvorgang wird wiederholt. | Nein |
| Gesendet | Die Zahlung wurde an Ihre Bank gesendet. | Nein |
| Erneute Verarbeitung | Bei der Zahlung ist ein Microsoft-Systemfehler aufgetreten, der erneut verarbeitet wird. | Nein |
| Reversed | Die Zahlung wurde von Ihrer Bank rückgängig gemacht und wird im nächsten Zahlungszeitraum erneut gesendet. | Nein |
| Steuerrechnung abgelehnt | Ihre Steuerrechnung wurde während der Überprüfung abgelehnt. Alle ausstehenden Zahlungen werden zurückgehalten, bis die Überprüfung der Steuerrechnung abgeschlossen ist. | Weitere Informationen erhalten Sie vom Microsoft Support. |
| Steuerrechnung wird geprüft | Ihre Steuerrechnung wird geprüft. Ihre Zahlung wird freigegeben, sobald die Steuerrechnung genehmigt wurde. | Nein |
| Rejected (Abgelehnt) | Die Zahlung wurde von Ihrer Bank abgelehnt. | Weitere Informationen erhalten Sie von Ihrer Bank. |
|

### <a name="payments-download"></a>Download der Zahlungen

 In der folgenden Tabelle werden die einzelnen Spalten im Bericht erläutert. Klicken Sie oben auf der Seite Zahlungen auf **herunterladen** , um weitere Details zu ihren Zahlungen anzuzeigen.

| Spaltenname | BESCHREIBUNG |
| --- | --- |
| participantID | Primäre Identität des Partners, der unter dem Programm die Einnahme erzielt |
| participantIDType | Normalerweise Programm-ID für Incentives-Programme und Verkäufer-ID für Store-Programme |
| participantName | Name des Partners, der die Einnahme erzielt |
| programName | Incentives/Name des Speicher Programms |
| earned | Einnahmebetrag in der Auszahlungswährung für diese Programm-/Teilnehmer-ID |
| earnedUSD | Einnahmebetrag für die Programm-/Teilnehmer-ID in US-Dollar |
| withheldTax | Einbehaltener Steuerbetrag in der Auszahlungswährung für die Programm-/Teilnehmer-ID |
| salesTax | Gesamtbetrag der Umsatzsteuer in der Zahlen-zu-Währung für das Programm/die participantid (gilt nur für Incentives-Programme) |
| serviceFeeTax | Gesamtbetrag der Steuer auf Servicegebühren in der Auszahlungswährung für die Programm-/Teilnehmer-ID (gilt nur für Store-Programme und Azure Marketplace) |
| totalPayment | Gesamtzahlung in der lokalen Währung ohne einbehaltene Steuern und einschließlich Verkaufssteuer (falls zutreffend) für die Programm-/Teilnehmer-ID |
| currencyCode | Code der Auszahlungswährung |
| paymentMethod | Die Methode, mit der der Partner bezahlt wird, z. B. Banküberweisung, Gutschrift |
| paymentID | Eindeutige ID für die Zahlung. Diese Nummer ist normalerweise auf Ihrem Kontoauszug zu sehen (gilt nur für SAP-Zahlungen). |
| paymentStatus | Zahlungsstatus |
| paymentStatusDescription | Benutzerfreundliche Beschreibung des Zahlungsstatus |
| paymentDate | Datum, an dem die Zahlung von Microsoft gesendet wurde |
|

## <a name="export-data"></a>Exportieren von Daten

Die Seite " **Daten exportieren** " wird nicht eigenständig aktualisiert. Möglicherweise müssen Sie die Seite manuell aktualisieren, um die neuesten Daten anzuzeigen. Wählen Sie aus den drei Registerkarten aus, um entweder **Transaktionsverlauf**, **Zahlungen**, **Transaktions Zusammenfassung** oder Verlaufs **Anweisung** zu exportieren.

Der Filter führt möglicherweise zu einem Fehler, der **nicht verfügbar** ist. Dies kann vorkommen, wenn Sie den Standard Zeitraum in drei Monaten ausgewählt haben und dann eine Zahlungs-ID aus einem Verdienst ausgewählt haben, das außerhalb dieses Zeitraums liegt. Wenn dies der Fall ist, erweitern Sie den Zeitraum, und versuchen Sie es noch mal.

Hier ist ein Beispiel für einen Export von Zahlungen:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Exportieren von Zahlungs Berichten.":::

### <a name="historical-statements"></a>Historische Auszüge

Die Zusammenfassung **Daten exportieren** bietet auch Zugriff auf Verlaufs Anweisungen.

> [!NOTE]
> Eine Verlaufs Anweisung ist eine Momentaufnahme und wird nicht aktualisiert. Wenden Sie sich an den [Support](https://partner.microsoft.com/support/v2/?stage=1) , und fordern Sie bei Bedarf die neuesten Daten an

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportieren von Verlaufs Anweisungen.":::

- Der Transaktionsverlauf von vor dem 1. Juli 2019 wird separat behandelt und verwendet andere Felder aus späteren Verlaufs Berichten.
- Der Legacy Transaktionsverlauf verfügt über eine Spalte mit dem Namen "reserviert", die der Spalte "Gewinn" im modernen Verlauf entspricht, mit dem Unterschied, dass alle Gewinne mit dem Status "Payment sent" ausgeschlossen werden.
- Filter wie „3M“, „6M“ oder „12M“ gelten nicht für den Abschnitt Historische Auszüge.

### <a name="historical-statement-downloads"></a>Downloads der historischen Anweisung

In der folgenden Tabelle werden die einzelnen Spalten in einer Verlaufs Anweisung erläutert.

| Feldname | BESCHREIBUNG |
| --- | --- |
| Umsatzquelle | Die Quelle Ihres Umsatzes basierend auf dem Ursprungsort der Transaktion, z. B. Microsoft Store, Windows Phone Store, Windows Store 8 oder Werbung |
| Bestell-ID | Eindeutiger Bestellungsbezeichner. Mit dieser ID können Sie Kauftransaktionen mit den jeweiligen Nicht-Kauftransaktionen, z. B. Rückerstattungen oder Rückzahlungen, identifizieren. Beide weisen die gleiche Bestell-ID auf. Wenn eine geteilte Gebühr vorliegt, bei der mehrere Zahlungsmethoden für einen einzelnen Kauf verwendet wurden, können Sie die Kauf Transaktionen auch verknüpfen. |
| TransactionID | Eindeutiger Transaktionsbezeichner. |
| Datum/Uhrzeit der Transaktion | Das Datum und die Uhrzeit, zu der die Transaktion stattfand (UTC). |
| Übergeordnete Produkt-ID | Eindeutige ID des übergeordneten Produkts. Wenn kein übergeordnetes Produkt für die Transaktion vorhanden ist, entspricht die ID des übergeordneten Produkts der Produkt-ID. |
| Product ID | Eindeutiger Produktbezeichner. |
| Übergeordneter Produktname | Name des übergeordneten Produkts. Wenn kein übergeordnetes Produkt für die Transaktion vorhanden ist, entspricht der Name des übergeordneten Produkts dem Produktnamen. |
| Produktname | Name des Produkts |
| Produkttyp | Produkttyp, z. B. App, Add-On oder Spiel |
| Menge | Wenn Microsoft Store für Unternehmen die Umsatzquelle ist, stellt die Menge die Anzahl der erworbenen Lizenzen dar. Bei allen anderen Umsatzquellen ist die Menge immer 1. Auch wenn eine einzelne Transaktion in zwei Positionen aufgeteilt ist, weil zwei verschiedene Zahlungsmethoden verwendet wurden, wird für jede Position eine Menge von 1 angezeigt. |
| Transaktionstyp | Transaktionstyp, z. B. Kauf, Erstattung, Stornierung oder Rückbelastung |
| Zahlungsmethode | Vom Kunden für die Transaktion verwendetes Zahlungsmittel, z. B. Kreditkarte, Abrechnung des Mobilfunkanbieters oder PayPal |
| Land/Region | Land/Region, in dem/der die Transaktion stattfand |
| Lokaler Anbieter/Verkäufer | Lokaler Anbieter/Seller of Record |
| Transaktionswährung | Währung der Transaktion |
| Transaktionsbetrag | Betrag der Transaktion |
| Bezahlte Steuern | Betrag der abgeführten Steuern (Verkaufssteuer, Nutzungssteuer oder Mehrwertsteuer/Waren- und Dienstleistungssteuer) |
| Nettoeinnahmen | Transaktionsbetrag abzüglich abgeführter Steuern |
| Store-Gebühr | Der von Microsoft als Gebühr für die Bereitstellung der App oder des Add-Ons im Store einbehaltene Prozentsatz der Nettoeinnahmen |
| App-Erlöse | Nettoeinnahmen abzüglich Store-Gebühr |
| Einbehaltene Steuern | Betrag der einbehaltenen Einkommenssteuern (nicht in CSV-Datei **Reserviert** enthalten) |
| payment | App-Erlöse abzüglich aller anwendbaren Einkommenssteuereinbehalte (Betrag in Transaktionswährung) Nicht in CSV-Datei **Reserviert** enthalten. |
| Wechselkurs | Zum Umrechnen der Transaktionswährungen in die Zahlungswährung verwendeter Wechselkurs |
| Zahlungswährung | Währung, in der Ihre Zahlung erfolgt |
| Umgerechnete Zahlung | Zahlungsbetrag, der anhand des Wechselkurses in die Zahlungswährung umgerechnet wurde |
| Steuerzahlungsmodell | Partei, die für das Abführen von Steuern (Verkaufssteuer, Nutzungssteuer oder Mehrwertsteuer/Waren- und Dienstleistungssteuer) verantwortlich ist |
| Datum/Uhrzeit der Berechtigung | Das Datum und die Uhrzeit, zu der Transaktionserlöse auszahlungsberechtigt werden (UTC). Beim Erstellen einer Auszahlung enthält diese Transaktionserlöse mit einem Berechtigungsdatum, das vor dem Erstellungsdatum der Auszahlung liegt (nur in CSV-Datei **Reserviert** enthalten). |
| Charges | Zeigt eine Aufschlüsselung aller in der Spalte „Transaktionsbetrag“ aggregierten Gebührendetails (nur für Azure Marketplace enthalten; nicht in CSV-Datei **Reserviert** enthalten). |
|||

## <a name="next-steps"></a>Nächste Schritte

- [Partnerauszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Auszahlungsrichtliniendetails](payout-policy-details.md)
- Abrechnungsunterstützung erhalten Sie vom [Support für Herausgeber](https://partner.microsoft.com/support/v2/?stage=1).
