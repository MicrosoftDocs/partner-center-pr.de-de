---
title: Der Co-Selling-Connector für das Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisieren Ihrer Verweise in Partner Center mit Ihrem Salesforce CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 0a22587f5b555281cae6f557acfc2695ba92727e
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302377"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Co-Selling-Connector für Salesforce CRM – Übersicht

### <a name="appropriate-roles"></a>Geeignete Rollen

- Empfehlungsadministrator
- Systemadministrator oder systemanpassungsprogramm im CRM

Der Partner Center-Co-Selling-Connector ermöglicht ihren Verkäufern das Co-Selling mit Microsoft innerhalb Ihrer CRM-Systeme. Sie müssen nicht für die Verwendung von Partner Center zur Verwaltung von Co-Selling-Geschäften geschult werden. Mithilfe der Co-Selling-Connectors können Sie einen neuen Co-Selling-Verweis zum Einbinden eines Microsoft-Verkäufers erstellen, Referenzen vom Microsoft-Verkäufer erhalten, Verweise akzeptieren/ablehnen, Geschäftsdaten ändern, wie z. b. den Geschäftswert und das Enddatum.  Sie können für diese Co-Selling-Angebote auch Updates von den Microsoft-Verkäufern erhalten. Sie können alle Ihre Verweise ausführen, während Sie im CRM Ihrer Wahl arbeiten und nicht im Partner Center. 

Die Lösung basiert auf der Microsoft Power automatisieren-Lösung und verwendet Partner Center-APIs.

## <a name="before-you-install---pre-requisites"></a>Vor der Installation von-Pre-Requirements

|**Sonder**   |**Details**   |**Links**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Sie benötigen eine gültige MPN-ID.|So fügen Sie [MPN](https://partner.microsoft.com/) an|
|Co-Selling bereit|Ihre IP-/Dienst-Lösung muss für den Co-Selling bereit sein.|[Vertrieb mit Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partner Center-Konto|Die MPN-ID, die dem Partner Center-Mandanten zugeordnet ist, muss mit der MPN-ID identisch sein, die ihrer Co-Selling-Lösung zugeordnet ist. Vergewissern Sie sich, dass Sie Ihre Co-Selling-Verweise im Partner Center-Portal sehen können, bevor Sie die Connectors bereitstellen.|[Verwalten Ihres Kontos](create-user-accounts-and-set-permissions.md)|
|Partner Center-Benutzerrollen|Der Mitarbeiter, der die Connectors installieren und verwenden soll, muss ein Administrator sein.|[Zuweisen von Rollen und Berechtigungen zu Benutzern](create-user-accounts-and-set-permissions.md)|
|Salesforce-CRM|Die CRM-Benutzerrolle ist Systemadministrator oder SystemCustomizer.|[Zuweisen von Rollen in Salesforce CRM](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Energie automatisierter Fluss Konto|Ein aktives, [Energie automatisierbares](https://flow.microsoft.com) Konto für den CRM-Systemadministrator oder den SystemCustomizer. Dieser Benutzer sollte sich mindestens einmal vor der Installation bei der [Strom Automatisierung](https://flow.microsoft.com) anmelden.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installieren der Partner Center-Synchronisierung für Salesforce CRM

1. Wechseln Sie zu " [Energie Automatisierung](https://flow.microsoft.com) ", und wählen Sie in der rechten oberen Ecke **Umgebungen** aus. Dadurch werden die verfügbaren CRM-Instanzen angezeigt.

2. Wählen Sie in der Dropdown-Dropdown-Ecke in der rechten oberen Ecke die entsprechende CRM-Instanz aus.

3. Wählen Sie in der linken Navigationsleiste **Lösungen** aus.

4. Klicken Sie im oberen Menü auf den Link **appsource öffnen** .

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Appsource öffnen":::

5. Suchen Sie im Popup-Bildschirm nach **Partner Center-verweisverweisconnectors für Salesforce** .  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Klicken Sie auf die Schaltfläche **jetzt starten** und dann auf **weiter**.

7. Daraufhin wird die Seite geöffnet, auf der Sie die Salesforce CRM-Umgebung zum Installieren der Anwendung auswählen können.  Stimmen Sie den Geschäftsbedingungen zu.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Verfügbare CRMs":::

8. Anschließend werden Sie zur Seite **Verwalten Ihrer Lösungen** weitergeleitet.  Navigieren Sie zu "Partner Center-Verweise", indem Sie die Pfeil Schaltflächen unten auf der Seite verwenden. Die **geplante Installation** sollte neben der Projekt Mappe für Partner Center-Verweise angezeigt werden. Die Installation wird 10-15 Minuten dauern.

9. Nachdem die Installation fertiggestellt ist, navigieren Sie zurück zu [Energie Automatisierung](https://flow.microsoft.com) , und wählen Sie im linken Navigationsbereich **Lösungen** aus. Beachten Sie, dass die **Synchronisierung der Partner Center-Verweise für Salesforce** in der Lösungs Liste verfügbar ist.

10. Wählen Sie die **Synchronisierung der Partner Center-Verweise für Salesforce aus**. Die folgenden Strom automatisierten Flows und Entitäten sind verfügbar:

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce-Flows":::

## <a name="best-practice-test-before-you-go-live"></a>Bewährte Vorgehensweise: testen, bevor Sie fortfahren

Stellen Sie sicher, dass Sie die Lösung in einer-Staging-Instanz von CRM testen, bevor Sie die Energie automatisierte Lösung in der Produktionsumgebung installieren, konfigurieren und anpassen.

- Installieren Sie die Microsoft powerautomatisieren-Lösung auf einer Staging-Umgebung/CRM-Instanz.

- Erstellen Sie eine Kopie der Projekt Mappe, und führen Sie die Konfiguration aus, und führen Sie die Automatisierung der Fluss Anpassungen in der Stagingumgebung durch

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

   2. Erstellen Sie eine Verbindung, indem Sie auf **Verbindung erstellen**klicken.

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Erstellen der Verbindung":::

   3. Suchen Sie in der Suchleiste in der oberen rechten Ecke nach **Partner Center-Referenzen (Vorschau)** .

   4. Erstellen Sie eine Verbindung für Ihren Partner Center-Benutzer mit der Rolle "Anmelde Informationen" des Administrators "Administrator".

   5. Erstellen Sie als nächstes eine Partner Center-Ereignis Verbindung für Ihren Partner Center-Benutzer mit den Anmelde Informationen für den Administrator.

   6. Erstellen Sie eine Verbindung für Common Data Service (aktuelle Umgebung) für den CRM-Administrator Benutzer.

4. Um die Strom automatisierten Flows den Verbindungen zuzuordnen, bearbeiten Sie jeden der Strom automatisierten Flows, um eine Verbindung mit Common Data Service-und Partner Center-Referenzen herzustellen. Speichern Sie die Änderungen.

5. **Schalten** Sie die Strom automatisierten Flows ein.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse

Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren. Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.

1. Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.

2. Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Wenn Sie diese Updates vornehmen, wird Folgendes angezeigt:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Speichern Sie die Änderungen, und wählen Sie **einschalten aus**.

   Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen zu aktivieren:

5. Wählen Sie **Partner Center zu Salesforce CRM (Insider Preview)** aus.

6. Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.

7. Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieren der URL":::

8. Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.

9. Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.

10. Geben Sie die folgenden Details ein:

    1. **Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL

    2. **Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"

    3. **Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)

11. Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**

Der webhook kann nun auf Create-und Update-Ereignisse lauschen.

## <a name="customize-synchronization-steps"></a>Synchronisierungs Schritte anpassen

Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.

Häufig sind CRM-Systeme hochgradig angepasst. Sie können die Strom automatisierten Flows anpassen. Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.  Microsoft Partner Centers für CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.

Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden. Im folgenden finden Sie Beispiele für verfügbare Anpassungen:

1. So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an:

   1. Wählen Sie Partner Center zu Salesforce CRM (Insider Preview) aus.

   2. Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.

   3. Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.

2. **Wenn Sie die CRM-** Feld Zuordnungen für Erstellungs Ereignisse anpassen möchten, wählen Sie aus, ob es sich um eine neue Freigabe Chance handelt Wählen Sie den untergeordneten **Schritt** aus, und erweitern Sie dann die Option **Erstellen einer neuen Verkaufschance im CRM**. Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.

   1. Zum Anpassen von CRM-Feld Zuordnungen für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".

   2. Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**. Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.  

   3. Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**

3. So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an

   1. Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.

   2. Select **(Bereich) Synchronisieren der Verkaufschance**.

   3. Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**.

   4. Wählen Sie den unterschritt aus, **Wenn ja** , und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.

   Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.

4. Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse

   1. Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.

   2. Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**

   3. Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**.

Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>Erstellen eines separaten Abschnitts im Salesforce-CRM-Verkaufschancen Layout

Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen. Dies bietet Ihren Verkäufer Teams die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.

Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM-Verkaufs **Chancen** Entität verfügbar. Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.
Der Salesforce CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll

- **Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz

- **Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center

- **Wie kann Microsoft helfen?** Von Microsoft für den Verweis erforderliche Hilfe

- **Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind

- Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit dem Microsoft Partner Center-Verweis

### <a name="set-up-fields-and-relationships"></a>Einrichten von Feldern und Beziehungen

1. Melden **Sie sich bei**Ihrem Salesforce-Konto an.

2. Klicken Sie auf die Optionen **Setup** und **Objekt bearbeiten** , um die erforderlichen Felder hinzuzufügen.

3. **Felder & Beziehungen** im linken Navigationsbereich auswählen

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Felder":::

4. Fügen Sie die folgenden Felder in den **Feldern & Beziehungs** Tabelle hinzu:

   |**Feld Bezeichnung**   |**Feldname**|**Datentyp**|**Zierenden**|
   |---------------------|:-------------------|:--------------|:----------------|
   |Audit| Audit__c|Long-Text Bereich (100000) (sichtbare Zeile 4)||
   |Wie kann Microsoft helfen?|How_can_Microsoft_help_c|Auswahlliste|
   |Produkte|Products_c|Text (255)||
   |Referral | Referral_Identfier_c|Text (100) (externe ID)|ja|
   |Verweis Link| Referral_Link_c_|URL (255)||
   |Mit Partner Center synchronisieren|sync_with_partner_center_c|CheckBox (Standardeinstellung deaktiviert)||

   * Picklist-Werte:

   - Auslastungs spezifischer Wert-Vorschlag
   - Technische Kunden Architektur
   - Proof of Concept oder Demo
   - Anführungszeichen oder Lizenzierung
   - Kunden Erfolg nach dem Verkauf
   - Allgemein oder andere

5. Die Felder werden unter " **Felder & Beziehungen** " erstellt.

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Erstellte Felder":::

6. Erstellen Sie im Layout der Verkaufschancen einen separaten Abschnitt mit den oben aufgeführten Feldern.

   - Dieser Abschnitt sollte für die Verkäufer im Verkaufschancen Layout verfügbar sein.

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Layout der Partner Center-Felder":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-End-bidirektionale Co-Selling-Synchronisierung

Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Salesforce CRM und Partner Center testen.

### <a name="pre-requisites"></a>Voraussetzungen

Um die Verweise auf Partner Center und Salesforce CRM zu synchronisieren, muss die Energie automatisierte Lösung die Microsoft-spezifischen verweigerfelder eindeutig abgrenzen. Diese Identifikation bietet Ihren Verkäufer Teams die Möglichkeit, sich zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.

Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für die Salesforce CRM Solution **Opportunity** -Entität verfügbar. Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll

- **Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz

- **Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center

- **Wie kann Microsoft Help**: Hilfe von Microsoft für den Verweis

- **Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind

- Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen

### <a name="scenarios"></a>SS

1. Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:

   1. Melden Sie sich bei ihrer Salesforce CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.

   2. Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Salesforce CRM-Umgebung erstellen.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-Umgebung":::

   3. Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

       - "Mit Partner Center synchronisieren": Ja
       - "Wie kann Microsoft Help?": Wählen Sie eine der folgenden Optionen aus:
       - Produkte: Lösungs-IDs des Produkts

   4. Nachdem Sie die Option für die Verkaufschancen **Synchronisierung mit Partner Center** auf **Ja**festgelegt haben, können Sie sich bei Ihrem Partner Center-Konto anmelden. Ihre Verweise werden mit Salesforce CRM synchronisiert.

   5. Wenn die Option "Sync with Partner Center" auf "yes" festgelegt ist, werden die Änderungen, wenn Sie die Verkaufschance in Salesforce CRM aktualisieren, mit Ihrem Partner Center-Konto synchronisiert.

   6. Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Salesforce CRM identifiziert.

2. Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Salesforce CRM-Umgebung synchronisiert wird:

    1. Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.

    2. Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.

    3. Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.

    4. Melden Sie sich bei ihrer Salesforce CRM-Umgebung an.

    5. Navigieren Sie zu **Open Verkaufschancen**. Der im Microsoft Partner Center erstellte Verweis ist nun in Salesforce CRM synchronisiert.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce-Verkaufschancen Bildschirm":::

    6. Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.

## <a name="next-steps"></a>Nächste Schritte

- [Weitere Informationen zur Microsoft powerautomatisieren-Plattform](https://docs.microsoft.com/-automate/)

- [Verwalten von Leads](manage-leads.md)

- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)

- [Partner Center-Webhooks](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)