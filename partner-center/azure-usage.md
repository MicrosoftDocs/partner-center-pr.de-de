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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="a707a-104">Microsoft Azure VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="a707a-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="a707a-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="a707a-105">**Applies to**</span></span>

- <span data-ttu-id="a707a-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="a707a-106">Partner Center</span></span>
- <span data-ttu-id="a707a-107">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="a707a-107">Azure portal</span></span>
- <span data-ttu-id="a707a-108">Partner im CSP</span><span class="sxs-lookup"><span data-stu-id="a707a-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="a707a-109">Determine the VM size for a customer's Azure reservation</span><span class="sxs-lookup"><span data-stu-id="a707a-109">Determine the VM size for a customer's Azure reservation</span></span> 

<span data-ttu-id="a707a-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span><span class="sxs-lookup"><span data-stu-id="a707a-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="a707a-111">Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:</span><span class="sxs-lookup"><span data-stu-id="a707a-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="a707a-112">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="a707a-112">Azure utilization API</span></span>
- <span data-ttu-id="a707a-113">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="a707a-113">The Azure portal</span></span>
- <span data-ttu-id="a707a-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a707a-114">Azure PowerShell</span></span>
- <span data-ttu-id="a707a-115">Die API für Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="a707a-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="a707a-116">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="a707a-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="a707a-117">Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="a707a-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="a707a-118">You don't need to assign the reservation to a VM.</span><span class="sxs-lookup"><span data-stu-id="a707a-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="a707a-119">Reservation discounts don't apply to classic or promotional VMs.</span><span class="sxs-lookup"><span data-stu-id="a707a-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a707a-120">Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="a707a-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="a707a-121">**Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API**</span><span class="sxs-lookup"><span data-stu-id="a707a-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="a707a-122">Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="a707a-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="a707a-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="a707a-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="a707a-124">**Abrufen der VM-Größeninformationen im Microsoft Azure-Portal**</span><span class="sxs-lookup"><span data-stu-id="a707a-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="a707a-125">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="a707a-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="a707a-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span><span class="sxs-lookup"><span data-stu-id="a707a-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="a707a-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="a707a-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="a707a-128">Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="a707a-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="a707a-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a707a-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Informationen zu Größe und Region auf der Detailseite](images/usage1.png)

<span data-ttu-id="a707a-131">**Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell**</span><span class="sxs-lookup"><span data-stu-id="a707a-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="a707a-132">Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="a707a-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![VM-Standort und Größe](images/usage2.png)

<span data-ttu-id="a707a-134">**Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API**</span><span class="sxs-lookup"><span data-stu-id="a707a-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="a707a-135">Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="a707a-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="a707a-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a707a-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="a707a-137">Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).</span><span class="sxs-lookup"><span data-stu-id="a707a-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="a707a-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="a707a-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span></span>

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="a707a-139">Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts</span><span class="sxs-lookup"><span data-stu-id="a707a-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="a707a-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span><span class="sxs-lookup"><span data-stu-id="a707a-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="a707a-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span><span class="sxs-lookup"><span data-stu-id="a707a-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="a707a-142">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="a707a-142">The Azure portal</span></span>
- <span data-ttu-id="a707a-143">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="a707a-143">Azure utilization API</span></span>

<span data-ttu-id="a707a-144">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="a707a-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="a707a-145">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="a707a-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="a707a-146">Verify the customer's reservation usage in the Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="a707a-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="a707a-147">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="a707a-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="a707a-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span><span class="sxs-lookup"><span data-stu-id="a707a-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="a707a-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="a707a-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="a707a-150">Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.</span><span class="sxs-lookup"><span data-stu-id="a707a-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="a707a-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span><span class="sxs-lookup"><span data-stu-id="a707a-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a707a-152">Nutzungsdaten können um bis zu 8 Stunden verzögert sein.</span><span class="sxs-lookup"><span data-stu-id="a707a-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="a707a-153">a.</span><span class="sxs-lookup"><span data-stu-id="a707a-153">a.</span></span> <span data-ttu-id="a707a-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span><span class="sxs-lookup"><span data-stu-id="a707a-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="a707a-155">b.</span><span class="sxs-lookup"><span data-stu-id="a707a-155">b.</span></span> <span data-ttu-id="a707a-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span><span class="sxs-lookup"><span data-stu-id="a707a-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="a707a-157">c.</span><span class="sxs-lookup"><span data-stu-id="a707a-157">c.</span></span> <span data-ttu-id="a707a-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span><span class="sxs-lookup"><span data-stu-id="a707a-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="a707a-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span><span class="sxs-lookup"><span data-stu-id="a707a-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="a707a-160">Verify the customer's reservation usage with the Azure utilization API</span><span class="sxs-lookup"><span data-stu-id="a707a-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="a707a-161">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="a707a-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="a707a-162">Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="a707a-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="a707a-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span><span class="sxs-lookup"><span data-stu-id="a707a-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

![Beispiele für die Reservierungsnutzung](images/usage5.png)

- <span data-ttu-id="a707a-165">Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="a707a-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="a707a-166">consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="a707a-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="a707a-167">ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="a707a-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="a707a-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="a707a-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="a707a-169">Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung.</span><span class="sxs-lookup"><span data-stu-id="a707a-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="a707a-170">Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet.</span><span class="sxs-lookup"><span data-stu-id="a707a-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="a707a-171">Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="a707a-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="a707a-172">Ressourcen zu Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="a707a-172">Azure reservations resources</span></span>

|<span data-ttu-id="a707a-173">**Weitere Informationen zu**</span><span class="sxs-lookup"><span data-stu-id="a707a-173">**For information about**</span></span>   |<span data-ttu-id="a707a-174">**Bitte lesen**</span><span class="sxs-lookup"><span data-stu-id="a707a-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="a707a-175">Azure-Reservierungen in CSP (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="a707a-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="a707a-176">Verkaufen von Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="a707a-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="a707a-177">Erwerb von Azure-Reservierungen für Ihre Kunden im Partner Center</span><span class="sxs-lookup"><span data-stu-id="a707a-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="a707a-178">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="a707a-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="a707a-179">Verwalten von Azure-Reservierungen im Partner Center</span><span class="sxs-lookup"><span data-stu-id="a707a-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="a707a-180">Verwalten von Azure-Reservierungen im Partner Center</span><span class="sxs-lookup"><span data-stu-id="a707a-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="a707a-181">Erwerb von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="a707a-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="a707a-182">[Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="a707a-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="a707a-183">Verwalten von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="a707a-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="a707a-184">[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="a707a-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="a707a-185">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="a707a-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="a707a-186">[Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="a707a-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
