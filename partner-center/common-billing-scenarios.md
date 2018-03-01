---
title: Allgemeine Abrechnungsszenarien | Partner Center
description: "In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Lizenzen für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, free period, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.openlocfilehash: 0bfdf6e5f5a9617413981f0a0758f25e0a0eca54
ms.sourcegitcommit: 359ba82a9e337b1f04d62f0bb2d5eb8f87102e34
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/09/2018
---
# <a name="common-billing-scenarios"></a>Allgemeine Abrechnungsszenarien

**Betrifft**

-  Partner Center
-  Partner Center für Microsoft Cloud für US-Behörden
-  Partner Center für Microsoft Cloud Deutschland

In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Lizenzen für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus.

## <a name="in-this-section"></a>In diesem Abschnitt

-   [Nutzungsbasierte Abrechnung](#usagebased)

-   [Lizenzbasierte Abrechnung](#licensebased)

## <a href="" id="usagebased"></a>Nutzungsbasierte Abrechnung

Es werden Ihnen nur Dienste berechnet, die im vorherigen Abrechnungszeitraums genutzt wurden. Alle Azure-Dienste oder -Anwendungen, die während des Abrechnungszeitraums aktiviert und genutzt werden, erscheinen in der nächsten Rechnung.

-   Getaktete Dienstleistungspreise können sich während des Abrechnungszyklus ändern.
    -   Preiserhöhungen werden 30 Tage zuvor bekanntgegeben.
    -   Preissenkungen werden am Tag angezeigt, an dem sie wirksam werden.
    -   Vorhandene Abonnements werden zu dem zum Anfang des Abrechnungszyklus gültigen Preis in Rechnung gestellt.
    -   Neue Abonnements (die, die während des Rechnungszyklus erstellt wurden) werden zu dem Preis in Rechnung gestellt, der gültig war, als Sie sie hinzugefügt haben.
-   Wenn Sie ein Abonnement während des ersten Abrechnungszyklus kündigen, erscheinen die Nutzungsgebühren in der Abstimmungsdatei für den Zeitraum, in dem das Abonnement aktiv war.

## <a href="" id="licensebased"></a>Lizenzbasierte Abrechnung

**Abrechnung:** lizenzbasierte Abonnements werden im Voraus zum Dauerauftragsdatum abgerechnet.

**Dauerauftragsdatum:** Abonnements mit monatlichen Abrechnungen stimmen mit dem Abrechnungsdatum des Partners überein und Abonnements mit einer jährlichen Abrechnung stimmen mit dem Kaufdatum überein.

**Kostenloser Zeitraum:** Abonnements mit monatlichen Abrechnungen erhalten eine kostenlose Testphase ab dem Kaufdatum bis zum nächsten Abrechnungsdatum des Partners.

**Laufzeit:** alle lizenzbasierten Abonnements haben einen kostenpflichtigen 12-Monats-Zahlungszeitraum. Der kostenpflichtige Zahlungszeitraum beginnt mit dem Kaufdatum für Abonnements mit einer jährlichen Abrechnung und mit dem Abrechnungsdatum nach dem Kaufdatum für Abonnements mit monatlichen Abrechnungen.

**Stornierung:** Wird das Abonnement in den ersten 30Tagen des kostenpflichtigen Zahlungszeitraums storniert, wird der gesamte Betrag dem Abonnement gutgeschrieben. Wird das Abonnement nach den ersten 30Tagen storniert, wird der anteilige Betrag dem Abonnement gutgeschrieben.

**Verlängerung:** alle lizenzbasierte Abonnements werden automatisch 12Monate nach dem kostenpflichtigen Zahlungszeitraum erneuert.

## <a href="" id="licensebasedmonthly"></a>Monatliche Abrechnungsszenarien

**Szenario 1: Neues Abonnement**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         | 14.01.2018   |Kaufgebühr   |0,00       |1       |0,00    
|15.01.2018         |14.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15.02.2018         |14.03.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    
Sie werden weiterhin am 15.Tag des Monats belastet, bis das Abonnement storniert wird.

**Szenario 2: Die Anzahl der Lizenzen ändern**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |14.01.2018    |Kaufgebühr   |0,00       |1        |0,00    
|15.01.2018         |14.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 1.Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15.01.2018        |14.02.2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |4,00    
|15.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2,21       |1        |2,21    
|1.2.2018         |14.02.2018    | Anteiliger Zyklus für Instanz   |1,82       |2        |3,64    
|15.02.2018         |14.03.2018    | Anteiliger Zyklus für Instanz   |4,00       |2        |8,00    

**Preisformel pro Einheit:**

Die monatliche Gebühr liegt bei 4,00 und es gibt 31Tage im Dienstzeitraum vom 15.1.2018-14.2.2018. Dies entspricht einem täglichen Preis von 0,13 (4 x 31).

Es gibt 17Tage im anteiligen Zeitraum vom 15.01.2018-31.01.2018.

Anteiliger Preis pro Einheit = 2,21 = 17 x 0,13

Es gibt 14Tage im anteiligen Zeitraum vom 01.02.2018-14.02.2018.

Anteiliger Preis pro Einheit = 1,82 = 14 x 0,13

**Szenario 3: Stornieren eines Abonnements innerhalb von 30Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |14.01.2018    |Kaufgebühr   |0,00       |1        |0,00    
|15.01.2018         |14.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    

Am 1.Februar stornieren Sie das Abonnement. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15.01.2018|14.02.2018|Stornierungsgebühr|-4,00|1|4,00

**Szenario 4: Stornieren eines Abonnements nach 30Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|14.01.2018|Kaufgebühr|0,00|1|0,00
15.01.2018|14.02.2018|Gebühr für Zyklus|4,00|1|4,00

Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15.02.2018|14.03.2018|Gebühr für Zyklus|4,00|1|4,00

Am 1.März stornieren Sie das Abonnement. Am 15. März enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|14.03.2018|Stornierungsgebühr|-1,96|1|-1,96

**Preisformel pro Einheit:**

Die monatliche Gebühr liegt bei 4,00 und es gibt 31Tage im Dienstzeitraum vom 15.02.2018-14.03.2018. Dies entspricht einem täglichen Preis von 0,14 (28 x 04).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 14Tage im anteiligen Zeitraum vom 01.03.2018-14.03.2018. 

Der Preis pro Einheit beträgt also =-1,96 (14 x 0,14 x (-1)).

## <a name="annual-billing-scenarios"></a>Jährliche Abrechnung: Szenarien

**Szenario 1: Neues Abonnement**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

**Szenario2: Hinzufügen einer Lizenz nach Abonnementdatum, aber vor Abrechnungsdatum**

Sie erwerben am 11.02.17 ein neues Abonnement mit einer Lizenz für 211,20 USD pro Jahr. Das Abonnementdatum ist der 11. in jedem Monat. Das Microsoft Abrechnungssystem erstellt die folgenden Rechnungspositionen: 

-   211,20USD Gebühr für den Zeitraum vom 11.02.2017 bis zum 10.02.2018. 

Am 12.02.17 erwerben Sie eine zweite Lizenz. Ihr Abrechnungsdatum ist der 14.02.17. Es wird eine Rechnungs- und Abstimmungsdatei generiert. Die Abstimmungsdatei enthält folgende Rechnungspositionen: 
|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteilige Gebühren beim Kauf |211,20 |1 | 211,20 |
 
Zum Abonnementdatum 11.03.17 generiert das Microsoft- Abrechnungssystem die folgenden Abrechnungszeilen für die Lizenzerhöhung am 12.02.17: 
-   211,20USD Gutschrift für den Zeitraum vom 11.02.2017 bis 10.02.2018. 
-   0,58USD anteilige Gebühr pro Lizenz für 1 Lizenz im Zeitraum vom 11.02.2017 bis 11.02.2017. 
-   15,62 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 12.02.2017 bis 10.03.2017. 
-   195,00 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 11.03.2017 bis 10.02.2018. 
 
Am 11.02.2017 kaufen Sie eine Abonnement. An 12.02.17 fügen Sie eine Lizenz hinzu. Ihr Abrechnungsdatum ist der 14.02.17. Am 11.02.18 wird Ihr Abonnement erneuert.

Am nächsten Abrechnungsdatum, dem 14.03.2017, wird eine Rechnung- und Abstimmungsdatei generiert. Die Abstimmungsdatei enthält folgende Rechnungspositionen: 
|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |-211,20 |1 |-211,20 |
|11.02.2017 |11.02.2017 |Anteiliger Zyklus für Instanz |0,58 |1 |0,58 |
|12.02.2017 |10.03.2017 |Anteiliger Zyklus für Instanz |15,62 |2 |31,25 |
|11.03.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |195,00 |2 |390,00 |
 
Am 11.02.2018 wird das Abonnement um weitere 12Monate verlängert.


**Szenario 3: Anzahl der Lizenzen ändern**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1.Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13.01.2018|12.01.2019|Anteiliger Zyklus für Instanz|-48,00|1|-48,00
13.01.2018|31.01.2018|Anteiliger Zyklus für Instanz|2,47|1|2,47
1.2.2018|12.01.2019|Anteiliger Zyklus für Instanz|44,98|2|89,96

**Preisformel pro Einheit:**

Der jährliche Preis ist 48,00, was einem täglichen Preis von 0,13 entspricht (48,00/365).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 19Tage im Service-Zeitraum vom 13.01.2018-31.01.2018. 

Der Preis pro Einheit beträgt also = 2,47 (19 x 0.13 x 1)

Es gibt 346Tage im Service-Zeitraum vom 01.02.2018-12.01.2019. 

Der Preis pro Einheit beträgt also 44,98 (346 x 0,13 x 2)

**Szenario 4: Stornieren eines Abonnements innerhalb von 30Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1.Februar stornieren Sie Ihr Abonnement. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

**Szenario 5: Stornieren eines Abonnements nach 30Tagen**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 15. Februar enthält die lizenzbasierte Erstattungsdatei keine Rechnungspositionen für dieses Abonnement.
Am 1.März stornieren Sie Ihr Abonnement. Am 15. März enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Stornierungsgebühr|-41,34|1|-41,34

**Preisformel pro Einheit:**

Der jährliche Preis ist 48,00, was einem täglichen Preis von 0,13 entspricht (48,00/365).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 318Tage im Service-Zeitraum vom 01.03.2018-12.01.2019. 

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1). Da dies eine Erstattung ist, beträgt der Preis pro Einheit -41,34.

**Szenario 6: Anhalten und neu aktivieren**

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13.Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1.Februar stornieren Sie Ihr Abonnement. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

Am 1.März aktivieren Sie Ihr Abonnement erneut. Am 15. März enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:
|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Anteilige Gebühren beim Kauf|41,34|1|41,34

**Preisformel pro Einheit:**

Der jährliche Preis ist 48,00, was einem täglichen Preis von 0,13 entspricht (48,00/365).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 318Tage im Service-Zeitraum vom 01.03.2018-12.01.2019. 

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1).
