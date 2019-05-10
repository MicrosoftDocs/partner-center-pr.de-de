---
title: Allgemeine Abrechnungsszenarien | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Anzahl von Lizenzen für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: Abrechnung, Zahlungen, Bestellungen, Nutzung, lizenzbasierte Abrechnung, Abonnementdatum, Laufzeit, Kündigung, Verlängerung, Kontenabstimmungsdatei, Abstimmungsdatei
ms.localizationpriority: medium
ms.openlocfilehash: 2a619356577345923cd78499d2ae5a1f3c6c1614
ms.sourcegitcommit: f916aa2884239b205398c24d04d1f1dc41b63c2b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2019
ms.locfileid: "64668715"
---
# <a name="common-billing-scenarios"></a>Allgemeine Abrechnungsszenarien

**Gilt für**

-   Programm für Cloud-Lösungsanbieter – Abrechnung

In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Anzahl von Lizenzen für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus.

## <a name="in-this-section"></a>Inhalt dieses Abschnitts

-   [Nutzungsbasierte Abrechnung](#usagebased)

-   [Lizenzbasierte Abrechnung](#licensebased)

## <a href="" id="usagebased"></a>Nutzungsbasierte Abrechnung

Nutzungsbasierte Abonnements werden zum Abonnementdatum monatlich rückwirkend abgerechnet. Wenn beispielsweise das Abonnementdatum der 15. ist, werden Sie am 15. Januar für den Dienstzeitraum vom 15. Dezember bis zum 14. Januar belastet. Am 15. Februar werden Sie für den Dienstzeitraum 15. Januar bis zum 14. Februar erneut belastet usw. Die am Abonnementdatum generierten Gebühren werden in der dann folgenden Rechnung und Kontenabstimmungsdatei angezeigt.

Gelegentlich werden Sie feststellen, dass einige Nutzungsgebühren auf Ihrer Rechnung fehlen oder dass die Nutzung aus einem vorhergehenden Monat in der Rechnung des laufenden Monats berechnet wird. Dies ist kein Fehler. Es bedeutet lediglich, dass der Dienst mit einem Zeitstempel versehen wurde, nachdem die Dienste erfolgt sind. Die innerhalb von 24 Stunden nach dem Ende des Abrechnungszyklus berichtete Nutzung wird dann in der Rechnung des nächsten Monats angezeigt. 

Nutzungsbasierte Abonnements können jederzeit ausgesetzt werden. 

Die Azure-CSP-Preisliste wird monatlich veröffentlicht und ist auf der Partner Center-Seite „Verkaufen“ -> „Preise und Angebote“ zu finden. Bitte beachten Sie, dass die Preise sich täglich ändern können und auf der Registerkarte „Änderungsverlauf“ der Preisliste angezeigt werden.

Nutzungsgebühren basieren auf Preisen pro Tag. Wenn sich der Preis während des Dienstzeitraums ändert, sehen Sie eine Rechnungsposition für jeden anteiligen Dienstzeitraum und den anzuwendenden Preis.

## <a href="" id="licensebased"></a>Lizenzbasierte Abrechnung

**Abrechnung:** Lizenzbasierte Abonnements werden zum Abonnementdatum im Voraus abgerechnet.

**Abonnementdatum:** Das Abonnementdatum ist der Tag des Monats, an dem Sie das Abonnement erworben haben. Wenn Sie das Abonnement beispielsweise am 15. Januar erworben haben, ist das Abonnementdatum der 15. jedes Monats.

**Laufzeit:** Alle lizenzbasierten Abonnements haben eine kostenpflichtige 12-Monats-Laufzeit, die am Kaufdatum beginnt.

**Kündigung:** Abonnements, die im Monat 1 ausgesetzt wurden, werden zu 100 % gutgeschrieben. Wird das Abonnement in dem Monaten 2 – 12 ausgesetzt, wird ein anteiliger Betrag gutgeschrieben.

**Verlängerung:** Alle lizenzbasierten Abonnements werden 12 Monate nach der kostenpflichtigen Laufzeit automatisch verlängert.

## <a href="" id="licensebasedmonthly"></a>Monatliche Abrechnungsszenarien

**Szenario 1: Neues Abonnement**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.02.2018         |12.03.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

**Szenario 2: Änderung der Lizenzanzahl**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13.01.2018        |12.02.2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |-4,00    
|13.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2,45       |1        |2,45    
|01.02.2018         |12.02.2018    | Anteiliger Zyklus für Instanz   |1,55       |2        |3,10    
|13.02.2018         |12.03.2018    | Anteiliger Zyklus für Instanz   |4,00       |2        |8,00    

**Preisformel pro Einheit:**

Die monatliche Gebühr liegt bei 4,00, und es gibt 31 Tage im Dienstzeitraum vom 13.01.2018 bis zum 12.02.2018. Dies entspricht einem Preis pro Tag von 0,129 (4/31).

Es gibt 19 Tage im anteiligen Zeitraum vom 13.01.2018 bis zum 31.01.2018.

Anteiliger Preis pro Einheit = 2,451 = 19 x 0,129

Es gibt 12 Tage im anteiligen Zeitraum vom 01.02.2018 bis zum 12.02.2018.

Anteiliger Preis pro Einheit = 1,54 = 12 x 0,129

**Szenario: 3: Aussetzen eines Abonnements innerhalb von 30 Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 1. Februar setzen Sie das Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Stornierungsgebühr|-4,00|1|-4,00

**Szenario 4: Aussetzen eines Abonnements nach 30 Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Gebühr für Zyklus|4,00|1|4,00

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.02.2018|12.03.2018|Gebühr für Zyklus|4,00|1|4,00

Am 1. März setzen Sie das Abonnement aus. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.03.2018|Stornierungsgebühr|-1,72|1|-1,72

**Preisformel pro Einheit:**

Die monatliche Gebühr liegt bei 4,00, und es gibt 28 Tage im Dienstzeitraum vom 13.02.2018 bis zum 12.03.2018. Dies entspricht einem Preis pro Tag von 0,143 (4/28).

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 12 Tage im anteiligen Zeitraum vom 01.03.2018 bis zum 12.03.2018. 

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).

## <a name="annual-billing-scenarios"></a>Jährliche Abrechnungsszenarien

**Szenario 1: Neues Abonnement**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

**Szenario 2: Hinzufügen einer Lizenz nach dem Abonnementdatum, aber vor dem Abrechnungsdatum**

Sie erwerben am 11.02.2017 ein neues Abonnement mit einer Lizenz für 211,20 USD pro Jahr. Das Abonnementdatum ist der 11. in jedem Monat. Das Microsoft-Abrechnungssystem erstellt folgende Rechnungspositionen: 

-   211,20 USD Gebühr für den Zeitraum vom 11.02.2017 bis zum 10.02.2018. 

Am 12.02.2017 erwerben Sie eine zweite Lizenz. Ihr Abrechnungsdatum ist der 14.02.2017. Es werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen: 

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteilige Gebühren beim Kauf |211,20 |1 | 211,20 |

Zum Abonnementdatum 11.03.2017 generiert das Microsoft-Abrechnungssystem die folgenden Rechnungspositionen für die Lizenzerhöhung am 12.02.2017: 
-   Gutschrift über 211,20 USD für den Zeitraum vom 11.02.2017 bis zum 10.02.2918. 
-   0,58 USD anteilige Gebühr pro Lizenz für 1 Lizenz im Zeitraum vom 11.02.2017 bis zum 11.02.2017. 
-   15,62 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 12.02.2017 bis 10.03.2017. 
-   195,00 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 11.03.2017 bis zum 10.02.2018. 

Am 11.02.2017 erwerben Sie ein Abonnement. Am 12.02.2017 fügen Sie eine Lizenz hinzu. Ihr Abrechnungsdatum ist der 14.02.2017. Am 11.02.2018 wird Ihr Abonnement verlängert.

Am nächsten Abrechnungsdatum, dem 14.03.2017, werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen: 

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |-211,20 |1 |-211,20 |
|11.02.2017 |11.02.2017 |Anteiliger Zyklus für Instanz |0,58 |1 |0,58 |
|12.02.2017 |10.03.2017 |Anteiliger Zyklus für Instanz |15,62 |2 |31,25 |
|11.03.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |195,00 |2 |390,00 |

Am 11.02.2018 wird das Abonnement um weitere 12 Monate verlängert.


**Szenario: 3: Änderung der Lizenzanzahl**

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

Es gibt 19 Tage im Dienstzeitraum vom 13.01.2018 – 31.01.2018. 

Der Preis pro Einheit beträgt also = 2,47 (19 x 0,13 x 1)

Es gibt 346 Tage im Dienstzeitraum vom 01.02.2018 – 12.01.2019. 

Der Preis pro Einheit beträgt also 44,98 (346 x 0,13 x 2).

**Szenario 4: Aussetzen eines Abonnements innerhalb von 30 Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar setzen Sie Ihr Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

**Szenario 5: Aussetzen eines Abonnements nach 30 Tagen**

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

Es gibt 318 Tage im Dienstzeitraum vom 01.03.2018 bis zum 12.01.2019. 

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1). Da dies eine Gutschrift ist, beträgt der Preis pro Einheit -41,34.

**Szenario 6: Aussetzen und erneutes Aktivieren eines Abonnements**

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

Es gibt 318 Tage im Dienstzeitraum vom 01.03.2018 bis zum 12.01.2019. 

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1).
