---
title: Übertragen von Azure-Abonnements | Partner Center
description: Kunden können den Partner im Programm für Cloud Solution Provider ändern, den sie für Microsoft Azure-Dienste verwenden möchten. Dies ist jedoch ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
keywords: Azure-Abonnement, Partner wechseln, Partner ändern, neue Partner, andere Partner
ms.openlocfilehash: a4b9c0a320808f1d8a4a630a035660813a3f9c74
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2018
ms.locfileid: "2088957"
---
# <a name="transfer-azure-subscriptions"></a>Übertragen von Azure-Abonnements 

**Betrifft**

-  Partner Center

Kunden können den Cloud Solution Provider-Partner oder einen anderen Partner für Microsoft Azure-Dienste ändern. Dies ist jedoch ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert.

**Hinweis** Es ist zurzeit nicht möglich, Partner für Cloud Solution Provider-Abonnements für Office 365, Enterprise Mobility Suite oder Microsoft Dynamics CRM-Abonnements zu ändern.



**Partner für Azure-Abonnements wechseln**

1.  Um ein Azure-Abonnement auf einen neuen Partner zu übertragen, muss der Kunde den Prozess starten und sich schriftlich an seinen aktuellen registrierten Abonnementberater wenden. 

    >**Hinweis:**<br> Es liegt in der Verantwortung des aktuellen Partners, das Serviceticket zu erstellen, das den Übertragungsprozess initiiert. Microsoft kann nicht im Auftrag der Kunden oder des neuen Partner eingreifen. Der Kunde sollte planen, eng mit dem aktuellen Partner zusammenzuarbeiten, um den Übergang reibungslos zu gestalten.

2.  Der Partner für das Abonnement muss folgende Schritte ausführen:

    Erstellen eines Azure-Servicetickets in Partner Center, um eine Abonnementübertragung anzufordern.

    -   Wählen Sie vom Menü „Dashboard“ die Option **Kunden** aus, und wählen Sie den Kunden aus der Liste aus. Wählen Sie anschließend **Dienstverwaltung** aus. Wählen Sie im Abschnitt **Supporttickets** die Dropdownliste **Neues Ticket** aus und anschließend **Microsoft Azure**.

    -   Wählen Sie im Azure-Portal **Neue Supportanfrage** aus.

        Wählen Sie in Schritt 1 **Abonnementverwaltung** als Art des Problems aus, geben Sie die ID des Abonnements ein, das Sie übertragen möchten, und wählen Sie **Cloud Solution Provider** als Supportplan aus.

        Wählen Sie in Schritt2 **C – Minimale Auswirkungen** und anschließend als Problemtyp **Andere allgemeine Fragen** aus.

        Laden Sie das [Formular für Übertragungen von CSP-Abonnements](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip) herunter.

3.  Der Partner für das Abonnement: Füllen Sie das [Formular zur Übertragung des CSP-Abonnements](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip) aus, signieren Sie es, und senden Sie es dann an den Kunden. Sie benötigen folgende Informationen, um das Formular auszufüllen:

    -   Die Kontaktinformationen und die Microsoft-ID des aktuellen Partners. Wählen Sie im Partner Center-Menü **Kontoeinstellungen** &gt; **Organisationsprofil** aus, und verwenden Sie die **Microsoft-ID**, den **Organisationsnamen** und die **Adresse**, die hier aufgeführt werden.

    -   Die Microsoft-ID des Kunden. Wählen Sie im Menü „Partner Center” **Kunden**, erweitern Sie dann den Kundeneintrag, um die **Microsoft-ID** anzuzeigen.

    -   Die zu übertragende Abonnement-ID. Wählen Sie in der erweiterten Kundenliste **Abonnements anzeigen** aus. Erweitern Sie das ausgewählte Abonnement, um die **Abonnement-ID** anzuzeigen.

    >**Hinweis:**<br> Das Übertragen eines Abonnements führt zu zwei Abonnement-IDs, die auf der Seite **Anmeldung bearbeiten** des übertragenen Abonnements angezeigt werden: **1**- die Partner Center-Abonnement-ID dient zu Abrechnungszwecken. 
    **2**- Die ursprüngliche Azure-Abonnement-ID bleibt erhalten und wird im Partner Center genau wie im Azure-Verwaltungsportal angezeigt. Diese ID wird in der Abstimmungsdatei angezeigt.  **Bei der Anmeldung von Supportanfragen müssen Sie beide IDs verwenden.**

4.  Der Kunde und der neue CSP-Partner für das Abonnement:

    Überprüfen Sie das Formular, geben Sie Daten zum neuen Partner ein, und signieren Sie es. Überprüfen Sie, ob der neue Kunde über einen Vertrag verfügt. Senden Sie das Formular an den aktuellen eingetragenen Partner zurück.

    *Wichtig*: Wenn der neue CSP-Partner keine Vertriebspartnerbeziehung mit dem Kunden hat, muss diese vor der Übertragung des Abonnements eingerichtet werden. [Informationen hierzu finden Sie hier](request-a-relationship-with-a-customer.md).

5.  Aktueller Partner:

    Stellen Sie sicher, dass das Formular Kontaktinformationen für die Administratoren beider Partner enthält. Microsoft-Support wird sich an beide Administratoren wenden, um die Übertragung zu verifizieren. Stellen Sie sicher, dass alle drei Unterschriften vorhanden sind, und fügen Sie dann das ausgefüllte Formular über die Option **Dateiupload** der vorhandenen Serviceanfrage hinzu. Ein Microsoft-Support-Mitarbeiter wird Sie innerhalb von acht Geschäftsstunden kontaktieren, um den Erhalt und den Abschluss zu bestätigen.

6.  Neuer Partner:

    Aktualisieren Sie die Einstellungen des Azure-Abonnements, um den alten Partner aus dem Konto zu entfernen. Um anzuzeigen, welche Rollenzuweisungen bereitgestellt wurden, führen Sie zwei PowerShell-Commandlets aus.

    -   Hinzufügen des neuen Partners als Vertriebspartner für das Konto:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        So finden Sie den Namen der Domäne des Kunden: Wählen Sie im Partner Center-Menü **Kunden** aus. Wählen Sie den Kunden aus der Kundenliste aus. Wählen Sie im Menü „Kunden” **Konto**, und verwenden Sie den **Domänennamen**.

    -   Anzeigen der Rollen für das Konto, einschließlich des vorherigen CSP-Partners:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Entfernen veralteter Zugriffsberechtigungen

    -  Wählen Sie **Kunden** im Partner Center-Menü. 
    -  Erweitern Sie den Kundeneintrag und wählen Sie **Abonnements anzeigen**. 
    -  Wählen Sie im Menü „Kunden” **Service management**. 
    -  Unter **Microsoft Azure** klicken Sie auf den Link, um zum **Microsoft Azure-Verwaltungsportal** zu wechseln.

 

 



