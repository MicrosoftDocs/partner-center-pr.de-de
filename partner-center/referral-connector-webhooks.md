---
title: Verwenden von webhooks zum erhalten von Ressourcen Änderungs Ereignissen
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verwenden Sie die webhook-APIs, um herauszufinden, wann Ressourcen Änderungen der Verweise auftreten.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: Verweise, webhook-API, Ressourcen Änderungs Ereignisse
ms.localizationpriority: medium
ms.openlocfilehash: a141776f1b591ebe41bb740051802b4b55cf36f0
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/22/2020
ms.locfileid: "83796206"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Verwenden von webhook-APIs zum Registrieren für Ressourcen Änderungs Ereignisse

### <a name="appropriate-roles"></a>Geeignete Rollen

- Empfehlungsadministrator
- Systemadministrator oder systemanpassungsmodul für Dynamics 365 CRM oder Salesforce CRM


Die Partner Center-webhook-APIs ermöglichen es Ihnen, sich für Ressourcen Änderungs Ereignisse zu registrieren. Diese Änderungs Ereignisse werden als http-Beiträge an Ihre URL gesendet.

>[!NOTE]
>In diesem Thema werden webhook-APIs für Dynamics 365 CRM und Salesforce CRM erläutert.

1. Um Ihre URL zu registrieren, wählen Sie **Partner Center-webhook-Registrierung (Insider Vorschau)** Energie automatisierter Flow aus.

2. Hinzufügen von Verbindungen für (a.) Partner Center-Benutzer mit referengenalen Administrator Anmelde Informationen (b) Partner Center-Veranstaltungen wie unten gezeigt

![Trigger](images/cosellconnectors/triggerflow.png)

3. Wenn Sie diese Updates vornehmen, sehen Sie

![webhooks](images/cosellconnectors/webhook1.png)

4. Speichern Sie die Änderungen, und wählen Sie **einschalten aus**. 

Führen Sie die folgenden Schritte aus, um Partner Center-webhooks zum lauschen auf Ereignis Änderungen in den IP-Co-Selling/Independent-Referenzobjekten in Partner Center und CRM-Systemen zu aktivieren:

5. Wählen Sie **Partner Center für Dynamics 365 (Insider Preview)** oder **Partner Center für Salesforce (Insider Preview)** aus.

6. Wählen Sie das **Bearbeitungs** Symbol aus, und wählen Sie **bei Empfang einer HTTP-Anforderung**aus.

7. Wählen Sie das **Kopier** Symbol aus, um die bereitgestellte HTTP Post-URL zu kopieren.

![Kopieren der URL](images/cosellconnectors/copyurl.png)

8. Wählen Sie jetzt die Option "Partner Center-webhook-Registrierung (Insider Vorschau)", und wählen Sie **Ausführen**aus.

9. Stellen Sie sicher, dass im rechten Bereich das Fenster "Flow ausführen" geöffnet wird, und klicken Sie auf **weiter**.

10. Geben Sie die folgenden Details ein: 

    a. **Http-auslöserendpunkt**: aus dem vorherigen Schritt kopierte URL

    b. **Zu Registrier folgende Ereignisse**: "Verweis-erstellt" und "Verweis-aktualisiert"

    c. **Vorhandene auslöserendpunkte überschreiben, falls vorhanden**: Ja (Dadurch werden alle vorhandenen Endpunkte überschrieben.)

Der webhook kann nun auf Änderungen lauschen (erstellen und Aktualisieren von Ereignissen). 

11. Wählen Sie **Ausführen** aus, und wählen Sie dann **abgeschlossen aus.**

 ## <a name="customize-synchronization-steps"></a>Synchronisierungs Schritte anpassen

Wenn Co-Selling-Referenzen zwischen Partner Center und Ihrem CRM-System synchronisiert werden, werden die Felder, die auf dem Partner Center-PC synchronisiert werden, hier aufgeführt.

Häufig sind CRM-Systeme hochgradig angepasst. Sie können die Strom automatisierten Flows anpassen. Befolgen Sie den Leitfaden für die Feld Zuordnung, und nehmen Sie ggf. entsprechende Änderungen in den Schritten der Strom automatisierten Flows vor.  Microsoft Partner Center-zu-CRM-Zuordnungen werden bereitgestellt, aber je nach Ihrer CRM-Umgebung können Sie die Felder weiter anpassen.

Je nach Ihren Anforderungen können mehrere Schritte der einzelnen Strom automatisierten Flows angepasst werden. Im folgenden finden Sie Beispiele für verfügbare Anpassungen:

1. So passen Sie die Felder für die CREATE-oder Update-Ereignisse im Partner Center an die CRM-Referenz Synchronisierung an: 

    a. Wählen Sie Partner Center für Dynamics 365 (Insider Preview) oder Partner Center für Salesforce (Insider Preview) aus.

    b. Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.

    c. Select **(Bereich) Hiermit wird der Lead oder die Verkaufschance synchronisiert**.

2. Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Erstellungs Ereignisse aus, wenn es sich um eine **neue freigegebene Chance handelt, und** Wählen Sie den unterschritt aus, **Falls ja** , und erweitern Sie dann die Option **neue Gelegenheit im CRM**. Sie können die Zuordnungen in diesem Abschnitt mithilfe des Leitfaden für die Feld Zuordnung bearbeiten.

    d. Zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Update Ereignisse klicken Sie auf den Schritt "(Bereich) Synchronisieren des Leads oder der Verkaufschance".

    e. Wählen Sie aus **, ob es sich um ein Update für eine Verkaufschance handelt**. Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann bei **Unterschied zwischen den Verkaufschancen-Objekten in Partner Center und CRM**.  

    f. Wählen Sie aus, **ob ja** gefolgt von **vorhandener Option aktualisieren**
       
3. So passen Sie die Felder für die CRM-zu-PC-Referenz Synchronisierung für Update Ereignisse an

    a. Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.

    b. Select **(Bereich) Synchronisieren der Verkaufschance**.

    c. Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Aktualisierungs Ereignisse aus, **ob es Unterschiede zwischen den führenden Objekten in Partner Center und CRM gibt**. 

    d. Wählen Sie den unterschritt **bei ja** aus, und erweitern Sie dann den Schritt **Aktualisieren eines Verweises mit Verkaufschancen Daten**.

Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.

4. Zum Anpassen der Felder für die CRM-zu-PC-Referenz Synchronisierung für Erstellungs Ereignisse

   a. Wählen Sie **Bearbeiten** aus, um den Energie automatisierten Flow zu bearbeiten bzw. anzupassen.

   b. Wählen Sie die **Synchronisierungs Verweise aus (Bereich).**

   c. Wählen Sie zum Anpassen von CRM-Feld Zuordnungen (basierend auf Feld Zuordnungs Handbuch) für Create Events die Option **Microsoft-Verweis erstellen**. 

Sie können die Zuordnungen in diesem Abschnitt basierend auf dem Leitfaden für die Feld Zuordnung bearbeiten.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-End-bidirektionale Co-Selling-Synchronisierung

Nachdem Sie die Energie automatisierte Lösung installiert, konfiguriert und angepasst haben, können Sie die Synchronisierung von Co-Selling-Referenzen zwischen Dynamics 365 oder Salesforce und Partner Center testen.

### <a name="pre-requisites"></a>Voraussetzungen

Um die Verweise über Partner Center und Dynamics 365 CRM oder über Partner Center und Salesforce CRM zu synchronisieren, muss die Lösung für die Energie Automatisierung Microsoft-spezifische verweigerfelder eindeutig abgrenzen. Dies bietet Ihren Verkäufer Teams die Möglichkeit, zu entscheiden, welche Referenzen Sie gemeinsam mit Microsoft für Co-Selling verwenden möchten.

Eine Reihe von benutzerdefinierten Feldern ist als Teil der Synchronisierung von Partner Center-Referenzen für Dynamics 365 Solution **Opportunity** verfügbar. Ein CRM-Administrator Benutzer muss einen separaten CRM-Abschnitt mit den benutzerdefinierten Feldern für die Verkaufs **Chance** erstellen.

Die folgenden benutzerdefinierten Felder sollten Teil des CRM-Abschnitts sein:

- **Synchronisierung mit Partner Center**: ob die Gelegenheit mit dem Microsoft Partner Center synchronisiert werden soll

- **Verweis Bezeichner**: ein Schreib geschütztes Bezeichnerfeld für die Microsoft Partner Center-Referenz

- **Verweis Link**: ein Schreib geschützter Link zum Verweis im Microsoft Partner Center

- **Wie kann Microsoft Hilfe erhalten?**: Hilfe von Microsoft für den Verweis

- **Produkte**: Liste der Produkte, die dieser Verkaufschance zugeordnet sind

- Überwachung **: ein**Schreib geschützter Überwachungs Pfad für die Synchronisierung mit Partner Center-verweisen

### <a name="scenarios"></a>SS

1. Verweis Synchronisierung, wenn der Verweis in CRM erstellt oder aktualisiert und in Partner Center synchronisiert wird:

    a. Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung oder Salesforce CRM-Umgebung mit einem Benutzer an, der im Bereich "Verkaufs **Chancen** " von CRM Einblick hat.

    b. Stellen Sie sicher, dass der folgende Abschnitt vorhanden ist, wenn Sie eine "neue Verkaufschance" in der Dynamics 365-Umgebung erstellen.

   ![Verkaufschance](images/cosellconnectors/opportunity.png)

    c. Wenn Sie diese Gelegenheit mit dem Microsoft Partner Center synchronisieren möchten, stellen Sie sicher, dass Sie die folgenden Felder in der Kartenansicht festlegen:

    - "Mit Partner Center synchronisieren": Ja

    - "Wie kann Microsoft Help?": Wählen Sie eine der folgenden Aktionen aus:

    ![Auswahl von Hilfe](images/cosellconnectors/help.png)

    - Produkte: Lösungs-IDs des Produkts

    d. Wenn die Verkaufschance in Dynamics 365 mit **sync with Partner Center** auf **Ja**festgelegt ist, warten Sie 10 Minuten, und melden Sie sich bei Ihrem Partner Center-Konto an. Ihre Verweise werden mit Dynamics 365 synchronisiert.

    e. Wenn Sie die Option in Dynamics 365 CRM aktualisieren, werden die Änderungen daher in Ihrem Partner Center-Konto synchronisiert, wenn Sie die Option "mit Partner Center synchronisieren" auf "Ja" festlegen.

    f. Verkaufschancen, die mit Partner Center erfolgreich synchronisiert werden, werden mit ✔ Symbol in Dynamics 365 identifiziert.

2. Verweis Synchronisierung, wenn der Verweis im Microsoft Partner Center erstellt oder aktualisiert und in der Dynamics 365-Umgebung synchronisiert wird: 

    a. Melden Sie sich bei Ihrem Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/home)an.

    b. Wählen Sie im Menü auf der linken Seite die Option **Verweise** aus.

    c. Erstellen Sie einen neuen Co-Selling-Verweis aus Partner Center, indem Sie auf die Option "neu erstellen" klicken.

    d. Melden Sie sich bei ihrer Dynamics 365 CRM-Umgebung an. 

    e. Navigieren Sie zu **Open Verkaufschancen**. Der im Microsoft Partner Center erstellte Verweis ist nun in Dynamics 365 CRM synchronisiert.

    f. Wenn Sie einen synchronisierten Verweis auswählen, werden die Details der Kartenansicht aufgefüllt.

 ### <a name="next-steps"></a>Nächste Schritte

- [Weitere Informationen zur Microsoft powerautomatisieren-Plattform](https://docs.microsoft.com/power-automate/)

- [Partner Center-webhook-Ereignisse](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [Verwalten von Leads](manage-leads.md)

- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
