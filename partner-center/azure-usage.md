---
title: Microsoft Azure VM-Größe für die Verwendung der maximalen Reservierung | Partner-Dashboard
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: Azure, Reservierungen, virtueller Computer, verwalten, Nutzung, Größe
ms.openlocfilehash: 9ddf74d209f9174b4192a9d89b65a41e371f37ae
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2018
ms.locfileid: "1883101"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure VM-Größe für die maximale Reservations-Nutzung 

**Betriff:**

-  Partner-Dashboard
-  Azure-Portal
-  CSP-Partner

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Bestimmen Sie die Größe der virtuellen Computer für die Reservierung eines Kunden in Azure 

Wenn Sie Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden kaufen, müssen Sie einen virtuellen Computer (VM) wählen, dessen Größe die Computing-Anforderungen des Kunden erfüllt. Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:

-   Azure-Nutzungs-API
-   Das Azure-Portal
-   Azure PowerShell
-   Die API für Azure Resource Manager (ARM)

Nachstehend finden Sie Anleitungen für jede dieser Vorgehensweisen. Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet. Sie müssen die Reservierung keinem virtuellen Computer zuweisen.

>[!NOTE]
>Reservierungsrabatte gelten nicht für klassische VMs oder zu Werbezwecken.

>[!IMPORTANT]
>Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ der VM in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.


**Rufen Sie die VM-Größeninformationen mit der Azure-Nutzungs-API ab**

1.  Verwenden Sie den Wert für Diensttyp-Attribute aus Information in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren. 

2.  Weitere Informationen finden Sie unter [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner-Dashboard-API](https://docs.microsoft.com/partner-center/develop/). 

**Rufen Sie die VM-Größeninformationen im Microsoft Azure-Portal ab**

1.  Wechseln Sie in Ihrem Partner-Dashboard zur Seite Ihres **Kunden**.

2.  Suchen Sie den Kunden, der Azure VM Reservations kaufen möchte, und wählen Sie dann den Pfeil nach unten, um die Informationen des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal**, um die Daten des Kunden im Azure-Portal zu öffnen. 

3.  Wählen Sie **virtueller Computer** aus dem Portalmenü und wählen Sie dann den virtuellen Computer, für den Sie eine Reservierung erwerben möchten. 

4.  Erhalten Sie auf der Seite mit den Details des virtuellen Computers die Größe und Region, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung im Partner Center zu erwerben.  

    ![](images/usage1.png)

**Rufen Sie die VM-Größeninformationen in Microsoft Azure PowerShell ab**

Verwenden Sie die Informationen in der Abbildungunten zum Abrufen der Position und Größe des virtuellen Computers, für die Sie eine Reservierung erwerben möchten. 

![](images/usage2.png)

**Rufen Sie die VM-Größeninformationen in der Azure Resource Manager (ARM)-API ab**

1.  Rufen Sie mithilfe der ARMClient oder der ARM-APIs den ARM-Client für den virtuellen Computer, für den Sie eine Reservierung erwerben möchten.

2.  /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3.  Der Aufruf gibt die Werte für **VmSize** und **Speicherort** wieder, wie unten dargestellt.

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Überprüfen Sie die Azure-VM-Nutzung und den Reservierungsrabatt

Nach dem Erwerb einer Azure Reserved VM Instance im Auftrag eines Kunden wird der Rabatt für den im Voraus bezahlten VM-Speicherplatz automatisch auf den virtuellen Computer angewendet, der dem Attribute und der Menge der Reservierung des Kunden entsprechen. 

Überprüfen Sie die Reservierungsnutzung des Kunden und sehen Sie, auf welchen virtuellen Computer der Reservierungsrabatt angewendet wird, mithilfe einer der folgenden Methoden:   

-   Das Azure-Portal
-   Azure-Nutzungs-API

Nachstehend finden Sie Anleitungen für jede dieser Vorgehensweisen.

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt, auf welchen virtuellen Computer der Rabatt angewendet wird.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Überprüfen Sie die Reservierungsnutzung des Kunden im Microsoft Azure-Portal

1.  Wechseln Sie in Ihrem Partner-Dashboard zur Seite Ihres **Kunden**.

2.  Suchen Sie den Kunden, dessen Reservierungsrabatt und -nutzung Sie überprüfen möchten, und wählen Sie dann den Pfeil nach unten, um die Informationen des Kunden zu erweitern. Wählen Sie **Microsoft Azure-Verwaltungsportal**, um die Daten des Kunden im Azure-Portal zu öffnen. 

3.  Wählen Sie **Reservierung** aus dem Portalmenü und wählen Sie dann die Reservierung, für die Sie die Nutzung überprüfen möchten. 

4.  Auf der Seite **Übersicht** überprüfen Sie das Reservierungs-Auslastungsdiagramm, das zeigt, welcher Anteil der Reservierung für den virtuellen Computer angewendet wurde. 

    >[!NOTE]
    >Nutzungsdaten können auf bis zu 8 Stunden verzögert werden.
    
    a.  Ist die Reservierungsauslastung 100%, erhält Ihr Kunde alle möglichen Einsparungen, die der Kauf der Reservierung ermöglicht. 
    
    b.  Ist die Reservierungsnutzung 0%, wird kein Rabatt auf dem virtuellen Computer angewendet. 
    
    c.  Wenn die Reservierung zwischen 1 und 99% ist, gibt es nicht verwendete Vorteile. 

5.  Um dies zu vermeiden, bestimmen Sie die richtige Größe der VM zur Unterstützung des Computingbedarfs des Kunden vor dem Kauf.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Überprüfen Sie die Reservierungsnutzung des Kunden mit der Azure Nutzungs-API

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt, auf welchen virtuellen Computer der Rabatt angewendet wird.  

Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält und um zu sehen, auf welche VMs (virtuelle Maschinen) der Rabatt angewendet wird. Vergleichen Sie Beispiel A mit Beispiel B um die Reservierungsnutzung des Kunden zu überprüfen. 

![](images\usage5.png)

-   Die ReservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.
-   ConsumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.
-   ReservationMeter zeigt $0, da der Reservierungsrabatt angewendet wurde. 

Weitere Informationen finden Sie unter [Abrufen der Nutzungseinträge eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Kosten für Software, z.B. Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und werden als separate Positionen in den Daten und auf Ihrer Rechnung angezeigt. Wenn ein Kunde über die Azure-Hybridnutzung verfügt, werden die Softwarekosten nicht angewendet. Weitere Informationen finden Sie unter [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Azure Reservations-Ressourcen
|**Weitere Informationen**   |**Bitte lesen**    |
|:-----------------------------|:-----------------|
|Azure Reservations in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure Reservations für Ihre Kunden im Partner-Dashboard   |[Azure Reservations kaufen](azure-reservations-buying.md)
|Abrechnung für Azure Reservations   |[Abrechnung für Azure Reservations](azure-reservations-billing.md)   |
| Verwalten von Azure Reservations in Ihrem Partner-Dashboard | [Verwalten von Azure Reservations in Ihrem Partner-Dashboard](azure-reservations-manage.md)
|Erwerb von Azure Reservations im Azure-Portal | [Für virtuelle Maschinen mit Azure Reserved VM Instances im Voraus bezahlen](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure Reservations im Azure-Portal   |[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure Reservations über die Partner Center-API | [Erwerben Sie Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) in die Partner Center-Entwicklerdokumentation



