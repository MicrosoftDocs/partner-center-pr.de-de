---
title: Ermitteln der Desktopanzahl und der Gebührenstufe
ms.topic: how-to
ms.date: 02/18/2021
description: Erfahren Sie, wie Sie die Channel Incentives-Plattform (CHIP) verwenden, um informationen zur Desktopanzahl und zum Gebührentarif für eine Vereinbarung zu finden.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276936"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Suchen der Desktopanzahl und Gebührenstufe für eine Vereinbarung

**Geeignete Rollen:** Primärer Kontakt oder Programmadministrator

Sie können sich bei [explore.ms](https://www.explore.ms/) anmelden, um die Vereinbarung zu überprüfen, oder eine Datei herunterladen, die Vertragsdetails für die Desktopanzahl und die Gebührenstufe bereitstellt.

## <a name="to-locate-the-information"></a>So suchen Sie die Informationen

### <a name="method-1--explorems"></a>Methode 1 – Explore.ms

1. Öffnen [Sie explore.ms](https://www.explore.ms/) in Internet Explorer. 

>[!Note]
>Sie können diese Funktion nicht in Google Chrome oder Microsoft Edge ausführen.

2. Melden Sie sich mit Ihrem Arbeits-, Schul- oder Schulkonto oder Ihrer Live-ID an.  

3. Wählen Sie im Feld **Berichte** die Option **Vereinbarungen aus.**

4. Geben Sie auf der resultierenden Seite die Vereinbarungsnummer in das Feld **Suche** ein, und wählen Sie dann **Spalten auswählen/sortieren aus.**

5. Wählen Sie im Popupfenster in der Liste der verfügbaren Spalten die **Option Vertragsdesktopanzahl** aus, und wählen Sie dann den Pfeil nach rechts aus, um die Spalte hinzuzufügen. Klicken Sie auf **OK**.

6. Wählen Sie **Suchen aus.**

7. Scrollen Sie auf dem daraufhin angezeigten Bildschirm durch die Ergebnisse, um die Spalte **Agreement Desktop Count (Vertragsdesktopanzahl)** zu finden. 

8. Verwenden Sie die Desktopanzahl, um die Gebührenstufe basierend auf der unten angegebenen Gebührentabelle zu ermitteln.  

| Gebührenstufe | Desktopanzahl |
| ------ | :-----------: |
|  Ein | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Enterprise Incentive-Ebenen basieren auf der Desktop- oder Benutzeranzahl (je nachdem, welcher Wert höher ist) bei Registrierungen im kommerziellen und öffentlichen Sektor (PS). Für Registrierungen ohne natürliche zugeordnete Desktop- oder Benutzeranzahl wendet Microsoft eine Desktopanzahl basierend auf der Desktopanzahl oder Benutzeranzahl des zugehörigen EA an. <br><br>Wenn kein begleitendes EA vorhanden ist, basiert die Gebührenstufe auf dem Tarif der Registrierung. Die Preisstufe des Deals kann auch auf [www.explore.ms](https://www.explore.ms/)angezeigt werden. <br><br>Wenn es mehrere Pool- und/oder Preisebenen für das vorhandene EA/EAS gibt, zahlen Microsoft Incentives auf der höchsten zugewiesenen Preis-/Poolebene, wobei Ebene A die niedrigste ebene und Ebene D die höchste ist.

#### <a name="pool-and-pricing-levels"></a>Pool- und Preisebenen

Nachdem Sie mithilfe der oben beschriebenen Schritte in explore.ms nach der Vertragsnummer gesucht haben, wählen Sie die Vertragsnummer aus. Dadurch gelangen Sie zur Seite mit den Vertragsdetails, auf der die **Vertragszusammenfassung** und **die Angebote** angezeigt werden. Der Abschnitt "Angebote" enthält die Preisstufen.

## <a name="method-2---chip"></a>Methode 2 – CHIP

1. Melden Sie sich bei CHIP an, und wählen Sie LSP-Incentives aus.

2. Wählen Sie auf der Seite **Partner payment summary (Partnerzahlungszusammenfassung)** den Berichtsmonat aus, den Sie anzeigen möchten, und wählen Sie dann **berechnungsdetails** aus der Dropdownliste unter **Export to Excel (Nach Excel exportieren)** aus:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Suchen Sie nach Programmdetails.":::

3. Der Export wird gestartet, und Sie können die Datei öffnen oder unter in einem Ziel speichern.)

4. Wenn der Bericht geöffnet ist, navigieren Sie ganz links zur Registerkarte **DetailReport-FlatFile:**

:::image type="content" source="images/chip/flatfile.png" alt-text="Flatfiledownload.":::

Sie können nun nach der Vertragsnummer suchen, die Sie in Spalte J suchen, und sie finden die zugewiesene Desktopanzahl in Spalte R mit der Bezeichnung Agreement_DesktopCount. Sie können die Gebührenstufe für diese Vereinbarung auch in der Spalte "KI" mit der Bezeichnung Tarif bestätigen.

## <a name="next-steps"></a>Nächste Schritte

- [Behandeln von Problemen mit dem CHIP-Zugriff](chip-access-trouble.md)
