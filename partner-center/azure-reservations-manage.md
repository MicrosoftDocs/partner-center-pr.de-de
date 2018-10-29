---
title: Azure Reservations im Auftrag Ihrer Kunden verwalten | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
ms.author: v-petand
keywords: Azure, Reservierungen, verwalten, Abrechnung, kaufen
ms.localizationpriority: medium
ms.openlocfilehash: 20286d269a3074f89ca1368c26992feb03f9d182
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795453"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Microsoft Azure Reservations im Auftrag Ihrer Kunden verwalten | Partner Center

**Betriff:**

-  Partner Center
-  Microsoft Azure-Portal
-  CSP-Partner

Zum Verwalten Ihrer Kunden Azure Reservations nach dem Kauf Sie wählen Sie den Kunden und die Reservierung, die Sie im Partner Center verwalten möchten, und nehmen Sie Änderungen dann die Reservierung im Azure-Portal. 

1. Um zu beginnen, wählen Sie **Kunden** aus Ihrem Partner Center-Menü, und wählen Sie dann den Kunden, deren Reservierungen Sie verwalten möchten. 

2. Der Kunde Detail Seite Menü Wählen Sie **Azure Reservations** , und wählen Sie dann die spezifische Reservierung, die Sie verwalten möchten.  

3. Klicken Sie unter **Aktionen**auf **verwalten** und wechseln Sie zur Kunden-Reservierung im Azure-Portal. Führen Sie auf der Seite der Reservierungsdetails die unten beschriebenen Schrittezum Abschließen der Aufgaben durch.  

| **Wählen Sie**   | **Zweck**    |
|:-----------------------------|:-----------------|
| **Übersicht**   | Hier werden Details des Kundenreservierung angezeigt, einschließlich Ablaufdatum, Bereich und Nutzungsdaten **Hinweis:** Wählen Sie **Rückerstattung** aus, um eine Supportanfrage für eine Rückerstattung zu erstellen. Wählen Sie **Exchange**, um eine Supportanfrage zu erstellen, um nicht verwendete Teile der Reservierung auszutauschen.  
| **Zugriffssteuerung (IAM)**   | Verwalten des Zugriffs auf die Informationen der Kundenreservierung.|
| **Konfiguration**   | Ändern Sie den Reservierungsbereich bzw. das Azure-Abonnement, dem die Reservierung zugeordnet ist.    |
| **Eigenschaften**   | Zeigen Sie Eigenschaften für die Reservierung an und kopieren Sie die Reservierungs-ID und die Reservierungsbestellungs-ID in die Zwischenablage. **Hinweis:** Support fordert möglicherweise die Reservierungs-ID und die Reservierungsauftrags-ID an, wenn Sie im Auftrag eines Kunden Support anfordern.    |
| **Neue Supportanfrage**    | Support von Microsoft-Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Stornieren oder austauschen der Reservierung 
Wenn die geschäftliche Anforderung Ihrer Kunden sich ändert, können Sie die Reservierung stornieren oder einen anteiligen Erstattungsbetrag des Preises für eine neue Reservierung verwenden. 

**Funktionsweise von Stornierungen**

Kunden können Sie die Reservierung (bis zu 50.000 USD pro Jahr) jederzeit abbrechen. Durch eine Kündigung kann der Kunde die verbleibenden Monate der Azure-Reservierung an Microsoft für eine Gebühr der vorzeitigen Kündigung zurückzugeben. Der anteilige Restbetrag, abzüglich der Gebühr, wird dem Originalkauf des Kunden erstattet. 

Nachfolgend finden Sie Abbruch Details und Gebühren.

|**Kündigungsdatum**<br> (in Tagen)   |**Verwendungszweck**    |**Erstattung**  |**Vorzeitige Beendigung**<br> gebühr    |**Rückerstattung Obergrenze** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|Weniger als 5                       | Nein          | 100%       | Nein                              | 50.000 US-DOLLAR   |
|Weniger als 5                       | Ja         | Anteilsmäßigen  | Nein                              | 50.000 US-DOLLAR   |
|Mehr als 5                        | Nein          | Anteilsmäßigen  | 12 %                             | 50.000 US-DOLLAR   |
|Mehr als 5                        | Ja         | Anteilsmäßigen  | 12 %                             | 50.000 US-DOLLAR   |


**Funktionsweise des Austauschs** 

Ein Austausch ermöglicht dem Kunden, die anteilige Erstattung basierend auf der verbleibenden Dauer der Reservierung zu erhalten und eine neue Reservierung mit dem Rückerstattungsbetrag einzugehen.   

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Fordern Sie eine Rückerstattung oder einen Austausch im Auftrag eines Kunden an 

Um eine Supportanfrage für eine Rückerstattung oder einen Austausch im Auftrag Ihrer Kunden anzufordern, Sie wählen Sie den Kunden und die Reservierung im Partner Center, und klicken Sie dann die Supportanfrage im Azure-Portal erstellen. 

>[!NOTE]
>Microsoft-Support-Agents können Sie nach der Reservierungs-ID und der Reservierungsbestellungs-ID fragen. Sie finden diese Informationen auf der Reservierungsseite unter **Eigenschaften** im Azure-Portal. 

1. Um zu beginnen, wählen Sie **Kunden** aus dem Menü "Partner Center", und wählen Sie dann den Kunden, der eine Rückerstattung möchte. 

2. Wählen Sie auf der Detailseite des Kunden **Azure Reservations**, und wählen Sie die spezifische Reservierung, die der Kunde zurückerstattet haben möchte.  

3. Wählen Sie unter **Aktionen**, um die Kunden-Reservierung im Azure-Portal aufzurufen und initiieren Sie eine Supportanfrage **eine Rückerstattung anfordern** .  

4. Auf der Seite **neue Supportanfrage**, führen Sie die folgenden Schritteaus, um eine Rückerstattung anzufordern. Wählen Sie **Weiter** nach jedem Schritt. 

|**Schritt**   |**Auswahl**    |
|:-----------------------------|:-----------------|
|**1 Grundlagen**   |Problemtyp: Abrechnung.  |
|**2 Problem**   |Problemtyp: Reservierungsverwaltung. Kategorie: Austausch und Rückerstattungen. |
|**3 Kontaktinformationen**   |Wählen Sie Ihre Einstellungen, und geben Sie die erforderlichen Informationen an. Wählen Sie abschließend **Erstellen** aus.   |

## <a name="azure-reservations-resources"></a>Azure Reservations-Ressourcen
|**Weitere Informationen**   |**Bitte lesen**    |
|:-----------------------------|:-----------------|
|Azure Reservations in CSP (Übersicht)  | [Verkaufen Microsoft Azure Reserved Instances](azure-reservations.md) |
|Erwerb von Azure Reservations für Ihre Kunden im Partner Center   |[Azure Reservations kaufen](azure-reservations-buying.md) |
|Bestimmen Sie die richtige Größe für den virtuellen Computer, und überprüfen Sie die Kunden VM-Nutzung   |[VM-Größe für die maximale Azure Reservations-Nutzung](azure-usage.md)   |
|Erwerb von Azure Reservations über die Partner Center-API | [Erwerben Sie Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in die Partner Center-Entwicklerdokumentation

