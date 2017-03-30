---
title: "Übertragen von Azure-Abonnements auf einen anderen Partner | Partner Center"
description: "Kunden können den Partner im Programm für Cloud-Lösungsanbieter ändern, den sie für Microsoft Azure-Dienste verwenden möchten. Dies ist jedoch ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert."
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.openlocfilehash: ec227dac6f8b0625120bf4b5d1bc76fbeaaae635
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="switch-azure-subscriptions-to-a-different-partner"></a>Übertragen von Azure-Abonnements auf einen anderen Partner

**Betrifft**

-  Partner Center

Kunden können den Partner im Programm für Cloud-Lösungsanbieter ändern, den sie für Microsoft Azure-Dienste verwenden möchten. Dies ist jedoch ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert.

**Hinweis** Zurzeit gibt es keinen automatischen Vorgang, über den Azure-Kunden von EA, Open oder anderen Lizenzierungsprogrammen zu CSP wechseln können. Dies ist ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert. Darüber hinaus ist es zurzeit nicht möglich, für Office365-, Enterprise Mobility Suite- oder Microsoft Dynamics CRM-Abonnements den Partner im Programm für Cloud-Lösungsanbieter zu ändern.

 

**Partner für Azure-Abonnements wechseln**

1.  Um ein Azure-Abonnement auf einen neuen Partner zu übertragen, muss der Kunde den Vorgang starten und sich schriftlich an den aktuellen eingetragenen CSP-Partner wenden.

2.  Der CSP-Partner für das Abonnement muss folgende Schritte ausführen:

    Erstellen eines Azure-Servicetickets in Partner Center, um eine Abonnementübertragung anzufordern.

    -   Wählen Sie in Partner Center im Menü „Dashboard“ die Option **Kunden** aus, und wählen Sie den Kunden aus der Liste aus. Wählen Sie anschließend **Dienstverwaltung** aus. Wählen Sie im Abschnitt **Supporttickets** die Dropdownliste **Neues Ticket** aus und anschließend **Microsoft Azure**.

    -   Wählen Sie im Azure-Portal **Neue Supportanfrage** aus.

        Wählen Sie in Schritt 1 **Abonnementverwaltung** als Art des Problems aus, geben Sie die ID des Abonnements ein, das Sie übertragen möchten, und wählen Sie **Cloud-Lösungsanbieter** als Supportplan aus.

        Wählen Sie in Schritt2 **C – Minimale Auswirkungen** und anschließend als Problemtyp **Andere allgemeine Fragen** aus.

        Laden Sie das [Formular für Übertragungen von CSP-Abonnements](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip) herunter.

3.  Aktueller CSP-Partner für das Abonnement: Füllen Sie das [Formular zur Übertragung des CSP-Abonnements](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip) aus, signieren Sie es, und senden Sie es dann an den Kunden. Sie benötigen folgende Informationen, um das Formular auszufüllen:

    -   Die Kontaktinformationen und die Microsoft-ID des aktuellen Partners. Wählen Sie im Partner Center-Menü **Kontoeinstellungen** &gt; **Organisationsprofil** aus, und verwenden Sie die **Microsoft-ID**, den **Organisationsnamen** und die **Adresse**, die hier aufgeführt werden.

    -   Die Microsoft-ID des Kunden. Wählen Sie im Menü „Partner Center” **Kunden**, erweitern Sie dann den Kundeneintrag, um die **Microsoft-ID** anzuzeigen.

    -   Die zu übertragende Abonnement-ID. Wählen Sie in der erweiterten Kundenliste **Abonnements anzeigen** aus. Erweitern Sie das ausgewählte Abonnement, um die **Abonnement-ID** anzuzeigen.

4.  Kunde und neuer CSP-Partner für das Abonnement:

    Überprüfen Sie das Formular, geben Sie Daten zum neuen Partner ein, und signieren Sie es. Überprüfen Sie, ob der neue Kunde über einen Vertrag verfügt. Senden Sie das Formular an den aktuellen eingetragenen Partner zurück.

    *Wichtig*: Wenn der neue CSP-Partner keine Vertriebspartnerbeziehung mit dem Kunden hat, muss diese vor der Übertragung des Abonnements eingerichtet werden. [Informationen hierzu finden Sie hier](https://int.msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

5.  Aktueller CSP-Partner:

    Stellen Sie sicher, dass das Formular Kontaktinformationen für die Administratoren beider Partner enthält. Microsoft Support wird sich an beide Administratoren wenden, um die Übertragung zu verifizieren. Stellen Sie sicher, dass alle drei Unterschriften vorhanden sind, und fügen Sie dann das ausgefüllte Formular über die Option **Dateiupload** der vorhandenen Serviceanfrage hinzu. Ein Microsoft Support-Mitarbeiter wird innerhalb von 8Geschäftsstunden Kontakt mit Ihnen aufnehmen, um Erhalt und Abschluss zu bestätigen.

6.  Neuer CSP-Partner:

    Aktualisieren Sie die Einstellungen des Azure-Abonnements, um den alten Partner aus dem Konto zu entfernen. Um anzuzeigen, welche Rollenzuweisungen bereitgestellt wurden, führen Sie zwei PowerShell-Commandlets aus.

    -   Hinzufügen des neuen Partners als Vertriebspartner für das Konto:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        So finden Sie den Namen der Domäne des Kunden: Wählen Sie im Partner Center-Menü **Kunden** aus. Wählen Sie den Kunden aus der Kundenliste aus. Wählen Sie im Menü „Kunden” **Konto**, und verwenden Sie den **Domänennamen**.

    -   Anzeigen der Rollen für das Konto, einschließlich des vorherigen CSP-Partners:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

    Entfernen Sie veraltete Berechtigungen für das Abonnement und Ressourcen, indem Sie das Abonnement im Azure-Portal verwalten. Wählen Sie im Menü „Partner Center” **Kunden**. Erweitern Sie den Kundeneintrag und wählen Sie **Abonnements anzeigen**. Wählen Sie im Menü „Kunden” **Service management**. Unter **Microsoft Azure** klicken Sie auf den Link, um zum **Microsoft Azure-Verwaltungsportal** zu wechseln.

 

 



