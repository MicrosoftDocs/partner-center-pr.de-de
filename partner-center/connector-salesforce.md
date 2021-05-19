---
title: Der Co-Sell-Connector für Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Sie Ihre Empfehlungen in Partner Center Salesforce CRM. Verkäufer können dann in Ihren CRM-Systemen gemeinsam mit Microsoft verkaufen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148413"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Co-Selling-Connector für Salesforce CRM – Übersicht

**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Systemadministrator oder Systemanpasser im CRM

Partner Center Co-Sell-Connector ermöglicht Es Ihren Verkäufern, in Ihren CRM-Systemen gemeinsam mit Microsoft zu verkaufen. Sie müssen nicht trainiert werden, um co-Partner Center verwalten zu können. Mithilfe der Co-Sell-Connectors können Sie eine neue Co-Sell-Empfehlung erstellen, um einen Microsoft-Verkäufer zu kontaktieren, Empfehlungen vom Microsoft-Verkäufer zu erhalten, Empfehlungen zu akzeptieren/ablehnen, Dealdaten wie den Dealwert und das Abschlussdatum zu ändern.  Sie können auch updates von den Microsoft-Verkäufern zu diesen Co-Sell-Deals erhalten. Sie können alle Ihre Empfehlungen nutzen, während Sie innerhalb des CRM Ihrer Wahl arbeiten und nicht in Partner Center. 

Die Lösung basiert auf Microsoft Power Automate Solution und verwendet Partner Center APIs.

## <a name="before-you-install---pre-requisites"></a>Voraussetzungen vor der Installation

|**Themen**   |**Details**   |**Links**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Sie benötigen eine gültige MPN-ID.|So treten Sie [MPN bei](https://partner.microsoft.com/)|
|Co-Sell Ready|Ihre IP/Services-Lösung muss co-sell ready sein.|[Verkaufen mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partner Center-Konto|Die MPN-ID, die dem Partner Center Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die Ihrer Co-Sell-Lösung zugeordnet ist. Stellen Sie sicher, dass Ihre Co-Sell-Empfehlungen im Partner Center angezeigt werden, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
|Partner Center-Benutzerrollen|Der Mitarbeiter, der die Connectors installiert und verwendet, muss ein Empfehlungsadministrator sein.|[Zuweisen von Rollen und Berechtigungen zu Benutzern](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Die CRM-Benutzerrolle ist "Systemadministrator" oder "Systemanpasser".|[Zuweisen von Rollen in Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow-Konto|Ein aktives [Power Automate](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder systemanpasser. Dieser Benutzer sollte sich mindestens einmal vor der Installation bei [Power Automate](https://flow.microsoft.com) anmelden.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installation des Salesforce-Pakets für benutzerdefinierte Microsoft-Felder 

Um die Empfehlungen über Partner Center und Salesforce CRM hinweg zu synchronisieren, muss die Power Automate Lösung microsoftspezifische Empfehlungsfelder eindeutig identifizieren. Diese Demarzierung bietet Partnerverkäuferteams die Möglichkeit zu entscheiden, welche Empfehlungen sie für den Co-Selling mit Microsoft teilen möchten.

1. Aktivieren Sie in Salesforce **Notizen,** und fügen Sie sie der Liste mit den Verkaufschancen hinzu. 
[Verweis](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aktivieren Sie **Opportunity-Teams,** indem Sie die folgenden Schritte ausführen: 
    - Verwenden Sie im Setup das Feld **Schnellsuche,** um nach Opportunity Team Settings zu suchen.
    - Definieren Sie die Einstellungen nach Bedarf.
[Verweis](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Installieren Sie in Salesforce benutzerdefinierte Felder und Objekte mithilfe des [Paketinstallationsprogramms](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Verwenden Sie diese, um das Paket in einem beliebigen Unternehmen zu installieren.

>[!NOTE]
>Wenn Sie in einer Sandbox installieren, müssen Sie den ursprünglichen Teil der URL durch ersetzen. http://test.salesforce.com

4. Fügen Sie in Salesforce Microsoft-Lösungen zur Liste **Verkaufschancen** hinzu. Wählen Sie nach dem Hinzufügen das **Schraubenschlüsselsymbol** aus, und aktualisieren Sie die Eigenschaften.

## <a name="best-practice-test-before-you-go-live"></a>Bewährte Methode: Testen, bevor Sie live gehen

Bevor Sie die Power Automate Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen, müssen Sie die Lösung auf einer STAGING-CRM-Instanz testen.

- Installieren Sie Microsoft Power Automate Lösung in einer Stagingumgebung/CRM-Instanz.

- Erstellen Sie eine Kopie der Projektmappe, und führen Sie Ihre Konfiguration aus, und Power Automate Flowanpassungen in der Stagingumgebung.

- Testen Sie die Lösung in einer Staging-/CRM-Instanz.

- Importieren Sie bei Erfolg als verwaltete Lösung in die Produktionsinstanz.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installieren Partner Center Synchronisierung von Empfehlungen für Salesforce CRM

1. Wechseln Sie [zu Power Automate,](https://flow.microsoft.com) und wählen **Sie in der** rechten oberen Ecke Umgebungen aus. Dadurch werden die verfügbaren CRM-Instanzen gezeigt.

2. Wählen Sie in der Dropdownliste rechts oben die entsprechende CRM-Instanz aus.

3. Wählen **Sie in** der linken Navigationsleiste Lösungen aus.

4. Wählen Sie im oberen Menü den Link **AppSource** öffnen aus.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öffnen von AppSource":::

5. Suchen Sie **Partner Center Popupbildschirm nach** Connectors für Empfehlungen für Salesforce.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Wählen Sie die **Schaltfläche Jetzt holen** und dann Weiter **aus.**

7. Dadurch wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung auswählen können, um die Anwendung zu installieren.  Stimmen Sie den Geschäftsbedingungen zu.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Verfügbare CRMS":::

8. Sie werden dann zur Seite Manage **your solutions (Lösungen verwalten)** geleitet.  Navigieren Sie zu "Partner Center Empfehlungen", indem Sie die Pfeilschaltflächen unten auf der Seite verwenden. **Die geplante Installation** sollte neben Partner Center Empfehlungslösung angezeigt werden. Die Installation dauert 10 bis 15 Minuten.

9. Navigieren Sie nach Abschluss der Installation zurück zum Power Automate [und](https://flow.microsoft.com) wählen Sie **im linken** Navigationsbereich Lösungen aus. Beachten Sie, dass **Partner Center Empfehlungssynchronisierung für Salesforce** in der Liste Lösungen verfügbar ist.

10. Wählen Sie **Partner Center Synchronisierung von Empfehlungen für Salesforce** aus. Die folgenden Power Automate Flows und Entitäten sind verfügbar:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-Flows":::



## <a name="configure-the-solution"></a>Konfigurieren der Projektmappe

1. Nachdem Sie die Lösung in Ihrer CRM-Instanz installiert haben, navigieren Sie zurück zu [Power Automate](https://flow.microsoft.com/).

2. Wählen Sie in der Dropdown-Dropdownseite **Umgebungen** in der rechten oberen Ecke die CRM-Instanz aus, auf der Sie die Power Automate-Lösung installiert haben.
3. Sie müssen Verbindungen erstellen, die die drei Benutzerkonten zuordnen:
    - Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen
    - Partner Center-Ereignisse
    - CRM-Administrator mit den Power Automate Flows in der Lösung.
4. Klicken Sie auf der linken Navigationsleiste auf **Verbindungen,** und wählen Sie in der Liste die Lösung "Partner Center Empfehlungen" aus.

5. Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen** klicken.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Erstellen der Verbindung":::

- Suchen Sie in der Suchleiste in der oberen rechten Ecke nach Partner Center Empfehlungen (Vorschau).

- Erstellen Sie eine Verbindung für Ihren Partner Center Benutzer mit der Rolle "Anmeldeinformationen" des Empfehlungsadministrators.

-  Erstellen Sie als Nächstes eine Partner Center Events-Verbindung für Ihren Partner Center-Benutzer mit den Anmeldeinformationen des Empfehlungsadministrators.

- Erstellen Sie eine Verbindung für Salesforce für den CRM-Administratorbenutzer.

-  Nachdem Sie alle Verbindungen hinzugefügt haben, sollten in Ihrer Umgebung die folgenden Verbindungen angezeigt werden:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Beobachten von Verbindungen":::

### <a name="edit-the-connections"></a>Bearbeiten der Verbindungen

1. Kehren Sie zur Seite Projektmappen zurück, und wählen Sie **Standardlösung** aus.  Wählen Sie **Verbindungsverweis (Vorschau)** aus, indem Sie auf **Alle** klicken.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Connectorbearbeitung starten":::

2. Bearbeiten Sie die einzelnen Verbindungen einzeln, indem Sie auf das Symbol mit drei Punkten klicken. Fügen Sie die relevanten Verbindungen hinzu.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Bearbeiten von Connectors":::

3. Aktivieren Sie die Flows in der folgenden Reihenfolge:

- Partner Center Webhookregistrierung (Insider Preview)
- Erstellen einer Co-Sell-Empfehlung – Salesforce Partner Center (Insider Preview)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center to Salesforce (Insider Preview)
- Salesforce to Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von Webhook-APIs zum Registrieren für Ressourcenänderungsereignisse

Mit Partner Center Webhook-APIs können Sie sich für Ressourcenänderungsereignisse registrieren. Diese Änderungsereignisse werden als HTTP-Beiträge an Ihre URL gesendet.

1. Wählen Sie zum Registrieren Ihrer URL Partner Center **Webhookregistrierung (Insider Preview) Power Automate** aus.

2. Fügen Sie Verbindungen für (a.) Partner Center Benutzer mit Administratoranmeldeinformationen für Empfehlungen (b.) Partner Center Ereignisse hinzu, wie unten hervorgehoben.

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Wenn Sie diese Updates machen, sehen Sie:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Speichern Sie Ihre Änderungen, und wählen **Sie Aktivieren aus.**

   Um webhooks Partner Center ereignisänderungen zu lauschen, führen Sie die folgenden Schritte aus:

5. Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.

6. Wählen Sie das Symbol **Bearbeiten** und **dann When a HTTP request is received (Wenn eine HTTP-Anforderung empfangen wird)** aus.

7. Wählen Sie das Symbol **Kopieren** aus, um die angegebene HTTP POST-URL zu kopieren.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieren der URL":::

8. Wählen Sie nun den Flow "Partner Center Webhookregistrierung (Insider Preview)" Power Automate aus, und wählen Sie **Ausführen** aus.

9. Stellen Sie sicher, dass das Fenster "Flow ausführen" im rechten Bereich geöffnet wird, und wählen Sie **Weiter** aus.

10. Geben Sie die folgenden Details ein:

    1. **HTTP-Triggerendpunkt:** URL aus dem vorherigen Schritt kopiert

    2. **Zu registrierende Ereignisse:**"Empfehlung erstellt" und "Empfehlung aktualisiert"

    3. **Vorhandene Triggerendpunkte überschreiben, falls vorhanden:** Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)

11. Wählen Sie **Ausführen** und dann **Fertig aus.**

Der Webhook kann jetzt auf Erstellungs- und Aktualisierungsereignisse lauschen.

## <a name="customize-synchronization-steps"></a>Anpassen der Synchronisierungsschritte

Wenn Co-Selling-Empfehlungen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf Partner Center PC synchronisiert werden, hier aufgeführt.

CRM-Systeme sind häufig stark angepasst. Sie können die Power Automate Flows anpassen. Befolgen Sie die Anleitung für die Feldzuordnung, und nehmen Sie bei Bedarf entsprechende Änderungen in den Schritten der Power Automate Flows vor.  Microsoft Partner Center-to-CRM-Zuordnungen werden bereitgestellt, aber basierend auf Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.

Mehrere Schritte der einzelnen Power Automate Flows können je nach Ihren Anforderungen angepasst werden. Im Folgenden finden Sie Beispiele für verfügbare Anpassungen:

1. So passen Sie die Felder für die Erstellungs- oder Aktualisierungsereignisse im Partner Center zur CRM-Empfehlungssynchronisierung an:

   1. Wählen Sie Partner Center salesforce CRM (Insider Preview) aus.

   2. Wählen **Sie Bearbeiten** aus, um den Power Automate anzupassen.

   3. Wählen **Sie (Bereich) Lead oder Verkaufschance synchronisieren aus.**

2. Um CRM-Feldzuordnungen für Erstellungsereignisse anzupassen, wählen Sie If it es new Shared opportunity (Wenn es sich um eine neue freigegebene **Verkaufschance) und dann aus.** Wählen Sie den unteren Schritt **aus, falls ja,** und erweitern Sie dann **Erstellen einer neuen Verkaufschance in CRM**. Sie können die Zuordnungen in diesem Abschnitt mithilfe des Feldzuordnungshandbuchs bearbeiten.

   1. Um CRM-Feldzuordnungen für Updateereignisse anzupassen, wählen Sie den Schritt "(Bereich) Lead oder Verkaufschance synchronisieren" aus.

   2. Wählen Sie If it es a update to an opportunity (Wenn es sich um **ein Update einer Verkaufschance) und dann um .** Wählen Sie den unteren Schritt **aus,** falls ja, und erweitern Sie **if difference between the opportunity objects in Partner Center and CRM (Wenn** Unterschied zwischen den Opportunityobjekten in Partner Center CRM) und dann .  

   3. Wählen Sie **Bei Ja** gefolgt von Update existing **opportunity (Vorhandene Verkaufschance aktualisieren) aus.**

3. So passen Sie die Felder für die CRM-zu-PC-Empfehlungssynchronisierung für Updateereignisse an:

   1. Wählen **Sie Bearbeiten**  aus, um den Power Automate anzupassen.

   2. Wählen **Sie (Bereich) Die Verkaufschance synchronisieren aus.**

   3. Wählen Sie zum Anpassen von CRM-Feldzuordnungen (basierend auf dem Leitfaden für Feldzuordnungen) für Updateereignisse die Option Wenn ein Unterschied zwischen den Leadobjekten **in Partner Center und CRM besteht, dann aus.**

   4. Wählen Sie den unteren Schritt **aus, falls ja,** und erweitern Sie dann den Schritt **Empfehlung mit Verkaufschancedaten aktualisieren.**

   Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Feldzuordnungshandbuch bearbeiten.

4. Zum Anpassen der Felder für die CRM-zu-PC-Empfehlungssynchronisierung zum Erstellen von Ereignissen?

   1. Wählen **Sie Bearbeiten**  aus, um den Power Automate anzupassen.

   2. Wählen **Sie (Bereich) Empfehlungen synchronisieren aus.**

   3. Wählen Sie zum Anpassen von CRM-Feldzuordnungen (basierend auf dem Feldzuordnungsleitfaden) für Erstellungsereignisse die Option **Microsoft-Empfehlung erstellen aus.**

Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Feldzuordnungshandbuch bearbeiten.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Bidirektionale End-to-End-Co-Selling-Empfehlungssynchronisierung

Nachdem Sie die Power Automate Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Empfehlungen zwischen Salesforce CRM und Partner Center testen.

### <a name="pre-requisites"></a>Voraussetzungen

Um die Empfehlungen über Partner Center und Salesforce CRM hinweg zu synchronisieren, muss die Power Automate Lösung eindeutig Microsoft-spezifische Empfehlungsfelder abgrenzen. Diese Identifizierung bietet Ihren Verkäuferteams die Möglichkeit, zu entscheiden, welche Empfehlungen sie für den Co-Selling mit Microsoft teilen möchten.

Eine Reihe von benutzerdefinierten Feldern ist als Teil Partner Center Entität Empfehlungssynchronisierung für Salesforce CRM-Lösung **Opportunity** verfügbar. Ein CRM-Administratorbenutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern **Opportunity** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center:** Gibt an, ob die Verkaufschance mit Microsoft Partner Center synchronisiert werden soll.

- **Empfehlungsbezeichner:** Ein schreibgeschütztes Bezeichnerfeld für Microsoft Partner Center-Empfehlung

- **Empfehlungslink:** Ein schreibgeschützter Link zur Empfehlung in Microsoft Partner Center

- How can Microsoft help : Help required from Microsoft for the referral **(Wie kann Microsoft helfen?**: Hilfe von Microsoft für die Empfehlung erforderlich)

- **Produkte:** Liste der Produkte, die dieser Verkaufschance zugeordnet sind

- **Überwachung:** Ein schreibgeschützter Überwachungspfad für die Synchronisierung mit Partner Center Empfehlungen

### <a name="scenarios"></a>Szenarien:

1. Empfehlungssynchronisierung, wenn die Empfehlung in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:

   1. Melden Sie sich mit einem Benutzer bei Ihrer Salesforce CRM-Umgebung an, der im Abschnitt **Opportunity** des CRM-Abschnitts über Sichtbarkeit verfügt.

   2. Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "Neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-Umgebung":::

   3. Um diese Verkaufschance mit Microsoft Partner Center zu synchronisieren, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

       - "Sync with Partner Center": Yes
       - "Wie kann Microsoft helfen?": Wählen Sie eine der folgenden Optionen aus:
       - Produkte: Lösungs-IDs des Produkts

   4. Nachdem Sie die Option  **Sync with Partner Center** auf **Ja** festgelegt haben, warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center an. Ihre Empfehlungen werden mit Salesforce CRM synchronisiert.

   5. Wenn die Option "Mit Partner Center synchronisieren" auf "Ja" festgelegt ist und Sie die Verkaufschance in Salesforce CRM aktualisieren, werden die Änderungen mit Ihrem Partner Center synchronisiert.

   6. Verkaufschancen, die erfolgreich mit Partner Center synchronisiert werden, werden mithilfe ✔ in Salesforce CRM identifiziert.

2. Empfehlungssynchronisierung, wenn die Empfehlung in Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:

    1. Melden Sie sich bei Ihrem [Partner Center dashboard an.](https://partner.microsoft.com/dashboard/home)

    2. Wählen **Sie im menü** auf der linken Seite die Option Empfehlungen aus.

    3. Erstellen Sie eine neue Co-Sell-Empfehlung aus Partner Center, indem Sie auf die Option "Neuer Deal" klicken.

    4. Melden Sie sich bei Ihrer Salesforce CRM-Umgebung an.

    5. Navigieren Sie zu **Open Opportunities (Verkaufschancen öffnen).** Die im Microsoft Partner Center erstellte Empfehlung wird jetzt in Salesforce CRM synchronisiert.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Bildschirm &quot;Salesforce-Verkaufschance&quot;":::

    6. Wenn Sie eine synchronisierte Empfehlung auswählen, werden die Details der Kartenansicht aufgefüllt.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)

- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)

- [Partner Center-Webhooks](/partner-center/develop/partner-center-webhooks)
