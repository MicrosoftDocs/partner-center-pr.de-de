---
title: Kauf des Azure-Plans
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie einzelne oder mehrere Azure-Abonnements und Azure-Reservierungen im Azure-Plan erwerben, Ressourcen konfigurieren sowie Abonnements anzeigen oder hinzufügen.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 04d47cef596b2c0a0ae13ff3f087d4b1b5f0437c
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215899"
---
# <a name="purchase-the-azure-plan-for-customers--access-the-latest-azure-services-at-pay-as-you-go-rates"></a>Erwerben Sie den Azure-Plan für Kunden und greifen Sie auf die neuesten Azure-Dienste zu nutzungsbasierten Tarifen zu.

**Geeignete Rollen**
- Globaler Administrator
- Benutzeradministrator
- Vertriebsbeauftragter

Wenn Sie im Rahmen des Microsoft-Kundenvertrags einen Azure-Plan für Ihre Kunden erwerben, haben Sie Zugriff auf den Gesamtkatalog der neuesten Azure-Dienste zu nutzungsbasierten Tarifen. CSP-Partner können jetzt auf jeden Azure-Dienst zugreifen, sobald er die allgemeine Verfügbarkeit erreicht hat. Ein Partner kann über mehrere Azure-Abonnements in einem Azure-Plan verfügen. 

## <a name="countryregion-availability"></a>Verfügbarkeit nach Land/Region

Für die neue Commerce-Benutzeroberfläche in CSP für Azure ist aktuell Verfügbarkeit in 139 Ländern geplant. Details finden Sie in der vollständigen Liste dieser [Länder/Regionen](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x). 

## <a name="how-to-purchase-azure-plan"></a>Erwerben des Azure-Plans

Der Erwerb eines Azure-Plans ähnelt dem Erwerb eines beliebigen anderen Abonnements. Der Hauptunterschied besteht darin, dass Sie vor der eigentlichen Bestellung bestätigen müssen, dass Ihr Kunde den Microsoft-Kundenvertrag unterzeichnet hat.

1. Wählen Sie **Segment: gewerblich** aus, und geben Sie **Microsoft Azure** ein 
2. Wählen Sie unter Azure-Plan **In den Warenkorb** aus

:::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Kauf":::

Der Partner muss bestätigen, dass der Kunde die Geschäftsbedingungen des Microsoft Kundenvertrags gelesen und ihnen zugestimmt hat. Weitere Informationen, wie der Partner dies sicherstellen kann, finden Sie unter [Bestätigen der Zustimmung des Kunden zum Microsoft-Kundenvertrag](confirm-customer-agreement.md). Weitere Ressourcen stehen im [Ressourcenkatalog](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/) zur Verfügung.

**Die Bestätigung können Sie wahlweise folgendermaßen vornehmen:** 

1. Digitales Bestätigen oder

2. Aufforderung an den Kunden, den Microsoft-Kundenvertrag direkt mit Microsoft abzuschließen. 

### <a name="to-confirm"></a>Zur Bestätigung 

1. Wählen Sie auf der Seite **Konto** des Kunden **Aktualisieren** neben **Microsoft-Kundenvertrag** aus  

2. Setzen Sie die Informationen zu der Person im Unternehmen des Kunden ein, die dem Microsoft-Kundenvertrag zugestimmt hat.

3. Wählen Sie **Speichern und fortfahren** aus.  

## <a name="review-and-buy"></a>Überprüfung und Kauf

Sie gelangen zur Seite **Produkt hinzufügen** zurück, auf der Sie sehen können, dass der Azure-Plan hinzugefügt wurde. Wählen Sie **Überprüfen** aus, um Ihren Kauf zu überprüfen, und wählen Sie dann **Kaufen** aus. 

>[!Note]
>Nachdem Sie den Azure-Plan für einen Kunden erworben haben, können Sie für diesen Kunden Microsoft Azure (0145p) nicht mehr kaufen. Sie müssen zukünftige Abonnements im Rahmen des Azure-Plans erstellen.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Erwerb von Azure-Reservierungen im Rahmen des Azure-Plans 
  
Im Partner Center können Sie darüber hinaus Microsoft Azure-Reservierungen im Rahmen des Azure-Plans im Kundenauftrag erwerben. (Alternativ können Sie Ihren [Kunden die Berechtigung erteilen, eigene Azure-Reservierungen zu erwerben](give-customers-permission.md), die aus einem früheren Abonnement stammen, das Sie für die Kunden erworben haben.)

1. Wählen Sie im Partner Center-Menü auf Ihrem [Dashboard](https://partner.microsoft.com/dashboard/) die Option **Kunden** aus. Suche den Kunden, der Azure-Reservierungen kaufen möchte. Klicke dann auf den nach unten zeigenden Pfeil, um den Datensatz des Kunden zu erweitern.

2. Wählen Sie **Produkte hinzufügen** und dann **Azure** aus. 

   - Wählen Sie in der Liste **Segment** das Marktsegment des Kunden aus.
   - Wählen Sie **Reservierungen** in der Liste **Typ** für Produkte aus.
   - Wählen Sie in der Liste **Reservierungstyp** den vom Kunden gewünschten Typ der Reservierung aus.

Azure-Reservierungen müssen einem aktiven Azure-Abonnement zugeordnet werden. Wählen Sie den Azure-Plan im Abonnement des Kunden aus, dem Sie Azure-Reservierungen hinzufügen möchten. 

>[!Important] 
>Wenn der Kunde noch keinen aktiven Azure-Plan besitzt, wähle Azure aus, um jetzt einen hinzuzufügen. Weitere Anweisungen finden Sie unter [Kaufen von Azure-Reservierungen](azure-reservations-buying.md#purchase-azure-reservations).

>[!Note]
>Der Umfang einer Reservierung kann im Partner Center derzeit nur auf **Freigegeben** festgelegt werden. Um den Umfang eines Einzelabonnements auszuwählen oder den Umfang von einem freigegebenen in ein Einzelabonnement zu aktualisieren, wechseln Sie wie nachfolgend beschrieben zum **Microsoft Azure-Verwaltungsportal**. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Einstellung „Freigegeben“ für den Umfang der Reservierungen":::

So verwalten Sie die Reservierung des Kunden im Azure-Portal: 

1. Wählen Sie unter **Kunden** den Kunden aus, den Sie verwalten möchten. 

2. Erweitern Sie mit dem Pfeil nach unten die Zeile des Kunden, und wählen Sie **Microsoft Azure-Verwaltungsportal** aus.  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Anzeigen von Azure-Abonnements im Azure-Plan

Erweitern Sie auf der Seite **Abonnements** im Abschnitt für nutzungsbasierte Angaben **Azure-Plan**, um die zugeordneten Azure-Abonnements unter dem Azure-Plan anzuzeigen.

:::image type="content" source="images/azure/addprods2.png" alt-text="Anzeigen der Liste mit Azure-Abonnements"::: 


## <a name="add-subscriptions-and-configure-resources"></a>Hinzufügen von Abonnements und Konfigurieren von Ressourcen

Im Azure-Portal fügen Sie Abonnements für Ihren Kunden hinzu und konfigurieren Ressourcen für ihn. Ferner kann die Umgebung deines Kunden nach Workload oder Projekt unterteilt werden. Abonnements können sowohl im Azure-Portal als auch in [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) verwaltet werden. 

Um die Ressourcen und Abonnements Ihres Kunden zu verwalten, benötigen Sie **AOBO**-Berechtigungen (Admin on Behalf Of, Administrator im Auftrag von). Informationen zum Verwalten Ihres Zugriffs finden Sie unter [Verwalten von Abonnements und Ressourcen im Rahmen des Azure-Plans](azure-plan-manage.md)

## <a name="next-steps"></a>Nächste Schritte

- [Umstellung von Kunden auf einen Azure-Plan](azure-plan-transition.md)

- [Vom Partner erworbenes Guthaben – Übersicht](partner-earned-credit.md)
