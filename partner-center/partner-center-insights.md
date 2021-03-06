---
title: Partner Center-Einblicke
description: Sehen Sie sich Partner Center dashboard für einheitliche Berichte an. Erfahren Sie, wie Sie kpIs für Vertrieb und Bereitstellung, Kundenentwicklung und mehr verwenden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 05fad9c7eecbc8b7f639faa24b654fb0474245ca
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277622"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Insights: Ein Dashboard, das die Funktionsweise eines kommerziellen Microsoft-Partners zeigt.

**Geeignete Rollen:** Globale Administratorrechte | Kontoadministrator-| Berichts-Viewer-| Berichts-Viewer

## <a name="introduction"></a>Einführung

Das Insights-Dashboard ist ein vereinheitlichtes Berichtsdashboard in Partner Center für kommerzielle Partner von Microsoft, die für das programm Microsoft Partner Network (MPN) registriert sind. Das Insights-Dashboard bietet eine 360-Grad-Ansicht Ihrer Key Performance Indicators (KPI) für Cloudprodukte wie Office, Azure, Dynamics und Lizenzierungsmodelle wie CSP und EA. Es werden umfangreiche KPI-Berichte verfügbar, die Ihnen helfen können, datengesteuerte Entscheidungen für Ihre Organisation zu treffen. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Rollenbasierte Zugriffssteuerung für das Insights-Dashboard

Es gibt zwei neue Rollen in Partner Center, die speziell für den Zugriff auf Insights entwickelt wurden: **Berichts-Viewer** und **Executive Report Viewer**. Benutzer mit der Rolle "Berichts-Viewer" haben Zugriff auf alle Berichtsdatensätze, während Benutzer mit der Berichts-Viewer-Rolle keinen Zugriff auf vertrauliche Datensätze wie Umsatz- und personenbezogene Daten von Kunden/Mitarbeitern haben. 

Der globale Administrator oder der Kontoadministrator kann Benutzern diese Rollen zuweisen und werden entweder für das gesamte Unternehmen oder für einen bestimmten MPN-Standort zugewiesen.  

>[!Note] 
>Benutzer, die seit dem 20. Januar 2020 MPN-Administratoren waren, wurden automatisch der unternehmensweiten Rolle "Berichts-Viewer" hinzugefügt. Sie können als Berichts-Viewer auf die Berichte zugreifen, ohne dass vom globalen Administrator oder Kontoadministrator explizite Aktionen erforderlich sind. Die globalen Administratoren oder Kontoadministratoren können diese Zuweisungen bei Bedarf überschreiben. 

## <a name="reports-available"></a>Verfügbare Berichte

Die folgenden Berichte sind als Teil des Insights-Dashboards verfügbar.

**Übersicht:** Der Übersichtsbericht enthält eine Momentaufnahmeansicht verschiedener KPIs, die für Sie von Interesse sind, z. B. Kundenanzahl, Anzahl aktiver Abonnements, Azure Consumption Revenue, Aktive Lizenzen usw.

**Kunde:** Im Kundenbericht werden Analysen für Ihre Kunden angezeigt, z. B. Kundendaten, aktive Kunden usw.

**Produkt – Abonnements:** Im Abonnementbericht werden Die Erfassungs- und Nutzungsanalysen für Ihre Cloudabonnements (z. B. O365, Azure, Dynamics usw.) angezeigt.

**Produkt– Lizenzen:** Im Dashboard Lizenzen werden Lizenzanalysen für lizenzbasierte Cloudprodukte wie O365, Dynamics, Power BI usw. angezeigt.

**Produkt – Azure-Nutzung:** Der Azure-Nutzungsbericht enthält Metriken im Zusammenhang mit den Azure-Abonnements Ihrer Kunden, einschließlich Azure-Verbrauchsumsatz und Nutzung nach Verbrauchskategorien.

**Kompetenzen:** Der Bericht Kompetenzen enthält Metriken zu Ihren Kompetenzen "Aktiv", "Qualifiziert" und "Gefährdet".

**Vorteile:** Der Bericht "Vorteile" enthält Analysen zu den Vorteilen von Partnern, die Sie im Vergleich zu den vorteilen erhalten haben.

## <a name="navigating-the-insights-reports"></a>Navigieren in den Insights-Berichten

**Datumsbereichsfilter:** Eine Datumsbereichsauswahl finden Sie in der oberen rechten Ecke jeder Seite. Die Ausgabe der Übersichtsseitendiagramme kann angepasst werden, indem ein Datumsbereich basierend auf den letzten 3, 6 oder 12 Monaten oder ein benutzerdefinierter Datumsbereich ausgewählt wird. Die Standardauswahl für den Datumsbereich beträgt 12 Monate. 

:::image type="content" source="images/pci/intro1.png" alt-text="Einführungsübersicht.":::

**Schaltfläche "Feedback":** Jedes Diagramm/Steuerelement in allen Insights-Berichten wird mit einer Feedbackschaltfläche integriert, mit der Sie Instanzfeedback zu einem Berichtsfeature bereitstellen können. 

 
**Filter auf Seitenebene:** Mit Ausnahme der Berichte Übersicht, Vorteile und Kompetenzen können Sie mit allen Insights-Berichten Filter auf Seitenebene anwenden. 

- Die ausgewählten Filter gelten für alle Diagramme und Metriken auf einer Seite, einschließlich des Zusammenfassungsabschnitts. Ein Filterelement ist verfügbar, wenn Sie Daten innerhalb dieser Filterkriterien haben. 

- Die Standardauswahl jeder Filterliste ist **.** Wenn Sie beispielsweise kein bestimmtes Produkt im Produktfilter ausgewählt haben, werden standardmäßig alle Produkte ausgewählt.

- Die ausgewählten Filter werden oben auf der Seite angezeigt. 

:::image type="content" source="images/pci/filters.png" alt-text="Teilabbildung der Leiste Angewendete Filter mit Filterauswahl für Produkte, Kundenmarkt, Partnerzuordnungen und Vertriebskanäle.":::

### <a name="filters-definitions"></a>Filterdefinitionen:

- Produkte: Liste aller Microsoft Cloud-Produkte, die von Ihrer Organisation verkauft/verwaltet werden, z. B. O365, Azure, D365, EMS, Power BI usw.
- Kundenmarkt: Liste der Kundenländer
- Partnerzuordnungen: Ihr Zuordnungstyp zu den Abonnements Ihrer Kunden, z. B. Digital Partner of Record (DPOR), Delegierte Administratorrechte (Delegated Admin Privilege, DAP) und Partneradministratorlink (PAL). 
- Partnerstandorte: Liste aller MPN-Standorte Ihrer Organisation.
- Vertriebskanäle: Alle Vertriebskanäle/Preise, über die Sie Produkte und Dienste kaufen/bereitstellen, nämlich CSP, EA, CSP indirect, Direct, Advisor, Open, andere
- Kundensegmente: Liste der Kundensegmente für den Kundenstamm des Partners.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Erfahren Sie mehr über die einzelnen Dashboards und Berichte:

- [Partner Center Insights – Übersichtsdashboard](pci-overview-report.md)

- [Partner Center-Einblicke – Dashboard „Kunde“](pci-customer-report.md)

- [Partner Center Insights – Bericht "Abonnements"](pci-product-subscriptions-report.md)

- [Partner Center Insights – Bericht "Lizenzen"](pci-product-licenses-report.md)

- [Partner Center Insights – Azure-Nutzungsbericht](pci-azure-usage-report.md)

- [Partner Center-Einblicke – Bericht „Kompetenzen“](pci-competencies-report.md)

- [Partner Center-Einblicke – Bericht „Vorteile“](pci-benefits-report.md)
