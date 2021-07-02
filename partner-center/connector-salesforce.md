---
title: Der Co-Sell-Connector für Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Sie Ihre Empfehlungen in Partner Center Salesforce CRM. Verkäufer können dann in Ihren CRM-Systemen gemeinsam mit Microsoft verkaufen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173682"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Co-Selling-Connector für Salesforce CRM – Übersicht

**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Systemadministrator oder Systemanpasser im CRM

Partner Center Co-Sell-Connector ermöglicht es Ihren Verkäufern, in Ihren CRM-Systemen gemeinsam mit Microsoft zu verkaufen. Sie müssen nicht trainiert werden, um co-Partner Center verwalten zu können. Mithilfe der Co-Sell-Connectors können Sie eine neue Co-Sell-Empfehlung erstellen, um einen Microsoft-Verkäufer zu kontaktieren, Empfehlungen vom Microsoft-Verkäufer zu erhalten, Empfehlungen zu akzeptieren/ablehnen, Dealdaten wie den Dealwert und das Abschlussdatum zu ändern.  Sie können auch updates von den Microsoft-Verkäufern zu diesen Co-Sell-Deals erhalten. Sie können alle Ihre Empfehlungen nutzen, während Sie innerhalb des CRM Ihrer Wahl arbeiten und nicht in Partner Center.

Die Lösung basiert auf Microsoft Power Automate Solution und verwendet Partner Center APIs.

## <a name="before-you-install---pre-requisites"></a>Voraussetzungen vor der Installation

|**Themen**|**Details**|**Links**|
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Sie benötigen eine gültige MPN-ID.|So treten Sie [MPN bei](https://partner.microsoft.com/)|
|Co-Sell Ready|Ihre IP/Services-Lösung muss co-sell ready sein.|[Verkaufen mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partner Center-Konto|Die MPN-ID, die dem Partner Center Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die Ihrer Co-Sell-Lösung zugeordnet ist. Stellen Sie sicher, dass Ihre Co-Sell-Empfehlungen im Partner Center angezeigt werden, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
|Partner Center-Benutzerrollen|Der Mitarbeiter, der die Connectors installiert und verwendet, muss ein Empfehlungsadministrator sein.|[Zuweisen von Rollen und Berechtigungen zu Benutzern](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Die CRM-Benutzerrolle ist "Systemadministrator" oder "Systemanpasser".|[Zuweisen von Rollen in Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Konto|Erstellen Sie eine neue Produktionsumgebung mit einer Datenbank für Tests, Staging und Produktion. Wenn Sie über eine vorhandene Produktionsumgebung mit einer Datenbank verfügen, kann sie wiederverwendet werden. Der Benutzer, der die Connectorlösung installieren wird, muss über Power Automate Lizenz und Zugriff auf diese Umgebung verfügen. Sie können den Fortschritt überwachen und weitere Informationen [im](https://flow.microsoft.com/) Power Automate, wenn die Installation fehlschlägt. Wählen Sie **unter Lösungen die Option** Verlauf sehen **aus.**|[Erstellen oder Verwalten einer Umgebung](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installation des Salesforce-Pakets für benutzerdefinierte Microsoft-Felder

Um die Empfehlungen über Partner Center Salesforce CRM hinweg zu synchronisieren, muss die Power Automate-Lösung Microsoft-spezifische Empfehlungsfelder eindeutig identifizieren. Diese Abgrenzung bietet Partner-Verkäuferteams die Möglichkeit zu entscheiden, welche Empfehlungen sie für den Co-Selling an Microsoft freigeben möchten.

1. Aktivieren Sie in Salesforce **Notizen,** und fügen Sie sie der Liste der Verkaufschancen hinzu. [Referenz](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Aktivieren **Sie Opportunity-Teams,** indem Sie die folgenden Schritte ausführen:
    - Verwenden Sie unter Setup das Feld **Schnellstart,** um nach Opportunity Team Einstellungen.
    - Definieren Sie die Einstellungen nach Bedarf. [Referenz](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Installieren Sie in Salesforce benutzerdefinierte Felder und Objekte mithilfe des [Paketinstallationsprogramms](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Verwenden Sie dieses Installationsprogramm, um das Paket in einem beliebigen Unternehmen zu installieren.

    >[!NOTE]
    >Wenn Sie in einer Sandbox installieren, müssen Sie den ersten Teil der URL durch `http://test.salesforce.com` ersetzen.

1. Fügen Sie microsoft Solutions in Salesforce der Liste Opportunity related **(Verkaufschance)** hinzu. Wählen Sie nach dem Hinzugefügten das **Schraubenschlüsselsymbol aus,** und aktualisieren Sie die Eigenschaften.

## <a name="best-practice-test-before-you-go-live"></a>Bewährte Methode: Testen, bevor Sie live gehen

Bevor Sie die Power Automate-Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen, müssen Sie die Lösung auf einer CRM-Staginginstanz testen.

- Installieren Sie die Microsoft Power Automate-Lösung in einer Stagingumgebung/CRM-Instanz.

- Erstellen Sie eine Kopie der Lösung, und führen Sie Ihre Konfiguration aus, und Power Automate in der Stagingumgebung anpassen.

- Testen Sie die Lösung in einer Staging-/CRM-Instanz.

- Importieren Sie bei Erfolg als verwaltete Lösung in die Produktionsinstanz.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installieren Partner Center Synchronisierung von Empfehlungen für Salesforce CRM

1. Wechseln Sie [zu Power Automate,](https://flow.microsoft.com) und wählen **Sie in der rechten** oberen Ecke Umgebungen aus. Dadurch werden die verfügbaren CRM-Instanzen gezeigt.

1. Wählen Sie in der Dropdownliste in der oberen rechten Ecke die entsprechende CRM-Instanz aus.

1. Wählen **Sie in** der linken Navigationsleiste Lösungen aus.

1. Wählen Sie **im oberen Menü den Link AppSource** öffnen aus.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Öffnen Sie AppSource.":::

1. Suchen Sie **Partner Center Popupbildschirm nach Empfehlungsconnectors** für Salesforce.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Screenshot: Jetzt kaufen":::

1. Wählen Sie die **Schaltfläche Jetzt holen** und dann Weiter **aus.**

1. Wählen Sie auf der nächsten Seite die Salesforce CRM-Umgebung aus, um die Anwendung zu installieren. Stimmen Sie den Geschäftsbedingungen zu.

1. Sie werden dann zur Seite Manage **your solutions (Lösungen verwalten)** geleitet.  Navigieren Sie zu "Partner Center Empfehlungen", indem Sie die Pfeilschaltflächen unten auf der Seite verwenden. **Die geplante Installation** sollte neben Partner Center Empfehlungslösung angezeigt werden. Die Installation dauert 10 bis 15 Minuten.

1. Navigieren Sie nach Abschluss der Installation zurück zum Power Automate [und](https://flow.microsoft.com) wählen Sie **im linken** Navigationsbereich Lösungen aus. Beachten **Sie, Partner Center Synchronisierung von** Empfehlungen für Salesforce jetzt in der Lösungsliste verfügbar ist.

1. Wählen **Partner Center Synchronisierung von Empfehlungen für Salesforce aus.** Die folgenden Power Automate und Entitäten sind verfügbar:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce-Flows.":::

## <a name="configure-the-solution"></a>Konfigurieren der Projektmappe

1. Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Power Automate.](https://flow.microsoft.com/)

1. Wählen Sie **in der** Dropdownliste Umgebungen in der oberen rechten Ecke die CRM-Instanz aus, in der Sie die Power Automate installiert haben.

1. Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:

   - Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen
   - Partner Center-Ereignisse
   - CRM-Administrator mit den Power Automate Flows in der Lösung

   1. Wählen **Sie in** der linken Navigationsleiste Verbindungen aus, und wählen Sie Partner Center Lösung **Empfehlungen** aus der Liste aus.

   1. Erstellen Sie eine Verbindung, indem Sie **Verbindung erstellen auswählen.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot: Verbindung erstellen":::

   1. Suchen Sie **Partner Center In der** Suchleiste in der oberen rechten Ecke nach Empfehlungen (Vorschau).

   1. Erstellen Sie eine Verbindung für Ihren Partner Center benutzer mit der Rolle Anmeldeinformationen des Empfehlungsadministrators.

   1. Erstellen Sie als Nächstes eine Partner Center Events-Verbindung für Ihren Partner Center-Benutzer mit den Anmeldeinformationen des Empfehlungsadministrators.

   1. Erstellen Sie eine Verbindung für Salesforce für den CRM-Administratorbenutzer.
  
   1. Erstellen Sie eine Verbindung für Microsoft Dataverse für den CRM-Administratorbenutzer.

   1. Nachdem Sie alle Verbindungen hinzugefügt haben, sollten die folgenden Verbindungen in Ihrer Umgebung zu sehen sein:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Screenshot, der zeigt, wie Verbindungen beobachtet werden.":::

### <a name="edit-the-connections"></a>Bearbeiten der Verbindungen

1. Kehren Sie zur **Seite Lösungen zurück,** und wählen Sie **Standardlösung aus.** Wählen **Sie Verbindungsverweis (Vorschau) aus,** indem Sie auf **Alle klicken.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot: Bearbeiten der Verbindungen":::

1. Bearbeiten Sie die einzelnen Verbindungen einzeln, indem Sie auf das Symbol mit den Auslassungszeichen klicken. Fügen Sie die relevanten Verbindungen hinzu.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Screenshot: Bearbeiten von Connectors":::

1. Aktivieren Sie die Flows in der folgenden Reihenfolge:
   - Partner Center Webhookregistrierung (Insider Preview)
   - [Anpassen] Erstellen oder Abrufen von Details aus Salesforce
   - Erstellen eines Co-Selling-Referral-Salesforce an Partner Center (Insider Preview)
   - Partner Center Microsoft Co-Selling-Empfehlungsupdates für Salesforce (Insider Preview)  
   - Partner Center zu Salesforce (Insider Preview)
   - Salesforce zu Partner Center (Insider Preview)
   - Salesforce Opportunity to Partner Center (Insider Preview)
   - Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von Webhook-APIs zum Registrieren für Ressourcenänderungsereignisse

Sie können die Partner Center-Webhook-APIs verwenden, um sich für Ressourcenänderungsereignisse zu registrieren. Diese Änderungsereignisse werden als HTTP-Beiträge an Ihre URL gesendet.

1. Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.

1. Wählen Sie das **Symbol Bearbeiten** und dann Beim Empfang **einer HTTP-Anforderung** aus.

1. Wählen Sie das **Symbol Kopieren** aus, um die angegebene **HTTP POST-URL** zu kopieren.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Screenshot: Kopieren der URL":::

1. Wählen Sie die **Partner Center Webhookregistrierung (Insider Preview)** Power Automate Flow und dann **Ausführen** aus.

1. Stellen Sie sicher, dass das Fenster **Flow ausführen** im rechten Bereich geöffnet wird, und wählen Sie **Weiter** aus.

1. Geben Sie die folgenden Details ein:

   - **HTTP-Triggerendpunkt:** Diese URL wurde aus einem früheren Schritt kopiert.
   - **Zu registrierende Ereignisse:** Wählen Sie alle verfügbaren Ereignisse aus (**von der Empfehlung erstellt,** mit **Verweis aktualisiert,** **related-referral-created** und **related-referral-updated**).
   - **Vorhandene Triggerendpunkte überschreiben, falls vorhanden?**: Ja. Für ein bestimmtes Webhookereignis kann nur eine URL registriert werden.

1. Wählen Sie **Flow ausführen** und dann **Fertig** aus.

Der Webhook kann jetzt Ereignisse abhören, erstellen und aktualisieren.

## <a name="customize-synchronization-steps"></a>Anpassen der Synchronisierungsschritte

CRM-Systeme sind stark angepasst, und Sie können die Power Automate Lösung basierend auf Ihrem CRM-Setup anpassen. Wenn Co-Selling-Empfehlungen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center PC synchronisiert werden, im [Leitfaden Benutzerdefinierte Feldzuordnung](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)aufgeführt.

Befolgen Sie die Anleitung für die Feldzuordnung, und nehmen Sie bei Bedarf entsprechende Änderungen in **[Anpassen] Erstellen oder Abrufen von Details aus Salesforce** oder Umgebungsvariablen vor. Aktualisieren Sie keine anderen Flows in der Power Automate Lösung, da sich dies auf zukünftige Lösungsupgrades auswirken kann.

Die folgenden Anpassungen sind verfügbar:

- **Häkchen im Verkaufschancennamen anzeigen:** Standardmäßig wird neben dem Verkaufschancennamen ein Häkchen angezeigt, um anzugeben, dass die Synchronisierung zwischen Partner Center und Salesforce CRM erfolgreich durchgeführt wird. Ebenso wird eine Kreuzmarkierung angezeigt, wenn die Synchronisierung fehlschlägt. Um das Hinzufügen eines Häkchens oder Kreuzstrichs im Verkaufschancennamen zu vermeiden, legen Sie den aktuellen Wert des **Häkchens Anzeigen in der** Umgebungsvariablen opportunity name auf Nein fest.

- **Phasenname:**

  - Name der **aktiven Phase:** Dies ist die Phase in der Verkaufspipeline einer Verkaufschance in Salesforce.  Sie stellt eine aktive Phase dar und entspricht einer Empfehlung im akzeptierten Zustand in Partner Center. Dies kann die nächste Phase in der Vertriebspipeline nach der Zurückhaltungsphase sein. Wenn Die Verkaufsphase der Verkaufschance aus der Zurückhaltungsphase in die aktive Phase verschoben wird, wird die Empfehlung in Partner Center akzeptiert, und die Änderungen beginnen mit der Synchronisierung.

  - Name der **zurückgehaltenen Phase:** Name der Phase in der Verkaufspipeline einer Verkaufschance in Salesforce. Es stellt eine Zurückhaltungsphase dar. Neue, von Microsoft freigegebene Co-Selling-Empfehlungen, die noch nicht akzeptiert wurden, werden in Salesforce auf diese Phase festgelegt. Änderungen an einer Verkaufschance während der Zurückhaltungsphase werden nicht mit Partner Center synchronisiert. Wenn sie die Verkaufsphase der Verkaufschance aus dieser Zurückhaltungsphase verschieben, wird die Empfehlung in Partner Center akzeptiert, und die Änderungen beginnen mit der Synchronisierung.

- **Ländercode** des Kundenkontos: Bei der Erstellung einer neuen Empfehlung ist es obligatorisch, einen zweistelligen Ländercode (ISO 3166) anzugeben. Standardmäßig wird der Ländercode mit und aus dem Feld **BillingCountry** des Kontos in Salesforce synchronisiert. Wenn Sie in Salesforce ein anderes Feld für den Ländercode haben, aus dem synchronisiert werden soll:

  - Für ein feld nicht absteigendes Ländercodefeld in dem Konto, das einen aus zwei Buchstaben besteht:

    - Aktualisieren Sie den Feldnamen des **Kundenkonto-Ländercodes** in der Salesforce-Umgebungsvariablen mit dem Feldnamen des CRM. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.

    - Bearbeiten Sie **[Anpassen] Erstellen oder Abrufen von Details aus Salesforce,** und wechseln Sie zu **Kundenkonto in CRM-Aktion erstellen oder abrufen,** um dem richtigen Feld im CRM einen **Länderwert** zuzuweisen. Entfernen Sie außerdem die **Wertzuweisung Country** aus **BillingCountry**.

  - Für ein nachschlagende Ländercodefeld im Konto:

    - Fügen Sie dem Konto ein neues benutzerdefiniertes Feld hinzu, und füllen Sie es automatisch mit einem zweistelligen Ländercode (ISO 3166) auf, der auf dem wert basiert, der im suchbasierten Feld ausgewählt wurde (und umgekehrt).

    - Führen Sie die vorherigen Schritte für das Feld für den Nicht-Abgleich des Ländercodes aus, um ein neues benutzerdefiniertes Feld aus dem CRM mit und aus Partner Center zu synchronisieren.

- **Dealwert:** Standardmäßig wird der Dealwert von Partner Center mit und von **Amount** im CRM synchronisiert. Wenn im CRM ein anderes Feld für den Dealwert vorhanden ist, aus dem synchronisiert werden soll:

  - Aktualisieren Sie den Feldnamen **des Deal-Werts** in der Salesforce-Umgebungsvariablen mit dem Feldnamen des CRM. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.

  - Bearbeiten **Sie [Anpassen] Erstellen oder Abrufen von Details aus Salesforce,** und wechseln Sie zu Create or update opportunity in CRM **(Erstellen oder Aktualisieren** einer Verkaufschance in CRM), und aktualisieren Sie die Aktionen **Create a new opportunity (Neue Verkaufschance erstellen)** und Update existing opportunity actions **(Vorhandene Verkaufschancen** aktualisieren), um **DealValue** dem richtigen Feld in Salesforce zuzuweisen.

- **Währungscode** des Dealwerts: Name des Währungscodefelds für den Dealwert in Salesforce. Dieser Feld-API-Name wird verwendet, um den Geschäftswertcode der Verkaufschance beim Erstellen oder Aktualisieren von Empfehlungen in Microsoft Partner Center abzurufen. Wenn sich das Währungscodefeld für den Dealwert vom Standardfeld **CurrencyIsoCode** unterscheidet, aktualisieren Sie den aktuellen Wert dieser Umgebungsvariablen.

  - Aktualisieren Sie den Namen des **Felds** Deal value currency in der Salesforce-Umgebungsvariablen mit dem Feldnamen des CRM. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.

  - Bearbeiten **Sie [Anpassen] Erstellen oder Abrufen von Details aus Salesforce,** und wechseln Sie zu Verkaufschance in CRM **erstellen oder aktualisieren,** und aktualisieren Sie die Aktionen **Create a new opportunity (Neue Verkaufschance erstellen)** und **Update existing opportunity (Vorhandene Verkaufschance aktualisieren),** um **DealValueCurrency** dem richtigen Feld in Salesforce zuzuweisen.

- **Co-Selling-Verkaufschance** synchronisieren: Wenn **ja** festgelegt ist, werden nur Co-Selling- und Pipelinefreigabemöglichkeiten von Partner Center mit Salesforce synchronisiert. Wenn **kein** festgelegt ist, werden Leads, Co-Selling- und Pipelinefreigabemöglichkeiten von Partner Center mit Salesforce synchronisiert. Diese Variable hat keine Auswirkungen auf die Verkaufschancen, die von Salesforce mit Partner Center synchronisiert werden.

## <a name="update-environment-variable"></a>Aktualisieren der Umgebungsvariablen

So aktualisieren Sie einen Umgebungsvariablenwert:

1. Wechseln Sie zur Seite **Lösungen,** und wählen Sie **Standardlösung** aus. Wählen Sie **Umgebungsvariable** aus, indem Sie **Alle** auswählen.

1. Wählen Sie die Umgebungsvariable für den Wert aus, der aktualisiert werden muss, und wählen **Sie bearbeiten** aus, indem Sie das Symbol mit den Auslassungszeichen verwenden.

1. Aktualisieren Sie **den aktuellen Wert** (nicht den **Standardwert** aktualisieren), indem Sie die Option **Neuer Wert** verwenden und den Wert bereitstellen. Der Wert muss mit dem Datentyp der Variablen übereinstimmen. Beispielsweise akzeptiert der Datentyp Ja oder Nein entweder den Wert Ja oder Nein.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Screenshot: Aktualisieren von Umgebungsvariablen":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Bidirektionale End-to-End-Co-Selling-Empfehlungssynchronisierung

Nachdem Sie die Power Automate Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Empfehlungen zwischen Salesforce CRM und Partner Center testen.

### <a name="pre-requisites"></a>Voraussetzungen

Um die Empfehlungen über Partner Center und Salesforce CRM hinweg zu synchronisieren, muss die Power Automate Lösung microsoftspezifische Empfehlungsfelder eindeutig abgrenzen. Diese Identifizierung bietet Ihren Verkäuferteams die Möglichkeit, zu entscheiden, welche Empfehlungen sie für den Co-Selling mit Microsoft teilen möchten.

Eine Reihe von benutzerdefinierten Feldern ist als Teil Partner Center Entität Empfehlungssynchronisierung für Salesforce CRM-Lösung **Opportunity** verfügbar. Ein CRM-Administratorbenutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern **Opportunity** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center:** Gibt an, ob die Verkaufschance mit Partner Center synchronisiert werden soll. Standardmäßig ist der Wert dieses Felds Nein und muss von Ihrem Verkäufer explizit auf Ja festgelegt werden, um eine Verkaufschance für Microsoft freizugeben. Für neue Empfehlungen, die von Partner Center an CRM freigegeben werden, wird dieser Feldwert auf Ja festgelegt.

- **Empfehlungsbezeichner:** Ein schreibgeschütztes Bezeichnerfeld für Microsoft Partner Center-Empfehlung.

- **Empfehlungslink:** Ein schreibgeschützter Link zur Empfehlung in Microsoft Partner Center.

- **Wie kann Microsoft helfen:** Hilfe, die von Microsoft für die Empfehlung benötigt wird. Um eine Co-Selling-Empfehlung zu erstellen, wählen Sie die entsprechende Hilfe aus, die von Microsoft benötigt wird. Ein Kundenkontakt muss der Möglichkeit zugeordnet werden, eine Co-Selling-Empfehlung zu erstellen. Um eine Nicht-Co-Selling-Empfehlung zu erstellen, wählen Sie dieses Feld nicht aus. Eine Nicht-Co-Selling-Empfehlung kann jederzeit in eine Co-Selling-Empfehlung konvertiert werden, indem die entsprechende Option für die erforderliche Hilfe ausgewählt wird.

- **Microsoft Partner Center-Empfehlungssichtbarkeit:** Wählen Sie Sichtbarkeit für die Partner Center Empfehlung aus. Wenn sie für Microsoft-Verkäufer sichtbar gemacht wird, kann eine Nicht-Co-Sell-Empfehlung in Co-Sell konvertiert werden. Wenn Microsoft-Hilfe erforderlich ist, ist die Empfehlung standardmäßig für Microsoft-Verkäufer sichtbar. Nachdem dieses Feld als sichtbar markiert wurde, kann es nicht mehr rückgängig gemacht werden.

- **Microsoft CRM Bezeichner:** Wenn eine Co-Sell-Empfehlung erstellt und von Microsoft akzeptiert wird, wird dieses Feld mit dem CRM-Bezeichner von Microsoft aufgefüllt.

- **Microsoft Partner Center Solutions:** Ein benutzerdefiniertes Objekt, um Co-Sell-bereite Lösungen oder Microsoft-Lösungen der Verkaufschance zu zuordnen. Eine oder mehrere Lösungen können hinzugefügt oder aus der Verkaufschance entfernt werden. Es ist obligatorisch, der Verkaufschance mindestens eine Co-Sell Ready- oder Microsoft-Lösung hinzuzufügen, bevor Sie sie mit Microsoft teilen. Um dieses Objekt der Verkaufschance zu zuordnen, aktualisieren Sie das **Formular Verkaufschance** im CRM.

- **Überwachung:** Ein schreibgeschützter Überwachungspfad für die Synchronisierung mit Partner Center Empfehlungen

### <a name="scenarios"></a>Szenarien

1. Empfehlungssynchronisierung beim Erstellen oder Aktualisieren von Empfehlungen in CRM und Synchronisierung in Partner Center:

   1. Melden Sie sich bei Ihrer Salesforce CRM-Umgebung mit einem Benutzer an, der über Sichtbarkeit im Abschnitt **Verkaufschance** des CRM verfügt.

   1. Stellen Sie sicher, dass der Abschnitt **Microsoft Partner Center** vorhanden ist, wenn Sie eine **neue Verkaufschance** in einer Salesforce CRM-Umgebung erstellen.

   1. Verkaufschancen, die erfolgreich mit dem Partner Center synchronisiert werden, werden mit dem ✔ in Salesforce CRM identifiziert.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Screenshot der Salesforce-Umgebung":::

   1. Um diese Verkaufschance mit Microsoft Partner Center zu synchronisieren, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

      - **Wie kann Microsoft helfen?**: Wählen Sie eine geeignete Hilfeoption aus, um eine Co-Sell-Empfehlung zu erstellen.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Screenshot: Anzeigen der entsprechenden Felder in der Kartenansicht":::

      - **Sync with Partner Center**: Ja
      - **Kundenkontakt:** Fügen Sie der Verkaufschance einen Kundenkontakt hinzu, um eine Co-Sell-Empfehlung zu erstellen.
      - **Microsoft Solutions:** Um eine Empfehlung mit Microsoft zu teilen, fügen Sie der Verkaufschance eine gültige Co-Sell Ready- oder Microsoft-Lösung hinzu.

   1. Nachdem Sie die Option Sync **with Partner Center** auf Ja festgelegt **haben,** warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center an. Ihre Empfehlungen werden mit Salesforce CRM synchronisiert, und der Empfehlungslink wird aufgefüllt. Wenn ein Fehler auftritt, wird das Feld Überwachung mit Fehlerinformationen aufgefüllt.

   1. Wenn die Option **Sync with Partner Center** auf Ja festgelegt ist, werden die Änderungen mit Ihrem Partner Center synchronisiert, wenn Sie die Verkaufschance in Salesforce CRM aktualisieren.

2. Empfehlungssynchronisierung, wenn die Empfehlung in Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:

    1. Melden Sie sich bei Ihrem [Partner Center-Dashboard an.](https://partner.microsoft.com/dashboard/home)

    1. Wählen **Sie im menü auf** der linken Seite die Option Empfehlungen aus.

    1. Erstellen Sie eine neue Co-Sell-Empfehlung aus Partner Center indem Sie auf die Option "Neuer Deal" klicken.

    1. Melden Sie sich bei Ihrer Salesforce CRM-Umgebung an.

    1. Navigieren Sie zu **Open Opportunities (Verkaufschancen öffnen).** Die im Microsoft Partner Center erstellte Empfehlung wird jetzt in Salesforce CRM synchronisiert.

    1. Wenn Sie eine synchronisierte Empfehlung auswählen, werden die Details der Kartenansicht aufgefüllt.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Screenshot der Salesforce-Verkaufschanceseite":::

>[!NOTE]
>**Benötigen Sie Hilfe bei der Bereitstellung?**
>Um Unterstützung bei der Bereitstellung Ihres Co-Sell-Empfehlungsconnectors zu erhalten, können Sie sich an einen technischen Berater des Partners wenden. Sie können Unterstützung bei der Bereitstellung und bewährte Methoden für eine erfolgreiche Implementierung bereitstellen.
>
>Weitere Informationen finden Sie unter Übermitteln einer Anforderung für technische [Presales- und Bereitstellungsdienste.](technical-benefits.md)

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)

- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)

- [Partner Center-Webhooks](/partner-center/develop/partner-center-webhooks)
