---
title: Verwalten von Azure-Reservierungen für Kunden
description: Erfahren Sie, wie Sie Azure-Reservierungen für einen Kunden verwalten, einschließlich der Stornierung einer Reservierung, des Umtauschs einer Reservierung oder des Anforderns einer Rückerstattung.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149484"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Verwalten, Stornieren, Umtausch oder Rückerstattung Microsoft Azure Reservierungen für Kunden

**Geeignete Rollen:** Administrator-Agent-| Globale | | des Helpdesk-Agents | des Vertriebsmitarbeiters Benutzerverwaltungsadministrator

In diesem Artikel wird erläutert, wie Sie Azure-Reservierungen für einen Kunden verwalten, einschließlich der Stornierung einer Reservierung, des Umtauschs einer Reservierung oder des Anforderns einer Rückerstattung.

> [!NOTE]
> Dieser Artikel gilt nur für Partner im CSP-Programm (Cloud Solution Provider). Kunden, die andere Abonnementtypen verwenden (z. B. Abonnements mit nutzungsbasierter Bezahlung, Einzelabonnements, Microsoft-Kundenvereinbarung oder Enterprise Agreement Abonnements), sollten stattdessen [diese Dokumentation zu Azure-Reservierungen](/azure/cost-management-billing/reservations)lesen.

Um die Azure-Reservierungen Ihrer Kunden nach dem Kauf zu verwalten, wählen Sie den Kunden und die Reservierung aus, die Sie in Partner Center verwalten möchten, und nehmen dann Änderungen an der Reservierung im Azure-Portal vor.

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, dessen Reservierungen Sie verwalten möchten. 

2. Wählen Sie im Menü der Detailseite des Kunden **Azure-Reservierungen** und dann die spezifische Reservierung aus, die Sie verwalten möchten.  

3. Wählen Sie unter **Aktionen** die Option **Verwalten** aus, um zum Reservierungsdatensatz des Kunden im Azure-Portal zu wechseln. Führen Sie auf der Seite „Reservierungsdetails“ die folgenden Schritte zum Abschließen der Aufgaben durch.  

    | **Auswählen**   | **An**    |
    |:-----------------------------|:-----------------|
    | **Übersicht**   | Zeigen Sie Details zur Reservierung eines Kunden an, einschließlich Ablaufdatum, Umfang und Nutzungsdaten. **Hinweis** Wählen Sie **Rückerstattung** aus, um eine Supportanfrage für eine anteilige Rückerstattung zu stellen. Wählen Sie **Umtausch** aus, um eine Supportanfrage zu stellen, um den ungenutzten Teil Ihrer Reservierungslaufzeit umzutauschen.  
    | **Zugriffssteuerung (IAM)**   | Verwalten sie den Zugriff auf die Reservierungsinformationen des Kunden.|
    | **Configuration**   | Ändern Sie den Reservierungsbereich und/oder das Azure-Abonnement, dem die Reservierung zugeordnet ist.    |
    | **Eigenschaften**   | Zeigen Sie die Eigenschaften der Reservierung an, und kopieren Sie die Reservierungs-ID und die Reservierungsauftrags-ID in die Zwischenablage. **Hinweis** Der Support fordert möglicherweise die Reservierungs-ID und Reservierungsauftrags-ID an, wenn Sie im Auftrag eines Kunden Support anfordern.    |
    | **Neue Supportanfrage**    | Dient zum Anfordern von Hilfe vom Microsoft-Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Stornieren oder Umtauschen einer Reservierung

Wenn sich die geschäftlichen Anforderungen eines Kunden zu einem beliebigen Zeitpunkt ändern, kann es sinnvoll sein, eine Reservierung zu stornieren und eine Rückerstattung zu erhalten oder den anteiligen Rückerstattungsbetrag einer Reservierung umtauschen zu lassen, der für den Preis einer neuen Reservierung verwendet wird.

In beiden Szenarien erstattet Ihnen Microsoft den Betrag zurück, sodass Sie die daraus resultierenden Finanztransaktionen mit Ihren Kunden abwickeln können. Microsoft kontaktiert Kunden in Bezug auf Abrechnung, Stornierungen oder Rückerstattungen nicht direkt.

### <a name="how-cancellations-work"></a>Funktionsweise von Stornierungen

Kunden können jederzeit die Stornierung einer Reservierung beantragen (maximaler Rückerstattungsbetrag pro Jahr: 50.000 US-Dollar). Durch das Stornieren einer Reservierung kann der Kunde den Betrag der verbleibenden Monate einer Azure-Reservierung gegen eine Gebühr für die vorzeitige Kündigung zurückgeben. Der verbleibende anteilige Saldo wird abzüglich der Gebühr für die vorzeitige Kündigung an Ihr Konto zurückerstattet, sodass Sie das Konto des Kunden zurückerstatten können. 

Nachfolgend finden Sie Details zu Kündigung und Gebühren.


|**Kündigungsdatum**<br> (Tage)   |**Verwendung**    |**Quelle**  |**Frühzeitige Kündigung**<br> gebühr    |**Max. Rückerstattungsbetrag** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 oder weniger                         | Nein          | 100%       | Nein                              | 50.000 USD   |
|5 oder weniger                         | Ja         | Anteilig  | Nein                              | 50.000 USD   |
|Mehr als 5                        | Nein          | Anteilig  | 12 %                             | 50.000 USD   |
|Mehr als 5                        | Ja         | Anteilig  | 12 %                             | 50.000 USD   |

### <a name="how-exchanges-work"></a>Funktionsweise des Umtauschs 

Wenn ein Kunde eine andere Reservierung kaufen möchte als die, die er ursprünglich bei Ihnen gekauft hat, kann er einen Umtausch beantragen. Der Umtausch einer Reservierung kann eine attraktive Alternative zum Stornieren einer Reservierung sein, da der Kunde den anteiligen Rückerstattungsbetrag für den Preis der neuen Reservierung verwenden kann. 

Der anteilige Rückerstattungsbetrag wird Ihrem Konto gutgeschrieben, damit Sie dem Kunden einen Umtausch anbieten können.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Anfordern einer Rückerstattung oder eines Umtauschs im Auftrag eines Kunden

Um eine Supportanfrage für eine Rückerstattung oder einen Umtausch im Namen Ihrer Kunden zu stellen, wählen Sie den Kunden und die Reservierung in Partner Center aus und erstellen dann die Supportanfrage im Azure-Portal. 

>[!NOTE]
>Microsoft-Supportmitarbeiter fragen Sie ggf. nach der Reservierungs-ID und Reservierungsauftrags-ID. Diese Informationen finden Sie auf der Seite **Eigenschaften** der Reservierung im Azure-Portal.

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, der eine Rückerstattung wünscht. 

2. Wählen Sie auf der Detailseite des Kunden **Azure-Reservierungen** und dann die spezifische Reservierung aus, die der Kunde zurückerstatten möchte.  

3. Wählen Sie unter **Aktionen** die Option **Erstattung** aus, um zum Reservierungsdatensatz des Kunden im Azure-Portal zu wechseln und eine Supportanfrage zu initiieren.  

4. Führen Sie auf der Seite **Neue Supportanfrage** die folgenden Schritte aus, um eine Rückerstattung zu beantragen. Klicken Sie nach jedem Schritt auf **Weiter**. 

   |**Schritt**                    |**Optionen**    |
   |:---------------------------|:-----------------|
   |**1 Grundlagen**                |Problemtyp: Abrechnung.  |
   |**2 Problem**               |Problemtyp: Reservierungsverwaltung. Kategorie: Umtausch und Rückerstattungen. |
   |**3: Kontaktinformationen**   |Wählen Sie Ihre Einstellungen aus, und geben Sie die erforderlichen Informationen ein. 

5. Wählen Sie **Erstellen** aus, wenn Sie fertig sind.

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen

|**Informationen über**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center   | [Kaufen von Azure-Reservierungen](azure-reservations-buying.md) |
|Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden   | [Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation   |
|Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen über ein Abonnement zu erwerben, das Sie für sie erworben haben. | [Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben](give-customers-permission.md)   |