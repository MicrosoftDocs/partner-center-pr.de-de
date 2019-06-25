---
title: Grundlegendes zu den Abrechnungsarten im Partner Center | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Information zu unterschiedlichen Abrechnungsarten, Abrechnungszeiträumen und Abrechnungsdaten
author: MaggiePucciEvans
ms.author: evansma
keywords: Abrechnung, Zahlungen, Bestellungen, Kontenabstimmungsdateien, Kontenabstimmungsdatei
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 3e664a8a539125bce21d256c6e6d88d1ab22d14d
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343458"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Grundlegendes zu Abrechnungsarten in Partner Center

**Gilt für**

-  Partner Center
-  Partner im CSP-Programm

Je nach den Typen der Produkte, die Sie für Ihre Kunden erwerben, gibt es möglicherweise unterschiedliche Abrechnungszeiträume, die an verschiedenen Tagen desselben Monats in Rechnung gestellt werden. In diesem Artikel wird erläutert, was sich ab dem 1. März 2019 geändert hat und wie sich die Änderungen auf Sie auswirken werden.

## <a name="billing-for-recurring-charges"></a>Abrechnung für wiederkehrende Gebühren

Das Abrechnungssystem für wiederkehrende Gebühren von lizenzbasierten und nutzungsbasierten Abonnements ändert sich nicht. Wir werden Ihnen weiterhin eine Rechnung an dem Tag des Monats stellen, den Sie als Ihr Abrechnungsdatum ausgewählt haben, und Ihr Abrechnungszeitraum bleibt weiterhin der Monat vor diesem Datum. Wenn Sie den 15. Tag des Monats als Ihr Abrechnungsdatum ausgewählt haben, werden wir Ihnen sämtliche Aktivitäten ab dem 15. eines Kalendermonats bis zum 14. des nächsten Kalendermonats in Rechnung stellen. Rechnungen und Kontenabstimmungsdateien stehen in der Regel 2–4 Tage nach Ihrem Abrechnungsdatum zur Verfügung.

Wie zuvor werden wir Ihnen diese Produkte in der Währung für das Land/die Region, in dem/der Sie sich befinden, in Rechnung stellen – unabhängig vom Standort des Kunden, an den Sie das Produkt verkauft haben.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Abrechnung für einmalige und ausgewählte wiederkehrende Gebühren

Ab dem 1. März 2019 haben wir ein neues Abrechnungssystem für wiederkehrende und einmalige Gebühren bei Produkten von Microsoft und Drittanbieter-ISVs eingeführt.

Bei diesen Produkten beginnt der Abrechnungszeitraum am 1. Tag des Kalendermonats, und er endet am letzten Tag des Kalendermonats. Wir werden Ihre Rechnung am 8. Tag des Folgemonats zur Verfügung stellen. 

Anders ausgedrückt: Alle Transaktionen, die Sie zwischen dem 1. Mai und dem 31. Mai 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juni angezeigt. Alle Transaktionen, die Sie zwischen dem 1. Juni und dem 30. Juni 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juli angezeigt. Möglicherweise werden wiederkehrende und einmalige Käufe in derselben Monatsrechnung abgerechnet. 

Sie können auch jederzeit Ihren Kontostand/Ihre Rechnung überprüfen (z.B. zwischen dem 1. Mai und dem 7. Juni) und die neueste Kontoaktivität sehen, ohne auf die Monatsrechnung warten zu müssen. Beachten Sie bitte Folgendes: Wenn wir Ihre Rechnung am 8. bereitstellen, enthält sie Steuern sowie alle anderen anwendbaren Gebühren und Guthaben. Deshalb kann der endgültige Betrag von demjenigen abweichen, der Ihnen während des Abrechnungszeitraums angezeigt wird. 

Sie werden auf Ihre Rechnungen genauso wie jetzt zugreifen – entweder im Partner Center oder über API. Die Rechnungen werden am 8. Tag des Monats vor Mitternacht UTC angezeigt. 

|**Abrechnungssystem**|**Produkttyp(en)**|**Abrechnungsdatum**|**Abrechnungszeitraum**|**Abrechnungswährung**|**Aktuelle Aktivität anzeigen?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Wiederkehrende Gebühren für lizenzbasierte und nutzungsbasierte Abonnements |Alle Produkte aus dem [Katalog der Onlinedienste](https://partner.microsoft.com/commerce/preferredoffers/list). Beispiele hierfür sind Office 365, Microsoft 365, Azure Active Directory, Azure (nutzungsbasierte Bezahlung), Dynamics 365, Power BI Pro |Das Datum, das Sie bei der Erstellung Ihres Partner Center-Kontos ausgewählt haben |Der Monat vor Ihrem Abrechnungsdatum. |Die Währung des Landes/der Region, in dem/der Sie sich befinden. Wenn sich Ihr Unternehmen beispielsweise in Großbritannien befindet, werden wir die Rechnung in Britische Pfund (GBP) stellen. Befindet sich Ihr Unternehmen in Indien, erhalten Sie eine Rechnung in Indische Rupien (INR).  |Nein |
|Wiederkehrende und einmalige Gebühren für Produkte von Microsoft und Drittanbieter-ISVs |Alle SaaS-Abonnements, Azure-Reservierungen und Softwareprodukte (unbefristet und abonnementbasiert), die von Microsoft und Drittanbieter-ISVs angeboten werden. Sehen Sie dazu verfügbare Produkte im [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Beispiele hierfür sind SUSE Linux-Software (Softwareabonnement), Windows Server 2019 Essentials (unbefristete Software), Azure ISV-SaaS-Produktabonnement. |Der 8. Tag jedes Monats |Vom ersten Tag bis zum letzten Tag jedes Kalendermonats |Die Währung des Landes/der Region, in dem/der sich Ihr Kunde befindet. Dies bedeutet: Sie erhalten getrennte Rechnungen und Kontenabstimmungsdateien in der Währung für das Land/die Region jedes Kunden, an den Sie im Abrechnungszeitraum verkauft haben. |Ja |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Szenarien für die einmalige Ausführungen und zeitplanserien Käufe Abrechnung
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Szenario 1: erwerben Sie ein Abonnement, und fügen Sie einen Sitzplatz am selben Tag hinzu

In Szenario 1 erwerben Sie ein Abonnement für den 11. Juni, zum Einheitenpreis von je 4 $. Später denselben Tag erwerben Sie einen anderen des gleichen Abonnements zum selben Preis. 

Die Abstimm Datei umfasst Folgendes: 
-   je 4 $ Rechnung für Dienst-Zeitraum 10. Juni – 9. Juli. 
-   $-4.00 anteilig Rebill für Dienst-Zeitraum am 11. Juni – 11. Juni. Dies ist der Zeitraum, wenn Sie 1-Lizenz haben. Berechnung (monatliche Preis/Gesamt Tage innerhalb des Diensts) = x Tage in anteilige Service Zeitraum X Anzahl der Lizenzen (4/30) X = 30 x 1 = 4.00.
-   $8.00 anteilig Rebill Service Zeitraum 10. Juni – 9. Juli. Dies ist der Zeitraum, wenn Sie 2 Lizenzen haben. Berechnung = (4/30) X 30 x 2 = 8.00.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Neu         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Szenario 2 – ein Abonnement erwerben, und klicken Sie dann später weitere hinzufügen

In Szenario 2 Sie erwerben Sie ein Abonnement für den 11. Juni zum Einheitenpreis von je 4 $ und am 12. Juni erwerben Sie ein anderes Abonnement, für das gleiche Produkt zum selben Preis. 

Die Abstimm Datei umfasst Folgendes: 
-   je 4 $ Rechnung für Dienst-Zeitraum 10. Juni – 9. Juli. 
-   $-3.87 anteilig Rebill für Dienst-Zeitraum am 11. Juni – 12. Juni. Dies ist der Zeitraum, wenn Sie 1-Lizenz haben. Berechnung (monatliche Preis/Gesamt Tage innerhalb des Diensts) = x Tage in anteilige Service Zeitraum X Anzahl der Lizenzen (4/30) X = 29 x 1 = 3.87.
-   $7.74 anteilig Rebill für Dienst-Zeitraum dem 12. Juni – 9. Juli. Dies ist der Zeitraum, wenn Sie 2 Lizenzen haben. Berechnung = (4/30) X 29 x 2 = 7.74.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (Sie müssen eine Lizenz)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Neu         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3.87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7.74       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Szenario 3: ein Abonnement erwerben, und entfernen Sie einen Sitzplatz am selben Tag

In Szenario 3 erwerben Sie zwei Abonnements für das gleiche Produkt am 11. Juni zum Einheitenpreis von je 4 $. Später denselben Tag entfernen Sie eines der Arbeitsplätze.  

Die Abstimm Datei umfasst Folgendes: 
-   8 US -Dollar Stückliste für zwei Lizenzen für Dienst-Zeitraum 10. Juni – 9. Juli. 
-   $-8.00 anteilig Rebill für Dienst-Zeitraum am 11. Juni – 11. Juni. Dies ist der Zeitraum, wenn Sie 2 Lizenzen haben. Berechnung (monatliche Preis/Gesamt Tage innerhalb des Diensts) = x Tage in anteilige Service Zeitraum X Anzahl der Lizenzen (4/30) X = 30 x 2 = 8.00.
-   $4.00 anteilig Rebill für Dienst-Zeitraum am 11. Juni – 9. Juli. Dies ist der Zeitraum, wenn Sie 1-Lizenz haben. Berechnung = (4/30) X 30 x 1 = 4.00.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Neu         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Szenario 4: ein Abonnement erwerben, und entfernen Sie dann das Arbeitsplätze später

In Szenario 4 Sie am 11. Juni 2-Abonnements erwerben, zum Einheitenpreis von je 4 $, und am 12. Juni, entfernen Sie eines der die Arbeitsplätze. 

Die Abstimm Datei umfasst Folgendes: 
-   8 US -Dollar-Rechnung für Service-Dauer 10. Juni – 9. Juli. 
-   $-7.74 anteilig Rebill für Dienst-Zeitraum am 11. Juni – 12. Juni. Dies ist der Zeitraum, wenn Sie 2 Lizenzen haben. Berechnung (monatliche Preis/Gesamt Tage innerhalb des Diensts) = x Tage in anteilige Service Zeitraum X Anzahl der Lizenzen (4/30) X = 29 x 2 = 7.74.
-   $3.87 anteilig Rebill für Dienst-Zeitraum dem 12. Juni – 9. Juli. Dies ist der Zeitraum, wenn Sie 1-Lizenz haben. Berechnung = (4/30) X 29 x 1 = 3.87.

|**Kaufdatum**   |**Beginn der Abrechnung**  |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (müssen 2 Lizenzen)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Neu       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7.74       |removeQuantity           |
|6/12/2019 (Sie haben ein 1-Lizenz)    | 6/10/2019    |7/09/2019   |$4    |1      |$3.87    |removeQuantity |
