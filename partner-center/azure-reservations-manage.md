---
title: Verwalten von Azure-Reservierungen für Kunden
description: Erfahren Sie, wie Sie Azure-Reservierungen für einen Kunden verwalten und wie Sie eine Reservierung stornieren, eine Reservierung austauschen oder eine Rückerstattung anfordern.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: fba1427978e61b739c8ffb14374a44331ef51d27
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "89366874"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Verwalten, Abbrechen, austauschen oder Rückerstattung von Microsoft Azure Reservierungen für Kunden

**Zielgruppe**

- Partner Center
- Microsoft Azure-Portal 
- Partner im CSP

**Geeignete Rollen**

- Administrator-Agent
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

> [!NOTE]
> Dieser Artikel gilt nur für Partner im CSP-Programm (Cloud Solution Provider). Kunden, die andere Abonnementtypen (z. b. Pay-as-you-go, individuelle, Microsoft-Kunden Vereinbarung oder Konzernvertrag Abonnements) verwenden, sollten stattdessen [diese Azure-Reservierungs Dokumentation](https://docs.microsoft.com/azure/cost-management-billing/reservations)lesen.

Um die Azure-Reservierungen ihrer Kunden nach dem Kauf zu verwalten, wählen Sie den Kunden und die Reservierung aus, die Sie in Partner Center verwalten möchten, und nehmen dann Änderungen an der Reservierung im Azure-Portal vor.

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, dessen Reservierungen Sie verwalten möchten. 

2. Wählen Sie im Menü Detailseite des Kunden die Option **Azure-Reservierungen** aus, und wählen Sie dann die jeweilige Reservierung aus, die Sie verwalten möchten.  

3. Wählen Sie unter **Aktionen**die Option **Verwalten** aus, um zum Reservierungsdaten Satz des Kunden in der Azure-Portal zu wechseln. Führen Sie auf der Seite „Reservierungsdetails“ die folgenden Schritte zum Abschließen der Aufgaben durch.  

    | **Auswählen**   | **An**    |
    |:-----------------------------|:-----------------|
    | **Übersicht**   | Anzeigen von Details der Reservierung eines Kunden, einschließlich Ablaufdatum, Bereich und Verwendungs Daten. **Hinweis** Wählen Sie **Rückerstattung** aus, um eine Supportanfrage für eine anteilige Rückerstattung zu stellen. Wählen Sie **Umtausch** aus, um eine Supportanfrage zu stellen, um den ungenutzten Teil Ihrer Reservierungslaufzeit umzutauschen.  
    | **Access Control (IAM)**   | Verwalten des Zugriffs auf die Reservierungs Informationen des Kunden.|
    | **Konfiguration**   | Ändern Sie den Bereich der Reservierung und/oder das Azure-Abonnement, dem die Reservierung zugeordnet ist.    |
    | **Eigenschaften**   | Zeigen Sie die Reservierungs Eigenschaften an, und kopieren Sie die Reservierungs-ID und die Reservierungs Auftrags-ID in die Zwischenablage. **Hinweis** Der Support fordert möglicherweise die Reservierungs-ID und Reservierungsauftrags-ID an, wenn Sie im Auftrag eines Kunden Support anfordern.    |
    | **Neue Supportanfrage**    | Dient zum Anfordern von Hilfe vom Microsoft-Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Stornieren oder Umtauschen einer Reservierung

Wenn sich die Geschäftsanforderungen eines Kunden an einem beliebigen Punkt ändern, möchten Sie ggf. eine Reservierung stornieren und eine Rückerstattung oder einen Reservierungsbetrag für eine Reservierung erhalten, der zum Preis einer neuen Reservierung verwendet wird.

In beiden Szenarien erstattet Ihnen Microsoft den Betrag zurück, sodass Sie die daraus resultierenden Finanztransaktionen mit Ihren Kunden abwickeln können. Microsoft kontaktiert Kunden in Bezug auf Abrechnung, Stornierungen oder Rückerstattungen nicht direkt.

### <a name="how-cancellations-work"></a>Funktionsweise von Stornierungen

Kunden können jederzeit die Stornierung einer Reservierung beantragen (maximaler Rückerstattungsbetrag pro Jahr: 50.000 US-Dollar). Das Abbrechen einer Reservierung ermöglicht es dem Kunden, die Menge der verbleibenden Monate einer Azure-Reservierung für eine frühe abbruchgebühr zurückzugeben. Der verbleibende gleichmäßige Saldo (abzüglich der frühen abbruchgebühr) wird an Ihr Konto zurückerstattet, damit Sie das Konto des Kunden zurückerstatten können. 

Nachfolgend finden Sie Details zu Kündigung und Gebühren.


|**Kündigungsdatum**<br> (Tage)   |**Verwendung**    |**Quelle**  |**Frühzeitige Kündigung**<br> gebühr    |**Max. Rückerstattungsbetrag** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 oder weniger                         | Nein          | 100 %       | Nein                              | 50.000 USD   |
|5 oder weniger                         | Ja         | Anteilig  | Nein                              | 50.000 USD   |
|Mehr als 5                        | Nein          | Anteilig  | 12 %                             | 50.000 USD   |
|Mehr als 5                        | Ja         | Anteilig  | 12 %                             | 50.000 USD   |

### <a name="how-exchanges-work"></a>Funktionsweise des Umtauschs 

Wenn ein Kunde eine andere Reservierung kaufen möchte als die, die er ursprünglich bei Ihnen gekauft hat, kann er einen Umtausch beantragen. Der Austausch einer Reservierung kann eine attraktive Alternative zum Abbrechen einer Reservierung sein, da der Kunde die anteilsmäßig auf den Preis der neuen Reservierung angerechnet. 

Der anteilige Rückerstattungsbetrag wird Ihrem Konto gutgeschrieben, damit Sie dem Kunden einen Umtausch anbieten können.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Anfordern einer Rückerstattung oder eines Umtauschs im Auftrag eines Kunden

Wenn Sie eine Supportanfrage für eine Erstattung oder einen Austausch im Auftrag ihrer Kunden einreichen möchten, wählen Sie den Kunden und die Reservierung im Partner Center aus, und erstellen Sie dann die Supportanfrage im Azure-Portal. 

>[!NOTE]
>Microsoft-Supportmitarbeiter fragen Sie ggf. nach der Reservierungs-ID und Reservierungsauftrags-ID. Diese Informationen finden Sie auf der **Eigenschaften** Seite der Reservierung in der Azure-Portal.

1. Wählen Sie zunächst im Menü „Partner Center“ **Kunden** und dann den Kunden aus, der eine Rückerstattung wünscht. 

2. Wählen Sie auf der Detailseite des Kunden die Option **Azure-Reservierungen** aus, und wählen Sie dann die spezifische Reservierung aus, die der Kunde erstattet.  

3. Wählen Sie unter **Aktionen**die Option **Erstattung** aus, um zum Reservierungsdaten Satz des Kunden im Azure-Portal zu wechseln und eine Supportanfrage zu initiieren.  

4. Führen Sie auf der Seite **Neue Supportanfrage** die folgenden Schritte aus, um eine Rückerstattung zu beantragen. Klicken Sie nach jedem Schritt auf **Weiter**. 

   |**Schritt**                    |**Optionen**    |
   |:---------------------------|:-----------------|
   |**1 Grundlagen**                |Problemtyp: Abrechnung.  |
   |**2 Problem**               |Problemtyp: Reservierungs Verwaltung. Kategorie: Austausch Vorgänge und Rückerstattungen. |
   |**3: Kontaktinformationen**   |Wählen Sie Ihre Einstellungen aus, und geben Sie die erforderlichen Informationen ein. 

5. Wählen Sie **Erstellen** aus, wenn Sie fertig sind.

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen

|**Informationen über**   |**Artikel**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved Instances](azure-reservations.md) |
|Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center   | [Kaufen von Azure-Reservierungen](azure-reservations-buying.md) |
|Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden   | [Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen](azure-usage.md)   |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation   |
|Erteilen von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von einem Abonnement zu erwerben, das Sie für Sie erworben haben. | [Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.](give-customers-permission.md)   |

