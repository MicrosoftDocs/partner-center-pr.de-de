---
title: Anpassen des Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen | Partner Center
description: Vorkonfigurieren eines Geräts Out-of-Box-Experience mit Autopilot-Profilen.
author: maggiepuccievans
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 70740212f433ad6eb4f2f04d63708fff436024ad
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995934"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Anpassen des Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen

**Betrifft:**

- CSP-Rechnung Direct-Partner, indirekte Anbieter und indirekte Wiederverkäufer

Wenn Sie Kundengeräte verwalten, müssen Sie die Out-of-Box-Experience (OOBE) für Benutzer des Kunden anpassen. Sie können neue Geräte mit Windows Autopilot-Profilen vorab zu konfigurieren, bevor Sie die Geräte an Kunden liefern und Anwenden von neuen Profilen auf Geräte, die Kunden bereits erworben haben. In diesem Artikel wird erläutert, wie Sie erstellen und Anwenden von Autopilot-Profilen auf Geräte in Partner Center.

Wenn Sie nicht bereits mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:

- [Übersicht über Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot-Referenz-Bereitstellungshandbuch](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Übersicht

Mit dem Windows Autopilot-Feature im Partner Center können Sie benutzerdefinierte Profile für Kundengeräte erstellen. Zum Zeitpunkt der Veröffentlichung dieses Artikels, waren die folgenden profileinstellungen verfügbar:

- Überspringen Sie datenschutzeinstellungen. Dieser optionalen Einstellung der Autopilot-Profil kann Organisationen während des Prozesses der Windows-Willkommensseite nicht zu Datenschutz und Fragen.

- Deaktivieren Sie die Erstellung des lokalen Administratorkontos auf dem Gerät. Organisationen können entscheiden, ob der Benutzer das Gerät einrichten Administratorzugriff haben soll, nachdem der Vorgang abgeschlossen ist.

- Automatisch Gerät für die Arbeit oder Schule einrichten. Alle Geräte mit Autopilot registriert werden automatisch als Arbeit betrachtet werden oder Geräte, Schule, damit diese Frage nicht während der OOBE-Prozesses aufgefordert wird.

- Überspringen Sie Cortana-, Onedrive- und OEM-registrierungssetupseiten. Alle Geräte mit Autopilot registriert werden automatisch diese Seiten während des Out-of-Box-Experience (OOBE) zu überspringen.

- Überspringen Sie Endbenutzer-Lizenzvertrag (EULA). Ab Windows 10, Version 1709, können Organisationen entscheiden, überspringen die Endbenutzer-Lizenzvertrag-Seite, die bei der Windows-Willkommensseite angezeigt. Finden Sie unter [EULA zu Windows Autopilot](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Endbenutzer-Lizenzvertrag Seite während des Windows Setup berücksichtigen.

Wenden Sie die folgenden Profil und Geräte-Management-Berechtigungen und Einschränkungen:

- CSP-Partner können weiterhin zum Verwalten von Autopilot Profile für vorhandene Kunden, mit denen sie Reseller-Geschäftsbeziehungen haben, auch wenn die Kunden die delegierten Administratorrechte des Partners entfernt haben.

- Sie können vorhandene Geräte für Ihre Kunden verwalten, die von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.

- Sie können keine Geräte verwalten, die Microsoft Store für Unternehmen oder Microsoft Intune-Portal Ihr Kunde hochgeladen hat.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Erstellen Sie und Verwalten von Autopilot-Profilen in Partner Center

Im Partner Center können Sie Windows Autopilot-bereitstellungsprofile erstellen und diese auf Geräte anzuwenden.

>[!NOTE]
>Nur Admin-Agents können erstellen und Anwenden von Profilen.

### <a name="create-a-new-autopilot-profile"></a>Erstellen Sie ein neues Autopilot-Profil

1. Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, die, dem Sie für die Autopilot-Bereitstellungsprofil erstellen.

2. Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.

3. Wählen Sie unter **Windows Autopilot Profile** **Neues Profil hinzufügen**.

4. Geben Sie Namen und eine Beschreibung des Profils, und konfigurieren Sie die Einstellungen für die Windows-Willkommensseite. Wählen Sie aus:  

   - Überspringen der datenschutzeinstellungen im setup

   - Deaktivieren des lokalen Administratorkontos während des Setups
  
   - Automatisches Überspringen von Seiten im Setup<br>
        (Einschließlich *Automatisches Setup für Arbeit oder Schule auswählen* und *Überspringen Cortana, OneDrive und OEM-registrierungssetupseiten*)
  
   - Endbenutzer-Lizenzvertrag (EULA) überspringen<br> 
       >[!IMPORTANT] 
       >Finden Sie unter [EULA zu Windows Autopilot](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Endbenutzer-Lizenzvertrag Seite während des Windows Setup berücksichtigen.

5. Wählen Sie abschließend **Übermitteln** aus.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Anwenden einer Autopilot-Profilen auf Kundengeräte

>[!NOTE]
>Die folgenden Anweisungen wird davon ausgegangen, dass Sie bereits Geräte des Kunden in das Partner Center hinzugefügt haben, und Sie ihre Liste der Geräte zugreifen können. Wenn Sie Geräte des Kunden bereits hinzugefügt haben, folgen Sie den Anweisungen im [Konto eines Kunden Geräte hinzufügen](#add-devices-to-a-customers-account) , und führen Sie dann die folgenden Schritte aus.

Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es an den Kunden Geräte anwenden.

1. Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, die, dem Sie für die Autopilot-Profil erstellt.

2. Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.

3. Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte oder Gerätegruppen, die Sie Profile für, und wählen Sie dann **Profil anwenden**möchten. Das Profil, das Sie nur angewendet, die in der Spalte **Profil** wird angezeigt.

4. Gehen Sie folgendermaßen vor, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet werden.

    a.  Verbinden Sie ein Gerät mit dem Netzwerk, und schalten Sie es ein.

    b.  Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.

    c.  Wenn der OOBE-Prozess beendet wird, wird zurücksetzen Sie das Gerät auf die werksseitigen Standardeinstellungen, die sie für einen neuen Benutzer vorzubereiten.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Entfernen Sie ein Autopilot-Profil aus dem Gerät eines Kunden

1. Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, die, dem Sie für die Autopilot-Profil erstellt.

2. Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.

3. Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte, die Sie verwenden möchten, entfernen Sie das Profil aus, und wählen Sie dann **Entfernen eines Profils**.

   >[!NOTE]
   >Entfernen eines Profils von einem Gerät wird nicht das Profil aus der Liste gelöscht. Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualisieren Sie oder löschen Sie ein Autopilot-Profil

Wenn ein Kunde die Out-of-Box-Experience zu ändern möchte, nachdem Sie die Geräte geliefert haben, können Sie das Profil in Partner Center ändern.

Wenn das Gerät des Kunden mit dem Internet verbunden ist, wird es die neueste Version der Profile herunterladen, während der Windows-Willkommensseite. Außerdem wird jedes Mal ein Kunde ein Gerät auf die werksseitigen Standardeinstellungen wiederherstellt das Gerät erneut herunter die neueste Version der Profile während des Prozesses der Windows-Willkommensseite.

1. Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, der Sie ein Autopilot-Profil zu ändern möchten.

2. Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.

3. Wählen Sie unter **Windows Autopilot Profile** das Profil, das Sie aktualisieren müssen. Nehmen Sie die erforderlichen Änderungen vor, und wählen Sie dann **übermitteln**.

Wählen Sie aus der oberen rechten Ecke der Seite **Profil löschen** , um diesem Profil zu löschen.

### <a name="add-devices-to-a-customers-account"></a>Hinzufügen von Geräten auf dem Konto eines Kunden

>[!NOTE]
>Verkaufsvertreter und Admin-Agents können Geräte Konto eines Kunden hinzufügen.

Bevor Sie benutzerdefinierte Autopilot Profile auf Kundengeräte anwenden können, müssen Sie auf dem Gerät der Kundenliste zugreifen können.

Wenn Sie die OEM-Namen, Seriennummer und Modell Kombination verwenden möchten, achten Sie darauf, dass Sie diese Einschränkungen:

- Das Tupel funktioniert nur für neue Geräte (4 k Hashes, z. B.) und wird für 128b Hashes (RS2 und vorherigen Geräte) nicht unterstützt.

- Die Registrierung Tupel ist groß-und Kleinschreibung unterschieden, damit die Daten in der Datei der Hersteller und Modell Namen ***genau*** entsprechen müssen, wie durch den OEM-Anbieter (Hardwareanbieter) bereitgestellt.

Führen Sie die folgenden Anweisungen von Geräten auf dem Konto eines Kunden im Partner Center.

1. Wählen Sie **Kunden** im Partner Center, und wählen Sie dann den Kunden, deren Geräte, die Sie verwalten möchten.

2. Wählen Sie auf der Detailseite des Kunden die **Geräte aus**.

3. Wählen Sie unter **Anwenden von Profilen auf Geräte** **Geräte hinzufügen**.

4. Geben Sie einen Namen für die Liste der Geräte, und wählen Sie dann die Kundenliste (im CSV-Format) für das Partner Center hochladen **Durchsuchen** .

    >[!NOTE]
    >Sie sollten diese CSV-Datei mit dem Gerät Kauf erhalten haben. Wenn Sie eine CSV-Datei nicht erhalten haben, können Sie selbst erstellen, mithilfe der Schritte im [Windows Autopilot-Geräte hinzufügen](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Laden Sie die CSV-Datei, und wählen Sie dann **Speichern**.

Wenn Sie eine Fehlermeldung erhalten, bei dem Versuch, die CSV-Datei hochzuladen, überprüfen Sie das Format der Datei. Sie können nur den Hardwarehash oder den OEM-Namen, Seriennummer, und Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID. Die Beispiel-CSV-Datei über den Link neben **Hinzufügen Geräte** bereitgestellt können auch um eine Liste der Geräte zu erstellen.

## <a name="windows-autopilot-eula-dismissal"></a>EULA zu Windows Autopilot

### <a name="important-information"></a>WICHTIGE INFORMATIONEN

Windows Autopilot können Sie benutzerdefinierte Installationen von Windows auf Geräten zu konfigurieren, die Sie für Ihre Kunden verwalten. Wenn dazu berechtigt, durch den Kunden, können Sie unterdrücken oder ausblenden bestimmte Setupbildschirme, die normalerweise für Benutzer beim Einrichten von Windows, einschließlich des Endbenutzer-Lizenzvertrag (End User License Agreement) Annahme Bildschirms angezeigt werden.

Durch die Verwendung dieser Funktion stimmen Sie, dass das unterdrücken oder Ausblenden von Bildschirmen, die Benutzer bereitstellen, oder die Annahme von Begriffe bedeutet, dass Sie über ausreichende Zustimmung und Autorisierung von ausblenden Begriffe und, die Sie für Ihre Kunden erworben haben Ihre Kunden (gibt an, ob eine Organisation oder einzelner Benutzer die Groß-/Kleinschreibung), stimmen hinweisen und akzeptiert Begriffe, die an den Kunden relevant sind. Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten. Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.