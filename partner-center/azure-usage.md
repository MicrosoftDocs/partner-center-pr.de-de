---
title: Azure-VM-Größe für die maximale Reservierungsnutzung
description: Erfahren Sie, wie Sie die Größe eines virtuellen Computers (VM) mit den computinganforderungen ihrer Kunden skalimachen, wenn Sie Microsoft Azure Reservierungen für diese Computer erwerben.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 226ebd27b4ca4cdef56ce833a58a10bed89f8056
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534946"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="e4c62-103">Microsoft Azure VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="e4c62-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="e4c62-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="e4c62-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e4c62-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="e4c62-105">Admin agent</span></span>
- <span data-ttu-id="e4c62-106">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="e4c62-106">Sales agent</span></span>

<span data-ttu-id="e4c62-107">In diesem Artikel wird erläutert, wie Sie die Größe eines virtuellen Computers (VM) mit den computinganforderungen ihrer Kunden anpassen, wenn Sie Microsoft Azure Reservierungen für diese Computer erwerben.</span><span class="sxs-lookup"><span data-stu-id="e4c62-107">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="e4c62-108">Dieser Artikel gilt nur für Partner im CSP-Programm (Cloud Solution Provider).</span><span class="sxs-lookup"><span data-stu-id="e4c62-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="e4c62-109">Kunden, die andere Abonnementtypen (z. b. Pay-as-you-go, individuelle, Microsoft-Kunden Vereinbarung oder Konzernvertrag Abonnements) verwenden, sollten stattdessen [diese Azure-Reservierungs Dokumentation](/azure/cost-management-billing/reservations)lesen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="e4c62-110">Ermitteln der VM-Größe für die Azure-Reservierung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="e4c62-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="e4c62-111">Beim Kauf von Microsoft Azure Reservierungen im Auftrag ihrer Kunden müssen Sie einen virtuellen Computer (VM) auswählen, um die Anforderungen des Kunden zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="e4c62-112">Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:</span><span class="sxs-lookup"><span data-stu-id="e4c62-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="e4c62-113">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="e4c62-113">Azure utilization API</span></span>
- <span data-ttu-id="e4c62-114">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="e4c62-114">The Azure portal</span></span>
- <span data-ttu-id="e4c62-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e4c62-115">Azure PowerShell</span></span>
- <span data-ttu-id="e4c62-116">Die API für Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="e4c62-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="e4c62-117">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="e4c62-118">Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="e4c62-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="e4c62-119">Sie müssen die Reservierung nicht einem virtuellen Computer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="e4c62-120">Reservierungs Rabatte gelten nicht für klassische oder Werbe-VMS.</span><span class="sxs-lookup"><span data-stu-id="e4c62-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="e4c62-121">Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e4c62-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="e4c62-122">Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="e4c62-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="e4c62-123">Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="e4c62-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="e4c62-124">Weitere Informationen finden Sie unter Ermitteln der [Auslastungs Datensätze eines Kunden für Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="e4c62-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="e4c62-125">Abrufen der VM-Größeninformationen im Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="e4c62-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e4c62-126">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="e4c62-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e4c62-127">Suchen Sie den Kunden, der Azure-VM-Reservierungen erwerben möchte, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="e4c62-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e4c62-128">Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="e4c62-129">Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="e4c62-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="e4c62-130">Suchen Sie auf der Detailseite des virtuellen Computers die Größe und Regions Informationen, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung in Partner Center zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="e4c62-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informationen zu Größe und Region auf der Detailseite":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="e4c62-132">Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e4c62-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="e4c62-133">Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="e4c62-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM-Standort und Größe":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="e4c62-135">Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API</span><span class="sxs-lookup"><span data-stu-id="e4c62-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="e4c62-136">Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="e4c62-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="e4c62-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e4c62-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="e4c62-138">Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).</span><span class="sxs-lookup"><span data-stu-id="e4c62-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmsize-Wert":::
    :::image type="content" source="images/usage4.png" alt-text="Location-Wert":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="e4c62-141">Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts</span><span class="sxs-lookup"><span data-stu-id="e4c62-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="e4c62-142">Nachdem Sie im Auftrag eines Kunden eine reservierte Azure-VM-Instanz erworben haben, wird der Rabatt für die Zahlung von VM-Speicherplatz im Voraus automatisch auf die virtuellen Computer angewendet, die den Attributen und der Menge der Kunden Reservierung entsprechen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="e4c62-143">Mithilfe einer der folgenden Methoden können Sie die Reservierungs Nutzung des Kunden überprüfen und überprüfen, auf welche virtuellen Computer die Reservierungs Rabatte angewendet werden:</span><span class="sxs-lookup"><span data-stu-id="e4c62-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="e4c62-144">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="e4c62-144">The Azure portal</span></span>
- <span data-ttu-id="e4c62-145">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="e4c62-145">Azure utilization API</span></span>

<span data-ttu-id="e4c62-146">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="e4c62-147">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="e4c62-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="e4c62-148">Überprüfen Sie die Reservierungs Nutzung des Kunden im Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="e4c62-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e4c62-149">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="e4c62-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e4c62-150">Suchen Sie nach dem Kunden, dessen Reservierungs Rabatt und deren Nutzung Sie überprüfen möchten, und klicken Sie dann auf den Pfeil nach unten, um die Kundeninformationen zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="e4c62-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e4c62-151">Wählen Sie **Microsoft Azure-Verwaltungsportal** aus, um den Datensatz des Kunden im Azure-Portal zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="e4c62-152">Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.</span><span class="sxs-lookup"><span data-stu-id="e4c62-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="e4c62-153">Überprüfen Sie auf der Seite **Übersicht** das Auslastungs Diagramm der Reservierung, das anzeigt, wie viel der Reservierung auf virtuelle Computer angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="e4c62-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e4c62-154">Nutzungsdaten können um bis zu 8 Stunden verzögert sein.</span><span class="sxs-lookup"><span data-stu-id="e4c62-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="e4c62-155">a.</span><span class="sxs-lookup"><span data-stu-id="e4c62-155">a.</span></span> <span data-ttu-id="e4c62-156">Wenn die Nutzung der Reservierung 100% beträgt, erhält der Kunde alle möglichen Einsparungen, die der reservierte Kauf bereitstellen kann.</span><span class="sxs-lookup"><span data-stu-id="e4c62-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="e4c62-157">b.</span><span class="sxs-lookup"><span data-stu-id="e4c62-157">b.</span></span> <span data-ttu-id="e4c62-158">Wenn die Nutzung der Reservierung 0% beträgt, wird der Rabatt nicht auf einen virtuellen Computer angewendet.</span><span class="sxs-lookup"><span data-stu-id="e4c62-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="e4c62-159">c.</span><span class="sxs-lookup"><span data-stu-id="e4c62-159">c.</span></span> <span data-ttu-id="e4c62-160">Wenn die Reservierungs Nutzung zwischen 1% und 99% liegt, gibt es nicht genutzte Vorteile.</span><span class="sxs-lookup"><span data-stu-id="e4c62-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="e4c62-161">Um dieses Problem zu vermeiden, sollten Sie die richtige VM-Größe festlegen, um die computingressourcen der Kunden vor dem Erwerb zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e4c62-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="e4c62-162">Überprüfen der Reservierungs Nutzung des Kunden mit der Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="e4c62-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="e4c62-163">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="e4c62-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="e4c62-164">Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="e4c62-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="e4c62-165">Vergleichen Sie Beispiel a mit Beispiel B, um zu erfahren, wie Sie die Reservierungs Nutzung eines Kunden überprüfen.</span><span class="sxs-lookup"><span data-stu-id="e4c62-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Beispiele für die Reservierungsnutzung":::

- <span data-ttu-id="e4c62-167">Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="e4c62-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="e4c62-168">consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="e4c62-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="e4c62-169">ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="e4c62-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="e4c62-170">Weitere Informationen finden Sie unter Ermitteln der [Auslastungs Datensätze eines Kunden für Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in der [Partner Center-API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="e4c62-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="e4c62-171">Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung.</span><span class="sxs-lookup"><span data-stu-id="e4c62-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="e4c62-172">Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet.</span><span class="sxs-lookup"><span data-stu-id="e4c62-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="e4c62-173">Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="e4c62-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="e4c62-174">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="e4c62-174">Next steps</span></span>

|<span data-ttu-id="e4c62-175">**Informationen über**</span><span class="sxs-lookup"><span data-stu-id="e4c62-175">**For information about**</span></span>   |<span data-ttu-id="e4c62-176">**Artikel**</span><span class="sxs-lookup"><span data-stu-id="e4c62-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="e4c62-177">Azure-Reservierungen in CSP (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="e4c62-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="e4c62-178">Verkaufen von Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="e4c62-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="e4c62-179">Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="e4c62-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="e4c62-180">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="e4c62-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="e4c62-181">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="e4c62-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="e4c62-182">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="e4c62-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="e4c62-183">Erwerb von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="e4c62-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="e4c62-184">[Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="e4c62-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="e4c62-185">Verwalten von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="e4c62-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="e4c62-186">[Verwalten von reservierten VM-Instanzen](/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="e4c62-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="e4c62-187">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="e4c62-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="e4c62-188">[Kaufen von Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="e4c62-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="e4c62-189">Erteilen von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von einem Abonnement zu erwerben, das Sie für Sie erworben haben.</span><span class="sxs-lookup"><span data-stu-id="e4c62-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="e4c62-190">Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="e4c62-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |