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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172216"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Effektive Berechnung des Einzelpreises für die Nutzung des Azure-Plans

**Geeignete Rollen**

- Abrechnungsadministrator

## <a name="the-effective-unit-price"></a>Der effektive Einzelpreis

Der effektive Einzelpreis wird auf Verbrauchseinheitsebene (im Gegensatz zur Ressourcenebene) berechnet und täglich entsprechend der Verbrauchseinheit angepasst.

Wir berechnen den effektiven Einzelpreis anhand der folgenden drei Faktoren:

- Verbrauch, der während des gesamten Abrechnungszyklus täglich überwacht wird
- Abrechenbare Kosten für die Verbrauchsmessung
- Tiering (falls zutreffend)

Da der Verbrauch während des gesamten Abrechnungszyklus täglich überwacht wird, schwankt der effektive Einzelpreis. Der Endpreis für einen bestimmten Abrechnungszyklus ist verfügbar, nachdem wir die Verbrauchsberechnung beendet und den Abrechnungszeitraum geschlossen haben. Nach der vierten oder fünften Dezimalstelle werden die meisten Verbrauchsänderungen angezeigt.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ermitteln, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet

Wenn Sie nicht wissen, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet, verwenden Sie das folgende Verfahren, um dies zu ermitteln. 

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.
2. Wählen Sie **Verkaufen** aus, wählen Sie **Preise und Angebote** aus, und wählen Sie dann Preise für den **Azure-Plan** aus.
3. Suchen Sie Ihre Verbrauchsnummer nach ID, und laden Sie dann Ihre Preisdaten herunter. 

## <a name="sample-calculation"></a>Beispielberechnung

Die folgende Tabelle enthält ein Beispiel dafür, wie wir den effektiven Einzelpreis während des Öffnungszeitraums berechnen.

In der Tabelle gelten die folgenden Werte: 

- **UP** = Einzelpreis der Ressource/Stunde = 0,868

- **BCU** = Arechnungsfähige Verbrauchseinheit für die Verbrauchseinheit

- **BC** = Arechnungsfähige Kosten für die Verbrauchsanzeige = BCU * UP * 0,85. Dies spiegelt eine Anpassung des PEC-Rabatts von 15 % wider. Wir verwenden dann die Untergrenze der Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den Mindestbetrag in Rechnung zu stellen. 

- **Effektiver Einzelpreis** = BCU/BC

>[!NOTE]

>Hinweis: Die Verbrauchseinheit in diesem Beispiel verfügt nicht über Tarife für Preise oder andere Rabatte– die Effektiven Einzelpreisfaktoren in Rabattprozentsätzen und andere Anpassungen.


| Date | BCU (Arechnungsfähige Verbrauchseinheit) | BC (agerechnete Kosten) | Effektiver Einzelpreis |
| ------ | ----------- | ----------- | ----------- |  
| 3:00 Uhr | 29 | 21.39 | 0.737586206896552 |
| 10:00 Uhr | 210.950039 | 155.63 | 0.737757626107858 |
| 25:00 Uhr | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Steuern](billing.md)
