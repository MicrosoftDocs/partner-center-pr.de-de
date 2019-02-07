---
title: Anpassen eines Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen | Partner Center
description: Vorkonfigurieren eines Geräts Out-of-Box-Experience mit Autopilot-Profilen.
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, Zero-Touch Deployment, Windows-Willkommensseite, Anmeldebildschirme, Out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062278"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Anpassen eines Geräts Out-of-Box-Experience mit Windows Autopilot-Profilen

**Gilt für:**

- CSP-Direct-Rechnung-Partner, indirekte Anbieter und indirekte Wiederverkäufer

Wenn Sie Kundengeräte verwalten, müssen Sie die Out-of-Box-Experience (OOBE) für die Kunden eines Benutzers anpassen. Sie können neue Geräte mit Windows Autopilot-Profilen vorab zu konfigurieren, bevor die Geräte an Kunden und Anwenden von neuen Profilen auf Geräte, die Kunden bereits erworben haben. In diesem Artikel wird erläutert, wie Sie erstellen und Anwenden von Autopilot-Profilen auf Geräte in Partner Center.

Wenn Sie nicht bereits mit Autopilot vertraut sind, lesen Sie die Informationen in diesen Artikeln:

- [Übersicht über Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot-Referenz-Bereitstellungshandbuch](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Übersicht

Mit dem Windows Autopilot-Feature im Partner Center können Sie benutzerdefinierte Profile für Kundengeräte erstellen. Die folgenden profileinstellungen waren zum Zeitpunkt der Veröffentlichung dieses Artikels verfügbar:

- Überspringen Sie datenschutzeinstellungen. Dieser optionalen Einstellung der Autopilot-Profil kann Organisationen nicht datenschutzeinstellungen während der OOBE-Prozesses Fragen.

- Deaktivieren Sie die Erstellung des lokalen Administratorkontos auf dem Gerät. Organisationen können entscheiden, ob der Benutzer das Gerät einrichten Administratorzugriff haben soll, nachdem der Vorgang abgeschlossen ist.

- Automatisch Gerät für die Arbeit oder Schule einrichten. Alle Geräte mit Autopilot registriert automatisch berücksichtigt werden Arbeit, Schule oder UNI Geräte, damit diese Frage nicht während der OOBE-Prozesses aufgefordert werden.

- Überspringen Sie Cortana-, Onedrive- und OEM-registrierungssetupseiten. Alle Geräte mit Autopilot registriert werden automatisch diese Seiten während des Out-of-Box-Experience (OOBE) zu überspringen.

- Überspringen Sie Endbenutzer-Lizenzvertrag (EULA) Ab Windows 10, Version 1709, können Organisationen entscheiden, auf die Seite EULA während der OOBE-Prozess zu überspringen. Finden Sie unter [Ablehnung der EULA für Windows Autopilot zu](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Seite "EULA" während des Windows Setup berücksichtigen.

Das folgende Profil und Gerät Delegieren von Berechtigungen und Einschränkungen gelten:

- CSP-Partner können weiterhin zum Verwalten von Autopilot Profile für vorhandene Kunden, mit denen sie Reseller-Geschäftsbeziehungen, haben, auch wenn die Kunden delegierten Administratorrechte des Partners entfernt haben.

- Sie können vorhandene Geräte für Ihre Kunden verwalten, die entweder von Ihnen oder von einem anderen CSP-Partner hinzugefügt wurden.

- Sie können keine Geräte verwalten, die Microsoft Store für Unternehmen oder Microsoft Intune-Portal Ihr Kunde hochgeladen hat.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Erstellen Sie und Verwalten von Autopilot-Profilen in Partner Center

Im Partner Center können Sie Windows Autopilot-bereitstellungsprofile erstellen und auf Geräte anwenden.

>[!NOTE]
>Nur Admin-Agents können erstellen und Anwenden von Profilen.

### <a name="create-a-new-autopilot-profile"></a>Erstellen Sie ein neues Autopilot-Profil

1. Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, die, dem Sie für das Autopilot-Profil erstellen.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Wählen Sie unter **Windows Autopilot Profile** **Neues Profil hinzufügen**.

4. Geben Sie Namen und eine Beschreibung des Profils, und konfigurieren Sie die Windows-Willkommensseite-Einstellungen. Wählen Sie aus:  

   - Überspringen der datenschutzeinstellungen im setup

   - Deaktivieren des lokalen Administratorkontos während des Setups
  
   - Automatisches Überspringen von Seiten im Setup<br>
        (Einschließlich *Automatisches Setup für Arbeit oder Schule auswählen* und *Überspringen Cortana, OneDrive und OEM-registrierungssetupseiten*)
  
   - Endbenutzer-Lizenzvertrag (EULA) überspringen<br> 
       >[!IMPORTANT] 
       >Finden Sie unter [Ablehnung der EULA für Windows Autopilot zu](#windows-autopilot-eula-dismissal) unten wichtige Informationen zum Überspringen der Seite "EULA" während des Windows Setup berücksichtigen.

5. Wählen Sie abschließend **Übermitteln** aus.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Anwenden einer Autopilot-Profilen auf Kundengeräte

>[!NOTE]
>Die folgenden Anweisungen wird davon ausgegangen, dass Sie bereits Geräte des Kunden in das Partner Center hinzugefügt haben und dass Sie ihre Liste der Geräte zugreifen können. Wenn Sie Geräte des Kunden bereits hinzugefügt haben, folgen Sie den Anweisungen im [Konto eines Kunden Geräte hinzufügen](#add-devices-to-a-customers-account) , und führen Sie dann die folgenden Schritte aus.

Nachdem Sie ein Autopilot-Profil für einen Kunden erstellt haben, können Sie es auf Geräte des Kunden anwenden.

1. Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, die, dem Sie für das Autopilot-Profil erstellt.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte oder Gerätegruppen, die Sie Profile hinzufügen, und wählen Sie dann **Profil anwenden**möchten. Das Profil, das Sie gerade angewendet wird in der Spalte **Profil** angezeigt.

4. Gehen Sie folgendermaßen vor, um sicherzustellen, dass das Profil erfolgreich auf das Gerät angewendet werden.

    a.  Verbinden Sie ein Gerät mit dem Netzwerk, und schalten Sie es ein.

    b.  Stellen Sie sicher, dass die entsprechenden Bildschirme der Windows-Willkommensseite (sofern vorhanden) angezeigt werden.

    c.  Wenn der OOBE-Prozess beendet wird, setzen Sie das Gerät auf die werksseitigen Standardeinstellungen, um sie für einen neuen Benutzer vorzubereiten.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Entfernen Sie ein Autopilot-Profil aus dem Gerät eines Kunden

1. Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, die, dem Sie für das Autopilot-Profil erstellt.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Wählen Sie unter **Anwenden von Profilen auf Geräte** die Geräte, die Sie entfernen Sie das Profil aus, und wählen Sie dann **Profil entfernen**möchten.

   >[!NOTE]
   >Entfernen ein Profil von einem Gerät wird nicht das Profil aus der Liste gelöscht. Wenn Sie ein Profil löschen möchten, folgen Sie den Anweisungen in [Aktualisieren oder Löschen eines Autopilot-Profils](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualisieren Sie oder löschen Sie ein Autopilot-Profil

Wenn ein Kunde die Out-of-Box-Erfahrung zu ändern möchte, nachdem Sie die Geräte darauf geliefert haben, können Sie das Profil in Partner Center ändern.

Wenn dem Gerät des Kunden mit dem Internet verbunden ist, wird es die neueste Version der Profile herunterladen, während der Windows-Willkommensseite. Darüber hinaus wird jedes Mal ein Kunde ein Gerät auf die werksseitigen Standardeinstellungen wiederherstellt das Gerät erneut herunter die neueste Version der Profile während der OOBE-Prozesses.

1. Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, der Sie ein Autopilot-Profil zu ändern möchten.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Wählen Sie unter **Windows Autopilot Profile** das Profil, das Sie aktualisieren müssen. Nehmen Sie die erforderlichen Änderungen vor, und wählen Sie dann **übermitteln**.

Wählen Sie aus der oberen rechten Ecke der Seite **Profil löschen** , um diesem Profil zu löschen.

### <a name="add-devices-to-a-customers-account"></a>Hinzufügen von Geräten auf dem Konto eines Kunden

>[!NOTE]
>Verkaufsvertreter und Admin-Agents können Geräte auf dem Konto eines Kunden hinzufügen.

Bevor Sie benutzerdefinierte Autopilot Profile auf Kundengeräte anwenden können, müssen Sie auf dem Gerät der Kundenliste zugreifen können.

Wenn Sie die OEM Name Seriennummer und Modell Kombination verwenden möchten, achten Sie darauf, dass Sie diese Einschränkungen:

- Das Tupel funktioniert nur für neuere Geräte (4 k Hashes, z. B.) und wird für 128b Hashes (RS2 und vorherigen Geräte) nicht unterstützt.

- Die Tupel-Registrierung wird Groß-/Kleinschreibung, damit die Daten in der Datei der Hersteller und Modell Namen ***genau*** übereinstimmen müssen von der OEM-Anbieter (Hardwareanbieter) bereitgestellt werden.

Gehen Sie von Geräten auf dem Konto eines Kunden im Partner Center.

1. Wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, deren Geräte, die Sie verwalten möchten.

2. Wählen Sie auf der Detailseite des Kunden **Geräte**.

3. Wählen Sie unter **Anwenden von Profilen auf Geräte** **Geräte hinzufügen**.

4. Geben Sie einen Namen für die Liste der Geräte, und wählen Sie dann zum Hochladen des Kunden Liste (CSV-Format) in Partner Center **Durchsuchen** .

    >[!NOTE]
    >Sie sollten diese CSV-Datei mit dem Gerät Kauf erhalten haben. Wenn Sie eine CSV-Datei nicht erhalten haben, können Sie selbst erstellen, mithilfe der Schritte im [Windows Autopilot-Geräte hinzufügen](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Laden Sie die CSV-Datei, und wählen Sie dann **Speichern**.

Wenn Sie eine Fehlermeldung, beim Versuch erhalten, die CSV-Datei hochzuladen, überprüfen Sie das Format der Datei. Sie können nur den Hardwarehash oder den OEM-Namen, Seriennummer, und Modell (in dieser Spaltenreihenfolge) oder die Windows-Produkt-ID verwenden. Sie können auch die Beispiel-CSV-Datei über den Link neben **Hinzufügen Geräte** bereitgestellt verwenden, um eine Liste der Geräte zu erstellen.

## <a name="windows-autopilot-eula-dismissal"></a>Ablehnung der EULA für Windows Autopilot zu

### <a name="important-information"></a>WICHTIGE INFORMATIONEN

Windows Autopilot können Sie benutzerdefinierte Installationen von Windows auf Geräten zu konfigurieren, die Sie für Ihre Kunden verwalten. Wenn dazu berechtigt, vom Kunden, können bestimmte Setupbildschirme, die normalerweise für Benutzer beim Einrichten von Windows, darunter der Bildschirm für die Annahme EULA (End User License Agreement) angezeigt werden Sie unterdrücken oder ausblenden.

Durch die Verwendung dieser Funktion stimmen Sie, dass das unterdrücken oder Ausblenden von Bildschirmen, die so konzipiert sind, um Benutzern zu liefern oder die Annahme von Begriffe bedeutet, dass Sie über ausreichende Zustimmung und Autorisierung von Ihrem Kunden Begriffe und, dass Sie im Auftrag von ausblenden abgerufen haben Ihr Kunde (gibt an, ob eine Organisation oder einzelner Benutzer der Fall sein kann), um solche Zustimmung und akzeptiert Begriffe, die an den Kunden relevant sind. Dazu gehört auch die Zustimmung zu den allgemeinen Geschäftsbedingungen der Lizenz oder des Hinweises, der dem Benutzer angezeigt werden würde, wenn Sie ihn nicht mit diesem Tool unterdrückt oder ausgeblendet hätten. Ihr Kunde darf die Windows-Software auf diesen Geräten nicht nutzen, wenn der Kunde nicht über eine gültig erworbene Lizenz für die Software von Microsoft oder dessen lizenzierten Distributoren verfügen.