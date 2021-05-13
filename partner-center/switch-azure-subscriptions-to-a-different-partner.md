---
title: Übertragen eines Azure-Abonnements an einen anderen Partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie den Cloud Solution Provider Programmpartner ändern, der den Azure-Abonnements eines Kunden zugeordnet ist.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856065"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Erfahren Sie, wie Sie die Azure-Abonnements eines Kunden auf einen anderen Partner übertragen

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Globaler Administrator

In diesem Artikel wird beschrieben, wie ein Kunde seine Microsoft Azure Dienste von einem Cloud Solution Provider (CSP) auf einen anderen umstellen kann.

Führen Sie die folgenden manuellen Schritte aus, um die Azure-Dienste oder -Abonnements eines Kunden zu einem anderen Partner zu wechseln. Sowohl der Partner als auch der Kunde müssen die Schritte ausführen.

>[!Note]  
>Derzeit können nur direkte oder indirekte Anbieter Abonnements übertragen.
>Partner für Cloud Solution Provider Abonnements, die Azure-Plänen, Office 365-, Enterprise Mobility Suite- oder Microsoft Dynamics CRM-Abonnements zugeordnet sind, können nicht geändert werden.

## <a name="switch-partners-for-azure-subscriptions"></a>Partner für Azure-Abonnements wechseln

1. Um ein Azure-Abonnement auf einen neuen Partner zu übertragen, muss der Kunde den Prozess starten und sich schriftlich an seinen aktuellen registrierten Abonnementberater wenden.

   >[!Note]
   > Es liegt in der Verantwortung des aktuellen Partners, das Serviceticket zu erstellen, das den Übertragungsprozess initiiert. Microsoft kann nicht im Auftrag der Kunden oder des neuen Partner eingreifen. Der Kunde sollte planen, eng mit dem aktuellen Partner zusammenzuarbeiten, um den Übergang reibungslos zu gestalten.

2. Der Partner für das Abonnement muss die folgenden Aufgaben ausführen:

   Erstellen eines Azure-Servicetickets in Partner Center, um eine Abonnementübertragung anzufordern.

   1. Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie den Kunden aus der Liste aus. Wählen Sie anschließend **Dienstverwaltung** aus.

   2. Wählen Sie im Abschnitt **Supporttickets** die Dropdownliste **Neues Ticket** aus und anschließend **Microsoft Azure**.
   
   3. Wählen Sie [im Azure-Portal](https://portal.azure.com)die Option **Neue Supportanfrage** aus.
   
   4. Wählen Sie in Schritt 1 **Abonnementverwaltung** als Problemtyp aus, geben Sie die Abonnement-ID an, die Übertragen werden soll, und wählen Sie **Cloud Solution Provider** als Supportplan aus.
   
   5. Wählen Sie in Schritt 2 **die Option C–Minimale Auswirkung** und dann Andere allgemeine **Fragen** als Problemtyp aus.
   
   6. Laden Sie das [CSP-Abonnementübertragungsformular](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC) herunter.

3. Der Partner für das Abonnement: Füllen Sie das [CSP-Abonnementübertragungsformular](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)aus, signieren Sie es, und senden Sie es an den Kunden. 

   Sie benötigen folgende Informationen, um das Formular auszufüllen:

   - Die Kontaktinformationen und die Microsoft-ID des aktuellen Partners. Wählen Sie im Menü „Partner Center” **Kontoeinstellungen** &gt; **Organisationsprofil**, und verwenden Sie die **Microsoft-ID**, **Name der Organisation** und **Adresse**, die dort aufgeführt sind.

   - Die Microsoft-ID des Kunden. Wählen Sie im Menü „Partner Center” **Kunden**, erweitern Sie dann den Kundeneintrag, um die **Microsoft-ID** anzuzeigen.

   - Die zu übertragende Abonnement-ID. Wählen Sie in der erweiterten Kundenliste **Abonnements anzeigen** aus. Erweitern Sie das ausgewählte Abonnement, um die **Abonnement-ID** anzuzeigen.

   >[!Note]
   >Die Übertragung eines Abonnements führt zu zwei Abonnement-IDs, die auf der Seite **Abonnement bearbeiten** des übertragenen Abonnements angezeigt werden: **1–** Die Partner Center Abonnement-ID wird zu Abrechnungszwecken verwendet. **2** – die ursprüngliche Azure-Abonnement-ID bleibt erhalten und wird im Partner Center genau wie im Azure-Verwaltungsportal angezeigt. Diese ID wird in der Abstimmungsdatei angezeigt.  **Bei der Anmeldung von Supportanfragen müssen Sie beide IDs verwenden.**

4. Der Kunde und der neue CSP-Partner für das Abonnement:

   Überprüfen Sie das Formular, geben Sie Daten zum neuen Partner ein, und signieren Sie es. Überprüfen Sie, ob der neue Kunde über einen Vertrag verfügt. Senden Sie das Formular an den aktuellen eingetragenen Partner zurück.

   *Wichtig:* Wenn der neue CSP-Partner keine Vertriebspartnerschaft mit dem Kunden hat, muss er eine Vertriebspartnerbeziehung einrichten, bevor das Abonnement übertragen wird. [Informationen hierzu finden Sie hier](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Der neue CSP-Partner und der Mandant des Kunden müssen sich im selben Land befinden. 

5. Aktueller Partner:

   Stellen Sie sicher, dass das Formular Kontaktinformationen für beide Partneradministratoren enthält. Microsoft-Support wenden sich an beide Administratoren, um die Übertragung zu überprüfen. Stellen Sie sicher, dass Sie über alle drei Signaturen verfügen. Verwenden Sie dann die **Option Dateiupload,** um das fertige Formular an Ihre vorhandene Dienstanforderung anfügen. Ein Microsoft-Supporttechniker wird innerhalb von acht Geschäftsstunden zu Ihnen zurückkommen, um Den Empfang und Abschluss zu überprüfen.

6. Neuer Partner:

   Aktualisieren Sie die Einstellungen des Azure-Abonnements, um den alten Partner aus dem Konto zu entfernen. Führen Sie zwei PowerShell-Cmdlets aus, um zu sehen, welche Rollenzuweisungen bereitgestellt werden.

   - Hinzufügen des neuen Partners als Vertriebspartner für das Konto:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > Die **Mandanten-ID des Kunden** wird im Partner Center Microsoft-ID des Kunden **angezeigt.** Um die Microsoft-ID (Mandanten-ID) für einen bestimmten Kunden zu finden, melden Sie sich beim dashboard Partner Center [an.](https://partner.microsoft.com/dashboard) Wählen Sie dann **im Menü Kunden** aus. Suchen Sie den Kunden in der Liste. Wählen Sie den Pfeil nach unten aus, um die Auflistung des Kunden zu erweitern. Es werden Informationen zum Domänennamen des Kunden *und* zur **Microsoft-ID des Kunden einsingen.** Verwenden Sie die 16-stellige **Microsoft-ID** im PowerShell-Cmdlet.

   - Anzeigen der Rollen für das Konto, einschließlich des vorherigen CSP-Partners:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Veraltete Zugriffsberechtigungen entfernen:

   - Wählen Sie im Menü „Partner Center” **Kunden**.
   - Suchen Sie den Kunden in der Liste. Wählen Sie den Firmennamen aus (doppelklicken Sie darauf). Durch diese Aktion wird die Seite **Kundenabonnements** geöffnet.
   - Wählen Sie im Detailmenü des Kunden die Option **Dienstverwaltung aus.**
   - Wählen **Microsoft Azure** den Link aus, um zum **-Microsoft Azure-Verwaltungsportal.**

## <a name="next-steps"></a>Nächste Schritte

- Laden Sie das [CSP-Abonnementübertragungsformular](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA) herunter.

- Erfahren Sie mehr [über die Unterstützung für mehrere Partner.](multipartner.md)

- [Unterstützung für mehrere Partner.](multipartner.md)
- [Unterstützung für mehrere Kanäle.](multichannel.md)
- [Übertragen von Azure-Abonnements](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)