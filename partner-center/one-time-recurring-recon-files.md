---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389678"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

Betrifft

- Partner Center
- Partner Center für Microsoft Cloud for US Government

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| Column | Beschreibung |
| ------ | ----------- |
| PartnerID | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. In allen Zeilen gleich. |
| Kunden-ID | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| Kundenname | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Land des Kunden | Das Land, in dem sich der Kunde befindet. |
| Rechnungsnummer | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
| MPNID | MPN identifier of the CSP partner. |
| MPN-ID des Handelspartners | MPN identifier of the reseller of record for the subscription. |
| Bestellnummer | Eindeutiger Bezeichner für eine Bestellung auf der Microsoft Commerce Platform. Not used for reconciliation. |
| Bestellungsdatum | Das Datum, an dem die Bestellung aufgegeben wurde. |
| ProductID | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU-Name | Der Titel einer bestimmten SKU. |
| Produktname | Name des Produkts. |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Abonnementbeschreibung | Anzeigename eines Abonnements. |
| Abonnement-ID | Eindeutiger Bezeichner eines Abonnements auf der Microsoft Commerce Platform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Der erste Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. |
| ChargeEndDate | Letzter Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| Laufzeit und Abrechnungszyklus | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| Gebührenart | Art der Gebühren oder der Anpassung. |
| Preis pro Einheit | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effektiver Preis pro Einheit | Der Preis pro Einheit, nachdem Anpassungen vorgenommen wurden. |
| Anzahl | Anzahl der Einheiten. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Typ der Einheit | Der Typ der Einheit, die gekauft wird. |
| DiscountDetails | Eine Erklärung der geltenden Rabatte. |
| Zwischensumme | Gesamtbetrag vor Steuern Checks if your subtotal matches your expected total, in case of a discount. |
| Steuern gesamt | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| Gesamt | Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden. |
| Währung | Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
