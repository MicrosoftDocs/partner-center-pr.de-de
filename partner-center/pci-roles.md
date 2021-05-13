---
title: rollenbasierter Partner Center Insights-Zugriff
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die spezifischen Rollen, die erforderlich sind, um Partner Center Insights-Berichte anzuzeigen. Dazu gehören die Rollen des Berichts-Viewers der Geschäftsleitung und des Berichts-Viewers.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 803c299311f129c4842a92a27abd9b9addb49f17
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854433"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Rollenbasierte Zugriffssteuerung für das Partner Center Insights-Dashboard

**Geeignete Rollen:** globale | | des Administrator-Agents Berichts-Viewer-| Berichtanzeige der Geschäftsleitung

Das Insights-Dashboard verwendet zwei neue Rollen in Partner Center, um den Mitarbeiterzugriff auf die Berichte zu verwalten: Berichts-Viewer der Geschäftsleitung und Berichts-Viewer.  Benutzer in der Rolle "Berichts-Viewer der Geschäftsleitung" haben Zugriff auf alle Berichtsdatasets, während Benutzer in der Berichts-Viewer-Rolle keinen Zugriff auf sensible Datasets wie Umsatz- und personenbezogene Daten von Kunden/Mitarbeitern haben.  

Wie bei anderen Partner Center Rollen kann der globale Administrator oder der Kontoadministrator diesen Rollen auf der Seite Benutzerverwaltung Benutzer zuweisen. Die Rollen können für das gesamte Unternehmen oder für bestimmte MPN-Standorte gelten. Rollen, die für bestimmte MPN-Speicherorte zugewiesen sind, beschränken den Benutzer auf die Anzeige von Berichtsdaten, die nur den ausgewählten MPN-Speicherorten zugeordnet sind. Partner können einen oder mehrere Standorte aus der folgenden Ansicht auswählen.

:::image type="content" source="images/pci/roles.png" alt-text="Zeigt standortspezifische Partner Center Insights-Rolleneinstellungen für Berichts-Viewer und Berichts-Viewer der Geschäftsleitung an.":::

>[!Note]
> Benutzer, die ab dem 20. Januar 2020 MPN-Administratoren sind, werden automatisch der unternehmensweiten Rolle **Executive Report Viewer** für alle Standorte für diesen Mandanten hinzugefügt. Diese Benutzer können daher ohne explizite Aktion des globalen Administrators oder Kontoadministrators auf die Berichte als Managerberichts-Viewer zugreifen. Die globalen Administratoren und Kontoadministratoren können die automatisch zugewiesenen Rollen dieser Benutzer überschreiben, um ihre Funktionen weiter zu erhöhen oder einzuschränken.

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie mehr über [Partner Center Insights](partner-center-insights.md) und die verschiedenen Berichte.
