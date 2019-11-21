---
title: Azure Reservations im Auftrag Ihrer Kunden verwalten | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie Sie Azure-Reservierungen im Auftrag eines Kunden verwalten, wie Sie eine Reservierung stornieren, eine Reservierung austauschen oder eine Rückerstattung anfordern.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, verwalten, Abrechnung, Kauf, Stornierung, Umtausch, Gebühr bei vorzeitiger Kündigung
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b71457f0bd75008db9ed704784a39b082983501d
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252638"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Verwalten von Microsoft Azure Reservations im Auftrag Ihrer Kunden       

**Gilt für**

-  Partner Center
-  Microsoft Azure-Portal 
-  CSP-Partner

Um die Azure-Reservierungen ihrer Kunden nach dem Kauf zu verwalten, wählen Sie den Kunden und die Reservierung aus, die Sie in Partner Center verwalten möchten, und nehmen dann Änderungen an der Reservierung im Azure-Portal vor. 

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, dessen Reservierungen Sie verwalten möchten. 

2. Wählen Sie im Menü Detailseite des Kunden die Option **Azure-Reservierungen** aus, und wählen Sie dann die jeweilige Reservierung aus, die Sie verwalten möchten.  

3. Wählen Sie unter **Aktionen**die Option **Verwalten** aus, um zum Reservierungsdaten Satz des Kunden in der Azure-Portal zu wechseln. Führen Sie auf der Seite der Reservierungsdetails die unten beschriebenen Schritte zum Abschließen der Aufgaben durch.  

    | **Auswahl**   | **Aktion**    |
    |:-----------------------------|:-----------------|
    | **Übersicht**   | Anzeigen von Details der Reservierung eines Kunden, einschließlich Ablaufdatum, Bereich und Verwendungs Daten. **Hinweis:** Wählen Sie **Rückerstattung** aus, um eine Supportanfrage für eine Rückerstattung zu erstellen. Wählen Sie **Exchange**, um eine Supportanfrage zu erstellen, um nicht verwendete Teile der Reservierung auszutauschen.  
    | **Zugriffssteuerung (IAM)**   | Verwalten des Zugriffs auf die Reservierungs Informationen des Kunden.|
    | **Configuration**   | Ändern Sie den Bereich der Reservierung und/oder das Azure-Abonnement, dem die Reservierung zugeordnet ist.    |
    | **Eigenschaften**   | Zeigen Sie die Reservierungs Eigenschaften an, und kopieren Sie die Reservierungs-ID und die Reservierungs Auftrags-ID in die Zwischenablage. **Hinweis:** Support fordert möglicherweise die Reservierungs-ID und die Reservierungsauftrags-ID an, wenn Sie im Auftrag eines Kunden Support anfordern.    |
    | **Neue Supportanfrage**    | Support von Microsoft-Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Stornieren oder austauschen der Reservierung 

Wenn sich die Geschäftsanforderungen eines Kunden an einem beliebigen Punkt ändern, möchten Sie ggf. eine Reservierung stornieren und eine Rückerstattung oder einen Reservierungsbetrag für eine Reservierung erhalten, der zum Preis einer neuen Reservierung verwendet wird.

In beiden Szenarien erstattet Ihnen Microsoft den Betrag zurück, sodass Sie die daraus resultierenden Finanztransaktionen mit Ihren Kunden abwickeln können. Microsoft kontaktiert Kunden in Bezug auf Abrechnung, Stornierungen oder Rückerstattungen nicht direkt.   
 

**Funktionsweise von Stornierungen**

Kunden können jederzeit die Stornierung einer Reservierung beantragen (maximaler Rückerstattungsbetrag pro Jahr: 50.000 US-Dollar). Bei Stornierung einer Reservierung kann der Kunde die verbleibenden Monate einer Azure-Reservierung an Microsoft gegen eine Gebühr bei vorzeitigen Kündigung zurückzugeben. Der verbleibende gleichmäßige Saldo (abzüglich der frühen abbruchgebühr) wird an Ihr Konto zurückerstattet, damit Sie das Konto des Kunden zurückerstatten können. 

Nachfolgend finden Sie Details zu Kündigung und Gebühren.


|**Kündigungsdatum**<br> (Tage)   |**Verwendung**    |**Guthaben**  |**Frühzeitige Kündigung**<br> gebühr    |**Max. Rückerstattungsbetrag** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 oder weniger                         | Nein          | 100 %       | Nein                              | 50.000 USD   |
|5 oder weniger                         | Ja         | Anteilig  | Nein                              | 50.000 USD   |
|Mehr als 5                        | Nein          | Anteilig  | 12 %                             | 50.000 USD   |
|Mehr als 5                        | Ja         | Anteilig  | 12 %                             | 50.000 USD   |


**Funktionsweise des Umtauschs** 

Wenn ein Kunde eine andere Reservierung kaufen möchte als die, die er ursprünglich bei Ihnen gekauft hat, kann er einen Umtausch beantragen. Der Umtausch einer Reservierung kann eine attraktive Alternative zur Stornierung einer Reservierung sein, da er es dem Kunden ermöglicht, den anteiligen Rückerstattungsbetrag auf den Preis der neuen Reservierung anzurechnen. 

Der anteilige Rückerstattungsbetrag wird Ihrem Konto gutgeschrieben, damit Sie dem Kunden einen Umtausch anbieten können.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Fordern Sie eine Rückerstattung oder einen Austausch im Auftrag eines Kunden an 

Wenn Sie eine Supportanfrage für eine Erstattung oder einen Austausch im Auftrag ihrer Kunden einreichen möchten, wählen Sie den Kunden und die Reservierung im Partner Center aus, und erstellen Sie dann die Supportanfrage im Azure-Portal. 

>[!NOTE]
>Microsoft-Support-Agents können Sie nach der Reservierungs-ID und der Reservierungsbestellungs-ID fragen. Diese Informationen finden Sie auf der **Eigenschaften** Seite der Reservierung in der Azure-Portal. 

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, der eine Rückerstattung wünscht. 

2. Wählen Sie auf der Detailseite des Kunden die Option **Azure-Reservierungen** aus, und wählen Sie dann die spezifische Reservierung aus, die der Kunde erstattet.  

3. Wählen Sie unter **Aktionen**die Option **Erstattung** aus, um zum Reservierungsdaten Satz des Kunden im Azure-Portal zu wechseln und eine Supportanfrage zu initiieren.  

4. Auf der Seite **neue Supportanfrage**, führen Sie die folgenden Schritte aus, um eine Rückerstattung anzufordern. Wählen Sie **Weiter** nach jedem Schritt. 

    |**Schritt**                    |**Optionen**    |
    |:---------------------------|:-----------------|
    |**1 Grundlagen**                |Problemtyp: Abrechnung.  |
    |**2 Problem**               |Problemtyp: Reservierungsverwaltung. Kategorie: Austausch und Rückerstattungen. |
    |**3: Kontaktinformationen**   |Wählen Sie Ihre Einstellungen, und geben Sie die erforderlichen Informationen an. 

5.  Wählen Sie abschließend **Erstellen** aus.

## <a name="azure-reservations-resources"></a>Azure Reservations-Ressourcen
|**Weitere Informationen zu**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure Reservations in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Erwerb von Azure-Reservierungen für Ihre Kunden im Partner Center   |[Kaufen von Azure-Reservierungen](azure-reservations-buying.md) |
|Bestimmen der richtigen Größe für den virtuellen Computer und Überprüfen der Kunden-VM-Nutzung   |[Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Erwerb von Azure Reservations über die Partner Center-API | [Erwerben Sie Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in die Partner Center-Entwicklerdokumentation

