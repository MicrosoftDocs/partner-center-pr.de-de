---
title: Common monthly billing scenarios | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common scenarios in Partner Center when you use monthly billing (such as adding new subscriptions, changing license quantity, and suspending subscriptions.)
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, monthly billing, subscriptions, reconciliation file
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389618"
---
# <a name="monthly-billing-scenarios"></a>Monthly billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable if you use monthly billing in Partner Center.

## <a name="new-monthly-subscription"></a>New monthly subscription

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00 |

Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.02.2018         |12.03.2018    |Gebühr für Zyklus   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Change license quantity

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    |

Am 1. Februar erhöhen Sie die Anzahl der Lizenzen von 1 auf 2. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13.01.2018        |12. Februar 2018    |Anteiliger Zyklus für Instanz   |-4,00       |1        |-4,00   |
|13.01.2018         |31.01.2018    | Anteiliger Zyklus für Instanz   |2,45       |1        |2,45    |
|01.02.2018         |12. Februar 2018    | Anteiliger Zyklus für Instanz   |1.55       |2        |3,10    |
|13.02.2018         |12.03.2018    | Anteiliger Zyklus für Instanz   |4,00       |2        |8,00    |

Die monatliche Gebühr liegt bei 4,00, und es gibt 31 Tage im Dienstzeitraum vom 13.01.2018 bis zum 12.02.2018. Dies entspricht einem Preis pro Tag von 0,129 (4/31).

Es gibt 19 Tage im anteiligen Zeitraum vom 13.01.2018 bis zum 31.01.2018.

Anteiliger Preis pro Einheit = 2,451 = 19 x 0,129

Es gibt 12 Tage im anteiligen Zeitraum vom 01.02.2018 bis zum 12.02.2018.

Anteiliger Preis pro Einheit = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspend before 30 days

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD pro Monat und wählen eine monatliche Abrechnung aus. Am 15. Januar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungspositionen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12. Februar 2018    |Gebühr für Zyklus   |4,00       |1        |4,00    |

Am 1. Februar setzen Sie das Abonnement aus. Am 15. Februar enthält die lizenzbasierte Kontenabstimmungsdatei folgende Rechnungsposition:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührenart |Preis pro Einheit |Anzahl |Betrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12. Februar 2018|Stornierungsgebühr|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspend after 30 days

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

Die monatliche Gebühr liegt bei 4,00, und es gibt 28 Tage im Dienstzeitraum vom 13.02.2018 bis zum 12.03.2018. Dies entspricht einem Preis pro Tag von 0,143 (4/28).

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 12 Tage im anteiligen Zeitraum vom 01.03.2018 bis zum 12.03.2018.

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).
