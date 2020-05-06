---
title: Häufige monatliche Abrechnungs Szenarien | Partner Center
ms.topic: article
ms.date: 11/25/2019
description: Häufige Szenarien in Partner Center, wenn Sie die monatliche Abrechnung verwenden (z. b. das Hinzufügen neuer Abonnements, das Ändern der Lizenz Menge und das Anhalten von Abonnements)
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: Abrechnung, Zahlungen, Aufträge, Nutzung, monatliche Abrechnung, Abonnements, Abstimmungs Datei
ms.localizationpriority: medium
ms.openlocfilehash: e67281a0bf7d5649a68a6a3f3c27c40e3666eb14
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798538"
---
# <a name="monthly-billing-scenarios"></a>Monatliche Abrechnungsszenarien

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter

Diese Beispiel [Szenarien gelten für allgemeine Abrechnungs Szenarien](common-billing-scenarios.md) , wenn Sie die monatliche Abrechnung in Partner Center verwenden.

## <a name="new-monthly-subscription"></a>Neues monatliches Abonnement

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4.00       |1        |4.00 |

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.02.2018         |12.03.2018    |Gebühr für Zyklus   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Anzahl an Lizenzen ändern

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4.00       |1        |4.00    |

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13.01.2018        |12.02.2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |-4,00   |
|13.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2.45       |1        |2.45    |
|2/1/2018         |12.02.2018    | Anteiliger Zyklus für Instanz   |1,55       |2        |3.10    |
|13.02.2018         |12.03.2018    | Anteiliger Zyklus für Instanz   |4.00       |2        |8.00    |

Die monatliche Gebühr liegt bei 4,00, und es gibt 31 Tage im Dienstzeitraum vom 13.01.2018 bis zum 12.02.2018. Dies entspricht einem Preis pro Tag von 0,129 (4/31).

Es gibt 19 Tage im anteiligen Zeitraum vom 13.01.2018 bis zum 31.01.2018.

Anteiliger Preis pro Einheit = 2,451 = 19 x 0,129

Es gibt 12 Tage im anteiligen Zeitraum vom 01.02.2018 bis zum 12.02.2018.

Anteiliger Preis pro Einheit = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Aussetzen eines Abonnements innerhalb von 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4.00       |1        |4.00    |

Am 1. Februar setzen Sie das Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Stornierungsgebühr|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Aussetzen eines Abonnements nach 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Gebühr für Zyklus|4.00|1|4.00

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.02.2018|12.03.2018|Gebühr für Zyklus|4.00|1|4.00

Am 1. März setzen Sie das Abonnement aus. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.03.2018|Stornierungsgebühr|-1,72|1|-1,72

Die monatliche Gebühr liegt bei 4,00, und es gibt 28 Tage im Dienstzeitraum vom 13.02.2018 bis zum 12.03.2018. Dies entspricht einem Preis pro Tag von 0,143 (4/28).

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 12 Tage im anteiligen Zeitraum vom 01.03.2018 bis zum 12.03.2018.

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).
