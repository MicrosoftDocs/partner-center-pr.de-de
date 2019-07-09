---
title: Microsoft-Learn-Analysen | Partner Center
ms.topic: article
ms.date: 07/05/2019
description: Informationen zum Verstehen Sie Ihre Analysen learning
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09d4ca14c1b407e9010ab26bccaf612f9caad732
ms.sourcegitcommit: bd83621eb29fafbda341ad41814a9ae5c1e78b00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/08/2019
ms.locfileid: "67622528"
---
# <a name="microsoft-learn-analytics-report"></a>Microsoft-Learn-Analysebericht

Die Microsoft-Learn-Bericht bietet Ihnen mit Informationen über die lerner in Ihrem Unternehmen, einschließlich Module, mit denen, die Sie abgeschlossen sind, und die Lernpfade, die, denen Sie sich befinden. Der Bericht zeigt den Status jedes einzelnen lerner. Der globale Administrator und der MPN-Administrator für Ihr Unternehmen können die Daten anzeigen.

## <a name="how-to-read-the-report"></a>Gewusst wie: Lesen Sie den Bericht

### <a name="summary-charts"></a>Diagramme mit testzusammenfassungen

**Anzahl der Personen trainiert**: Anzahl der alle unterschiedlichen lerner, die mindestens ein Modul während des ausgewählten Datumsbereichs abgeschlossen haben 

**Trainierte Einzelpersonen trend Mini-Diagramm**: Monat für Monat die kumulierte Anzahl der aktiven lernmodule 

**Anzahl der Module vervollständigungen**: Die Anzahl der Module vervollständigungen durch die lerner im Unternehmen die Partners während des ausgewählten Datumsbereichs.
Angenommen, "Modul 1" von 15 Personen, abgeschlossen ist und die "Modul 2" durch die gleichen 15 Personen abgeschlossen wurde, wird die Anzahl der Module vervollständigungen 30. Das Abschlussdatum Modul sollten im ausgewählten Datumsbereich fallen.

**Modul vervollständigungen trend Mini-Diagramm**: Monat für Monat die kumulierte Anzahl von der Modul-vervollständigungen 

**Lernen die Anzahl der Abschlüsse Pfad**: Anzahl von Learning Pfad vervollständigungen durch die lerner im Unternehmen die Partners während des ausgewählten Datumsbereichs.
Wenn Lernpfad "Path-1" von 20 Einzelpersonen und Lernpfad abgeschlossen ist z. B. "Pfad 2" von den gleichen 20 Reviewern abgeschlossen wurde, wird die Anzahl der Lernpfad für Abschluss 40. Das Abschlussdatum des Learning-Pfad sollten in den ausgewählten Datumsbereich fallen.

**Lernen Sie die Pfad-vervollständigungen trend Mini-Diagramm**: Monat für Monat die kumulierte Anzahl der Learning Pfad vervollständigungen 

### <a name="trained-individuals-monthly-trend"></a>Trainiertes Einzelpersonen nutzungstrend für diesen Monat

**X-Achse** Monat für den Zeitfilter ausgewählt ist. 

**Y-Achse** ist die Anzahl der aktiven lerner, die für diesen Monat (erstmaligen Abschluss eines Moduls) registriert haben. Dies ist nicht kumulativ.

### <a name="module-completions-monthly-trend"></a>Vervollständigungen auftragstrend für Modul

**X-Achse** Monat für den Zeitfilter ausgewählt ist. 

**Y-Achse** ist von der Modul-vervollständigungen für diesen Monat. Dies ist nicht kumulativ.

### <a name="learning-path-completions-monthly-trend"></a>Vervollständigungen auftragstrend für Learning den Pfad

**X-Achse** Monat für den Zeitfilter ausgewählt ist. 

**Y-Achse** ist die Anzahl der Modul-Abschlüsse in diesem Monat. Dies ist nicht kumulativ.

### <a name="learning-path-completion-tabs"></a>Lernen die Pfad-Abschluss-Registerkarten 

- Registerkarte "Modul"

**Modul vervollständigungen Ringdiagramm**: Aufschlüsselung von der Modul-vervollständigungen (Anzahl, die im Abschnitt "Zusammenfassung" angezeigt werden) durch die Modulnamen.

Anzahl, die in der Mitte des Diagramms angezeigt wird, die Gesamt-Module abgeschlossen

**Vervollständigungen von Rolle**: Aufschlüsselung von der Modul-vervollständigungen von der Rolle des Moduls. Wenn ein Modul mehrere Rollen zugeordnet ist, wird jede der Rollen für die Anzahl der Modul-vervollständigungen hinzugefügt.

In der Mitte der Ringdiagramm angezeigten Anzahl ist die Anzahl der unterschiedlichen Rollen für die vervollständigungen Modul. 

**Vervollständigungen nach Produkt**: Aufschlüsselung von der Modul-vervollständigungen durch das Produkt, das Modul zugeordnet ist. Wenn ein Modul mit mehreren Produkten zugeordnet ist, wird jedes der Produkte für die Anzahl der Modul-vervollständigungen hinzugefügt.    

In der Mitte Ringdiagramm angezeigten Zahl ist die Anzahl der unterschiedlichen Produkte für die vervollständigungen Modul.  

- Registerkarte "Learning Pfad"    

**Lernen die Pfade vervollständigungen Ringdiagramm**: Aufschlüsselung von dem Learning Pfade vervollständigungen (Anzahl, die im Abschnitt "Zusammenfassung" angezeigt) anhand des Namens.

**Vervollständigungen von Rolle**: Aufschlüsselung der Learning Pfade vervollständigungen von der Rolle. Wenn ein Modul mehrere Rollen zugeordnet ist, wird jede der Rollen für die Anzahl der Modul-vervollständigungen hinzugefügt.

**Vervollständigungen nach Produkt**: Aufschlüsselung der Learning Pfade vervollständigungen durch das Produkt, der der Lernpfad zugeordnet ist. Wenn ein Modul mit mehreren Produkten zugeordnet ist, wird jedes der Produkte für die Anzahl der Modul-vervollständigungen hinzugefügt.

### <a name="completions-by-learning-individuals"></a>Vervollständigungen, indem Sie lernen, Personen

Microsoft-Learn identifiziert lernmodule mit einem User-Objekt-ID Unter den **Registerkarte Module**, alle lerner werden von den Modulen abgeschlossen sortiert. Sie werden mit ihren Microsoft-Learn-Benutzernamen, Objekt-ID und Anzahl der Module angezeigt. Sie können die Verwendung von Benutzername suchen.

So erhalten Sie einen lerner des wird erläutert, wie die Objekt-ID des Benutzers: 

1. Melden Sie sich beim [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Sie müssen der globale Administrator des Azure AD-Mandanten des Unternehmens sein.)

2. Kopieren Sie die Benutzerobjekt-ID, die [Bereich hervorgehoben](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) im Graph-Explorer. 

