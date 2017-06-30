---
title: "Hinzufügen eines Zero Touch-Bereitstellungsprofils zur Vereinfachung der Geräteeinrichtung mit Windows Autopilot | Partner Center"
description: "Hinzufügen eines Zero Touch-Bereitstellungsprofils in Partner Center zur Vereinfachung der Geräteeinrichtung mit Windows Autopilot"
author: KPacquer
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, ZTD, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: c51d9204b352b548a4095e96944aacdbcde97fa2
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/19/2017
---
# <a name="add-a-zero-touch-deployment-profile-to-simplify-device-setup-with-windows-autopilot"></a>Hinzufügen eines Zero Touch-Bereitstellungsprofils zur Vereinfachung der Geräteeinrichtung mit Windows Autopilot

Windows Autopilot kann die Geräteeinrichtung für neue Windows10 Pro-Geräte vom ersten Start in nur wenigen Schritten optimieren und sichern. 

## <a name="features"></a>Features

*  **Deaktivieren der lokalen Administratorberechtigungen** für die Endbenutzer, die Geräte einrichten
*  **Anzeigen einer Anmeldeseite für die Organisation**. Die Organisation kann eine Anmeldeseite vordefinieren, die das Gerät als ein Gerät für die Arbeit hinzufügt und es mit Azure Active Directory verknüpft.
*  **Registrieren Sie das Gerät in einer MDM**, z.B. Microsoft Intune, nachdem die Windows-Willkommensseite abgeschlossen ist.
*  **Optimieren Sie die Windows-Willkommensseite**, um nur die erforderlichen Schritteund Entscheidungen zu verwenden, mithilfe eines ZTD-Profils (Zero-Touch Deployment, berührungslose Bereitstellung). 

## <a name="requirements"></a>Anforderungen

*  Geräte, auf denen Windows 10 Pro Creators Update (mind. Version 1703) installiert ist
*  Geräte-ID, die als Hardwarehash (128 HWH oder 4k HWH) bezeichnet wird und in der Regel von einem OEM bereitgestellt wird. Sie verwenden IDs, um Organisationsprofile im Partner Center zuzuweisen.
*  Die Geräte müssen Zugriff auf das Internet haben. Wenn das Gerät keine Verbindung herstellen kann, zeigt es die standardmäßigen Bildschirme der Windows-Willkommensseite an.
*  Die Registrierung des Geräts in einer MDM erfordert Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Hinzufügen von Organisationsanmeldeseiten zur Windows-Willkommensseite

Um unternehmensspezifische Seiten hinzuzufügen, fügen Sie die Geräte dem [Azure AD-Verzeichnis](https://go.microsoft.com/fwlink/?linkid=848958) Ihrer Organisation hinzu und erstellen Anmeldeseiten.


## <a name="remove--windows-pages-from-oobe-with-a-zero-touch-deployment-ztd-profile"></a>Entfernen Sie Windows-Seiten von der Windows-Willkommensseite mit einem ZTD-Profil (Zero-Touch Deployment)

### <a name="examples-of-settings-in-a-ztd-profile"></a>Beispiele für Einstellungen in einem ZTD-Profil
*  Überspringen der Datenschutzeinstellungen im Setup
*  Deaktivieren des lokalen Administratorkontos während des Setups
*  Automatisches Überspringen von Seiten im Setup
   *  Automatisches Auswählen des Setups für die Arbeit oder Schule
   *  Überspringen der Cortana-, OneDrive- und OEM-Registrierungssetupseiten

### <a name="add-devices-and-apply-a-profile"></a>Hinzufügen von Geräten und Anwenden eines Profils

In Partner Center können Sie ein ZTD-Profil erstellen und auf eine Liste der Geräte anwenden.

Laden Sie zum Konfigurieren von Geräten eine Liste der Geräte in Partner Center hoch, erstellen Sie ein Profil, das für die Geräte gilt, und wenden Sie es an.

1.  Fügen Sie die Liste der Geräte in Partner Center hinzu. (Verkaufsvertreter und und Admin-Agents haben Zugriff, um die Liste der Geräte in Partner Center hinzuzufügen.)

    a.  Bitten Sie Ihren OEM um eine CSV-Datei, die die neuen Geräte aufführt. Diese Datei enthält die Seriennummer, Produkt-ID und die Geräte-ID, die vom OEM Activation 3.0-Tool generiert wurden. 

    b.  Navigieren Sie über das Partner Center-Dashboard zu **Kunden**. Wählen Sie den Kunden aus, der die Geräte erhält, und navigieren Sie zu **Geräte > Geräte hinzufügen**.

    c.  Geben Sie der Gerätegruppe einen Namen, z.B. "PCs der Contoso-Vertriebsabteilung – Bestellung April 2017". 

    d.  Klicken Sie auf **Durchsuchen** > Geräteinformationsdatei auswählen > **Überprüfen**.

2.  Erstellen Sie ein Profil, das Sie auf die Geräte anwenden können. (Nur Admin-Agents haben Zugriff zum Erstellen und Anwenden von Profilen in Partner Center.)

    a.  Klicken Sie unter **Geräte** auf **Neues Profil hinzufügen**.

    b.  Benennen Sie das Profil, z.B. "Contoso-Desktopprofil – Gesamte Windows-Willkommensseite überspringen".

    c.  Konfigurieren Sie die Einstellungen der Windows-Willkommensseite. Aktivieren Sie z.B. **Skip Express Settings in setup**.

    d.  Klicken Sie auf **Übermitteln**.

3.  Wenden Sie das Profil an.

    a.  Wählen Sie unter **Geräte** im Bereich **Assign and delete devices** die Geräte aus, die Sie konfigurieren möchten. Um eine gesamte Gruppe auszuwählen, aktivieren Sie das Kontrollkästchen neben dem Gruppennamen (z.B. "PCs der Contoso-Vertriebsabteilung – Bestellung März 2017").

    b.  Klicken Sie auf **Apply profile**, und wählen Sie das Profil (z.B. "Contoso-Desktopprofil – Gesamte Windows-Willkommensseite überspringen") aus. Die Geräte zeigen das Profil in der Spalte Profil an.

4.  Optional: Überprüfen Sie, ob Ihr Profil funktioniert.

    a.  Schließen Sie ein Gerät an das Netzwerk an, und schalten Sie es ein.

    b.  Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.

    c.  Um das Gerät für einen neuen Benutzer vorzubereiten, schließen Sie die Windows-Willkommensseite ab, und setzen Sie das Gerät auf die werksseitigen Standardeinstellungen zurück.


## <a name="to-update-or-delete-a-profile"></a>So aktualisieren oder löschen Sie ein Profil 

Nachdem Sie ein Profil einem Gerät zugeordnet haben, können Sie es aktualisieren, auch wenn Sie das Gerät bereits an den Kunden übergeben haben. Wenn das Gerät mit dem Internet verbunden ist, lädt es die neueste Version Ihres Profils während des Prozesses der Windows-Willkommensseite herunter. Wenn der Kunde das Gerät auf die werksseitigen Standardeinstellungen wiederherstellt, lädt das Gerät erneut die neuesten Updates an Ihrem Profil herunter. 

###<a name="you-can-remove-a-profile-from-a-device"></a>Sie können ein Profil von einem Gerät entfernen.
1. Wählen Sie das Gerät (oder die Gruppe von Geräten), von dem Sie das Profil entfernen möchten. 

2. Wählen Sie unter **Assign and delete devices** die Option **Profil entfernen**.

3. Wechseln Sie zu dem Profil, das Sie entfernen möchten, und löschen Sie es. Das Profil wird von allen Geräten gelöscht.


Wählen Sie unter **Geräte** das Profil aus. Von hier aus können Sie die vorhandenen Einstellungen ändern.

