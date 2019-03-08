---
title: Erstellen mehrerer Benutzer für ein Kundenkonto | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in Partner Center hochladen.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: Stapelweises Hochladen, mehrere Benutzer einem Kundenkonto hinzufügen, Kunden eines Benutzers hinzufügen, stapelweises Hochladen der Benutzer des Kunden, Kundenkonto, Kunden des Benutzers, Benutzer
ms.localizationpriority: medium
ms.openlocfilehash: 12bb42d4e1dcf5003ac8790be777c483f216fd6f
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584243"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Hinzufügen von mehreren Benutzern zu einem Kundenkonto

**Gilt für**

-  Partner Center

Sie können mehrere Benutzer gleichzeitig, um ein Kundenkonto hinzufügen, durch Hochladen von einer Datendatei im CSV-Format (.csv) in das Partner Center. Können Sie eine Datei mit Beispieldaten im Partner Center herunterladen und bearbeiten Sie es für Ihre Verwendung, oder Sie können eine neue Datei mit dem unten definierten Datenmodell erstellen.

## <a href="" id="creatingtheimportcsvfile"></a>Anforderungen an die Datei


Damit Sie mit dem Massenupload mehrere Benutzer zum Konto eines Kunden hinzufügen können, müssen die folgenden Voraussetzungen erfüllt sein:

-   Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.
-   Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.
-   Sie können bis zu 100 Datensätze gleichzeitig hochladen. Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.
-   Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.
-   Geben Sie nur die unten beschriebenen Daten ein. Zusätzliche Daten führen zu einem Uploadfehler.

Geben Sie die folgenden Daten in die Datendatei ein:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Name der Spalte** | **Beschreibung**                                                              | **Limitation**                             |
| Vorname      | Vorname des Benutzers (optionales Feld)                                           | Begrenzung von 50 Zeichen                         |
| Nachname       | Nachname des Benutzers (optionales Feld)                                            | Begrenzung von 50 Zeichen                         |
| Anzeigename    | Anzeigenamen im Partner Center (Pflichtfeld)                            | Begrenzung von 50 Zeichen                         |
| E-Mail           | Geschäftliche E-Mail-Adresse des Benutzers beim Kundenunternehmen (erforderliches Feld)           | Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen. |
| Statusupdate   | Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde. | \*\*Leer lassen\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Um mehrere Benutzerkonten zu erstellen.

<a href="" id="creatingtheaccounts"></a>
1.  Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.
2.  Von der **Partner Center** , wählen Sie im Menü **Kunden**, wählen Sie dann einen Kunden aus der Liste.
3.  Wählen Sie **Upload users**.
4.  Wählen Sie unter **Upload user info** die Option **Durchsuchen**.
5.  Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.
6.  Wählen Sie **Überprüfen**.

    **Beachten Sie**  die meisten Fehler bei der kontoerstellung werden durch Dateiprobleme für Daten, z.B. durch fehlende Informationen, ungültige oder doppelte e-Mail-Adressen oder zu viele Einträge in der Datei verursacht.

7.  Nachdem der Partner Center die Datei überprüft hat, wählen Sie den geografischen **Speicherort** für neue Benutzer.
8.  Wählen Sie **Speichern**.
9.  Laden Sie die Informationen zum temporären Kennwort für die Benutzer herunter.

**WICHTIG:** Achten Sie darauf, dass Sie zum Herunterladen der Datei mit den temporären Kennwörtern nun, da Sie dies später vornehmen, können nicht. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

10. Neuen Benutzern werden automatisch die Berechtigungen **Can use licenses and services** zugewiesen. 

 

 



