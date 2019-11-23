---
title: Abrechnungsübersicht | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Basic billing and invoice information for Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
keywords: Abrechnung, Zahlungen, Bestellungen, Kündigung, Auftragsverwaltung, Nichtbezahlung, Betrug, Missbrauch, Steuern, Steuerbefreiungen, Kontenabstimmungsdateien, Kontenabstimmungsdatei
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 10fe47ea038fadf8ca26fe0ab42a0d0d3a9472bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384544"
---
# <a name="billing-overview"></a>Abrechnungsübersicht

Betrifft

- Partner Center
- Partners in the Cloud Solution Provider (CSP) program

## <a name="find-your-bill"></a>Find your bill

To find your bill:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. In the left-hand menu, choose **Billing**.
3. On the **Billing** page, you can download your latest bill or download previous bills in the **Billing history** section.

## <a name="bill-your-customers"></a>Bill your customers

Microsoft has no requirements or conditions about how you handle your own invoicing.

To determine a customer's usage, [see your reconciliation files](#find-your-bill). You can use the customer name and other relevant fields to determine usage.

Next, you can add your own fees and charges for services and products that you provide. Then, you can send a single bill for all charges to your customer.

### <a name="billing-types"></a>Billing types

Billing types in Partner Center include **license-based billing**, **usage-based billing**, and **one-time billign**. For more information, see the full explanation of [billing types in Partner Center](billing-different-types.md).

### <a name="billing-currency"></a>Abrechnungswährung

You'll be billed for product(s) in the currency of the country or region in which you're located. You're billed the same regardless of the location of the customer to whom you sold the product(s).

## <a name="invoices"></a>Rechnungen

Your invoice is a summary of all charges for the current billing period. This includes charges across the program, all products, and all customers. For examples of monthly and annual billing scenarios, see [common billing scenarios](common-billing-scenarios.md)

Your invoice is available within two (2) days of your selected billing date in UTC time. Wenn beispielsweise das Abrechnungsdatum der 12. September ist, beginnt der Prozess zur Rechnungsgenerierung am 13. September um 12:00 Uhr UTC und endet am 14. September um 12:00 Uhr UTC. Sollte Ihre Rechnung bis zum 15. September, 11:59 Uhr UTC, nicht angezeigt werden, befinden Sie sich außerhalb der Vereinbarung zum Servicelevel (Service Level Agreement, SLA) und sollten eine Serviceanfrage senden.

Partners in the Cloud Solution Provider (CSP) program who choose to be billed monthly pay Microsoft 60 days in arrears for their customers' subscriptions (both license-based and usage-based).

## <a name="price-lists"></a>Price lists

Price lists are updated monthly. Preview price lists are available one (1) month in advance.

To view price lists:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. In the left-hand menu, choose **Sell**, then select **Pricing and offers**.
3. On the **Pricing and offers** page, you can see 6 months of price lists (including the current month) and preview price lists (where applicable).

**License-based** prices are guaranteed for the term of the subscription, usually 12 months from the purchase date. 

**Usage-based prices** can change on a monthly basis.

**Prices for products, services, and software subscriptions** are guaranteed through the subscription duration. However, prices may change when you renew.

You'll see **adjustments** and **credits** in arrears on your next billing invoice after the credit or adjustment is applied.

## <a name="payment-terms"></a>Zahlungsbedingungen

Die Zahlungsbedingungen sind 60 Tage netto. Rechnungen müssen bis zum Fälligkeitsdatum (60 Tage nach dem Abrechnungsdatum) bezahlt werden. Andernfalls ist Ihr Konto im Rückstand, und das kann sich auf Ihre Registrierung im CSP auswirken. 

Sie können den vollen Funktionsumfang Ihrer ausgesetzten Konten zurückerhalten, wenn Sie den fälligen Betrag zahlen.

### <a name="taxes-and-vat"></a>Taxes and VAT

You are taxed based on your details (not your customers' details) because the billing relationship is between Microsoft and you. You can submit your tax identifier during the account setup process or through a support request later. Die Änderungen werden im nächsten Abrechnungszyklus angezeigt.

For **withholding and sales tax exemption**, you must submit tax documentation through a support request. Die Änderungen und entsprechenden Erstattungen werden in Ihrem nächsten Abrechnungszyklus angezeigt.

For **value-added tax (VAT) exemption**, you must submit your VAT ID (validated by Microsoft) through a service request. Die Änderungen und entsprechenden Erstattungen werden in Ihrem nächsten Abrechnungszyklus angezeigt.

Weitere Steuerinformationen erhalten Sie von Ihrem örtlichen Finanzamt oder Steuerberater.

### <a name="annual-billing-rules"></a>Annual billing rules

Abonnements gelten für ein Jahr und werden automatisch verlängert.

Die Abrechnung erfolgt in 12 monatlichen Zahlungen oder einer jährlichen Zahlung pro Jahresabonnement.

Lizenzbasierte Dienste werden (basierend auf der Anzahl an Lizenzen am Ende des vorherigen Abrechnungszeitraums) im Voraus für den nächsten Abrechnungszeitraum abgerechnet.

Änderungen an der Anzahl der Lizenzen (anteilsmäßige Berechnung basierend auf Lizenzen/Tagen) werden nachträglich in Rechnung gestellt/gutgeschrieben. Pro-rata calculation uses the following formula:

`[ROUND((ROUND(Unit Price * Quantity / Number of days in pro-rated Month, 2) * Number of pro-rated days) / Quantity, 2) * Quantity]`

Payments are billed for licenses sold, not licenses provisioned.

### <a name="change-billing-frequency"></a>Change billing frequency

To change the billing frequency of an online service for a customer:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. In the left-hand menu, choose **Customers**.
3. Select the customer whose subscription billing frequency you want to change.
4. On the customer's **Subscriptions** page, select the subscription that you want to change.
5. On the **Details** page, under **Billing frequency**, select **Monthly** or **Annual**. Es wird Ihnen eine Bestätigungsseite mit wichtigen Informationen zum Ändern der Abrechnungshäufigkeit sowie eine Liste der Abonnements angezeigt, die gleich geändert werden.
6. Choose **OK** to make the change (or **Cancel** to undo it).

### <a name="adjustmentscreditscancellations"></a>Anpassungen/Guthaben/Kündigungen

Microsoft stellt keine Gebühren für eine vorzeitige Beendigung bei der Kündigung lizenzbasierter Dienste in Rechnung.

Cancellation credits for licensed-based services are pro-rated for unused days for mid-cycle cancellations (as well as license decreases according to the formula above).

### <a name="billing-rules"></a>Abrechnungsregeln

Abonnements laufen von Monat zu Monat und werden zu den neuen getakteten Dienstleistungspreisen automatisch verlängert. Ihnen wird jeden Monat die Nutzung während des Vormonats in Rechnung gestellt.

Getaktete Dienstleistungspreise können sich innerhalb des Abrechnungszyklus ändern.

#### <a name="price-changes"></a>Price changes

For **price increases**, 30 days' notice is provided.

**Price decreases** are reflected on the day of change.

**Existing subscriptions** use the rate in effect at the beginning of the bill cycle.

**New subscriptions**, when created within the same billing cycle, use the rate in effect on the date you create them. 

### <a name="adjustmentscreditscancellations"></a>Anpassungen/Guthaben/Kündigungen

Zahlungen mit Anpassungen werden in der nächsten monatlichen Rechnung angezeigt.

Microsoft stellt keine Gebühren für eine vorzeitige Beendigung bei der Kündigung nutzungsbasierter Dienste in Rechnung. 

Alle Guthaben, einschließlich SLA-Guthaben, werden in der nächsten monatlichen Rechnung angezeigt.

>[!IMPORTANT]
>Wenn Sie Azure-Reservierungen und/oder Softwareabonnements für einen Kunden an einem Standort mit einer anderen Währung als Ihrer Währung erwerben, basiert die Standardabrechnungswährung auf dem Standort des Kunden, nicht Ihrem Standort. Wenn Sie Kunden an mehreren Standorten haben, erhalten Sie getrennte Rechnungen und Kontenabstimmungsdateien für jede Währung der Kunden, die in Rechnung gestellt werden müssen, damit Sie Ihren Kunden Rechnungen in der entsprechenden Währung ausstellen können.

## <a name="manage-one-time-billing"></a>Manage one-time billing

### <a name="billing-status-invoices-and-reconciliation-files"></a>Billing status, invoices and reconciliation files

To view your current billing status, invoices, and reconciliation files:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. On the left-hand menu, choose **Billing**, then select **One time**.
3. On the billing status page, select an invoice or reconciliation file to view more detailed information.

### <a name="customer-order-history"></a>Customer order history

To view a customer's order history:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. On the left-hand menu, choose **Customers**.
3. On the **Customers** page, find the customer whose order history you want to view. Select the down arrow to expand the customer's record.
4. Choose **View orders** to display the customer's order history.

### <a name="credit-notes"></a>Credit notes

You might need to request a credit or rebill for the following reasons:

- You need to make address or purchase order corrections.
- A tax refund was applied after the invoice was generated. You can request a credit or rebill to get the tax refund pulled back into the original invoice. The same is also true for refunds. You can request a credit or rebill of the original invoice, then pull in a refund.

If you request a credit or rebill, we'll give you a **credit note** to cancel the original invoice.
