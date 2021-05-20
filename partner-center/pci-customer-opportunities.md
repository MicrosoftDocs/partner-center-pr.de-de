---
title: Partner Center Insights– CloudAscent Propensity-Berichte
description: Erfahren Sie mehr über die CloudAscent-Propensity-Berichte in Partner Center. Enthält Informationen zur Bereitschaft eines Kunden, Microsoft-Produkte zu erwerben.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153037"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity-Berichte, die über Partner Center Dashboard verfügbar sind

**Geeignete Rollen:**| Berichts-Viewer

Das dashboard Partner Center stellt herunterladbare Propensity-Daten aus dem CloudAscent-Programm bereit. Die Daten zeigen die Wahrscheinlichkeit der Kunden, Microsoft-Produkte zu erwerben.  In diesem Artikel wird die Aufschlüsselung dieser Daten, die Verwendung der Bewertung und ihre Funktionsweise beschrieben.

## <a name="summary-definitions"></a>Zusammenfassungsdefinitionen

- **SMC-Kunden:** Dies ist die Gesamtzahl der Kunden in den Propensity-Downloads.  Kunden werden anhand des Datensatzpartners identifiziert.
- **Abgelaufene Verträge:** Innerhalb des aktuellen Geschäftsjahrs geben wir die Anzahl ablaufender Vereinbarungen an.
- **Open Expiring Revenue**: Der Umsatz, der den offenen ablaufenden Vereinbarungen zugeordnet ist.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Screenshot des Dashboards &quot;Kundenchancen– Zusammenfassung&quot;.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent-SMB-Segmentierung

Das Segment small to medium business (SMB) ist in drei unterschiedliche Untersegmente unterteilt.

1. **Top Unmanaged** umfasst die größten SMB-Kunden mit der größten Chance für Microsoft. Typische Top-Kunden ohne Verwaltung haben ähnliche Merkmale wie verwaltete Konten: eine große Anzahl von Mitarbeitern, große IT-Budgets und -Ausgaben sowie große Mengen an potenziellem Umsatz für Microsoft.

   Wir definieren Top Unmanaged auf zwei Arten:

   - **Top Unmanaged User Based**– umfasst Konten mit 300 oder mehr Mitarbeitern. User-Based Konten sind hervorragende Ziele für den erstmaligen Kauf oder die Erweiterung von benutzerbasierten Abonnementprodukten wie Microsoft 365, Dynamics 365 oder Surface.
   - **Top Unmanaged Compute Based (** Nicht verwaltete Compute-Basiert) – umfasst Konten mit einem Azure-Potenzial von mehr als 10.000 US-Dollar. Computebasierte Konten umfassen vorhandene Azure-Konten. Konten mit erheblichem zukünftigem Potenzial und Konten, die Azure noch erwerben müssen, aber ein Potenzial von mehr als 10.000 USD für Azure haben.

2. **Das mittlere Unternehmen** umfasst Bestandskunden und Kundenkonten mit 25 bis 300 Mitarbeitern.

3. **Kleine Unternehmen** umfassen Unternehmen mit 10 bis 25 Mitarbeitern.

4. **Sehr kleine Unternehmen** umfassen Unternehmen mit 1 bis 9 Mitarbeitern.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Kunde nach SMC-Typ.":::

**Die untersegmente Top Unmanaged** und **Medium Business** stellen LTV-Kunden (High Life Time Value) für Microsoft und Microsoft-Partner dar. Aus diesem Grund sind sie die Hauptbereiche, um das Wachstum in diesem Segment zu fördern. In diesen beiden Untersegmenten sind wir besser positioniert, um den Socket mit Microsoft 365 zu erwerben, mit D365-/Branchen-Apps (LOB) weiter zu monetarisieren und einen hohen LTV für Microsoft zu realisieren.

Heute haben wir zwei Hauptbereiche der Verkaufschance: 1. unser Kunde zuwachst; 2. Obwohl wir Cloudsockets gut erwerben, die Microsoft 365, haben wir in Dynamics 365 und Azure eine große Chance.

Der folgende Screenshot stellt die vier SMB-Untersegmente dar. CloudAscent priorisiert die Profilerstellung, Bewertung und Modellierung aller Konten mit den wichtigsten nicht verwalteten und mittleren Unternehmen.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Screenshot: SMB-Untersegmente":::

## <a name="cloudascent-machine-learning"></a>CloudAscent-Machine Learning

SMB nutzt Machine Learning-Technologie, um Kundenvorhersagen für Vertrieb und Marketing innerhalb der Segmente Top Unmanaged und Medium Business zu fördern. Wie werden Signale gesammelt und in Propensity-Empfehlungen umgewandelt?

- **Datensammlung:** Webcrawler scannen und sammeln Milliarden von Kundensignalen, indem sie die Unternehmensdomänen pingen und Blogbeiträge, Veröffentlichungen, Social Streams und technische Foren überwachen.  Zusätzlich zu den gesammelten Signalen werden firmographics-Informationen sowohl aus internen als auch aus externen Quellen wie D&B, internem Microsoft-Abonnement und Transaktionsdaten gesammelt.

- **Machine Learning:** Die Signale werden in das Machine Learning-Modell eingespeist, das ein strukturiertes Dataset mit Vertriebs- und Marketingvorhersagen für jeden Kunden nach Cloudprodukt und -cluster ausgibt.  Jeder Kunde wird mit einem Modell bewertet, das dem obersten SMB von Microsoft entspricht, das die Fit- und Machine Learning-Algorithmen des Kunden bestimmt, die das Onlineverhalten des Kunden integrieren und als Absicht definieren. Die Bewertung wird in Clustern zusammengeführt, die die Kaufbereitschaft eines Kunden für Microsoft Cloud-Produkte zeigen.

- **Optimierung:** Das Machine Learning System optimiert die Modelle, indem die Transaktionsdaten monatlich und die Abonnementdaten vierteljährlich verarbeitet werden.  Mithilfe der Win/Loss-Daten passt der Machine Learning die Algorithmen an und überprüft, ob die Modelle erwartungsgemäß funktionieren, indem Clusterempfehlungen mit in MSX ausgeführten Verkaufschancen verglichen werden.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot: SMB-Machine Learning":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Wie werden Propensity-Empfehlungen erstellt?

Mithilfe von Signalen, die über Webcrawler gesammelt werden, und daten, die aus verschiedenen Quellen bereitgestellt werden, konsolidieren wir die firmographics-Daten und die Signale der sozialen Medien des Kunden.  Die Bewertung verwendet diese Signale und Daten in Vergleichsmodellen für Anpassungs- und Bewertungsmodelle für Intent.

1. Kundenkonto anpassen

   - Interne und externe Datenpunkte, die Firmografien definieren.

   - Bei der Bewertung von Anpassungen wird ein Modell mit gleichem Aussehen für unseren besten SMB verwendet, um Kunden zu vergleichen und zu prüfen, ob sie für Microsoft Cloud-Produkte geeignet sind.

   - Die Bewertung der Anpassung wird vierteljährlich aktualisiert.

2. Kundenkontoabsicht

   - Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht.

   - Die Absichtsbewertung wird überlagert, um die Cluster zu definieren.

   - Die Absichtsbewertung wird monatlich aktualisiert.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent-SMB-Vorhersagemodelle.":::

3. Clustering

   Die Signale für "Fit" und "Intent" werden zu einer Clustering-Bewertung konsolidiert. CloudAscent verfügt über vier Cluster:

      - Jetzt handeln : Kunden, die für den Vertrieb bereit sind
      - Auswerten – Marketingbereite Kunden
      - Nurture – Fördern von Bewusstseinskampagnen
      - Schulen – Schulen und Überwachen der Absicht

   Mit dem Clustering können Benutzer bestimmte Kunden für Vertriebs- und Marketinginitiativen basierend auf Segmentfaktoren als Ziel verwenden, z. B. Produkt, Geografisches, Branchen- und vertikales Produkt.

   Die **Registerkarte Propensity model (Propensity-Modell)** in den CloudAscent-Arbeitsmappen teilt die Neigung und den geschätzten Leerraumumsatz. Um das Clustering von "Fit" und "Intent" zu definieren, führen wir die folgenden Schritte aus:

      1. Mit ml-Modellen berechnen wir zunächst die Kunden-Anpassungsbewertung und die Absichtsbewertung auf einer Skala von 100.  Die genauen Ergebnisse variieren je nach ML-Modellen.  Beispielergebnisse unten:

         |**Klassifizierung**|**Wert**|
         |---------|:---------|
         |Hoch|75 - 100|
         |Medium|55 - 74|
         |Niedrig|30 - 54|
         |Sehr niedrig|0 - 29|

      2. Mithilfe der oben genannten Regel klassifizieren wir Unternehmen sowohl für Kundenpass- als auch für Absichtssignale als Hoch-, Mittel-, Niedrig- und Sehr niedrig.

      3. Wir zeichnen Kundenpass- und Absichtssignale in einer 2D-Matrix, wobei jede Schnittmenge die Propensität darstellt. Beispiel: High Fit + High Intent = A1, die die höchste Propensität darstellt.

      4. Schließlich gruppieren sich diese Segmente zu Clustern.  Beispielsweise bilden A1, A2, A3 und A4 den Act Now-Cluster.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-Modelle.":::

   Für diese Kunden empfehlen wir, Act Now- und Evaluate-Kunden als Ziel zu betrachten.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

Die folgende Grafik bietet eine Ansicht der einzelnen Propensity-Modelle in CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent-Propensity-Modell.":::

Leerraummodelle bestehen aus Vorhersagen für bestehende Microsoft-Kunden, bei denen sie kein Produkt haben und/oder neue Kunden sind.

Upsellmodelle verwenden Transaktionsdaten, um das Potenzial für upselling in Azure und Microsoft 365 SKUs vorherzusagen.

Diese Kunden verfügen bereits über Azure oder Microsoft 365, und das Upsellmodell zeigt, dass sie wahrscheinlich mehr ihrer vorhandenen SKU erwerben werden.

FÜR WIN 7, Office 2010, SQL Server und Windows Server gibt DIE END OF SERVICE-Kunden (END OF SERVICE) gemeinsam. Die EOS-Daten werden aus MS Sales abgerufen und mit der CloudAscent-Propensitätsmodellierung überlagert, sofern verfügbar. DIE EOS-Daten werden in Modern Work und Azure Sales abgespielt.
