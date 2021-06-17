---
title: Partner Center Insights Resellers Performance-Dashboard
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Das Dashboard zur Handelspartnerleistung in Partner Center Insights bietet eine Übersicht über die Leistung verschiedener indirekter Vertriebspartner eines CSP Indirect Provider.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cc0fb8a56d397cebeb5a40fa1a1c8d6eae77fe25
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277367"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>Dashboard "Reseller Performance" in Partner Center Insights

**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent| Berichts-Viewer| Executive Report Viewer

Das Dashboard zur Handelspartnerleistung in Partner Center Insights bietet eine Übersicht über die Leistung verschiedener indirekter Vertriebspartner eines CSP Indirect Provider. Das Dashboard enthält Daten zu den aktiven Handelspartnern, zu deren Umsatz und zu den Produkten, die den Umsatz steigern. Indirekte Anbieter können über den Namen nach einem bestimmten Handelspartner suchen und details für den Vertriebspartner im Dashboard für die Wiederverkäuferleistung suchen.

Sie können die folgenden Abschnitte im Dashboard "Reseller Performance" (Handelspartnerleistung) anzeigen.

- Zusammenfassung
- Geografische Verteilung von Handelspartnern
- Hinzufügen/Abwanderung von Handelspartnern 
- Umsatztrend bei Wiederverkäufern 
- Wiederverkäuferleistung nach Produkten
- Aktive Wiederverkäufer nach Partnerstandorten
- Trend zur geografischen Verteilung des Umsatzes
- Wiederverkäuferleistung nach Kundensegment
- MPA-Signaturstatus des Wiederverkäufers

 > [!NOTE]
 > Dieser Bericht ist über das Insights-Dashboard verfügbar. Um diesen Bericht anzeigen zu können, muss Ihnen eine bestimmte Rolle in Partner Center zugewiesen werden, z. B. globaler Administrator, Kontoadministrator, Berichts-Viewer oder Berichts-Viewer für Führungskräfte. Weitere Informationen finden Sie im globalen Administrator Ihres Unternehmens. Bestimmte Datentypen in diesem Bericht sind möglicherweise auch nur für Benutzer verfügbar, die über Berechtigungen des Berichts-Viewers verfügen.

## <a name="summary"></a>Zusammenfassung

Der Zusammenfassungsabschnitt enthält eine Momentaufnahmeansicht der Key Performance Indicators (KPIs), die sich auf die CSP Indirect Provider.

- Aktive Wiederverkäufer: Anzahl der Handelspartner, die während dieses Monats mindestens ein aktives Abonnement haben.

Das Mikrodiagramm zeigt den Monatlichen Trend unterschiedlicher Handelspartner an, die während des ausgewählten Datumsbereichs aktiv waren.

- Transaktionshändler: Anzahl der Handelspartner, die in diesem Monat mindestens ein Abonnement verkauft haben. 

Das Mikrodiagramm zeigt den Trend von Handelspartnern, die für den ausgewählten Datumsbereich registriert sind.

- Neue Wiederverkäufer: Anzahl der Handelspartner, die im Laufe dieses Monats mit der Transaktion mit dem indirekten Anbieter begonnen haben. 

Das Mikrodiagramm zeigt den Trend von Monat zu Monat für die Gesamtzahl der neuen Handelspartner während des ausgewählten Datumsbereichs an.

- Abgerechneter Umsatz IN USD: Umsatz in USD, der von den Handelspartnern in diesem Monat gesteuert wird. 

Das Mikrodiagramm zeigt den Monatlichen Umsatztrend während des ausgewählten Datumsbereichs an.

- Der Abschnitt "Abgerechneter Umsatz nach Produkten" enthält eine Monatsaufschlüsselung des abgerechneten Umsatzes in USD, aufgeteilt nach verkauften Produkten. 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="Reseller-Leistungszusammenfassung.":::

## <a name="geographical-spread-of-resellers"></a>Geografische Verteilung von Handelspartnern

Die Ansicht **Resellers by geography (Handelspartner nach Geografie) stellt die geografische Verteilung von Handelspartnern zur Verfügung. Mithilfe dieses **Widgets** können Partner die Gesamtanzahl von Handelspartnern, Neuen Vertriebspartnern und abgerechneten Umsatz **(USD)** nach verschiedenen geografischen Regionen teilen.

Sie können ein Land im Raster suchen und auswählen, um an den Ort in der Karte zu zoomen. Klicken Sie **auf der** Karte auf die Option Start, um zur ursprünglichen Ansicht zurück zu gehen. Zeigen Sie auf die Karte, um den abgerechneten **Umsatz (USD) nach** Land anzuzeigen. Das Feld Abgerechneter Umsatz (USD) im Raster ist sortierbar.

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="Wiederverkäufer nach Geografie.":::

## <a name="resellers-addchurns"></a>Hinzufügen/Abwanderung von Handelspartnern

Diese Ansicht enthält eine Monatsteilung der Anzahl neuer Vertriebspartner, **abwanderungser** Handelspartner und **vorhandener Handelspartner.** 

- Neue Vertriebspartner: Anzahl der Handelspartner, die während des ausgewählten Datumsbereichs neu beim indirekten Anbieter registriert wurden.
- Vertriebspartner mit Änderungsabwanderung: Anzahl der Handelspartner, die in den letzten sechs Monaten keine Transaktion ausgeführt haben, mit Ausnahme des aktuellen Monats.
- Vorhandene Handelspartner: Anzahl der Handelspartner, die im vorherigen Monat Transaktionen durchgeführt haben.

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="Vertriebspartner add/churns.":::

## <a name="resellers-revenue-trend"></a>Umsatztrend bei Wiederverkäufern 

Diese Ansicht enthält einen monatlichen Trend des abgerechneten Umsatzes (USD), der nach Produkten aufgeteilt ist: O365, D365, EMS, Power BI und Azure. Die allgemeinen Metriken werden für jeden Monat über die verschiedenen Produkte aggregiert. Der Partner kann nach einem bestimmten Handelspartner mit dem Namen suchen und nach Daten für diesen bestimmten Handelspartner suchen. Das Feld Abgerechneter Umsatz (USD) im Raster ist sortierbar.

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="Umsatztrend bei Wiederverkäufern.":::

## <a name="reseller-performance-by-products"></a>Wiederverkäuferleistung nach Produkten

Diese Ansicht enthält eine Aufteilung der wichtigsten Metriken wie z. B. abgerechneter Umsatz, Anzahl der Abonnements und Anzahl der Lizenzen nach verschiedenen Produkten auf Monatsbasis. Das Kreisdiagramm auf der rechten Seite gibt die gesamte Aufteilung der Metriken nach verschiedenen Produkten an, sodass der Partner einen schnellen Überblick über die Aufteilung der verschiedenen Produkte erhält, die der Handelspartner verkauft.

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="Wiederverkäuferleistung nach Produkten.":::

## <a name="active-resellers-by-partner-locations"></a>Aktive Wiederverkäufer nach Partnerstandorten

Diese Ansicht enthält eine Aufteilung der aktiven Handelspartner nach Partnergeografien. Die ersten fünf Geografischen Regionen werden in der Legende angezeigt, die übrigen werden als "Andere" kategorisiert.

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="Aktive Handelspartner nach Partnerstandorten.":::

## <a name="revenue-geo-distribution-trend"></a>Trend zur geografischen Verteilung des Umsatzes

Diese Ansicht enthält einen Monatlichen Trend des abgerechneten Umsatzes (USD), der nach den fünf wichtigsten geografischen Regionen aufgeteilt ist.  Der Rest des Umsatzes wird als "Andere" kategorisiert.

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="Trend der geografischen Verteilung des Umsatzes.":::

## <a name="reseller-performance-by-customer-segment"></a>Wiederverkäuferleistung nach Kundensegment

In dieser Ansicht kann ein Partner den monatlichen Umsatztrend in USD, die Anzahl der Abonnements und Lizenzen nach verschiedenen Kundensegmenten aufteilen. Die fünf wichtigsten Kundensegmente werden im Diagramm angezeigt, die übrigen werden als "Andere" kategorisiert.

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="Wiederverkäuferleistung nach Kundensegment.":::

## <a name="reseller-mpa-signing-status"></a>MPA-Signaturstatus des Wiederverkäufers

Diese Ansicht stellt den MPA-Signaturstatus für Handelspartner zusammen mit zusätzlichen Metadaten wie MPN-Überprüfungsstatus, PMC zu PC-Migrationsstatus usw. zur Verfügung.

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="MPA-Signaturstatus des Wiederverkäufers.":::

## <a name="next-steps"></a>Nächste Schritte

- Weitere Berichte finden Sie unter [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Sie können die Rohdaten, die diesen Bericht unterstützen, aus dem Abschnitt Berichte herunterladen des Insights-Dashboards herunterladen. [Weitere Informationen](pci-download-reports.md) 
