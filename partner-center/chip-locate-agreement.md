---
title: Suchen nach Desktopanzahl und Gebührenstufe
ms.topic: how-to
ms.date: 02/18/2021
description: Erfahren Sie, wie Sie die Channel Incentives-Plattform (CHIP) verwenden, um informationen zur Desktopanzahl und zum Gebührentarif für eine Vereinbarung zu finden.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148991"
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
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Die Enterprise Incentive-Ebenen basieren auf der Desktop- oder Benutzeranzahl (je nach Höherem) bei Registrierungen im kommerziellen und öffentlichen Sektor (Public Sector, PS). Für Registrierungen ohne natürlich zugeordnete Desktop- oder Benutzeranzahl wendet Microsoft eine Desktopanzahl basierend auf der Anzahl der Desktops oder der Benutzeranzahl des zugehörigen EA an. <br><br>Wenn es kein zugehöriges EA gibt, basiert die Gebührenstufe auf dem Tarif der Registrierung. Die Preisstufe des Deals kann auch auf der Seite [www.explore.ms.](https://www.explore.ms/) <br><br>Wenn es mehrere Pool- und/oder Preisstufen für das vorhandene EA/EAS gibt, zahlen Microsoft Incentives auf der Ebene mit den höchsten zugewiesenen Preisen/Pools, bei denen Ebene A die niedrigste und Ebene D die höchste ist.

#### <a name="pool-and-pricing-levels"></a>Pool- und Preisstufen

Wählen Sie nach der Suche nach der Vereinbarungsnummer in explore.ms den oben beschriebenen Schritten die Vertragsnummer aus. Dadurch wird die Seite mit den Vertragsdetails angezeigt, auf der die **Zusammenfassung und** angebote der Vereinbarung **angezeigt werden.** Der Abschnitt "Angebote" enthält die Tarife.

## <a name="method-2---chip"></a>Methode 2– CHIP

1. Melden Sie sich bei CHIP an, und wählen Sie LSP-Incentives aus.

2. Wählen Sie **auf der Seite** Partner payment Summary (Partnerzahlungszusammenfassung) den Berichtsmonat aus, den Sie anzeigen möchten, und wählen Sie dann in der Dropdownliste unter Nach Excel exportieren die Option Berechnungsdetails **aus:** 

:::image type="content" source="images/chip/chiplocate.png" alt-text="Suchen von Programmdetails":::

3. Der Export wird gestartet, und Sie können entweder die Datei öffnen oder unter einem Ziel speichern bzw. speichern.

4. Wenn der Bericht geöffnet ist, navigieren Sie ganz unten links zur Registerkarte **DetailReport-FlatFile:**

:::image type="content" source="images/chip/flatfile.png" alt-text="Flat file download (Flatdateidownload)":::

Sie können nun nach der Vertragsnummer suchen, die Sie in Spalte J suchen. Sie finden die anzahl der zugewiesenen Desktops in spalte R mit der Bezeichnung Agreement_DesktopCount. Sie können die Gebührenstufe für diese Vereinbarung auch in der Spalte "KI" mit der Bezeichnung Tarif bestätigen.

## <a name="next-steps"></a>Nächste Schritte

- [Behandeln von CHIP-Zugriffsproblemen](chip-access-trouble.md)
