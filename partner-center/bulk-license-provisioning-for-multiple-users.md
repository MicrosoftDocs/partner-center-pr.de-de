---
title: Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie ein Kundenkonto verwenden, um einem Benutzer oder mehreren Benutzern gleichzeitig Lizenzen und Dienste zuzuweisen oder zu widerrufen.
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 79f66e759385f6c7c7928dba58e052ea8699cf21
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149212"
---
# <a name="assign-or-revoke-licenses-at-the-same-time-to-multiple-users-in-a-customer-account"></a>Gleichzeitiges Zuweisen oder Widerrufen von Lizenzen für mehrere Benutzer in einem Kundenkonto

**Geeignete Rollen:** Administrator-Agent| Globale Administratorrechte | Helpdesk-| Sales agent | Benutzerverwaltungsadministrator

Sie können Lizenzen und Dienste einem Benutzer oder gleichzeitig mehreren Benutzern in einem Benutzerkonto zuweisen und die Lizenzzuweisung für Benutzer aufheben.

Im Partner Center werden alle Lizenzberechtigungen im Besitz des Kunden verfolgt und gezeigt.

## <a name="assign-licenses-to-multiple-users"></a>Zuweisen von Lizenzen zu mehreren Benutzern

1. Wählen Sie im Menü **Partner Center** die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

2. Wählen Sie **Benutzer und Lizenzen aus.**

3. Aktivieren Sie das Kontrollkästchen für zwei oder mehr Benutzer aus der Liste. (Aktivieren Sie zum Auswählen aller Benutzer auf der aktuellen Seite das Kontrollkästchen oben in der Spalte **Benutzer**.)

    Mithilfe der Optionen **First**, **Previous**, **Next** und **Last** können Sie Benutzer auf mehreren Seiten suchen und auswählen.

4. Wählen Sie den Link **Ausgewählte Benutzer**. Die angezeigte Liste enthält die ausgewählten Benutzer.

5. Wählen Sie den Link **Lizenzen verwalten**.

    Auf der Seite „Lizenzen verwalten“ werden die Liste der Lizenzansprüche für die Kundenkonten sowie die Anzahl für **Available licenses** für jedes Produkt angezeigt.

    - Die Kontrollkästchen in der Spalte **Produkt** zeigen den Status aller ausgewählten Benutzer für die Produkte, für die Kundenansprüche vorliegen:

       - Wenn alle ausgewählten Benutzer bereits eine Lizenz besitzen, ist das Kontrollkästchen des Produkts ausgefüllt.

       - Wenn einige der ausgewählten Benutzer über eine Produktlizenz verfügen, ist das Kontrollkästchen des Produkts teilweise ausgefüllt.

       - Besitzt keiner der ausgewählten Benutzer eine Produktlizenz, ist das Kontrollkästchen leer.

    - Jeder ausgewählte Benutzer wird in einem kleinen Feld am oberen Seitenrand angezeigt. Benutzer werden in einer sortierten Reihenfolge angezeigt.

    - Wählen Sie einen Link in der Spalte **Assigned**, um eine QuickInfo-Liste der ausgewählten Benutzer anzuzeigen, die bereits über eine Lizenz verfügen.

    - Für alle Produkte ohne verfügbare Lizenzen wird der Link **Buy more** angezeigt. Sie können weitere Lizenzen erwerben, wenn Kunden sie benötigen.

6. Wählen Sie unter **Assign and revoke licenses** die Produktlizenzen für die neuen Benutzer aus. 

   Beispiel: Wenn keiner der ausgewählten Benutzer Office 365 Enterprise-Lizenzen besitzt und Sie diese hinzufügen möchten, aktivieren Sie das Kontrollkästchen. Sie benötigen ausreichend Lizenzen für jedes ausgewählte Produkt.

7. Durch Aktivierung des Kontrollkästchens aller Produkte wählen Sie mehrere Produkte für die Benutzer aus.
    -   Wählen Sie für ein beliebiges Produkt **View service plans**, um die von den Benutzern benötigten Servicepläne anzuzeigen und auszuwählen.

8. Klicken Sie auf **Speichern**. Partner Center öffnet die Bestätigungsseite **Licenses updated**, auf der die Benutzer und ihre neuen Lizenzen aufgeführt sind.

>[!NOTE]
>Einige Microsoft-Produkte sind an bestimmten Standorten möglicherweise nicht verfügbar. Wieder andere Produkte sind abhängig von anderen Produkten oder Diensten oder können dem gleichen Benutzer nicht zusammen zugewiesen werden. Nach dem Speichern werden auf der Bestätigungsseite die Ergebnisse der erfolgreichen Lizenzzuweisung für alle Benutzer sowie fehlerhafte Lizenzzuweisungen angezeigt.

## <a name="revoke-users-license-assignments"></a>Widerrufen von Benutzerlizenzzuweisungen

1. Wählen Sie im Menü **Partner Center** die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

2. Wählen Sie **Benutzer und Lizenzen aus.**

3. Aktivieren Sie das Kontrollkästchen für zwei oder mehr Benutzer aus der Liste. (Aktivieren Sie zum Auswählen aller Benutzer auf der aktuellen Seite das Kontrollkästchen oben in der Spalte **Benutzer**.)

    Blättern Sie durch die Optionen **First**, **Previous**, **Next** und **Last**, um weitere Benutzer zu suchen und auszuwählen. Sie können Benutzer auf mehreren Seiten auswählen.

4. Klicken Sie nach dem Auswählen der Benutzer auf den Link **Ausgewählte Benutzer**. Die angezeigte Liste enthält nur die ausgewählten Benutzer.

5. Wählen Sie den Link **Lizenzen verwalten**.

6. Deaktivieren Sie unter **Assign and revoke licenses** die Kontrollkästchen für den Benutzern zugewiesene Produkte.

   Beispiel: Wenn alle ausgewählten Benutzer Office 365 Enterprise-Lizenzen besitzen und Sie diese widerrufen möchten, deaktivieren Sie das Kontrollkästchen.

7. Wählen Sie **Speichern** aus.

## <a name="next-steps"></a>Nächste Schritte

- [Zuweisen von Lizenzen an einen Benutzer](assign-licenses-to-users.md)

- [Wiederherstellen von Administratorrechten für Azure CSP-Abonnements eines Kunden](revoke-reinstate-csp.md)