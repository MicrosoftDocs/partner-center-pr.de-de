---
title: Microsoft Azure VM-Größe für die Verwendung der maximalen Reservierung | Partner-Dashboard
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: Azure, Reservierungen, virtueller Computer, verwalten, Nutzung, Größe
ms.openlocfilehash: 4050780f9d3dc3ad7d3c4ece0d363845ec1efe9c
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/11/2018
ms.locfileid: "1873788"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="5577c-103">Microsoft Azure VM-Größe für die maximale Reservations-Nutzung</span><span class="sxs-lookup"><span data-stu-id="5577c-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="5577c-104">Betriff:</span><span class="sxs-lookup"><span data-stu-id="5577c-104">Applies to</span></span>**

-  <span data-ttu-id="5577c-105">Partner-Dashboard</span><span class="sxs-lookup"><span data-stu-id="5577c-105">Partner Dashboard</span></span>
-  <span data-ttu-id="5577c-106">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="5577c-106">Azure portal</span></span>
-  <span data-ttu-id="5577c-107">CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="5577c-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="5577c-108">Bestimmen Sie die Größe der virtuellen Computer für die Reservierung eines Kunden in Azure</span><span class="sxs-lookup"><span data-stu-id="5577c-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="5577c-109">Wenn Sie Microsoft Azure-Reservierungen im Auftrag Ihrer Kunden kaufen, müssen Sie einen virtuellen Computer (VM) wählen, dessen Größe die Computing-Anforderungen des Kunden erfüllt.</span><span class="sxs-lookup"><span data-stu-id="5577c-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="5577c-110">Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:</span><span class="sxs-lookup"><span data-stu-id="5577c-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="5577c-111">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="5577c-111">Azure utilization API</span></span>
-   <span data-ttu-id="5577c-112">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="5577c-112">The Azure portal</span></span>
-   <span data-ttu-id="5577c-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5577c-113">Azure PowerShell</span></span>
-   <span data-ttu-id="5577c-114">Die API für Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="5577c-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="5577c-115">Nachstehend finden Sie Anleitungen für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="5577c-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="5577c-116">Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="5577c-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="5577c-117">Sie müssen die Reservierung keinem virtuellen Computer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="5577c-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="5577c-118">Reservierungsrabatte gelten nicht für klassische VMs oder zu Werbezwecken.</span><span class="sxs-lookup"><span data-stu-id="5577c-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="5577c-119">Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ der VM in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5577c-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="5577c-120">Rufen Sie die VM-Größeninformationen mit der Azure-Nutzungs-API ab</span><span class="sxs-lookup"><span data-stu-id="5577c-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="5577c-121">Verwenden Sie den Wert für Diensttyp-Attribute aus Information in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="5577c-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="5577c-122">Weitere Informationen finden Sie unter [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner-Dashboard-API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="5577c-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="5577c-123">Rufen Sie die VM-Größeninformationen im Microsoft Azure-Portal ab</span><span class="sxs-lookup"><span data-stu-id="5577c-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="5577c-124">Wechseln Sie in Ihrem Partner-Dashboard zur Seite Ihres **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="5577c-124">In your Partner Dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="5577c-125">Suchen Sie den Kunden, der Azure VM Reservations kaufen möchte, und wählen Sie dann den Pfeil nach unten, um die Informationen des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="5577c-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="5577c-126">Wählen Sie **Microsoft Azure-Verwaltungsportal**, um die Daten des Kunden im Azure-Portal zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="5577c-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="5577c-127">Wählen Sie **virtueller Computer** aus dem Portalmenü und wählen Sie dann den virtuellen Computer, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="5577c-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="5577c-128">Erhalten Sie auf der Seite mit den Details des virtuellen Computers die Größe und Region, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung im Partner Center zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="5577c-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![](images/usage1.png)

**<span data-ttu-id="5577c-129">Rufen Sie die VM-Größeninformationen in Microsoft Azure PowerShell ab</span><span class="sxs-lookup"><span data-stu-id="5577c-129">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="5577c-130">Verwenden Sie die Informationen in der Abbildungunten zum Abrufen der Position und Größe des virtuellen Computers, für die Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="5577c-130">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![](images/usage2.png)

**<span data-ttu-id="5577c-131">Rufen Sie die VM-Größeninformationen in der Azure Resource Manager (ARM)-API ab</span><span class="sxs-lookup"><span data-stu-id="5577c-131">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="5577c-132">Rufen Sie mithilfe der ARMClient oder der ARM-APIs den ARM-Client für den virtuellen Computer, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="5577c-132">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="5577c-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="5577c-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="5577c-134">Der Aufruf gibt die Werte für **VmSize** und **Speicherort** wieder, wie unten dargestellt.</span><span class="sxs-lookup"><span data-stu-id="5577c-134">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="5577c-135">Überprüfen Sie die Azure-VM-Nutzung und den Reservierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="5577c-135">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="5577c-136">Nach dem Erwerb einer Azure Reserved VM Instance im Auftrag eines Kunden wird der Rabatt für den im Voraus bezahlten VM-Speicherplatz automatisch auf den virtuellen Computer angewendet, der dem Attribute und der Menge der Reservierung des Kunden entsprechen.</span><span class="sxs-lookup"><span data-stu-id="5577c-136">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="5577c-137">Überprüfen Sie die Reservierungsnutzung des Kunden und sehen Sie, auf welchen virtuellen Computer der Reservierungsrabatt angewendet wird, mithilfe einer der folgenden Methoden:</span><span class="sxs-lookup"><span data-stu-id="5577c-137">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="5577c-138">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="5577c-138">The Azure portal</span></span>
-   <span data-ttu-id="5577c-139">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="5577c-139">Azure utilization API</span></span>

<span data-ttu-id="5577c-140">Nachstehend finden Sie Anleitungen für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="5577c-140">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="5577c-141">Nur die Azure-Nutzungs-API-zeigt, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="5577c-141">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="5577c-142">Überprüfen Sie die Reservierungsnutzung des Kunden im Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="5577c-142">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="5577c-143">Wechseln Sie in Ihrem Partner-Dashboard zur Seite Ihres **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="5577c-143">In your Partner Dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="5577c-144">Suchen Sie den Kunden, dessen Reservierungsrabatt und -nutzung Sie überprüfen möchten, und wählen Sie dann den Pfeil nach unten, um die Informationen des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="5577c-144">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="5577c-145">Wählen Sie **Microsoft Azure-Verwaltungsportal**, um die Daten des Kunden im Azure-Portal zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="5577c-145">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="5577c-146">Wählen Sie **Reservierung** aus dem Portalmenü und wählen Sie dann die Reservierung, für die Sie die Nutzung überprüfen möchten.</span><span class="sxs-lookup"><span data-stu-id="5577c-146">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="5577c-147">Auf der Seite **Übersicht** überprüfen Sie das Reservierungs-Auslastungsdiagramm, das zeigt, welcher Anteil der Reservierung für den virtuellen Computer angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="5577c-147">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="5577c-148">Nutzungsdaten können auf bis zu 8 Stunden verzögert werden.</span><span class="sxs-lookup"><span data-stu-id="5577c-148">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="5577c-149">a.</span><span class="sxs-lookup"><span data-stu-id="5577c-149">a.</span></span>  <span data-ttu-id="5577c-150">Ist die Reservierungsauslastung 100%, erhält Ihr Kunde alle möglichen Einsparungen, die der Kauf der Reservierung ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="5577c-150">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="5577c-151">b.</span><span class="sxs-lookup"><span data-stu-id="5577c-151">b.</span></span>  <span data-ttu-id="5577c-152">Ist die Reservierungsnutzung 0%, wird kein Rabatt auf dem virtuellen Computer angewendet.</span><span class="sxs-lookup"><span data-stu-id="5577c-152">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="5577c-153">c.</span><span class="sxs-lookup"><span data-stu-id="5577c-153">c.</span></span>  <span data-ttu-id="5577c-154">Wenn die Reservierung zwischen 1 und 99% ist, gibt es nicht verwendete Vorteile.</span><span class="sxs-lookup"><span data-stu-id="5577c-154">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="5577c-155">Um dies zu vermeiden, bestimmen Sie die richtige Größe der VM zur Unterstützung des Computingbedarfs des Kunden vor dem Kauf.</span><span class="sxs-lookup"><span data-stu-id="5577c-155">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="5577c-156">Überprüfen Sie die Reservierungsnutzung des Kunden mit der Azure Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="5577c-156">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="5577c-157">Nur die Azure-Nutzungs-API-zeigt, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="5577c-157">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="5577c-158">Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält und um zu sehen, auf welche VMs (virtuelle Maschinen) der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="5577c-158">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="5577c-159">Vergleichen Sie Beispiel A mit Beispiel B um die Reservierungsnutzung des Kunden zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="5577c-159">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![](images\usage5.png)

-   <span data-ttu-id="5577c-160">Die ReservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="5577c-160">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="5577c-161">ConsumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="5577c-161">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="5577c-162">ReservationMeter zeigt $0, da der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="5577c-162">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="5577c-163">Weitere Informationen finden Sie unter [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner-Dashboard-API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="5577c-163">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="5577c-164">Kosten für Software, z.B. Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und werden als separate Positionen in den Daten und auf Ihrer Rechnung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5577c-164">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="5577c-165">Wenn ein Kunde über die Azure-Hybridnutzung verfügt, werden die Softwarekosten nicht angewendet.</span><span class="sxs-lookup"><span data-stu-id="5577c-165">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="5577c-166">Weitere Informationen finden Sie unter [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="5577c-166">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="5577c-167">Azure Reservations-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="5577c-167">Azure reservations resources</span></span>
|**<span data-ttu-id="5577c-168">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="5577c-168">For information about</span></span>**   |**<span data-ttu-id="5577c-169">Bitte lesen</span><span class="sxs-lookup"><span data-stu-id="5577c-169">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="5577c-170">Azure Reservations in CSP (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="5577c-170">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="5577c-171">Verkaufen von Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="5577c-171">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="5577c-172">Erwerb von Azure Reservations für Ihre Kunden im Partner-Dashboard</span><span class="sxs-lookup"><span data-stu-id="5577c-172">Purchasing Azure reservations for your customers in your Partner Dashboard</span></span>   |[<span data-ttu-id="5577c-173">Azure Reservations kaufen</span><span class="sxs-lookup"><span data-stu-id="5577c-173">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="5577c-174">Abrechnung für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="5577c-174">Billing for Azure reservations</span></span>   |[<span data-ttu-id="5577c-175">Abrechnung für Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="5577c-175">Billing for Azure reservations</span></span>](azure-reservations-billing.md)   |
| <span data-ttu-id="5577c-176">Verwalten von Azure Reservations in Ihrem Partner-Dashboard</span><span class="sxs-lookup"><span data-stu-id="5577c-176">Managing Azure reservations in your Partner Dashboard</span></span> | [<span data-ttu-id="5577c-177">Verwalten von Azure Reservations in Ihrem Partner-Dashboard</span><span class="sxs-lookup"><span data-stu-id="5577c-177">Managing Azure reservations in your Partner Dashboard</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="5577c-178">Erwerb von Azure Reservations im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="5577c-178">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="5577c-179">[Für virtuelle Maschinen mit Azure Reserved VM Instances im Voraus bezahlen](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="5577c-179">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="5577c-180">Verwalten von Azure Reservations im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="5577c-180">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="5577c-181">[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="5577c-181">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="5577c-182">Erwerb von Azure Reservations über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="5577c-182">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="5577c-183">[Erwerben Sie Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) in die Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="5577c-183">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) in the Partner Center developer documentation</span></span>



