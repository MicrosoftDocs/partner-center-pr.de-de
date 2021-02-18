---
title: Der Co-Selling-Connector für Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Sie Verweise in Partner Center mit Ihrem Co-Selling-Connector für Dynamics 365 CRM. Verkäufer können sich dann in Ihrem CRM-System mit Microsoft zusammen verkaufen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645773"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Co-Selling-Connector für Dynamics 365 CRM – Übersicht

### <a name="appropriate-roles"></a>Geeignete Rollen

- Empfehlungsadministrator
- Systemadministrator oder systemanpassungsprogramm im CRM

Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme. Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden. Verwenden Sie die Co-Selling-Connectors, um einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers zu erstellen, Referenzen von Microsoft-Verkäufern zu erhalten, Verweise zu akzeptieren/ablehnen, Daten zu ändern, wie z. b. den Geschäftswert und das Enddatum. Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten. Sie können Ihre gesamten Verweise im CRM Ihrer Wahl und nicht im Partner Center verwalten. 

Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.

## <a name="before-you-install---pre-requisites"></a>Vor der Installation von-Pre-Requirements

|**Themen**   |**Details**   |**Links**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Sie benötigen eine gültige MPN-ID.|So fügen Sie [MPN](https://partner.microsoft.com/) an|
|Cosell bereit|Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.|[Vertrieb mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partner Center-Konto|Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist. Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
|Partner Center-Benutzerrollen|Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.|[Zuweisen von Rollen und Berechtigungen zu Benutzern](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.|[Zuweisen von Rollen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Energie automatisierter Fluss Konto|Erstellen Sie eine neue Produktionsumgebung mit einer Datenbank für Test/Staging und Produktion. Wenn Sie über eine vorhandene Produktionsumgebung mit einer Datenbank verfügen, kann Sie wieder verwendet werden. Der Benutzer, der die Connector-Lösung installieren möchte, muss über eine Energie automatisierte Lizenz und Zugriff auf diese Umgebung verfügen. Sie können den Fortschritt überwachen und weitere Details erhalten, wenn die Installation in der [Energie Automatisierung](https://flow.microsoft.com/) fehlschlägt, indem Sie unter Lösungen auf Verlauf anzeigen klicken.|[Umgebung erstellen oder verwalten](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installieren der Partner Center-Synchronisierung für Dynamics 365 (Energie automatisierte Lösung)

1. Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus. In diesem Schritt werden die verfügbaren CRM-Instanzen angezeigt.

2. Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.

3. Wählen Sie in der linken Navigationsleiste **Lösungen** aus.

4. Klicken Sie im oberen Menü auf den Link **appsource öffnen** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Appsource öffnen":::

5. Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Dynamics365** .  

6. Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.

7. Dadurch wird die Seite geöffnet, auf der Sie die CRM-Umgebung (Dynamics 365) zum Installieren der Anwendung auswählen können.  Stimmen Sie den Geschäftsbedingungen zu.

8. Sie können den Fortschritt überwachen und weitere Details erhalten, wenn die Installation in der Energie Automatisierung fehlschlägt, indem Sie unter **Lösungen** auf **Verlauf** anzeigen klicken.
 

9. Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus. Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Dynamics 365** in der Lösungs Liste verfügbar ist.

10. Wählen Sie **Partner Center-Synchronisierungs Referenz für Dynamics 365 aus**. Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Verfügbare CRMs":::

## <a name="best-practice-test-before-you-go-live"></a>Bewährte Vorgehensweise: testen, bevor Sie fortfahren

Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.

- Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.
- Konfigurieren und Anpassen der Microsoft Power automatisiert-Lösung in der Stagingumgebung.
- Testen Sie die Lösung auf einer Staging/CRM-Instanz. 
- Importieren Sie bei Erfolg als verwaltete Lösung in die Produktions Instanz. 

## <a name="configure-the-solution"></a>Konfigurieren der Projektmappe

1. Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com/).


2. Wählen Sie in der Dropdown- **Umgebung** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Energie automatisierte Lösung installiert haben.

3. Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:

   - Partner Center-Benutzer mit referenrals Administrator Anmelde Informationen

   - Partner Center-Ereignisse

   - Der CRM-Administrator mit den Energie automatisierten Flows in der Lösung.

      1. Wählen Sie in der linken Navigationsleiste **Verbindungen** aus, und wählen Sie die Projekt Mappe "Partner Center-Verweise" aus der Liste aus.

      2. Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen** klicken.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Erstellen der Verbindung":::

      3. Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .

      4. Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".

      5. Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.

      6. Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.
     
      7. Nachdem Sie alle Verbindungen hinzugefügt haben, sollten in Ihrer Umgebung die folgenden Verbindungen angezeigt werden:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Verbindungen":::
   
## <a name="edit-the-connections"></a>Verbindungen bearbeiten

1. Kehren Sie zur Seite **Lösungen** zurück, und wählen Sie **Standard** Projekt Mappe aus. Wählen Sie **Verbindungs Verweis (Vorschau)** aus, indem Sie auf **alle** klicken.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Herstellen einer Verbindung":::

2. Bearbeiten Sie jede der Verbindungen nacheinander, indem Sie das Symbol drei Punkte auswählen. Fügen Sie die relevanten Verbindungen hinzu.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Aufgeführte Verbindungen"::: 

3.  Kehren Sie zur Seite Lösungen zurück, wählen Sie Partner Center-Synchronisierungs Synchronisierung für Dynamics 365 aus, und schalten Sie den Flow ein, indem Sie in der folgenden Reihenfolge auf das drei-Punkte-Symbol neben jedem Flow klicken. Wenn beim Einschalten des Flows Probleme auftreten, lesen Sie die Schritte zur [Anpassung](connector-dynamics.md#customize-synchronization-steps) und [Problem](connectors-troubleshoot.md)Behandlung. 

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

Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren. Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.

1. Wählen Sie **Partner Center auf Dynamics 365 (Insider Preview)** aus.

2. Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung** aus.

3. Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopieren der URL":::

4. Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen** aus.

5. Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.

6. Geben Sie die folgenden Details ein:

   - **Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL

   - **Zu registrierende Ereignisse**: Wählen Sie alle verfügbaren Ereignisse ("Verweis-erstellt", "Verweis-aktualisiert", "Related-Referral-created", "Related-Referral-aktualisierte") aus.

   -**Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja, es ist wichtig zu beachten, dass nur eine URL für ein bestimmtes webhook-Ereignis registriert werden kann. Es ist wichtig zu beachten, dass nur eine URL für ein bestimmtes webhook-Ereignis registriert werden kann. 

7. Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**

Der webhook kann nun auf Create-und Update-Ereignisse lauschen.

## <a name="customize-synchronization-steps"></a>Synchronisierungs Schritte anpassen

CRM-Systeme sind hochgradig angepasst, und Sie können die Energie automatisierte Lösung basierend auf Ihrem CRM-Setup anpassen.  Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, im [Leitfaden für benutzerdefinierte Feld Zuordnung](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)aufgeführt.

Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in **[anpassen] erstellen oder erhalten von Details aus Dynamics 365 Flow**  oder Umgebungsvariablen vor. Es wird empfohlen, keine anderen Flows in der Energie automatisierten Lösung zu aktualisieren, da dies Auswirkungen auf zukünftige Lösungs Upgrades haben kann. 

Im folgenden finden Sie die verfügbaren Anpassungen:

- Häkchen in Name der Verkaufschance: Standardmäßig wird ein Häkchen neben dem Namen der Verkaufschance angezeigt, um anzugeben, dass die Synchronisierung zwischen Partner Center und Dynamics 365 CRM erfolgreich durchgeführt wird. Auf ähnliche Weise wird eine Kreuz Markierung angezeigt, wenn bei der Synchronisierung ein Fehler auftritt. Wenn Sie das Hinzufügen von Check-oder Cross-Markierungen in den Namen der Verkaufschance vermeiden möchten, legen Sie den aktuellen Wert von Anzeige Häkchen in Name der Verkaufschance

- Wert für die Handhabung: Standardmäßig wird der Wert für den Wert aus Partner Center in CRM mit und von **estimatedvalue** synchronisiert. Wenn Sie in CRM ein anderes Feld für den zu synchronisierenden Wert haben:

    a.    Aktualisieren Sie den Feldnamen für den Geschäftswert in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen von CRM. Beachten Sie, dass Sie den Namen des Felds nicht seinen anzeigen Amen angeben sollten.

    b.    Bearbeiten **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow**  , navigieren Sie zu **erstellen oder aktualisieren** der Gelegenheit in CRM, und aktualisieren Sie **eine neue Gelegenheit** , und **Aktualisieren Sie vorhandene** Verkaufschancen Aktionen, um den Wert von **dealvalue** dem richtigen Feld in CRM zuzuweisen. Entfernen Sie außerdem die **dealvalue-Zuweisung** aus dem Feld **geschätztes Umsatz** .

- Ländercode des Kundenkontos: Es ist obligatorisch, bei der Erstellung eines neuen Verweises einen Ländercode mit zwei Buchstaben (ISO 3166) bereitzustellen. Standardmäßig wird Ländercode mit dem address1_country-Feld des Kontos in CRM synchronisiert. Wenn Sie in CRM ein anderes Feld für die Synchronisierung von Ländercode haben:

   a.    Für ein Feld mit zwei Buchstaben, das kein Such Land für Ländercodes ist:

   - Aktualisieren Sie den Ländercode-Feldnamen für das Kundenkonto in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen von CRM. Beachten Sie, dass Sie den Namen des Felds nicht seinen anzeigen Amen angeben sollten.

   - Bearbeiten **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow**  , und navigieren Sie zu erstellen oder in der CRM-Aktion zum Erstellen eines Kundenkontos, um dem richtigen Feld in CRM einen Länder Wert zuzuweisen. Entfernen Sie außerdem die Länder Wert Zuweisung aus dem Feld Adresse 1: Land/Region.

   b.    Für ein suchbasiertes Ländercode Feld Unterkonto:

   - Fügen Sie ein neues benutzerdefiniertes Feld in "Account" hinzu, und füllen Sie es mit zwei buchstabischem Ländercode (ISO 3166) auf der Grundlage des im Nachschlage basierten Feld ausgewählten Werts und umgekehrt.

   - Führen Sie die obigen Schritte aus, um ein neues benutzerdefiniertes Feld aus CRM in das und aus dem Partner Center zu synchronisieren.

- Verkaufschancen Felder: Wenn es Pflichtfelder gibt, die ausgefüllt werden müssen, bearbeiten **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow**  , und navigieren Sie zu **erstellen oder Aktualisieren der Gelegenheit** in CRM und aktualisieren **Erstellen Sie eine neue Verkaufschance** , um den obligatorischen Feldern basierend auf Ihren geschäftlichen Anforderungen Werte zuzuweisen.

- Führende Felder: Wenn es verbindliche Felder gibt, die ausgefüllt werden müssen, bearbeiten **[anpassen] erstellen oder Aktualisieren von Details aus Dynamics 365 Flow**  und navigieren zu **Create or Update Lead** in CRM und Update **Erstellen Sie eine neue Lead Aktion** , um den obligatorischen Feldern basierend auf Ihren Geschäftsanforderungen Werte zuzuweisen.

- Kundenkonto: Wenn ein neuer Verweis von Partner Center mit CRM synchronisiert wird, versucht die Energie automatisierte Lösung, ein vorhandenes Konto in CRM mithilfe des Kunden Firmennamens und der Postleitzahl zu suchen. Wenn eine solche nicht gefunden wird, wird ein neues Kundenkonto in CRM erstellt. Um die Suchkriterien zu aktualisieren und Details zu den neuen Konten zu erstellen, bearbeiten Sie **[anpassen] erstellen oder erhalten Sie Details aus Dynamics 365 Flow** , und navigieren Sie zu **erstellen oder Erstellen eines Kundenkontos** in CRM und Erstellen einer Aktion für das **Kundenkonto**.

## <a name="update-environment-variable"></a>Umgebungsvariable aktualisieren

So aktualisieren Sie einen Umgebungsvariablen Wert:

1. Wechseln Sie zur Seite **Lösungen** , und wählen Sie **Standardlösung** aus. Wählen Sie **Umgebungs Variable** aus, indem Sie auf alle klicken.

2. Wählen Sie die Umgebungsvariable für den zu aktualisierenden Wert aus, und klicken Sie auf mit drei Punkten Symbol auf **Bearbeiten** .

3. Aktualisieren Sie den **aktuellen Wert** (Standardwert nicht aktualisieren) mithilfe der Option " **neuer Wert** ", und geben Sie den Wert an. Der Wert muss mit dem Datentyp der Variablen identisch sein, z. b. wenn der Datentyp Yes/No entweder yes oder No Value annimmt.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Bearbeitungsfeld für Standardwerte":::

- End-to-End-bidirektionale Co-Selling-Synchronisierung

Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 und Partner Center testen.

### <a name="pre-requisites"></a>Voraussetzungen

Um die Verweise auf Partner Center und Dynamics 365 CRM zu synchronisieren, werden die Microsoft-spezifischen verweigerfelder von der Energie automatisierten Lösung eindeutig abgegrenzt. Diese Identifikation gibt Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.

Ein Satz von benutzerdefinierten Feldern und Objekten wird als Teil der projektmappeninstallation hinzugefügt. Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center**: gibt an, ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll. Standardmäßig ist der Wert dieses Felds Nein und muss von Ihrem Verkäufer explizit auf Yes festgelegt werden, um eine Gelegenheit für Microsoft zu geben. Für neue Verweise, die von Partner Center an CRM gemeinsam genutzt werden, wird dieser Feldwert auf Ja festgelegt.

- **Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz

- **Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center
- **Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis. Um einen Co-Selling-Verweis zu erstellen, wählen Sie die entsprechende Hilfe von Microsoft aus. Ein Kundenkontakt muss der Gelegenheit zur Erstellung eines Co-Selling-Verweises zugeordnet werden. Lassen Sie dieses Feld deaktiviert, um einen nicht-Co-Selling-Verweis zu erstellen. Ein nicht Co-Selling-Verweis kann jederzeit in eine Co-Selling-Referenz konvertiert werden, indem die entsprechende Hilfe Option erforderlich ausgewählt wird.

- **Übersicht über das Microsoft Partner Center**-Portal: Wählen Sie Sichtbarkeit für Microsoft Partner Center-Referenz Wenn Sie ihn für Microsoft-Verkäufer sichtbar machen, kann ein nicht Co-Selling-Verweis in Co-Selling konvertiert werden. Wenn die Microsoft-Hilfe erforderlich ist, ist der Verweis standardmäßig für Microsoft-Verkäufer sichtbar. Nachdem das Feld als sichtbar markiert wurde, kann es nicht wieder hergestellt werden.

- **Microsoft CRM-Bezeichner**: Wenn ein Co-Selling-Verweis von Microsoft erstellt und akzeptiert wird, wird dieses Feld mit dem CRM-Bezeichner von Microsoft aufgefüllt.

- **Produkte: veraltet** – verwenden Sie dieses Feld nicht, oder fügen Sie es dem CRM-Abschnitt hinzu. es ist nur aus Gründen der Abwärtskompatibilität verfügbar. Verwenden Sie stattdessen Microsoft Partner Center-Lösungen.

- Überwachung **: ein** Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen

- **Microsoft Partner Center-Lösungen**: ein benutzerdefiniertes Objekt, mit dem Co-Selling-Lösungen oder Microsoft-Lösungen mit der Gelegenheit verknüpft werden können. Eine oder mehrere Lösungen können hinzugefügt und/oder aus der Verkaufschance entfernt werden. Es ist obligatorisch, der Gelegenheit mindestens eine Co-Selling-oder Microsoft-Lösung hinzuzufügen, bevor Sie Sie für Microsoft freigeben. Um dieses Objekt der Gelegenheit zuzuordnen, aktualisieren Sie das Verkaufschancen Formular in CRM:

  Wählen Sie die entsprechende Registerkarte in der Verkaufschance aus, und fügen Sie wie unten gezeigt ein unter Raster hinzu:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Verkaufschancen Formular":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Nachdem Sie Microsoft-Lösungen hinzugefügt haben, können Sie die Details der Co-Selling-Lösung vorab auffüllen, damit ihre Verkäufer Sie nicht hinzufügen müssen. Zum Hinzufügen eines neuen Lösungs Details wechseln Sie in CRM zum Microsoft Solution Details-Objekt, und klicken Sie auf **Datensatz hinzufügen** , um einen Eintrag hinzuzufügen, oder verwenden Sie **Excel Upload** , um mehrere Einträge hinzuzufügen.

:::image type="content" source="images/dynamic-1a.png" alt-text="Details zur Lösung":::

### <a name="scenarios"></a>SS

1. Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:

   1. Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.

   2. Stellen Sie sicher, dass der Microsoft Partner Center-Abschnitt vorhanden ist, wenn Sie eine neue Verkaufschance in der Dynamics 365-Umgebung erstellen.

   :::image type="content" source="images/dynamic-2a.png" alt-text="Neue Verkaufschance"::: 

   3. Wenn Sie diese Gelegenheit mit Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

      - **Wie kann Microsoft helfen?**: Wählen Sie zum Erstellen eines Co-Selling-Verweises eine entsprechende Hilfe Option aus.

         :::image type="content" source="images/dynamic-3a.png" alt-text="So erhalten Sie geeignete Felder in der Kartenansicht":::

      - **Kundenkontakt**: um eine Co-Selling-Referenz zu erstellen, fügen Sie der Verkaufschance einen Kundenkontakt hinzu.
      - **Mit Partner Center synchronisieren**: Ja

      - Microsoft-Lösungen: zum Freigeben eines Verweises an Microsoft fügen Sie der Verkaufschance eine gültige Co-Selling-oder Microsoft-Lösung hinzu.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Lösungs-ID":::

   4. Wenn die Verkaufschance in Dynamics 365 mit der Option sync with Partner Center auf Ja festgelegt ist, warten Sie 10 Minuten, und melden Sie sich dann bei Ihrem Partner Center-Konto an. Ihre Verweise werden mit Dynamics 365 und der Verweis Kennung synchronisiert. Der Verweis Link wird aufgefüllt. Bei einem Fehler wird das Überwachungs Feld mit den Fehlerinformationen aufgefüllt.
     
    5. Für eine Gelegenheit, bei der die Option "Synchronisierung mit Partner Center" auf "Ja" festgelegt wurde, werden die Änderungen bei der Aktualisierung der Gelegenheit in Dynamics 365 CRM in Ihrem Partner Center-Konto synchronisiert.

    6. Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.

2. Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:

   1. Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.

   2. Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.

   3. Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie die Option "  **neues Geschäft** " auswählen.

   4. Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an.

   5. Navigieren Sie zu **Open Verkaufschancen**. Der im Microsoft Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.

   6. Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)

- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)

- [Weitere Informationen zur Microsoft powerautomatisieren-Plattform](/power-automate/)

- [Partner Center-Webhooks](/partner-center/develop/partner-center-webhooks)