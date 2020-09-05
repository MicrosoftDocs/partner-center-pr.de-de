---
title: Rollen basierter Zugriff auf Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informieren Sie sich über die spezifischen Rollen, die zum Anzeigen von Partner Center Insights-Berichten erforderlich sind Hierzu gehören die Rollen des Executive Report Viewer und der Berichts-Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2020
ms.locfileid: "89490608"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Rollenbasierte Zugriffs Steuerung für das Partner Center Insights-Dashboard

Das Insights-Dashboard verwendet zwei neue Rollen im Partner Center, um den Mitarbeiter Zugriff auf die Berichte-Executive Report Viewer und Report Viewer zu verwalten.  Benutzer in der Rolle "Executive Report Viewer" haben Zugriff auf alle Berichts Datasets, während Benutzer in der Rolle "Berichts-Viewer" keinen Zugriff auf sensible Datasets haben, wie z. b. Umsatz und persönliche Daten von Kunden und Mitarbeitern.  

Wie bei anderen Partner Center-Rollen kann der globale Administrator oder der Konto Administrator diesen Rollen auf der Seite "Benutzerverwaltung" Benutzer zuweisen. Die Rollen können auf das gesamte Unternehmen oder auf bestimmte MPN-Orte angewendet werden. Rollen, die für bestimmte MPN-Orte zugewiesen werden, begrenzen den Benutzer für die Anzeige von Berichtsdaten, die nur den ausgewählten MPN-Orten zugeordnet sind. Partner können einen oder mehrere Standorte aus der folgenden Ansicht auswählen.

:::image type="content" source="images/pci/roles.png" alt-text="Zeigt standortspezifische Partner Center Insights-Rollen Einstellungen für die Berichts Anzeige und die Executive Report Viewer an.":::

>[!Note]
> Benutzer, die MPN-Administratoren seit dem 20. Januar 2020 sind, werden automatisch der unternehmensweiten **Executive Report Viewer** -Rolle für alle Standorte dieses Mandanten hinzugefügt. Diese Benutzer können auf die Berichte als Executive Report Viewer zugreifen, ohne dass für den globalen Administrator oder Konto Administrator eine explizite Aktion erforderlich ist. Die globalen Administratoren und Konto Administratoren können die automatisch zugewiesenen Rollen dieser Benutzer außer Kraft setzen, um ihre Funktionen weiter zu erhöhen oder einzuschränken.

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie mehr über [Partner Center Insights](partner-center-insights.md) und die verschiedenen Berichte.
