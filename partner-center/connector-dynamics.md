---
title: Der Co-Sell-Connector für Dynamics 365 CRM Partner Center
description: Synchronisieren Sie Empfehlungen in Partner Center mit Ihrem Co-Sell-Connector für Dynamics 365 CRM. Sie können dann in Ihrem CRM-System co-sell mit Microsoft verkaufen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425088"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Übersicht über den Co-Sell-Connector für Dynamics 365 CRM

**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Systemadministrator oder Systemanpasser im CRM

Partner Center Co-Sell-Connectors ermöglichen Es Ihren Verkäufern, in Ihren CRM-Systemen gemeinsam mit Microsoft zu verkaufen. Sie müssen nicht trainiert werden, um co-Partner Center zu verwalten. Verwenden Sie die Co-Sell-Connectors, um eine neue Co-Sell-Empfehlung zu erstellen, um einen Microsoft-Verkäufer zu kontaktieren, Empfehlungen vom Microsoft-Verkäufer zu erhalten, Empfehlungen zu akzeptieren oder zu ablehnen und Dealdaten wie Den Dealwert und Abschlussdatum zu ändern. Sie können auch updates von den Microsoft-Verkäufern zu diesen Co-Sell-Deals erhalten. Sie können alle Ihre Empfehlungen im CRM Ihrer Wahl verwalten und nicht in Partner Center.

Die Lösung basiert auf Power Automate und verwendet Partner Center APIs.

## <a name="prerequisites"></a>Voraussetzungen

Stellen Sie vor der Installation der Lösung sicher, dass die folgenden Voraussetzungen erfüllt sind.

|**Themen**   |**Details**   |**Links**   |
|--------------|--------------------|------|
|MPN-ID (Microsoft Partner Network) |Sie benötigen eine gültige MPN-ID.|[Beitreten zum Partnernetzwerk](https://partner.microsoft.com/)|
|Co-Sell Ready|Ihre IP/Services-Lösung muss co-sell ready sein.|[Verkaufen mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partner Center-Konto|Die MPN-ID, die dem Partner Center Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die Ihrer Co-Sell-Lösung zugeordnet ist. Vergewissern Sie sich, dass Ihre Co-Sell-Empfehlungen im Partner Center angezeigt werden, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
|Partner Center-Benutzerrollen|Der Mitarbeiter, der die Connectors installiert und verwendet, muss ein Empfehlungsadministrator sein.|[Zuweisen von Rollen und Berechtigungen zu Benutzern](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Die CRM-Benutzerrolle ist Systemadministrator oder Systemanpasser.|[Zuweisen von Rollen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate Flowkonto|Erstellen Sie eine neue Produktionsumgebung mit einer Datenbank für Tests, Staging und Produktion. Wenn Sie über eine vorhandene Produktionsumgebung mit einer Datenbank verfügen, kann sie wiederverwendet werden. Der Benutzer, der die Connectorlösung installieren wird, muss über eine Lizenz Power Automate Zugriff auf diese Umgebung verfügen. Sie können den Fortschritt überwachen und weitere Informationen [im](https://flow.microsoft.com/) Power Automate, wenn die Installation fehlschlägt. Wählen Sie **unter Lösungen die Option** Verlauf sehen **aus.**|[Erstellen oder Verwalten einer Umgebung](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installieren Partner Center Synchronisierung von Empfehlungen für Dynamics 365 (Power Automate Lösung)

1. Wechseln Sie [Power Automate](https://flow.microsoft.com), und wählen **Sie** oben rechts Umgebungen aus. In diesem Schritt werden die verfügbaren CRM-Instanzen gezeigt.

1. Wählen Sie in der Dropdownliste in der oberen rechten Ecke die entsprechende CRM-Instanz aus.

1. Wählen **Sie auf der** linken Seite Lösungen aus.

1. Wählen Sie **im oberen Menü den Link AppSource** öffnen aus.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Screenshot: Open AppSource":::

1. Suchen Sie **Partner Center Popupbildschirm nach Empfehlungsconnectors für Dynamics 365.**  

1. Wählen Sie die **Schaltfläche Jetzt holen** und dann Weiter **aus.**

1. Es wird eine Seite angezeigt, auf der Sie die CRM-Umgebung (Dynamics 365) auswählen können, um die Anwendung zu installieren. Stimmen Sie den Geschäftsbedingungen zu.

1. Sie können den Fortschritt überwachen. Wenn bei der Installation ein Fehler auftritt,  können Sie weitere Details in Power Automate, indem Sie unter Lösungen die Option Verlauf **anzeigen auswählen.**

1. Wechseln Sie nach Abschluss der Installation zurück zu Power Automate [und](https://flow.microsoft.com) wählen Sie auf der linken **Seite Lösungen** aus. **Partner Center Synchronisierung von Empfehlungen für Dynamics 365** ist jetzt in der **Lösungsliste** verfügbar.

1. Wählen **Partner Center Empfehlungssynchronisierung für Dynamics 365 aus.** Die folgenden Power Automate und Entitäten sind verfügbar.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Screenshot: verfügbare CRMs":::

## <a name="test-before-you-go-live"></a>Testen, bevor Sie live gehen

Bevor Sie die Lösung installieren, konfigurieren und Power Automate in der Produktionsumgebung anpassen, müssen Sie die Lösung auf einer CRM-Staginginstanz testen. Folgendes ist erforderlich:

- Installieren Sie die Power Automate-Lösung in einer CRM-Instanz der Stagingumgebung.
- Konfigurieren und anpassen sie Power Automate Lösung in einer Stagingumgebung.
- Testen Sie die Lösung in einer CRM-Staginginstanz.
- Importieren Sie nach einem erfolgreichen Test als verwaltete Lösung in die Produktionsinstanz.

## <a name="configure-the-solution"></a>Konfigurieren der Projektmappe

1. Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, wechseln Sie zurück zu [Power Automate.](https://flow.microsoft.com/)

1. Wählen Sie **in der** Dropdownliste Umgebungen in der oberen rechten Ecke die CRM-Instanz aus, in der Sie die Power Automate installiert haben.

1. Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:

   - Partner Center benutzer mit Administratoranmeldeinformationen für Empfehlungen
   - Partner Center-Ereignisse
   - CRM-Administrator mit den Power Automate Flows in der Lösung

   1. Klicken **Sie auf** der linken Seite auf Verbindungen, und wählen Sie Partner Center Lösung **Empfehlungen** aus der Liste aus.

   1. Erstellen Sie eine Verbindung, indem Sie **Verbindung erstellen auswählen.**

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot: Erstellen einer Verbindung":::

   1. Suchen Sie **Partner Center In der** Suchleiste in der oberen rechten Ecke nach Empfehlungen (Vorschau).

   1. Erstellen Sie eine Verbindung für Ihren Partner Center benutzer mit der Rolle Anmeldeinformationen des Empfehlungsadministrators.

   1. Erstellen Sie als Nächstes eine Partner Center Events-Verbindung für Ihren Partner Center-Benutzer mit den Administratoranmeldeinformationen für Empfehlungen.

   1. Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administratorbenutzer.
     
   1. Nachdem Sie alle Verbindungen hinzugefügt haben, sollten die folgenden Verbindungen in Ihrer Umgebung zu sehen sein.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Screenshot: Verbindungen":::

## <a name="edit-the-connections"></a>Bearbeiten der Verbindungen

1. Kehren Sie zur **Seite Lösungen zurück,** und wählen Sie **Standardlösung aus.** Wählen **Sie Verbindungsverweis (Vorschau) aus,** indem Sie Alle **auswählen.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot: Bearbeiten der Verbindungen":::

1. Bearbeiten Sie jede der Verbindungen einzeln, indem Sie auf das Symbol mit den Auslassungszeichen klicken. Fügen Sie die relevanten Verbindungen hinzu.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Screenshot, der die aufgelisteten Verbindungen zeigt.":::

1. Kehren  Sie zur Seite Lösungen zurück, wählen Sie **Partner Center Referrals Synchronization for Dynamics 365 (Empfehlungssynchronisierung für Dynamics 365)** aus, und aktivieren Sie den Flow, indem Sie in der folgenden Sequenz neben jedem Flow auf das Symbol mit den Auslassungszeichen klicken. Wenn beim Aktivieren des Datenflusses Probleme auftreten, finden Sie weitere Informationen unter [Anpassungsschritte und](connector-dynamics.md#customize-synchronization-steps) [Problembehandlungsschritte.](connectors-troubleshoot.md)

Aktivieren Sie die Flows in der folgenden Reihenfolge:

- Partner Center Webhookregistrierung (Insider Preview)
- Erstellen einer Co-Sell-Empfehlung – Dynamics 365 to Partner Center (Insider Preview)
- [Anpassen] Erstellen oder Erhalten von Details aus dem Dynamics 365-Flow
- Partner Center Dynamics 365 – Helper (Insider Preview)
- Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)
- Partner Center to Dynamics 365 (Insider Preview)
- Dynamics 365 to Partner Center (Insider Preview)
- Dynamics 365 Opportunity to Partner Center (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von Webhook-APIs zum Registrieren für Ressourcenänderungsereignisse

Sie können die Partner Center-Webhook-APIs verwenden, um sich für Ressourcenänderungsereignisse zu registrieren. Diese Änderungsereignisse werden als HTTP-Beiträge an Ihre URL gesendet.

1. Wählen Sie **Partner Center zu Dynamics 365 (Insider Preview)** aus.

1. Wählen Sie das Symbol **Bearbeiten** und dann **When a HTTP request is received (Wenn eine HTTP-Anforderung empfangen wird)** aus.

1. Wählen Sie das Symbol **Kopieren** aus, um die angegebene HTTP POST-URL zu kopieren.

   :::image type="content" source="images/webhook-video.gif" alt-text="Screenshot: Verwenden von Webhooks zum Registrieren von Ressourcenänderungen":::

1. Wählen Sie **die Partner Center Webhookregistrierung (Insider Preview)** Power Automate Flow und dann **Ausführen** aus.

1. Stellen Sie sicher, dass das Fenster **Flow ausführen** im rechten Bereich geöffnet wird, und wählen Sie **Weiter** aus.

1. Geben Sie die folgenden Details ein:

   - **HTTP-Triggerendpunkt:** Diese URL wurde aus einem früheren Schritt kopiert.
   - **Zu registrierende Ereignisse:** Wählen Sie alle verfügbaren Ereignisse aus (**von der Empfehlung erstellt,** mit **Verweis aktualisiert,** **related-referral-created** und **related-referral-updated**).
   - **Vorhandene Triggerendpunkte überschreiben, falls vorhanden?**: Ja. Für ein bestimmtes Webhookereignis kann nur eine URL registriert werden.

1. Wählen Sie **Flow ausführen** und dann **Fertig aus.**

Der Webhook kann jetzt Ereignisse abhören, erstellen und aktualisieren.

## <a name="customize-synchronization-steps"></a>Anpassen der Synchronisierungsschritte

CRM-Systeme sind stark angepasst, und Sie können die Power Automate Lösung basierend auf Ihrem CRM-Setup anpassen. Wenn Co-Selling-Empfehlungen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center PC synchronisiert werden, im [Leitfaden Benutzerdefinierte Feldzuordnung](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)aufgeführt.

Befolgen Sie die Anleitung für die Feldzuordnung, und nehmen Sie bei Bedarf entsprechende Änderungen in **[Anpassen] Erstellen oder Abrufen von Details aus dynamics 365-Fluss-** oder Umgebungsvariablen vor. Aktualisieren Sie keine anderen Flows in der Power Automate Lösung, da sich dies auf zukünftige Lösungsupgrades auswirken kann.

Die folgenden Anpassungen sind verfügbar:

- **Häkchen im Verkaufschancennamen anzeigen:** Standardmäßig wird neben dem Verkaufschancennamen ein Häkchen angezeigt, um anzugeben, dass die Synchronisierung zwischen Partner Center und Dynamics 365 CRM erfolgreich durchgeführt wird. Ebenso wird eine Kreuzmarkierung angezeigt, wenn die Synchronisierung fehlschlägt. Um das Hinzufügen eines Häkchens oder Kreuzstrichs im Verkaufschancennamen zu vermeiden, legen Sie den aktuellen Wert des **Häkchens Anzeigen in der** Umgebungsvariablen opportunity name auf Nein fest.
- **Deal-Wert:** Standardmäßig wird der Dealwert aus Partner Center mit und von **estimatedvalue** im CRM synchronisiert. Wenn im CRM ein anderes Feld für den Dealwert enthalten ist, der synchronisiert werden soll:

  - Aktualisieren Sie den **Feldnamen des Deal-Werts** in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen des CRM. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.
  - Bearbeiten **Sie [Anpassen] Erstellen oder Abrufen von Details aus dem Dynamics 365-Flow,** und wechseln Sie zu Verkaufschance in CRM **erstellen oder aktualisieren,** und aktualisieren **Sie Create a new opportunity (Neue Verkaufschance erstellen)** und Update existing opportunity actions **(Vorhandene Verkaufschancenaktionen aktualisieren),** um den **DealValue-Wert** dem richtigen Feld im CRM zuzuweisen. Entfernen Sie außerdem die **DealValue-Zuweisung** aus dem Feld **Geschätzter Umsatz.**

- **Ländercode** des Kundenkontos: Es ist obligatorisch, einen zweistelligen Ländercode (ISO 3166) anzugeben, wenn Sie eine neue Empfehlung erstellen. Standardmäßig wird der Ländercode mit dem feld **address1_country** des Kontos im CRM synchronisiert. Wenn sie im CRM ein anderes Feld für den Ländercode haben, aus dem synchronisiert werden soll:

  - Für ein feld nicht absteigendes Ländercodefeld im Konto, das einen aus zwei Buchstaben besteht:
    - Aktualisieren Sie den Feldnamen des Ländercodes des **Kundenkontos** in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen des CRM. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.
    - Bearbeiten Sie **[Anpassen] Erstellen oder Abrufen von Details aus dem Dynamics 365-Flow,** und wechseln Sie in der CRM-Aktion zu **Kundenkonto erstellen oder abrufen,** um dem richtigen Feld im CRM einen **Länderwert** zuzuweisen. Entfernen Sie außerdem die **Wertzuweisung Country** aus dem Feld **Adresse 1: Land/Region.**

  - Für ein nachschlagende Ländercodefeld im Konto:
    - Fügen Sie dem Konto ein neues benutzerdefiniertes Feld hinzu, und füllen Sie es automatisch mit einem zweistelligen Ländercode (ISO 3166) auf, der auf dem wert basiert, der im suchbasierten Feld ausgewählt wurde (und umgekehrt).
    - Führen Sie die vorherigen Schritte für das Feld für den Nicht-Abgleich des Ländercodes aus, um ein neues benutzerdefiniertes Feld aus dem CRM mit und aus Partner Center zu synchronisieren.

- **Verkaufschancenfelder:** Wenn pflichtbare Felder in **Opportunity** vorhanden sind, die aufgefüllt werden müssen, bearbeiten Sie **[Anpassen] Erstellen oder Details aus Dynamics 365 abrufen,** und wechseln Sie im CRM zu Erstellen oder Aktualisieren einer **Verkaufschance,** und aktualisieren Sie die **Aktion Neue Verkaufschance** erstellen, um den Pflichtfeldern Werte basierend auf Ihren Geschäftsanforderungen zuzuweisen.
- **Leadfelder:** Wenn im **Lead** Pflichtfelder vorhanden sind, die aufgefüllt werden müssen, bearbeiten Sie **[Anpassen] Erstellen oder Abrufen von Details aus dem Dynamics 365-Flow,** und wechseln Sie im CRM zu **Lead erstellen oder aktualisieren** und aktualisieren Sie die Aktion Neuen **Lead** erstellen, um den Pflichtfeldern Werte basierend auf Ihren Geschäftsanforderungen zuzuweisen.
- **Kundenkonto:** Wenn eine neue Empfehlung von Partner Center mit dem CRM synchronisiert wird, versucht die Power Automate-Lösung, mithilfe des Kundenunternehmensnamens und der Postleitzahl nach einem vorhandenen Konto im CRM zu suchen. Wenn kein Kundenkonto gefunden wird, wird im CRM ein neues Kundenkonto erstellt. Um die Suchkriterien und details zur Erstellung neuer Konten zu aktualisieren, bearbeiten Sie **[Anpassen] Erstellen oder Abrufen von Details aus dem Dynamics 365-Flow,** und wechseln Sie in der CRM- und **Create customer account-Aktion** zu Erstellen oder Abrufen eines **Kundenkontos.**

## <a name="update-environment-variable"></a>Aktualisieren der Umgebungsvariablen

So aktualisieren Sie einen Umgebungsvariablenwert:

1. Wechseln Sie zur Seite **Lösungen,** und wählen Sie **Standardlösung** aus. Wählen Sie **Umgebungsvariable** aus, indem Sie **Alle** auswählen.

1. Wählen Sie die Umgebungsvariable für den Wert aus, der aktualisiert werden muss, und wählen **Sie bearbeiten** aus, indem Sie das Symbol mit den Auslassungszeichen verwenden.

1. Aktualisieren Sie **den aktuellen Wert** (nicht den **Standardwert** aktualisieren), indem Sie die Option **Neuer Wert** verwenden und den Wert bereitstellen. Der Wert muss mit dem Datentyp der Variablen übereinstimmen. Beispielsweise akzeptiert der Datentyp Ja oder Nein entweder den Wert Ja oder Nein.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Screenshot: Aktualisieren von Umgebungsvariablen":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>End-to-End-Synchronisierung bidirektionaler Co-Selling-Empfehlungen

Nachdem Sie die Power Automate Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Empfehlungen zwischen Dynamics 365 und Partner Center testen.

### <a name="prerequisites"></a>Voraussetzungen

Um die Empfehlungen über Partner Center und Dynamics 365 CRM hinweg zu synchronisieren, stellt die Power Automate Lösung eindeutig microsoftspezifische Empfehlungsfelder ab. Diese Identifizierung gibt Ihren Verkäuferteams die Möglichkeit zu entscheiden, welche Empfehlungen sie für den Co-Selling mit Microsoft teilen möchten.

Im Rahmen der Projektmappeninstallation werden benutzerdefinierte Felder und Objekte hinzugefügt. Ein CRM-Administratorbenutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern **Opportunity** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center:** Gibt an, ob die Verkaufschance mit Partner Center synchronisiert werden soll. Standardmäßig ist der Wert dieses Felds Nein und muss von Ihrem Verkäufer explizit auf Ja festgelegt werden, um eine Verkaufschance für Microsoft freizugeben. Für neue Empfehlungen, die von Partner Center an CRM freigegeben werden, wird dieser Feldwert auf Ja festgelegt.
- **Empfehlungsbezeichner:** Ein schreibgeschütztes Bezeichnerfeld für die Partner Center Empfehlung.
- **Empfehlungslink:** Ein schreibgeschützter Link zur Empfehlung in Partner Center.
- **Wie kann Microsoft helfen?**: Hilfe von Microsoft für die Empfehlung erforderlich. Um eine Co-Selling-Empfehlung zu erstellen, wählen Sie die entsprechende Hilfe aus, die von Microsoft benötigt wird. Ein Kundenkontakt muss der Möglichkeit zugeordnet werden, eine Co-Selling-Empfehlung zu erstellen. Um eine Nicht-Co-Selling-Empfehlung zu erstellen, wählen Sie dieses Feld nicht aus. Eine Nicht-Co-Selling-Empfehlung kann jederzeit in eine Co-Selling-Empfehlung konvertiert werden, indem die entsprechende Option für die erforderliche Hilfe ausgewählt wird.
- **Microsoft Partner Center-Empfehlungssichtbarkeit:** Wählen Sie Sichtbarkeit für die Partner Center Empfehlung aus. Indem sie für Microsoft-Verkäufer sichtbar gemacht wird, kann eine Nicht-Co-Selling-Empfehlung in Co-Selling umgewandelt werden. Wenn Microsoft-Hilfe erforderlich ist, ist die Empfehlung standardmäßig für Microsoft-Verkäufer sichtbar. Nachdem dieses Feld als sichtbar markiert wurde, kann es nicht mehr zurückgesetzt werden.
- **Microsoft CRM-Bezeichner:** Wenn eine Co-Selling-Empfehlung von Microsoft erstellt und akzeptiert wird, wird dieses Feld mit dem CRM-Bezeichner von Microsoft aufgefüllt.
- **Produkte: Veraltet:** Verwenden Sie dieses Feld nicht, oder fügen Sie es dem CRM-Abschnitt hinzu. Sie ist nur aus Gründen der Abwärtskompatibilität verfügbar. Verwenden Sie stattdessen Partner Center Lösungen.
- **Audit**: Ein schreibgeschützter Überwachungspfad für die Synchronisierung mit Partner Center Empfehlungen.
- **Microsoft Partner Center Solutions:** Ein benutzerdefiniertes Objekt zum Zuordnen von Co-Selling-Lösungen oder Microsoft-Lösungen. Eine oder mehrere Lösungen können der Verkaufschance hinzugefügt oder daraus entfernt werden. Es ist obligatorisch, der Verkaufschance mindestens eine Co-Selling-bereit- oder Microsoft-Lösung hinzuzufügen, bevor Sie sie mit Microsoft teilen. Um dieses Objekt der Verkaufschance zuzuordnen, aktualisieren Sie das **Formular Opportunity** im CRM.

  Wählen Sie im Formular **Opportunity** die entsprechende Registerkarte aus, und fügen Sie wie hier gezeigt ein Unterraster hinzu.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Screenshot: Formular &quot;Verkaufschance&quot;":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Screenshot: Microsoft-Lösungen":::

- Nachdem Sie Microsoft-Lösungen hinzugefügt haben, können Sie Vorabdetails für die Co-Selling-Lösung auffüllen, damit Ihre Verkäufer sie nicht hinzufügen müssen. Um ein neues Lösungsdetail hinzuzufügen, wechseln Sie zum Microsoft Solution Details-Objekt im CRM, und wählen **Sie Datensatz hinzufügen** aus, um einen Eintrag hinzuzufügen, oder verwenden Sie den **Excel-Upload,** um mehrere Einträge hinzuzufügen.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Screenshot: Details zur neuen Microsoft-Lösung":::

### <a name="scenarios"></a>Szenarien

1. Empfehlungssynchronisierung, wenn die Empfehlung im CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:

   1. Melden Sie sich bei Ihrer Dynamics 365 CRM-Umgebung mit dem Benutzer an, der im Abschnitt **Opportunity** des CRM über Sichtbarkeit verfügt.

   1. Stellen Sie sicher, dass der Abschnitt **Microsoft Partner Center** vorhanden ist, wenn Sie eine neue Verkaufschance in der Dynamics 365-Umgebung erstellen.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Screenshot: Neue Verkaufschance":::

   1. Um diese Verkaufschance mit Partner Center zu synchronisieren, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

      - **Wie kann Microsoft helfen?**: Um eine Co-Selling-Empfehlung zu erstellen, wählen Sie eine geeignete Hilfeoption aus.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Screenshot: Abrufen der entsprechenden Felder in der Kartenansicht":::

      - **Kundenkontakt:** Um eine Co-Selling-Empfehlung zu erstellen, fügen Sie der Verkaufschance einen Kundenkontakt hinzu.
      - **Sync With Partner Center:** Ja.
      - **Microsoft Solutions:** Um eine Empfehlung mit Microsoft zu teilen, fügen Sie der Verkaufschance eine gültige Co-Sell Ready- oder Microsoft-Lösung hinzu.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Screenshot: Projektmappen-ID":::

   1. Nachdem die Verkaufschance in Dynamics 365 mit der Option Sync **With Partner Center** auf Ja festgelegt wurde, warten Sie 10 Minuten. Melden Sie sich dann bei Ihrem Partner Center an. Ihre Empfehlungen werden mit Dynamics 365 und der **Empfehlungs-ID synchronisiert.** **Der Verweislink** wird aufgefüllt. Wenn ein Fehler auftritt, **wird** das Feld Überwachung mit Fehlerinformationen aufgefüllt.

      1. Für eine Verkaufschance, bei der die Option Sync **With Partner Center** (Mit Partner Center synchronisieren) auf Ja festgelegt wurde, werden die Änderungen in Ihrem Partner Center synchronisiert, wenn Sie die Verkaufschance in Dynamics 365 CRM aktualisieren.

      1. Verkaufschancen, die erfolgreich mit dem Partner Center synchronisiert werden, werden mithilfe ✔ in Dynamics 365 identifiziert.

1. Empfehlungssynchronisierung beim Erstellen oder Aktualisieren der Empfehlung in Partner Center und Synchronisierung in der Dynamics 365-Umgebung:

   1. Melden Sie sich bei Ihrem [Partner Center-Dashboard an.](https://partner.microsoft.com/dashboard/home)

   1. Wählen **Sie im menü auf** der linken Seite die Option Empfehlungen aus.

   1. Erstellen Sie eine neue Co-Sell-Empfehlung aus Partner Center, indem Sie die **Option New deal (Neuer Deal)** auswählen.

   1. Melden Sie sich bei Ihrer Dynamics 365 CRM-Umgebung an.

   1. Wechseln Sie zu **Open Opportunities (Verkaufschancen öffnen).** Die in diesem Partner Center erstellte Empfehlung wird jetzt in Dynamics 365 CRM synchronisiert.

   1. Wenn Sie eine synchronisierte Empfehlung auswählen, werden die Details der Kartenansicht aufgefüllt.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)
- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
- [Weitere Informationen zur Microsoft Power Automate-Plattform](/power-automate/)
- [Partner Center-Webhooks](/partner-center/develop/partner-center-webhooks)
