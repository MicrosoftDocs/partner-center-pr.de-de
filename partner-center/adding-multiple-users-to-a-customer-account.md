---
title: Erstellen mehrerer Benutzer für ein Kundenkonto | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in Partner Center hochladen.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: Massenupload, einem Kundenkonto mehrere Benutzer hinzufügen, Benutzer eines Kunden hinzufügen, Massenupload der Benutzer eines Kunden, Kundenkonto, Kundenbenutzer, Benutzer
ms.localizationpriority: medium
ms.openlocfilehash: 36130f268c9d33217ef3473136ec511f374fb583
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798628"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Hinzufügen von mehreren Benutzern zu einem Kundenkonto

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator

Sie können dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzufügen, indem Sie eine Datendatei im CSV-Format in das Partner Center hochladen. Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Anforderungen an die Datendatei

Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:

- Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.
- Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.
- Sie können bis zu 100 Datensätze gleichzeitig hochladen. Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.
- Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.
- Geben Sie nur die unten beschriebenen Daten ein. Zusätzliche Daten führen zu einem Uploadfehler.

Geben Sie die folgenden Daten in die Datendatei ein:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Spaltenname** | **Beschreibung**                                                              | **Einschränkung**                             |
| Vorname      | Vorname des Benutzers (optionales Feld)                                           | Maximal 50 Zeichen                         |
| Nachname       | Nachname des Benutzers (optionales Feld)                                            | Maximal 50 Zeichen                         |
| `Display name`    | Der im Partner Center angezeigte Name (erforderliches Feld)                            | Maximal 50 Zeichen                         |
| E-Mail           | Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)           | Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen. |
| Statusaktualisierung   | Hiermit wird angegeben, ob der Datensatz des neuen Benutzers erfolgreich erstellt wurde. | \*\*Keine Angabe\*\*                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a>So erstellen Sie mehrere Benutzerkonten

<a href="" id="creatingtheaccounts"></a>

1. Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können.

2. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

3. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

4. Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.

5. Wählen Sie unter **Upload user info** die Option **Durchsuchen**.

6. Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.

7. Wählen Sie **Überprüfen** aus.

    **Beachten Sie**  , dass die meisten Fehler bei der Kontoerstellung durch Datendatei Probleme verursacht werden, einschließlich fehlender Informationen, fehlerhafter oder doppelter e-Mail-Adressen oder zu viele Datensätze in der Datei.

8. Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.
9. Wählen Sie **Speichern** aus.
10. Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.

**WICHTIG:** Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, da dies später nicht mehr möglich ist. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

10. Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen. 

 

 



