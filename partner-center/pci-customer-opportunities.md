---
title: Partner Center Insights-cloudascent-Neigungs Berichte
description: Erfahren Sie mehr über die cloudascent-Neigungs Berichte in Partner Center. Enthält Informationen über die Neigung eines Kunden, Microsoft-Produkte zu erwerben.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175286"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Im Partner Center-Dashboard verfügbare cloudascent-Neigungs Berichte

**Geeignete Rollen**
- Executive Report-Leser
- Berichtleser

Das Partner Center-Dashboard bietet herunterladbare Daten aus dem cloudascent-Programm. Die Daten zeigen die Kunden Neigung zum Kauf von Microsoft-Produkten an.  In diesem Artikel wird beschrieben, wie Sie diese Daten zusammenbrechen, wie Sie die Bewertung nutzen und was Sie bedeutet.

## <a name="summary-definitions"></a>Zusammenfassungs Definitionen

- **SMC-Kunden**– Dies ist die Gesamtzahl der Kunden in den "Neigungen"-Downloads.  Kunden werden nach Partner of Record identifiziert.
- **Verträge ablaufen**– innerhalb des aktuellen Geschäftsjahrs geben wir die Anzahl der ablaufenden Vereinbarungen an.
- **Ablaufender Umsatz**– der Umsatz, der den ablaufenden Vereinbarungen zugeordnet ist.
- **Öffnen**Sie den abgelaufenen Umsatz – den Umsatz, der den offenen Ablauf Verträgen zugeordnet ist.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen.":::

## <a name="cloudascent-smb-segmentation"></a>Cloudascent-SMB-Segmentierung

Das Segment Small to Mittel Business (SMB) ist weiter in drei unterschiedliche unter Segmente unterteilt.

1. **Top nicht verwaltet** umfasst die größten SMB-Kunden mit den meisten Verkaufschancen für Microsoft. Typische, nicht verwaltete Kunden haben ähnliche Merkmale wie verwaltete Konten, eine große Anzahl von Mitarbeitern, große IT-Budgets und Ausgaben sowie große Mengen potenzieller Umsätze für Microsoft.

   Wir definieren Top nicht verwaltete zwei Möglichkeiten:

   - **Top nicht verwaltetes Benutzer basiertes**– umfasst Konten mit 300 oder mehr Mitarbeitern. User-Based Konten sind hervorragend für den erstmaligen Kauf oder die Erweiterung von benutzerbasierten Abonnement Produkten wie M365, D365 oder Surface geeignet.
   - **Top nicht verwaltetes serverbasiertes** – schließt Konten mit Azure-Potenzial ein, das größer als $10K ist. Compute-basierte Konten enthalten bereits vorhandene Azure. Konten mit erheblichem Potenzial für das zukünftige Jahr und Konten, die noch Azure erwerben, aber ein Potenzial für Azure haben, das größer als $10K ist.

2. **Mittelständische Unternehmen** umfassen vorhandene Kunden und Perspektiven Konten mit 25 bis 300 Mitarbeitern.

3. **Small Business** umfasst alle verbleibenden Unternehmen mit weniger als 25 Mitarbeitern.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen.":::

Die meisten **nicht verwalteten** und **mittelständischen unter** Segmente stellen High-Life-Time-Kunden (LTV)-Kunden für Microsoft und Microsoft-Partner dar. Daher sind Sie die führenden Schwerpunktbereiche für das Wachstum in diesem Segment. In diesen beiden unter Segmenten sind wir besser positioniert, um den Socket mit M365 zu erwerben, mit D365/Azure Line of Business (LOB)-apps weiter zu monetarisieren und ein hohes LTV für Microsoft zu realisieren.

Heute haben wir zwei wichtige Bereiche von Verkaufschancen – 1. Unsere Kunden fügen Wachstum hinzu. 2. Wir haben zwar eine gute Lösung für Cloud Sockets mit M365, aber wir haben eine große Gelegenheit in D365 und Azure.

Der folgende Screenshot stellt die drei SMB-unter Segmente und die optimierten Routen zu Market dar. Cloudascent priorisieren Sie die Profilerstellung, Bewertung und Modellierung aller obersten, nicht verwalteten und mittelgroßen Geschäftskonten.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen.":::

## <a name="cloudascent-machine-learning"></a>Cloudascent-Machine Learning

SMB nutzt Machine Learning-Technologie, um Kunden Vorhersagen für Umsätze und Marketing in den obersten, nicht verwalteten und mittelgroßen Geschäfts Segmenten zu fördern. Wie werden Signale gesammelt und in neiglichkeits Empfehlungen umgewandelt?

- **Erfassung von Daten**: Webcrawler Scannen und erfassen Milliarden von Kunden Signalen, indem Sie die Unternehmens Domänen pingen und überwachen: Blogbeiträge, Pressemitteilungen, Social Streams und technische Foren.  Zusätzlich zu den erfassten Signalen werden firmugraphics-Informationen sowohl aus internen als auch aus externen Quellen wie D&B, internen Microsoft-Abonnements und Transaktionsdaten gesammelt.

- **Machine Learning**: die Signale werden in das Machine Learning-Modell einfließen, das ein strukturiertes Dataset mit Umsatz-und Marketing Vorhersagen für jeden Kunden nach cloudprodukt und-Cluster ausgibt.  Jeder Kunde wird mit einem ähnlichen Modell wie der Top-SMB von Microsoft bewertet, der die Anpassung des Kunden bestimmt, sowie Machine Learning-Algorithmen, die das Online Verhalten des Kunden als Absicht integrieren. Die Bewertung wird in Clustern zusammengeführt, die die Neigung eines Kunden zum Erwerb Microsoft Cloud Produkte anzeigen.

- **Optimierung**: das Machine Learning System optimiert die Modelle, indem die Transaktionsdaten monatlich und die Abonnement Daten vierteljährlich genutzt werden.  Mithilfe der Win/Loss-Daten passt der Machine Learning die Algorithmen an und überprüft, ob die Modelle erwartungsgemäß funktionieren, indem Sie Cluster Empfehlungen mit Verkaufschancen in MSX vergleicht.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen.":::

## <a name="cloudascent-propensity"></a>Cloudascent-Neigung

Wie werden Empfehlungen zur Neigung erstellt?

Mithilfe von Signalen, die mithilfe von Webcrawlern und Daten aus verschiedenen Quellen gesammelt werden, konsolidieren wir die Signale der firmugraphics-Daten und der Social Media-Daten des Kunden.  Die Bewertung verwendet diese Signale und Daten in Vergleichsmodellen für die Anpassung und Bewertung von Modellen.

1. Anpassung an das Kundenkonto

   - Interne und externe Datenpunkte, die firmugraphics definieren.

   - Bei der Bewertungs Bewertung wird ein ähnliches Modell verwendet, um Kunden zu vergleichen und zu überprüfen, ob Sie für Microsoft Cloud Produkte geeignet sind.

   - Die Anpassungs Bewertung wird vierteljährlich aktualisiert.

2. Absicht des Kundenkontos

   - Signale im Zusammenhang mit sozialen Medien und dem Online Verhalten eines Kunden definieren beabsichtigt.

   - Die beabsichtigte Bewertung ist überlastet, um die Cluster zu definieren.

   - Die beabsichtigte Bewertung wird monatlich aktualisiert.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen." zu definieren, werden die folgenden Schritte durchlaufen:

      1. Mithilfe von ml-Modellen berechnen wir zuerst die Customer fit-Bewertung und die Intent-Bewertung auf einer Skala von 100.  Genaue Ergebnisse variieren basierend auf ml-Modellen.  Folgende Beispiel Ergebnisse:

         |**Klassifizierung**|**Wert**|
         |---------|:---------|
         |High|75-100|
         |Medium|55-74|
         |Niedrig|30 - 54|
         |Sehr niedrig|0 - 29|

      2. Mithilfe der oben genannten Regel klassifizieren wir Unternehmen als hoch, Mittel, niedrig und sehr niedrig zwischen Kunden-und Intent-Signalen.

      3. Wir zeichnen Customer fit-und Intent-Signale in einer 2D-Matrix, wobei jede Schnittmenge die Neigung darstellt.     Beispielsweise "High fit + High Intent = a1", die die höchste Neigung darstellt.

      4. Schließlich gruppieren Sie diese Segmente, um Cluster zu bilden.  Beispiel: a1, a2, a3, A4 bildet den Act Now-Cluster.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen.":::

   Für diese Kunden empfiehlt es sich, jetzt agieren und Kunden zu evaluieren.

## <a name="cloudascent-products--models"></a>Cloudascent-Produkte & Modelle

Die folgende Grafik enthält eine Ansicht der einzelnen Modell Modell in cloudascent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Screenshot des Übersichts Dashboards für Kunden Chancen.":::

Leerraum Modelle bestehen aus Vorhersagen für vorhandene Microsoft-Kunden, bei denen Sie nicht über ein Produkt und/oder Kunden für neue potenziellen Kunden verfügen.

Upselling-Modelle verwenden Transaktionsdaten, um das Potenzial für Upselling in Azure und M365-SKUs vorherzusagen.

EOS nutzt das Ende der Dienst Kunden für Win 7, Office 2010, SQL Server und Windows Server. Die EOS-Daten werden aus MS Sales abgerufen und mit dem Modell der cloudascent-Neigung, soweit verfügbar, überlagert. EOS-Daten sind in den modernen arbeiten und Azure-Verkaufs spielen tätig.
