---
title: Verwalten von Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden | Partner Center
ms.topic: article
ms.date: 03/15/2019
Description: Um Azure-Reservierungen nach dem Kauf für Ihre Kunden zu verwalten, wählen Sie den Kunden und die Reservierung, die Sie im Partner Center verwalten möchten, und nehmen Sie dann die Änderungen an der Reservierung im Azure-Portal vor.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, verwalten, Abrechnung, Kauf, Stornierung, Umtausch, Gebühr bei vorzeitiger Kündigung
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b7e9726acbba54daf8404fdf4a3d2b4961c5123a
ms.sourcegitcommit: 4b8cad9f24229767dd44fa9418fe57e10d74f390
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2019
ms.locfileid: "71704161"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Verwalten von Microsoft Azure Reservations im Auftrag Ihrer Kunden       

**Gilt für**

-  Partner Center
-  Microsoft Azure-Portal 
-  Partner im Cloud Solution Provider-Programm

Um Azure-Reservierungen nach dem Kauf für Ihre Kunden zu verwalten, wählen Sie den Kunden und die Reservierung, die Sie im Partner Center verwalten möchten, und nehmen Sie dann die Änderungen an der Reservierung im Azure-Portal vor. 

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, dessen Reservierungen Sie verwalten möchten. 

2. Wählen Sie im Menü auf der Detailseite des Kunden **Azure-Reservierungen** und dann die spezifische Reservierung aus, die Sie verwalten möchten.  

3. Klicken Sie unter **Aktionen**auf **verwalten**, und wechseln Sie zum Reservierungsdatensatz des Kunden im Azure-Portal. Führen Sie auf der Seite „Reservierungsdetails“ die folgenden Schritte zum Abschließen der Aufgaben durch.  

    | **Auswahl**   | **Zweck**    |
    |:-----------------------------|:-----------------|
    | **Übersicht**   | Hier werden Reservierungsdetails des Kunden angezeigt, einschließlich Ablaufdatum, Bereich und Nutzungsdaten. **Hinweis** Wählen Sie **Rückerstattung** aus, um eine Supportanfrage für eine anteilige Rückerstattung zu stellen. Wählen Sie **Umtausch** aus, um eine Supportanfrage zu stellen, um den ungenutzten Teil Ihrer Reservierungslaufzeit umzutauschen.  
    | **Zugriffssteuerung (IAM)**   | Dient zum Verwalten des Zugriffs auf die Informationen zur Reservierung des Kunden.|
    | **Konfiguration**   | Dient zum Ändern des Reservierungsbereichs bzw. Azure-Abonnements, dem die Reservierung zugeordnet ist.    |
    | **Eigenschaften**   | Dient zum Anzeigen der Eigenschaften der Reservierung und Kopieren der Reservierungs-ID und Reservierungsauftrags-ID in die Zwischenablage. **Hinweis** Der Support fordert möglicherweise die Reservierungs-ID und Reservierungsauftrags-ID an, wenn Sie im Auftrag eines Kunden Support anfordern.    |
    | **Neue Supportanfrage**    | Dient zum Anfordern von Hilfe vom Microsoft-Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Stornieren oder Umtauschen einer Reservierung 

Wenn sich die geschäftliche Anforderung eines Kunden zu einem beliebigen Zeitpunkt ändert, können Sie die Reservierung stornieren oder einen anteiligen Rückerstattungsbetrag mit dem Preis einer neuen Reservierung verrechnen.

In beiden Szenarien erstattet Ihnen Microsoft den Betrag zurück, sodass Sie die daraus resultierenden Finanztransaktionen mit Ihren Kunden abwickeln können. Microsoft kontaktiert Kunden in Bezug auf Abrechnung, Stornierungen oder Rückerstattungen nicht direkt.   
 

**Funktionsweise von Stornierungen**

Kunden können jederzeit die Stornierung einer Reservierung beantragen (maximaler Rückerstattungsbetrag pro Jahr: 50.000 US-Dollar). Bei Stornierung einer Reservierung kann der Kunde die verbleibenden Monate einer Azure-Reservierung an Microsoft gegen eine Gebühr bei vorzeitigen Kündigung zurückzugeben. Der verbleibende anteilige Saldo, abzüglich der Gebühren bei vorzeitiger Kündigung, wird Ihrem Konto gutgeschrieben, sodass Sie den Betrag dem Konto des Kunden zurückerstatten können. 

Nachfolgend finden Sie Details zu Kündigung und Gebühren.


|**Kündigungsdatum**<br> (Tage)   |**Nutzung**    |**Guthaben**  |**Frühzeitige Kündigung**<br> gebühr    |**Max. Rückerstattungsbetrag** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 oder weniger                         | Nein          | 100 %       | Nein                              | 50.000 USD   |
|5 oder weniger                         | Ja         | Anteilig  | Nein                              | 50.000 USD   |
|Mehr als 5                        | Nein          | Anteilig  | 12 %                             | 50.000 USD   |
|Mehr als 5                        | Ja         | Anteilig  | 12 %                             | 50.000 USD   |


**Funktionsweise des Umtauschs** 

Wenn ein Kunde eine andere Reservierung kaufen möchte als die, die er ursprünglich bei Ihnen gekauft hat, kann er einen Umtausch beantragen. Der Umtausch einer Reservierung kann eine attraktive Alternative zur Stornierung einer Reservierung sein, da er es dem Kunden ermöglicht, den anteiligen Rückerstattungsbetrag auf den Preis der neuen Reservierung anzurechnen. 

Der anteilige Rückerstattungsbetrag wird Ihrem Konto gutgeschrieben, damit Sie dem Kunden einen Umtausch anbieten können.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Anfordern einer Rückerstattung oder eines Umtauschs im Auftrag eines Kunden 

Um eine Supportanfrage für eine Rückerstattung oder einen Umtausch im Auftrag Ihres Kunden zu stellen, wählen Sie den Kunden und die Reservierung im Partner Center aus, und erstellen Sie dann die Supportanfrage im Azure-Portal. 

>[!NOTE]
>Microsoft-Supportmitarbeiter fragen Sie ggf. nach der Reservierungs-ID und Reservierungsauftrags-ID. Sie finden diese Informationen auf der Seite **Eigenschaften** der Reservierung im Azure-Portal. 

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, der eine Rückerstattung wünscht. 

2. Wählen Sie auf der Detailseite des Kunden **Azure-Reservierungen** und dann die spezifische Reservierung aus, die der Kunde zurückerstattet haben möchte.  

3. Klicken Sie unter **Aktionen** auf **Rückerstattung**, um zu den Daten der Kundenreservierung im Azure-Portal zu wechseln und eine Supportanfrage zu stellen.  

4. Führen Sie auf der Seite **Neue Supportanfrage** die folgenden Schritte aus, um eine Rückerstattung zu beantragen. Klicken Sie nach jedem Schritt auf **Weiter**. 

    |**Schritt**                    |**Optionen**    |
    |:---------------------------|:-----------------|
    |**1 Grundlagen**                |Art des Anliegens: Abrechnung.  |
    |**2 Problem**               |Art des Problems: Reservierungsverwaltung. Kategorie: Umtausche und Rückerstattungen. |
    |**3: Kontaktinformationen**   |Wählen Sie Ihre Einstellungen aus, und geben Sie die erforderlichen Informationen ein. 

5.  Klicken Sie abschließend auf **Erstellen**.

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen
|**Weitere Informationen zu**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Erwerb von Azure-Reservierungen für Ihre Kunden im Partner Center   |[Kaufen von Azure-Reservierungen](azure-reservations-buying.md) |
|Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden   |[Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Kaufen von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation

