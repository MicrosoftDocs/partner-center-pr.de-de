---
title: Allgemeine Abrechnungsszenarien | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn what you will see on your bill after you add new subscriptions, adjust the number of licenses in a subscription, or cancel a subscription.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: Abrechnung, Zahlungen, Bestellungen, Nutzung, lizenzbasierte Abrechnung, Abonnementdatum, Laufzeit, Kündigung, Verlängerung, Kontenabstimmungsdatei, Abstimmungsdatei
ms.localizationpriority: medium
ms.openlocfilehash: d8afffa1dd11e386b03548c8f10e5490e6db5894
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253398"
---
# <a name="common-billing-scenarios"></a>Allgemeine Abrechnungsszenarien

**Zielgruppe**

-   Programm für Cloud-Lösungsanbieter – Abrechnung

In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Anzahl von Lizenzen für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus.

## <a name="in-this-section"></a>In diesem Abschnitt

-   [Nutzungsbasierte Abrechnung](#usagebased)

-   [Lizenzbasierte Abrechnung](#licensebased)

## <a href="" id="usagebased"></a>Nutzungsbasierte Abrechnung

Nutzungsbasierte Abonnements werden zum Abonnementdatum monatlich rückwirkend abgerechnet. For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period December 15 - January 14. You will be charged again on February 15 for the service period January 15 - February 14, etc. The charges that are generated on the subscription anniversary day will appear on the following invoice and reconciliation file.

You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice. Dies ist kein Fehler. Es bedeutet lediglich, dass der Dienst mit einem Zeitstempel versehen wurde, nachdem die Dienste erfolgt sind. Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill. 

Nutzungsbasierte Abonnements können jederzeit ausgesetzt werden. 

Die Azure-CSP-Preisliste wird monatlich veröffentlicht und ist auf der Partner Center-Seite „Verkaufen“ -> „Preise und Angebote“ zu finden. Bitte beachten Sie, dass die Preise sich täglich ändern können und auf der Registerkarte „Änderungsverlauf“ der Preisliste angezeigt werden.

Nutzungsgebühren basieren auf Preisen pro Tag. Wenn sich der Preis während des Dienstzeitraums ändert, sehen Sie eine Rechnungsposition für jeden anteiligen Dienstzeitraum und den anzuwendenden Preis.

## <a href="" id="licensebased"></a>Lizenzbasierte Abrechnung

**Abrechnung:** lizenzbasierte Abonnements werden im Voraus zum Dauerauftragsdatum abgerechnet.

**Dauerauftragsdatum:** Das Dauerauftragsdatum ist der Tag des Monats, an dem Sie das Abonnement erworben haben. Wenn Sie das Abonnement beispielsweise am 15. Januar erworben haben, ist das Abonnementdatum der 15. jedes Monats.

**Laufzeit:** alle lizenzbasierten Abonnements haben einen kostenpflichtigen 12-Monats-Zahlungszeitraum, der am Kaufdatum beginnt.

**Kündigung:** Abonnements, die im ersten Monat angehalten werden, werden 100 % gutgeschrieben. Wird das Abonnement in dem Monaten 2 – 12 ausgesetzt, wird ein anteiliger Betrag gutgeschrieben.

**Verlängerung:** alle lizenzbasierte Abonnements werden automatisch 12 Monate nach dem kostenpflichtigen Zahlungszeitraum erneuert.

## <a href="" id="licensebasedmonthly"></a>Monatliche Abrechnungsszenarien

**Scenario 1: New subscription**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.02.2018         |12.03.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

**Scenario 2: Change license quantity**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13.01.2018        |12. Februar 2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |-4,00    
|13.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2,45       |1        |2,45    
|01.02.2018         |12. Februar 2018    | Anteiliger Zyklus für Instanz   |1.55       |2        |3,10    
|13.02.2018         |12.03.2018    | Anteiliger Zyklus für Instanz   |4,00       |2        |8,00    

**Preisformel pro Einheit:**

The monthly price is 4.00 and there are 31 days in the service period 1/13/2018 - 2/12/2018. Dies entspricht einem Preis pro Tag von 0,129 (4/31).

There are 19 days in the proration period 1/13/2018 - 1/31/2018.

Anteiliger Preis pro Einheit = 2,451 = 19 x 0,129

There are 12 days in the proration period 2/1/2018 - 2/12/2018.

Anteiliger Preis pro Einheit = 1,54 = 12 x 0,129

**Scenario 3: Suspend before 30 days**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 1. Februar setzen Sie das Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12. Februar 2018|Stornierungsgebühr|-4,00|1|-4,00

**Scenario 4: Suspend after 30 days**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12. Februar 2018|Gebühr für Zyklus|4,00|1|4,00

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.02.2018|12.03.2018|Gebühr für Zyklus|4,00|1|4,00

Am 1. März setzen Sie das Abonnement aus. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.03.2018|Stornierungsgebühr|-1,72|1|-1,72

**Preisformel pro Einheit:**

The monthly price is 4.00 and there are 28 days in the service period 2/13/2018 - 3/12/2018. Dies entspricht einem Preis pro Tag von 0,143 (4/28).

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

There are 12 days in the cancellation period 3/1/2018 - 3/12/2018. 

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).

## <a name="annual-billing-scenarios"></a>Jährliche Abrechnungsszenarien

**Scenario 1: New subscription**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

**Scenario 2: Add license after subscription anniversary date but before billing date**

Sie erwerben am 11.02.2017 ein neues Abonnement mit einer Lizenz für 211,20 USD pro Jahr. Das Abonnementdatum ist der 11. in jedem Monat. Das Microsoft-Abrechnungssystem erstellt folgende Rechnungspositionen: 

-   $211.20 charge for period 2/11/17 - 2/10/18. 

Am 12.02.2017 erwerben Sie eine zweite Lizenz. Ihr Abrechnungsdatum ist der 14.02.2017. Es werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen: 

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteilige Gebühren beim Kauf |211,20 |1 | 211,20 |

Zum Abonnementdatum 11.03.2017 generiert das Microsoft-Abrechnungssystem die folgenden Rechnungspositionen für die Lizenzerhöhung am 12.02.2017: 
-   -$211.20 credit for period 2/11/17 - 2/10/18. 
-   $0.58 prorated charge per license for 1 license for period 2/11/17 - 2/11/17. 
-   $15.62 prorated charge per license for 2 licenses for period 2/12/17 - 3/10/2017. 
-   $195.00 prorated charge per license for 2 licenses for period 3/11/2017 - 2/10/2018. 

Am 11.02.2017 erwerben Sie ein Abonnement. Am 12.02.2017 fügen Sie eine Lizenz hinzu. Ihr Abrechnungsdatum ist der 14.02.2017. Am 11.02.2018 wird Ihr Abonnement verlängert.

Am nächsten Abrechnungsdatum, dem 14.03.2017, werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen: 

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |-211,20 |1 |-211,20 |
|11.02.2017 |11.02.2017 |Anteiliger Zyklus für Instanz |0,58 |1 |0,58 |
|12.02.2017 |10.03.2017 |Anteiliger Zyklus für Instanz |15,62 |2 |31,25 |
|11.03.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |195,00 |2 |390,00 |

Am 11.02.2018 wird das Abonnement um weitere 12 Monate verlängert.


**Scenario 3: Change license quantity**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13.01.2018|12.01.2019|Anteiliger Zyklus für Instanz|-48,00|1|-48,00
13.01.2018|31.01.2018|Anteiliger Zyklus für Instanz|2,47|1|2,47
01.02.2018|12.01.2019|Anteiliger Zyklus für Instanz|44,98|2|89,96

**Preisformel pro Einheit:**

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

There are 19 days in service period 1/13/2018 - 1/31/2018. 

Der Preis pro Einheit beträgt also = 2,47 (19 x 0,13 x 1)

There are 346 days in service period 2/1/2018 - 1/12/2019. 

Der Preis pro Einheit beträgt also 44,98 (346 x 0,13 x 2).

**Scenario 4: Suspend before 30 days**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar setzen Sie Ihr Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

**Scenario 5: Suspend after 30 days**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei keine Rechnungspositionen für dieses Abonnement.
Am 1. März setzen Sie Ihr Abonnement aus. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Stornierungsgebühr|-41,34|1|-41,34

**Preisformel pro Einheit:**

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

There are 318 days in service period 3/1/2018 - 1/12/2019. 

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1). Da dies eine Gutschrift ist, beträgt der Preis pro Einheit -41,34.

**Scenario 6: Suspend and reactivate**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar setzen Sie Ihr Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

Am 1. März aktivieren Sie Ihr Abonnement erneut. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Anteilige Gebühren beim Kauf|41,34|1|41,34

**Preisformel pro Einheit:**

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

There are 318 days in service period 3/1/2018 - 1/12/2019. 

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1).
