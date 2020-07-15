---
title: Azure-VM-Größenanpassung für die maximale Reservierungs Nutzung
ms.topic: article
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie Sie die Größe eines virtuellen Computers (VM) mit den computinganforderungen ihrer Kunden skalimachen, wenn Sie Microsoft Azure Reservierungen für diese Computer erwerben.
author: BillLinzbach
ms.author: BillLi
keywords: Azure, Reservierungen, VM, verwalten, Nutzung, Größe
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 00da6723fc8aa4a5b3f1e0f747cb63acc1a504a8
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377654"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="3fed4-104">Microsoft Azure VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="3fed4-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="3fed4-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="3fed4-105">**Applies to**</span></span>

- <span data-ttu-id="3fed4-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="3fed4-106">Partner Center</span></span>
- <span data-ttu-id="3fed4-107">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-107">Azure portal</span></span>
- <span data-ttu-id="3fed4-108">Partner im CSP</span><span class="sxs-lookup"><span data-stu-id="3fed4-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="3fed4-109">Ermitteln der VM-Größe für die Azure-Reservierung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="3fed4-109">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="3fed4-110">Beim Kauf von Microsoft Azure Reservierungen im Auftrag ihrer Kunden müssen Sie einen virtuellen Computer (VM) auswählen, um die Anforderungen des Kunden zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="3fed4-111">Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:</span><span class="sxs-lookup"><span data-stu-id="3fed4-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="3fed4-112">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="3fed4-112">Azure utilization API</span></span>
- <span data-ttu-id="3fed4-113">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-113">The Azure portal</span></span>
- <span data-ttu-id="3fed4-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3fed4-114">Azure PowerShell</span></span>
- <span data-ttu-id="3fed4-115">Die API für Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="3fed4-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="3fed4-116">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="3fed4-117">Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="3fed4-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="3fed4-118">Sie müssen die Reservierung nicht einem virtuellen Computer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="3fed4-119">Reservierungs Rabatte gelten nicht für klassische oder Werbe-VMS.</span><span class="sxs-lookup"><span data-stu-id="3fed4-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="3fed4-120">Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3fed4-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="3fed4-121">Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="3fed4-121">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="3fed4-122">Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="3fed4-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="3fed4-123">Weitere Informationen finden Sie unter Ermitteln der [Auslastungs Datensätze eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="3fed4-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="3fed4-124">Abrufen der VM-Größeninformationen im Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-124">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="3fed4-125">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="3fed4-125">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="3fed4-126">Suchen Sie den Kunden, der Azure-VM-Reservierungen erwerben möchte, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="3fed4-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="3fed4-127">Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="3fed4-128">Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="3fed4-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="3fed4-129">Suchen Sie auf der Detailseite des virtuellen Computers die Größe und Regions Informationen, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung in Partner Center zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="3fed4-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informationen zu Größe und Region auf der Detailseite":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="3fed4-131">Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3fed4-131">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="3fed4-132">Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="3fed4-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM-Standort und Größe":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="3fed4-134">Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API</span><span class="sxs-lookup"><span data-stu-id="3fed4-134">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="3fed4-135">Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="3fed4-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="3fed4-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="3fed4-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="3fed4-137">Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).</span><span class="sxs-lookup"><span data-stu-id="3fed4-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmsize-Wert":::
    :::image type="content" source="images/usage4.png" alt-text="Location-Wert":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="3fed4-140">Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts</span><span class="sxs-lookup"><span data-stu-id="3fed4-140">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="3fed4-141">Nachdem Sie im Auftrag eines Kunden eine reservierte Azure-VM-Instanz erworben haben, wird der Rabatt für die Zahlung von VM-Speicherplatz im Voraus automatisch auf die virtuellen Computer angewendet, die den Attributen und der Menge der Kunden Reservierung entsprechen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-141">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="3fed4-142">Mithilfe einer der folgenden Methoden können Sie die Reservierungs Nutzung des Kunden überprüfen und überprüfen, auf welche virtuellen Computer die Reservierungs Rabatte angewendet werden:</span><span class="sxs-lookup"><span data-stu-id="3fed4-142">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="3fed4-143">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-143">The Azure portal</span></span>
- <span data-ttu-id="3fed4-144">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="3fed4-144">Azure utilization API</span></span>

<span data-ttu-id="3fed4-145">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-145">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="3fed4-146">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="3fed4-146">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="3fed4-147">Überprüfen Sie die Reservierungs Nutzung des Kunden im Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-147">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="3fed4-148">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="3fed4-148">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="3fed4-149">Suchen Sie nach dem Kunden, dessen Reservierungs Rabatt und deren Nutzung Sie überprüfen möchten, und klicken Sie dann auf den Pfeil nach unten, um die Kundeninformationen zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="3fed4-149">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="3fed4-150">Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-150">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="3fed4-151">Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.</span><span class="sxs-lookup"><span data-stu-id="3fed4-151">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="3fed4-152">Überprüfen Sie auf der Seite **Übersicht** das Auslastungs Diagramm der Reservierung, das anzeigt, wie viel der Reservierung auf virtuelle Computer angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="3fed4-152">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3fed4-153">Nutzungsdaten können um bis zu 8 Stunden verzögert sein.</span><span class="sxs-lookup"><span data-stu-id="3fed4-153">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="3fed4-154">a.</span><span class="sxs-lookup"><span data-stu-id="3fed4-154">a.</span></span> <span data-ttu-id="3fed4-155">Wenn die Nutzung der Reservierung 100% beträgt, erhält der Kunde alle möglichen Einsparungen, die der reservierte Kauf bereitstellen kann.</span><span class="sxs-lookup"><span data-stu-id="3fed4-155">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="3fed4-156">b.</span><span class="sxs-lookup"><span data-stu-id="3fed4-156">b.</span></span> <span data-ttu-id="3fed4-157">Wenn die Nutzung der Reservierung 0% beträgt, wird der Rabatt nicht auf einen virtuellen Computer angewendet.</span><span class="sxs-lookup"><span data-stu-id="3fed4-157">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="3fed4-158">c.</span><span class="sxs-lookup"><span data-stu-id="3fed4-158">c.</span></span> <span data-ttu-id="3fed4-159">Wenn die Reservierungs Nutzung zwischen 1% und 99% liegt, gibt es nicht genutzte Vorteile.</span><span class="sxs-lookup"><span data-stu-id="3fed4-159">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="3fed4-160">Um dieses Problem zu vermeiden, sollten Sie die richtige VM-Größe festlegen, um die computingressourcen der Kunden vor dem Erwerb zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="3fed4-160">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="3fed4-161">Überprüfen der Reservierungs Nutzung des Kunden mit der Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="3fed4-161">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="3fed4-162">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="3fed4-162">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="3fed4-163">Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="3fed4-163">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="3fed4-164">Vergleichen Sie Beispiel a mit Beispiel B, um zu erfahren, wie Sie die Reservierungs Nutzung eines Kunden überprüfen.</span><span class="sxs-lookup"><span data-stu-id="3fed4-164">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Beispiele für die Reservierungsnutzung":::

- <span data-ttu-id="3fed4-166">Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="3fed4-166">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="3fed4-167">consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="3fed4-167">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="3fed4-168">ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="3fed4-168">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="3fed4-169">Weitere Informationen finden Sie unter Ermitteln der [Auslastungs Datensätze eines Kunden für Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="3fed4-169">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="3fed4-170">Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung.</span><span class="sxs-lookup"><span data-stu-id="3fed4-170">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="3fed4-171">Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet.</span><span class="sxs-lookup"><span data-stu-id="3fed4-171">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="3fed4-172">Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="3fed4-172">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="3fed4-173">Ressourcen zu Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="3fed4-173">Azure reservations resources</span></span>

|<span data-ttu-id="3fed4-174">**Informationen über**</span><span class="sxs-lookup"><span data-stu-id="3fed4-174">**For information about**</span></span>   |<span data-ttu-id="3fed4-175">**Artikel**</span><span class="sxs-lookup"><span data-stu-id="3fed4-175">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="3fed4-176">Azure-Reservierungen in CSP (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="3fed4-176">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="3fed4-177">Verkaufen von Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="3fed4-177">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="3fed4-178">Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="3fed4-178">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="3fed4-179">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="3fed4-179">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="3fed4-180">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="3fed4-180">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="3fed4-181">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="3fed4-181">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="3fed4-182">Erwerb von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-182">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="3fed4-183">[Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="3fed4-183">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="3fed4-184">Verwalten von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3fed4-184">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="3fed4-185">[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="3fed4-185">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="3fed4-186">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="3fed4-186">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="3fed4-187">[Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="3fed4-187">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="3fed4-188">Erteilen von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von einem Abonnement zu erwerben, das Sie für Sie erworben haben.</span><span class="sxs-lookup"><span data-stu-id="3fed4-188">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="3fed4-189">Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="3fed4-189">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
