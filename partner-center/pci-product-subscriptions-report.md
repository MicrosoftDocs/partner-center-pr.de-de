---
title: Bericht zu Partner Center Insights-Abonnements
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sehen Sie sich an, was Sie gut machen und wo Sie die Cloudabonnements verbessern können, die Sie für Ihre Kunden verkaufen oder verwalten.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89806b08485bc4bd286c2e14a19924ca0e281b6d
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854467"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Bericht "Produktabonnements" über das Dashboard "Partner Center Insights" verfügbar

**Geeignete Rollen:** globale | | des Administrator-Agents Berichts-Viewer-| Berichtanzeige der Geschäftsleitung

Der Bericht "Produktabonnements" enthält Analysen zu Cloudabonnements, die Sie verkauft haben oder die Sie für Ihre Kunden verwalten. Dies ist ein produktspezifischer Bericht, der die Leistung von Abonnements enthält, die Cloudprodukten wie Office 365, Azure, Dynamics und anderen zugeordnet sind.

Sie können die folgenden Abschnitte im Bericht "Produktabonnements" anzeigen.

- Zusammenfassung
- Geografische Verteilung von Abonnements
- Trend zum Hinzufügen/Abwanderung von Abonnements
- Abonnementverteilung nach Partnerstandorten, Vertriebskanal, SKUs, Partner-Attach-Typ, Segment
- Trend nach Abonnementzuständen
- Produkttrend

 > [!NOTE]
 > Dieser Bericht ist über das Insights-Dashboard verfügbar. Um diesen Bericht anzuzeigen, muss Ihnen eine bestimmte Rolle in Partner Center zugewiesen werden, z. B. globaler Administrator, Kontoadministrator, Berichts-Viewer oder Berichts-Viewer der Geschäftsleitung. Weitere Informationen finden Sie unter Globaler Administrator Ihres Unternehmens. Bestimmte Datentypen in diesem Bericht sind möglicherweise auch nur für Benutzer mit Berechtigungen des Berichts-Viewers der Geschäftsleitung verfügbar.

## <a name="summary"></a>Zusammenfassung

Der Zusammenfassungsabschnitt enthält eine Momentaufnahmeansicht der Key Performance Indicators (KPIs) im Zusammenhang mit Abonnements, die von Ihnen für Ihre Kunden verkauft oder verwaltet werden.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Zusammenfassung des Abonnementsberichts":::

Weitere Informationen zu den einzelnen Abschnitten der Zusammenfassung finden Sie unten:

- Abonnements:
  - Aktuelle Anzahl der von Ihnen verkauften oder verwalteten Cloudproduktabonnements.
  - Prozentuales Wachstum oder Ablehnen von Abonnements während des ausgewählten Datumsbereichs.
  - Das Mikrodiagramm zeigt einen Monatlichen Trend der Abonnementanzahl während des ausgewählten Datumsbereichs an.

- Aktive Abonnements:
  - Aktuelle Anzahl von Cloudproduktabonnements mit basierend auf Produkttelemetriedaten gemessener aktiver Nutzung. Dies schließt alle Testabonnements im Fall von Azure-Abonnements aus.
  - Prozentuales Wachstum oder Rückgang aktiver Abonnements im ausgewählten Zeitraum.
  - Das Mikrodiagramm zeigt einen Monatlichen Trend aktiver Abonnements während des ausgewählten Datumsbereichs an.

- Hinzugefügte Abonnements:
  - Gesamtanzahl der Kundenabonnements, die von Ihnen während des ausgewählten Datumsbereichs hinzugefügt (verkauft oder verwaltet) wurden. Neue Abonnements mit **dem Status Aktiv** **oder** Erneuert werden als Hinzugefügte Abonnements gezählt.
  - Prozentuales Wachstum oder Rückgang der Abonnements, die im letzten vollständigen Monat im Vergleich zum ersten vollständigen Monat hinzugefügt wurden.
  - Das Mikrodiagramm zeigt einen monatlichen Trend von Abonnements an, die während des ausgewählten Datumsbereichs hinzugefügt wurden.

- Abwanderung von Abonnements:
  - Gesamtanzahl der Kundenabonnements, die während des ausgewählten Datumsbereichs abwanderungen. Abonnements mit dem Status **"Deprovisioned"** oder **"Suspended"** in diesem Monat werden als abwanderungsabonnement gezählt.  
  - Prozentsatz der Abonnements, die während des ausgewählten Datumsbereichs abwanderungen.
  - Das Mikrodiagramm zeigt einen monatlichen Trend der Abonnements an, die über den ausgewählten Datumsbereich abwanderungen.

- Abonnements nach Produkten: Aufschlüsselung der aktuellen Abonnementanzahl nach Cloudprodukten.

## <a name="geographical-spread-of-subscriptions"></a>Geografische Verteilung von Abonnements

In **der Ansicht Abonnements nach Geografie** wird die geografische Verteilung der Gesamtabonnements nach Kundenmarkt angezeigt. Der Gesamtabonnementbetrag umfasst sowohl verkaufte Abonnements als auch aktive Abonnements.

Die Tabelle **Anzahl der Länder/Regionen** enthält die Gesamtanzahl der Länder/Regionen, in denen Sie Abonnements besitzen, sowie den Betrag pro Land der gesamten und aktiven Abonnements.

Sie können ein Land im Raster suchen und auswählen, um an den Ort in der Karte zu zoomen. Drücken Sie die Option **Start** auf der Karte, um zur ursprünglichen Ansicht zurückzukehren. Zeigen Sie auf die Karte, um alle Abonnements und aktiven Abonnements nach Land anzuzeigen. Beide Felder im Raster sind sortierbar.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="Abonnements nach Geografie":::

## <a name="subscription-addschurns"></a>Hinzufügen/Abwanderungen von Abonnements

In dieser Ansicht wird ein Trend von Abonnements dargestellt. Diese werden in verschiedene Kategorien (Neu, Vorhanden, Änderung) für den ausgewählten Datumsbereich unterteilt. Die X-Achse stellt Monate des ausgewählten Datumsbereichs dar. Die Y-Achse stellt die Abonnementanzahl dar. Abwanderungsabonnements werden auf der negativen Skala der Y-Achse dargestellt. 

Das gestapelte Säulendiagramm zeigt eine Aufschlüsselung der neuen, vorhandenen und abwanderungsierten Abonnements für den Monat. Sie können das Säulendiagramm neu erstellen, aufgeschlüsselt nach bestimmten Stapelelementen. Wählen Sie dazu diese spezifischen Elemente in der Legende aus. Sie können auch den Schieberegler oben im Diagramm verwenden, um einen bestimmten Punkt zu vergrößern.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="Abonnement: Hinzufügen und Abwanderungen":::

## <a name="subscription-distribution"></a>Abonnementverteilung

Diese Ansicht zeigt eine Aufschlüsselung Ihrer aktuellen Abonnements nach MpN-Standorten, Kundensegmenten, Vertriebskanal/Azure-Preismodell und dem Zuordnungstyp (z. B. DPOR, DAP usw.). Wählen Sie die entsprechenden Registerkarten aus, um die Aufschlüsselung nach diesen Kategorien anzuzeigen. Um das Kreisdiagramm mit einer Aufschlüsselung bestimmter Elementkategorien zu erstellen, wählen Sie diese Elementkategorien in der Legende aus.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="Abonnementverteilung":::

## <a name="subscription-state-distribution"></a>Verteilung des Abonnementstatus

In dieser Ansicht wird die Verteilung Ihrer aktuellen Kundenabonnements nach Abonnementstatus oder -status angezeigt. Dies schließt die folgenden Abonnementzustände **ein:** **Aktiv**, **Deaktiviert**, Nicht mehr **zurProvision,** **Öffnen**, **InGracePeriod**, **Geschlossen** und Andere .

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="Abonnementstatusverteilung":::

## <a name="products-trend"></a>Produkttrend

Diese Ansicht zeigt ein Balkendiagramm und zwei Kreisdiagramme. Das Balkendiagramm zeigt einen monatlichen Trend von Abonnements, aufgeschlüsselt nach kommerziellen Produkten wie Azure, Office, Dynamics usw.

Die beiden Kreisdiagramme zeigen eine Aufschlüsselung Ihrer aktuellen Kundenabonnements. Das erste Kreisdiagramm bricht Abonnements nach Produkten auf. Das zweite Kreisdiagramm unterbricht Abonnements nach SKUs oder Plänen. Wenn Sie in der  Aufschlüsselung nach Kreisdiagramm Produkte ein Produkt auswählen, wird im angrenzenden Kreisdiagramm eine Aufschlüsselung der Abonnements dieses Produkts nach SKUs angezeigt.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="Produkttrend":::

> [!NOTE]
 > Die Abonnementanzahl, aufgeschlüsselt nach SKUs, stimmen möglicherweise nicht immer mit der Gesamtabonnementanzahl für dieses Produkt überein. Dies kann auftreten, wenn ein Kunde mehrere SKUs unter demselben Produktabonnement erworben hat.

## <a name="next-steps"></a>Nächste Schritte

- Weitere Berichte finden Sie unter [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Sie können die Rohdaten, die diesen Bericht unterstützen, aus dem Abschnitt Berichte herunterladen des Insights-Dashboards herunterladen. [Weitere Informationen](pci-download-reports.md) 
