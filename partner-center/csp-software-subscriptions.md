---
title: Verkaufen von Softwareabonnements über CSP | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how partners in the CSP program can use Partner Center to buy, manage, sell, and cancel Azure reserved instances and Server subscriptions for customers.
author: MaggiePucciEvans
ms.author: evansma
keywords: Cloud Solution Provider, CSP, cloudbasierte Dienste, Azure, Azure RI, Windows Server, SQL Server, Softwareabonnements
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 32efdc721bd9a81ff04527ca82e5e71c1fe7cb58
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253550"
---
# <a name="sell-software-subscriptions-through-csp"></a>Verkaufen von Softwareabonnements über CSP

With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads. 

You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure Portal by taking advantage of the Azure Hybrid Benefit. 

Der Azure-Hybridvorteil hilft Ihnen, mehr Nutzen aus Ihren Windows Server-Lizenzen zu ziehen und bei virtuellen Computern bis zu 40 % zu sparen. Sie können mit Windows Server Datacenter und Standard Edition-Lizenzen mit Software Assurance in den Genuss des Vorteils kommen. Je nach Edition können Sie Ihre Lizenzen zum Ausführen von Windows Server-VMs in Azure konvertieren oder erneut verwenden und einen niedrigeren Computetarif (z.B. Tarife für Linux-VMs) zahlen.

> [!NOTE]  
> Azure-Reservierungen sind in den folgenden Märkten nicht verfügbar:  
> * Argentinien
> * Brasilien
> * China
> * Indonesien
> * Liechtenstein
> * Jersey
> * Malaysia
> * Mexiko
> * Russische Föderation
> * Saudi-Arabien
> * Südafrika
> * Türkei

<!--March 20, 2019 - this list of countries was correct as of today. Maggie last updated the list according to FAREAST\v-pubobb in bug 20907186.
-->

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Kaufen von Softwareabonnements im Auftrag von Kunden

Um Softwareabonnements im Auftrag eines Kunden zu erwerben, wechseln Sie zur Detailseite des Kunden. Wählen Sie **Produkte hinzufügen** aus, und befolgen Sie dann die Bildschirmanweisungen, um die Bestellung zu erstellen und zu bezahlen. Alle kommerziellen Preise verstehen sich ohne Steuern mit Ausnahme von Australien und Brasilien. Für Australien und Brasilien sind Steuern im Preis inbegriffen.

## <a name="activate-and-manage-software-subscriptions"></a>Aktivieren und Verwalten von Softwareabonnements

Nachdem Sie das Softwareabonnement erworben haben, führen Sie die folgenden Schritte aus, um es herunterzuladen.

>[!NOTE]
>Sie müssen ein Administrator-Agent sein, um Software herunterladen und Aktivierungsschlüssel abrufen zu können.

1. Wechseln Sie zur Detailseite des Kunden, und wählen Sie dann **Software** aus. You'll see a list of all the software you've purchased on behalf of the customer. 
2.  Erweitern Sie das Produkt, das Sie herunterladen möchten. Wählen Sie im Feld **Produkt auswählen** die **Version**, **Sprache** sowie **Dateityp/Betriebssystem** aus. 
3.  Klicken Sie auf **Senden**, um die spezifischen Produkte anzuzeigen. 
4.  Wählen Sie **Schlüssel und Downloads abrufen**. 
5.  Klicken Sie auf **Herunterladen**, um den Download zu starten, oder **Link kopieren**, um den Link zu kopieren und an den Kunden zu senden. 

>[!NOTE]
>Dieser Link läuft nach zwei Wochen bzw. 50 Downloads ab, je nachdem, was zuerst eintritt. Kehren Sie nach Ablauf des Links zu dieser Seite zurück, und wählen Sie erneut **Schlüssel und Downloads abrufen** aus, um ihn für weitere zwei Wochen oder 50 Downloads zu aktivieren. Sie können dies beliebig oft tun. 

## <a name="view-activity-for-software-key-access-and-software-downloads"></a>View activity for software key access and software downloads
For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software. Use the procedure below to access this information. 

>[!NOTE]
>You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs. 

1.  In Partner Center, select the gear icon from the upper right corner. 
2.  In the menu, select **Activity log**.
3.  Enter the date range for the activity you want to see. The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified. 

## <a name="cancel-a-purchase"></a>Stornieren eines Einkaufs

Sie können einen Softwarekauf binnen 60 Tagen nach Kaufdatum stornieren. Microsoft erhebt keine Gebühr bei vorzeitiger Kündigung, jedoch können Sie einen Kauf nicht nach Ablauf von 60 Tagen ab Kaufdatum stornieren.

Nachdem Sie den Kauf storniert haben, wird der Softwareschlüssel widerrufen. 

Gehen Sie folgendermaßen vor, um einen Kauf zu stornieren:

>[!NOTE]
>Sie müssen ein Administrator-Agent sein, um einen Kauf zu stornieren. 

1.  Bevor Sie beginnen, sollten Sie sicherstellen, dass Sie über Folgendes verfügen:
    -   Mandanten-GUID oder Domänenname des Kunden
    -   Auftrags- oder Abonnement-ID
    -   Grund für Rückerstattung
    -   Angeforderter Betrag

2.  On the customer's details page, select **Software** to see the list of all the software you've purchased for the customer. 

3.  Suchen Sie die Software, die Sie stornieren möchten, und wählen Sie dann **Abbrechen** aus. Die Seite **Melden eines Problems mit Partner Center** wird geöffnet. 

4.  Wählen Sie unter **Details** in der Liste **Art des Problems** die Option **CSP-Kauf/Rückerstattung im Auftrag der Kunden** aus.

5.  Füllen Sie die Felder **Auswirkungen** und **Titel** aus. 

6.  Geben Sie im Feld **Beschreibung** Folgendes ein: 
    -   Mandanten-GUID oder Domänenname des Kunden
    -   Auftrags- oder Abonnement-ID
    -   Grund für Rückerstattung
    -   Angeforderter Betrag

7.  Geben Sie im Feld **Kontakt** Ihren Namen, Ihre E-Mail-Adresse und Telefonnummer ein. 

8.  Wenn Sie aus einem beliebigen Grund eine Datei anfügen möchten, wählen Sie **Dateien hinzufügen** aus. Dieser Schritt ist optional. 

9.  When you're finished, select **Submit**.
