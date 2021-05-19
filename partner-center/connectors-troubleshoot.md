---
title: Problembehandlung bei Connectors mit Co-Selling-Empfehlungen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier finden Sie Antworten auf häufig gestellte Fragen zur Verwendung von Co-Sell-Connectors. Lesen Sie diese häufig gestellten Fragen zur Problembehandlung für Co-Sell-Connectors.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148345"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Problembehandlung bei Connectors mit Co-Selling-Empfehlungen

**Gilt für**: Dynamics 365 CRM | Salesforce CRM

**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Systemadministrator oder Systemanpasser im CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Fragen und Antworten zu Voraussetzungen

1. Können Sie eine Testlösung für Co-Sell-Empfehlungsconnectors für Ihre Umgebung verwenden?

Wenn Sie sich in der Test-/Stagingumgebung befinden, können Sie eine Testlösung wählen. Die kostenpflichtige Version der Connectors ist in AppSource für 15 US-Dollar pro Monat verfügbar. Mit der kostenpflichtigen Verbindung erhalten Sie 10.000 API-Aufrufe pro Tag. Die Connectors sind Wrapper auf Partner Center Empfehlungs-APIs. Wenn die Connectorlösungen für ein **Create-** oder **Update-Ereignis** für die Verkaufschancen auf Partner Center crm-Seite ausgeführt werden, wird ein API-Aufruf ausgeführt.

2. Welche Rolle benötigen Sie, um Abschnitte in der CRM-Umgebung zu erstellen?

Benutzer, die Systemadministratoren oder Systemanpasser sind, können Änderungen für alle Benutzer anwenden. Alle App-Benutzer können jedoch das System personalisieren und sogar einige ihrer Anpassungen mit anderen teilen. 

3. Benötigen Partnerverkäufer spezielle Rollen, um an Partner Center?
 
Partnerverkäufern muss die Rolle "Empfehlungsadministrator" zugewiesen werden. Weitere Informationen finden Sie unter [Übersicht über Berechtigungen.](create-user-accounts-and-set-permissions.md)

4. Welche Felder müssen zuerst in Ihrer CRM-Umgebung eingerichtet werden? 

• Stellen Sie sicher, dass Ihre Währung für Ihren Standort geeignet ist und sich genau in Ihrer CRM-Umgebung befindet. • Ihr Vertriebsteam sollte in Ihrer CRM-Umgebung als CRM-Benutzer aufgeführt werden.

5. Welche Voraussetzungen sind für die Erstellung Power Automate Umgebung erforderlich?

Um die Power Automate-Umgebung verwenden zu können, benötigen Sie Folgendes:

- Eine Power Automate Lizenz ist erforderlich.
- Mindestens 1 GB Speicher ist erforderlich.

6.  Benötigen Sie ein Dynamics 365-Abonnement, um die Salesforce Connectors-Lösung verwenden zu können?

Die Salesforce Connector-Lösung ist vom Typ "Dynamics Flow", der die Synchronisierung mit anderen CRM-Systemen unterstützt. Für die Lösung ist es nicht erforderlich, dass Sie über eine Dynamics 365-Instanz oder ein Abonnement verfügen. Während der Installation der Salesforce-Lösung wird möglicherweise eine Dropdown-Datei mit vorhandener CDS-Umgebung in Ihrem Unternehmen angezeigt. Sie müssen diese Umgebung auswählen. Wenn Sie außerdem die Fehlermeldung "Es konnte keine Dynamics 365-Organisation gefunden werden, die mit einem angemeldeten Benutzer verbunden ist" erhalten, müssen Sie eine neue Umgebung für den Connector erstellen.

## <a name="questions-and-answers-about-configuration"></a>Fragen und Antworten zur Konfiguration

1. Was sollten Sie tun, wenn beim Aktivieren von Flows in Power Automate Platform der folgende Fehler auftritt?

Fehler: Fehler bei Anforderung an Azure Resource Manager mit folgendem Fehler: '{"error":{"code":"WorkflowTriggerNotFound","message":"Der Workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'. 

Führen Sie die folgenden Schritte zur Problembehandlung aus:

- Löschen Sie die CDS-Verbindung, und erstellen Sie die CDS-Verbindungen neu.
- Deaktivieren und Aktivieren des untergeordneten Flows 
- Löschen Sie die Projektmappe, und installieren Sie sie neu. 

2.  Was sollten Sie tun, wenn beim Hinzufügen eines Partner Center Connectors in Power Automate Platform der Fehler "Anmelden" auftritt?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fehlermeldung, die eine Anmeldung erfordert":::

Führen Sie diesen Problembehandlungsschritt aus:

- Verwenden Sie Partner Center Anmeldeinformationen, um sich einmal bei der Flowumgebung anzumelden (flow.microsoft.com).


3. Was sollten Sie tun, wenn sie beim Aktivieren des Partner Center crm-Flusses in der Power Automate-Plattform die folgende Fehlermeldung erhalten?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fehlermeldung, die Updates erfordert":::

Führen Sie die folgenden Schritte zur Problembehandlung aus:

- Aktivieren Sie zuerst die folgenden beiden untergeordneten Flows, bevor Sie den Partner Center CRM-Flow aktivieren.
      - Partner Center crm – Helper (Insider Preview)
      - Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)

4. Was sollten Sie tun, wenn Sie keine Verbindungen zum Flow hinzufügen können, wenn Sie versuchen, den Flow zu bearbeiten?

Sie fügen verbindungen zum Flow hinzu, während der Flow ausgeführt wird, und fügen sie jedem Flow separat hinzu.  Wenn das Dialogfeld zum Hinzufügen von Verbindungen beim Bearbeiten des Flows nicht automatisch geöffnet wird, können Sie die einzelnen Schritte und Unterschritte der Flows einzeln bearbeiten.

- Wählen Sie jeden Flow aus, und bearbeiten Sie sie einzeln.
- Erweitern aller Schritte im Flow 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Schritte, die Verbindungen benötigen":::

- Wählen Sie die Schritte aus, in denen ein Warnsymbol angezeigt wird, in dem Sie aufgefordert werden, Verbindungen zu verknüpfen und Verbindungen hinzuzufügen. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Schritt-für-Schritt-Bearbeiten des Datenflusses":::


5. Was sollten Sie tun, wenn die Flows der Lösung für Co-Sell-Empfehlungsconnectors nicht ein aktivieren?

A. In Power Automate müssen Sie Flows in der folgenden Reihenfolge bearbeiten und aktualisieren, um die richtigen Verbindungen zu verwenden:

- Partner Center Webhookregistrierung (Insider Preview)
- Erstellen einer Co-Sell-Empfehlung – Salesforce Partner Center (Insider Preview)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center zu Salesforce (Insider Preview)
- Salesforce zu Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

 B. Wählen Sie für jeden Flow die Option **Nur Benutzer ausführen** aus. Wählen Sie Verbindung anstelle **von Vom benutzer nur ausführen bereitgestellt** **verwenden** aus.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="So aktivieren Sie einen Flow":::


C. Aktivieren Sie diese unten erwähnten Flows:

 - Partner Center Microsoft Co-Selling-Empfehlungsupdates für Salesforce (Insider Preview)

- Salesforce zu Partner Center (Insider Preview)

    
D: Aktivieren Sie alle verbleibenden Flows.

E. Wählen Sie unter Flow Partner Center Webhookregistrierung die Option **Ausführen** aus. Geben Sie die **HTTP-URL** aus der ersten Aktion in Partner Center salesforce flow **an.** Wählen Sie unter **Zu registrierende Ereignisse** alle vier Optionen aus, und wählen Sie für Überschreiben die Option **Ja** aus.

## <a name="questions-and-answers-about-runmaintenance"></a>Fragen und Antworten zu Ausführung/Wartung

1. Wie beheben Sie Fehler während Power Automate Flowausführung?

Um sicherzustellen, dass Ihre Power Automate Flows erwartungsvoll ausgeführt werden und Fehler während der Ausführung behoben werden können, lesen Sie [Beheben von Flowfehlern.](/power-automate/fix-flow-failures)

2. Was sollten Sie tun, wenn Empfehlungen angezeigt werden, die in Partner Center- oder CRM-Umgebung nicht ordnungsgemäß synchronisiert werden?
 
Wählen Sie **Überwachen** aus, um den Status der Empfehlungssynchronisierung zu bestimmen. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisieren von Empfehlungen":::

Stellen Sie sicher, dass die folgenden Bedingungen erfüllt sind:

- Die Lösungs-ID wird im Rahmen der Verkaufschance bereitgestellt.

- Der Ländercode mit zwei Buchstaben ist erforderlich.

- Wenn hilfe von Microsoft für die Verkaufschance ausgewählt ist, sind Kundenkontaktinformationen erforderlich.

3. Wie kann sichergestellt werden, dass eine Empfehlung bidirektional synchronisiert wird?

Führen Sie die folgenden Schritte aus:

- Partnerverkäufer müssen sicherstellen, dass sie die Option **Sync with Partner Center** im CRM-Abschnitt aktiviert haben.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Stellen Sie sicher, dass Synch aktiviert ist.":::

- Verkäufer müssen umsatz- und enddatumsgemäß bereitstellen, wenn sie einen Lead qualifizieren.

- Wenn die CRM-ID  in  der Erstellungs- oder Aktualisierungsphase der Co-Sell-Verkaufschance angegeben wird, aber eine Leadchance mit dieser ID in CRM nicht gefunden wird, wird das Aktualisieren oder Erstellen ignoriert.

- Stellen Sie sicher, dass das Feld für die Empfehlungswährung in der Salesforce-Umgebung konfiguriert ist. 

4. Was sollten Sie tun, wenn der Connector getrennt wird und Sie eine Empfehlungssynchronisierung verpasst haben?

Im Folgenden finden Sie einige der Optionen, die Sie ausprobieren können:

- Überprüfen Sie, ob der Benutzername oder das Kennwort für den Partner Center Benutzer mit Administratorrollen für Empfehlungen abgelaufen ist.

- Sie können zur nicht synchronisierten Verkaufschance wechseln, ein kleineres Update machen und beobachten, ob die Empfehlung synchronisiert wurde.

- Wenn die Flows ausgeführt wurden und fehlgeschlagen sind, wählen Sie den Flow aus, und übermitteln Sie die fehlgeschlagene Ausführung erneut.

5. Was sollten Sie tun, wenn Sie Zugriffsfehler erhalten?

Stellen Sie sicher, dass die entsprechenden Rollen vorhanden sind.

- Rolle "Empfehlungsadministrator" für Partner Center Verkäufer 
 
- Systemadministrator oder Systemanpasserrolle für Ihre CRM-Instanz

- Stellen Sie sicher Power Automate dass sich der Benutzer des Kontos mindestens https://flow.microsoft.com einmal im Voraus bei anmeldet.

6. Wenn Sie sehen, dass **der Ländercode des** Kundenkontos beim Erstellen einer Co-Sell-Verkaufschance fehlt, was sollten Sie tun?

Sie müssen dem Kundenkonto in CRM den zwei buchstabenbasierten ISO-Ländercode hinzufügen.

7. Was sollten Sie tun, wenn der Fehler angezeigt wird, dass die **Lösungs-ID** beim Erstellen einer Co-Sell-Verkaufschance erforderlich ist?

Um eine Co-Sell-Empfehlung zu erstellen, benötigen Sie eine Microsoft-Lösung, die für den Co-Sell bereit ist. 

8. Was sollten Sie tun, wenn in Partner Center Co-Sell-Verkaufschancen entstehen, die nicht mit CRM synchronisiert werden, obwohl keine Flowfehler auftreten?

Gehen Sie folgendermaßen vor:

- Nachdem Sie in Partner Center einen neuen Co-Sell-Deal erstellt haben, überprüfen Sie, ob der Flow Partner Center zu Dynamics 365 aufgerufen wird (er wird möglicherweise mehrmals aufgerufen).

- Wenn der Flow aufgerufen wird, überprüfen Sie alle aufgerufenen Flows, und identifizieren Sie die Flow-Ausführung, die das CRM aktualisieren würde. Sie können die Aktionen ausführen und überprüfen, ob das CRM aktualisiert wurde oder ein Problem aufgetreten ist.

- Überprüfen **Sie in der** Partner Center, ob er mit der CRM-ID aufgefüllt wird.

- Stellen Sie sicher, dass der Deal nicht versehentlich als **Won** oder **Lost** in Partner Center.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)
 
- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
