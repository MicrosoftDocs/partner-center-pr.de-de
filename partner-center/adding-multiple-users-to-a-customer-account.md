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
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474188"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Hochladen einer CSV-Datei von Benutzern in das Konto eines Kunden


**Geeignete Rollen**

- Globaler Administrator

Fügen Sie dem Konto eines Kunden mehrere Benutzer gleichzeitig hinzu, indem Sie eine Datendatei im CSV-Dateiformat (Comma-Separated Value File Format) in das Partner Center hochladen. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Erstellen der Datei von Kunden Benutzern und Hochladen in das Kundenkonto

1. Erstellen Sie eine durch Trennzeichen getrennte Datendatei (.csv) mit den oben beschriebenen Daten. Speichern Sie die Datei, sodass Sie in einem späteren Schritt zu dieser Datei navigieren können. Weitere Informationen finden [Sie Unterfelder für CSV-Datei, um mehrere Benutzer für ein Kundenkonto zu importieren](file-customer-users.md). 

2. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.

3. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.

4. Wählen Sie die Registerkarte **Benutzer und Lizenzen** des Kunden aus, und wählen Sie dann **Benutzer hochladen** aus.

5. Wählen Sie unter **Upload user info** die Option **Durchsuchen**.

6. Wählen Sie in der Dateiauswahl Ihre Datendatei aus, und klicken Sie dann auf **Öffnen**.

7. Wählen Sie **Überprüfen** aus.

    **Hinweis:** Der Großteil der Fehler bei der Kontoerstellung wird durch Datendateifehler verursacht, beispielsweise durch fehlende Informationen, falsch formatierte oder doppelte E-Mail-Adressen oder eine zu große Anzahl von Datensätzen in einer Datei.

8. Wählen Sie nach der Überprüfung der Datei durch das Partner Center den geografischen **Standort** für die neuen Benutzer aus.
9. Wählen Sie **Speichern** aus.
10. Laden Sie die Informationen zu den temporären Kennwörtern für die Benutzer herunter.

    >[!IMPORTANT]
    > Laden Sie die Datei mit den temporären Kennwörtern unbedingt jetzt herunter, weil dies später nicht mehr möglich ist. Neue Benutzer müssen sich mit dem temporären Kennwort für die neuen Konten beim neuen Konto anmelden.

11. Neuen Benutzern werden automatisch die Berechtigungen **Kann Lizenzen und Dienste nutzen** zugewiesen. 

## <a name="next-steps"></a>Nächste Schritte

- [Erteilen Sie Kunden eine Berechtigung im Partner Center, um Ihre eigenen Produkte oder Dienste zu erwerben.](give-customers-permission.md)
