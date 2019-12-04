---
title: Erstellen mehrerer Benutzer für ein Kundenkonto | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in Partner Center hochladen.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: Massenupload, einem Kundenkonto mehrere Benutzer hinzufügen, Benutzer eines Kunden hinzufügen, Massenupload der Benutzer eines Kunden, Kundenkonto, Kundenbenutzer, Benutzer
ms.localizationpriority: medium
ms.openlocfilehash: 2195d23074a3e7c397b5f557fd3bed9ec0cc518e
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721984"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Hinzufügen von mehreren Benutzern zu einem Kundenkonto

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator

Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in das Partner Center hochladen. Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.

## <a href="" id="creatingtheimportcsvfile"></a>Anforderungen an die Datendatei

Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:

- Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.
- Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.
- Sie können bis zu 100 Datensätze gleichzeitig hochladen. Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.
- Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.
- Geben Sie nur die unten beschriebenen Daten ein. Zusätzliche Daten führen zu einem Uploadfehler.

Geben Sie die folgenden Daten in die Datendatei ein:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Name der Spalte** | **Beschreibung**                                                              | **Einschränkung**                             |
| Vorname      | Vorname des Benutzers (optionales Feld)                                           | Begrenzung von 50 Zeichen                         |
| Nachname       | Nachname des Benutzers (optionales Feld)                                            | Begrenzung von 50 Zeichen                         |
| Anzeigename    | Der im Partner Center angezeigte Name (erforderliches Feld)                            | Begrenzung von 50 Zeichen                         |
| „E-Mail“           | Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)           | Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen. |
| Statusupdate   | Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde. | \*\*Keine Angabe\*\*                        |

### <a href="" id="createmultipleuseraccounts"></a>So erstellen Sie mehrere Benutzerkonten

<a href="" id="creatingtheaccounts"></a>

1. Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.

2. Melden Sie sich beim Partner Center- [Dashboard](https://partner.microsoft.com/dashboard)an.

3. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

4. Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.

5. Wählen Sie unter **Upload user info** die Option **Durchsuchen**.

6. Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.

7. Wählen Sie **Überprüfen**.

    **Hinweis**  Die meisten Fehler bei der Kontoerstellung werden durch Datendateiprobleme verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in der Datei.

8. Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.
9. Wählen Sie **Speichern**.
10. Laden Sie die Informationen zum temporären Kennwort für die Benutzer herunter.

**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

10. Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen. 

 

 



