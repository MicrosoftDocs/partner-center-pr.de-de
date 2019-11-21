---
title: How the partner earned credit is calculated | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how the partner earned credit (PEC) aspect of Azure plan is calculated. This includes eligibility requirements for partners and indirect providers.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 59cbc822e886b031a49c281334e8287580311408
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253416"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a>How the partner earned credit (PEC) is calculated


Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC. The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft. The credit is calculated daily and reflected in the monthly invoice. By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription. Additional ways in which customer can provision access for transacting partner are described in the following section.   


## <a name="important-eligibility-and-calculation-requirements"></a>Important eligibility and calculation requirements:

- A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage. Learn more about [valid RBAC roles]

- The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.

- PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner. 

- PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).

- Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list. There are exceptions including, but not limited to, 3PP and Azure Reservations.

- PEC is calculated daily and can be viewed in the daily recon file. A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.

- PEC wird bis hinab zur Azure-Ressourcenebene erworben. If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC. 

- PEC will be included on the partner's monthly invoice. The invoice is net of charges. The details are shown in the invoice recon file.

For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).

Weitere Informationen

- [Azure plan - billing](azure-plan-billing.md)

- [Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP ](azure-plan-price-list.md)