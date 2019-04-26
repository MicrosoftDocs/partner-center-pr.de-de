---
title: Übertragen von Azure-Abonnements | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Kunden können den Partner im Programm für Cloud-Lösungsanbieter ändern, den sie für Microsoft Azure-Dienste verwenden möchten. Dies ist jedoch ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.author: evansma
keywords: Azure-Abonnement, Partner wechseln, Partner ändern, neue Partner, andere Partner
ms.localizationpriority: medium
ms.openlocfilehash: 2298763cd01ebc2f1b3849db27363b0a39eb78bf
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133857"
---
# <a name="transfer-azure-subscriptions"></a>Azure-Abonnements übertragen 

**Gilt für**

-  Partner Center

Kunden können den Cloud Solution Provider-Partner oder einen anderen Partner für Microsoft Azure-Dienste ändern. Dies ist jedoch ein manueller Vorgang, der Aktionen von Partnern und Kunden erfordert.

>[!Note]  
>Zu diesem Zeitpunkt sind nur direkte oder indirekte Anbieter können Abonnements übertragen.
>Es ist zurzeit nicht möglich, Partner für Cloud-Lösungsanbieter-Abonnements für Office 365, Enterprise Mobility Suite oder Microsoft Dynamics CRM-Abonnements zu ändern.



**Switch-Partnern für Azure-Abonnements**

1. Um ein Azure-Abonnement auf einen neuen Partner zu übertragen, muss der Kunde den Prozess starten und sich schriftlich an seinen aktuellen registrierten Abonnementberater wenden. 
>[!Note]
>Es liegt in der Verantwortung des aktuellen Partners, das Serviceticket zu erstellen, das den Übertragungsprozess initiiert. Microsoft kann nicht im Auftrag der Kunden oder des neuen Partner eingreifen. Der Kunde sollte planen, eng mit dem aktuellen Partner zusammenzuarbeiten, um den Übergang reibungslos zu gestalten.

2. Der Partner für das Abonnement muss folgende Schritte ausführen:

Erstellen eines Azure-Servicetickets in Partner Center, um eine Abonnementübertragung anzufordern.
-   Wählen Sie im Partner Center-Menü **Kunden**, wählen Sie Ihren Kunden aus der Liste aus, und wählen Sie dann **Dienstverwaltung**. Wählen Sie im Abschnitt **Supporttickets** die Dropdownliste **Neues Ticket** aus und anschließend **Microsoft Azure**.

-   Wählen Sie im Azure-Portal **Neue Supportanfrage** aus.

Wählen Sie in Schritt 1 **Abonnementverwaltung** als Art des Problems aus, geben Sie die ID des Abonnements ein, das Sie übertragen möchten, und wählen Sie **Cloud-Lösungsanbieter** als Supportplan aus.

Wählen Sie in Schritt 2 **C – Minimale Auswirkungen** und anschließend als Problemtyp **Andere allgemeine Fragen** aus.

Laden Sie das [Formular für Übertragungen von CSP-Abonnements](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip) herunter.

3. Der Partner für das Abonnement: Geben Sie die [CSP-abonnementübertragungsformular](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), melden Sie sich, und klicken Sie dann an den Kunden senden. Sie benötigen folgende Informationen, um das Formular auszufüllen:

- Die Kontaktinformationen und die Microsoft-ID des aktuellen Partners. Wählen Sie im Partner Center-Menü **Kontoeinstellungen** &gt; **Organisationsprofil**, und verwenden Sie die **Microsoft-ID**, **Organisationsname** , und **Adresse** aufgeführt.

- Die Microsoft-ID des Kunden. Wählen Sie im Menü „Partner Center” **Kunden**, erweitern Sie dann den Kundeneintrag, um die **Microsoft-ID** anzuzeigen.

- Die zu übertragende Abonnement-ID. Wählen Sie in der erweiterten Kundenliste **Abonnements anzeigen** aus. Erweitern Sie das ausgewählte Abonnement, um die **Abonnement-ID** anzuzeigen.

>[!Note]
>Übertragen eines Abonnements führt zu zwei-Abonnement-IDs, die in angezeigt werden, die **Abonnement bearbeiten** übertragen Abonnements auf der Seite: **1**: der Partner Center-Abonnement-ID wird für Abrechnungszwecke verwendet. 
**2**- die ursprüngliche Azure-Abonnement-ID bleibt erhalten und wird im Partner Center genau wie im Azure-Verwaltungsportal angezeigt. Diese ID wird in der Abstimmungsdatei angezeigt.  **Beim Protokollieren von supporttickets, müssen Sie beide IDs verwenden.**

4. Der Kunde und der neue CSP-Partner für das Abonnement:

Überprüfen Sie das Formular, geben Sie Daten zum neuen Partner ein, und signieren Sie es. Überprüfen Sie, ob der neue Kunde über einen Vertrag verfügt. Senden Sie das Formular an den aktuellen eingetragenen Partner zurück.

*Wichtig*: Wenn der neue CSP-Partner keine vertriebspartnerbeziehung mit dem Kunden, müssen sie vor dem Abonnement übertragen einrichten. [Informationen hierzu finden Sie hier](request-a-relationship-with-a-customer.md).

>[!Note]
>Der neue CSP-Partner und Mandanten des Kunden müssen im gleichen Land befinden. 

5. Aktueller Partner:

Stellen Sie sicher, dass das Formular Kontaktinformationen für die Administratoren beider Partner enthält. Microsoft Support wird sich an beide Administratoren wenden, um die Übertragung zu verifizieren. Stellen Sie sicher, dass alle drei Unterschriften vorhanden sind, und fügen Sie dann das ausgefüllte Formular über die Option **Dateiupload** der vorhandenen Serviceanfrage hinzu. Ein Microsoft Support-Mitarbeiter wird innerhalb von 8 Geschäftsstunden Kontakt mit Ihnen aufnehmen, um Erhalt und Abschluss zu bestätigen.

6. Neuer Partner:

Aktualisieren Sie die Einstellungen des Azure-Abonnements, um den alten Partner aus dem Konto zu entfernen. Um anzuzeigen, welche Rollenzuweisungen bereitgestellt wurden, führen Sie zwei PowerShell-Commandlets aus.

-   Hinzufügen des neuen Partners als Vertriebspartner für das Konto:

**PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

So finden Sie den Namen der Domäne des Kunden: Wählen Sie im Partner Center-Menü **Kunden** aus. Wählen Sie den Kunden aus der Kundenliste aus. Wählen Sie im Menü „Kunden” **Konto**, und verwenden Sie den **Domänennamen**.

-   Anzeigen der Rollen für das Konto, einschließlich des vorherigen CSP-Partners:

**PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Entfernen veralteter Zugriffsberechtigungen

-  Wählen Sie im Menü „Partner Center” **Kunden**. 
-  Erweitern Sie den Kundeneintrag und wählen Sie **Abonnements anzeigen**. 
-  Wählen Sie im Menü „Kunden” **Service management**. 
-  Unter **Microsoft Azure** klicken Sie auf den Link, um zum **Microsoft Azure-Verwaltungsportal** zu wechseln.

 

 



