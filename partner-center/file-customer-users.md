---
title: Felder für CSV-Datei zum Importieren mehrerer Benutzer für ein Kundenkonto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wenn Sie einem Kundenkonto mehrere Benutzer hinzufügen möchten, erstellen Sie eine Datei mit Komma getrennten Werten (CSV-Datei) mit entsprechenden Feldern.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441420"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Hinzufügen mehrerer Benutzer zu einem Kundenkonto durch Erstellen einer CSV-Datei

**Geeignete Rollen**

- Globaler Administrator

Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in das Partner Center hochladen. Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Anforderungen an die Datendatei

Wenn Sie dem Konto eines Kunden mithilfe des Massen Uploads mehrere Benutzer hinzufügen möchten, müssen Sie die folgenden Anforderungen erfüllen:

- Sie müssen über globale Administratorberechtigungen für das Kundenkonto verfügen.
- Jeder Benutzer muss eine eindeutige E-Mail-Adresse besitzen, die an die E-Mail-Domäne(n) des Kunden angehängt sind.
- Sie können bis zu 100 Datensätze gleichzeitig hochladen. Wenn Sie mehr als 100 Benutzer hinzufügen müssen, erstellen Sie zusätzliche Datendateien, und laden Sie sie hoch.
- Alle Benutzer müssen sich am gleichen geografischen **Standort** befinden.
- Geben Sie nur die unten beschriebenen Daten ein. Zusätzliche Daten führen zu einem Uploadfehler.

Geben Sie die folgenden Daten in die Datendatei ein:

| **Spaltenname** | **Beschreibung**  | **Einschränkung**  |
|:-------- |:------  |:----- |
| Vorname  | Vorname des Benutzers (optionales Feld)  | Maximal 50 Zeichen  |
| Nachname  | Nachname des Benutzers (optionales Feld)  | Maximal 50 Zeichen  |
| `Display name`    | Der im Partner Center angezeigte Name (erforderliches Feld)                            | Maximal 50 Zeichen                         |
| Email   | Geschäftliche e-Mail-Adresse des Benutzers im Kunden Unternehmen (Pflichtfeld)           | Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen. |
| Statusaktualisierung   | Wird verwendet, um anzugeben, ob der neue Benutzerdaten Satz erfolgreich erstellt wurde. | \*\*Keine Angabe\*\*                        |

## <a name="next-steps"></a>Nächste Schritte

- [Hinzufügen mehrerer Benutzer für einen Kunden](adding-multiple-users-to-a-customer-account.md)