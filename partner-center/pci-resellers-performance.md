---
title: Leistungs Dashboard für Partner Center Insights-Reseller
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Das Reseller Performance-Dashboard in Partner Center Insights bietet einen Überblick über die Leistung verschiedener indirekter Reseller eines indirekten CSP-Anbieters.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d2331cfb1b0edf25815de0070b5668d0b91df6f
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086888"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>Reseller Performance Dashboard in Partner Center Insights

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent
- Berichtleser
- Executive Report-Leser

Das Reseller Performance-Dashboard in Partner Center Insights bietet einen Überblick über die Leistung verschiedener indirekter Reseller eines indirekten CSP-Anbieters. Das Dashboard enthält Daten zu den Wiederverkäufern, die aktiv sind, wie viel Umsatz Sie generieren und welche Produkte Umsatz bringen. Indirekte Anbieter können anhand ihres Namens nach einem bestimmten Reseller suchen und im Reseller Performance-Dashboard nach Details für den Reseller suchen.

Die folgenden Abschnitte können Sie im Reseller Performance-Dashboard anzeigen.

- Zusammenfassung
- Geografische Verteilung von Wiederverkäufern
- Hinzufügen/Abwanderung von Wiederverkäufern 
- Umsatz Trend für Reseller 
- Wiederverkäufer Leistung nach Produkten
- Aktive Wiederverkäufer nach Partnerstandorten
- Trend für Umsatz-Geothermie-Verteilung
- Reseller Performance by Customer-Segment
- Reseller MPa-Signatur Status

 > [!NOTE]
 > Dieser Bericht ist über das Insights-Dashboard verfügbar. Zum Anzeigen dieses Berichts müssen Sie eine bestimmte Rolle im Partner Center zuweisen, z. b. globaler Administrator, Konto Administrator, Berichts-Viewer oder Executive Report Viewer. Weitere Informationen finden Sie unter der globale Administrator Ihres Unternehmens. bestimmte Datentypen in diesem Bericht sind möglicherweise auch nur für Benutzer verfügbar, die über Administratorrechte für Berichte verfügen.

## <a name="summary"></a>Zusammenfassung

Der Abschnitt Zusammenfassung enthält eine Momentaufnahme Ansicht der KPIs (Key Performance Indicator), die sich auf den indirekten CSP-Anbieter beziehen.

- Aktive Wiederverkäufer: Anzahl der Wiederverkäufer, die während dieses Monats mindestens ein aktives Abonnement besitzen.

Das Micro-Diagramm zeigt den Monat-zu-Monat-Trend von unterschiedlichen Wiederverkäufern, die während des ausgewählten Datums Bereichs aktiv waren.

- Transaktionsreseller: Anzahl der Wiederverkäufer, die mindestens ein Abonnement während dieses Monats verkauft haben. 

Das Micro-Diagramm zeigt den Monat-über-Monat-Trend von Wiederverkäufern, die für den ausgewählten Datumsbereich registriert sind.

- Neuhändler: Anzahl der Wiederverkäufer, die während dieses Monats mit der Transaktion mit dem indirekten Anbieter begonnen haben. 

Das Micro-Diagramm zeigt den Monat-über-Monat-Trend der Gesamtanzahl neuer Reseller während des ausgewählten Datums Bereichs.

- Berechneter Umsatz USD: Umsatz in USD, der von den Wiederverkäufern während dieses Monats gesteuert wird. 

Das Micro-Diagramm zeigt den Monat-über-Monat-Trend des Umsatzes während des ausgewählten Datums Bereichs.

- Der Abschnitt "Umsatz nach Produkte abgerechnet" bietet einen Monat lang eine Aufschlüsselung der in Rechnung gestellten Umsätze in USD, aufgeteilt nach verkauften Produkten. 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="Zusammenfassung der Wiederverkäufer":::

## <a name="geographical-spread-of-resellers"></a>Geografische Verteilung von Wiederverkäufern

Die Ansicht * * Reseller by geography stellt die geografische Verteilung der Wiederverkäufer bereit. Mithilfe dieses Widgets können **Partner Gesamt** Umsätze, **neuhändler** und in **Rechnung gestellte Umsätze (USD)** anzeigen, die nach verschiedenen geografischen Regionen aufgeteilt werden.

Sie können ein Land im Raster suchen und auswählen, um an den Ort in der Karte zu zoomen. Drücken Sie die **Start** Option in der Karte, um zur ursprünglichen Ansicht zurückzukehren. Zeigen Sie auf die Karte, um den in **Rechnung gestellten Umsatz (USD)** nach Land anzuzeigen. Der in Rechnung gestellte Umsatz (USD) im Raster ist Sortier Bar.

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="Wiederverkäufer nach Geografie ":::

## <a name="resellers-addchurns"></a>Hinzufügen/Abwanderung von Wiederverkäufern

Diese Ansicht bietet einen Monat für die Aufteilung der Anzahl neuer wieder **Verkäufer** **, weiter Verkäufer und** **vorhandener Reseller**. 

- Neuhändler: Anzahl der Wiederverkäufer, die während des ausgewählten Datums Bereichs neu bei dem indirekten Anbieter registriert wurden.
- Verteilende Wiederverkäufer: Anzahl der Wiederverkäufer, die in den letzten sechs Monaten keine Transaktion mit Ausnahme des aktuellen Monats durchgeführt haben.
- Vorhandene Wiederverkäufer: Anzahl der Wiederverkäufer, die im vorherigen Monat transaagiert haben.

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="Hinzufügen/Abwanderung von Wiederverkäufern":::

## <a name="resellers-revenue-trend"></a>Umsatz Trend für Reseller 

In dieser Ansicht wird ein monatlicher Trend des in Rechnung gestellten Umsatzes (USD) mit den Produkten O365, D365, EMS, Power BI und Azure angezeigt. Die gesamtmetriken werden für jeden Monat über die verschiedenen Produkte aggregiert. Der Partner kann anhand des Namens nach einem bestimmten Reseller suchen und nach Daten für diesen bestimmten Reseller suchen. Der in Rechnung gestellte Umsatz (USD) im Raster ist Sortier Bar.

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="Umsatz Trend für Reseller":::

## <a name="reseller-performance-by-products"></a>Wiederverkäufer Leistung nach Produkten

In dieser Ansicht werden wichtige Metriken wie der in Rechnung gestellte Umsatz, die Anzahl der Abonnements und die Anzahl der Lizenzen für verschiedene Produkte monatlich im Monat angezeigt. Das Kreis Diagramm auf der rechten Seite zeigt die allgemeine Aufteilung der Metriken nach verschiedenen Produkten an, sodass der Partner einen kurzen Einblick in die unterschiedlichen Produkte erhält, die der Händler verkauft.

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="Wiederverkäufer Leistung nach Produkten":::

## <a name="active-resellers-by-partner-locations"></a>Aktive Wiederverkäufer nach Partnerstandorten

Diese Ansicht bietet eine Aufteilung aktiver Wiederverkäufer nach Partner geografischen Regionen. Die fünf wichtigsten geografischen Regionen werden in der Legende angezeigt, und die restlichen Regionen werden als "andere" kategorisiert.

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="Aktive Wiederverkäufer nach Partnerstandorten":::

## <a name="revenue-geo-distribution-trend"></a>Trend für Umsatz-Geothermie-Verteilung

Diese Ansicht bietet einen Monat im Monats Trend des in Rechnung gestellten Umsatzes (USD), der durch die fünf wichtigsten Regionen aufgeteilt ist.  Der Rest des Umsatzes wird als "Sonstige" kategorisiert.

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="Trend für Umsatz-Geothermie-Verteilung":::

## <a name="reseller-performance-by-customer-segment"></a>Reseller Performance by Customer-Segment

Diese Ansicht ermöglicht einem Partner, den monatlichen Trend von Umsatz USD, Anzahl der Abonnements und Lizenzen, die durch verschiedene Kundensegmente aufgeteilt werden, zu verstehen. Die fünf wichtigsten Kundensegmente werden im Diagramm angezeigt, und die restlichen werden als "andere" kategorisiert.

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="Reseller Performance by Customer-Segment":::

## <a name="reseller-mpa-signing-status"></a>Reseller MPa-Signatur Status

In dieser Ansicht wird der Status der MPA-Signatur für Reseller zusammen mit zusätzlichen Metadaten, wie z. b. MPN-Status Status, PMC-zu-PC-Migrationsstatus usw.

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="Reseller MPa-Signatur Status":::

## <a name="next-steps"></a>Nächste Schritte

- Weitere Berichte finden Sie unter [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Sie können die Rohdaten, die diesen Bericht über den Abschnitt Berichte herunterladen im Insights-Dashboard herunterladen. [Weitere Informationen](pci-download-reports.md) 
