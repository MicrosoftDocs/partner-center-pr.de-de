---
title: Übertragen von Azure-Abonnements auf einen anderen Partner
ms.topic: article
ms.date: 04/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Kunden dabei helfen, den CSP-Programmpartner zu ändern, der den Azure-Abonnements dieses Kunden zugeordnet ist.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: LauraBrenner
ms.author: labrenne
keywords: Azure-Abonnement, Partner wechseln, Partner ändern, neue Partner, andere Partner
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 01316ceebcd2f969c89b4160bf5d95dcc44b1366
ms.sourcegitcommit: 46b86ac7467afa43bedb0943dc8dc45a69caf1dd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2020
ms.locfileid: "83194395"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Erfahren Sie, wie Sie die Azure-Abonnements eines Kunden auf einen anderen Partner übertragen.

**Zielgruppe**

- Partner Center für Microsoft Cloud for US Government
- Partner Center für Microsoft Global Cloud
- Partner im CSP-Programm (Cloud Solution Provider)

In diesem Artikel wird beschrieben, wie ein Kunde seine Microsoft Azure Dienste von einem Cloud Solution Provider (CSP) zu einem anderen wechseln kann.

Führen Sie die folgenden manuellen Schritte aus, um die Azure-Dienste oder-Abonnements eines Kunden zu einem anderen Partner zu wechseln. Sowohl der Partner als auch der Kunde müssen die Schritte ausführen.

>[!Note]  
>Derzeit können nur direkte oder indirekte Anbieter Abonnements übertragen.
>Sie können keine Partner für Cloud Solution Provider-Abonnements ändern, die mit den Azure-Plänen, Office 365, Enterprise Mobility Suite oder Microsoft Dynamics CRM-Abonnements verknüpft sind.

**Partner für Azure-Abonnements wechseln**

1. Um ein Azure-Abonnement auf einen neuen Partner zu übertragen, muss der Kunde den Prozess starten und sich schriftlich an seinen aktuellen registrierten Abonnementberater wenden.

   >[!Note]
   >Es liegt in der Verantwortung des aktuellen Partners, das Serviceticket zu erstellen, das den Übertragungsprozess initiiert. Microsoft kann nicht im Auftrag der Kunden oder des neuen Partner eingreifen. Der Kunde sollte planen, eng mit dem aktuellen Partner zusammenzuarbeiten, um den Übergang reibungslos zu gestalten.

2. Der Partner für das Abonnement muss die folgenden Aufgaben ausführen:

   Erstellen eines Azure-Servicetickets in Partner Center, um eine Abonnementübertragung anzufordern.

   - Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie den Kunden aus der Liste aus. Wählen Sie anschließend **Dienstverwaltung** aus. Wählen Sie im Abschnitt **Supporttickets** die Dropdownliste **Neues Ticket** aus und anschließend **Microsoft Azure**.

   - Wählen Sie im [Azure-Portal](https://portal.azure.com)die Option **neue Supportanfrage**aus.

     Wählen Sie in Schritt 1 **Abonnement Verwaltung** als Problemtyp aus, geben Sie die Abonnement-ID an, die Sie übertragen möchten, und wählen Sie **Cloud Solution Provider** als Support Plan aus.

     Wählen Sie in Schritt 2 die Option **C-minimale Auswirkung** aus, und wählen Sie **andere allgemeine Fragen** als Problemtyp aus.

     Laden Sie das [CSP-Abonnementübertragungsformular](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip) herunter.

3. Der Partner für das Abonnement: füllen Sie das [Formular für das CSP-Abonnement Transfer](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip)aus, Signieren Sie es, und senden Sie es dann an den Kunden. Sie benötigen folgende Informationen, um das Formular auszufüllen:

   - Die Kontaktinformationen und die Microsoft-ID des aktuellen Partners. Wählen Sie im Menü „Partner Center” **Kontoeinstellungen** &gt; **Organisationsprofil**, und verwenden Sie die **Microsoft-ID**, **Name der Organisation** und **Adresse**, die dort aufgeführt sind.

   - Die Microsoft-ID des Kunden. Wählen Sie im Menü „Partner Center” **Kunden**, erweitern Sie dann den Kundeneintrag, um die **Microsoft-ID** anzuzeigen.

   - Die zu übertragende Abonnement-ID. Wählen Sie in der erweiterten Kundenliste **Abonnements anzeigen** aus. Erweitern Sie das ausgewählte Abonnement, um die **Abonnement-ID** anzuzeigen.

   >[!Note]
   >Das übertragen eines Abonnements führt zu zwei Abonnement-IDs, die auf der Seite **Abonnement bearbeiten** des übertragenen Abonnements angezeigt werden: **1**: die Partner Center-Abonnement-ID wird für Abrechnungszwecke verwendet. **2** – die ursprüngliche Azure-Abonnement-ID bleibt erhalten und wird im Partner Center genau wie im Azure-Verwaltungsportal angezeigt. Diese ID wird in der Abstimmungsdatei angezeigt.  **Bei der Anmeldung von Supportanfragen müssen Sie beide IDs verwenden.**

4. Der Kunde und der neue CSP-Partner für das Abonnement:

   Überprüfen Sie das Formular, geben Sie Daten zum neuen Partner ein, und signieren Sie es. Überprüfen Sie, ob der neue Kunde über einen Vertrag verfügt. Senden Sie das Formular an den aktuellen eingetragenen Partner zurück.

   *Wichtig*: Wenn der neue CSP-Partner keine Handels Partner Beziehung mit dem Kunden hat, müssen Sie einen erstellen, bevor das Abonnement übertragen wird. [Informationen hierzu finden Sie hier](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Der neue CSP-Partner und der Mandant des Kunden müssen sich im selben Land befinden. 

5. Aktueller Partner:

   Stellen Sie sicher, dass das Formular Kontaktinformationen für beide Partner Administratoren enthält. Microsoft-Support werden beide Administratoren kontaktiert, um die Übertragung zu überprüfen. Stellen Sie sicher, dass alle drei Signaturen vorhanden sind. Verwenden Sie dann die Option zum **Hochladen von Dateien** , um das abgeschlossene Formular an den vorhandenen Service Request anzufügen. Ein Microsoft-Supportmitarbeiter wird innerhalb von acht Geschäftszeiten zurückkehren, um den Empfang und den Abschluss zu überprüfen.

6. Neuer Partner:

   Aktualisieren Sie die Einstellungen des Azure-Abonnements, um den alten Partner aus dem Konto zu entfernen. Führen Sie zwei PowerShell-Commandlets aus, um anzuzeigen, welche Rollenzuweisungen bereitgestellt werden.

   - Hinzufügen des neuen Partners als Vertriebspartner für das Konto:

     ```powershell
     Add-AzureRMAccount -tenant "CustomerDomainName"
     ```

     So finden Sie den Namen der Domäne des Kunden: Wählen Sie im Partner Center-Menü **Kunden** aus. Wählen Sie den Kunden aus der Kundenliste aus. Wählen Sie im Menü „Kunden” **Konto**, und verwenden Sie den **Domänennamen**.

   - Anzeigen der Rollen für das Konto, einschließlich des vorherigen CSP-Partners:

     ```powershell
     Get-AzureRMRoleAssignment
     ```

7. Entfernen veralteter Zugriffsberechtigungen

   - Wählen Sie im Menü „Partner Center” **Kunden**.
   - Erweitern Sie den Kundeneintrag und wählen Sie **Abonnements anzeigen**.
   - Wählen Sie im Menü „Kunden” **Service management**.
   - Unter **Microsoft Azure** klicken Sie auf den Link, um zum **Microsoft Azure-Verwaltungsportal** zu wechseln.
