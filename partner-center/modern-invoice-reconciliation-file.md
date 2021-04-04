---
title: Felder für das Wiederholen von Dateien für CSP-einmalige Käufe
ms.topic: conceptual
ms.date: 01/29/2021
description: Erfahren Sie mehr über alle Elemente in ihrer CSP-Datei für die einmalige Kauf Abstimmung in Partner Center, einschließlich Beispiel Werten.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 66159d886914336180e8531ec07db3a9d8880a88
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103773"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Felder für die einmalige Kauf Abstimmung von CSP-Dateien

## <a name="using-the-recon-file"></a>Verwenden der Datei "Reconnaissance"
In der folgenden Tabelle finden Sie Beschreibungen und Beispiel Werte für die Felder in der Abstimmungs Datei für die einmaligen Käufe von CSP.

Weitere Informationen zum Abgleich von Dateien finden Sie unter [use the Versöhnungs files](use-the-reconciliation-files.md).

| Column | BESCHREIBUNG | Beispielwert |
| ------ | ----------- | ------------ |
| PartnerId | Eindeutiger Bezeichner im GUID-Format für eine bestimmte Abrechnungs Entität. Für die Abstimmung nicht erforderlich. In allen Zeilen gleich. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. Diese Spalte ist wichtig, um die Rechnung mit ihren Systeminformationen abzustimmen. | *Johnny modern cust DE2* |
| CustomerDomainName | Der Domänen Name des Kunden. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Das Land, in dem sich Ihr Kunde befindet. Sehen Sie sich die vollständige [Liste der Länder](./regional-authorization-overview.md) für Ihre Region an.  | *DE* |
| InvoiceNumber | Die Rechnungsnummer, die der Abstimmungs Datei zugeordnet ist.  | *G002297372* |
| MPNID | MPN-Bezeichner des CSP-Partners. Weitere Informationen finden Sie unter Vorgehens [Weise beim itemisieren nach Partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| Resellermpnid | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement. | *6048879* |
| OrderId | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um die Reihenfolge zu identifizieren, in der der Support kontaktiert Wird nicht für die Abstimmung verwendet. | *0et2qazvjgff9wgsknwzr5jlmhp10loc1* |
| OrderDate | Datum, an dem die Bestellung platziert wurde. | *10/3/2020* |
| ProductId | Der eindeutige Bezeichner des Produkts. | *DZH318Z0BNZ5* |
| SkuId | Der eindeutige SKU-Bezeichner. | *006g* |
| AvailabilityId | Der eindeutige Verfügbarkeits Bezeichner. | *DZH318Z08B80* |
| SkuName | Der SKU-Name. | *Tabellen-LRS* |
| ProductName | Der Produktname. | *Tabellen* |
| ChargeType | Der [Typ der Belastung](./recon-file-charge-types.md) oder der Anpassung. | *Neu* |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert | *0,045* |
| Menge | Die Anzahl der Lizenzen. Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert | *1* |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern Das Teilergebnis sollte gleich der abrechenbaren Menge sein, multipliziert mit dem effektiven Einheitspreis. | *0* |
| TaxTotal | Steuern der Steuerbeträge. Basierend auf den Steuerregeln Ihres Marktes und bestimmten Bedingungen. | *0* |
| Gesamt | Der Gesamtbetrag ist gleich dem Teilergebnis plus dem Steuerbetrag. | *0* |
| Währung | Ihre Rechnung wird im Kontext der Kunden Währung generiert. Dies bedeutet: Wenn Sie als Partner Transaktionen mit Kunden aus unterschiedlichen abrechenbaren Währungen durchführen, erhalten Sie für jeden Kundenwährungstyp eine Rechnung.  | *EUR* |
| Preis Beschreibung | Die Gründe für die Anpassungen im Einzelpreis. Dies sind die Hauptgründe, aber nicht auf die Bestimmung des effektiven Einheits Preises beschränkt. | *["15,0% Partner Guthaben für verwaltete Dienste"]* |
| PublisherName | Herausgeber des Produkts.  | *Microsoft* |
| PublisherId | Ein eindeutiger Bezeichner, der vom Partner Center zum Identifizieren des Verlegers verwendet wird. | *AS* |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. Diese Spalte ist ein identisches Feld für "Offername". | *Azure-Plan* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. Beachten Sie, dass dieser Bezeichner nicht mit der Abonnement-ID in der Partner Administrator Konsole identisch ist. | *307628r1-d9d2-f. c-ea1f -4183f 0cae308* |
| ChargeStartDate | Das Datum, an dem der Abrechnungszeitraum eines Abonnements beginnt. | *9/1/2020* |
| ChargeEndDate | Das Datum, an dem der Abrechnungszeitraum eines Abonnements endet. | *30.09.2020* |
| Termandbillingcycle | Die Dauer der weiteren Verpflichtung zum Fortsetzen des Abonnements zum Zeitpunkt des Kaufs. | *Gespeicherte Daten (GB/Monat)* |
| Effectiveunitprice | Der Anteils mäßige Einheitspreis zum Berechnen der Kosten für den Abrechnungszeitraum. Rabatte, Anpassungen in Abrechnungs Tagen und andere Faktoren bestimmen den effektiven Einzelpreis. Weitere Informationen finden Sie unter [effektive Unit Price-Berechnung](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Der Typ der Einheit, in der die Verbrauchseinheit berechnet wird. | *1 GB/Monat* |
| AlternateId | Die Alternative ID des Auftrags Elements, auf das verwiesen wird. | *6dc5c039750a* |
| Billablemenge | Die Gesamtmenge, die abgerechnet wird.  | *0,005001* |
| Billingfrequency | Der zum Zeitpunkt des Kaufs ausgewählte Abrechnungsplan. | *AS*  |
| PricingCurrency | Die Währung in der Preisliste. | *USD* |
| Pctobcexchangerate | Der Wechselkurs, der für die Preiswährung auf Abrechnungswährung angewendet wird. | *0,846202666* |
| Pctobcexchangeratedate | Das Datum, an dem die Preiswährung der Abrechnungswährung festgelegt wird. | *30.09.2020* |
| Meterbeschreibung | Beschreibung der Verbrauchseinheit.  | *Tabellen-lokal gespeicherte LRS-Daten (GB/Monat)* |
| ReservationOrderId | Die Reservierungs Auftrags-ID. | *E21A6344E398FFC1C4D7...* |
| "Credideboncode" | Die Bonitäts Beschreibung. | *Azure-Verbrauchs Guthaben* |

>[!NOTE]
>Sie können Ihren Azure-Verbrauch in ihrer einmaligen Kauf Datei abstimmen. Wechseln Sie zu diesem Zweck zu Ihrer Datei für die tägliche Nutzung der Nutzungsdauer, und suchen Sie nach ihrer Abonnement-ID. Dadurch werden alle Kosten angezeigt, die ihrer Azure-Plan-ID zugeordnet sind. Ihre Azure-Abonnement-ID wird als "" "" "" "" "".

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Steuern](billing.md)
