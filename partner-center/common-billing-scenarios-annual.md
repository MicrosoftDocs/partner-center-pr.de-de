---
title: 'Jährliche Abrechnung: Häufige Szenarien'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Jährliche Abrechnung von Partner Center: Wenn Sie neue Abonnements hinzufügen, Lizenzen vor dem Abrechnungsdatum hinzufügen, die Lizenz Menge ändern oder Abonnements aussetzen/reaktivieren.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7494fd7cc003d1179c0ed959b21e1be2cbcc3255
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502479"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Häufige jährliche Abrechnungs Szenarien im Partner Center

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter

Diese Beispiel [Szenarien gelten für allgemeine Abrechnungs Szenarien](common-billing-scenarios.md) , wenn Sie die jährliche Abrechnung in Partner Center verwenden.

## <a name="new-annual-subscription"></a>Neues Jahresabonnement

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für "$ 4/Monat" und wählen die jährliche Abrechnung aus. Die Lizenz basierte ababstimmungs Datei für den 15. Januar enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Hinzufügen einer Lizenz nach dem Abonnementdatum, aber vor dem Abrechnungsdatum

Sie erwerben am 11.02.2017 ein neues Abonnement mit einer Lizenz für 211,20 USD pro Jahr. Das Abonnementdatum ist der 11. in jedem Monat. Das Microsoft-Abrechnungssystem erstellt folgende Rechnungspositionen:

- 211,20 USD Gebühr für den Zeitraum vom 11.02.2017 bis zum 10.02.2018.

Auf 2/12/17 können Sie eine zweite Lizenz erwerben. Ihr Abrechnungsdatum ist der 14.02.2017. Es werden eine Rechnung und eine Kontenabstimmungsdatei generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen:

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührentyp  |Unit Price |Menge | Amount (Betrag) |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteilige Gebühren beim Kauf |211,20 |1 | 211,20 |

Zum Abonnementdatum 11.03.2017 generiert das Microsoft-Abrechnungssystem die folgenden Rechnungspositionen für die Lizenzerhöhung am 12.02.2017:

- $211,20-Gutschrift für den Zeitraum 2/11/17 – 2/10/18.
- $0,58 anteilsmäßig abgerechnet pro Lizenz für eine Lizenz für den Zeitraum 2/11/17 – 2/11/17.
- $15,62 anteilsmäßig abgerechnet pro Lizenz für zwei Lizenzen für den Zeitraum 2/12/17 – 3/10/2017.
- $195,00 anteilsmäßig abgerechnet pro Lizenz für zwei Lizenzen für den Zeitraum 3/11/2017 – 2/10/2018.

Auf 2/11/17 erwerben Sie ein Abonnement. Auf 2/12/17 können Sie eine Lizenz hinzufügen. Ihr Abrechnungsdatum ist der 14.02.2017. Am 11.02.2018 wird Ihr Abonnement verlängert.

Das nächste Abrechnungsdatum ist 3/14/17, und eine Rechnungs-und Abstimmungs Datei wird generiert. Die Kontenabstimmungsdatei enthält folgende Rechnungspositionen:

|Startdatum der Abrechnung  |Enddatum der Abrechnung  |Gebührentyp  |Unit Price |Menge | Amount (Betrag) |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11.02.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |-211,20 |1 |-211,20 |
|11.02.2017 |11.02.2017 |Anteiliger Zyklus für Instanz |0,58 |1 |0,58 |
|12.02.2017 |10.03.2017 |Anteiliger Zyklus für Instanz |15,62 |2 |31,25 |
|11.03.2017 |10.02.2018 |Anteiliger Zyklus für Instanz |195,00 |2 |390,00 |

Am 11.02.2018 wird das Abonnement um weitere 12 Monate verlängert.

## <a name="change-license-quantity"></a>Lizenzanzahl ändern

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für "$ 4/Monat" und wählen die jährliche Abrechnung aus. Die Lizenz basierte ababstimmungs Datei für den 15. Januar enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar erhöhen Sie Ihre Lizenz Menge von einem auf zwei. Die Lizenz basierte ababstimmungs Datei für den 15. Februar enthält die folgenden Abrechnungs Zeilen:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteiliger Zyklus für Instanz|-48,00|1|-48,00
13.01.2018|31.01.2018|Anteiliger Zyklus für Instanz|2.47|1|2.47
2/1/2018|12.01.2019|Anteiliger Zyklus für Instanz|44,98|2|89,96

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 19 Tage im Dienstzeitraum vom 13.01.2018 – 31.01.2018.

Der Preis pro Einheit beträgt also = 2,47 (19 x 0,13 x 1)

Es gibt 346 Tage im Dienstzeitraum vom 01.02.2018 – 12.01.2019.

Der Preis pro Einheit beträgt also 44,98 (346 x 0,13 x 2).

## <a name="suspend-before-30-days"></a>Aussetzen eines Abonnements innerhalb von 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für "$ 4/Monat" und wählen die jährliche Abrechnung aus. Die Lizenz basierte ababstimmungs Datei für den 15. Januar enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar brechen Sie Ihr Abonnement ab. Die Lizenz basierte ababstimmungs Datei von Februar 15 enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Aussetzen eines Abonnements nach 30 Tagen

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für "$ 4/Monat" und wählen die jährliche Abrechnung aus. Die Lizenz basierte ababstimmungs Datei für den 15. Januar enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Die Lizenz basierte ababstimmungs Datei für den 15. Februar enthält keine Abrechnungs Zeilen für dieses Abonnement.
Am 1. März brechen Sie Ihr Abonnement ab. Die Lizenz basierte ababstimmungs Datei vom März 15 enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Stornierungsgebühr|-41,34|1|-41,34

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 318 Tage im Dienstzeitraum vom 01.03.2018 bis zum 12.01.2019.

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1). Da dies eine Gutschrift ist, beträgt der Preis pro Einheit -41,34.

## <a name="suspend-and-reactivate"></a>Aussetzen und erneutes Aktivieren eines Abonnements

Ihr Abrechnungsdatum ist der 15. jedes Monats. Am 13. Januar erwerben Sie ein neues Abonnement mit einer Lizenz für "$ 4/Monat" und wählen die jährliche Abrechnung aus. Die Lizenz basierte ababstimmungs Datei für den 15. Januar enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Anteilige Gebühren beim Kauf|48,00|1|48,00

Am 1. Februar brechen Sie Ihr Abonnement ab. Die Lizenz basierte ababstimmungs Datei von Februar 15 enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13.01.2018|12.01.2019|Stornierungsgebühr|-48,00|1|-48,00

Am 1. März aktivieren Sie Ihr Abonnement erneut. Die Lizenz basierte ababstimmungs Datei vom März 15 enthält die folgende Abrechnungs Zeile:

|Startdatum der Abrechnung |Enddatum der Abrechnung |Gebührentyp |Unit Price |Menge |Amount (Betrag) |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01.03.2018|12.01.2019|Anteilige Gebühren beim Kauf|41,34|1|41,34

Der jährliche Preis ist 48,00, was einem Preis pro Tag von 0,13 (48,00/365) entspricht.

Preis pro Einheit = Tage im Dienstzeitraum x Preis pro Tag x Anzahl der Lizenzen.

Es gibt 318 Tage im Dienstzeitraum vom 01.03.2018 bis zum 12.01.2019.

Der Preis pro Einheit beträgt also = 41,34 (318 x 0,13 x 1).
