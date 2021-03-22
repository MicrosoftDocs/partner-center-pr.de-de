---
title: Der Co-Selling-Connector für Dynamics 365 CRM Partner Center
description: Synchronisieren Sie Verweise in Partner Center mit Ihrem Co-Selling-Connector für Dynamics 365 CRM. Sie können dann in Ihrem CRM-System mit Microsoft zusammen verkaufen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768770"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Übersicht über den Co-Selling-Connector für Dynamics 365 CRM

### <a name="appropriate-roles"></a>Geeignete Rollen

- Empfehlungsadministrator
- Systemadministrator oder systemanpassungsprogramm im CRM

Partner Center-Co-Selling-Connectors ermöglichen es ihren Verkäufern, gemeinsam mit Microsoft über Ihre CRM-Systeme zu verkaufen. Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden. Verwenden Sie die Co-Selling-Connectors, um einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers zu erstellen, Referenzen vom Microsoft-Verkäufer zu erhalten, Verweise zu akzeptieren oder abzulehnen und Geschäftsdaten zu ändern, wie z. b. den Geschäftswert und das Enddatum. Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten. Sie können Ihre gesamten Verweise im CRM Ihrer Wahl und nicht im Partner Center verwalten.

Die Lösung basiert auf der Strom Automatisierung und verwendet Partner Center-APIs.

## <a name="prerequisites"></a>Voraussetzungen

Stellen Sie sicher, dass die folgenden Voraussetzungen erfüllt sind, bevor Sie die Lösung installieren.

|**Themen**   |**Details**   |**Links**   |
|--------------|--------------------|------|
|MPN-ID (Microsoft Partner Network) |Sie benötigen eine gültige MPN-ID.|[Beitreten zum Partner Netzwerk](https://partner.microsoft.com/)|
|Co-Sell Ready (Für Co-Selling bereit)|Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.|[Vertrieb mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partner Center-Konto|Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist. Vergewissern Sie sich, dass Ihre Co-Selling-Verweise im Partner Center-Portal angezeigt werden, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
|Partner Center-Benutzerrollen|Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.|[Zuweisen von Rollen und Berechtigungen zu Benutzern](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.|[Zuweisen von Rollen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Energie automatisierter Fluss Konto|Erstellen Sie eine neue Produktionsumgebung mit einer Datenbank für Tests, Staging und Produktion. Wenn Sie über eine vorhandene Produktionsumgebung mit einer-Datenbank verfügen, kann diese wieder verwendet werden. Der Benutzer, der die Connector-Lösung installieren möchte, muss über eine Strom Automatisierungs Lizenz verfügen und auf diese Umgebung zugreifen können. Wenn bei der Installation ein Fehler auftritt, können Sie den Fortschritt überwachen und weitere Informationen in der [Energie Automatisierung](https://flow.microsoft.com/) erhalten. Wählen Sie unter **Lösungen** die Option **Verlauf** anzeigen aus.|[Umgebung erstellen oder verwalten](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installieren der Partner Center-Synchronisierung für Dynamics 365 (Energie automatisierte Lösung)

1. Wechseln Sie zu [Energie Automatisierung](https://flow.microsoft.com), und wählen Sie in der oberen rechten Ecke die Option **Umgebungen** aus. In diesem Schritt werden die verfügbaren CRM-Instanzen angezeigt.

1. Wählen Sie in der Dropdown Liste in der oberen rechten Ecke die entsprechende CRM-Instanz aus.

1. Wählen Sie auf der linken Seite **Lösungen** aus.

1. Wählen Sie im oberen Menü den Link **appsource öffnen** aus.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Screenshot, der das Öffnen von appsource anzeigt":::

1. Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Dynamics 365** .  

1. Wählen Sie die Schaltfläche **jetzt starten** aus, und klicken Sie dann auf **weiter**.

1. Es wird eine Seite angezeigt, auf der Sie die CRM-Umgebung (Dynamics 365) zum Installieren der Anwendung auswählen können. Stimmen Sie den Geschäftsbedingungen zu.

1. Sie können den Fortschritt überwachen. wenn die Installation fehlschlägt, können Sie weitere Details in der Energie Automatisierung anzeigen, indem Sie unter **Lösungen** die Option **Verlauf** anzeigen auswählen.

1. Wechseln Sie nach Abschluss der Installation wieder zur [Energie Automatisierung](https://flow.microsoft.com) , und klicken Sie auf der linken Seite auf **Lösungen** . Die **Synchronisierung der Partner Center-Verweise für Dynamics 365** ist nun in der **Lösungs** Liste verfügbar.

1. Wählen Sie **Partner Center-Synchronisierungs Referenz für Dynamics 365 aus**. Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Screenshot mit verfügbaren CRMs.":::

## <a name="test-before-you-go-live"></a>Testen, bevor Sie fortfahren

Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen. Folgendes ist erforderlich:

- Installieren Sie die Lösung für die Energie Automatisierung in einer Instanz der Staging-Umgebung CRM.
- Konfigurieren und Anpassen der Energie automatisierten Lösung in einer Stagingumgebung.
- Testen Sie die Projekt Mappe in einer Staging-CRM-Instanz.
- Importieren Sie nach einem erfolgreichen Test als verwaltete Lösung in die Produktions Instanz.

## <a name="configure-the-solution"></a>Konfigurieren der Projektmappe

1. Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, wechseln Sie zurück zur [Energie Automatisierung](https://flow.microsoft.com/).

1. Wählen Sie in der Dropdown Liste **Umgebungen** in der oberen rechten Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.

1. Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:

   - Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen
   - Partner Center-Ereignisse
   - CRM-Administrator mit den Energie automatisierten Flows in der Lösung

   1. Wählen Sie Links **Verbindungen** aus, und wählen Sie die Projekt Mappe **Partner Center-Verweise** aus der Liste aus.

   1. Erstellen Sie eine Verbindung, indem Sie **Verbindung herstellen** auswählen.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot, der das Erstellen einer Verbindung zeigt.":::

   1. Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .

   1. Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".

   1. Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.

   1. Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.
     
   1. Nachdem Sie alle Verbindungen hinzugefügt haben, sollten in Ihrer Umgebung die folgenden Verbindungen angezeigt werden.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Screenshot, der Verbindungen anzeigt.":::

## <a name="edit-the-connections"></a>Verbindungen bearbeiten

1. Kehren Sie zur Seite **Lösungen** zurück, und wählen Sie **Standard** Projekt Mappe aus. Wählen Sie **Verbindungs Verweis (Vorschau)** aus, indem Sie **alle** auswählen.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot, der die Bearbeitung der Verbindungen anzeigt.":::

1. Bearbeiten Sie jede der Verbindungen nacheinander, indem Sie das Symbol mit den Auslassungs Punkten auswählen. Fügen Sie die relevanten Verbindungen hinzu.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Screenshot, der die aufgelisteten Verbindungen anzeigt.":::

1.  Kehren Sie zur Seite **Lösungen** zurück, wählen Sie **Partner Center-Synchronisierungs Synchronisierung für Dynamics 365 aus**, und aktivieren Sie den Flow, indem Sie in der folgenden Reihenfolge das Symbol mit den Auslassungs Punkten neben den einzelnen Flows auswählen. Wenn beim Einschalten des Flows Probleme auftreten, finden Sie weitere Informationen unter [Anpassungsschritte](connector-dynamics.md#customize-synchronization-steps) und [Schritte zur Problem](connectors-troubleshoot.md)Behandlung.

Aktivieren Sie die Flows in der folgenden Reihenfolge:

- Partner Center-webhook-Registrierung (Insider Preview)
- Erstellen einer Co-Selling-Referenz – Dynamics 365 to Partner Center (Insider Preview)
- Anzupassen Erstellen oder erhalten von Details aus Dynamics 365 Flow
- Partner Center auf Dynamics 365-Helper (Insider Vorschau)
- Partner Center Microsoft Co-Selling-Verweises Aktualisierungen an Dynamics 365 (Insider Preview)
- Partner Center auf Dynamics 365 (Insider-Vorschau)
- Dynamics 365 to Partner Center (Insider Vorschau)
- Dynamics 365-Chance an Partner Center (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse

Sie können die Partner Center-webhook-APIs verwenden, um sich für Ressourcen Änderungs Ereignisse zu registrieren. Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.

1. Wählen Sie **Partner Center auf Dynamics 365 (Insider Preview)** aus.

1. Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie aus, **Wenn eine HTTP-Anforderung empfangen wird**.

1. Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.

   :::image type="content" source="images/webhook-video.gif" alt-text="Screenshot, der die Verwendung von webhooks zum Registrieren von Ressourcen Änderungen anzeigt.":::

1. Wählen Sie die Option **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisiert aus, und klicken Sie dann auf **Ausführen**.

1. Stellen Sie sicher, dass das Fenster " **Flow ausführen** " im rechten Bereich geöffnet wird, und wählen Sie **weiter** aus.

1. Geben Sie die folgenden Details ein:

   - **Endpunkt des http-Auslösers**: diese URL wurde aus einem vorherigen Schritt kopiert.
   - **Zu registrierende Ereignisse**: Wählen Sie alle verfügbaren Ereignisse aus (**Verweis-erstellt**, **Verweis-aktualisiert**, **bezogen-Verweis-erstellt** und **Verwandte Verweise**).
   - **Vorhandene auslöserendpunkte überschreiben, falls vorhanden?**: Ja. Für ein bestimmtes webhook-Ereignis kann nur eine URL registriert werden.

1. Wählen Sie **Flow ausführen** aus, und wählen Sie dann **abgeschlossen aus.**

Der webhook kann nun Ereignisse lauschen, erstellen und aktualisieren.

## <a name="customize-synchronization-steps"></a>Synchronisierungs Schritte anpassen

CRM-Systeme sind hochgradig angepasst, und Sie können die Energie automatisierte Lösung basierend auf Ihrem CRM-Setup anpassen. Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, im [Leitfaden benutzerdefinierte Feld Zuordnung](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)aufgeführt.

Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in **[anpassen] erstellen oder erhalten von Details aus Dynamics 365 Flow** oder Umgebungsvariablen vor. Aktualisieren Sie keine anderen Flows in der Energie automatisierten Lösung, da dies Auswirkungen auf zukünftige Lösungs Upgrades haben kann.

Die folgenden Anpassungen sind verfügbar:

- **Anzeige Häkchen im Namen der Verkaufschance**: Standardmäßig wird ein Häkchen neben dem Namen der Verkaufschance angezeigt, um anzugeben, dass die Synchronisierung zwischen Partner Center und Dynamics 365 CRM erfolgreich durchgeführt wird. Auf ähnliche Weise wird eine Kreuz Markierung angezeigt, wenn bei der Synchronisierung ein Fehler auftritt. Um zu vermeiden, dass der Name einer Überprüfung oder Kreuz Markierung hinzugefügt wird, legen Sie den aktuellen Wert des **Anzeige Häkchens in der Umgebungsvariablen "Name der Verkaufschance** " auf Nein fest.
- **Wert "Wert**": Standardmäßig wird der Wert "Wert" aus Partner Center mit und von " **estimatedvalue** " im CRM synchronisiert. Wenn Sie über ein anderes Feld im CRM verfügen, aus dem der Wert für den Wert synchronisiert werden soll:

  - Aktualisieren Sie den Feldnamen für den Wert des Geschäfts **Werts** in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen von CRM. Stellen Sie sicher, dass Sie den Feldnamen und nicht den anzeigen Amen angeben.
  - Bearbeiten **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow**. wechseln Sie zu **Create or Update Opportunity** in CRM, und aktualisieren Sie **neue Verkaufschancen** , und aktualisieren Sie **vorhandene** Verkaufschancen Aktionen, um den Wert **dealvalue** dem richtigen Feld im CRM zuzuweisen. Entfernen Sie außerdem die **dealvalue** -Zuweisung aus dem Feld **geschätztes Umsatz** .

- **Ländercode des Kundenkontos**: Es ist obligatorisch, einen aus zwei Buchstaben bestehenden Ländercode (ISO 3166) anzugeben, wenn Sie einen neuen Verweis erstellen. Standardmäßig wird der Ländercode mit dem **address1_country** Feld des Kontos im CRM synchronisiert. Wenn Sie über ein anderes Feld im CRM verfügen, aus dem der Ländercode synchronisiert werden soll:

   - Für ein Feld für eine nicht-Lookup-Landesvorwahl in dem Konto, das einen aus zwei Buchstaben bestehenden Code enthält:
     - Aktualisieren Sie den Feldnamen für den **Länder Code des Kundenkontos** in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen von CRM. Stellen Sie sicher, dass Sie den Feldnamen und nicht den anzeigen Amen angeben.
     - Bearbeiten **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow**, und wechseln Sie zum **erstellen oder Erstellen eines Kundenkontos** in der CRM-Aktion, um dem richtigen Feld im CRM einen **Länder** Wert zuzuweisen. Entfernen Sie außerdem die **Länder** Wert Zuweisung aus dem Feld **Adresse 1: Land/Region** .

   - Für ein Nachschlage basiertes Ländercode Feld im Konto:
     - Fügen Sie ein neues benutzerdefiniertes Feld in das Konto ein, und füllen Sie es automatisch mit einem aus zwei Buchstaben bestehenden Ländercode (ISO 3166) auf der Grundlage des im Lookup-basierten Feld ausgewählten Werts und umgekehrt.
     - Führen Sie die obigen Schritte für das Feld "nonlookup Country Code" aus, um ein neues benutzerdefiniertes Feld vom CRM zum und aus dem Partner Center zu synchronisieren.

- Verkaufs **Chancen Felder**: Wenn es Pflichtfelder gibt **, die ausgefüllt werden müssen, bearbeiten** Sie **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow** , und wechseln Sie zu **Create or Update Opportunity** in the CRM und Update **Create a New Opportunity Action** , um den obligatorischen Feldern basierend auf Ihren geschäftlichen Anforderungen Werte zuzuweisen.
- **Führende Felder**: Wenn es verbindliche Felder gibt, **die ausgefüllt werden müssen, bearbeiten** Sie **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow** , und wechseln Sie zu **Create or Update Lead** in the CRM und Update **Create a New Lead Action** , um den obligatorischen Feldern basierend auf Ihren Geschäftsanforderungen Werte zuzuweisen.
- **Kundenkonto**: Wenn ein neuer Verweis von Partner Center mit dem CRM synchronisiert wird, versucht die Energie automatisierte Lösung, mithilfe des Firmennamens und der Postleitzahl des Kunden nach einem vorhandenen Konto im CRM zu suchen. Wenn eine solche nicht gefunden wird, wird im CRM ein neues Kundenkonto erstellt. Um die Suchkriterien zu aktualisieren und Details zu den neuen Konten zu erstellen, bearbeiten Sie **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow** und wechseln zum **erstellen oder Erstellen eines Kundenkontos** in der CRM-Aktion und zum **Erstellen eines Kundenkontos**.

## <a name="update-environment-variable"></a>Umgebungsvariable aktualisieren

So aktualisieren Sie einen Umgebungsvariablen Wert:

1. Wechseln Sie zur Seite **Lösungen** , und wählen Sie **Standardlösung** aus. Wählen Sie die **Umgebungs Variable** aus, indem Sie **alle** auswählen.

1. Wählen Sie die Umgebungsvariable für den zu aktualisierenden Wert aus, und klicken Sie auf das Symbol mit den Auslassungs Punkten **Bearbeiten** .

1. Aktualisieren Sie den **aktuellen Wert** ( **Standardwert** nicht aktualisieren), indem Sie die Option **neuer Wert** verwenden und den Wert angeben. Der Wert muss mit dem Datentyp der Variablen identisch sein. Der Datentyp yes oder No akzeptiert z. b. entweder den Wert yes oder No.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Screenshot, der die Umgebungsvariablen aktualisieren anzeigt.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>End-to-End-bidirektionale Co-Selling-Synchronisierung

Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 und Partner Center testen.

### <a name="prerequisites"></a>Voraussetzungen

Um die Verweise auf Partner Center und Dynamics 365 CRM zu synchronisieren, werden die Microsoft-spezifischen verweigerfelder von der Energie automatisierten Lösung eindeutig abgegrenzt. Diese Identifikation gibt Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.

Ein Satz von benutzerdefinierten Feldern und Objekten wird als Teil der projektmappeninstallation hinzugefügt. Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center**: gibt an, ob die Gelegenheit mit Partner Center synchronisiert werden soll. Standardmäßig ist der Wert dieses Felds Nein und muss von Ihrem Verkäufer explizit auf Yes festgelegt werden, um eine Gelegenheit für Microsoft zu geben. Für neue Verweise, die von Partner Center an CRM gemeinsam genutzt werden, wird dieser Feldwert auf Ja festgelegt.
- **Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Partner Center-Referenz.
- **Verweis Link**: ein Schreib geschützter Link zum Verweis in Partner Center.
- **Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis. Um einen Co-Selling-Verweis zu erstellen, wählen Sie die entsprechende Hilfe aus, die von Microsoft benötigt wird. Ein Kundenkontakt muss der Gelegenheit zur Erstellung eines Co-Selling-Verweises zugeordnet werden. Wählen Sie dieses Feld nicht aus, um einen nicht-Co-Selling-Verweis zu erstellen. Ein nicht-Co-Selling-Verweis kann jederzeit in eine Co-Selling-Referenz konvertiert werden, indem die entsprechende Hilfe Option ausgewählt wird.
- **Microsoft Partner Center-Referenz Sichtbarkeit**: Wählen Sie die Sichtbarkeit für die Partner Center-Referenz. Wenn Sie ihn für Microsoft-Verkäufer sichtbar machen, kann ein nicht-Co-Selling-Verweis in Co-Selling konvertiert werden. Wenn die Microsoft-Hilfe erforderlich ist, ist der Verweis standardmäßig für Microsoft-Verkäufer sichtbar. Nachdem dieses Feld als sichtbar markiert wurde, kann es nicht wieder hergestellt werden.
- **Microsoft CRM-Bezeichner**: Wenn ein Co-Selling-Verweis von Microsoft erstellt und akzeptiert wird, wird dieses Feld mit dem CRM-Bezeichner von Microsoft aufgefüllt.
- **Products: veraltet**: Verwenden Sie dieses Feld nicht, oder fügen Sie es dem CRM-Abschnitt hinzu. Sie steht nur aus Gründen der Abwärtskompatibilität zur Verfügung. Verwenden Sie stattdessen Partner Center-Lösungen.
- **Audit**: ein Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen.
- **Microsoft Partner Center-Lösungen**: ein benutzerdefiniertes Objekt, mit dem Co-Selling-Lösungen oder Microsoft-Lösungen mit der Gelegenheit verknüpft werden können. Eine oder mehrere Lösungen können der Verkaufschance hinzugefügt oder daraus entfernt werden. Es ist obligatorisch, der Gelegenheit mindestens eine Co-Selling-oder Microsoft-Lösung hinzuzufügen, bevor Sie Sie für Microsoft freigeben. Um dieses Objekt der Verkaufschance zuzuordnen, aktualisieren Sie das Verkaufs **Chancen** Formular im CRM.

  Wählen Sie die entsprechende Registerkarte im Formular für die Verkaufs **Chance** aus, und fügen Sie wie hier gezeigt ein unter Raster hinzu.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Screenshot, der das Formular für die Verkaufschance anzeigt.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Screenshot, der Microsoft-Lösungen zeigt.":::

- Nachdem Sie Microsoft-Lösungen hinzugefügt haben, können Sie die Details der Projekt Mappe vorab auffüllen, damit ihre Verkäufer Sie nicht hinzufügen müssen. Zum Hinzufügen eines neuen Lösungs Details wechseln Sie im CRM zum Microsoft Solution Details-Objekt, und wählen Sie **Datensatz hinzufügen** aus, um einen Eintrag hinzuzufügen, oder verwenden Sie **Excel Upload** , um mehrere Einträge hinzuzufügen.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Screenshot mit neuen Details der Microsoft-Lösung.":::

### <a name="scenarios"></a>Szenarien

1. Verweis Synchronisierung, wenn der Verweis im CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:

   1. Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung mit dem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.

   1. Stellen Sie sicher, dass der **Microsoft Partner Center** -Abschnitt vorhanden ist, wenn Sie eine neue Gelegenheit in der Dynamics 365-Umgebung erstellen.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Screenshot, in dem neue Möglichkeiten angezeigt werden.":::

   1. Wenn Sie diese Gelegenheit mit Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

      - **Wie kann Microsoft helfen?**: Wählen Sie eine entsprechende Hilfe Option aus, um einen Co-Selling-Verweis zu erstellen.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Screenshot, der zeigt, wie Sie geeignete Felder in der Kartenansicht erhalten.":::

      - **Kundenkontakt**: um eine Co-Selling-Referenz zu erstellen, fügen Sie der Verkaufschance einen Kundenkontakt hinzu.
      - **Mit Partner Center synchronisieren**: Ja.
      - **Microsoft-Lösungen**: zum Freigeben eines Verweises an Microsoft fügen Sie der Verkaufschance eine gültige Co-Selling-oder Microsoft-Lösung hinzu.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Screenshot, der die Lösungs-ID anzeigt.":::

   1. Wenn die Verkaufschance in Dynamics 365 mit der Option **sync with Partner Center** auf Ja festgelegt ist, warten Sie 10 Minuten. Melden Sie sich dann bei Ihrem Partner Center-Konto an. Ihre Verweise werden mit Dynamics 365 und der **Verweis Kennung** synchronisiert. Der **Verweis Link** wird aufgefüllt. Wenn ein Fehler auftritt, **wird das Überwachungs** Feld mit den Fehlerinformationen aufgefüllt.
     
    1. Für eine Gelegenheit, bei der die Option **sync with Partner Center** auf Yes festgelegt war, werden die Änderungen in Dynamics 365 CRM in Ihrem Partner Center-Konto synchronisiert, wenn Sie die Gelegenheit in Dynamics CRM aktualisieren.

    1. Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.

1. Verweis Synchronisierung, wenn der Verweis in Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:

   1. Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.

   1. Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.

   1. Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie die Option " **neues Geschäft** " auswählen.

   1. Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an.

   1. Wechseln Sie zu **Open Verkaufschancen**. Der im Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.

   1. Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)
- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
- [Weitere Informationen zur Microsoft Power automatisieren-Plattform](/power-automate/)
- [Partner Center-Webhooks](/partner-center/develop/partner-center-webhooks)
