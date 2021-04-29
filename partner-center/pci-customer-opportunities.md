---
title: Partner Center Insights – CloudAscent Propensity-Berichte
description: Erfahren Sie mehr über die CloudAscent Propensity-Berichte in Partner Center. Enthält Informationen über die Neigung eines Kunden, Microsoft-Produkte zu erwerben.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213443"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity-Berichte, die über Partner Center verfügbar sind

**Geeignete Rollen**

- Executive Report-Leser
- Berichtleser

Das Partner Center-Dashboard stellt herunterladbare Propensity-Daten aus dem CloudAscent-Programm bereit. Die Daten zeigen die Wahrscheinlichkeit der Kunden, Microsoft-Produkte zu kaufen.  In diesem Artikel werden die Aufschlüsselung dieser Daten, die Verwendung der Bewertung und ihre Verwendung beschrieben.

## <a name="summary-definitions"></a>Zusammenfassungsdefinitionen

- **SMC-Kunden:** Dies ist die Gesamtzahl der Kunden in den Propensity-Downloads.  Kunden werden anhand des Datensatzpartners identifiziert.
- **Ablaufvereinbarungen:** Innerhalb des aktuellen Geschäftsjahrs geben wir die Anzahl der ablaufenden Vereinbarungen an.
- **Open Expiring Revenue**: Der Umsatz, der den offenen läuftden Vereinbarungen zugeordnet ist.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Screenshot des Dashboards &quot;Kundenchancezusammenfassung&quot;":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent-SMB-Segmentierung

Das Segment small to medium business (SMB) ist in drei unterschiedliche Untersegmente unterteilt.

1. **Top Nicht verwaltet umfasst** die größten SMB-Kunden mit den meisten Verkaufschancen für Microsoft. Typische Nicht verwaltete Top-Kunden haben ähnliche Merkmale wie verwaltete Konten mit einer großen Anzahl von Mitarbeitern, großen IT-Budgets und -Ausgaben und großen Potenziellen Umsatzzahlen für Microsoft.

   Wir definieren Top Unmanaged auf zwei Arten:

   - **Top Unmanaged User Based –** enthält Konten mit 300 oder mehr Mitarbeitern. User-Based Konten sind hervorragende Ziele für den erstmaligen Kauf oder die Erweiterung von benutzerbasierten Abonnementprodukten wie Microsoft 365, Dynamics 365 oder Surface.
   - **Top Unmanaged Compute Based (Top-Basiert für nicht verwaltetes Compute)** – umfasst Konten mit Azure-Potenzial, die größer als 10.000 USD sind. Computebasierte Konten umfassen vorhandene Azure-Konten. Konten mit erheblichem Potenzial für das zukünftige Jahr und Konten, die Azure noch nicht erwerben müssen, aber über ein Azure-Potenzial von mehr als 10.000 USD verfügen.

2. **Mittleres Unternehmen** umfasst Bestandskunden und Kundenkonten mit 25 bis 300 Mitarbeitern.

3. **Small Business** umfasst Unternehmen mit 10 bis 25 Mitarbeitern.

4. **Sehr kleine Unternehmen** umfassen Unternehmen mit 1 bis 9 Mitarbeitern.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Kunde nach SMC-Typ.":::

**Die wichtigsten nicht verwalteten** und **mittleren Geschäftssegmente** stellen LTV-Kunden (High Life Time Value) für Microsoft und Microsoft-Partner dar. Aus diesem Grund sind sie die Hauptbereiche, die das Wachstum in diesem Segment fördern. In diesen beiden Untersegmenten sind wir besser positioniert, um den Socket mit Microsoft 365 zu erwerben, mit D365/LOB-Apps (Line of Business) weiter zu monetarisieren und einen hohen LTV für Microsoft zu erzielen.

Heute haben wir zwei wichtige Möglichkeiten: 1. unserem Kunden wird Wachstum hinzugefügt. 2. Cloudsockets werden zwar gut mit Microsoft 365 erworben, aber wir haben in Dynamics 365 und Azure eine große Chance.

Der folgende Screenshot zeigt die vier SMB-Untersegmente. CloudAscent priorisiert die Profilerstellung, Bewertung und Modellierung aller Top-Konten für nicht verwaltete und mittlere Unternehmen.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Screenshot der SMB-Untersegmente":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB verwendet Machine Learning-Technologie, um Kundenvorhersagen für Vertrieb und Marketing in den Segmenten "Top Unmanaged" und "Medium Business" zu fördern. Wie werden Signale gesammelt und in Empfehlungen zur Propensität umgewandelt?

- **Datensammlung:** Webcrawler scannen und sammeln Milliarden von Kundensignalen, indem sie die Unternehmensdomänen pingen und Blogbeiträge, Veröffentlichungen, Social Streams und technische Foren überwachen.  Zusätzlich zu den gesammelten Signalen werden Firmographics-Informationen sowohl aus internen als auch aus externen Quellen wie D&B, internem Microsoft-Abonnement und Transaktionsdaten gesammelt.

- **Machine Learning:** Die Signale werden in das Machine Learning-Modell eingespeist, das ein strukturiertes DataSet mit Verkaufs- und Marketingvorhersagen für jeden Kunden nach Cloudprodukt und -cluster aus gibt.  Jeder Kunde wird anhand eines Look-as-Look-n-Modells mit dem top-SMB von Microsoft ermittelt, das die Anpassung des Kunden bestimmt, und Machine Learning-Algorithmen, die das Onlineverhalten des Kunden integrieren, definieren als Absicht. Die Bewertung wird in Clustern zusammengeführt, die die Kaufneigenheit eines Kunden zum Erwerb von Microsoft Cloud-Produkten zeigen.

- **Optimierung:** Das Machine Learning optimiert die Modelle, indem die Transaktionsdaten monatlich und die Abonnementdaten vierteljährlich verwendet werden.  Mithilfe der Win/Loss-Daten passt die Machine Learning die Algorithmen an und überprüft, ob die Modelle erwartungsgemäß funktionieren, indem Clusterempfehlungen mit Denkmöglichkeiten in MSX verglichen werden.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot: SMB-Machine Learning":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Wie werden Empfehlungen zur Propensität erstellt?

Mithilfe von Signalen, die über Webcrawler und Daten aus verschiedenen Quellen gesammelt werden, konsolidieren wir die Firmographics-Daten und die Signale in sozialen Medien des Kunden.  Bei der Bewertung werden diese Signale und Daten in Vergleichsmodellen für Anpassungs- und Bewertungsmodelle für intent verwendet.

1. Anpassung des Kundenkontos

   - Interne und externe Datenpunkte, die Firmographics definieren.

   - Bei der Anpassungsbewertung wird ein Modell verwendet, das dem besten SMB gleicht, um Kunden zu vergleichen und zu sehen, ob sie für Microsoft Cloud Products geeignet sind.

   - Die Bewertung der Anpassung wird vierteljährlich aktualisiert.

2. Kundenkontoabsicht

   - Signale im Zusammenhang mit sozialen Medien und dem Onlineverhalten eines Kunden definieren die Absicht.

   - Die Absichtsbewertung wird überlagert, um die Cluster zu definieren.

   - Die Absichtsbewertung wird monatlich aktualisiert.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent-SMB-Vorhersagemodelle.":::

3. Clustering

   Die Signale für "fit" und "intent" werden in einer Clusteringbewertung konsolidiert. CloudAscent verfügt über vier Cluster:

      - Jetzt handeln – vertriebsbereite Kunden
      - Auswerten – Marketingbereite Kunden
      - Nurture : Fördern von Bewusstseinskampagnen
      - Schulen : Schulen und Überwachen auf Absichten

   Mit dem Clustering können Benutzer bestimmte Kunden für Vertriebs- und Marketinginitiativen basierend auf Segmentfaktoren wie Produkt, Geo, Branche und Vertikal anzielen.

   Die Registerkarte **"Propensity model" (Propensity-Modell)** in CloudAscent Workbooks (CloudAscent-Arbeitsmappen) teilt die Propensität und den geschätzten Leerraumumsatz. Um das Clustering von "Fit" und "Intent" zu definieren, gehen wir die folgenden Schritte durch:

      1. Mithilfe von ML-Modellen berechnen wir zunächst die Kundenbewertung und die Absichtsbewertung auf einer Skala von 100.  Die genauen Bewertungen variieren basierend auf ML-Modellen.  Beispielergebnisse unten:

         |**Klassifizierung**|**Wert**|
         |---------|:---------|
         |High|75 - 100|
         |Medium|55 - 74|
         |Niedrig|30 - 54|
         |Sehr niedrig|0 - 29|

      2. Mithilfe der oben genannten Regel klassifizieren wir Unternehmen sowohl für Kundenpass- als auch für Absichtssignale als Hoch-, Mittel-, Niedrig- und Sehr niedrig.

      3. Wir zeichnen Kundenpass- und Absichtssignale in einer 2D-Matrix, wobei jede Schnittmenge die Propensität darstellt. Beispiel: High Fit + High Intent = A1, die die höchste Propensität darstellt.

      4. Schließlich gruppieren sich diese Segmente zu Clustern.  Beispielsweise bilden A1, A2, A3 und A4 den Act Now-Cluster.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-Modelle.":::

   Für diese Kunden wird empfohlen, auf Act Now und Evaluate-Kunden zu abzielen.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

Die folgende Grafik bietet eine Ansicht der einzelnen Propensity-Modelle in CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent-Propensity-Modell.":::

Leerzeichenmodelle bestehen aus Vorhersagen für vorhandene Microsoft-Kunden, bei denen sie kein Produkt haben und/oder neue Kunden sind.

Upsellmodelle verwenden Transaktionsdaten, um das Potenzial für Upselling in Azure und Microsoft 365 ZU prognostizieren.

Diese Kunden verfügen bereits über Azure oder Microsoft 365 und das Upsellingmodell zeigt, dass sie wahrscheinlich mehr ihrer vorhandenen SKU erwerben werden.

DIE END OF-Kunden (End of Service, EOS) werden für Win 7, Office 2010, SQL Server und Windows Server verwendet. Die EOS-Daten werden aus MS Sales gezogen und mit der CloudAscent-Propensity-Modellierung überlagert, sofern verfügbar. DIE EOS-Daten sind in modernen Arbeits- und Azure Sales-Spielen gespeichert.
