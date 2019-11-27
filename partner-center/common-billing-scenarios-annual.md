---
title: Allgemeine Abrechnungsszenarien | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Häufige Abrechnungs Szenarien im Partner Center für die jährliche Abrechnung (z. b. das Hinzufügen neuer Abonnements, das Hinzufügen von Lizenzen vor dem Abrechnungsdatum, das Ändern der Lizenz Menge und das Anhalten und erneute Aktivieren von Abonnements).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: Abrechnung, Zahlungen, Bestellungen, Nutzung, lizenzbasierte Abrechnung, Abonnementdatum, Laufzeit, Kündigung, Verlängerung, Kontenabstimmungsdatei, Abstimmungsdatei
ms.localizationpriority: medium
ms.openlocfilehash: 91b8e318e2122f9510b160339984cc0743c318ee
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389628"
---
# <a name="annual-billing-scenarios"></a>Jährliche Abrechnungs Szenarien

Diese Beispiel [Szenarien gelten für allgemeine Abrechnungs Szenarien](common-billing-scenarios.md) , wenn Sie die jährliche Abrechnung in Partner Center verwenden.

## <a name="new-annual-subscription"></a>Neues Jahresabonnement

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Lizenz nach Abonnement Jahrestag, aber vor Abrechnungsdatum hinzufügen

Sie erwerben am 11.02.2017 ein neues Abonnement mit einer Lizenz für 211,20 USD pro Jahr. Das Abonnementdatum ist der 11. in jedem Monat. Das Microsoft-Abrechnungssystem erstellt folgende Rechnungspositionen:

- 211,20 USD Gebühr für den Zeitraum vom 11.02.2017 bis zum 10.02.2018.

Am 12.02.2017 erwerben Sie eine zweite Lizenz. Ihr Abrechnungsdatum ist der 14.02.2017. Es werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen:

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteilige Gebühren beim Kauf |211,20 |1 | 211,20 |

Zum Abonnementdatum 11.03.2017 generiert das Microsoft-Abrechnungssystem die folgenden Rechnungspositionen für die Lizenzerhöhung am 12.02.2017:

- $211,20-Gutschrift für den Zeitraum 2/11/17 – 2/10/18.
- 0,58 USD anteilige Gebühr pro Lizenz für 1 Lizenz im Zeitraum vom 11.02.2017 bis zum 11.02.2017.
- 15,62 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 12.02.2017 bis 10.03.2017.
- 195,00 USD anteilige Gebühr pro Lizenz für 2 Lizenzen im Zeitraum vom 11.03.2017 bis zum 10.02.2018.

Am 11.02.2017 erwerben Sie ein Abonnement. Am 12.02.2017 fügen Sie eine Lizenz hinzu. Ihr Abrechnungsdatum ist der 14.02.2017. Am 11.02.2018 wird Ihr Abonnement verlängert.

Am nächsten Abrechnungsdatum, dem 14.03.2017, werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen:

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührenart  |Preis pro Einheit |Anzahl | Betrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |-211,20 |1 |-211,20 |
|11.02.2017 |11.02.2017 |Anteiliger Zyklus für Instanz |0,58 |1 |0,58 |
|12.02.2017 |10.03.2017 |Anteiliger Zyklus für Instanz |15,62 |2 |31,25 |
|11.03.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |195,00 |2 |390,00 |

Am 11.02.2018 wird das Abonnement um weitere 12 Monate verlängert.

## <a name="change-license-quantity"></a>Ändern der Lizenz Anzahl

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

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 19 Tage im Dienstzeitraum vom 13.01.2018 – 31.01.2018.

Der Preis pro Einheit beträgt also = 2,47 (19 x 0,13 x 1)

Es gibt 346 Tage im Dienstzeitraum vom 01.02.2018 – 12.01.2019.

Der Preis pro Einheit beträgt also 44,98 (346 x 0,13 x 2).

## <a name="suspend-before-30-days"></a>Vor 30 Tagen aussetzen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar setzen Sie Ihr Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Nach 30 Tagen aussetzen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine jährliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei keine Rechnungspositionen für dieses Abonnement.
Am 1. März setzen Sie Ihr Abonnement aus. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Stornierungsgebühr|-41,34|1|-41,34

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 318 Tage im Dienstzeitraum vom 01.03.2018 bis zum 12.01.2019.

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1). Da dies eine Gutschrift ist, beträgt der Preis pro Einheit -41,34.

## <a name="suspend-and-reactivate"></a>Aussetzen und reaktivieren

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

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 318 Tage im Dienstzeitraum vom 01.03.2018 bis zum 12.01.2019.

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1).
