---
title: Berechnung der effektiven Einheiten Preise
ms.topic: how-to
ms.date: 11/10/2020
description: Erfahren Sie mehr über die effektive Preis Einheit und deren Berechnung. Schließt eine Beispiel Berechnung ein.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498567"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Berechnung der effektiven Einheiten Preise für die Nutzung des Azure-Plans

## <a name="the-effective-unit-price"></a>Der effektive Einheitspreis

Der Preis für die effektive Einheit wird auf der Verbrauchseinheit berechnet (im Gegensatz zur Ressourcenebene) und entsprechend der Verbrauchseinheit täglich angepasst.

Wir berechnen den effektiven Einzelpreis mithilfe der folgenden drei Faktoren:

- Verbrauch, der täglich im gesamten Abrechnungszeitraum überwacht wird
- Abrechnungskosten für die Verbrauchseinheit
- Tiering (falls zutreffend)

Da wir die tägliche Nutzung im gesamten Abrechnungszeitraum überwachen, schwankt der effektive Einzelpreis. Der endgültige Preis für einen bestimmten Abrechnungszeitraum ist verfügbar, nachdem die Verbrauchs Berechnung angehalten und der Abrechnungszeitraum geschlossen wurde. Die meisten Änderungen am Verbrauch werden nach dem vierten oder fünften Dezimaltrennzeichen angezeigt.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Erfahren Sie, ob Ihre Verbrauchseinheit mehrstufige Preise verwendet.

Wenn Sie nicht wissen, ob Ihre Verbrauchseinheit mehrstufige Preise verwendet, verwenden Sie das unten beschriebene Verfahren, um sich zu informieren. 

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.
2. Wählen Sie **verkaufen** aus, wählen Sie **Preise und Angebote** aus, und wählen Sie dann **Azure-Plan Preise** aus.
3. Suchen Sie nach ihrer ID, und laden Sie dann Ihre Preisdaten herunter. 

## <a name="sample-calculation"></a>Beispiel Berechnung

In der folgenden Tabelle finden Sie ein Beispiel dafür, wie der effektive Einzelpreis während des Öffnungs Zeitraums berechnet wird.

In der Tabelle gelten die folgenden Werte: 

- **Up** = Einheitspreis der Ressource/Stunde = 0,868

- **BCU** = abrechenbare Verbrauchseinheit für die Verbrauchseinheit

- **BC** = Abrechnungskosten für die Verbrauchseinheit = BCU * up * 0,85. Dies spiegelt eine Anpassung für den 15% PEC-Rabatt wider. Wir verwenden dann den unteren Grenzwert der-Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den minimalen Betrag zu berechnen. 

- **Effektiver Einheitspreis** = BCU/BC

>[!NOTE]
>Hinweis: die Verbrauchseinheit in diesem Beispiel enthält keine Tarife in den Preisen.

| Datum | BCU (abrechenbare Verbrauchseinheit) | BC (Abrechnungskosten) | Effektiver Einheitspreis |
| ------ | ----------- | ----------- | ----------- |  
| 3. Aug | 29 | 21,39 | 0.737586206896552 |
| 10. Aug | 210,950039 | 155,63 | 0.737757626107858 |
| 25. Aug | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Nächste Schritte

- [Abrechnung und Steuern](billing.md)
