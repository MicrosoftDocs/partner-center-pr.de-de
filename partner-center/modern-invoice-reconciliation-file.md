---
title: Neukonstruieren von Dateifeldern für einmalige CSP-Käufe
ms.topic: conceptual
ms.date: 01/29/2021
description: Erfahren Sie mehr über alle Elemente in Ihrer CSP-Abstimmungsdatei für einmaligen Kauf in Partner Center, einschließlich Beispielwerten.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146254"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Felder für die CSP-Abstimmungsdatei für einmaligen Kauf

**Geeignete Rollen:** Kontoadministrator-| Abrechnungs-Agent

## <a name="using-the-recon-file"></a>Verwenden der Recon-Datei
Die folgende Tabelle enthält Beschreibungen und Beispielwerte für die Felder in der Abstimmungsdatei für einmalige CSP-Käufe.

Weitere Informationen zu Abstimmungsdateien finden Sie unter [Verwenden der Abstimmungsdateien.](use-the-reconciliation-files.md)

| Column | BESCHREIBUNG | Beispielwert |
| ------ | ----------- | ------------ |
| PartnerId | Eindeutiger Bezeichner im GUID-Format für eine bestimmte Abrechnungsentität. Nicht erforderlich für die Abstimmung. In allen Zeilen gleich. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. Diese Spalte ist wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Der Domänenname des Kunden. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Das Land, in dem sich Ihr Kunde befindet. Sehen Sie sich die vollständige [Liste der Länder](./regional-authorization-overview.md) für Ihre Region an.  | *DE* |
| InvoiceNumber | Die der Abstimmungsdatei zugeordnete Rechnungsnummer.  | *G002297372* |
| MPNID | MPN-Bezeichner des CSP-Partners. Weitere Informationen finden Sie unter [Itemisieren nach Partner.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | MPN-Bezeichner des Vertriebspartners des Datensatzes für das Abonnement. | *6048879* |
| OrderId | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um die Bestellung zu identifizieren, wenn Sie sich an den Support wenden. Wird nicht für die Abstimmung verwendet. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Datum in UTC, an dem die Bestellung platziert wurde. | *10/3/2020* |
| ProductId | Der eindeutige Bezeichner des Produkts. | *DZH318Z0BNZ5* |
| SkuId | Der eindeutige SKU-Bezeichner. | *006G* |
| AvailabilityId | Der eindeutige Verfügbarkeitsbezeichner. | *DZH318Z08B80* |
| SkuName | Der SKU-Name. | *Tabellen – LRS* |
| ProductName | Der Produktname. | *Tabellen* |
| ChargeType | Der [Typ der Gebühr oder](./recon-file-charge-types.md) Anpassung. | *Neu* |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die während des Abgleichs in Ihrem Abrechnungssystem gespeichert sind. | *0.045* |
| Menge | Die Anzahl der Lizenzen. Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die während des Abgleichs in Ihrem Abrechnungssystem gespeichert sind. | *1* |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern Die Teilsumme sollte gleich der abrechenbaren Menge multipliziert mit dem effektiven Einzelpreis sein. | *0* |
| TaxTotal | Gebühr für den Steuerbetrag. Basierend auf den Steuerregeln Ihres Markts und bestimmten Umständen. | *0* |
| Gesamt | Der Gesamtbetrag entspricht dem Teilsummenbetrag zuzüglich des Steuerbetrags. | *0* |
| Währung | Ihre Rechnung wird im Kontext der Währung des Kunden generiert. Dies bedeutet: Wenn Sie als Partner Transaktionen mit Kunden aus unterschiedlichen abrechenbaren Währungen durchführen, erhalten Sie für jeden Kundenwährungstyp eine Rechnung.  | *EUR* |
| PriceAdjustmentDescription | Die Gründe für die Anpassungen im Einzelpreis. Dies sind die Hauptgründe, aber nicht beschränkt auf die Bestimmung des effektiven Einzelpreises. | *["15,0 % vom Partner erworbenes Guthaben für verwaltete Dienste"]* |
| PublisherName | Herausgeber des Produkts.  | *Microsoft* |
| PublisherId | Ein eindeutiger Bezeichner, den der Partner Center verwendet, um den Herausgeber zu identifizieren. | *Na* |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. Diese Spalte ist ein identisches Feld mit OfferName. | *Azure-Plan* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. Beachten Sie, dass dieser Bezeichner nicht mit der Abonnement-ID in der Partneradministratorkonsole identisch ist. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Das Datum, an dem der Abrechnungszeitraum eines Abonnements beginnt. | *9/1/2020* |
| ChargeEndDate | Das Datum, an dem der Abrechnungszeitraum eines Abonnements endet. | *30.09.2020* |
| TermAndBillingCycle | Die Dauer, mit der das Abonnement zum Zeitpunkt des Kaufs fortgesetzt werden soll. | *Gespeicherte Daten (GB/Monat)* |
| EffectiveUnitPrice | Der anteilsierte Einzelpreis, um die Kosten für den Abrechnungszyklus zu berechnen. Rabatte, Anpassungen an Abrechnungstagen und andere Faktoren bestimmen den effektiven Einzelpreis. Weitere Informationen finden Sie unter [Effective Unit Price Calculation](./effective-unit-price-calculation.md).  | *0.03825* |
| Unittype | Der Typ der Einheit, in der die Verbrauchseinheit berechnet wird. | *1 GB/Monat* |
| AlternateId | Die alternative ID des Auftragspositionselements, auf das verwiesen wird. | *6dc5c039750a* |
| BillableQuantity | Die Gesamtmenge, die abgerechnet wird.  | *0.005001* |
| BillingFrequency | Der zum Zeitpunkt des Kaufs ausgewählte Abrechnungsplan. | *Na*  |
| PricingCurrency | Die Währung in der Preisliste. | *USD* |
| PCToBCExchangeRate | Der Wechselkurs, der für die Preiswährung auf die Abrechnungswährung angewendet wird. | *0.846202666* |
| PCToBCExchangeRateDate | Das Datum, an dem die Preiswährung auf die Abrechnungswährung festgelegt wird. | *30.09.2020* |
| MeterDescription | Beschreibung der Verbrauchseinheiten.  | *Tabellen – gespeicherte LRS-Daten (GB/Monat)* |
| ReservationOrderId | Die ID des Reservierungsauftrags. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Die Kreditbeschreibung. | *Azure-Verbrauchsguthaben* |

>[!NOTE]
>Sie können Ihren Azure-Verbrauch in Der Abstimmungsdatei für einmalige Käufe abstimmen. Wechseln Sie hierzu zur Neukonfigurationsdatei für die täglich bewertete Nutzung, und suchen Sie nach Ihrer SubscriptionID. Dadurch werden alle Kosten angezeigt, die Ihrer Azure-Plan-ID zugeordnet sind. Ihre Azure-Abonnement-ID wird als EntitlementID angezeigt.

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Steuern](billing.md)
