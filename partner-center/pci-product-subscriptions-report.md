---
title: Partner Center Insights-Abonnementbericht
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sehen Sie sich an, was Ihnen gut geht und wo Sie die Cloudabonnements verbessern können, die Sie für Ihre Kunden verkaufen oder verwalten.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cd226122f8e69e0667006f274d2ef080bbe47b9b
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565422"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Bericht zu Produktabonnements, der über das Dashboard Partner Center Insights verfügbar ist

**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent| Berichts-Viewer| Executive Report Viewer

Der Bericht Produktabonnements enthält Analysen zu Cloudabonnements, die Sie verkauft haben oder die Sie für Ihre Kunden verwalten. Dies ist ein produktspezifischer Bericht, der die Leistung von Abonnements enthält, die Cloudprodukten wie Office 365, Azure, Dynamics und anderen zugeordnet sind.

Sie können die folgenden Abschnitte im Bericht Produktabonnements anzeigen.

- Zusammenfassung
- Geografische Verteilung von Abonnements
- Trend zum Hinzufügen/Ändern von Abonnements
- Abonnementverteilung nach Partnerstandorten, Vertriebskanal, SKUs, Anfügen von Partnern, Segment
- Trend nach Abonnementzuständen
- Produkttrend

 > [!NOTE]
 > Dieser Bericht ist über das Insights-Dashboard verfügbar. Um diesen Bericht anzeigen zu können, muss Ihnen eine bestimmte Rolle in Partner Center zugewiesen sein, z. B. globaler Administrator, Kontoadministrator, Berichts-Viewer oder Berichts-Viewer für Führungskräfte. Weitere Informationen finden Sie unter Globaler Administrator Ihres Unternehmens. Bestimmte Datentypen in diesem Bericht sind möglicherweise auch nur für Benutzer mit Berechtigungen des Berichts-Viewers für Führungskräfte verfügbar.

## <a name="summary"></a>Zusammenfassung

Der Zusammenfassungsabschnitt enthält eine Momentaufnahmeansicht der Key Performance Indicators (KPIs) im Zusammenhang mit Abonnements, die von Ihnen für Ihre Kunden verkauft oder verwaltet werden.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Zusammenfassung des Abonnementsberichts.":::

Weitere Informationen zu den einzelnen Abschnitten der Zusammenfassung finden Sie unten:

- Abonnements:
  - Aktuelle Anzahl der cloudbasierten Produktabonnements, die von Ihnen verkauft oder verwaltet werden.
  - Prozentuales Wachstum oder Rückgang von Abonnements während des ausgewählten Datumsbereichs.
  - Das Mikrodiagramm zeigt einen Monatlichen Trend der Abonnementanzahl während des ausgewählten Datumsbereichs an.

- Aktive Abonnements:
  - Aktuelle Anzahl von Cloudproduktabonnements mit basierend auf Produkttelemetriedaten gemessener aktiver Nutzung. Dies schließt alle Testabonnements für Azure-Abonnements aus.
  - Prozentuales Wachstum oder Rückgang aktiver Abonnements im ausgewählten Zeitraum.
  - Das Mikrodiagramm zeigt einen Monatlichen Trend aktiver Abonnements während des ausgewählten Datumsbereichs an.

- Hinzugefügte Abonnements:
  - Gesamtanzahl der Kundenabonnements, die von Ihnen während des ausgewählten Datumsbereichs hinzugefügt (verkauft oder verwaltet) wurden. Neue Abonnements mit **dem Status Aktiv** **oder** Erneuert werden als Hinzugefügte Abonnements gezählt.
  - Prozentuales Wachstum oder Rückgang der Abonnements, die im letzten vollständigen Monat im Vergleich zum ersten vollständigen Monat hinzugefügt wurden.
  - Das Mikrodiagramm zeigt einen monatlichen Trend von Abonnements an, die während des ausgewählten Datumsbereichs hinzugefügt wurden.

- Abwanderung von Abonnements:
  - Gesamtanzahl der Kundenabonnements, die während des ausgewählten Datumsbereichs abwanderungen. Abonnements mit dem Status **"Deprovisioned"** oder **"Suspended"** in diesem Monat werden als abwanderungsabonnement gezählt.  
  - Prozentsatz der Abonnements, die während des ausgewählten Datumsbereichs abwanderungen.
  - Das Mikrodiagramm zeigt einen monatlichen Trend der Abonnements, die im ausgewählten Datumsbereich abwanderungen.

- Abonnements nach Produkten: Aufschlüsselung der aktuellen Abonnementanzahl nach Cloudprodukten.

## <a name="geographical-spread-of-subscriptions"></a>Geografische Verteilung von Abonnements

In **der Ansicht Abonnements nach Geografie** wird die geografische Verteilung der Gesamtabonnements nach Kundenmarkt angezeigt. Der Gesamtabonnementbetrag umfasst sowohl verkaufte Abonnements als auch aktive Abonnements.

In **der Tabelle Anzahl der Länder/Regionen** werden die Gesamtanzahl der Länder/Regionen, in denen Sie Abonnements haben, und der Betrag pro Land der gesamten und aktiven Abonnements angezeigt.

Sie können ein Land im Raster suchen und auswählen, um an den Ort in der Karte zu zoomen. Klicken Sie **auf der** Karte auf die Option Start, um zur ursprünglichen Ansicht zurück zu gehen. Zeigen Sie auf die Karte, um alle Abonnements und aktiven Abonnements nach Land anzuzeigen. Beide Felder im Raster sind sortierbar.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="Abonnements nach Geografie.":::

## <a name="subscription-addschurns"></a>Add-/Änderungs-/Änderungsabonnements für Abonnements

Diese Ansicht zeigt einen Trend von Abonnements. Diese sind für den ausgewählten Datumsbereich in verschiedene Kategorien (Neu, Vorhanden, Änderung) unterteilt. Die X-Achse stellt Monate des ausgewählten Datumsbereichs dar. Die Y-Achse stellt die Abonnementanzahl dar. Abwanderungsabonnements werden auf der negativen Skala der Y-Achse dargestellt. 

Das gestapelte Säulendiagramm zeigt eine Aufschlüsselung neuer, vorhandener und abwanderungsabonnements für den Monat. Sie können das Säulendiagramm neu erstellen, aufgeschlüsselt nach bestimmten Stapelelementen. Wählen Sie dazu die spezifischen Elemente in der Legende aus. Sie können auch den Schieberegler oben im Diagramm verwenden, um einen bestimmten Zeitraum zu vergrößern.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="Abonnements werden addiert und abwanderungen.":::

## <a name="subscription-distribution"></a>Abonnementverteilung

Diese Ansicht enthält eine Aufschlüsselung Ihrer aktuellen Abonnements nach Ihren Microsoft Partner Network(MPN)-Standorten, Kundensegmenten, dem Vertriebskanal/Azure-Preismodell und dem Zuordnungstyp. Wählen Sie die entsprechenden Registerkarten aus, um die Aufschlüsselung nach diesen Kategorien zu sehen. Um das Kreisdiagramm mit einer Aufschlüsselung bestimmter Elementkategorien zu erstellen, wählen Sie diese Elementkategorien in der Legende aus.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="Abonnementverteilung.":::

## <a name="subscription-state-distribution"></a>Verteilung des Abonnementstatus

In dieser Ansicht wird die Verteilung Ihrer aktuellen Kundenabonnements nach Abonnementstatus oder -status angezeigt. Dies schließt die folgenden Abonnementzustände **ein:** **Aktiv**, **Deaktiviert** **,** Nicht mehr vorgesehen , **Öffnen**, **InGracePeriod**, **Geschlossen** und Andere .

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="Verteilung des Abonnementstatus.":::

## <a name="products-trend"></a>Produkttrend

Diese Ansicht zeigt ein Balkendiagramm und zwei Kreisdiagramme. Das Balkendiagramm zeigt einen monatlichen Trend von Abonnements, aufgeschlüsselt nach kommerziellen Produkten wie Azure, Office und Dynamics.

Die beiden Kreisdiagramme zeigen eine Aufschlüsselung Ihrer aktuellen Kundenabonnements. Das erste Kreisdiagramm bricht Abonnements nach Produkten auf. Das zweite Kreisdiagramm unterbricht Abonnements nach SKUs oder Plänen. Wenn Sie ein Produkt  im Aufschlüsselungsdiagramm nach Produkten auswählen, wird im angrenzenden Kreisdiagramm eine Aufschlüsselung der Abonnements dieses Produkts nach SKUs angezeigt.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="Produkttrend.":::

> [!NOTE]
 > Die Abonnementanzahl, aufgeschlüsselt nach SKUs, stimmen möglicherweise nicht immer mit der Gesamtabonnementanzahl für dieses Produkt überein. Dies kann auftreten, wenn ein Kunde mehrere SKUs unter demselben Produktabonnement erworben hat.

## <a name="next-steps"></a>Nächste Schritte

- Weitere Berichte finden Sie unter [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Sie können die Rohdaten, die diesen Bericht unterstützen, aus dem Abschnitt Berichte herunterladen des Insights-Dashboards herunterladen. [Weitere Informationen](pci-download-reports.md) 
