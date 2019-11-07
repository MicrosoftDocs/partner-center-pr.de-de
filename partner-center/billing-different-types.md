---
title: Grundlegendes zu den Abrechnungsarten im Partner Center | Partner Center
ms.topic: article
ms.date: 10/04/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Information zu unterschiedlichen Abrechnungsarten, Abrechnungszeiträumen und Abrechnungsdaten
author: MaggiePucciEvans
ms.author: evansma
keywords: Abrechnung, Zahlungen, Bestellungen, Kontenabstimmungsdateien, Kontenabstimmungsdatei
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b5991e5134d56684fb1ef43db5785d904fc9c15a
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653749"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Grundlegendes zu Abrechnungsarten in Partner Center

**Zielgruppe**

-  Partner Center
-  Partner im CSP-Programm

Je nach den Typen der Produkte, die Sie für Ihre Kunden erwerben, gibt es möglicherweise unterschiedliche Abrechnungszeiträume, die an verschiedenen Tagen desselben Monats in Rechnung gestellt werden. In diesem Artikel wird erläutert, was sich ab dem 1. März 2019 geändert hat und wie sich die Änderungen auf Sie auswirken werden.

## <a name="billing-for-recurring-charges"></a>Abrechnung für wiederkehrende Gebühren

Das Abrechnungssystem für wiederkehrende Gebühren von lizenzbasierten und nutzungsbasierten Abonnements ändert sich nicht. Wir berechnen Ihnen weiterhin den Tag des Monats, den Sie als Abrechnungsdatum ausgewählt haben, und der Abrechnungszeitraum liegt weiterhin im Monat vor diesem Datum. Wenn Sie den 15. Tag des Monats für das Abrechnungsdatum ausgewählt haben, werden Ihnen alle Aktivitäten von 15. eines Kalendermonats bis zum 14. des nächsten Kalendermonats in Rechnung gestellt. Rechnungen und Kontenabstimmungsdateien stehen in der Regel 2–4 Tage nach Ihrem Abrechnungsdatum zur Verfügung.

Wie zuvor berechnen wir Ihnen diese Produkte in der Währung für das Land/die Region, in dem Sie sich befinden, und zwar unabhängig vom Standort des Kunden, an den Sie das Produkt verkauft haben.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Abrechnung für einmalige und ausgewählte wiederkehrende Gebühren

Ab dem 1. März 2019 haben wir ein neues Abrechnungssystem für wiederkehrende und einmalige Gebühren bei Produkten von Microsoft und Drittanbieter-ISVs eingeführt.

Bei diesen Produkten beginnt der Abrechnungszeitraum am 1. Tag des Kalendermonats, und er endet am letzten Tag des Kalendermonats. Wir machen Ihre Rechnung am 8. Tag des folgenden Monats verfügbar. 

Anders ausgedrückt: Alle Transaktionen, die Sie zwischen dem 1. Mai und dem 31. Mai 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juni angezeigt. Alle Transaktionen, die Sie zwischen dem 1. Juni und dem 30. Juni 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juli angezeigt. Möglicherweise werden wiederkehrende und einmalige Käufe in derselben Monatsrechnung abgerechnet. 

Sie können auch jederzeit Ihren Kontostand/Ihre Rechnung überprüfen (z.B. zwischen dem 1. Mai und dem 7. Juni) und die neueste Kontoaktivität sehen, ohne auf die Monatsrechnung warten zu müssen. Beachten Sie bitte Folgendes: Wenn wir Ihre Rechnung am 8. bereitstellen, enthält sie Steuern sowie alle anderen anwendbaren Gebühren und Guthaben. Deshalb kann der endgültige Betrag von demjenigen abweichen, der Ihnen während des Abrechnungszeitraums angezeigt wird. 

Sie können auf Ihre Rechnungen auf die gleiche Weise wie in der Partner Center-oder API-API zugreifen. Sie werden am 8. Tag des Monats vor Mitternacht UTC angezeigt. 

|**Abrechnungssystem**|**Produkttyp(en)**|**Abrechnungsdatum**|**Abrechnungszeitraum**|**Abrechnungswährung**|**Aktuelle Aktivität anzeigen?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Wiederkehrende Gebühren für lizenzbasierte und nutzungsbasierte Abonnements |Alle Produkte aus dem [Katalog der Onlinedienste](https://partner.microsoft.com/commerce/preferredoffers/list). Beispiele hierfür sind Office 365, Microsoft 365, Azure Active Directory, Azure (nutzungsbasierte Bezahlung), Dynamics 365, Power BI Pro |Das Datum, das Sie bei der Erstellung Ihres Partner Center-Kontos ausgewählt haben |Der Monat vor Ihrem Abrechnungsdatum. |Die Währung des Landes bzw. der Region, in dem Sie sich befinden. Wenn sich Ihr Unternehmen z. b. im Vereinigten Königreich befindet, rechnen wir Sie mit den US-Amerika US US-Amerika-Pfund Sterling (GBP). Wenn sich Ihr Unternehmen in Indien befindet, werden wir Sie in den indischen Rupes (INR) berechnen.  |Nein |
|Wiederkehrende und einmalige Gebühren für Produkte von Microsoft und Drittanbieter-ISVs |Alle SaaS-Abonnements, Azure-Reservierungen und Softwareprodukte (unbefristet und abonnementbasiert), die von Microsoft und Drittanbieter-ISVs angeboten werden. Sehen Sie dazu verfügbare Produkte im [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Beispiele hierfür sind SUSE Linux-Software (Softwareabonnement), Windows Server 2019 Essentials (unbefristete Software), Azure ISV-SaaS-Produktabonnement. |Der 8. Tag jedes Monats |Vom ersten Tag bis zum letzten Tag jedes Kalendermonats |Die Währung des Landes/der Region, in dem/der sich Ihr Kunde befindet. Dies bedeutet, dass Sie separate Rechnungen und Abstimmungs Dateien in der Währung des Landes bzw. der Region für jeden Kunden, den Sie im Abrechnungszeitraum verkauft haben, erhalten. |„Ja“ |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Abrechnungsszenarien für einmalige und wiederkehrende Käufe
### <a name="scenario-1---purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Szenario 1: erwerben eines Abonnements und anschließendes Hinzufügen eines Arbeitsplatzes am selben Tag

In Szenario 1 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag erwerben ein weiteres gleiches Abonnement zum gleichen Preis. 

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $4 Rechnung für Dienst Zeitraum, 10. Juni, 9. Juli. 
-   $-4,00 anbidirektionierte Rechnung für den Dienst Zeitraum 11. Juni 11. Juni. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 1 = 4,00.
-   $8,00 anbidirektionierte Rechnung für den Dienst Zeitraum 10. Juni 9. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (4/30) x 30 x 2 = 8,00.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 USD                |1                 |4 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 2      |-8 USD         |addQuantity           |

### <a name="scenario-2---purchase-a-subscription-and-then-add-more-later"></a>Szenario 2: erwerben eines Abonnements und anschließendes Hinzufügen später

In Szenario 2 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Am 12. Juni erwerben Sie ein weiteres Abonnement für das gleiche Produkt zum gleichen Preis. 

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $4 Rechnung für Dienst Zeitraum, 10. Juni, 9. Juli. 
-   $-3,87 anbidirektionierte Rechnung für Dienst Zeitraum 11. Juni 12. Juni. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 1 = 3,87.
-   $7,74 anbidirektionierte Rechnung für den Dienst Zeitraum 12. Juli 9. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung = (4/30) x 29 x 2 = 7,74.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie verfügen über eine Lizenz)     |10.06.2019   |09.07.2019         |4 USD         |1        |4 USD            |Neu         |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

### <a name="scenario-3---purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Szenario 3: erwerben eines Abonnements und anschließendes Entfernen eines Arbeitsplatzes am selben Tag

In Szenario 3 erwerben Sie zwei Abonnements für das gleiche Produkt am 11. Juni mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag entfernen Sie einen der Arbeitsplätze.  

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $8 Rechnung für zwei Lizenzen für Dienst Zeitraum: 10. Juli 9. 
-   $-8,00 anbidirektionierte Rechnung für den Dienst Zeitraum 11. Juni 11. Juni. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 2 = 8,00.
-   $4,00 anbidirektionierte Rechnung für den Dienst Zeitraum am 11. Juli 9. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung = (4/30) x 30 x 1 = 4,00.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 USD                |2                 |-8 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 1      |4 USD         |removeQuantity           |

### <a name="scenario-4---purchase-a-subscription-and-then-remove-seats-later"></a>Szenario 4: erwerben eines Abonnements und anschließendes Entfernen der Arbeitsplätze

In Szenario 4 erwerben Sie am 11. Juni 2 Abonnements mit einem Preis pro Einheit von 4 USD. Am 12. Juni entfernen Sie einen der Arbeitsplätze. 

Die Kontenabstimmungsdatei enthält Folgendes: 
-   $8 Rechnung für Dienst Zeitraum, 10. Juni, 9. Juli. 
-   $-7,74 anbidirektionierte Rechnung für Dienst Zeitraum 11. Juni 12. Juni. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 2 = 7,74.
-   $3,87 anbidirektionierte Rechnung für den Dienst Zeitraum 12. Juli 9. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung = (4/30) x 29 x 1 = 3,87.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie haben 2 Lizenzen)     |10.06.2019   |09.07.2019         |4 USD         |2        |-8 USD       |Neu       |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12.06.2019 (Sie haben 1 Lizenz)    | 10.06.2019    |09.07.2019   |4 USD    |1      |3,87 USD    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Abrechnungsszenarien für SaaS-Transaktionen, die auf einer kostenlosen Testlizenz basieren
### <a name="scenario-5---renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Szenario 5: Erneuern einer lizenzbasierten kostenlosen Testversion von Saas-Abonnements für ein kostenpflichtiges Abonnement am Ende des kostenlosen Testzeitraums

In diesem Szenario erwerben Sie am 10. Juni ein kostenloses, testlizenzbasiertes SaaS-Abonnement (Software-as-a-Service), das sich nach Ablauf der kostenlosen Testphase automatisch als kostenpflichtiges Abonnement verlängert. 

Die Kontenabstimmungsdateien enthalten Folgendes: 
- $0 Rechnung für Dienst Zeitraum 10. Juni 9 
- $2 Rechnung für Dienst Zeitraum, 10. August, 9. August

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10.06.2019 (Sie haben 1 Lizenz)      |10.06.2019   |09.07.2019         |0 USD                |1                 |0 USD            |Neu         |
|10.07.2019 (Sie haben 1 Lizenz)     | 10.07.2019    |09.08.2019        |2 USD        |1        | 2 USD       |renew           |

### <a name="scenario-6---cancel-a-license-based-free-trial-saas-subscription"></a>Szenario 6: kündigen eines lizenzbasierten kostenlosen Testversion von Saas-Abonnements

Sie können ein lizenzbasiertes kostenloses SaaS-Testabonnement (Software-as-a-Service) jederzeit kündigen, auch während des kostenlosen Testzeitraums. 

In diesem Szenario erwerben Sie am 1. Juli ein lizenzbasiertes kostenloses SaaS-Testabonnement und kündigen es dann sofort im Partner Center. 

Die Kontenabstimmungsdatei enthält Folgendes: 
- $0 Rechnung für Dienst Zeitraum am 10. Juli bis zum 9. Juli für den neuen Kauf
- $0 Rechnung für Dienst Zeitraum, 10. Juli, 9. Juli für den Abbruch

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10.06.2019 (Sie haben 11 Lizenzen)      |10.06.2019   |09.07.2019         |0 USD                |11                |0 USD            |Neu         |
|10.06.2019 (Sie haben null Lizenzen)     | 10.06.2019    |09.07.2019        |0 USD        |11       | 0 USD       |cancel           |

### <a name="scenario-7---convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Szenario 7: Konvertieren eines benutzerdefinierten Abrechnungs-Saas-Abonnements von einer SKU in eine andere für dasselbe Produkt am selben Tag

In diesem Szenario erwerben Sie eine SKU (Silver) unter einem Produkt und konvertieren sie am gleichen Tag in eine andere verfügbare SKU (Bronze) unter diesem Produkt. 

Die Kontenabstimmungsdatei enthält Folgendes: 
- $20-Rechnung von Silber für Dienst Zeitraum, 10. Juni, 2019 Uhr, 9. Juli, 2020
- $20 anteilsmäßig auf Abrechnungen für Silber für den Dienst Zeitraum, 10. Juni, 2019-15. Juli, 2020
- $10 Rechnung von Bronze für Dienst Zeitraum, 10. Juni, 2019 Uhr, 9. Juli, 2020

|**Kaufdatum**   |**SKU**   |**Beginn der Abrechnung**   |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10.06.2019 (Sie haben 1 Lizenz) |Silver     |10.06.2019   |10.06.2019         |20 USD        |1         |20 USD            |Neu      |
|10.06.2019 (Sie haben 1 Lizenz) |Silver    | 10.06.2019    |10.06.2019        |20 USD        |1       | -20 USD       |Konvertieren           |
|10.06.2019 (Sie haben 1 Lizenz) |Bronze    | 10.06.2019    |10.06.2019        |10 USD        |1       | 10 USD       |Konvertieren           |

### <a name="scenario-8---purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Szenario 8: kaufen und kündigen eines benutzerdefinierten Abrechnungs-Saas-Abonnements aus dem Azure-Portal am selben Tag 

In diesem Szenario erwerben Sie ein benutzerdefiniertes SaaS-Abrechnungsabonnement im Azure-Portal und kündigen das Abonnement dann am gleichen Tag. 

|**Kaufdatum**   |**SKU**   |**Beginn der Abrechnung**   |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10.06.2019 (Sie haben 1 Lizenz) |Bronze     |10.06.2019   |10.06.2019         |10 USD        |1         |10 USD            |Neu      |
|10.06.2019 (Sie haben 0 Lizenzen) |Bronze    | 10.06.2019    |10.06.2019        |10 USD        |1       | -10 USD       |CancelImmediate  |

## <a name="billing-under-the-azure-plan"></a>Abrechnung im Azure-Plan

- **Rechnungsdatum**: die Rechnungs-und Abstimmungs Datei steht im Partner Center-Dashboard/in der API bis zum 8. (Mitternacht UTC) zur Verfügung.

- **Abrechnungszeitraum der Rechnung**: der Abrechnungszeitraum der Rechnung wird auf den Kalendermonat ausgerichtet, z. b. 10/1-10/31, 11/1-11/30).

- Gebühren für **Dienst Zeiträume**: die Gebühren richten sich nach dem Kalendermonat. Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10. Die Rechnung des nächsten Monats, die auf 12/8 generiert wird, enthält alle Gebühren für den Dienst Zeitraum 11/1-11/31.

- **Zahlungs Laufzeit der Rechnung**: net 60 Tage.

- **Rechnungswährung**: Partner werden weiterhin in der vom Kunden zugewiesenen Währung abgerechnet. Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.

- **Partner-Incentives**: bezahlt 45 Tage ab dem Ende des Rechnungsmonats.

Weitere Informationen zum Azure-Plan finden Sie unter:

- [Azure-Plan: Übersicht](azure-plan-get-started.md)

- [Azure-Plan: Abrechnung](azure-plan-billing.md)