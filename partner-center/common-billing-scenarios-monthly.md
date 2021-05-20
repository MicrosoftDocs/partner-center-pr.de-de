---
title: Allgemeine monatliche Abrechnungsszenarien
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Häufige Szenarien in Partner Center, wenn Sie die monatliche Abrechnung verwenden, z. B. das Hinzufügen neuer Abonnements, das Ändern der Lizenzmenge und das Anhalten von Abonnements.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148651"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Beispiele für monatliche Abrechnungsszenarien für neue Abonnements, Ändern von Lizenzbeträgen oder Unterbrechungen

**Geeignete Rollen:** Administrator-Agent-| Abrechnungsadministrator-| | des Helpdesk-Agents Vertriebsmitarbeiter

Diese [gängigen Beispielabrechnungsszenarien](common-billing-scenarios.md) sind anwendbar, wenn Sie die monatliche Abrechnung in Partner Center verwenden.

## <a name="new-monthly-subscription"></a>Neues monatliches Abonnement

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD/Monat und wählen die monatliche Abrechnung aus. Die lizenzbasierte Abstimmungsdatei vom 15. Januar enthält die folgenden Abrechnungszeilen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4.00       |1        |4.00 |

Die lizenzbasierte Abstimmungsdatei vom 15. Februar enthält die folgende Abrechnungszeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.02.2018         |12.03.2018    |Gebühr für Zyklus   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Lizenzanzahl ändern

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD/Monat und wählen die monatliche Abrechnung aus. Die lizenzbasierte Abstimmungsdatei vom 15. Januar enthält die folgenden Abrechnungszeilen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4.00       |1        |4.00    |

Am 1. Februar erhöhen Sie Ihre Lizenzmenge von eins auf zwei. Die lizenzbasierte Abstimmungsdatei vom 15. Februar enthält die folgenden Abrechnungszeilen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
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

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD/Monat und wählen die monatliche Abrechnung aus. Die lizenzbasierte Abstimmungsdatei vom 15. Januar enthält die folgenden Abrechnungszeilen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13.01.2018         |12.02.2018    |Gebühr für Zyklus   |4.00       |1        |4.00    |

Am 1. Februar setzen Sie ein Abonnement aus. Die lizenzbasierte Abstimmungsdatei vom 15. Februar enthält die folgende Abrechnungszeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Stornierungsgebühr|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Aussetzen eines Abonnements nach 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für 4 USD/Monat und wählen die monatliche Abrechnung aus. Die lizenzbasierte Abstimmungsdatei vom 15. Januar enthält die folgenden Abrechnungszeilen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.02.2018|Gebühr für Zyklus|4.00|1|4.00

Die lizenzbasierte Abstimmungsdatei vom 15. Februar enthält die folgende Abrechnungszeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.02.2018|12.03.2018|Gebühr für Zyklus|4.00|1|4.00

Am 1. März wird das Abonnement ausgesetzt. Die lizenzbasierte Abstimmungsdatei vom 15. März enthält die folgende Abrechnungszeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.03.2018|Stornierungsgebühr|-1,72|1|-1,72

Die monatliche Gebühr liegt bei 4,00, und es gibt 28 Tage im Dienstzeitraum vom 13.02.2018 bis zum 12.03.2018. Dies entspricht einem Preis pro Tag von 0,143 (4/28).

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 12 Tage im anteiligen Zeitraum vom 01.03.2018 bis zum 12.03.2018.

Deshalb beträgt der Preis pro Einheit = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnungsszenarien für einmalige und ausgewählte wiederkehrende Käufe](common-billing-scenarios-onetime-recurring.md)