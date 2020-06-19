---
title: Häufige monatliche Abrechnungs Szenarien
ms.topic: article
ms.date: 05/13/2020
description: 'Häufige Szenarien in Partner Center bei der monatlichen Abrechnung: umfasst das Hinzufügen neuer Abonnements, das Ändern der Lizenz Menge und das Anhalten von Abonnements.'
author: LauraBrenner
ms.author: labrenne
Keywords: Abrechnung, Zahlungen, Aufträge, Nutzung, monatliche Abrechnung, Abonnements, Abstimmungs Datei
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9da060e1c8b0a9d2f0a5de0987ccb4ea1e167b7c
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2020
ms.locfileid: "84908878"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Stichproben von monatlichen Abrechnungs Szenarien für neue Abonnements, Ändern von Lizenz Beträgen oder Suspendierungen

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
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00 |

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.02.2018         |12.03.2018    |Gebühr für Zyklus   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Anzahl an Lizenzen ändern

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    |

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13.01.2018        |12.02.2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |-4,00   |
|13.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2.45       |1        |2.45    |
|2/1/2018         |12.02.2018    | Anteiliger Zyklus für Instanz   |1,55       |2        |3.10    |
|13.02.2018         |12.03.2018    | Anteiliger Zyklus für Instanz   |4,00       |2        |8.00    |

Die monatliche Gebühr liegt bei 4,00, und es gibt 31 Tage im Dienstzeitraum vom 13.01.2018 bis zum 12.02.2018. Dies entspricht einem Preis pro Tag von 0,129 (4/31).

Es gibt 19 Tage im anteiligen Zeitraum vom 13.01.2018 bis zum 31.01.2018.

Anteiliger Preis pro Einheit = 2,451 = 19 x 0,129

Es gibt 12 Tage im anteiligen Zeitraum vom 01.02.2018 bis zum 12.02.2018.

Anteiliger Preis pro Einheit = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Aussetzen eines Abonnements innerhalb von 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4,00       |1        |4,00    |

Am 1. Februar setzen Sie das Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Stornierungsgebühr|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Aussetzen eines Abonnements nach 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Gebühr für Zyklus|4,00|1|4,00

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.02.2018|12.03.2018|Gebühr für Zyklus|4,00|1|4,00

Am 1. März setzen Sie das Abonnement aus. Am 15. März enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.03.2018|Stornierungsgebühr|-1,72|1|-1,72

Die monatliche Gebühr liegt bei 4,00, und es gibt 28 Tage im Dienstzeitraum vom 13.02.2018 bis zum 12.03.2018. Dies entspricht einem Preis pro Tag von 0,143 (4/28).

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 12 Tage im anteiligen Zeitraum vom 01.03.2018 bis zum 12.03.2018.

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).
