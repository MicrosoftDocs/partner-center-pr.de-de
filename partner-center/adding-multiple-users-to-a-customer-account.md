---
title: Hinzufügen mehrerer Benutzer für ein Kundenkonto
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wenn Sie dem Konto eines Kunden mehrere Benutzer hinzufügen möchten, laden Sie mithilfe des CSV-Datei Formats (Comma-Separated Value, CSV) eine Datendatei in das Partner Center hoch.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535740"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Hochladen einer CSV-Datei von Benutzern in das Konto eines Kunden


**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator

Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in das Partner Center hochladen. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Erstellen der Datei von Kunden Benutzern und Hochladen in das Kundenkonto

1. Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können. Weitere Informationen finden [Sie Unterfelder für CSV-Datei, um mehrere Benutzer für ein Kundenkonto zu importieren](file-customer-users.md). 

2. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

3. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

4. Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen**aus.

5. Wählen Sie unter **Upload user info** die Option **Durchsuchen**.

6. Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.

7. Wählen Sie **Überprüfen** aus.

    **Hinweis**    Die meisten Fehler bei der Kontoerstellung werden durch Probleme mit der Datendatei verursacht, darunter fehlende Informationen, falsch formatierte oder doppelte e-Mail-Adressen oder zu viele Datensätze in der Datei.

8. Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.
9. Wählen Sie **Speichern** aus.
10. Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.

    >[!IMPORTANT]
    > Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, weil dies später nicht mehr möglich ist. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

11. Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen. 

## <a name="next-steps"></a>Nächste Schritte

- [Erteilen Sie Kunden eine Berechtigung im Partner Center, um Ihre eigenen Produkte oder Dienste zu erwerben.](give-customers-permission.md)
