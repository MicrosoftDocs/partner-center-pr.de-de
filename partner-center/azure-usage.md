---
title: Microsoft Azure VM-Größe für die Verwendung der maximalen Reservierung | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, VM, verwalten, Nutzung, Größe
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2b8148d66be8a439056efa41eccb60cbc3e4274b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253248"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure VM-Größe für die maximale Reservierungsnutzung

**Zielgruppe**

- Partner Center
- Azure-Portal
- Partner im CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determine the VM size for a customer's Azure reservation 

When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs. Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:

- Azure-Nutzungs-API
- Das Azure-Portal
- Azure PowerShell
- Die API für Azure Resource Manager (ARM)

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen. Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet. You don't need to assign the reservation to a VM.

>[!NOTE]
>Reservation discounts don't apply to classic or promotional VMs.

>[!IMPORTANT]
>Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.

**Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API**

1. Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.
2. For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

**Abrufen der VM-Größeninformationen im Microsoft Azure-Portal**

1. Navigieren Sie im Partner Center zur Seite **Kunden**.
2. Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.
4. On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.  

    ![Informationen zu Größe und Region auf der Detailseite](images/usage1.png)

**Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell**

Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten. 

![VM-Standort und Größe](images/usage2.png)

**Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API**

1. Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).

    ![vmSize value](images/usage3.png) ![location value](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts

After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.

You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:

- Das Azure-Portal
- Azure-Nutzungs-API

Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verify the customer's reservation usage in the Microsoft Azure portal

1. Navigieren Sie im Partner Center zur Seite **Kunden**.

2. Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.
4. On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.

    >[!NOTE]
    >Nutzungsdaten können um bis zu 8 Stunden verzögert sein.

    a. If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.
    b. If the reservation's usage is 0%, the discount is not being applied to any virtual machine.
    c. If the reservation's usage is between 1% and 99%, there are unused benefits.

5. To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verify the customer's reservation usage with the Azure utilization API

>[!NOTE]
>Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.  

Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird. Compare Example A to Example B to see how to verify a customer's reservation usage.

![Beispiele für die Reservierungsnutzung](images/usage5.png)

- Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.
- consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.
- ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.

For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung. Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet. Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen

|**Weitere Informationen zu**   |**Bitte lesen**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure-Reservierungen für Ihre Kunden im Partner Center   |[Kaufen von Azure-Reservierungen](azure-reservations-buying.md)
|Verwalten von Azure-Reservierungen im Partner Center | [Verwalten von Azure-Reservierungen im Partner Center](azure-reservations-manage.md)
|Erwerb von Azure-Reservierungen im Azure-Portal | [Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure-Reservierungen im Azure-Portal   |[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation
