---
title: Der Co-Selling-Connector für Dynamics 365 CRM Partner Center
description: Synchronisieren Sie Empfehlungen in Partner Center mit Ihrem Co-Selling-Connector für Dynamics 365 CRM. Sie können dann in Ihrem CRM-System co-selling mit Microsoft anbieten.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: c399e00394208ec29dd59a41afe7cce1b1d07253
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284331"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Übersicht über den Co-Selling-Connector für Dynamics 365 CRM

**Geeignete Rollen**

- Empfehlungsadministrator
- Systemadministrator oder Systemanpasser im CRM

Partner Center Co-Selling-Connectors ermöglichen ihren Verkäufern das Co-Selling mit Microsoft aus Ihren CRM-Systemen. Sie müssen nicht trainiert werden, um Partner Center zum Verwalten von Co-Selling-Abschlüssen zu verwenden. Verwenden Sie die Co-Selling-Connectors, um eine neue Co-Selling-Empfehlung zu erstellen, um einen Microsoft-Verkäufer einzubinden, Empfehlungen vom Microsoft-Verkäufer zu erhalten, Empfehlungen zu akzeptieren oder abzulehnen und Dealdaten wie den Dealwert und das Enddatum zu ändern. Sie können auch alle Updates von den Microsoft-Verkäufern zu diesen Co-Selling-Abschlüssen erhalten. Sie können alle Ihre Empfehlungen im CRM Ihrer Wahl verwalten, anstatt in Partner Center.

Die Lösung basiert auf Power Automate und verwendet Partner Center-APIs.

## <a name="prerequisites"></a>Voraussetzungen

Stellen Sie vor der Installation der Lösung sicher, dass die folgenden Voraussetzungen erfüllt sind.

|**Themen**   |**Details**   |**Links**   |
|--------------|--------------------|------|
|MPN-ID (Microsoft Partner Network) |Sie benötigen eine gültige MPN-ID.|[Beitreten zum Partner Network](https://partner.microsoft.com/)|
|Co-Sell Ready|Ihre IP/Services-Lösung muss für den Co-Selling bereit sein.|[Verkaufen mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partner Center-Konto|Die MPN-ID, die dem Partner Center Mandanten zugeordnet ist, muss mit der MPN-ID ihrer Co-Selling-Lösung übereinstimmen. Vergewissern Sie sich, dass Ihre Co-Selling-Empfehlungen im Partner Center-Portal angezeigt werden, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
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

1. Sie können den Fortschritt überwachen. Wenn die Installation fehlschlägt, können Sie weitere Details in Power Automate abrufen, indem Sie unter **Lösungen** die Option **Verlauf anzeigen** auswählen.

1. Wechseln Sie nach Abschluss der Installation zurück zu [Power Automate,](https://flow.microsoft.com) und wählen Sie links **Lösungen** aus. **Partner Center Empfehlungssynchronisierung für Dynamics 365** ist jetzt in der Liste **Lösungen** verfügbar.

1. Wählen Sie **Partner Center Synchronisierung von Empfehlungen für Dynamics 365** aus. Die folgenden Power Automate Flows und Entitäten sind verfügbar.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Screenshot: Verfügbare CRMs":::

## <a name="test-before-you-go-live"></a>Testen, bevor Sie live gehen

Bevor Sie die Power Automate Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen, stellen Sie sicher, dass Sie die Lösung auf einer STAGING-CRM-Instanz testen. Folgendes ist erforderlich:

- Installieren Sie die Power Automate Lösung in einer CRM-Instanz in einer Stagingumgebung.
- Konfigurieren und anpassen Sie die Power Automate-Lösung in einer Stagingumgebung.
- Testen Sie die Lösung auf einer STAGING-CRM-Instanz.
- Importieren Sie nach einem erfolgreichen Test als verwaltete Lösung in die Produktionsinstanz.

## <a name="configure-the-solution"></a>Konfigurieren der Projektmappe

1. Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, wechseln Sie zurück zu [Power Automate](https://flow.microsoft.com/).

1. Wählen Sie in der Dropdownliste **Umgebungen** in der oberen rechten Ecke die CRM-Instanz aus, auf der Sie die Power Automate-Lösung installiert haben.

1. Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:

   - Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen
   - Partner Center-Ereignisse
   - CRM-Administrator mit den Power Automate Flows in der Lösung

   1. Klicken Sie auf der linken Seite auf **Verbindungen,** und wählen Sie in der Liste die **Lösung Partner Center Empfehlungen** aus.

   1. Erstellen Sie eine Verbindung, indem **Sie Verbindung erstellen** auswählen.

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

1.  Kehren  Sie zur Seite Lösungen zurück, wählen Sie **Partner Center Referrals Synchronization for Dynamics 365 (Empfehlungssynchronisierung für Dynamics 365)** aus, und aktivieren Sie den Flow, indem Sie in der folgenden Sequenz neben jedem Flow auf das Symbol mit den Auslassungszeichen klicken. Wenn beim Aktivieren des Datenflusses Probleme auftreten, finden Sie weitere Informationen unter [Anpassungsschritte und](connector-dynamics.md#customize-synchronization-steps) [Problembehandlungsschritte.](connectors-troubleshoot.md)

Aktivieren Sie die Flows in der folgenden Reihenfolge:

- Partner Center Webhookregistrierung (Insider Preview)
- Erstellen einer Co-Sell-Empfehlung – Dynamics 365 to Partner Center (Insider Preview)
- [Anpassen] Erstellen oder Erhalten von Details aus dem Dynamics 365-Flow
- Partner Center Dynamics 365 – Helper (Insider Preview)
- Partner Center Microsoft Co-Selling Referral Updates to Dynamics 365 (Insider Preview) (Microsoft Co-Selling-Empfehlungsupdates für Dynamics 365 (Insider Preview))
- Partner Center zu Dynamics 365 (Insider Preview)
- Dynamics 365 to Partner Center (Insider Preview)
- Dynamics 365 Opportunity to Partner Center (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von Webhook-APIs zum Registrieren für Ressourcenänderungsereignisse

Sie können die Partner Center-Webhook-APIs verwenden, um sich für Ressourcenänderungsereignisse zu registrieren. Diese Änderungsereignisse werden als HTTP-Beiträge an Ihre URL gesendet.

1. Wählen Sie **Partner Center zu Dynamics 365 (Insider Preview) aus.**

1. Wählen Sie das Symbol **Bearbeiten** und dann **Beim Empfang einer HTTP-Anforderung** aus.

1. Wählen Sie das Symbol **Kopieren** aus, um die angegebene HTTP POST-URL zu kopieren.

   :::image type="content" source="images/webhook-video.gif" alt-text="Screenshot: Verwenden von Webhooks zum Registrieren von Ressourcenänderungen":::

1. Wählen Sie die **Partner Center Webhookregistrierung (Insider Preview)** Power Automate Flow und dann **Ausführen** aus.

1. Stellen Sie sicher, dass das Fenster **Flow ausführen** im rechten Bereich geöffnet wird, und wählen Sie **Weiter** aus.

1. Geben Sie die folgenden Details ein:

   - **HTTP-Triggerendpunkt:** Diese URL wurde aus einem früheren Schritt kopiert.
   - **Zu registrierende Ereignisse:** Wählen Sie alle verfügbaren Ereignisse aus (**von der Empfehlung erstellt,** mit **Verweis aktualisiert,** **related-referral-created** und **related-referral-updated**).
   - **Vorhandene Triggerendpunkte überschreiben, falls vorhanden?**: Ja. Für ein bestimmtes Webhookereignis kann nur eine URL registriert werden.

1. Wählen Sie **Flow ausführen** und dann **Fertig aus.**

Der Webhook kann jetzt Ereignisse abhören, erstellen und aktualisieren.

## <a name="customize-synchronization-steps"></a>Anpassen von Synchronisierungsschritten

CRM-Systeme sind stark angepasst, und Sie können die Power Automate basierend auf Ihrem CRM-Setup anpassen. Wenn Co-Sell-Empfehlungen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, im Leitfaden benutzerdefinierte [Feldzuordnung aufgeführt.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Befolgen Sie den Leitfaden zur Feldzuordnung, und nehmen Sie bei Bedarf entsprechende Änderungen in [Anpassen] Erstellen oder Erhalten von Details aus **Dynamics 365-Fluss-** oder Umgebungsvariablen vor. Aktualisieren Sie keine anderen Flows in der Power Automate Lösung, da sich dies auf zukünftige Lösungsupgrades auswirken kann.

Die folgenden Anpassungen sind verfügbar:

- **Häkchen** im Namen der Verkaufschance anzeigen: Standardmäßig wird neben dem Namen der Verkaufschance ein Häkchen angezeigt, um anzugeben, dass die Synchronisierung zwischen Partner Center und Dynamics 365 CRM erfolgreich durchgeführt wird. Auf ähnliche Weise wird ein Kreuzzeichen angezeigt, wenn bei der Synchronisierung ein Fehler auftritt. Um das Hinzufügen eines Häkchens oder Kreuzzeichens im Namen der Verkaufschance zu vermeiden, legen Sie den aktuellen Wert des Häkchens Anzeigen **in** der Umgebungsvariablen für den Verkaufschancenamen auf Nein fest.
- **Dealwert:** Standardmäßig wird der Dealwert aus Partner Center mit und aus **dem geschätzten Wert** im CRM synchronisiert. Wenn sie über ein anderes Feld im CRM verfügen, aus dem der Dealwert synchronisiert werden soll:

  - Aktualisieren Sie **den Feldnamen deal** value (Dealwert) in der Dynamics 365-Umgebungsvariablen mit dem CRM-Feldnamen. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.
  - Bearbeiten Sie [Anpassen] Erstellen oder Erhalten von Details aus dem **Dynamics 365-Flow,** und wechseln Sie zu Create **or update opportunity** in CRM (Verkaufschance in CRM erstellen oder aktualisieren), und aktualisieren Sie Create a new **opportunity** and Update existing **opportunity** actions (Neue Verkaufschance erstellen und vorhandene Verkaufschanceaktionen aktualisieren), um den **DealValue-Wert** dem richtigen Feld im CRM zu zuweisen. Entfernen Sie außerdem die **DealValue-Zuweisung** aus dem Feld **Geschätzter** Umsatz.

- **Ländercode** des Kundenkontos: Beim Erstellen einer neuen Empfehlung ist es obligatorisch, einen zweistelligen Ländercode (ISO 3166) anzugeben. Standardmäßig wird der Ländercode mit dem feld **address1_country** des Kontos im CRM synchronisiert. Wenn im CRM ein anderes Feld für den Ländercode enthalten ist, aus dem die Synchronisierung erfolgt:

   - Für ein feld nicht absteigendes Ländercodefeld in dem Konto, das einen aus zwei Buchstaben besteht:
     - Aktualisieren Sie den Feldnamen des **Kundenkonto-Ländercodes** in der Dynamics 365-Umgebungsvariablen mit dem Feldnamen des CRM. Stellen Sie sicher, dass Sie den Namen des Felds und nicht den Anzeigenamen angeben.
     - Bearbeiten **Sie [Anpassen] Erstellen oder Abrufen von Details aus dem Dynamics 365-Flow,** und wechseln Sie in der CRM-Aktion zu **Kundenkonto erstellen oder abrufen,** um dem richtigen Feld im CRM einen **Länderwert** zuzuweisen. Entfernen Sie außerdem den **Wert country** aus dem Feld **Adresse 1: Land/Region.**

   - Für ein nachschlagende Ländercodefeld im Konto:
     - Fügen Sie dem Konto ein neues benutzerdefiniertes Feld hinzu, und füllen Sie es automatisch mit einem zweistelligen Ländercode (ISO 3166) auf, der auf dem wert basiert, der im suchbasierten Feld ausgewählt wurde (und umgekehrt).
     - Führen Sie die vorherigen Schritte für das Feld "Nonlookup country code" aus, um ein neues benutzerdefiniertes Feld aus dem CRM mit und aus Partner Center zu synchronisieren.

- **Verkaufschancenfelder:** Wenn pflichtbezogene Felder in **Opportunity** vorhanden sind, die aufgefüllt werden müssen, bearbeiten Sie **[Anpassen] Erstellen oder Abrufen von Details aus dem Dynamics 365-Flow,** und wechseln Sie im CRM zu **Verkaufschance erstellen oder aktualisieren,** und aktualisieren Sie die **Aktion Neue Verkaufschance** erstellen, um den Pflichtfeldern Werte basierend auf Ihren Geschäftsanforderungen zuzuweisen.
- **Leadfelder:** Wenn im **Lead** Pflichtfelder vorhanden sind, die aufgefüllt werden müssen, bearbeiten Sie **[Anpassen] Erstellen oder Abrufen von Details aus dynamics 365 flow,** und wechseln Sie im CRM zu **Lead erstellen oder aktualisieren** und aktualisieren Sie die Aktion Neuen **Lead** erstellen, um den Pflichtfeldern Werte basierend auf Ihren Geschäftsanforderungen zuzuweisen.
- **Kundenkonto:** Wenn eine neue Empfehlung von Partner Center mit dem CRM synchronisiert wird, versucht die Power Automate-Lösung, mithilfe des Firmennamens und der Postleitzahl des Kunden nach einem vorhandenen Konto im CRM zu suchen. Wenn kein Kundenkonto findet wird, wird im CRM ein neues Kundenkonto erstellt. Um die Suchkriterien und Details zur Erstellung neuer Konten zu aktualisieren, bearbeiten Sie [Anpassen] Erstellen oder Details aus **Dynamics 365-Flow,** und wechseln Sie in der CRM-Aktion und der Aktion Kundenkonto erstellen zu Erstellen oder Erhalten eines Kundenkontos. 

## <a name="update-environment-variable"></a>Aktualisieren der Umgebungsvariablen

So aktualisieren Sie einen Umgebungsvariablenwert:

1. Wechseln Sie zur Seite **Lösungen,** und wählen Sie **Standardlösung aus.** Wählen Sie **Umgebungsvariable** aus, indem Sie **Alle auswählen.**

1. Wählen Sie die Umgebungsvariable für den  Wert aus, der aktualisiert werden soll, und wählen Sie bearbeiten aus, indem Sie das Symbol mit den Auslassungszeichen verwenden.

1. Aktualisieren **Sie den aktuellen** Wert (aktualisieren Sie den Standardwert **nicht),** indem Sie die Option Neuer **Wert** verwenden und den Wert bereitstellen. Der Wert muss mit dem Datentyp der Variablen übereinstimmen. Beispielsweise akzeptiert der Datentyp Ja oder Nein entweder den Wert Ja oder Nein.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Screenshot: Aktualisieren von Umgebungsvariablen":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Bidirektionale End-to-End-Co-Sell-Empfehlungssynchronisierung

Nachdem Sie die Power Automate-Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Sell-Empfehlungen zwischen Dynamics 365 und Partner Center.

### <a name="prerequisites"></a>Voraussetzungen

Um die Empfehlungen über Partner Center dynamics 365 CRM hinweg zu synchronisieren, wird die Power Automate-Lösung microsoftspezifische Empfehlungsfelder eindeutig abgrenzen. Diese Identifikation gibt Ihren Verkäuferteams die Möglichkeit, zu entscheiden, welche Empfehlungen sie für den Co-Selling an Microsoft freigeben möchten.

Ein Satz benutzerdefinierter Felder und Objekte wird als Teil der Projektmappeninstallation hinzugefügt. Ein CRM-Administratorbenutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten **Opportunity-Feldern** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center:** Gibt an, ob die Verkaufschance mit Partner Center synchronisiert werden soll. Standardmäßig ist der Wert dieses Felds Nein und muss explizit von Ihrem Verkäufer auf Ja festgelegt werden, um eine Verkaufschance für Microsoft freizugeben. Für neue Empfehlungen, die von Partner Center an CRM freigegeben werden, wird dieser Feldwert auf Ja festgelegt.
- **Empfehlungsbezeichner:** Ein schreibgeschütztes Bezeichnerfeld für die Partner Center Empfehlung.
- **Empfehlungslink:** Ein schreibgeschützter Link zur Empfehlung in Partner Center.
- **Wie kann Microsoft helfen?**: Hilfe, die von Microsoft für die Empfehlung benötigt wird. Um eine Co-Selling-Empfehlung zu erstellen, wählen Sie die entsprechende Hilfe aus, die von Microsoft benötigt wird. Ein Kundenkontakt muss der Möglichkeit zugeordnet werden, eine Co-Selling-Empfehlung zu erstellen. Um eine Nicht-Co-Selling-Empfehlung zu erstellen, wählen Sie dieses Feld nicht aus. Eine Nicht-Co-Selling-Empfehlung kann jederzeit in eine Co-Selling-Empfehlung konvertiert werden, indem die entsprechende Option für die erforderliche Hilfe ausgewählt wird.
- **Microsoft Partner Center-Empfehlungssichtbarkeit:** Wählen Sie Sichtbarkeit für die Partner Center Empfehlung aus. Wenn sie für Microsoft-Verkäufer sichtbar gemacht wird, kann eine Nicht-Co-Selling-Empfehlung in Co-Selling umgewandelt werden. Wenn Microsoft-Hilfe erforderlich ist, ist die Empfehlung standardmäßig für Microsoft-Verkäufer sichtbar. Nachdem dieses Feld als sichtbar markiert wurde, kann es nicht mehr zurückgesetzt werden.
- **Microsoft CRM-Bezeichner:** Wenn eine Co-Selling-Empfehlung von Microsoft erstellt und akzeptiert wird, wird dieses Feld mit dem CRM-Bezeichner von Microsoft aufgefüllt.
- **Produkte: Veraltet:** Verwenden Sie dieses Feld nicht, oder fügen Sie es dem CRM-Abschnitt hinzu. Sie ist nur aus Gründen der Abwärtskompatibilität verfügbar. Verwenden Sie stattdessen Partner Center Lösungen.
- **Audit**: Ein schreibgeschützter Überwachungspfad für die Synchronisierung mit Partner Center Empfehlungen.
- **Microsoft Partner Center Solutions:** Ein benutzerdefiniertes Objekt, mit dem Co-Selling-Lösungen oder Microsoft-Lösungen der Gelegenheit zugeordnet werden können. Eine oder mehrere Lösungen können hinzugefügt oder aus der Verkaufschance entfernt werden. Es ist obligatorisch, der Verkaufschance mindestens eine Co-Sell Ready- oder Microsoft-Lösung hinzuzufügen, bevor Sie sie mit Microsoft teilen. Um dieses Objekt der Verkaufschance zu zuordnen, aktualisieren Sie das **Formular Verkaufschance** im CRM.

  Wählen Sie im Formular Verkaufschance die entsprechende **Registerkarte** aus, und fügen Sie wie hier gezeigt ein Unterraster hinzu.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Screenshot: Formular &quot;Verkaufschance&quot;":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Screenshot: Microsoft-Lösungen":::

- Nachdem Sie Microsoft-Lösungen hinzugefügt haben, können Sie Vorabdetails für Co-Sell-Lösungen aufbereiten, damit Ihre Verkäufer sie nicht hinzufügen müssen. Um ein neues Lösungsdetail hinzuzufügen, wechseln Sie zum  Objekt Microsoft Solution Details (Microsoft Solution Details) im CRM, und wählen Sie Datensatz hinzufügen aus, um einen Eintrag hinzuzufügen, oder verwenden Sie **den Excel-Upload,** um mehrere Einträge hinzuzufügen.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Screenshot: Neue Microsoft-Lösungsdetails":::

### <a name="scenarios"></a>Szenarien

1. Empfehlungssynchronisierung beim Erstellen oder Aktualisieren der Empfehlung im CRM und synchronisieren in Partner Center:

   1. Melden Sie sich bei Ihrer Dynamics 365 CRM-Umgebung mit dem Benutzer an, der im Abschnitt Verkaufschance **des** CRM Sichtbarkeit hat.

   1. Stellen Sie **sicher, dass Microsoft Partner Center** vorhanden ist, wenn Sie eine neue Verkaufschance in der Dynamics 365-Umgebung erstellen.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Screenshot: Neue Verkaufschance":::

   1. Um diese Verkaufschance mit Partner Center synchronisieren, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

      - **Wie kann Microsoft helfen?**: Wählen Sie eine geeignete Hilfeoption aus, um eine Co-Sell-Empfehlung zu erstellen.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Screenshot: Anzeigen der entsprechenden Felder in der Kartenansicht":::

      - **Kundenkontakt:** Fügen Sie der Verkaufschance einen Kundenkontakt hinzu, um eine Co-Sell-Empfehlung zu erstellen.
      - **Sync With Partner Center:** Ja.
      - **Microsoft Solutions:** Um eine Empfehlung mit Microsoft zu teilen, fügen Sie der Verkaufschance eine gültige Co-Sell Ready- oder Microsoft-Lösung hinzu.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Screenshot: Projektmappen-ID":::

   1. Nachdem die Verkaufschance in Dynamics 365 erstellt wurde und die Option **Mit Partner Center synchronisieren** auf Ja festgelegt ist, warten Sie 10 Minuten. Melden Sie sich dann bei Ihrem Partner Center-Konto an. Ihre Empfehlungen werden mit Dynamics 365 und **dem Empfehlungsbezeichner** synchronisiert. **Der Empfehlungslink** wird aufgefüllt. Wenn ein Fehler auftritt, wird das Feld **Überwachung** mit Fehlerinformationen aufgefüllt.
     
    1. Ebenso werden bei einer Verkaufschance, bei der die Option **Mit Partner Center synchronisieren** auf Ja festgelegt war, die Änderungen in Ihrem Partner Center-Konto synchronisiert, wenn Sie die Verkaufschance in Dynamics 365 CRM aktualisieren.

    1. Verkaufschancen, die erfolgreich mit Partner Center synchronisiert werden, werden mit ✔icon in Dynamics 365 identifiziert.

1. Empfehlungssynchronisierung, wenn die Empfehlung in Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird:

   1. Melden Sie sich bei Ihrem [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/home)an.

   1. Wählen Sie im linken Menü **Empfehlungen** aus.

   1. Erstellen Sie eine neue Co-Selling-Empfehlung aus Partner Center, indem Sie die Option **Neuer Deal** auswählen.

   1. Melden Sie sich bei Ihrer Dynamics 365 CRM-Umgebung an.

   1. Wechseln Sie zu **Open Opportunities (Verkaufschancen öffnen).** Die in Partner Center erstellte Empfehlung wird jetzt in Dynamics 365 CRM synchronisiert.

   1. Wenn Sie eine synchronisierte Empfehlung auswählen, werden die Kartenansichtsdetails aufgefüllt.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)
- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
- [Weitere Informationen zur Microsoft Power Automate-Plattform](/power-automate/)
- [Partner Center-Webhooks](/partner-center/develop/partner-center-webhooks)
