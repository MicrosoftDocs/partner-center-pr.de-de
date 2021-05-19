---
title: Felder für die CSV-Datei zum Importieren mehrerer Benutzer für ein Kundenkonto
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Um einem Kundenkonto mehrere Benutzer hinzuzufügen, erstellen Sie eine csv-Datei (durch Komma getrennte Werte) mit entsprechenden Feldern.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150980"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Hinzufügen mehrerer Benutzer zu einem Kundenkonto durch Erstellen einer CSV-Datei

**Geeignete Rollen**: Globaler Administrator

Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im durch Komma getrennten Wertdateiformat (CSV) in die Partner Center. Sie können eine Beispieldatendatei aus dem Partner Center herunterladen und sie für Ihre Zwecke anpassen oder anhand des unten definierten Datenmodells eine neue Datendatei erstellen.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Anforderungen an die Datendatei

Um dem Konto eines Kunden mithilfe des Massenuploadprozesses mehrere Benutzer hinzuzufügen, müssen Sie die folgenden Anforderungen erfüllen:

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
| Anzeigename    | Der im Partner Center angezeigte Name (erforderliches Feld)                            | Maximal 50 Zeichen                         |
| E-Mail   | Geschäftliche E-Mail-Adresse des Benutzers beim Kundenunternehmen (Pflichtfeld)           | Jeder Benutzer muss über eine eindeutige E-Mail-Adresse verfügen. |
| Statusaktualisierung   | Wird verwendet, um anzugeben, ob der neue Benutzerdatensatz erfolgreich erstellt wurde. | \*\*Keine Angabe\*\*                        |

## <a name="next-steps"></a>Nächste Schritte

- [Hinzufügen mehrerer Benutzer für einen Kunden](adding-multiple-users-to-a-customer-account.md)