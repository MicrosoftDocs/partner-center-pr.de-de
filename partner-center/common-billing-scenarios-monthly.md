---
title: Häufige monatliche Abrechnungs Szenarien | Partner Center
ms.topic: article
ms.date: 11/25/2019
description: Häufige Szenarien in Partner Center, wenn Sie die monatliche Abrechnung verwenden (z. b. das Hinzufügen neuer Abonnements, das Ändern der Lizenz Menge und das Anhalten von Abonnements)
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
Keywords: Abrechnung, Zahlungen, Aufträge, Nutzung, monatliche Abrechnung, Abonnements, Abstimmungs Datei
ms.localizationpriority: medium
ms.openlocfilehash: a9163f7b787d76373a427b9e2d9f09b131227888
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390140"
---
# <a name="monthly-billing-scenarios"></a>Monatliche Abrechnungs Szenarien

**Geeignete Rollen**

- Administratoragent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter

Diese Beispiel [Szenarien gelten für allgemeine Abrechnungs Szenarien](common-billing-scenarios.md) , wenn Sie die monatliche Abrechnung in Partner Center verwenden.

## <a name="new-monthly-subscription"></a>Neues monatliches Abonnement

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00 |

Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13. Februar 2018         |12. März 2018    |Gebühr für Zyklus   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Ändern der Lizenz Anzahl

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    |

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13.01.2018        |12. Februar 2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |-4,00   |
|13.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2.45       |1        |2.45    |
|1\.2.2018         |12. Februar 2018    | Anteiliger Zyklus für Instanz   |1,55       |2        |3.10    |
|13. Februar 2018         |12. März 2018    | Anteiliger Zyklus für Instanz   |4,00       |2        |8,00    |

Die monatliche Gebühr liegt bei 4,00 und es gibt 31 Tage im Dienstzeitraum vom 13.1.2018-12.2.2018. Dies entspricht einem täglichen Preis von 0,129 (4 x 31).

Es gibt 19 Tage im anteiligen Zeitraum vom 13.01.2018-31.01.2018.

Anteiliger Preis pro Einheit = 2,451 = 19 x 0,129

Es gibt 12 Tage im anteiligen Zeitraum vom 1.02.2018-12.02.2018.

Anteiliger Preis pro Einheit = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Vor 30 Tagen aussetzen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    |

Am 1. Februar setzen Sie das Abonnement aus. Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12. Februar 2018|Stornierungsgebühr|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Nach 30 Tagen aussetzen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12. Februar 2018|Gebühr für Zyklus|4,00|1|4,00

Am 15. Februar enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13. Februar 2018|12. März 2018|Gebühr für Zyklus|4,00|1|4,00

Am 1. März stornieren Sie das Abonnement. Am 15. März enthält die lizenzbasierte Erstattungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Menge |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12. März 2018|Stornierungsgebühr|-1.72|1|-1.72

Die monatliche Gebühr liegt bei 4,00 und es gibt 28 Tage im Dienstzeitraum vom 13.2.2018-12.3.2018. Dies entspricht einem täglichen Preis von 0,143 (4 x 28).

Preis pro Einheit = Tage Service-Zeitraum x täglicher Preis x Anzahl der Lizenzen.

Es gibt 12 Tage im anteiligen Zeitraum vom 01.03.2018-12.03.2018.

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).
