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
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795673"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Hinzufügen von mehreren Benutzern zu einem Kundenkonto

**Betrifft**

-  Partner Center

Sie können mehrere Benutzer gleichzeitig Konto eines Kunden hinzufügen, indem Sie eine Datendatei im CSV-Format (CSV) in das Partner Center hochladen. Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und bearbeiten Sie es für Ihre Zwecke, oder Sie können anhand des unten definierten Datenmodells eine neue Datendatei erstellen.

## <a href="" id="creatingtheimportcsvfile"></a>Anforderungen an die Datendatei


Damit Sie mit dem Massenupload mehrere Benutzer zum Konto eines Kunden hinzufügen können, müssen die folgenden Voraussetzungen erfüllt sein:

-   Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.
-   Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.
-   Sie können bis zu 100Datensätze gleichzeitig hochladen. Wenn Sie mehr als 100Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.
-   Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.
-   Geben Sie nur die unten beschriebenen Daten ein. Zusätzliche Daten führen zu einem Uploadfehler.

Geben Sie die folgenden Daten in die Datendatei ein:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Name der Spalte** | **Beschreibung**                                                              | **Einschränkung**                             |
| Vorname      | Vorname des Benutzers (optionales Feld)                                           | Begrenzung von 50Zeichen                         |
| Nachname       | Nachname des Benutzers (optionales Feld)                                            | Begrenzung von 50Zeichen                         |
| Anzeigename    | Im Partner Center (erforderliches Feld) angezeigte Name                            | Begrenzung von 50Zeichen                         |
| E-Mail           | Geschäftliche E-Mail-Adresse des Benutzers beim Kundenunternehmen (erforderliches Feld)           | Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen. |
| Statusupdate   | Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde. | \*\*Keine Angabe\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>So erstellen Sie mehrere Benutzerkonten

<a href="" id="creatingtheaccounts"></a>
1.  Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.
2.  Klicken Sie im Menü " **Partner Center** " Wählen Sie **Kunden**, und wählen Sie einen Kunden aus der Liste.
3.  Wählen Sie **Upload users**.
4.  Wählen Sie unter **Upload user info** die Option **Durchsuchen**.
5.  Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.
6.  Wählen Sie **Überprüfen**.

    **Hinweis:** die meisten Fehler bei der kontoerstellung werden durch datendateifehler, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte e-Mail-Adressen oder zu viele Datensätze in der Datei verursacht.

7.  Wählen Sie nach Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer.
8.  Wählen Sie **Speichern**.
9.  Laden Sie die Informationen zum temporären Kennwort für die Benutzer herunter.

**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

10. Neue Benutzer werden automatisch Berechtigungen **use Licenses and Services** zugewiesen. 

 

 



