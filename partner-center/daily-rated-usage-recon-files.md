---
title: Daily-rated usage reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand daily-rated usage reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389698"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Daily-rated usage reconciliation files

Betrifft

- Partner Center
- Partner Center für Microsoft Cloud for US Government

This topic explains how to read daily-rated usage reconciliation files.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Fields in daily-rated usage reconciliation files

| Column | Beschreibung |
| ------ | ----------- |
| PartnerID | Partner identifier in GUID format. |
| PartnerName | Partner name. |
| Kunden-ID | Unique Microsoft identifier for the customer in GUID format. |
| CustomerCompanyName | Firmenname des Kunden wie im Partner Center angegeben. *This column is very important for reconciling the invoice with your system information.* |
| CustomerDomainName | The customer's domain name. Für die aktuelle Aktivität nicht verfügbar. |
| Land des Kunden | Das Land, in dem sich der Kunde befindet. |
| MPNID | MPN identifier of the CSP partner. |
| MPN-ID des Handelspartners | MPN identifier of the reseller of record for the subscription. Für die aktuelle Aktivität nicht verfügbar. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. Für die aktuelle Aktivität nicht verfügbar. |
| ProductID | The identifier for the product. |
| SkuId | The identifier for a particular SKU. |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU-Name | Der Titel einer bestimmten SKU. |
| PublisherName | Der Name des Herausgebers. |
| PublisherID | The identifier of the publisher in GUID format. Für die aktuelle Aktivität nicht verfügbar. |
| Abonnementbeschreibung | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (This is an identical field to **OfferName**). |
| Abonnement-ID | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Start date of the billing cycle (except when presenting dates of previously uncharged latent usage data from the previous billing cycle). Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. |
| ChargeEndDate | End date of billing cycle (except when presenting dates of previously uncharged latent usage data from the previous biling cycle). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| Nutzungsdatum | Datum der Nutzung des Diensts. |
| Typ der Verbrauchseinheit | Der Typ der Verbrauchseinheit. |
| Kategorie der Verbrauchseinheit | Der Dienst der obersten Ebene für die Nutzung. |
| ID der Verbrauchseinheit | The identifier for the meter being used. |
| Unterkategorie der Verbrauchseinheit | The type of Azure service, which can affect the rate. |
| Name der Verbrauchseinheit | Die Maßeinheit für die genutzte Verbrauchseinheit. |
| Region der Verbrauchseinheit | Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft. |
| Einheit | The unit of the resource **Name**. |
| Verbrauchte Menge | The amount of service consumed (such as *hours* or *GB*) during the reporting period. Includes any unbilled usage from previous reporting periods. |
| Ressourcenspeicherort | >The data center where the meter is running. |
| Genutzter Dienst | Der Azure-Plattformdienst, den Sie verwendet haben. |
| Ressourcen-URI | Der URI der verwendeten Ressource. |
| Gebührenart | Art der Gebühren oder der Anpassung. Für die aktuelle Aktivität nicht verfügbar. |
| Preis pro Einheit | Price per license, as published in the price list at the time of purchase. Make sure this price matches the information stored in your billing system during reconciliation. |
| Anzahl | Anzahl der Lizenzen. Make sure this price matches the information stored in your billing system during reconciliation. |
| Typ der Einheit | Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird. Für die aktuelle Aktivität nicht verfügbar. |
| Abrechnung vor Steuern | Total billing amount before taxes. |
| Abrechnungswährung | The currency in the customer's geographic region. |
| Preise vor Steuern gesamt | Die Preise vor Hinzufügen von Steuern. |
| Währung der Preise | The currency in the price list. |
| Dienstinformationen 1 | The number of Service Bus connections that were provisioned and utilized on a given day. |
| Dienstinformationen 2 | Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden. |
| Zusätzliche Infos | Zusätzliche Informationen, die von anderen Spalten nicht abgedeckt werden. |
