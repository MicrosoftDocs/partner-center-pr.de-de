---
title: Common billing scenarios for one-time and select recurring purchases | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common billing scenarios in Partner Center for one-time and select recurring purchases (such as purchasing subscriptions, adding more subscriptions, adding and removing seats).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, one-time purchase, recurring purchase, subscriptions, seats
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389638"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>One-time and select recurring purchase billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable to [one-time and select recurring charges](one-time-and-recurring-billing.md) in Partner Center.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Purchase a subscription and add a seat on the same day

In Szenario 1 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag erwerben ein weiteres gleiches Abonnement zum gleichen Preis.

Die Kontenabstimmungsdatei enthält Folgendes:

- 4 USD Gebühr für den Leistungszeitraum 10. Juni bis 9. Juli.
- -4,00 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 11. Juni. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 1 = 4,00.
- 8,00 USD anteilige Weiterbelastung für den Leistungszeitraum 10. Juni bis 9. Juli. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (4/30) x 30 x 2 = 8,00.

|**Kaufdatum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 USD                |1                 |4 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 2      |-8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Purchase a subscription and add more subscriptions later

In Szenario 2 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Am 12. Juni erwerben Sie ein weiteres Abonnement für das gleiche Produkt zum gleichen Preis.

Die Kontenabstimmungsdatei enthält Folgendes:

- 4 USD Gebühr für den Leistungszeitraum 10. Juni bis 9. Juli.
- -3,87 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 12. Juni. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 1 = 3,87.
- 7,74 USD anteilige Weiterbelastung für den Leistungszeitraum 12. Juni bis 9. Juli. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung = (4/30) x 29 x 2 = 7,74.

|**Kaufdatum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie verfügen über eine Lizenz)     |10.06.2019   |09.07.2019         |4 USD         |1        |4 USD            |Neu         |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Purchase a subscription and remove a seat on the same day

In Szenario 3 erwerben Sie zwei Abonnements für das gleiche Produkt am 11. Juni mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag entfernen Sie einen der Arbeitsplätze.  

Die Kontenabstimmungsdatei enthält Folgendes:

- 8 USD Gebühr für zwei Lizenzen für den Leistungszeitraum 10. Juni bis 9. Juli.
- -8,00 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 11. Juni. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 2 = 8,00.
- 4,00 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 9. Juli. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung = (4/30) x 30 x 1 = 4,00.

|**Kaufdatum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 USD                |2                 |-8 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 USD        | 1      |4 USD         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Purchase a subscription and remove seats later

In Szenario 4 erwerben Sie am 11. Juni 2 Abonnements mit einem Preis pro Einheit von 4 USD. Am 12. Juni entfernen Sie einen der Arbeitsplätze.

Die Kontenabstimmungsdatei enthält Folgendes:

- 8 USD Gebühr für den Leistungszeitraum 10. Juni bis 9. Juli.
- -7.74 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 12. Juni. Dies ist der Zeitraum, in Sie zwei Lizenzen besessen haben. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 2 = 7,74.
- 3,87 USD anteilige Weiterbelastung für den Leistungszeitraum 12. Juni bis 9. Juli. Dies ist der Zeitraum, in Sie eine Lizenz besessen haben. Berechnung = (4/30) x 29 x 1 = 3,87.

|**Kaufdatum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Preis pro Einheit**  |**Anzahl**  |**Betrag** |**Gebührenart** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie haben 2 Lizenzen)     |10.06.2019   |09.07.2019         |4 USD         |2        |-8 USD       |Neu       |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12.06.2019 (Sie haben 1 Lizenz)    | 10.06.2019    |09.07.2019   |4 USD    |1      |3,87 USD    |removeQuantity |
