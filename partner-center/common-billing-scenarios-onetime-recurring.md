---
title: Abrechnung für einmalige & wiederkehrende Käufe
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Partner Center-Abrechnungs Beispiele für einmalige und wiederkehrende Käufe: Wenn Sie Abonnements erwerben, können Sie weitere Abonnements hinzufügen oder Lizenzen hinzufügen oder entfernen.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 329675e10205755819a19710976073d22f73eb58
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502530"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Partner Center-Abrechnungs Szenarien für einmal und Auswahl von wiederkehrenden Käufen

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter

Dabei handelt es sich um [häufige Abrechnungs Szenarien](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Erwerben eines Abonnements und Hinzufügen einer Lizenz am selben Tag

In Szenario 1 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Später am gleichen Tag erwerben ein weiteres gleiches Abonnement zum gleichen Preis.

Die Kontenabstimmungsdatei enthält Folgendes:

- 4 USD Gebühr für den Leistungszeitraum 10. Juni bis 9. Juli.
- -4,00 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 11. Juni. Dies ist der Zeitraum, in dem Sie über eine Lizenz verfügen. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 1 = 4,00.
- 8,00 USD anteilige Weiterbelastung für den Leistungszeitraum 10. Juni bis 9. Juli. Dies ist der Zeitraum, in dem Sie über zwei Lizenzen verfügen. Berechnung: (4/30) x 30 x 2 = 8,00.

|**Kauf Datum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Unit price**  |**Menge**  |**Amount (Betrag)** |**Gebührentyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 US-Dollar                |1                 |4 US-Dollar            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        |1        | -4 USD       |addQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        | 2      |-8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Erwerben eines Abonnements und Hinzufügen von weiteren Abonnements später

In Szenario 2 erwerben Sie am 11. Juni ein Abonnement mit einem Preis pro Einheit von 4 USD. Am 12. Juni erwerben Sie ein weiteres Abonnement für das gleiche Produkt zum gleichen Preis.

Die Kontenabstimmungsdatei enthält Folgendes:

- 4 USD Gebühr für den Leistungszeitraum 10. Juni bis 9. Juli.
- -3,87 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 12. Juni. Dies ist der Zeitraum, in dem Sie über eine Lizenz verfügen. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 1 = 3,87.
- 7,74 USD anteilige Weiterbelastung für den Leistungszeitraum 12. Juni bis 9. Juli. Dies ist der Zeitraum, in dem Sie über zwei Lizenzen verfügen. Berechnung = (4/30) x 29 x 2 = 7,74.

|**Kauf Datum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Unit price**  |**Menge**  |**Amount (Betrag)** |**Gebührentyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019 (Sie verfügen über eine Lizenz)     |10.06.2019   |09.07.2019         |4 US-Dollar         |1        |4 US-Dollar            |Neu         |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        |1        | -3,87 USD       |addQuantity           |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Erwerben eines Abonnements und Entfernen einer Lizenz am selben Tag

In Szenario 3 erwerben Sie zwei Abonnements für das gleiche Produkt am 11. Juni mit einem Preis pro Einheit von 4 USD. Zu einem späteren Zeitpunkt entfernen Sie eine der Lizenzen.  

Die Kontenabstimmungsdatei enthält Folgendes:

- 8 USD Gebühr für zwei Lizenzen für den Leistungszeitraum 10. Juni bis 9. Juli.
- -8,00 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 11. Juni. Dies ist der Zeitraum, in dem Sie über zwei Lizenzen verfügen. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 30 x 2 = 8,00.
- 4,00 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 9. Juli. Dies ist der Zeitraum, in dem Sie über eine Lizenz verfügen. Berechnung = (4/30) x 30 x 1 = 4,00.

|**Kauf Datum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Unit price**  |**Menge**  |**Amount (Betrag)** |**Gebührentyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11.06.2019      |10.06.2019   |09.07.2019         |4 US-Dollar                |2                 |-8 USD            |Neu         |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        |2        | \- 8 US-Dollar       |removeQuantity           |
|11.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        | 1      |4 US-Dollar         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Erwerben eines Abonnements und Entfernen von Lizenzen später

In Szenario 4 erwerben Sie zwei Abonnements am 11. Juni mit einem unitpreis von $4. am 12. Juni entfernen Sie eine der Lizenzen.

Die Kontenabstimmungsdatei enthält Folgendes:

- 8 USD Gebühr für den Leistungszeitraum 10. Juni bis 9. Juli.
- -7.74 USD anteilige Weiterbelastung für den Leistungszeitraum 11. Juni bis 12. Juni. Dies ist der Zeitraum, in dem Sie über zwei Lizenzen verfügen. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (4/30) x 29 x 2 = 7,74.
- 3,87 USD anteilige Weiterbelastung für den Leistungszeitraum 12. Juni bis 9. Juli. Dies ist der Zeitraum, in dem Sie über eine Lizenz verfügen. Berechnung = (4/30) x 29 x 1 = 3,87.

|**Kauf Datum**   |**Beginn der Abrechnung** |**Ende der Abrechnung**  |**Unit price**  |**Menge**  |**Amount (Betrag)** |**Gebührentyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (Sie haben zwei Lizenzen)     |10.06.2019   |09.07.2019         |4 US-Dollar         |2        |-8 USD       |Neu       |
|12.06.2019     | 10.06.2019    |09.07.2019        |4 US-Dollar        |2        | -7,74 USD       |removeQuantity           |
|6/12/2019 (Sie verfügen über eine Lizenz)    | 10.06.2019    |09.07.2019   |4 US-Dollar    |1      |3,87 USD    |removeQuantity |

## <a name="next-steps"></a>Nächste Schritte

- [Stichproben von monatlichen Abrechnungs Szenarien für neue Abonnements, Ändern von Lizenz Beträgen oder Suspendierungen](common-billing-scenarios-monthly.md)