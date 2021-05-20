---
title: Hinzufügen mehrerer Benutzer für ein Kundenkonto
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Um dem Konto eines Kunden mehrere Benutzer hinzuzufügen, laden Sie eine Datendatei in Partner Center mithilfe des csv-Dateiformats (durch Komma getrennte Werte) hoch.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150470"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Hochladen einer CSV-Datei von Benutzern in das Konto eines Kunden


**Geeignete Rollen**: Globaler Administrator

Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im durch Komma getrennten Wertdateiformat (CSV) in die Partner Center. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Erstellen der Datei mit Kundenbenutzern und Hochladen in das Kundenkonto

1. Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können. Informationen zum Importieren mehrerer Benutzer für ein Kundenkonto finden Sie unter Felder für [die CSV-Datei.](file-customer-users.md) 

2. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

3. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

4. Wählen Sie die Registerkarte Benutzer **und Lizenzen des** Kunden und dann Benutzer hochladen **aus.**

5. Wählen Sie unter **Upload user info** die Option **Durchsuchen**.

6. Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.

7. Wählen Sie **Überprüfen** aus.

    **Hinweis:** Der Großteil der Fehler bei der Kontoerstellung wird durch Datendateifehler verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in einer Datei.

8. Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.
9. Klicken Sie auf **Speichern**.
10. Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.

    >[!IMPORTANT]
    > Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, weil dies später nicht mehr möglich ist. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

11. Neuen Benutzern werden automatisch Berechtigungen von Kann Lizenzen und Dienste **verwenden zugewiesen.** 

## <a name="next-steps"></a>Nächste Schritte

- [Erteilen sie Kunden die Berechtigung, Partner Center eigene Produkte oder Dienste zu erwerben.](give-customers-permission.md)
