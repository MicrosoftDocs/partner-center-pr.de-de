---
title: Anpassen der Windows-Willkommensseite eines Geräts mit Windows Autopilot-Profilen | Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie die Out-of-Box-Benutzerfreundlichkeit eines neuen Geräts mit Autopilot-Profilen anpassen oder vorab konfigurieren, bevor Sie das Gerät an den Kunden übermitteln.
author: jasonwhowell
ms.author: jasonh
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Willkommensseite
ms.localizationpriority: medium
ms.openlocfilehash: c69b61256e19fd3a8becbfd546fd5b9a0b54654f
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390999"
---
# <a name="customize-the-out-of-box-experience-for-a-device-with-windows-autopilot-profiles"></a>Anpassen der Out-of-Box-Darstellung für ein Gerät mit Windows Autopilot-Profilen

**Gilt für:**

- CSP-Partner mit Direktfakturierung, indirekte Anbieter und indirekte Vertriebspartner

**Geeignete Rollen**

- Administratoragent
- Globaler Administrator
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

Wenn Sie Kundengeräte verwalten, müssen Sie die Windows-Willkommensseite für die Benutzer des Kunden anpassen. Sie können neue Geräte mit Windows Autopilot-Profilen vorkonfigurieren, bevor Sie die Geräte an Kunden ausliefern, und neue Profile auf bereits erworbene Geräte anwenden. 

Beachten Sie, dass OEMs damit begonnen haben, eine Versand Bezeichnung auf der Außenseite des Autopilot-Geräts hinzufügen, die die **Product Key-ID (pkid)** des Geräts anzeigt.  Dieser eindimensionale, lesbare Barcode bietet downstreampartnern eine Möglichkeit, Geräte für Autopilot zu registrieren, ohne die Geräte zu entpacken und die Geräte-ID auf alternative Weise zu erfassen.

In diesem Artikel wird erläutert, wie Sie im Partner Center Autopilot-Profile erstellen und auf Geräte anwenden.

Wenn Sie noch nicht mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:

- [Übersicht über Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Referenzhandbuch für die Bereitstellung mit Autopilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Übersicht

Mit der Windows-Funktion Autopilot im Partner Center können Sie benutzerdefinierte Profile erstellen und diese auf Kundengeräte anwenden. Zum Zeitpunkt der Veröffentlichung dieses Artikels waren die folgenden Profileinstellungen verfügbar:

- Datenschutzeinstellungen überspringen. Diese optionale Einstellung im Autopilot-Profil ermöglicht Organisationen, auf Fragen zu Datenschutzeinstellungen auf der Windows-Willkommensseite zu verzichten.

- Erstellung des lokalen Administratorkontos auf dem Gerät deaktivieren. Organisationen können entscheiden, ob der Benutzer, der das Gerät einrichtet, nach Abschluss des Vorgangs Administratorrechte erhalten soll.

- Gerät automatisch für Arbeit oder Bildungseinrichtung einrichten. Alle mit Autopilot registrierten Geräte gelten automatisch als Arbeits- und Bildungseinrichtungsgeräte, weshalb diese Frage im zur Windows-Willkommensseite gehörigen Prozess nicht gestellt wird.

- Setupseiten für Cortana-, OneDrive- und OEM-Registrierung überspringen. Bei allen mit Autopilot registrierten Geräten werden diese Seiten im zur Windows-Willkommensseite gehörigen Prozess automatisch übersprungen.

- Lizenzbedingungen überspringen. Ab Windows 10 Version 1709 können Organisationen sich entscheiden, ob die im zur Windows-Willkommensseite gehörigen Prozess gezeigte Seite mit den Lizenzbedingungen übersprungen werden soll. Unter [Ablehnung der Lizenzbedingungen für Windows Autopilot](#windows-autopilot-eula-dismissal) finden Sie wichtige zu beachtende Informationen beim Überspringen der Seite mit den Lizenzbedingungen während des Setups von Windows.

Die folgenden Berechtigungen und Einschränkungen für die Verwaltung von Profilen und Geräten gelten:

- CSP-Partner können weiterhin die Autopilot-Profile für Bestandskunden mit Vertriebspartnerschaft verwalten, auch wenn die Kunden die Berechtigungen für die delegierte Verwaltung für den Partner aufgehoben haben.

- Sie können vorhandene Geräte für Ihre Kunden verwalten, die Sie hinzugefügt haben.

- Sie können keine Geräte verwalten, die Ihr Kunde in Microsoft Store für Unternehmen oder das Microsoft InTune Portal hochgeladen hat.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Erstellen und Verwalten von Autopilot-Profilen im Partner Center

Im Partner Center können Sie Windows Autopilot-Bereitstellungsprofile erstellen und auf Geräte anwenden.

>[!NOTE]
>Nur Administrator-Agents können Profile erstellen und anwenden.

### <a name="create-a-new-autopilot-profile"></a>Erstellen eines neuen Autopilot-Profils

1. Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellen.

2. Wählen Sie auf der Detailseite des Kunden **Geräte** aus.

3. Klicken Sie unter **Windows Autopilot-Profile** auf **Neues Profil hinzufügen**.

4. Geben Sie Namen und eine Beschreibung des Profils ein, und konfigurieren Sie dann die Einstellungen für die Windows-Willkommensseite. Es stehen folgende Optionen zur Auswahl:  

   - Datenschutzeinstellungen beim Setup überspringen

   - Deaktivieren des lokalen Administratorkontos während des Setups
  
   - Automatisches Überspringen von Seiten im Setup<br>
        (Schließt *Setup für Arbeit oder Bildungseinrichtung automatisch auswählen* und *Setupseiten für Cortana-, OneDrive- und OEM-Registrierung überspringen* ein)
  
   - Lizenzbedingungen überspringen.<br> 
       >[!IMPORTANT] 
       >Unter [Ablehnung der Lizenzbedingungen für Windows Autopilot](#windows-autopilot-eula-dismissal) finden Sie wichtige zu beachtende Informationen beim Überspringen der Seite mit den Lizenzbedingungen während des Setups von Windows.

5. Wählen Sie abschließend **Übermitteln** aus.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Anwenden eines Autopilot-Profils auf Kundengeräte

>[!NOTE]
>Die folgenden Anweisungen gehen davon aus, dass Sie die Geräte des Kunden bereits dem Partner Center hinzugefügt haben und dass Sie auf dessen Geräteliste zugreifen können. Wenn Sie die Geräte des Kunden noch nicht hinzugefügt haben, folgen Sie den Anweisungen unter [Hinzufügen von Geräten zu einem Kundenkonto](#add-devices-to-a-customers-account), und führen Sie dann die folgenden Schritte aus.

Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es auf die Geräte des Kunden anwenden.

1. Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellt haben.

2. Wählen Sie auf der Detailseite des Kunden **Geräte** aus.

3. Wählen Sie unter **Profile auf Geräte anwenden** die Geräte oder Gerätegruppen aus, denen Sie Profile hinzufügen möchten, und klicken Sie dann auf **Profil anwenden**. Das Profil, das Sie soeben angewendet haben, wird in der Spalte **Profil** angezeigt.

4. Führen Sie die folgenden Schritte aus, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet wird.

    a.  Schließen Sie ein Gerät an das Netzwerk an, und schalten Sie es ein.

    b.  Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.

    c.  Wenn der zur Windows-Willkommensseite gehörige Prozess beendet ist, setzen Sie das Gerät auf die Werkseinstellungen zurück, um es für einen neuen Benutzer vorzubereiten.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Entfernen eines Autopilot-Profils von einem Kundengerät

1. Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, für den Sie das Autopilot-Profil erstellt haben.

2. Wählen Sie auf der Detailseite des Kunden **Geräte** aus.

3. Wählen Sie unter **Profile auf Geräte anwenden** die Geräte aus, von denen Sie das Profil entfernen möchten, und klicken Sie dann auf **Profil entfernen**.

   >[!NOTE]
   >Wenn Sie ein Profil von einem Gerät entfernen, wird das Profil nicht aus Ihrer Liste gelöscht. Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen unter [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualisieren oder Löschen eines AutoPilot-Profils

Wenn ein Kunde die Windows-Willkommensseite ändern möchte, nachdem Sie ihm Geräte geliefert haben, können Sie das Profil im Partner Center ändern.

Wenn sich das Gerät des Kunden mit dem Internet verbindet, wird während des zur Windows-Willkommensseite gehörigen Prozesses die neueste Profilversion heruntergeladen. Außerdem lädt das Gerät jedes Mal, wenn ein Kunde ein Gerät auf die Werkseinstellungen zurücksetzt, während des zur Windows-Willkommensseite gehörigen Prozesses erneut die neueste Profilversion herunter.

1. Wählen Sie **Kunden** im Menü „Partner Center“ und dann den Kunden aus, dessen Autopilot-Profil Sie ändern sollen.

2. Wählen Sie auf der Detailseite des Kunden **Geräte** aus.

3. Wählen Sie unter **Windows Autopilot-Profile** das Profil aus, das Sie aktualisieren müssen. Nehmen Sie die erforderlichen Änderungen vor, und klicken Sie dann auf **Senden**.

Um dieses Profil zu löschen, klicken Sie rechts oben auf der Seite auf **Profil löschen**.

### <a name="add-devices-to-a-customers-account"></a>Hinzufügen von Geräten zum Kundenkonto

>[!NOTE]
>Vertriebs- und Verwaltungsmitarbeiter können dem Konto eines Kunden Geräte hinzufügen.

Bevor Sie benutzerdefinierte Autopilot-Profile auf Kundengeräten anwenden können, müssen Sie Zugriff auf die Geräteliste des Kunden haben.

Wenn Sie planen, die Kombination aus OEM-Name, Seriennummer und Modell zu verwenden, beachten Sie diese Einschränkungen:

- Dieses Tupel funktioniert nur für neuere Geräte (z.B. 4K-Hashes) und wird für 128B-Hashes (RS2 und frühere Geräte) nicht unterstützt.

- Bei der Registrierung des Tupels wird zwischen Groß- und Kleinschreibung unterschieden. Daher müssen die Daten in der Datei mit den Modell- und Herstellernamen ***genau*** mit den Angaben des OEM-Anbieters (Hardwareanbieters) übereinstimmen.

Führen Sie die im Partner Center nachstehenden Anweisungen zum Hinzufügen von Geräten zum Konto eines Kunden aus.

1. Wählen Sie im Partner Center-Menü **Kunden** und dann den Kunden aus, dessen Geräte Sie verwalten möchten.

2. Wählen Sie auf der Detailseite des Kunden **Geräte** aus.

3. Klicken Sie unter **Profile auf Geräte anwenden**  auf **Geräte hinzufügen**.

4. Geben Sie einen Namen für die Geräteliste aus, und klicken Sie dann auf **Durchsuchen**, um die Kundenliste (im Dateiformat CSV) ins Partner Center hochzuladen.

    >[!NOTE]
    >Beim Kauf Ihres Geräts sollten Sie diese CSV-Datei erhalten haben. Wenn Sie keine CSV-Datei erhalten haben, können Sie selbst eine erstellen, indem Sie die Schritte unter [Hinzufügen von Geräten zu Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell) ausführen.  

5. Laden Sie die CSV-Datei hoch, und klicken Sie dann auf **Speichern**.

Wenn Sie beim Versuch, die CSV-Datei hochzuladen, eine Fehlermeldung erhalten, überprüfen Sie das Format der Datei. Sie können nur den Hardwarehash oder den OEM-Namen, die Seriennummer und das Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID verwenden. Sie können auch die CSV-Beispieldatei verwenden, die über den Link neben **Geräte hinzufügen** bereitgestellt wird, um eine Geräteliste zu erstellen.

Die CSV-Datei sollte in etwa wie folgt aussehen:

> **Seriennummer des Geräts, Windows-Produkt-ID, Hardware Hash, Herstellername, Gerätemodell**

> **{SerialNumber},,, Microsoft Corporation, Surface Laptop**

Beachten Sie, dass bei "Herstellername" und "Gerätemodell" die Groß-/Kleinschreibung beachtet wird.

Wenn Sie nicht wissen, welchen Wert Sie für Herstellername und Gerätemodell benötigen, können Sie diesen auf dem Gerät ausführen, um die richtigen Werte zu erfassen:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Ablehnung der Lizenzbedingungen für Windows Autopilot

### <a name="important-information"></a>WICHTIGE INFORMATIONEN

Mit Windows Autopilot können Sie angepasste Installationen von Windows auf Geräten konfigurieren, die Sie für Ihre Kunden verwalten. Wenn Sie vom Kunden entsprechend autorisiert wurden, können Sie bestimmte Setupbildschirme unterdrücken oder ausblenden, die Benutzern normalerweise beim Einrichten von Windows angezeigt werden, darunter der Bildschirm für das Annehmen der Lizenzbedingungen.

Mit der Nutzung dieser Funktion erklären Sie sich damit einverstanden, dass das Unterdrücken oder Ausblenden von Bildschirmen, die dazu bestimmt sind, den Benutzern eine Benachrichtigung oder Akzeptanz von Bedingungen zu ermöglichen, bedeutet, dass Sie von Ihrem Kunden eine ausreichende Zustimmung und Berechtigung erhalten haben, Bedingungen zu verbergen, und dass Sie im Namen Ihres Kunden (unabhängig davon, ob es sich um ein Unternehmen oder einen einzelnen Benutzer handelt) allen Benachrichtigungen zustimmen und alle Bedingungen akzeptieren, die für Ihren Kunden gelten. Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten. Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.
