---
title: Anpassen eines Geräts Out-of-Box-Erfahrung mit Windows Autopilot-Profile | Partner Center
description: Konfigurieren eines Geräts Out-of-Box-Experience mit Autopilot-Profile.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero Touch-Bereitstellung, Oobe, Anmeldung Bildschirme, Out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586913"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Anpassen eines Geräts Out-of-Box-Erfahrung mit Windows Autopilot-Profile

**Gilt für**

- Direkt vor kurzem verstorbenen Bill CSP-Partner, indirekte Anbieter und indirekten Vertriebspartner

Wenn Sie die Customer-Geräte verwalten, müssen Sie die Out-of-Box-Experience (OOBE) für den Kunden eines Benutzers anpassen. Sie können neue Geräte mit Windows Autopilot-Profile vorkonfigurieren, bevor die Bereitstellung von Geräten für Kunden, und wenden neue Profile für Geräte, die Kunden bereits gekauft haben. In diesem Artikel wird erläutert, wie zum Erstellen und Anwenden von Autopilot-Profile für Geräte im Partner Center wird.

Wenn Sie nicht bereits mit Autopilot vertraut sind, überprüfen Sie die Informationen in den folgenden Artikeln:

- [Übersicht über Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot Deployment-Referenzhandbuch](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Übersicht

Mit dem Windows Autopilot-Feature im Partner Center können Sie benutzerdefinierte Profile gelten für Kundengeräte erstellen. Die folgenden profileinstellungen, waren zum Zeitpunkt der Veröffentlichung dieses Artikels verfügbar:

- Überspringen Sie die datenschutzeinstellungen. Diese optionale Einstellung des Autopilot-Profil kann Organisationen nicht während des OOBE-Prozesses zu datenschutzeinstellungen zu stellen.

- Deaktivieren Sie die Erstellung des Kontos Lokaler Administrator auf dem Gerät. Organisationen können entscheiden, ob der Benutzer, die zum Einrichten des Geräts Administratorzugriff erhalten soll, sobald der Vorgang abgeschlossen ist.

- Richten Sie automatisch Geräte für Geschäfts-, Schul- oder unikonto ein. Alle Autopilot registrierten Geräte automatisch betrachtet Arbeit oder Schule Geräte aus, damit diese Frage nicht während des OOBE-Prozesses aufgefordert werden.

- Skip Cortana, OneDrive und OEM-Setup Registrierungsseiten. Alle Autopilot registrierten Geräte werden auf diesen Seiten automatisch bei der Out-of-Box-Experience (OOBE) übersprungen werden.

- Überspringen Sie die Endbenutzer-Lizenzvertrag (EULA). Ab Windows 10 Version 1709, können Organisationen entscheiden, um die EULA-Seite angezeigt, die während des OOBE-Prozesses zu überspringen. Finden Sie unter [Windows Autopilot-Endbenutzer-Lizenzvertrag Kündigung](#windows-autopilot-eula-dismissal) unten für wichtige Informationen, die über die Seite "LIZENZBEDINGUNGEN" wird übersprungen, während Windows einrichten.

Die folgenden Profile und Device Management-Berechtigungen und Einschränkungen gelten:

- CSP-Partner können weiterhin zum Verwalten von Autopilot-Profile für bestehende Kunden, mit denen sie Reseller Beziehungen haben, auch wenn Kunden die delegierte Administration Berechtigungen des Partners entfernt haben.

- Sie können ein vorhandenes Gerät für Ihre Kunden verwalten, die von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.

- Sie können keine Geräte verwalten, die Ihren Kunden zu Microsoft Store für Unternehmen oder das Microsoft Intune-Portal hochgeladen wurde.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Erstellen und Verwalten von Autopilot-Profile im Partner Center

Im Partner Center können Sie Windows Autopilot-bereitstellungsprofile erstellen und auf Geräte anwenden.

>[!NOTE]
>Nur Administrator-Agents erstellen und Anwenden von Profilen.

### <a name="create-a-new-autopilot-profile"></a>Erstellen eines neuen Autopilot-Profils

1. Wählen Sie **Kunden** aus dem Partner Center-Menü und wählen Sie dann den Kunden Sie erstellen das Autopilot-Profil für.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Klicken Sie unter **Windows Autopilot-Profile** wählen **neues Profil hinzufügen**.

4. Geben Sie Namen und eine Beschreibung des Profils, und klicken Sie dann konfigurieren Sie die OOBE-Einstellungen zu. Es stehen folgende Optionen zur Auswahl:  

   - Datenschutzeinstellungen für in-Setup überspringen

   - Deaktivieren des lokalen Administratorkontos während des Setups
  
   - Automatisches Überspringen von Seiten im Setup<br>
        (Umfasst *automatisch auswählen des Setupprogramms für Geschäfts-, Schul- oder unikonto* und *Skip Cortana, OneDrive und OEM-Setup Registrierungsseiten*)
  
   - Endbenutzer-Lizenzvertrag (EULA) überspringen<br> 
       >[!IMPORTANT] 
       >Finden Sie unter [Windows Autopilot-Endbenutzer-Lizenzvertrag Kündigung](#windows-autopilot-eula-dismissal) unten für wichtige Informationen, die über die Seite "LIZENZBEDINGUNGEN" wird übersprungen, während Windows einrichten.

5. Wählen Sie abschließend **Übermitteln** aus.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Ein Autopilot-Profil auf kundengeräten anwenden

>[!NOTE]
>Die folgenden Anweisungen wird davon ausgegangen, dass Sie bereits des Kunden Geräte zum Partner Center hinzugefügt haben und Sie ihre Geräteliste zugreifen können. Falls Sie bereits die Kunden-Geräte hinzugefügt haben, befolgen Sie die Anweisungen in [Geräte hinzufügen, um ein Kundenkonto](#add-devices-to-a-customers-account) und befolgen Sie dann die folgenden Schritte aus.

Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es an den Kunden Geräte anwenden.

1. Wählen Sie **Kunden** über das Partner Center-Menü, und wählen Sie dann den Kunden Sie erstellt haben das Autopilot-Profil für.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Klicken Sie unter **gelten Profile für Geräte** wählen Sie die Geräte oder Gerätegruppen, die Sie verwenden möchten, Hinzufügen von Profilen, und wählen Sie dann **Profil anwenden**. Das Profil, das Sie soeben angewendet wird, der **Profil** Spalte.

4. Gehen Sie folgendermaßen vor, um sicherzustellen, dass das Profil wird erfolgreich an das Gerät angewendet werden.

    a.  Verbinden Sie ein Gerät mit dem Netzwerk, und aktivieren Sie ihn.

    b.  Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.

    c.  Wenn Sie den OOBE-Prozess beendet wird, Zurücksetzen des Geräts, auf die werkseitigen Standardeinstellungen für die vorzubereitende für einen neuen Benutzer.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Entfernen Sie ein Autopilot-Profil von einem Kunden-Gerät

1. Wählen Sie **Kunden** über das Partner Center-Menü, und wählen Sie dann den Kunden Sie erstellt haben das Autopilot-Profil für.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Klicken Sie unter **gelten Profile für Geräte** wählen Sie die Geräte, die Sie verwenden möchten, entfernen Sie das Profil aus, und wählen Sie dann **Profil entfernen**.

   >[!NOTE]
   >Ein Profil von einem Gerät entfernen, wird das Profil nicht aus der Liste gelöscht. Wenn Sie ein Profil löschen möchten, befolgen Sie die Anweisungen in [Update- oder Delete ein Autopilot-Profil](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualisieren Sie oder löschen Sie ein Autopilot-Profil

Wenn ein Kunde die Out-of-Box-Experience zu ändern möchte, nachdem Sie die Geräte auf diese geliefert haben, können Sie das Profil im Partner Center ändern.

Wenn die das Gerät eines Kunden mit dem Internet verbunden ist, wird die aktuelle Profilversion während des OOBE-Prozesses heruntergeladen. Außerdem wird jedes Mal ein Kunde ein Gerät auf die werkseitigen Standardeinstellungen zurückgesetzt wird das Gerät erneut die neueste Profilversion während des OOBE-Prozesses herunterladen.

1. Wählen Sie **Kunden** aus dem Partner Center-Menü und wählen Sie dann den Kunden mit der Sie ein Autopilot-Profil ändern möchte.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Klicken Sie unter **Windows Autopilot-Profile** wählen Sie das Profil, das Sie aktualisieren müssen. Die erforderlichen Änderungen vornehmen, und wählen Sie dann **senden**.

Wählen Sie zum Löschen dieses Profils **Profil löschen** der oberen rechten Ecke der Seite.

### <a name="add-devices-to-a-customers-account"></a>Fügen Sie Geräte hinzu, um ein Kundenkonto

>[!NOTE]
>Vertreter und Administrator-Agents können Geräte, ein Kundenkonto hinzufügen.

Bevor Sie benutzerdefinierte Autopilot-Profile auf kundengeräten anwenden können, müssen Sie Geräteliste des Kunden Zugriff auf sein.

Wenn Sie die OEM-Name, Seriennummer und Modell Kombination verwenden möchten, achten Sie darauf, dass Sie diese Einschränkungen:

- Diese Tupel funktioniert nur für neuere Geräte (4 k Hashes, z. B.) und wird für 128b-Hashes (RS2 und vorherige Geräten) nicht unterstützt.

- Die Registrierung des Tupel ist Groß-/ Kleinschreibung, damit die Daten in der Datei den Hersteller und Modell-Namen übereinstimmen müssen ***genau*** gemäß der OEM-Anbieter (Hardwareanbieter).

Führen Sie die nachstehenden Anweisungen zum Hinzufügen von Geräten zum Konto eines Kunden im Partner Center.

1. Wählen Sie **Kunden** aus dem Partner Center-Menü und wählen Sie dann den Kunden, deren Geräte, die Sie verwalten möchten.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Klicken Sie unter **gelten Profile für Geräte** wählen **Geräte hinzufügen**.

4. Geben Sie einen Namen für die Geräteliste aus, und wählen Sie dann **Durchsuchen** die Kundenliste (im Format der CSV-Datei) in Partner Center hochladen.

    >[!NOTE]
    >Sie sollten diese CSV-Datei mit dem Gerät Kauf erhalten haben. Wenn Sie eine CSV-Datei nicht angezeigt wird, können Sie selbst eine erstellen, indem Sie die Schritte in [Hinzufügen von Geräten in Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Hochladen die CSV-Datei, und wählen Sie dann **speichern**.

Wenn Sie eine Fehlermeldung erhalten, bei dem Versuch, die zum Hochladen der CSV-Datei, überprüfen Sie das Format der Datei ein. Sie können nur der Hardwarehash oder der OEM-Name, Seriennummer und -Modell (in dieser Reihenfolge) oder die Windows-Produkt-ID verwenden. Sie können auch die Beispiel-CSV-Datei bereitgestellt über den Link neben **Geräte hinzufügen** um eine Liste der Geräte zu erstellen.

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot-Endbenutzer-Lizenzvertrag Kündigung

### <a name="important-information"></a>WICHTIGE INFORMATIONEN

Windows Autopilot können Sie zum Konfigurieren von benutzerdefinierter Installationen von Windows auf Geräten, die Sie für Ihre Kunden zu verwalten. Wenn dazu autorisiert, durch den Kunden, können bestimmte Einrichtung-Seiten, die normalerweise für Benutzer, beim Einrichten von Windows angezeigt werden, einschließlich des Bildschirms des Endbenutzer-Lizenzvertrag (End User License Agreement) akzeptieren Sie unterdrücken oder ausblenden.

Mit dieser Funktion stimmen Sie folgendem zu unterdrücken oder Ausblenden der Bildschirme, mit denen Benutzern bereitstellen, beachten Sie, dass oder Akzeptanz von Nutzungsbedingungen bedeutet, dass Sie ausreichend Zustimmung und Autorisierung aus Ihrem Kunden, die Begriffe und, die von Ihnen im Auftrag von ausblenden erhalten haben der Kunde (gibt an, ob eine Organisation oder einen einzelnen Benutzer als der Fall sein kann), stimmen von Hinweisen und akzeptieren Sie alle Bedingungen, die an den Kunden anwendbar sind. Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten. Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.