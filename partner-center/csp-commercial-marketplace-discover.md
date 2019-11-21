---
title: Discover offers in the commercial marketplace  | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how CSP partners can use Partner Center to view or search the marketplace for SaaS offers or pricing from Independent Software Vendors (ISVs).
author: MicheleHope
ms.author: v-mihope
keywords: subscriptions, marketplace, commercial marketplace, third party, ISV, SaaS offers, Cloud Solution Provider program, CSP program, CSP partners
ms.localizationpriority: medium
ms.openlocfilehash: 23a31646165576842b625ec4f05a8da404fae01d
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253718"
---
# <a name="discover-offers-and-pricing-in-the-commercial-marketplace"></a>Discover offers and pricing in the commercial marketplace

**Zielgruppe**

- Partner Center
- Partner im CSP-Programm

**Appropriate roles**

- Globaler Administrator
- Administratoragent

When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program. If they choose to sell the offer through the CSP program, CSP partners should see the offer in the Partner Center Marketplace area. 

If an ISV offer does not appear as you expect in the Partner Center, it may be because:

- The ISV decided not to sell the offer through the CSP program. For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for CSPs in the Partner Center marketplace.

- The ISV decided to make the offer exclusive to only a select number of CSP partners. For more information about exclusive offers, see later in this help topic.

- The offer type may not be transactable through the Partner Center or Azure portal (e.g. Containers or some usage-based offers).

- The billing country of your associated customer(s) may not be supported for this ISV offer.

## <a name="view-marketplace-offers-in-partner-center"></a>View Marketplace offers in Partner Center

To view available commercial marketplace offers in the CSP program: 

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.

2. Select **Sell**, followed by **Marketplace**. By default, you will see products of all types and categories.

3. Select a filter by type or category. You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.

4. Select a specific product offer from the list. This will take you to a product Overview tab where you can learn more about the offer. Information on this tab might include: 

    - A description of the product or offer

    - More information about the ISV publisher

    - Links to documentation or marketing materials uploaded by the ISV publisher

    - Other possible ISV contacts for customer support, engineering, or a contact for the CSP Program

5. To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:

    - The markets where this offer is available to you

    - A list of SKUs or plans available for the offer

    - Pricing for each SKU or Plan available

## <a name="view-marketplace-offers-via-partner-center-apis"></a>View Marketplace offers via Partner Center APIs

CSP program partners can also use APIs to return a list of eligible offers. Eligible offers will be only those SaaS ISV offers available for the partner to sell via the Partner Center marketplace. For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>View the latest Marketplace offer pricing in Partner Center

Follow these steps for the latest pricing details associated with an offer:

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.

2. Select **Sell**, followed by **Marketplace**. A list of Marketplace offers will appear.

3. Scroll down to the **Marketplace** section (below **Azure plan pricing**) and select **Export price list** from the upper right corner. This generates a spreadsheet with the latest pricing data for SaaS, license-based offers available from ISV publishers. Some Azure application pricing may also appear here. This information is updated daily, so you can check it for current prices as often as you choose.

4. If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:

    - One row shows the free trial price of zero. This means a free trial period is available.

    - The other row shows the price and terms that will apply after the free trial period is over.

As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers. For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).

## <a name="learn-about-marketplace-exclusive-offers"></a>Learn about marketplace exclusive offers

ISVs have the option to make their offers available only to specific partners in the CSP program. This is known as an Exclusive offer. All partners in the CSP program can still view all ISV offers in the Partner Center commercial marketplace, including those offers marked Exclusive.

If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).

For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.

> [!NOTE]
> If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer. When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.

To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](https://docs.microsoft.com/azure/marketplace/cloud-solution-providers).

For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Nächste Schritte

- [Purchase commercial marketplace offers](csp-commercial-marketplace-purchase.md)