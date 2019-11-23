---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389838"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| Feld | Definition |
| ----- | ---------- |
| US FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| Kundennummer | Ihre Kundennummer. |
| Rechnungsempfänger | Die Adresse, an die wir Ihre Rechnung senden. You can change your company name and/or address in your Partner Center billing profile. |
| Lizenzbasierte Gebühren | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| Nutzungsbasierte Gebühren | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| Rabatte | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| Gutschriften | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| Zwischensumme | Gesamtbetrag vor Steuern und Gebühren und Guthaben exklusive Steuern |
| Steuern | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| Andere Guthaben | Guthaben exklusive Steuern |
| Gesamtsumme der aktuellen Gebühren | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| Zahlungsanweisungen | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| Rechnungsnummer | Die Nummer Ihrer Rechnung. |
| Abrechnungszeitraum | Der monatliche Zeitraum bis zum Rechnungsdatum. Dies ist der Zeitraum, in dem nutzungsbasierte Dienste verbraucht und lizenzbasierte Dienste auf Guthabenanpassungen oder Änderungen in der Lizenzanzahl abgestimmt werden. |
| Rechnungsdatum | The billing date or anniversary date on which your invoice is generated each month. |
| Zahlungsbedingungen | The payment term. Für einmalige Einkäufe wird dies immer 60 Tage sein. |
| Fälligkeitsdatum der Zahlung | The date by which your payment must be received. |
| Name des Kunden | Your purchase number order. |
| Kundendienst | The website address where you can access customer service. |
| Dienstempfänger | The address where the service is being used. (Dies ist die rechtlich gültige Unternehmensadresse. Sie ist mit der Unternehmensprüfung verknüpft.) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| Feld | Definition |
| ----- | ---------- |
| Datum | Kaufdatum. |
| Beschreibung | Produktname. |
| Anzahl | The number of products (such as reservations) purchased. |
| Preis pro Einheit | Price per product (such as a reservation). |
| Rabatte | Alle anwendbaren Rabatte. |
| Vorsteuerbetrag | Zwischensumme der Einkäufe vor Steuern. |
| Mehrwertsteuer | Steuerbetrag. |
| Gesamt | Total amount to be paid. |
