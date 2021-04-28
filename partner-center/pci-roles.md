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
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120782"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Rollenbasierte Zugriffssteuerung für das Partner Center Insights-Dashboard

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent
- Berichtleser
- Executive Report-Leser

Das Insights-Dashboard verwendet zwei neue Rollen in Partner Center, um den Mitarbeiterzugriff auf die Berichte zu verwalten: Berichts-Viewer der Geschäftsleitung und Berichts-Viewer.  Benutzer in der Rolle "Berichts-Viewer der Geschäftsleitung" haben Zugriff auf alle Berichtsdatasets, während Benutzer in der Berichts-Viewer-Rolle keinen Zugriff auf vertrauliche Datasets wie Umsatz- und personenbezogene Daten von Kunden/Mitarbeitern haben.  

Wie bei anderen Partner Center Rollen kann der globale Administrator oder der Kontoadministrator diesen Rollen auf der Seite Benutzerverwaltung Benutzer zuweisen. Die Rollen können für das gesamte Unternehmen oder für bestimmte MPN-Standorte gelten. Rollen, die für bestimmte MPN-Speicherorte zugewiesen sind, beschränken den Benutzer auf die Anzeige von Berichtsdaten, die nur den ausgewählten MPN-Speicherorten zugeordnet sind. Partner können in der folgenden Ansicht einen oder mehrere Standorte auswählen.

:::image type="content" source="images/pci/roles.png" alt-text="Zeigt standortspezifische Partner Center Insights-Rolleneinstellungen für Berichts-Viewer und Berichts-Viewer der Geschäftsleitung an.":::

>[!Note]
> Benutzer, die ab dem 20. Januar 2020 MPN-Administratoren sind, werden automatisch der unternehmensweiten Rolle **Executive Report Viewer** für alle Standorte für diesen Mandanten hinzugefügt. Diese Benutzer können daher ohne explizite Aktion des globalen Administrators oder Kontoadministrators auf die Berichte als Berichts-Viewer der Geschäftsleitung zugreifen. Die globalen Administratoren und Kontoadministratoren können die automatisch zugewiesenen Rollen dieser Benutzer überschreiben, um ihre Funktionen weiter zu erhöhen oder einzuschränken.

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie mehr über [Partner Center Insights](partner-center-insights.md) und die verschiedenen Berichte.
