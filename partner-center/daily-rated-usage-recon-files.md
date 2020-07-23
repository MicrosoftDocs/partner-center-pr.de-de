---
title: Nutzungs Abgleich-Dateien mit täglicher Bewertung
ms.topic: article
ms.date: 06/12/2020
description: Erfahren Sie, wie Sie Nutzungs Abgleich-Dateien für die tägliche Bewertung in Partner Center lesen.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ec1b58206b4947ceadd98942e8c8b982749b8645
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943457"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Erfahren Sie, wie Sie Nutzungs Abgleich-Dateien für die tägliche Bewertung in Partner Center lesen.

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Vertriebsbeauftragter
- Helpdesk-Agent

In diesem Artikel wird erläutert, wie Sie Nutzungs Abgleich-Dateien mit täglicher Bewertung lesen.

>[!NOTE]
>Die tägliche Bewertung dauert normalerweise 24 Stunden, damit Sie im Partner Center angezeigt wird oder über die API darauf zugegriffen werden kann.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Felder in den Nutzungs Abgleich-Dateien mit täglicher Bewertung

| Column | BESCHREIBUNG |
| ------ | ----------- |
| PartnerId | Die Partner-ID im GUID-Format. |
| PartnerName | Name des Partners |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. *Diese Spalte ist wichtig, um die Rechnung mit ihren Systeminformationen abzustimmen.* |
| CustomerDomainName | Der Domänen Name des Kunden. |
| CustomerCountry | Das Land, in dem sich der Kunde befindet. |
| MPNID | MPN-Bezeichner des CSP-Partners. |
| Tier2MpnId | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
| ProductId | Der Bezeichner für das Produkt. |
| SkuId | Der Bezeichner für eine bestimmte SKU. |
| AvailabilityId | Der Bezeichner für die Verfügbarkeit einer bestimmten SKU. In dieser Spalte wird angezeigt, ob die SKU für den Erwerb in den angegebenen Ländern, Währungen, Industriesegmenten usw. verfügbar ist. |
| SkuName | Der Titel einer bestimmten SKU. |
| ProductName | Der Name des Produkts. |
| PublisherName | Der Name des Herausgebers. |
| PublisherId | Der Bezeichner des Verlegers im GUID-Format. |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Diese Spalte ist ein identisches Feld für **Offername**). |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. *Dieser Bezeichner ist nicht mit der **Abonnement-ID** in der Partner Administrator Konsole identisch.* |
| ChargeStartDate | Das Start Datum des Abrechnungszeitraums (außer bei der Darstellung von Datumsangaben für zuvor nicht berechnete latente Verwendungs Daten aus dem vorherigen Abrechnungszeitraum). Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). |
| ChargeEndDate | Das Enddatum des Abrechnungszeitraums (außer bei der Darstellung von Datums Werten früherer, nicht geladener latente Verwendungs Daten aus dem vorherigen Abrechnungszeitraum). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| UsageDate | Datum der Nutzung des Diensts. |
| MeterType | Der Typ der Verbrauchseinheit. |
| MeterCategory | Der Dienst der obersten Ebene für die Nutzung. |
| MeterId | Der Bezeichner für die Verbrauchseinheit, die verwendet wird. |
| MeterSubCategory | Der Typ des Azure-Dienstanbieter, der die Rate beeinflussen kann. |
| MeterName | Die Maßeinheit für die genutzte Verbrauchseinheit. |
| MeterRegion | In dieser Spalte wird der Speicherort eines Rechenzentrums innerhalb der Region für Dienste identifiziert, bei denen meterregion anwendbar und aufgefüllt ist. |
| Einheit | Die Einheit des Ressourcen **namens**. |
| ResourceLocation | Das Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird. |
| ConsumedService | Der verwendete Azure-Plattformdienst. |
| ResourceGroup | Stellt einen Container dar, der verwandte Ressourcen für eine Azure-Lösung enthält. |
| ResourceURI | Der URI der verwendeten Ressource. |
| ChargeType | Der Typ der Gebühr oder Berichtigung.  |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dieser Preis den im Abrechnungssystem während der Abstimmung gespeicherten Informationen entspricht. |
| Menge | Anzahl der Lizenzen. Stellen Sie sicher, dass dieser Preis den im Abrechnungssystem während der Abstimmung gespeicherten Informationen entspricht. |
| UnitType | Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird.  |
| Billingpretaxtotal | Gesamtbetrag der Abrechnung vor Steuern. |
| BillingCurrency | Die Währung in der geografischen Region des Kunden. |
| Pricingpretaxtotal | Die Preise, bevor Steuern hinzugefügt werden. |
| PricingCurrency | Die Währung in der Preisliste. |
| ServiceInfo1 | Die Anzahl der Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und verwendet wurden. |
| ServiceInfo2 | Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden. |
| `Tags` | Stellt eine logische Organisation von Azure-Ressourcen dar, die vom Benutzer festgelegt werden. |
| AdditionalInfo | Alle zusätzlichen Informationen, die in den anderen Spalten nicht enthalten sind. |
| Effectiveunitprice | Der tatsächliche Wert, der pro Einheit berechnet wird, einschließlich aller Rabatte, erworbenen Gutschriften usw. |
| Pctobcexchangerate | Wechselkurs für Preiswährung auf Abrechnungswährung. |
| Pctobcexchangeratedate | Das Datum, an dem die Preiswährung der Abrechnungswährung festgelegt wird. |
| Berelementid | Stellt die Azure-Abonnement-ID dar. |
| Berelementdescription | Stellt den Namen der Azure-Abonnement-ID dar. |
| Partnerearnedcreditprozentsatz | Zeigt die partnerearnedcredit für das Zeilen Element an. Das verdiente Guthaben ist entweder 0 oder 15 Prozent. |

>[!NOTE]
>Die tägliche Bewertung dauert normalerweise 24 Stunden, damit Sie im Partner Center angezeigt wird oder über API auf Sie zugegriffen werden kann.


