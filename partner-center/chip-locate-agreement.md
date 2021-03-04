---
title: Suchen nach der Desktop Anzahl und der Gebühr
ms.topic: how-to
ms.date: 02/18/2021
description: Erfahren Sie, wie Sie die Channel-Incentive-Plattform (Chip) verwenden, um die Informationen zur Desktop Anzahl und zur Gebühr für eine Vereinbarung zu ermitteln.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756121"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Suchen der Desktopanzahl und Gebührenstufe für eine Vereinbarung

**Geeignete Rollen**

- Primärer Kontakt oder Programm Administrator

Sie können sich bei [explore.ms](https://www.explore.ms/) anmelden, um die Vereinbarung zu überprüfen, oder Sie können eine Datei herunterladen, in der Vertragsdetails für die Desktop Anzahl und die Gebühren Stufe

## <a name="to-locate-the-information"></a>So suchen Sie die Informationen

### <a name="method-1--explorems"></a>Methode 1 – explore.ms

1. Öffnen Sie [explore.ms](https://www.explore.ms/) in Internet Explorer. 

>[!Note]
>Diese Funktion kann nicht in Google Chrome oder Microsoft Edge durchgeführt werden.

2. Melden Sie sich mit Ihrem Geschäfts-/Schulkonto oder ihrer Live ID an.  

3. Wählen Sie im Feld **Berichte** die Option **Verträge** aus.

4. Geben Sie auf der daraufhin resultierenden Seite die Vertragsnummer in das **Suchfeld** ein, und wählen Sie dann **Select/Order Columns** aus.

5. Wählen Sie im Popup Fenster in der Liste Verfügbare Spalten die Option **Agreement-Desktop Anzahl** aus, und klicken Sie dann auf den Pfeil nach rechts, um die Spalte hinzuzufügen. Klicken Sie auf **OK**.

6. Wählen Sie **Suchen aus.**

7. Scrollen Sie im resultierenden Bildschirm durch die Ergebnisse, um die Spalte Vereinbarungs **Desktop Anzahl** zu suchen. 

8. Verwenden Sie die Anzahl der Desktops, um die Gebühr basierend auf der unten aufgeführten Raten Tabelle zu ermitteln.  

| Gebühren Stufe | Anzahl der Desktops |
| ------ | :-----------: |
|  A | 0 – 2.399    |
|  B | 2.400 – 5.999    |
|  C | 6.000 – 14.999    |
|  D | 15.000 +   |

>[!NOTE]
>Die Enterprise-Incentive-Stufen basieren auf der Desktop-oder Benutzer Anzahl (je nachdem, welcher Wert höher ist) in den Registrierung von kommerziellen und öffentlichen Sektoren (PS). Bei Registrierungen ohne natürliche zugeordnete Desktop-oder Benutzer Anzahl wendet Microsoft eine Desktop Anzahl basierend auf der Anzahl der Desktops oder der Benutzer Anzahl des begleitenden EA an. <br><br>Wenn kein begleitendes EA vorhanden ist, basiert die Gebühr auf der Preisstufe der Registrierung. Der Preisstufe des Deals kann auch auf [www.explore.ms](https://www.explore.ms/)angezeigt werden. <br><br>Wenn für den vorhandenen EA/EAS-Tarif mehrere Pool-und/oder Preisstufen vorhanden sind, werden von Microsoft Anreize mit der höchsten zugewiesenen Preis-/Poolebene gezahlt, wobei Ebene A die niedrigste und die höchste Ebene D ist.

#### <a name="pool-and-pricing-levels"></a>Pool und Preisstufen

Wählen Sie nach der Durchsuchen der Vertragsnummer in explore.ms mithilfe der oben beschriebenen Schritte die Vertragsnummer aus. Dadurch gelangen Sie zur Seite mit den Vereinbarungs Details, auf der die **Zusammenfassung** und die **Angebote** der Vereinbarung angezeigt werden. Der Abschnitt "Angebote" enthält die Preisstufen.

## <a name="method-2---chip"></a>Methode 2: Chip

1. Melden Sie sich bei Chip an, und wählen Sie LSP-Anreize

2. Wählen Sie auf der Seite **Zusammenfassung der Partner Zahlungen** den Berichtsmonat aus, den Sie anzeigen möchten, und wählen Sie dann **Berechnungs Details** aus der Dropdown Liste unter **Exportieren nach Excel** aus:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Programm Details suchen":::

3. Der Export wird gestartet, und Sie können entweder die Datei öffnen oder speichern/speichern unter einem Ziel.

4. Wenn der Bericht geöffnet ist, navigieren Sie zu der Registerkarte **Detailreport-Flatfile** in der unteren linken Ecke:

:::image type="content" source="images/chip/flatfile.png" alt-text="Flatfiledownload":::

Sie können nun in der Spalte J nach der Vertragsnummer suchen, nach der Sie suchen, und die zugewiesene Desktop Anzahl finden Sie in der Spalte R mit der Bezeichnung Agreement_DesktopCount. Sie können auch die Gebühr für diese Vereinbarung in der Spalte "AI" mit der Bezeichnung "Tier" bestätigen.

## <a name="next-steps"></a>Nächste Schritte

- [Behandeln von Problemen mit dem Chip Zugriff](chip-access-trouble.md)
