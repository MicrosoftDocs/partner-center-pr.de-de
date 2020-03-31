---
title: Allgemeine Abrechnungsszenarien | Partner Center
ms.topic: article
ms.date: 11/25/2019
description: 'Weitere Informationen finden Sie in der jährlichen Abrechnung für Partner Center: Wenn Sie neue Abonnements hinzufügen, Lizenzen vor dem Abrechnungsdatum hinzufügen, die Lizenz Menge ändern, Abonnements aussetzen/reaktivieren.'
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
Keywords: Abrechnung, Zahlungen, Bestellungen, Nutzung, lizenzbasierte Abrechnung, Abonnementdatum, Laufzeit, Kündigung, Verlängerung, Kontenabstimmungsdatei, Abstimmungsdatei
ms.localizationpriority: medium
ms.openlocfilehash: fdfb242f51556ce924d06d7a35f32cf726803fe3
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390159"
---
# <a name="annual-billing-scenarios"></a>Jährliche Abrechnungs Szenarien

**Geeignete Rollen**

- Administratoragent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter

Diese Beispiel [Szenarien gelten für allgemeine Abrechnungs Szenarien](common-billing-scenarios.md) , wenn Sie die jährliche Abrechnung in Partner Center verwenden.

## <a name="new-annual-subscription"></a>Neues Jahresabonnement

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Lizenz nach Abonnement Jahrestag, aber vor Abrechnungsdatum hinzufügen

Sie erwerben am 11.02.17 ein neues Abonnement mit einer Lizenz für 211,20 USD pro Jahr. Das Abonnementdatum ist der 11. in jedem Monat. Das Microsoft Abrechnungssystem erstellt die folgenden Rechnungspositionen:

- 211,20 USD Gebühr für den Zeitraum vom 11.02.2017 bis zum 10.02.2018.

Am 12.02.17 erwerben Sie eine zweite Lizenz. Ihr Abrechnungsdatum ist der 14.02.17. Es wird eine Rechnungs- und Abstimmungsdatei generiert. Die Abstimmungsdatei enthält folgende Rechnungspositionen:

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Menge | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteilige Gebühren beim Kauf |211,20 |1 | 211,20 |

Zum Abonnementdatum 11.03.17 generiert das Microsoft- Abrechnungssystem die folgenden Abrechnungszeilen für die Lizenzerhöhung am 12.02.17:

- $211,20-Gutschrift für den Zeitraum 2/11/17 – 2/10/18.
- 0,58 USD anteilige Gebühr pro Lizenz für 1 Lizenz im Zeitraum vom 11.02.2017 bis 11.02.2017.
- 15,62 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 12.02.2017 bis 10.03.2017.
- 195,00 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 11.03.2017 bis 10.02.2018.

Am 11.02.2017 kaufen Sie eine Abonnement. An 12.02.17 fügen Sie eine Lizenz hinzu. Ihr Abrechnungsdatum ist der 14.02.17. Am 11.02.18 wird Ihr Abonnement erneuert.

Am nächsten Abrechnungsdatum, dem 14.03.2017, wird eine Rechnung- und Abstimmungsdatei generiert. Die Abstimmungsdatei enthält folgende Rechnungspositionen:

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Menge | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |-211,20 |1 |-211,20 |
|11.02.2017 |11.02.2017 |Anteiliger Zyklus für Instanz |0,58 |1 |0,58 |
|12.02.2017 |10.03.2017 |Anteiliger Zyklus für Instanz |15,62 |2 |31,25 |
|11.03.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |195,00 |2 |390,00 |

Am 11.02.2018 wird das Abonnement um weitere 12 Monate verlängert.

## <a name="change-license-quantity"></a>Ändern der Lizenz Anzahl

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteiliger Zyklus für Instanz|-48,00|1|-48,00
13.01.2018|31.01.2018|Anteiliger Zyklus für Instanz|2,47|1|2,47
1\.2.2018|12.01.2019|Anteiliger Zyklus für Instanz|44,98|2|89,96

Der jährliche Preis ist 48,00, was einem täglichen Preis von 0,13 entspricht (48,00/365).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 19 Tage im Service-Zeitraum vom 13.01.2018-31.01.2018.

Der Preis pro Einheit beträgt also = 2,47 (19 x 0.13 x 1)

Es gibt 346 Tage im Service-Zeitraum vom 01.02.2018-12.01.2019.

Der Preis pro Einheit beträgt also 44,98 (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Vor 30 Tagen aussetzen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar stornieren Sie Ihr Abonnement. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Nach 30 Tagen aussetzen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 15. Februar enthält die lizenzbasierte Erstattungsdatei keine Rechnungspositionen für dieses Abonnement.
Am 1. März stornieren Sie Ihr Abonnement. Am 15. März enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Stornierungsgebühr|-41,34|1|-41,34

Der jährliche Preis ist 48,00, was einem täglichen Preis von 0,13 entspricht (48,00/365).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 318 Tage im Service-Zeitraum vom 01.03.2018-12.01.2019.

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1). Da dies eine Erstattung ist, beträgt der Preis pro Einheit -41,34.

## <a name="suspend-and-reactivate"></a>Aussetzen und reaktivieren

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar stornieren Sie Ihr Abonnement. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

Am 1. März aktivieren Sie Ihr Abonnement erneut. Am 15. März enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Anteilige Gebühren beim Kauf|41,34|1|41,34

Der jährliche Preis ist 48,00, was einem täglichen Preis von 0,13 entspricht (48,00/365).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 318 Tage im Service-Zeitraum vom 01.03.2018-12.01.2019.

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1).
