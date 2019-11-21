---
title: Grundlegendes zu den Abrechnungsarten im Partner Center | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn about different billing types, billing periods, and billing dates you might see in Partner Center.
author: MaggiePucciEvans
ms.author: evansma
keywords: Abrechnung, Zahlungen, Bestellungen, Kontenabstimmungsdateien, Kontenabstimmungsdatei
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 539d3150e571c33114feee2d316611d7ac324f24
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253203"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Grundlegendes zu Abrechnungsarten in Partner Center

**Zielgruppe**

-  Partner Center
-  Partner im CSP-Programm

Je nach den Typen der Produkte, die Sie für Ihre Kunden erwerben, gibt es möglicherweise unterschiedliche Abrechnungszeiträume, die an verschiedenen Tagen desselben Monats in Rechnung gestellt werden. In diesem Artikel wird erläutert, was sich ab dem 1. März 2019 geändert hat und wie sich die Änderungen auf Sie auswirken werden.

## <a name="billing-for-recurring-charges"></a>Abrechnung für wiederkehrende Gebühren

Das Abrechnungssystem für wiederkehrende Gebühren von lizenzbasierten und nutzungsbasierten Abonnements ändert sich nicht. We'll continue to bill you on the day of the month you selected as your billing date, and your billing period will continue to be the month prior to that date. If you selected the 15th day of the month for your billing date, you'll be billed for all activity from the 15th of one calendar month to the 14th of the next calendar month. Rechnungen und Kontenabstimmungsdateien stehen in der Regel 2–4 Tage nach Ihrem Abrechnungsdatum zur Verfügung.

As before, we'll bill you for these products in the currency for the country/region you're located in, regardless of the location of the customer you sold the product to.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Abrechnung für einmalige und ausgewählte wiederkehrende Gebühren

Ab dem 1. März 2019 haben wir ein neues Abrechnungssystem für wiederkehrende und einmalige Gebühren bei Produkten von Microsoft und Drittanbieter-ISVs eingeführt.

Bei diesen Produkten beginnt der Abrechnungszeitraum am 1. Tag des Kalendermonats, und er endet am letzten Tag des Kalendermonats. We'll make your invoice available on the 8th day of the following month. 

Anders ausgedrückt: Alle Transaktionen, die Sie zwischen dem 1. Mai und dem 31. Mai 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juni angezeigt. Alle Transaktionen, die Sie zwischen dem 1. Juni und dem 30. Juni 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juli angezeigt. Möglicherweise werden wiederkehrende und einmalige Käufe in derselben Monatsrechnung abgerechnet. 

Sie können auch jederzeit Ihren Kontostand/Ihre Rechnung überprüfen (z.B. zwischen dem 1. Mai und dem 7. Juni) und die neueste Kontoaktivität sehen, ohne auf die Monatsrechnung warten zu müssen. Beachten Sie bitte Folgendes: Wenn wir Ihre Rechnung am 8. bereitstellen, enthält sie Steuern sowie alle anderen anwendbaren Gebühren und Guthaben. Deshalb kann der endgültige Betrag von demjenigen abweichen, der Ihnen während des Abrechnungszeitraums angezeigt wird. 

You'll access your invoices the same way you do now, either in Partner Center or by API. They'll appear before midnight UTC on the 8th day of the month. 

|**Abrechnungssystem**|**Produkttyp(en)**|**Abrechnungsdatum**|**Abrechnungszeitraum**|**Abrechnungswährung**|**Aktuelle Aktivität anzeigen?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Wiederkehrende Gebühren für lizenzbasierte und nutzungsbasierte Abonnements |Alle Produkte aus dem [Katalog der Onlinedienste](https://partner.microsoft.com/commerce/preferredoffers/list). Beispiele hierfür sind Office 365, Microsoft 365, Azure Active Directory, Azure (nutzungsbasierte Bezahlung), Dynamics 365, Power BI Pro |Das Datum, das Sie bei der Erstellung Ihres Partner Center-Kontos ausgewählt haben |Der Monat vor Ihrem Abrechnungsdatum. |The currency of the country/region you're located in. For example, if your company is located in the United Kingdom, we'll bill you in British pounds sterling (GBP). If your company is located in India, we'll bill you in India Rupees (INR).  |Nein |
|Wiederkehrende und einmalige Gebühren für Produkte von Microsoft und Drittanbieter-ISVs |Alle SaaS-Abonnements, Azure-Reservierungen und Softwareprodukte (unbefristet und abonnementbasiert), die von Microsoft und Drittanbieter-ISVs angeboten werden. Sehen Sie dazu verfügbare Produkte im [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Beispiele hierfür sind SUSE Linux-Software (Softwareabonnement), Windows Server 2019 Essentials (unbefristete Software), Azure ISV-SaaS-Produktabonnement. |Der 8. Tag jedes Monats |Vom ersten Tag bis zum letzten Tag jedes Kalendermonats |Die Währung des Landes/der Region, in dem/der sich Ihr Kunde befindet. This means you'll receive separate invoices and reconciliation files in the currency of the country/region each customer you sold to in the billing period. |„Ja“ |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Abrechnungsszenarien für einmalige und wiederkehrende Käufe
### <a name="scenario-1---purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Scenario 1 - Purchase a subscription and then add a seat on the same day

In Szenario 1 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag erwerben ein weiteres gleiches Abonnement zum gleichen Preis. 

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $4 bill for service period June 10 - July 9. 
-   $-4.00 prorated rebill for service period June 11 - June 11. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 1 = 4,00.
-   $8.00 prorated rebill for service period June 10 - July 9. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (4/30) x 30 x 2 = 8,00.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 USD                |1                 |4 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 2      |-8 USD         |addQuantity           |

### <a name="scenario-2---purchase-a-subscription-and-then-add-more-later"></a>Scenario 2 - Purchase a subscription and then add more later

In Szenario 2 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Am 12. Juni erwerben Sie ein weiteres Abonnement für das gleiche Produkt zum gleichen Preis. 

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $4 bill for service period June 10 - July 9. 
-   $-3.87 prorated rebill for service period June 11 - June 12. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 1 = 3,87.
-   $7.74 prorated rebill for service period June 12 - July 9. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung = (4/30) x 29 x 2 = 7,74.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie verfügen über eine Lizenz)     |10.06.2019   |09.07.2019         |4 USD         |1        |4 USD            |Neu         |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

### <a name="scenario-3---purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Scenario 3 - Purchase a subscription and then remove a seat on the same day

In Szenario 3 erwerben Sie zwei Abonnements für das gleiche Produkt am 11. Juni mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag entfernen Sie einen der Arbeitsplätze.  

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $8 bill for two licenses for service period June 10 - July 9. 
-   $-8.00 prorated rebill for service period June 11 - June 11. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 2 = 8,00.
-   $4.00 prorated rebill for service period June 11 - July 9. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung = (4/30) x 30 x 1 = 4,00.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 USD                |2                 |-8 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 1      |4 USD         |removeQuantity           |

### <a name="scenario-4---purchase-a-subscription-and-then-remove-seats-later"></a>Scenario 4 - Purchase a subscription and then remove seats later

In Szenario 4 erwerben Sie am 11. Juni 2 Abonnements mit einem Preis pro Einheit von 4 USD. Am 12. Juni entfernen Sie einen der Arbeitsplätze. 

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $8 bill for service period June 10 - July 9. 
-   $-7.74 prorated rebill for service period June 11 - June 12. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 2 = 7,74.
-   $3.87 prorated rebill for service period June 12 - July 9. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung = (4/30) x 29 x 1 = 3,87.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie haben 2 Lizenzen)     |10.06.2019   |09.07.2019         |4 USD         |2        |-8 USD       |Neu       |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12.06.2019 (Sie haben 1 Lizenz)    | 10.06.2019    |09.07.2019   |4 USD    |1      |3,87 USD    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Abrechnungsszenarien für SaaS-Transaktionen, die auf einer kostenlosen Testlizenz basieren
### <a name="scenario-5---renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Scenario 5 - Renew a license-based free trial SaaS subscription to a paid subscription at the end of the free trial period

In diesem Szenario erwerben Sie am 10. Juni ein kostenloses, testlizenzbasiertes SaaS-Abonnement (Software-as-a-Service), das sich nach Ablauf der kostenlosen Testphase automatisch als kostenpflichtiges Abonnement verlängert. 

Die Kontenabstimmungsdateien enthalten Folgendes: 
- $0 bill for service period June 10 - July 9 
- $2 bill for service period July 10 - August 9

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10.06.2019 (Sie haben 1 Lizenz)      |10.06.2019   |09.07.2019         |0 USD                |1                 |0 USD            |Neu         |
|10.07.2019 (Sie haben 1 Lizenz)     | 10.07.2019    |09.08.2019        |2 USD        |1        | 2 USD       |renew           |

### <a name="scenario-6---cancel-a-license-based-free-trial-saas-subscription"></a>Scenario 6 - Cancel a license-based free trial SaaS subscription

Sie können ein lizenzbasiertes kostenloses SaaS-Testabonnement (Software-as-a-Service) jederzeit kündigen, auch während des kostenlosen Testzeitraums. 

In diesem Szenario erwerben Sie am 1. Juli ein lizenzbasiertes kostenloses SaaS-Testabonnement und kündigen es dann sofort im Partner Center. 

Die Kontenabstimmungsdatei enthält Folgendes: 
- $0 bill for service period June 10th  - July 9th  for the new purchase
- $0 bill for service period July 10th  - July 9th for the cancelation

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10.06.2019 (Sie haben 11 Lizenzen)      |10.06.2019   |09.07.2019         |0 USD                |11                |0 USD            |Neu         |
|10.06.2019 (Sie haben null Lizenzen)     | 10.06.2019    |09.07.2019        |0 USD        |11       | 0 USD       |cancel           |

### <a name="scenario-7---convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Scenario 7 - Convert a custom meter SaaS subscription from one SKU to another for the same product on the same day

In diesem Szenario erwerben Sie eine SKU (Silver) unter einem Produkt und konvertieren sie am gleichen Tag in eine andere verfügbare SKU (Bronze) unter diesem Produkt. 

Die Kontenabstimmungsdatei enthält Folgendes: 
- $20 bill of Silver for service period June 10th, 2019 - July 9th, 2020
- $20 prorated rebill for Silver for service period June 10th, 2019 - July 9th, 2020
- $10 bill of Bronze for service period June 10th, 2019 - July 9th, 2020

|**Kaufdatum**   |**SKU**   |**Beginn der Abrechnung**   |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10.06.2019 (Sie haben 1 Lizenz) |Silver     |10.06.2019   |10.06.2019         |20 USD        |1         |20 USD            |Neu      |
|10.06.2019 (Sie haben 1 Lizenz) |Silver    | 10.06.2019    |10.06.2019        |20 USD        |1       | -20 USD       |Konvertieren           |
|10.06.2019 (Sie haben 1 Lizenz) |Bronze    | 10.06.2019    |10.06.2019        |10 USD        |1       | 10 USD       |Konvertieren           |

### <a name="scenario-8---purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Scenario 8 - Purchase and cancel a custom meter SaaS subscription from the Azure portal on the same day 

In diesem Szenario erwerben Sie ein benutzerdefiniertes SaaS-Abrechnungsabonnement im Azure-Portal und kündigen das Abonnement dann am gleichen Tag. 

|**Kaufdatum**   |**SKU**   |**Beginn der Abrechnung**   |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10.06.2019 (Sie haben 1 Lizenz) |Bronze     |10.06.2019   |10.06.2019         |10 USD        |1         |10 USD            |Neu      |
|10.06.2019 (Sie haben 0 Lizenzen) |Bronze    | 10.06.2019    |10.06.2019        |10 USD        |1       | -10 USD       |CancelImmediate  |

## <a name="billing-under-the-azure-plan"></a>Billing under the Azure plan

- **Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).

- **Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1 - 10/31, 11/1 - 11/30).

- **Charge service periods**: Charges will align to the calendar month. Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10. The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.

- **Invoice payment term**: Net 60 days.

- **Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency. Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.

- **Partner incentives**: Paid 45 days from the end of the invoice month.

For information on the Azure plan see:

- [Azure plan - overview](azure-plan-get-started.md)

- [Azure plan - billing](azure-plan-billing.md)