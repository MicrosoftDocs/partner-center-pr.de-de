---
title: Dateifelder für einmalige CSP-Käufe neu konfigurieren
ms.topic: conceptual
ms.date: 01/29/2021
description: Erfahren Sie mehr über alle Elemente in Ihrer CSP-Abstimmungsdatei für einmaligen Kauf in Partner Center, einschließlich Beispielwerten.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 7ff320124230ec8e0b3505b1c1dbbb7c811cb67f
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120714"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP-Felder für einmalige Kaufabstimmungsdatei

**Geeignete Rollen**

- Kontoadministrator
- Abrechnungs-Agent

## <a name="using-the-recon-file"></a>Verwenden der Recon-Datei
Die folgende Tabelle enthält Beschreibungen und Beispielwerte für die Felder in der Abstimmungsdatei für einmalige CSP-Käufe.

Weitere Informationen zu Abstimmungsdateien finden Sie unter [Verwenden der Abstimmungsdateien.](use-the-reconciliation-files.md)

| Column | BESCHREIBUNG | Beispielwert |
| ------ | ----------- | ------------ |
| PartnerId | Eindeutiger Bezeichner im GUID-Format für eine bestimmte Abrechnungsentität. Für die Abstimmung nicht erforderlich. In allen Zeilen gleich. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. Diese Spalte ist wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Domänenname des Kunden. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Das Land, in dem sich Ihr Kunde befindet. Sehen Sie sich [die vollständige Liste der Länder](./regional-authorization-overview.md) für Ihre Region an.  | *DE* |
| InvoiceNumber | Die Rechnungsnummer, die der Abstimmungsdatei zugeordnet ist.  | *G002297372* |
| MPNID | MPN-Bezeichner des CSP-Partners. Weitere Informationen finden Sie unter [Itemisieren nach Partner.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | MPN-ID des Vertriebspartners des Datensatzes für das Abonnement. | *6048879* |
| OrderId | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um den Auftrag zu identifizieren, wenn Sie sich an den Support wenden. Wird nicht für die Abstimmung verwendet. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Datum, an dem die Bestellung aufgegeben wurde. | *10/3/2020* |
| ProductId | Der eindeutige Bezeichner des Produkts. | *DESH318Z0BNZ5* |
| SkuId | Der eindeutige SKU-Bezeichner. | *006G* |
| AvailabilityId | Der eindeutige Verfügbarkeitsbezeichner. | *DESH318Z08B80* |
| SkuName | Der SKU-Name. | *Tabellen – LRS* |
| ProductName | Der Produktname. | *Tabellen* |
| ChargeType | Die [Art der Gebühr](./recon-file-charge-types.md) oder Anpassung. | *Neu* |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dies den Informationen entspricht, die während der Abstimmung in Ihrem Abrechnungssystem gespeichert sind. | *0.045* |
| Menge | Die Anzahl der Lizenzen. Stellen Sie sicher, dass dies den Informationen entspricht, die während der Abstimmung in Ihrem Abrechnungssystem gespeichert sind. | *1* |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern Die Teilsumme sollte gleich der agerechneten Menge multipliziert mit dem effektiven Einzelpreis sein. | *0* |
| TaxTotal | Steuerbetragsgebühr. Basierend auf den Steuerregeln Ihres Markts und bestimmten Umständen. | *0* |
| Gesamt | Der Gesamtbetrag entspricht der Teilsumme zuzüglich des Steuerbetrags. | *0* |
| Währung | Ihre Rechnung wird im Kontext der Währung des Kunden generiert. Dies bedeutet: Wenn Sie als Partner Transaktionen mit Kunden aus unterschiedlichen abrechenbaren Währungen durchführen, erhalten Sie für jeden Kundenwährungstyp eine Rechnung.  | *EUR* |
| PriceAdjustmentDescription | Die Gründe für die Anpassungen des Einzelpreises. Dies sind die Hauptgründe, aber nicht beschränkt auf die Bestimmung des effektiven Einzelpreises. | *["15,0% Vom Partner verdientes Guthaben für verwaltete Dienste"]* |
| PublisherName | Herausgeber des Produkts.  | *Microsoft* |
| PublisherId | Ein eindeutiger Bezeichner, Partner Center den Herausgeber identifiziert. | *Nicht verfügbar* |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. Diese Spalte ist ein identisches Feld mit OfferName. | *Azure-Plan* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. Beachten Sie, dass dieser Bezeichner nicht mit der Abonnement-ID in der Partner-Verwaltungskonsole identisch ist. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Das Datum, an dem der Abrechnungszeitraum eines Abonnements beginnt. | *9/1/2020* |
| ChargeEndDate | Das Datum, an dem der Abrechnungszeitraum eines Abonnements endet. | *30.09.2020* |
| TermAndBillingCycle | Die Verpflichtung zur Verlängerung des Abonnements zum Zeitpunkt des Kaufs. | *Gespeicherte Daten (GB/Monat)* |
| EffectiveUnitPrice | Der anteilsmäßig berechnete Einzelpreis zum Berechnen der Kosten für den Abrechnungszyklus. Rabatte, Anpassungen an Abrechnungstagen und andere Faktoren bestimmen den effektiven Einzelpreis. Weitere Informationen finden Sie unter [Effective Unit Price Calculation](./effective-unit-price-calculation.md).  | *0.03825* |
| Unittype | Der Typ der Einheit, in der die Verbrauchseinheit in Rechnung gestellt wird. | *1 GB/Monat* |
| AlternateId | Die alternative ID des Auftragszeilenelements, auf das verwiesen wird. | *6dc5c039750a* |
| BillableQuantity | Die in Rechnung gestellte Gesamtmenge.  | *0.005001* |
| BillingFrequency | Der zum Zeitpunkt des Kaufs ausgewählte Abrechnungsplan. | *Nicht verfügbar*  |
| PricingCurrency | Die Währung in der Preisliste. | *USD* |
| PCToBCExchangeRate | Der Wechselkurs, der für die Preiswährung in die Abrechnungswährung angewendet wird. | *0.846202666* |
| PCToBCExchangeRateDate | Das Datum, an dem die Preiswährung für die Abrechnungswährung bestimmt wird. | *30.09.2020* |
| MeterDescription | Beschreibung der Verbrauchsmessung.  | *Tabellen – Gespeicherte LRS-Daten (GB/Monat)* |
| ReservationOrderId | Die ID des Reservierungsauftrags. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Die Kreditbeschreibung. | *Azure-Verbrauchsguthaben* |

>[!NOTE]
>Sie können Ihren Azure-Verbrauch in Ihrer Einmaligen Kauf-Recon-Datei abstimmen. Wechseln Sie dazu zu Ihrer täglich bewerteten Nutzungs-Recon-Datei, und suchen Sie nach Ihrer SubscriptionID. Dadurch werden alle Kosten angezeigt, die Ihrer Azure-Plan-ID zugeordnet sind. Ihre Azure SubscriptionID wird als EntitlementID angezeigt.

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Steuern](billing.md)
