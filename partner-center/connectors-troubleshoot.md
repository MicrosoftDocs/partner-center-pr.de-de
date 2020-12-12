---
title: Problembehandlung bei Connectors mit Co-Selling-Empfehlungen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier finden Sie Antworten auf häufig gestellte Fragen zur Verwendung von Co-Selling-Connectors. In diesen FAQ finden Sie Informationen zur Problembehandlung bei Co-Selling-Connectors.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354541"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Problembehandlung bei Connectors mit Co-Selling-Empfehlungen

**Gilt für:**

- Dynamics 365 CRM
- Salesforce-CRM

**Geeignete Rollen**

- Empfehlungsadministrator
- Systemadministrator oder systemanpassungsprogramm im CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Fragen und Antworten zu Voraussetzungen

1. Können Sie für Ihre Umgebung eine "Test-Co-Selling-Connectors"-Lösung verwenden?

Wenn Sie sich in der Test-/Stagingumgebung befinden, können Sie sich für eine Testlösung entscheiden. Die kostenpflichtige Version der Connectors ist in appsource in US-Dollar 15 USD/Monat verfügbar. Mit der kostenpflichtigen Verbindung erhalten Sie pro Tag 10K API-Aufrufe. Die Connectors sind Wrapper zusätzlich zu den Partner Center-Referenz-APIs. Wenn die Connector-Lösungen für ein Erstellungs-oder **Update** Ereignis für die Verkaufschancen in Partner Center oder auf der CRM-Seite ausgeführt werden, **erfolgt ein API** -Aufruf.

2. Welche Rolle benötigen Sie, um Abschnitte in der CRM-Umgebung zu erstellen?

Benutzer, die Systemadministratoren oder Systemanpassungen sind, können Änderungen für jeden Benutzer anwenden. Alle App-Benutzer können das System jedoch personalisieren und sogar einige Ihrer Anpassungen mit anderen Teilen. 

3. Benötigen Partner Verkäufer spezielle Rollen, um im Partner Center arbeiten zu können?
 
Partner Verkäufern muss die Rolle "referenrals admin" zugewiesen werden. Weitere Informationen finden Sie in der folgenden [Berechtigungs Übersicht) (Create-User-Accounts-and-Set--Berechtigungen).

4. Welche Felder müssen zuerst in Ihrer CRM-Umgebung eingerichtet werden? 

• Stellen Sie sicher, dass Ihre Währung für Ihren Standort geeignet ist und sich in Ihrer CRM-Umgebung genau befindet. • Ihr Vertriebsteam sollte in Ihrer CRM-Umgebung als CRM-Benutzer aufgeführt sein.

5. Welche Voraussetzungen sind für das Erstellen der Energie automatisierten Umgebung erforderlich?

Um die Energie automatisierte Umgebung zu verwenden, benötigen Sie Folgendes:

- Eine Strom Automatisierungs Lizenz ist erforderlich.
- Es ist mindestens 1 GB Speicher erforderlich.

6.  Benötigen Sie ein Dynamics 365-Abonnement, um die Salesforce-Connectors-Lösung zu verwenden?

Die Salesforce-Connector-Lösung ist vom Typ "Dynamics Flow", der die Synchronisierung mit anderen CRM-Systemen unterstützt. Die Lösung erfordert nicht, dass Sie über eine Dynamics 365-Instanz oder ein-Abonnement verfügen. Beim Installieren der Salesforce-Lösung wird möglicherweise eine Dropdown-Datei mit vorhandener CDs-Umgebung in Ihrem Unternehmen angezeigt. Sie müssen diese Umgebung auswählen. Wenn Sie die Fehlermeldung "Es konnte keine Dynamics 365-Organisation gefunden werden, die mit dem angemeldeten Benutzer verbunden ist" erhalten, müssen Sie außerdem eine neue Umgebung für den Connector erstellen.

## <a name="questions-and-answers-about-configuration"></a>Fragen und Antworten zur Konfiguration

1. Was sollten Sie tun, wenn beim Aktivieren von Flows in der Energie automatisierten Plattform der folgende Fehler auftritt?

Fehler: die Anforderung zum Azure Resource Manager ist mit dem folgenden Fehler fehlgeschlagen: "{" Error ": {" Code ":" workflowtriggernotfound "," Message ":" der Workflow "e14d00f1-1fdf-4b1b-aaac-54a5064093d3"-Trigger "Manual" konnte nicht gefunden werden. "}}". 

Befolgen Sie diese Schritte zur Problembehandlung:

- Löschen Sie die CDs-Verbindung, und erstellen Sie dann die CDs-Verbindungen.
- Aktivieren und Deaktivieren des untergeordneten Flows 
- Löschen Sie die Lösung, und installieren Sie die Projekt Mappe neu. 

2.  Was sollten Sie tun, wenn Sie sich beim Hinzufügen eines Partner Center-Connector in der Energie automatisierten Plattform mit dem Fehler "Anmelden" auskennen?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fehlermeldung, die eine Anmeldung erfordert":::

Befolgen Sie diese Schritte zur Problembehandlung:

- Verwenden Sie Ihre Partner Center-Anmelde Informationen, um sich einmal bei der Flow-Umgebung anzumelden (Flow.Microsoft.com).


3. Was sollten Sie tun, wenn Sie den folgenden Fehler erhalten, während Sie den Partner Center für CRM-Flow in der Energie automatisierten Plattform aktivieren?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fehlermeldung, die Updates erfordert":::

Befolgen Sie diese Schritte zur Problembehandlung:

- Aktivieren Sie zuerst die folgenden beiden untergeordneten Flows, bevor Sie das Partner Center für CRM Flow aktivieren.
      - Partner Center auf CRM-Hilfsobjekt (Insider Vorschau)
      - Partner Center Microsoft Co-Selling-Verweises Aktualisierungen an CRM (Insider Preview)

4. Was sollten Sie tun, wenn Sie keine Verbindungen zum Flow hinzufügen können, wenn Sie versuchen, den Flow zu bearbeiten?

Wenn der Flow ausgeführt wird, fügen Sie Verbindungen zum Flow hinzu, und Sie fügen den einzelnen Flows separat hinzu.  Wenn das Dialogfeld zum Hinzufügen von Verbindungen beim Bearbeiten des Flows nicht automatisch geöffnet wird, können Sie die einzelnen Schritte und unter Schritte der Flows einzeln bearbeiten.

- Wählen Sie jeden Flow aus, und bearbeiten Sie ihn einzeln.
- Alle Schritte im Flow erweitern 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Schritte, die Verbindungen benötigen":::

- Wählen Sie die Schritte aus, bei denen das Warnsymbol angezeigt wird, um Verbindungen zuzuordnen, und fügen Sie Verbindungen hinzu. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Flow Schritt für Schritt bearbeiten":::


5. Was sollten Sie tun, wenn die Flows der Connectors-Lösung für Co-Selling-Verweise nicht aktiviert werden?

A. In der Energie Automatisierung müssen Sie Flows in der folgenden Reihenfolge bearbeiten und Sie aktualisieren, um die richtigen Verbindungen zu verwenden:

- Partner Center-webhook-Registrierung (Insider Preview)
- Erstellen eines Co-Selling-Verweises-Salesforce an Partner Center (Insider Preview)
- Partner Center Microsoft Co-Selling-Referenz Aktualisierungen an Salesforce (Insider Preview)
- Partner Center zu Salesforce (Insider Vorschau)
- Salesforce zu Partner Center (Insider Vorschau)
- Salesforce-Verkaufschance an Partner Center (Insider Preview)
- Salesforce Microsoft-Lösungen an Partner Center (Insider Preview)

 B. Wählen Sie für jeden Flow die Option **nur Benutzer ausführen** aus. Wählen Sie **Verbindung verwenden** anstelle von **nur Benutzer ohne Benutzer bereit** stellen aus.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="So aktivieren Sie einen Flow":::


C. Aktivieren Sie die folgenden genannten Flows:

 - Partner Center Microsoft Co-Selling-Referenz Aktualisierungen an Salesforce (Insider Preview)

- Salesforce zu Partner Center (Insider Vorschau)

    
D: Aktivieren Sie alle verbleibenden Flows.

E. Wählen Sie unter Flow Partner Center-webhook-Registrierung die Option **Ausführen** aus. Geben Sie die **http-URL** aus der ersten Aktion im **Partner Center für den Salesforce** -Flow an. Wählen Sie unter **zu registrierende Ereignisse** alle vier Optionen aus, und wählen Sie zum Überschreiben **Ja**

## <a name="questions-and-answers-about-runmaintenance"></a>Fragen und Antworten zur Wartung und Wartung

1. Wie werden Probleme bei Fehlern während der Energie automatisierten Fluss Ausführung behoben?

Um sicherzustellen, dass Ihre Energie automatisierenden Flows erwartungsgemäß ausgeführt werden und Fehler während der Ausführung behoben werden können, finden Sie unter [Beheben von Fluss Fehlern](/power-automate/fix-flow-failures)Weitere Informationen.

2. Was sollten Sie tun, wenn Verweise angezeigt werden, die nicht ordnungsgemäß in der Partner Center-oder CRM-Umgebung synchronisiert sind?
 
**Wählen Sie** überwachen aus, um den Status der Verweis Synchronisierung zu bestimmen. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisieren von verweisen":::

Stellen Sie sicher, dass die folgenden Bedingungen erfüllt sind:

- Die Lösungs-ID wird als Teil der Verkaufschance bereitgestellt.

- Zwei buchstabiger Ländercode ist erforderlich.

- Wenn die Hilfe von Microsoft für die Verkaufschance ausgewählt ist, sind Kundenkontaktinformationen erforderlich.

3. Wie kann sichergestellt werden, dass ein Verweis bidirektional synchronisiert wird?

Führen Sie die folgenden Schritte aus:

- Partner Verkäufer müssen sicherstellen, dass die **Synchronisierung mit der Partner Center** -Option im CRM-Abschnitt aktiviert ist.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Stellen Sie sicher, dass die Synchronisierung aktiviert ist":::

- Verkäufer müssen den Umsatz und das Enddatum angeben, wenn Sie einen Lead qualifizieren.

- Wenn die CRM-ID in der Erstellungs-oder **Aktualisierungs** **Phase der Co** -Selling-Verkaufschance bereitgestellt wird, aber eine Lead Gelegenheit mit dieser ID in CRM nicht gefunden wird, wird Update oder CREATE ignoriert.

- Stellen Sie sicher, dass das Feld für die Verweis Währung in der Salesforce-Umgebung 

4. Was Sie tun sollten, wenn der Connector getrennt wird und eine verweissynchronisierung fehlt. 

Im folgenden sind einige der Optionen aufgeführt, die Sie ausprobieren können:

- Überprüfen Sie, ob der Benutzername oder das Kennwort für den Partner Center-Benutzer mit Referenz Administrator Rollen abgelaufen ist

- Sie können zur nicht synchronisierten Gelegenheit wechseln, eine geringfügige Aktualisierung vornehmen und beobachten, ob der Verweis synchronisiert wurde.

- Wenn die Flows ausgeführt wurden und fehlgeschlagen sind, wählen Sie den Flow aus, und übermitteln Sie den ausgefallenen Testlauf erneut.

5. Was sollten Sie tun, wenn Sie Zugriffs Verweigerungs Fehler erhalten?

Stellen Sie sicher, dass die entsprechenden Rollen vorhanden sind

- Rolle "Verweis Administrator" für Partner Center-Verkäufer 
 
- System Administrator-oder systemanpassungsrolle in Ihrer CRM-Instanz

- Stellen Sie sicher, dass sich der Benutzer mit dem Datenfluss Konto automatisch https://flow.microsoft.com bei mindestens einmal anmeldet.

6. Was sollten Sie tun, wenn Sie sehen, dass der **Ländercode des Kundenkontos** beim Erstellen einer Co-Selling-Verkaufschance fehlt?

Sie müssen dem Kundenkonto in CRM den aus zwei Buchstaben bestehenden ISO-Code hinzufügen.

7. Was sollten Sie tun, wenn Sie sehen, dass die **Lösungs-ID erforderlich ist** , während Sie eine Co-Selling-Verkaufschance erstellen?

Um einen Co-Selling-Verweis zu erstellen, benötigen Sie eine Microsoft Co-Selling-Lösung. 

8. Was Sie tun sollten, wenn Sie die Co-Selling-Verkaufschancen in Partner Center sehen, die nicht mit CRM synchronisiert werden, auch wenn keine Datenflussfehler auftreten:

Gehen Sie folgendermaßen vor:

- Nachdem Sie im Partner Center einen neuen Co-Selling-Deal erstellt haben, überprüfen Sie, ob der Flow Partner Center auf Dynamics 365 aufgerufen wird (er wird möglicherweise mehrmals aufgerufen).

- Wenn der Flow aufgerufen wird, überprüfen Sie alle aufgerufenen Flows, und identifizieren Sie die flowausführung, die das CRM aktualisieren würde. Sie können den Aktionen folgen und überprüfen, ob das CRM-Update oder ein Problem aufgetreten ist.

- Überprüfen Sie den *neuen Deal** im Partner Center, um festzustellen, ob es mit der CRM-ID aufgefüllt wird

- Stellen Sie sicher, dass das Geschäft im Partner Center nicht versehentlich als "gewonnen" oder "verloren" geschlossen wird.

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Leads](manage-leads.md)
 
- [Co-Selling-Verkaufschancen](manage-co-sell-opportunities.md)
