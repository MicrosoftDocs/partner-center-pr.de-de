---
title: Abstimmungsdateien für die täglich bewertete Nutzung
ms.topic: article
ms.date: 06/12/2020
description: Erfahren Sie, wie Sie Abstimmungsdateien für die täglich bewertete Nutzung in Partner Center lesen. Enthält Beschreibungen für bestimmte Felder in der Recon-Datei.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147274"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Erfahren Sie, wie Sie Abstimmungsdateien für die täglich bewertete Nutzung in Partner Center

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Administrator-Agent-| Abrechnungsadministrator-| | des Vertriebsmitarbeiters Helpdesk-Agent

In diesem Artikel wird erläutert, wie Sie Abstimmungsdateien für die täglich bewertete Nutzung lesen.

>[!NOTE]
>Die täglich bewertete Nutzung dauert normalerweise 24 Stunden, bis sie in Partner Center angezeigt wird oder über die API aufgerufen wird.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Felder in Abstimmungsdateien für die täglich bewertete Nutzung

| Column | Beschreibung |
| ------ | ----------- |
| PartnerId | Partnerbezeichner im GUID-Format. |
| PartnerName | Name des Partners |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. *Diese Spalte ist wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.* |
| CustomerDomainName | Der Domänenname des Kunden. |
| CustomerCountry | Das Land, in dem sich der Kunde befindet. |
| MPNID | MPN-ID des CSP-Partners. |
| Tier2MpnId | MPN-ID des Resellers des Datensatzes für das Abonnement. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
| ProductId | Der Bezeichner für das Produkt. |
| SkuId | Der Bezeichner für eine bestimmte SKU. |
| AvailabilityId | Der Bezeichner für die Verfügbarkeit einer bestimmten SKU. In dieser Spalte wird angezeigt, ob die SKU für den Kauf im jeweiligen Land, in der jeweiligen Währung, im jeweiligen Branchensegment usw. verfügbar ist. |
| SkuName | Der Titel einer bestimmten SKU. |
| ProductName | Der Name des Produkts. |
| PublisherName | Der Name des Herausgebers. |
| PublisherId | Der Bezeichner des Herausgebers im GUID-Format. |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Diese Spalte ist ein identisches Feld mit **OfferName**). |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. *Dieser Bezeichner ist nicht mit der **Abonnement-ID** in der Partner-Verwaltungskonsole identisch.* |
| ChargeStartDate | Startdatum des Abrechnungszyklus (außer bei der Präsentation von Datumsangaben der zuvor nicht in Rechnung stellenden latenten Nutzungsdaten aus dem vorherigen Abrechnungszeitraum). Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). |
| ChargeEndDate | Enddatum des Abrechnungszyklus (außer bei der Präsentation von Datumsangaben der zuvor nicht in Rechnung stellenden latenten Nutzungsdaten aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| UsageDate | Datum der Nutzung des Diensts. |
| MeterType | Der Typ der Verbrauchseinheit. |
| MeterCategory | Der Dienst der obersten Ebene für die Nutzung. |
| MeterId | Der Bezeichner für die verwendete Verbrauchsanzeige. |
| MeterSubCategory | Der Typ des Azure-Diensts, der sich auf die Rate auswirken kann. |
| MeterName | Die Maßeinheit für die genutzte Verbrauchseinheit. |
| MeterRegion | Diese Spalte gibt den Standort eines Rechenzentrums in der Region für Dienste an, bei denen MeterRegion anwendbar und aufgefüllt ist. |
| Einheit | Die Einheit des **Ressourcennamens.** |
| ResourceLocation | Das Rechenzentrum, in dem die Verbrauchsmessung ausgeführt wird. |
| ConsumedService | Der verwendete Azure-Plattformdienst. |
| ResourceGroup | Stellt einen Container dar, der verwandte Ressourcen für eine Azure-Lösung enthält. |
| ResourceURI | Der URI der verwendeten Ressource. |
| ChargeType | Der Typ der Gebühr oder Berichtigung.  |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dieser Preis den Informationen entspricht, die während der Abstimmung in Ihrem Abrechnungssystem gespeichert sind. |
| Menge | Anzahl der Lizenzen. Stellen Sie sicher, dass dieser Preis den Informationen entspricht, die während der Abstimmung in Ihrem Abrechnungssystem gespeichert sind. |
| Unittype | Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird.  |
| BillingPreTaxTotal | Gesamtabrechnungsbetrag vor Steuern.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Die Währung in der geografischen Region des Kunden. |
| PreisePreTaxTotal | Die Preise, bevor Steuern hinzugefügt werden. |
| PricingCurrency | Die Währung in der Preisliste. |
| ServiceInfo1 | Die Anzahl der Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und verwendet wurden. |
| ServiceInfo2 | Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden. |
| `Tags` | Stellt eine logische, vom Benutzer festgelegte Organisation von Azure-Ressourcen dar. |
| AdditionalInfo | Alle zusätzlichen Informationen, die in den anderen Spalten nicht enthalten sind. |
| EffectiveUnitPrice | Der tatsächliche Wert, der pro Einheit abgerechnet wird, einschließlich aller Rabatte, erworbenen Gutschriften usw. |
| PCToBCExchangeRate | Wechselkurs, der für die Preiswährung auf die Abrechnungswährung angewendet wird. |
| PCToBCExchangeRateDate | Das Datum, an dem die Preiswährung für die Abrechnungswährung bestimmt wird. |
| EntitlementId | Stellt die Azure-Abonnement-ID dar. |
| EntitlementDescription | Stellt den Namen der Azure-Abonnement-ID dar. |
| PartnerEarnedCreditPercentage | Zeigt den PartnerEarnedCredit für das Zeilenelement an. Das erworbene Guthaben ist entweder 0 oder 15 Prozent. |
| CreditPercentage | Zeigt das Azure-Verbrauchsguthaben an. Das erworbene Guthaben ist entweder 0 oder 100 Prozent. |
| CreditType | Typ des Guthabens. Beispiel: **Azure-Gutschrift angewendet.** |
>[!NOTE]
>Die täglich bewertete Nutzung dauert normalerweise 24 Stunden, bis sie in Partner Center oder über die API angezeigt wird.


