---
title: Auszahlungsauszüge
description: Erfahren Sie mehr über Auszahlungsauszüge und -zusammenfassungen sowie über das Anzeigen und Exportieren Ihrer Zahlungsdaten aus Microsoft Partner Center.
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: 4e9ab721fe356dbcdff7316a5ed5b52c81f2d4eb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152595"
---
# <a name="payout-statements"></a>Auszahlungsauszüge

**Geeignete Rollen:** Kontoadministrator-| Globaler Administrator

Der **Auszahlungsauszug** bietet eine Übersicht über Ihre Auszahlungen von Angeboten, die über den kommerziellen Marketplace verkauft werden. Sie zeigt den Transaktionsverlauf Ihrer Einnahmen an, schätzt ihre nächste Zahlung und zeigt Zahlungstrends an. Sie können auch den Transaktionsverlauf und Zahlungsanweisungen herunterladen. In diesem Artikel wird erläutert, wie Sie auf Ihren Auszahlungsauszug und die verschiedenen Auszahlungsseiten und Downloads zugreifen, auf die Sie in Partner Center zugreifen können.

>[!NOTE]
>Es werden nur Daten für MPN-IDs und Programme angezeigt, denen Sie zugeordnet sind. Wenn Sie zusätzliche Daten anzeigen möchten, wenden Sie sich an Ihren Kontoadministrator, um Berechtigungen zu erhalten. 

## <a name="roles-and-permissions"></a>Rollen und Berechtigungen

Um auf einen Auszahlungsauszug zugreifen zu können, muss Ihnen die Rolle **Kontobesitzer** oder **Finanzmitwirkender** zugewiesen sein.

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

## <a name="access-your-payout-statement"></a>Zugreifen auf Ihren Auszahlungsauszug

Melden Sie sich bei [Partner Center](https://partner.microsoft.com/dashboard/home) an, und wählen Sie das Auszahlungssymbol in der oberen rechten Ecke des Bildschirms aus, um auf diese verschiedenen Zusammenfassungen zuzugreifen:

- Transaktionsverlauf
- Zahlungen
- Exportieren von Daten

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Veranschaulicht das Auszahlungssymbol in der oberen rechten Ecke des Partner Center-Portals":::

Sie können auch die [Partnerauszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts) verwenden, um direkt eine Verbindung mit Auszahlungstransaktionen und Zahlungsdaten herzustellen und diese abzurufen.


## <a name="transaction-history"></a>Transaktionsverlauf

Auf der Seite **Transaktionsverlauf** werden die Zusammenfassung Ihrer Einnahmen, die geschätzte nächste Zahlung sowie Der Umsatz- und Zahlungstrend der letzten 36 Monate angezeigt. Sie können auch Transaktionsdetails aus diesem Abschnitt herunterladen.<br><br>In diesem Bericht werden alle auszahlungsfähigen Einnahmen angezeigt, einschließlich der noch nicht gesendeten Zahlungen. Einnahmen sind zur Auszahlung berechtigt, wenn ein ISV alle Bank- und Steuerinformationen in Partner Center abgeschlossen hat, >50 USD erworben hat, das ISV-Konto aktiv ist und dem Kunden (für EA-Transaktionen) oder die Zahlung (für Nicht-EA-Transaktionen) in Rechnung gestellt wurde.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Transaktionsübersicht.":::

- **In diesem Jahr gesendete Einnahmen:** Die Gesamteinnahmen und die Aufschlüsselung der Einnahmen, die bezahlt wurden und im nächsten Monat bezahlt werden.
- **Geschätzter Zahlungsmonat:** Die insgesamt in den kommenden Monaten erwarteten Einnahmen.
- **Einnahmen- und Zahlungstrend:** Monatliche Einnahmen- und Zahlungsbeträge der letzten 36 Monate.
- **Herunterladen:** Laden Sie Transaktionsdetails im CSV- oder TSV-Format herunter.

Verwenden Sie die Datumsbereichsauswahl in der oberen rechten Ecke der Seite, um die Ausgabe der Seite so zu filtern, dass die letzten 3, 6, 12 oder 36 Monate angezeigt werden. Oder wählen Sie einen benutzerdefinierten Datumsbereich von bis zu 36 Monaten aus. Der Standarddatumsbereich beträgt 12 Monate. Sie können auch nach Registrierungs-ID, Programm, Zahlungs-ID, Einnahmentyp, Hebel und Status filtern. Daten sind für das aktuelle Geschäftsjahr (1. Juli bis 30. Juni) und die beiden vorherigen Geschäftsjahre verfügbar.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Der Suchfilter oben rechts auf der Seite.":::

Zum Anzeigen weiterer Details zu einer Einnahme klicken Sie rechts auf der Seite auf den Pfeil nach unten. Dadurch werden Hebel, Umsatzbetrag, Produkt und Kunde angezeigt. Wenn diese Daten aus irgendeinem Grund nicht verfügbar sind, Sie aber Zugriff darauf benötigen, wenden Sie sich an den Support. Wenn die Einnahmen das Ergebnis einer Anpassung und keine Transaktion sind, werden die Felder Produkt und Kunde nicht angezeigt.

### <a name="transaction-history-summary"></a>Zusammenfassung des Transaktionsverlaufs

In dieser Ansicht werden Einnahmendetails angezeigt, einschließlich des Ursprungs der Einnahmen aus dem verkauften Produkt, dem Status und dem geschätzten Zahlungsmonat.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Transaktionsverlauf.":::

- **Earned date** (Erwerbsdatum) – Das Kaufdatum.
- **Einnahmentyp:** Die Art der Einnahmen, z. B. Verkaufen, Besendung oder Co-Op.
- **Gesamtbetrag:** Der Nettogewinnbetrag. Im kommerziellen Marketplace bedeutet dies, dass die Standard-Marketplace-Gebühr abgezogen wurde.
- **Status:** Verfügt über drei Optionen:
    - **Anstehend:** Die Einnahmen befinden sich in einem ausstehenden Kühlzeitraum.
    - **Verarbeitet:** Einnahmen werden für die nächste Zahlung vorbereitet.
    - **Gesendet:** Die Einnahmen wurden bezahlt.
- **Geschätzter Zahlungsmonat:** Der Monat, in dem die Einnahmen voraussichtlich bezahlt werden. Weitere Informationen finden Sie im [nächsten Abschnitt.](#estimated-payment-month)

Einnahmentransaktionen werden angezeigt, sobald die Transaktion die Auszahlungsberechtigung erfüllt. Informationen dazu, warum Sie möglicherweise fehlende oder unerwartete Einnahmen haben, finden Sie unter [Allgemeine Fragen zu Auszahlungen](payout-faq.md#why-are-my-earnings-missing)für den kommerziellen Marketplace.

#### <a name="estimated-payment-month"></a>Geschätzter Zahlungsmonat

Die Seite Transaktionsverlauf enthält jetzt eine Tabelle mit Ihren geschätzten Zahlungsbeträgen für die nächsten Monate. Sie können diese Informationen auch in den Exporten transaktionsverlauf und Zusammenfassungsbericht anzeigen und herunterladen. Diese Informationen erleichtern Abstimmungen und Zahlungsprognosen.

Der geschätzte Zahlungsmonat wird basierend auf Programmkonfigurationsregeln und Zeitplänen berechnet und im nächsten/bevorstehenden Zahlungszyklus verarbeitet.

Der geschätzte Zahlungsmonat ist derzeit für alle Einnahmenarten verfügbar, mit Ausnahme der Co-Op, die als **Nicht zutreffend** angezeigt wird. Für Einnahmen vor dem 1. Juli 2020 wird der geschätzte Zahlungsmonat als **Nicht verfügbar** angezeigt.

Die folgende Tabelle zeigt ein Beispiel für einen geschätzten Zahlungsmonat.

| Month | Amount (Betrag) |
| ------ | :-----------: |
|  Sep-2020 |  7.273,99 USD   |
|  Oktober 2020 | 8.692,30 USD  |
|  Nov. 2020 | 107,89 USD  |

Der geschätzte Betrag kann aus verschiedenen Gründen vom tatsächlichen Betrag abweichen:

- Neuberechnung der Einnahmen: Wenn die Einnahmen neu berechnet werden, ist der tatsächliche Betrag unterschiedlich.
- Anpassungen: Der tatsächliche Betrag variiert je nach vorgenommenen oder übermittelten Anpassungen.
- Regeländerung: Eine Änderung der Regeln kann eine Neuberechnung des tatsächlich bezahlten Betrags widerspiegeln.
- Bezahlbar: Wenn ein Zahlungsfehler auftritt, kann der tatsächliche Betrag unterschiedlich sein.

Beachten Sie, dass Ihre Zahlung nur im voraussichtlichen Monat freigegeben wird, wenn die Schwellenwert- und Zahlungsberechtigungsregeln Ihres Programms erfüllt sind. Diese Regeln umfassen, sind aber nicht auf die folgende Liste beschränkt:

- Ihr Steuerprofil muss auf dem neuesten Stand sein.
- Ihre Einnahmen müssen den in Ihrem Programmleitfaden definierten Mindestverdienungsschwellenwert erfüllen oder überschreiten.
- Zurückbehaltene Auszahlung: Wenn Sie auf der Profilzuweisungsseite die Option "Meine Zahlung zurückhalten" auswählen.
- Auszahlungsinstrument nicht verfügbar: Zahlung oder/und Steuerprofil sind nicht abgeschlossen.

### <a name="transaction-history-download"></a>Download von Transaktionsverläufen

Klicken Sie oben auf der Seite auf **Herunterladen,** um weitere Details zu einer Einnahmen anzuzeigen. In der folgenden Tabelle wird jede Spalte im Bericht erläutert.

>[!NOTE]
>Der Export des Transaktionsverlaufsdownloads verfügt ab August 2020 über zwei neue Felder:
>
>- **lastPaymentCurrency**  Die Währung, in der die letzte Zahlung empfangen wurde, für alle MPNs, auf die der derzeit angemeldete Partner Zugriff hat. Wenn keine Zahlung empfangen wird, ist die letzte Zahlungswährung US-Dollar.
>- **earningAmountInLastPaymentCurrency**  Der Einnahmenbetrag in der Währung der letzten Zahlung.

| Spaltenname | BESCHREIBUNG | Anwendbarkeit für Incentive-Programme/Marketplaces |
| --- | --- | --- |
| agreementEndDate | Enddatum der Vereinbarung | Incentives – nur einige Programme |
| agreementNumber | Vereinbarungsnummer | Incentives – nur einige Programme |
| agreementStartDate | Startdatum der Vereinbarung | Incentives – nur einige Programme |
| calculationDate | Datum der Berechnung der Einnahme im System | All |
| claimId | Eindeutiger Bezeichner für den Anspruch | Incentives – nur einige Programme |
| customerCountry | Land/Region des Kunden | marketplaces |
| customerEmail |  |  |
| customerName | Kann leer sein. | Nur Incentive-Programme (Ausnahme: OEM) und Marketplaces. Für CSP-Transaktionen wird in Marketplaces der Name des CSP angezeigt. |
| customerTenantId |  |  |
| distributorId | Verteiler-ID | Incentives – nur einige Programme |
| distributorName | Verteilername | Incentives – nur einige Programme |
| earningamount | Einnahmebetrag in der ursprünglichen Transaktionswährung | All |
| earningAmountInLastPaymentCurrency | Einnahmebetrag in der Währung der letzten Zahlung (leer, wenn noch keine Zahlungen geleistet wurden) |  |
| earningAmountUSD | Einnahmebetrag in US-Dollar | All |
| earningDate | Datum der Einnahme | All |
| earningExchangeRate | Wechselkurs zum Anzeigen des entsprechenden Betrags in US-Dollar | All |
| earningId | Eindeutiger Bezeichner für jede Einnahme | All |
| earningrate | Incentives-Rate, die auf den Transaktionsbetrag angewendet wird, um eine Einnahmen zu generieren | All |
| earningType | Gibt an, ob es sich um eine Gebühr, einen Rabatt, Co-Op, Verkauf usw. handelt | All |
| exchangeRateDate | Datum des Wechselkurses, der zum Berechnen des Einnahmebetrags in US-Dollar verwendet wurde | All |
| externalReferenceId | Eindeutige ID für das Programm | Direct Pay-Programme (Incentives und Marketplaces) |
| externalReferenceIdLabel | Beschriftung der eindeutigen ID | Direct Pay-Programme (Incentives und Marketplaces) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| InvoiceNumber | Rechnungsnummer (gilt nur für Unternehmen) | Incentives und Marketplaces – nur einige Programme |
| lastPaymentCurrency | Währung der letzten Zahlung (leer, wenn noch keine Zahlungen geleistet wurden) |  |
| lever | Geschäftsregel für die Einnahme | All |
| LicensingProgramName | Name des Lizenzierungsprogramms |  |
| LineItemId | Einzelne Position in der Rechnung eines Kunden |  |
| localProviderSeller | Lokaler Anbieter/Seller of Record |  |
| Fälligkeitsmonat | Der geschätzte Zahlungsmonat | Alles |
| OrderId | Bezieht sich auf die Rechnung eines Kunden  | marketplaces |
| parentProductId | Eindeutige ID des übergeordneten Produkts. Wenn kein übergeordnetes Produkt für die Transaktion vorhanden ist, entspricht die ID des übergeordneten Produkts der Produkt-ID. | marketplaces |
| parentProductName | Name des übergeordneten Produkts. Wenn kein übergeordnetes Produkt für die Transaktion vorhanden ist, entspricht der Name des übergeordneten Produkts dem Produktnamen. | marketplaces |
| participantID | Primäre Identität des Partners, der unter dem Programm die Einnahme erzielt | All |
| participantIdType | Größtenteils Programm-ID für Incentive-Programme und Verkäufer-IF für Marketplaces | All |
| participantName | Name des Partners, der die Einnahme erzielt | All |
| partnerCountryCode | Standort/Land/Region des Partners, der die Einnahme erzielt | All |
| partNumber | Ist immer leer | Einige Incentiveprogramme und Marketplaces |
| paymentId | Eindeutiger Bezeichner zum Korrelieren aller Transaktionen im Transaktionsbericht mit einer bestimmten Zahlung im Zahlungsbericht | Alles |
| paymentStatus | Zahlungsstatus | All |
| paymentStatusDescription | Benutzerfreundliche Beschreibung des Zahlungsstatus | All |
| productId | Eindeutige Produkt-ID | marketplaces |
| ProductName | Mit der Transaktion verknüpfter Produktname | Alles |
| productType | Produkttyp, z. B. App, Add-On oder Spiel | marketplaces |
| Programmcode | Dem Programmnamen zuzuordnende Zeichenfolge |  |
| programName | Name des Incentive-/Store-Programms | All |
| purchaseOrderCoverageEndDate | Ist immer leer | Incentive-Programm – CRI |
| purchaseOrderCoverageStartDate | Ist immer leer | Incentive-Programm – CRI |
| purchaseOrderType | Ist immer leer | Incentive-Programm – CRI |
| purchaseTypeCode | Ist immer leer | Incentive-Programm – CRI |
| quantity | Abhängig vom Programm. Gibt die in Rechnung gestellte Menge für Transaktionsprogramme an | All |
| reasonCode |  |  |
| resellerCountry |  |  |
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
| tpan | Gibt das Ad Network (Werbenetzwerk) des Drittanbieters an | Nur Marketplaces Ads |
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

### <a name="transaction-adjustment-codes"></a>Transaktionsanpassungscodes

In der folgenden Tabelle sind die Ursachencodes für Anpassungen und deren Beschreibungen aufgeführt.

|**Grundcode**   |**Beschreibung**   |
|------------------|:-------------------------------------|
| AR-Konformität | Anpassung, die die Einnahmen reduziert, wenn Microsoft-Rechnungen nicht vom Partner zeitsentspricht. |
| Co-Op-Rollover | Anpassung, die Co-Op-Einnahmen auf einen anderen Zeitraum überträgt oder Co-Op-Einnahmen in Bereinigte umvertiert. |
| Ops-Anpassung | Anpassung, die Microsoft-Systemberechnungsfehler korrigiert. |
| Ops Adjustment Microsoft incorrect calc | Anpassung, die Fehlberechnungen korrigiert. |
| Ops Adjustment Microsoft incorrect enrollment | Anpassung für registrierungsbezogene Fehlberechnungen. |
| Partnerzuordnung (Abonnement) MCI/CSP | Anpassung, die die falsche Ausrichtung des Abonnements korrigiert. |
| Richtlinienausnahme | Anpassung, die eine Programmregel überschreibt.  |
| Einnahmen im vorherigen Zeitraum | Anpassung für Einnahmen außerhalb des aktuellen Einnahmenzeitraums. |

## <a name="payments"></a>Zahlungen

Auf **der Seite** Zahlungen wird das Geld angezeigt, das Sie mit Microsoft verdient haben. Außerdem wird gezeigt, wann und wie viel Sie bezahlen.

>[!Note]
> Qualifiziert für eine Auszahlung sind Beträge, die den [Zahlungsschwellenwert](payment-thresholds-methods-timeframes.md) von 50 US-Dollar erreichen. Weitere Informationen finden Sie in der [Microsoft-Herausgebervereinbarung.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Übersichtsbildschirm für Zahlungen.":::

- **In diesem Jahr gezahlter Gesamtbetrag:** Die gesamt an Sie in diesem Jahr in US-Dollar für alle Ihre Programme gezahlte Summe.
- **Nächste geschätzte Zahlung:** Die nächste einzelne Zahlung in US-Dollar (auch wenn weitere in Kürze verfügbar sind).
- **Letzte Zahlung:** Der Betrag (in US-Dollar), der Programmname und das Programm Ihrer letzten Zahlung.
- **Zahlung nach Quelle:** Die Höhe der Zahlungen (in US-Dollar) pro Programm in den letzten 12 Monaten.

### <a name="payments-list"></a>Zahlungsliste

In der Tabelle **Liste der Zahlungen** werden bezahlte und ausstehende Zahlungen angezeigt. Sie können Die Steuerinformationen zur Dienstgebühr im PDF-Format herunterladen und die Einnahmendetails für eine bestimmte Zahlung anzeigen.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportieren des Transaktionsverlaufs":::

- **Bezahlt:** Alle erfolgreich gesendeten Zahlungen. Wählen Sie im Dropdownmenü das Jahr aus, um nach den in diesem Jahr freigegebenen Zahlungen zu filtern.
- **Ausstehend:** Bevorstehende Zahlungen.
- **Dienstgebührensteuer (PDF-Formular):** Steht für die Zahlungen zur Verfügung, für die eine Dienstgebühr erhoben wird. Steuern von Dienstgebühren werden unter **Andere Steuern** angezeigt.
- **Ansicht:** Leitet zum Transaktionsverlauf mit einer Liste der in der Zahlung enthaltenen Einnahmen um.

Informationen dazu, warum Sie möglicherweise fehlende oder unerwartete Einnahmen haben, finden Sie unter [Allgemeine Fragen zu Auszahlungen](payout-faq.md#why-are-my-earnings-missing)für den kommerziellen Marketplace.

### <a name="payment-status"></a>Zahlungsstatus

In der folgenden Tabelle werden die verschiedenen Einnahmenstatus erläutert.

| Einnahmenstatus | `Reason` | Partneraktion erforderlich? |
| --- | --- | --- |
| Nicht verarbeitet | Die Einnahme ist für eine Auszahlung qualifiziert. Er verbleibt in diesem Zustand für einen Kühlzeitraum, wie im Programmleitfaden für die Incentives-Programm definiert. | Nein |
| Anstehend | Der Zahlungsauftrag hat ausstehende interne Überprüfungen generiert, bevor die Zahlung verarbeitet wird. | Nein |
| Ausstehende Steuerrechnung | Ihre Steuerrechnung ist unvollständig oder ungültig. | Sie müssen Ihre Steuerrechnung aktualisieren, bevor Sie bezahlt werden können. |
| Bei Überprüfung abgelehnt | Die Zahlung wurde während der Überprüfung abgelehnt. | Wenden Sie sich an den Microsoft-Support, um weitere Informationen zu erhalten. |
| Fehler | Die Zahlung ist aufgrund eines Microsoft-Systemfehlers fehlgeschlagen. | Wenden Sie sich an den Microsoft-Support, um Weitere Informationen zu erhalten. |
| In Bearbeitung | Die Zahlung wird in Bearbeitung. | Nein |
| Falsche Zahlung | Die Erneute Zahlung wird in Bearbeitung. | Nein |
| Gesendet | Die Zahlung wurde an Ihre Bank gesendet. | Nein |
| Erneute Verarbeitung | Bei der Zahlung ist ein Microsoft-Systemfehler aufgetreten, und die Zahlung wird erneut verarbeitet. | Nein |
| Reversed | Die Zahlung wurde von Ihrer Bank rückgängig gemacht und wird im nächsten Zahlungszyklus erneut gesendet. | Nein |
| Steuerrechnung abgelehnt | Ihre Steuerrechnung wurde während der Überprüfung abgelehnt. Alle ausstehenden Zahlungen werden zurückgehalten, bis die Überprüfung der Steuerrechnung abgeschlossen ist. | Wenden Sie sich an den Microsoft-Support, um Weitere Informationen zu erhalten. |
| Steuerrechnung wird geprüft | Ihre Steuerrechnung wird geprüft. Ihre Zahlung wird freigegeben, sobald die Steuerrechnung genehmigt wurde. | Nein |
| Rejected (Abgelehnt) | Die Zahlung wurde von Ihrer Bank abgelehnt. | Weitere Informationen erhalten Sie von Ihrer Bank. |
|

### <a name="payments-download"></a>Zahlungsdownload

 In der folgenden Tabelle wird jede Spalte im Bericht erläutert. Um weitere Details zu Ihren Zahlungen anzuzeigen, wählen Sie **oben** auf der Seite Zahlungen die Option Herunterladen aus.

| Spaltenname | BESCHREIBUNG |
| --- | --- |
| participantID | Primäre Identität des Partners, der unter dem Programm die Einnahme erzielt |
| participantIDType | Normalerweise Programm-ID für Incentives-Programme und Verkäufer-ID für Store-Programme |
| participantName | Name des Partners, der die Einnahme erzielt |
| programName | Incentives/Store-Programmname |
| earned | Einnahmebetrag in der Auszahlungswährung für diese Programm-/Teilnehmer-ID |
| earnedUSD | Einnahmebetrag für die Programm-/Teilnehmer-ID in US-Dollar |
| withheldTax | Einbehaltener Steuerbetrag in der Auszahlungswährung für die Programm-/Teilnehmer-ID |
| salesTax | Total amount of sales tax in the Pay To currency for the program/participantID (Total amount of sales tax in the Pay To currency for the program/participantID (gilt nur für Incentives-Programme) |
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

Die **Seite Daten** exportieren wird nicht allein aktualisiert. Möglicherweise müssen Sie die Seite manuell aktualisieren, um die neuesten Daten anzuzeigen. Wählen Sie auf den drei Registerkarten aus, um entweder den **Transaktionsverlauf,** **Zahlungen,** **die Transaktionszusammenfassung** oder die **verlaufsverlaufs-Anweisung zu exportieren.**

Ihr Filter kann zu einem Fehler **Keine Daten verfügbar** führen. Dies kann passieren, wenn Sie den ausgewählten Standardzeitraum bei drei Monaten be lassen und dann eine Zahlungs-ID aus einer Einnahmen ausgewählt haben, die außerhalb dieses Zeitraums liegt. Erweitern Sie in diesem Fall Ihren Zeitraum, und versuchen Sie es erneut.

Hier sehen Sie einen Beispielexport für Zahlungen:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Exportieren des Zahlungsberichts.":::

### <a name="historical-statements"></a>Historische Auszüge

Die Datenzusammenfassung **Exportieren** bietet auch Zugriff auf Verlaufsanweisungen.

> [!NOTE]
> Eine Verlaufs-Anweisung ist eine Momentaufnahme und wird nicht aktualisiert. Wenden Sie sich an den [Support,](https://partner.microsoft.com/support/v2/?stage=1) und fordern Sie bei Bedarf die neuesten Daten an.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportieren sie Verlaufsanweisungen.":::

- Der Transaktionsverlauf vor dem 1. Juli 2019 wird separat behandelt und verwendet andere Felder aus späteren Verlaufsberichten.
- Der Legacytransaktionsverlauf verfügt über eine Spalte namens "Reserved", die der Spalte "Einnahmen" im modernen Verlauf entspricht, mit der Ausnahme, dass alle Einnahmen mit dem Status "Zahlung gesendet" ausgeschlossen werden.
- Filter wie „3M“, „6M“ oder „12M“ gelten nicht für den Abschnitt Historische Auszüge.

### <a name="historical-statement-downloads"></a>Downloads von Verlaufshinweisen

In der folgenden Tabelle wird jede Spalte in einer historischen Anweisung erläutert.

| Feldname | BESCHREIBUNG |
| --- | --- |
| Umsatzquelle | Die Quelle Ihres Umsatzes basierend auf dem Ursprungsort der Transaktion, z. B. Microsoft Store, Windows Phone Store, Windows Store 8 oder Werbung |
| Bestell-ID | Eindeutiger Bestellungsbezeichner. Mit dieser ID können Sie Kauftransaktionen mit den jeweiligen Nicht-Kauftransaktionen, z. B. Rückerstattungen oder Rückzahlungen, identifizieren. Beide weisen die gleiche Bestell-ID auf. Außerdem können Sie die Kauftransaktionen verknüpfen, wenn mehrere Zahlungsmethoden für einen einzelnen Kauf verwendet wurden, wenn es eine getrennte Gebühr gibt. |
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