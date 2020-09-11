---
title: Rollen, Berechtigungen für Partner Gutschriften
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über die Rollen und Berechtigungen für Partner, die in der Lage sind, vom Partner erworbene Guthaben (PEC) zu verdienen. Diese unterscheiden sich von den Rollen, die in Partner Center funktionieren.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011740"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Rollen und Berechtigungen, die zum erwerben von Partnern berechtigt sind

Die folgenden Rollen entsprechen den Berechtigungsstufen, die bestimmen, ob ein Partner für Gutschriften für Partner qualifiziert ist.

>[!Important]
>Diese Rollen und Berechtigungen sind nicht identisch mit den Rollen und Berechtigungen, die ein Benutzer für die Arbeit im Partner Center benötigt.

|**Rolle**   |**Beschreibung**   |**PEC berechtigt**   |
|-----------------|:------------------|:--------------|
|Besitzer  |Sie verwalten alles, einschließlich des Zugriffs auf Ressourcen.|Ja|
|Mitwirkender |Sie verwalten alles außer dem Gewähren des Zugriffs auf Ressourcen.|Ja|
|Leser|Sie können alles anzeigen, aber keine Änderungen vornehmen.|Nein|
|Acrdelete|ACR-Löschvorgang|Ja|
|Acrimagesigner|ACR-Imagesignaturgeber|Ja|
|Acrpull|ACR-Pullvorgang|Ja|
|AcrPush|ACR-Pushvorgang|Ja|
|AcrQuarantineReader|ACR-Quarantänedatenleser|Nein|
|AcrQuarantineWriter| ACR-Quarantänedatenschreiber|Ja|
|Mitwirkender des API-Verwaltungsdienstes|Kann Dienst und APIs verwalten.|Ja|
|Operatorrolle des API Management-Diensts|Kann den Dienst, aber nicht die APIs verwalten.|Ja|
|Leserrolle des API Management-Diensts|Schreibgeschützter Zugriff auf Dienst und APIs|Nein|
|Mitwirkender der Application Insights-Komponente|Verwaltet Application Insights Komponenten|Ja|
|Application Insights-Momentaufnahmedebugger|Gibt dem Benutzer die Berechtigung zum Anzeigen und Herunterladen von Debugmomentaufnahmen, die mit dem Application Insights-Momentaufnahmedebugger erfasst wurden. Beachten Sie, dass diese Berechtigungen in der Rolle Besitzer oder Mitwirkender nicht enthalten sind.|Ja|
Automation-Auftragsoperator | Hiermit werden Aufträge mithilfe von Automation-Runbooks erstellt und verwaltet. | Ja | 
Operator für Automation | Automatisierungsoperatoren können Aufträge starten, beenden, anhalten und fortsetzen. | Ja | 
Automation-Runbookoperator | Runbookeigenschaften lesen: Ermöglicht das Erstellen von Runbookaufträgen. | Ja | 
Avere-Mitwirkender | Kann einen Avere vFXT-Cluster erstellen und verwalten. | Ja | 
Avere-Bediener | Wird vom Avere vFXT-Cluster zum Verwalten des Clusters verwendet | Ja | 
Azure Event Hubs-Datenbesitzer | Ermöglicht den uneingeschränkten Zugriff auf die Azure Event Hubs-Ressourcen. | Ja | 
Azure Event Hubs-Datenempfänger | Ermöglicht Empfängern den Zugriff auf die Azure Event Hubs-Ressourcen. | Ja | 
Azure Event Hubs-Datensender | Ermöglicht Absendern den Zugriff auf die Azure Event Hubs-Ressourcen. | Ja | 
Administratorrolle für Azure Kubernetes Service-Cluster | Listet die Aktion für Anmeldeinformationen des Clusteradministrators auf. | Ja | 
Benutzerrolle für Azure Kubernetes Service-Cluster | Listet die Aktion für Anmeldeinformationen des Clusterbenutzer auf. | Ja | 
Azure Maps-Datenleser (Vorschauversion) | Gewährt Lesezugriff auf kartenbezogene Daten von einem Azure Maps-Konto. | Nein | 
Azure Service Bus-Datenbesitzer | Ermöglicht den uneingeschränkten Zugriff auf die Azure Service Bus-Ressourcen. | Ja | 
Azure Service Bus-Datenempfänger | Ermöglicht Empfängern den Zugriff auf die Azure Service Bus-Ressourcen. | Ja | 
Azure Service Bus-Datensender | Ermöglicht Absendern den Zugriff auf die Azure Service Bus-Ressourcen. | Ja | 
Besitzer der Azure Stack-Registrierung | Ermöglicht Ihnen die Verwaltung von Azure Stack-Registrierungen. | Ja | 
Mitwirkender für Sicherungen | Ermöglicht Ihnen die Verwaltung des Sicherungsdiensts. Sie können jedoch keine Tresore erstellen oder anderen Benutzern Zugriff gewähren. | Ja | 
Sicherungsoperator | Ermöglicht Ihnen das Verwalten von Sicherungsdiensten, jedoch nicht das Entfernen der Sicherung, die Tresorerstellung und das Erteilen von Zugriff an andere Benutzer. | Ja | 
Sicherungsleser | Kann Sicherungsdienste anzeigen, aber keine Änderungen vornehmen. | Nein | 
Abrechnungsleser | Hiermit wird Lesezugriff auf Abrechnungsdaten ermöglicht. | Nein | 
Mitwirkender von BizTalk | Ermöglicht Ihnen das Verwalten von BizTalk-Diensten, nicht aber den Zugriff darauf. | Ja | 
Zugriff auf Blockchainmitgliedsknoten (Vorschauversion) | Ermöglicht den Zugriff auf Blockchainmitgliedsknoten. | Ja | 
Blueprint-Mitwirkender | Kann Blaupausendefinitionen verwalten, aber nicht zuweisen. | Ja | 
Blueprint-Operator | Kann vorhandene veröffentlichte Blaupausen zuweisen, aber keine neuen Blaupausen erstellen. HINWEIS: Dies funktioniert nur, wenn die Zuweisung mit einer vom Benutzer zugewiesenen verwalteten Identität erfolgt. | Ja | 
Mitwirkender für den CDN-Endpunkt | Kann CDN-Endpunkte verwalten, aber anderen Benutzern keinen Zugriff erteilen. | Ja | 
CDN-Endpunktleser | Kann CDN-Endpunkte anzeigen, aber keine Änderungen vornehmen. | Nein | 
Mitwirkender für das CDN-Profil | Kann CDN-Profile und deren Endpunkte verwalten, aber anderen Benutzern keinen Zugriff erteilen. | Ja | 
CDN-Profilleser | Kann CDN-Profile und deren Endpunkte anzeigen, aber keine Änderungen vornehmen. | Nein | 
Mitwirkender von klassischem Netzwerk | Ermöglicht Ihnen das Verwalten von klassischen Netzwerken, nicht aber den Zugriff darauf. | Ja | 
Mitwirkender von klassischem Speicherkonto | Ermöglicht Ihnen das Verwalten klassischer Speicherkonten, nicht aber den Zugriff darauf. | Ja | 
Klassische Dienstrolle „Speicherkonto-Schlüsseloperator“ | Klassische Speicherkonto-Schlüsseloperatoren dürfen Schlüssel für klassische Speicherkonten auflisten und neu generieren. | Ja | 
Mitwirkender von klassischen virtuellen Computern | Ermöglicht Ihnen das Verwalten klassischer virtueller Computer, aber weder den Zugriff darauf noch auf die mit ihnen verbundenen virtuellen Netzwerke oder Speicherkonten. | Ja | 
Mitwirkender für Cognitive Services | Ermöglicht Ihnen das Erstellen, Lesen, Aktualisieren, Löschen und Verwalten von Cognitive Services-Schlüsseln. | Ja | 
Cognitive Services-Datenleser (Vorschau) | Ermöglicht das Lesen von Cognitive Services-Daten. | Nein | 
Cognitive Services-Benutzer | Ermöglicht Ihnen das Lesen und Auflisten von Cognitive Services-Schlüsseln. | Nein | 
Cosmos DB-Rolle „Kontoleser“ | Kann Azure Cosmos DB-Kontodaten lesen. Informationen zum Verwalten von Azure Cosmos DB-Konten finden Sie unter Mitwirkender von DocumentDB-Konto. | Nein | 
Cosmos DB-Operator | Ermöglicht das Verwalten von Azure Cosmos DB-Konten, aber nicht das Zugreifen auf deren Daten. Verhindert den Zugriff auf Kontoschlüssel und Verbindungszeichenfolgen. | Ja | 
CosmosBackupOperator | Kann eine Wiederherstellungsanforderung für eine Cosmos DB-Datenbank oder einen Container für ein Konto übermitteln. | Ja | 
Mitwirkender für Cost Management | Ermöglicht Ihnen das Anzeigen der Kosten und das Verwalten der Kostenkonfiguration (z. B. Budgets, Exporte). | Ja | 
Cost Management-Leser | Ermöglicht Ihnen das Anzeigen der Kostendaten und -konfiguration (z. B. Budgets, Exporte). | Nein | 
Data Box-Mitwirkender | Ermöglicht Ihnen das Verwalten aller Komponenten unter dem Data Box-Dienst, mit Ausnahme der Gewährung des Zugriffs für andere Benutzer. | Ja | 
Data Box-Leser | Ermöglicht Ihnen das Verwalten des Data Box-Diensts, mit Ausnahme der Erstellung von Aufträgen oder der Bearbeitung von Auftragsdetails und der Gewährung des Zugriffs für andere Benutzer. | Nein | 
Mitwirkender von Data Factory | Erstellen und verwalten Sie Data Factorys sowie die darin enthaltenen untergeordneten Ressourcen. | Ja | 
Data Lake Analytics-Entwickler | Ermöglicht Ihnen das Übermitteln, Überwachen und Verwalten Ihrer eigenen Aufträge, aber nicht das Erstellen oder Löschen von Data Lake Analytics-Konten. | Ja | 
Datenpurger | Kann Analysedaten endgültig löschen. | Ja | 
DevTest Labs-Benutzer | Ermöglicht Ihnen das Verbinden, Starten, Neustarten und Herunterfahren Ihrer virtuellen Computer in Ihren Azure DevTest Labs. | Ja | 
DNS Zone Contributor | Ermöglicht Ihnen die Verwaltung von DNS-Zonen und Ressourceneintragssätzen in Azure DNS, aber nicht zu steuern, wer darauf Zugriff hat. | Ja | 
Mitwirkender von DocumentDB-Konto | Kann Azure Cosmos DB-Konten verwalten. Azure Cosmos DB wurde früher als DocumentDB bezeichnet. | Ja | 
EventGrid EventSubscription-Mitwirkender | Ermöglicht die Verwaltung von EventGrid-Ereignisabonnementvorgängen. | Ja | 
EventGrid EventSubscription-Leser | Ermöglicht das Lesen von EventGrid-Ereignisabonnements. | Nein | 
HDInsight-Clusteroperator | Ermöglicht Ihnen das Lesen und Ändern von HDInsight-Clusterkonfigurationen. | Ja | 
Mitwirkender für die HDInsight-Domänendienste | Ermöglicht Ihnen, Vorgänge im Zusammenhang mit Domänendiensten, die für das HDInsight Enterprise-Sicherheitspaket erforderlich sind, zu lesen, zu erstellen, zu ändern und zu löschen. | Ja | 
Mitwirkender von Intelligent Systems-Konto | Ermöglicht Ihnen das Verwalten von Intelligent Systems-Konten, nicht aber den Zugriff darauf. | Ja | 
Key Vault-Mitwirkender | Ermöglicht Ihnen die Verwaltung von Schlüsseltresoren, aber nicht den Zugriff darauf. | Ja | 
Lab-Ersteller | Ermöglicht Ihnen das Erstellen, Verwalten und Löschen verwalteter Labs unter Ihren Azure Lab-Konten. | Ja | 
Log Analytics-Mitwirkender | Ein Log Analytics-Mitwirkender kann alle Überwachungsdaten lesen und Überwachungseinstellungen bearbeiten. Das Bearbeiten von Überwachungseinstellungen schließt folgende Aufgaben ein: Hinzufügen der VM-Erweiterung zu VMs, Lesen von Speicherkontoschlüsseln zum Konfigurieren von Protokollsammlungen aus Azure Storage, Erstellen und Konfigurieren von Automation-Konten, Hinzufügen von Lösungen, Konfigurieren der Azure-Diagnose für alle Azure-Ressourcen. | Ja | 
Log Analytics-Leser | Ein Log Analytics-Leser kann alle Überwachungsdaten anzeigen und durchsuchen sowie Überwachungseinstellungen anzeigen. Hierzu zählt auch die Anzeige der Konfiguration von Azure-Diagnosen für alle Azure-Ressourcen. | Nein | 
Mitwirkender für Logik-Apps | Ermöglicht Ihnen die Verwaltung von Logik-Apps. Sie können aber nicht den App-Zugriff ändern. | Ja | 
Logik-App-Operator | Ermöglicht Ihnen das Lesen, Aktivieren und Deaktivieren von Logik-Apps. Sie können diese aber nicht bearbeiten oder aktualisieren. | Ja | 
Rolle „Bediener für verwaltete Anwendung“ | Ermöglicht Ihnen das Lesen und Durchführen von Aktionen für Ressourcen der verwalteten Anwendung. | Ja | 
Leser für verwaltete Anwendungen | Ermöglicht Ihnen, Ressourcen in einer verwalteten App zu lesen und JIT-Zugriff anzufordern. | Nein | 
Mitwirkender für verwaltete Identität | Dem Benutzer zugewiesene Identität erstellen, lesen, aktualisieren und löschen. | Ja | 
Operator für verwaltete Identität | Dem Benutzer zugewiesene Identität lesen und zuweisen. | Ja | 
Verwaltungsgruppenmitwirkender | Rolle „Verwaltungsgruppenmitwirkender“ | Ja | 
Verwaltungsgruppenleser | Rolle „Verwaltungsgruppenleser“ | Nein | 
Überwachungsmitwirkender | Kann sämtliche Überwachungsdaten lesen und Überwachungseinstellungen bearbeiten. Siehe auch Erste Schritte mit Rollen, Berechtigungen und Sicherheit in Azure Monitor. | Ja | 
Herausgeber von Überwachungsmetriken | Ermöglicht die Veröffentlichung von Metriken für Azure-Ressourcen. | Ja | 
Überwachungsleser | Kann alle Überwachungsdaten (Metriken, Protokolle usw.) lesen. Siehe auch Erste Schritte mit Rollen, Berechtigungen und Sicherheit in Azure Monitor. | Nein | 
Mitwirkender von virtuellem Netzwerk | Ermöglicht Ihnen das Verwalten von Netzwerken, nicht aber den Zugriff darauf. | Ja | 
Mitwirkender von New Relic APM-Konto | Ermöglicht Ihnen das Verwalten von New Relic Application Performance Management-Konten und -Anwendungen, nicht aber den Zugriff auf diese. | Ja | 
Lese- und Datenzugriff | Ermöglicht Ihnen das Anzeigen sämtlicher Aspekte, jedoch nicht das Löschen oder Erstellen eines Speicherkontos oder einer darin enthaltenen Ressource. Sie können auch Lese-/Schreibzugriff auf alle Daten in einem Speicherkonto durch Zugriff auf Speicherkontoschlüssel gewähren. | Ja | 
Mitwirkender von Redis-Cache | Ermöglicht Ihnen das Verwalten von Redis Caches, nicht aber den Zugriff darauf. | Ja | 
Mitwirkender an Ressourcenrichtlinien (Vorschau) | (Vorschau) Über EA abgeglichene Benutzer mit Rechten zum Erstellen/Ändern der Ressourcenrichtlinie, zum Erstellen eines Supporttickets und zum Lesen von Ressourcen/der Hierarchie. | Ja | 
Mitwirkender von Zeitplanungsauftragssammlung | Ermöglicht Ihnen das Verwalten von Scheduler-Auftragssammlungen, nicht aber den Zugriff darauf. | Ja | 
Mitwirkender von Suchdienst | Ermöglicht Ihnen das Verwalten von Search-Diensten, nicht aber den Zugriff darauf. | Ja | 
Sicherheitsadministrator | Nur in Security Center: Kann Sicherheitsrichtlinien und -zustände anzeigen, Sicherheitsrichtlinien bearbeiten sowie Warnungen und Empfehlungen anzeigen und verwerfen | Ja | 
Sicherheits-Manager (Legacy) | Dies ist eine Legacyrolle. Verwenden Sie stattdessen „Sicherheitsadministrator“. | Ja | 
Sicherheitsleseberechtigter | Nur in Security Center: Kann Empfehlungen und Warnungen sowie Sicherheitsrichtlinien und -zustände anzeigen, aber keine Änderungen vornehmen | Nein | 
Site Recovery-Mitwirkender | Ermöglicht Ihnen die Verwaltung des Site Recovery-Diensts mit Ausnahme der Tresorerstellung und der Rollenzuweisung. | Ja | 
Site Recovery-Operator | Ermöglicht Ihnen ein Failover und ein Failback, aber nicht das Durchführen weiterer Site Recovery-Verwaltungsvorgänge. | Ja | 
Site Recovery-Leser | Ermöglicht Ihnen die Anzeige des Site Recovery-Status, aber nicht die Durchführung weiterer Verwaltungsvorgänge. | Nein | 
Spatial Anchors-Kontomitwirkender | Ermöglicht Ihnen das Verwalten von Raumankern in Ihrem Konto, nicht jedoch das Löschen von Ankern. | Ja | 
Spatial Anchors-Kontobesitzer | Ermöglicht Ihnen das Verwalten von Raumankern in Ihrem Konto, einschließlich der Löschung von Ankern. | Ja | 
Spatial Anchors-Kontoleser | Ermöglicht Ihnen das Ermitteln und Lesen von Eigenschaften für Raumanker in Ihrem Dokument. | Nein | 
Mitwirkender von SQL DB | Ermöglicht Ihnen das Verwalten von SQL-Datenbanken, nicht aber den Zugriff darauf. Darüber hinaus können Sie deren sicherheitsbezogenen Richtlinien oder übergeordneten SQL-Server nicht verwalten. | Ja | 
Verwaltete SQL-Instanz: Mitwirkender | Ermöglicht Ihnen das Verwalten verwalteter SQL-Instanzen und der erforderlichen Netzwerkkonfiguration, jedoch nicht das Erteilen des Zugriffs an andere. | Ja | 
SQL-Sicherheits-Manager | Ermöglicht Ihnen das Verwalten von sicherheitsbezogenen Richtlinien von SQL-Server und Datenbanken, jedoch nicht den Zugriff darauf. | Ja | 
Mitwirkender von SQL Server | Ermöglicht Ihnen, SQL-Server und -Datenbanken zu verwalten, gewährt Ihnen jedoch keinen Zugriff darauf und auch nicht auf deren sicherheitsbezogenen Richtlinien. | Ja | 
Mitwirkender von Speicherkonto | Erlaubt die Verwaltung von Speicherkonten. Ermöglicht den Zugriff auf den Kontoschlüssel, der für den Datenzugriff über die Autorisierung mit einem gemeinsam verwendetem Schlüssel genutzt werden kann. | Ja | 
Dienstrolle „Speicherkonto-Schlüsseloperator“ | Ermöglicht das Auflisten und erneute Generieren von Zugriffsschlüsseln für Speicherkonten. | Ja | 
Mitwirkender an Storage-Blobdaten | Lesen, Schreiben und Löschen von Azure Storage-Containern und -Blobs. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Ja | 
Besitzer von Speicherblobdaten | Bietet Vollzugriff auf Azure Storage-Blobcontainer und -daten, einschließlich POSIX-Zugriffssteuerung. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Ja | 
Leser von Speicherblobdaten | Lesen und Auflisten von Azure Storage-Containern und -Blobs. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Nein | 
Storage Blob-Delegator | Abrufen eines Benutzerdelegierungsschlüssels, mit dem dann eine SAS (Shared Access Signature) für einen Container oder Blob erstellt werden kann, die mit Azure AD-Anmeldeinformationen signiert ist. Weitere Informationen finden Sie unter Erstellen einer SAS für die Benutzerdelegierung. | Ja | 
Speicherdateidaten-SMB-Freigabemitwirkender | Ermöglicht den Lese-, Schreib- und Löschzugriff in Azure Storage-Dateifreigaben über SMB. | Ja | 
Speicherdateidaten-SMB-Freigabemitwirkender mit erhöhten Rechten | Ermöglicht den Lese-, Schreib-, Lösch- und Änderungszugriff auf NTFS-Berechtigungen in Azure Storage-Dateifreigaben über SMB. | Ja | 
Speicherdateidaten-SMB-Freigabeleser | Ermöglicht den Lesezugriff auf Azure-Dateifreigaben über SMB. | Nein | 
Mitwirkender an Storage-Warteschlangendaten | Lesen, Schreiben und Löschen von Azure Storage-Warteschlangen und -Warteschlangennachrichten. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Ja | 
Verarbeiter von Speicherwarteschlangen-Datennachrichten | Einsehen, Abrufen und Löschen einer Nachricht aus einer Azure Storage-Warteschlange. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Ja | 
Absender der Speicherwarteschlangen-Datennachricht | Hinzufügen von Nachrichten zu einer Azure Storage-Warteschlange. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Ja | 
Storage-Warteschlangendatenleser | Lesen und Auflisten von Azure Storage-Warteschlangen und -Warteschlangennachrichten. Um zu erfahren, welche Aktionen für einen bestimmten Datenvorgang erforderlich sind, siehe Berechtigungen für den Aufruf von Datenvorgängen für Blobs und Warteschlangen. | Nein | 
Mitwirkender für Supportanfragen | Ermöglicht Ihnen die Erstellung und Verwaltung von Supportanfragen. | Ja | 
Traffic Manager-Mitwirkender | Ermöglicht Ihnen die Verwaltung von Traffic Manager-Profilen, aber nicht die Steuerung des Zugriffs darauf. | Ja | 
Benutzerzugriffsadministrator | Ermöglicht Ihnen die Verwaltung von Benutzerzugriffen auf Azure-Ressourcen. | Ja | 
VM-Administratoranmeldung | Anzeigen von virtuellen Computern im Portal und Anmelden als Administrator | Ja | 
Mitwirkender von virtuellen Computern | Ermöglicht Ihnen das Verwalten virtueller Computer, aber weder den Zugriff darauf, noch auf deren verbundenen virtuellen Netzwerke oder Speicherkonten. | Ja | 
VM-Benutzeranmeldung | Anzeigen von virtuellen Computern im Portal und Anmelden als regulärer Benutzer. | Ja | 
Mitwirkender von Webplan | Ermöglicht Ihnen das Verwalten der Webpläne für Websites, nicht aber den Zugriff darauf. | Ja | 
Mitwirkender von Website | Ermöglicht Ihnen das Verwalten von Websites (nicht webplänen), aber nicht den Zugriff darauf. | Ja |
