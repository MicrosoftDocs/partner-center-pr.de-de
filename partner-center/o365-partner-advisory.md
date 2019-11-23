---
title: Office 365 Partner Advisory - Microsoft 365 Voice in CSP | Partner Center
description: PSTN services in some countries may be subject to special tax and regulatory requirements that may affect partner order and invoicing.
ms.topic: article
ms.date: 11/04/2019
author: maggiepuccievans
ms.author: evansma
keywords: Office, O365, PSTN services, taxes, requirements, invoice, invoicing
ms.localizationpriority: medium
ms.openlocfilehash: b6359a49503237e72c8cffdb5758bdd418910306
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384813"
---
# <a name="office-365-partner-advisory-microsoft-365-voice-in-csp"></a>Office 365 Partner Advisory: Microsoft 365 Voice in CSP

**Zielgruppe**

- Partner Center  

Public Switched Telephone Network (PSTN) services in some countries may be subject to special tax and regulatory requirements that may affect partner order and invoicing.  In the United States, Puerto Rico, and Canada, Skype for Business PSTN and Microsoft 365 Voice services are subject to special tax and regulatory requirements. In the United States and Puerto Rico, Microsoft prices PSTN services as tax-inclusive.  Unique PSTN taxes and regulations will affect Office 365 partners transacting Microsoft 365 Voice products.  Wenn ein Partner einen Aufschlag auf den Preis eines PSTN-Diensts von Microsoft erhebt, ist er möglicherweise für die Berechnung und Abführung von Steuern und Gebühren für PSTN-Dienste verantwortlich.

## <a name="partner-recommendations"></a>Partner Recommendations

Informieren Sie sich bei Ihren Steuer- und Rechtsberatern über die Verantwortlichkeiten Ihres Unternehmens in Bezug auf Bestimmungen, Steuern und Gebühren für PSTN-Dienste und andere mögliche Verpflichtungen.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Invoice Presentation and Partner Reconciliation File

CSP invoices and CSP reconciliation files in the United States, Puerto Rico and Canada which include Skype for Business PSTN and Microsoft 365 Voice services will provide separate line items for the PSTN and non-PSTN components.

Additionally, CSP invoices will display the following footnote:

* The price displayed is a charge for Audio Conferencing and Calling Plan Services.  Any applicable transactional taxes are charged exclusively of the amount shown except for sales made within the United States.  In the U.S., the price displayed is tax inclusive as it includes a charge for the Calling Plan and Audio Conferencing Services and a charge for the taxes and fees we are required to charge.  Audio Conferencing and Calling Plan Services are serviced by the Microsoft Affiliate authorized to provide them.  See [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) for details.

## <a name="reconciliation-file-example"></a>Reconciliation File Example

Office 365 Enterprise E5 presents on reconciliation file as two line items with identical names and identical IDs, but each line item has a unique unit price (example: $28.40 and $2.00). Dies unterscheidet die Skype for Business PSTN Conferencing-Komponente vom Office 365-Angebot, sodass Sie Steuern korrekt anwenden können.

**Partner Reconciliation example #1 (select columns):**

|**Permanente Angebots-ID**|**Angebotsname**|**Startdatum des Abonnements**|**Enddatum des Abonnements**|**Startdatum der Abrechnung**|**Enddatum der Abrechnung**|**Typ der Abrechnung**|**Preis pro Einheit**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Gebühr für Zyklus   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Gebühr für Zyklus   |2,00   |

**Partner Reconciliation example #2**

Microsoft 365 Business Voice available in Canada has additional PSTN taxable components that are consolidated on CSP Invoice (similar to Office 365 E5, two line items are presented, one for PSTN components and the other for non-PSTN components).  The CSP Reconciliation file for Microsoft 365 Business Voice will display all PSTN taxable components individually (individual PSTN components will not be consolidated in .CSV or API tool).  The summation of order details and billed amounts for customers found in the reconciliation file will match the CSP Invoice.

## <a name="additional-resources"></a>Weitere Ressourcen
For more details, visit the [Microsoft 365 for Partners](https://drumbeat.office.com/Pages/home2016.aspx) site.

