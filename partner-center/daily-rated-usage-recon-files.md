---
title: Nutzungs Abgleich-Dateien mit täglicher Bewertung | Partner Center
ms.topic: article
ms.date: 01/14/2020
description: Erfahren Sie, wie Sie Nutzungs Abgleich-Dateien für die tägliche Bewertung in Partner Center lesen.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: a9c7f328cf1a10b4a23aeb775524d5931bdbb703
ms.sourcegitcommit: fc43ee25d405ef3dc673edd884c877bfc62ad6aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2020
ms.locfileid: "76021724"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Nutzungs Abgleich-Dateien mit täglicher Bewertung

**Gilt für**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Administratoragent
- Abrechnungsadministrator
- Vertriebsbeauftragter
- Helpdesk-Agent

In diesem Thema wird erläutert, wie Sie Nutzungs Abgleich-Dateien mit täglicher Bewertung lesen.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Felder in den Nutzungs Abgleich-Dateien mit täglicher Bewertung

| Spalte | Beschreibung |
| ------ | ----------- |
| PartnerID | Die Partner-ID im GUID-Format. |
| PartnerName | Name des Partners |
| Kunden-ID | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. |
| CustomerName | Firmenname des Kunden wie im Partner Center angegeben. *Diese Spalte ist sehr wichtig, um die Rechnung mit ihren Systeminformationen abzustimmen.* |
| CustomerDomainName | Der Domänen Name des Kunden. |
| CustomerCountry | Das Land, in dem sich der Kunde befindet. |
| MPNID | MPN-Bezeichner des CSP-Partners. |
| Tier2MpnId | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
| ProductID | Der Bezeichner für das Produkt. |
| SkuID | Der Bezeichner für eine bestimmte SKU. |
| AvailabilityId | Der Bezeichner für die Verfügbarkeit einer bestimmten SKU. Dies zeigt, ob die SKU für den Erwerb in den jeweiligen Ländern, Währungen, Industriesegmenten usw. verfügbar ist. |
| SkuName | Der Titel einer bestimmten SKU. |
| ProductName | Name des Produkts. |
| PublisherName | Der Name des Herausgebers. |
| PublisherId | Der Bezeichner des Verlegers im GUID-Format. |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Dies ist ein identisches Feld für **Offername**). |
| Abonnement-ID | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. *Dieser Bezeichner ist nicht mit der **Abonnement-ID** in der Partner Administrator Konsole identisch.* |
| ChargeStartDate | Das Start Datum des Abrechnungszeitraums (außer bei der Darstellung von Datumsangaben für zuvor nicht berechnete latente Verwendungs Daten aus dem vorherigen Abrechnungszeitraum). Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. |
| ChargeEndDate | Das Enddatum des Abrechnungszeitraums (außer bei der Darstellung von Datumsangaben für zuvor nicht berechnete latente Verwendungs Daten aus dem vorherigen abbildral). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| UsageDate | Datum der Nutzung des Diensts. |
| MeterType | Der Typ der Verbrauchseinheit. |
| MeterCategory | Der Dienst der obersten Ebene für die Nutzung. |
| MeterId | Der Bezeichner für die Verbrauchseinheit, die verwendet wird. |
| MeterSubCategory | Der Typ des Azure-Dienstanbieter, der die Rate beeinflussen kann. |
| MeterName | Die Maßeinheit für die genutzte Verbrauchseinheit. |
| MeterRegion | Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft. |
| Einheit | Die Einheit des Ressourcen **namens**. |
| ResourceLocation | Das Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird. |
| ConsumedService | Der Azure-Plattformdienst, den Sie verwendet haben. |
| ResourceGroup | Stellt einen Container dar, der verwandte Ressourcen für eine Azure-Lösung enthält. |
| ResourceURI | Der URI der verwendeten Ressource. |
| ChargeType | Art der Gebühren oder der Anpassung.  |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dieser Preis den im Abrechnungssystem während der Abstimmung gespeicherten Informationen entspricht. |
| Anzahl | Anzahl der Lizenzen. Stellen Sie sicher, dass dieser Preis den im Abrechnungssystem während der Abstimmung gespeicherten Informationen entspricht. |
| UnitType | Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird.  |
| Billingpretaxtotal | Gesamtbetrag der Abrechnung vor Steuern. |
| BillingCurrency | Die Währung in der geografischen Region des Kunden. |
| Pricingpretaxtotal | Die Preise vor Hinzufügen von Steuern. |
| PricingCurrency | Die Währung in der Preisliste. |
| ServiceInfo1 | Die Anzahl der Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und verwendet wurden. |
| ServiceInfo2 | Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden. |
| Tags | Stellt eine logische Organisation von Azure-Ressourcen dar, die vom Benutzer festgelegt werden. |
| AdditionalInfo | Zusätzliche Informationen, die von anderen Spalten nicht abgedeckt werden. |
| Effectiveunitprice | Der tatsächliche Wert, der pro Einheit berechnet wird, einschließlich aller Rabatte, Gutschriften usw. |
| Pctobcexchangerate | Wechselkurs für Preiswährung auf Abrechnungswährung. |
| Pctobcexchangeratedate | Das Datum, an dem die Preiswährung der Abrechnungswährung festgelegt wird. |
| Berelementid | Stellt die Azure-Abonnement-ID dar. |
| Berelementdescription | Stellt den Namen der Azure-Abonnement-ID dar. |
| Partnerearnedcreditprozentsatz | Zeigt die partnerearnedcredit für das Zeilen Element an. Das verdiente Guthaben ist entweder 0 oder 15 Prozent. |
