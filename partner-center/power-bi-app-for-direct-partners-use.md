---
title: Verwenden Partner Center Analytics für Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Ihre Geschäftsdaten mithilfe der Partner Center Analytics-App für Power BI anzeigen (für direkte Partner im Cloud Solution Provider(CSP)-Programm).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564980"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Ihre Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI anzeigen



**Geeignete Rollen**: Globaler Administrator | Benutzerverwaltungsadministrator | Vertriebsbeauftragter | Administrator-Agent

## <a name="view-your-business-data"></a>Anzeigen Ihrer Geschäftsdaten

Eine visuelle Darstellung Ihrer Geschäftsdaten mit der Partner Center Analytics-App für Microsoft Power BI, einschließlich:

- Wachstum bei Kundenstamm, Abonnements und Lizenzen

- Verwendung von Office 365-, Microsoft Dynamics- und Microsoft Azure-Produkten

- Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem Azure-Abonnement in den letzten 60 Tagen

- Geschätzte Kosten (auf Grundlage der aktuellen Gebührenkarte)

- Möglichkeit zum Exportieren von Datasets und Erstellen benutzerdefinierter Berichte, einschließlich pro Kunde.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informationen zur Vorschauversion der Partner Center Analytics-App

- Diese App ist nur für direkte Partner im Cloud Solution Provider-Programm (CSP) verfügbar. Andere Partner im CSP (z. B. indirekte Wiederverkäufer) können sich nicht anmelden.

- Alle geschätzten Kosten werden vor Steuern/Abrechnungsdaten angezeigt und sind nicht rechtlich bindend. Die geschätzten Kosten dienen nur zu Informationszwecken.

- Die Kundeninformationen basieren auf Abonnements. Alle Kunden, für die Sie vor Kurzem Konten erstellt haben, aber noch keine Abonnements haben, werden nicht in die Anzahl einbezogen.

- Die geschätzten Kosten basiert auf der aktuellen Gebührenkarte, die auf den CSP-Preisen basiert.

- Die Tage sind Kalendertage.

### <a name="business-insights-report"></a>Geschäftsinformationen-Bericht

- **Kunden-Mandanten:** Anzahl unterschiedlicher Azure Active Directory (Azure AD) Von Kunden, die Abonnements erworben haben

- **Neu (letzte 30 Tage):** Neue Kunden, die in den letzten 30 Tagen mindestens ein Abonnement erwerben

- **Änderungsabwanderung (letzte 30 Tage):** Kunden ohne "aktive", "in Grace"- oder "disabled"-Abonnements

- **Neu (letzte 24 Stunden):** Neue Kunden, die in den letzten 24 Stunden mindestens ein Abonnement erwerben

- Geschätzte monatliche Kosten in den letzten **12** Monaten: Trend von Monat zu Monat des geschätzten Rechnungsbetrags vor Steuern, der monatlich über den Zeitraum der letzten 12 Monate aggregiert wurde

- Geschätzte Kosten nach Produkt in den letzten **12** Monaten: Verkaufte Produkte sortiert nach geschätztem Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 12 Monate. Dieser Status gibt die wichtigsten Produkte mit dem größten Umsatz an.

- **Kunden in den letzten 12** Monaten: Monatlicher Trend von Neukunden und Kunden mit Kundenabwanderung im Zeitraum der letzten 12 Monate aggregiert

- Geschätzte Kosten nach Kunde in den letzten **12** Monaten: Kunden sortiert nach dem geschätzten Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 12 Monate. Dieser Status gibt die wichtigsten Kunden an, die den größten Umsatz erzielen.

- **Kundenanzahl nach Produkt:** Verkaufte Produkte sortiert nach zugeordneten Kunden. Dieser Status gibt die wichtigsten Produkte an, die an die meisten Kunden verkauft werden.

### <a name="subscription-insights-report"></a>Abonnement-Bericht

- **Abonnementstatus:**

- Aktiv: Abonnements, die entweder zum Zustand "Aktiv" oder "In Grace" gehören

  - Angehalten: Abonnements, die zum Status "Deaktiviert" gehören

  - Nicht mehr bereitgestellt: Abonnements, die zum Status "Bereitstellungslöschung" oder "Abgelaufen" gehören

- **Ablaufstatus**:

  - Abgelaufen: Abonnements, die bereits abgelaufen sind (wobei das Enddatum des Abonnements in der Vergangenheit liegt)

  - Ablauf nach 30 Tagen: Abonnements, die nach 30 Tagen ablaufen (wobei das Enddatum des Abonnements nach den nächsten 30 Tagen liegt)

  - Ablauf in 30 Tagen: Abonnements, die innerhalb der nächsten 30 Tage ablaufen (wobei das Enddatum des Abonnements zwischen heute und den nächsten 30 Tagen liegt)

- **Abonnements gesamt:** Abonnements im Status "Aktiv", "In Grace" oder "Deaktiviert"

- **Neu (letzte 30 Tage):** Neue Abonnements, die von Kunden innerhalb der letzten 30 Tage erworben wurden

- **Neu (letzte 24 Stunden):** Neue Abonnements, die von Kunden innerhalb der letzten 24 Stunden erworben wurden

- **Ablauf in 30 Tagen:** Abonnements, die innerhalb der nächsten 30 Tage ablaufen

- **Änderungsabwanderung (letzte 30 Tage):** Abonnements, deren Bereitstellung innerhalb der letzten 30 Tage aufgehoben oder angehalten (deaktiviert) wurde

- **Verteilung nach Abonnementtypen:**% Verteilung der Gesamtabonnements nach lizenzbasiertem und nutzungsbasiertem Abonnementtyp

- **Anzahl aktiver Abonnements nach Produkt:** Verkaufte Produkte sortiert nach anzahl aktiver Abonnements

- **Abonnements in den letzten 12 Monaten:** Monatlicher Trend für neue Abonnements und Abwanderungsabonnements, aggregiert über den Zeitraum der letzten 12 Monate

- **Details zum Kundenabonnement:** Detaillierte Ansicht der Kunden, Abonnements und Angebote

### <a name="license-insights-report"></a>Lizenzbericht:

- **Gesamtanzahl der** Lizenzen: Gesamtzahl der Lizenzen, die für alle lizenzbasierten Abonnements aggregiert wurden

- **Neu (letzte 30 Tage):** Lizenzer zusätzlich innerhalb der letzten 30 Tage

- **Änderungsabwanderung (letzte 30 Tage):** Lizenzreduzierung innerhalb der letzten 30 Tage

- **Neu (letzte 24 Stunden):** Lizenzer zusätzlich innerhalb der letzten 24 Stunden

- **Lizenzen in den letzten 90 Tagen:** Monatlicher Trend von Lizenzermäßigungen und -reduzierungen, die monatlich über den Zeitraum der letzten 90 Tage aggregiert wurden

- **Anzahl aktiver Lizenzen nach Produkt:** Verkaufte Produkte sortiert nach aktiver Lizenzanzahl

- **Anzahl aktiver Lizenzen nach Kunde:** Kunden sortiert nach aktiver Lizenzanzahl

- Details zu Kundenlizenzereignissen der letzten **90** Tage: Detaillierte Ansicht der Kunden-, Abonnement- und Abonnementereignisse, einschließlich Ereignisdatum, Ereignisname, Menge und Änderung der Menge.

### <a name="licenses-usage-report"></a>Lizenznutzungsbericht:

- **Nach Produkt zugewiesene Lizenzen:** Verkaufte Produkte sortiert nach Anzahl der Lizenzzuweisungen

- **Nach Produkt verwendete Lizenzen:** Verkaufte Produkte sortiert nach Anzahl der Lizenznutzungen

- **Kundenverteilung für zugewiesene Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenzzuweisung in Prozent

- **Kundenverteilung für genutzte Lizenzen**: Prozentuale Verteilung von Kunden in 20 Prozent-Schritten nach Lizenznutzung in Prozent

- **Vom Kunden zugewiesene Lizenzen:** Detaillierte Ansicht der verkauften lizenzen und von Kunden und Produkten zugewiesenen Lizenzen

- **Vom Kunden verwendete Lizenzen:** Detaillierte Ansicht der verkauften Lizenzen und lizenzen, die von Kunden und Produkten verwendet werden

### <a name="azure-insights-report"></a>Azure-Bericht:

- **Nutzungsbasierte Kunden** in den letzten 12 Monaten: Monatlicher Trend von neuen nutzungsbasierten Kunden und kunden, die auf der nutzungsbasierten Kundenabwanderung basieren, die monatlich über den Zeitraum der letzten 12 Monate aggregiert wurden

- **Nutzungsbasierte Abonnements** in den letzten 12 Monaten: Monatlicher Trend für neue nutzungsbasierte Abonnements und abwanderungsbasierte Abonnements, die monatlich über den Zeitraum der letzten 12 Monate aggregiert wurden

- Geschätzte Nutzungskosten nach Kunde in den letzten **60** Tagen: Nutzungsbasierte Kunden, sortiert nach dem geschätzten Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage. Dieser Status gibt die nutzungsbasierten Kunden an, die den meisten Umsatz erzielen.

- Geschätzte Nutzungskosten nach Kategorie in den letzten **60** Tagen: Verbrauchsklassen nutzungsbasierter Abonnements, sortiert nach dem geschätzten Rechnungs-Dollarbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.

- Geschätzte Nutzungskosten nach Abonnement in den letzten **60** Tagen: Nutzungsbasierte Abonnements nach geschätztem Rechnungsbetrag vor Steuern, aggregiert über den Zeitraum der letzten 60 Tage.

- **Geschätzte Nutzungskosten des Kunden nach Ausgabenbudget:** Kunden werden nach Dem Prozentsatz ihres aktuellen Ausgabenbudgets sortiert, das den Schwellenwert überschreitet (100 %).

### <a name="azure-resource-usage-report"></a>Azure-Ressourcennutzungsbericht:

- **Nutzung von Azure-Ressourcen** nach Tag für den ausgewählten Zeitraum: Tägliche Verbrauchseinheiten für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage.

- **Geschätzte Nutzungskosten** von Azure-Ressourcen für den ausgewählten Zeitraum: Geschätzte Kosten basierend auf der karte der neuesten Rate für jede gemessene Ressource in jedem nutzungsbasierten Abonnement für den ausgewählten Zeitraum innerhalb der letzten 60 Tage. 

## <a name="next-steps"></a>Nächste Schritte

- [Partner Center Analytics-App für Power BI – Übersicht](power-bi-app-for-direct-partners.md)

- [Installation und Vorschauversion der Partner Center Analytics-App für Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
