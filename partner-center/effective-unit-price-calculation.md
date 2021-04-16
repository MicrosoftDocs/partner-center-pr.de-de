---
title: Berechnung des effektiven Preises pro Einheit
ms.topic: how-to
ms.date: 04/02/2021
description: Erfahren Sie mehr über den effektiven Einzelpreis und seine Berechnung. Dieser Artikel enthält auch eine Beispielberechnung.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528571"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Effektive Berechnung des Einzelpreis für den Azure-Planverbrauch

## <a name="the-effective-unit-price"></a>Der effektive Einzelpreis

Der effektive Einzelpreis wird auf Verbrauchseinheitsebene (im Gegensatz zur Ressourcenebene) berechnet und täglich entsprechend der Verbrauchseinheitsnutzung angepasst.

Wir berechnen den effektiven Einzelpreis anhand der folgenden drei Faktoren:

- Verbrauch, der während des abrechnungszyklus täglich überwacht wird
- Arechnungsfähige Kosten für die Verbrauchsanzeige
- Tiering (falls zutreffend)

Da der Verbrauch während des abrechnungszyklus täglich überwacht wird, schwankt der effektive Einzelpreis. Der Endpreis für einen bestimmten Abrechnungszyklus ist verfügbar, nachdem wir die Verbrauchsberechnung beenden und den Abrechnungszeitraum geschlossen haben. Nach der vierten oder fünften Dezimalstelle werden die meisten Änderungen im Verbrauch angezeigt.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Finden Sie heraus, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet.

Wenn Sie nicht wissen, ob Ihre Verbrauchsanzeige mehrstufige Preise verwendet, gehen Sie wie folgt vor, um dies herauszufinden. 

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.
2. Wählen **Sie Verkaufen** aus, wählen Sie Preise und **Angebote** aus, und wählen Sie dann Preise **für Azure-Plan aus.**
3. Suchen Sie ihre Verbrauchsanzeige nach ID, und laden Sie dann Ihre Preisdaten herunter. 

## <a name="sample-calculation"></a>Beispielberechnung

Die folgende Tabelle enthält ein Beispiel dafür, wie wir den effektiven Einzelpreis während des offenen Zeitraums berechnen.

In der Tabelle gelten die folgenden Werte: 

- **UP** = Einzelpreis der Ressource/Stunde = 0,868

- **BCU** = Abrechenbare Verbrauchseinheit für die Verbrauchseinheit

- **BC** = Abrechenbare Kosten für die Verbrauchsmessung = BCU * UP * 0,85. Dies spiegelt eine Anpassung des PEC-Rabatts von 15 % wider. Wir verwenden dann die untere Grenze der Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den Mindestbetrag zu berechnen. 

- **Effektiver Einzelpreis** = BCU/BC

>[!NOTE]

>Hinweis: Die Verbrauchseinheit in diesem Beispiel verfügt nicht über Tarife für Preise oder andere Rabatte– die Effektiven Preiseinheitenfaktoren in Rabattprozentsätzen und andere Anpassungen.


| Date | BCU (Abrechenbare Verbrauchseinheit) | BC (Abrechenbare Kosten) | Effektiver Einzelpreis |
| ------ | ----------- | ----------- | ----------- |  
| 3-Aug | 29 | 21.39 | 0.737586206896552 |
| 10-Aug | 210.950039 | 155.63 | 0.737757626107858 |
| 25-Aug | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Steuern](billing.md)
