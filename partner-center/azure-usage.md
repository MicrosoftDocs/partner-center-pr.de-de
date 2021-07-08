---
title: Azure-VM-Größe für die maximale Reservierungsnutzung
description: Erfahren Sie, wie Sie die Größe eines virtuellen Computers (VM) an die Computinganforderungen Ihrer Kunden anpassen, wenn Microsoft Azure reservierungen erwerben.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510192"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="90231-103">Microsoft Azure VM-Größe für die maximale Reservierungsnutzung</span><span class="sxs-lookup"><span data-stu-id="90231-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="90231-104">**Geeignete Rollen:** Administrator-Agent| Vertriebs-Agent</span><span class="sxs-lookup"><span data-stu-id="90231-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="90231-105">In diesem Artikel wird erläutert, wie Sie die Größe eines virtuellen Computers (VM) an die Computinganforderungen Ihrer Kunden anpassen, wenn Microsoft Azure reservierungen erwerben.</span><span class="sxs-lookup"><span data-stu-id="90231-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="90231-106">Dieser Artikel gilt nur für Partner im Cloud Solution Provider -Programm (CSP).</span><span class="sxs-lookup"><span data-stu-id="90231-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="90231-107">Kunden, die andere Abonnementtypen verwenden (z. B. nutzungsbasierte Bezahlung, Einzelabonnements, Microsoft-Kundenvereinbarung- oder Enterprise Agreement-Abonnements), sollten stattdessen diese Dokumentation zu Azure-Reservierungen [lesen.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="90231-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="90231-108">Ermitteln der VM-Größe für die Azure-Reservierung eines Kunden</span><span class="sxs-lookup"><span data-stu-id="90231-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="90231-109">Wenn Sie Microsoft Azure Reservierungen im Namen Ihrer Kunden kaufen, müssen Sie einen virtuellen Computer (VM) auswählen, der die Computinganforderungen des Kunden erfüllt.</span><span class="sxs-lookup"><span data-stu-id="90231-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="90231-110">Verwenden Sie eine der folgenden Methoden, um diese Informationen zu finden:</span><span class="sxs-lookup"><span data-stu-id="90231-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="90231-111">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="90231-111">Azure utilization API</span></span>
- <span data-ttu-id="90231-112">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="90231-112">The Azure portal</span></span>
- <span data-ttu-id="90231-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="90231-113">Azure PowerShell</span></span>
- <span data-ttu-id="90231-114">Die API für Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="90231-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="90231-115">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="90231-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="90231-116">Nachdem Sie eine Reservierung erworben haben, wird der Reservierungsrabatt auf virtuelle Computer mit den Attributen und Mengen der Reservierung automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="90231-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="90231-117">Sie müssen die Reservierung nicht einem virtuellen Computer zuweisen.</span><span class="sxs-lookup"><span data-stu-id="90231-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="90231-118">Reservierungsrabatte gelten nicht für klassische oder Werbe-VMs.</span><span class="sxs-lookup"><span data-stu-id="90231-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="90231-119">Um den Typ und die Größe des virtuellen Computers im Auftrag des Kunden korrekt identifizieren zu können, müssen Sie die unten aufgeführten Methoden verwenden, da der Typ des virtuellen Computers in der Partner Center-Abstimmungsdatei nicht richtig angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="90231-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="90231-120">Abrufen der VM-Größeninformationen mit der Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="90231-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="90231-121">Verwenden Sie den Wert für Diensttyp-Attribute aus additionalInfo in der API-Antwort, um die VM-Größe für den Kauf zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="90231-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="90231-122">Weitere Informationen finden Sie unter [Abrufen der Nutzungsdatensätze](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) eines Kunden für Azure in der [Partner Center-API.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="90231-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="90231-123">Abrufen der VM-Größeninformationen im Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="90231-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="90231-124">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="90231-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="90231-125">Suchen Sie den Kunden, der Azure-VM-Reservierungen erwerben möchte, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="90231-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="90231-126">Wählen **Microsoft Azure Verwaltungsportal** aus, um den Datensatz des Kunden in der Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="90231-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="90231-127">Wählen Sie **Virtuelle Computer** aus dem Portalmenü aus, und wählen Sie anschließend den virtuellen Computer aus, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="90231-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="90231-128">Suchen Sie auf der Detailseite des virtuellen Computers die Informationen zu Größe und Region, wie unten dargestellt, und verwenden Sie diese Informationen, um die Reservierung im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="90231-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informationen zur Größe und Region auf der Detailseite.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="90231-130">Abrufen der VM-Größeninformationen in Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="90231-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="90231-131">Verwenden Sie die Informationen in der Abbildung unten zum Abrufen von Standort und Größe des virtuellen Computers, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="90231-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM-Speicherort und -Größe.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="90231-133">Abrufen der VM-Größeninformationen in der Azure Resource Manager (ARM)-API</span><span class="sxs-lookup"><span data-stu-id="90231-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="90231-134">Rufen Sie mithilfe der ARMClient- oder der ARM-APIs den ARM-Client für den virtuellen Computer auf, für den Sie eine Reservierung erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="90231-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="90231-135">Der Aufruf gibt die Werte für **vmSize** und **location** zurück (s. u.).</span><span class="sxs-lookup"><span data-stu-id="90231-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize-Wert.":::
    :::image type="content" source="images/usage4.png" alt-text="location-Wert.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="90231-138">Überprüfen der Azure-VM-Nutzung und des Reservierungsrabatts</span><span class="sxs-lookup"><span data-stu-id="90231-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="90231-139">Nachdem Sie eine reservierte Azure-VM-Instanz im Auftrag eines Kunden erwerben, wird der Rabatt für die Vorauszahlung für VM-Speicherplatz automatisch auf die virtuellen Computer angewendet, die mit den Attributen und der Menge der Reservierung des Kunden übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="90231-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="90231-140">Sie können die Reservierungsnutzung des Kunden überprüfen und mithilfe einer der folgenden Methoden überprüfen, auf welche virtuellen Computer die Reservierungsrabatte angewendet werden:</span><span class="sxs-lookup"><span data-stu-id="90231-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="90231-141">Das Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="90231-141">The Azure portal</span></span>
- <span data-ttu-id="90231-142">Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="90231-142">Azure utilization API</span></span>

<span data-ttu-id="90231-143">Nachstehend finden Sie eine Anleitung für jede dieser Vorgehensweisen.</span><span class="sxs-lookup"><span data-stu-id="90231-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="90231-144">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="90231-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="90231-145">Überprüfen der Reservierungsnutzung des Kunden im Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="90231-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="90231-146">Navigieren Sie im Partner Center zur Seite **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="90231-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="90231-147">Suchen Sie den Kunden, dessen Reservierungsrabatt und Nutzung Sie überprüfen möchten, und wählen Sie dann den Pfeil nach unten aus, um die Informationen des Kunden zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="90231-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="90231-148">Wählen **Microsoft Azure Verwaltungsportal** aus, um den Datensatz des Kunden in der Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="90231-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="90231-149">Wählen Sie im Portalmenü **Reservierungen** aus, und wählen Sie anschließend die Reservierung aus, für die Sie die Nutzung überprüfen möchten.</span><span class="sxs-lookup"><span data-stu-id="90231-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="90231-150">Überprüfen Sie **auf der** Seite Übersicht das Auslastungsdiagramm der Reservierung, das zeigt, wie viel der Reservierung auf virtuelle Computer angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="90231-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="90231-151">Nutzungsdaten können um bis zu 8 Stunden verzögert sein.</span><span class="sxs-lookup"><span data-stu-id="90231-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="90231-152">a.</span><span class="sxs-lookup"><span data-stu-id="90231-152">a.</span></span> <span data-ttu-id="90231-153">Wenn die Nutzung der Reservierung 100 % beträgt, erzielt Ihr Kunde alle möglichen Einsparungen, die durch den Reservierungskauf erzielt werden können.</span><span class="sxs-lookup"><span data-stu-id="90231-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="90231-154">b.</span><span class="sxs-lookup"><span data-stu-id="90231-154">b.</span></span> <span data-ttu-id="90231-155">Wenn die Nutzung der Reservierung 0 % beträgt, wird der Rabatt nicht auf einen virtuellen Computer angewendet.</span><span class="sxs-lookup"><span data-stu-id="90231-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="90231-156">c.</span><span class="sxs-lookup"><span data-stu-id="90231-156">c.</span></span> <span data-ttu-id="90231-157">Wenn die Nutzung der Reservierung zwischen 1 % und 99 % liegt, gibt es nicht genutzte Vorteile.</span><span class="sxs-lookup"><span data-stu-id="90231-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="90231-158">Um diese Situation zu vermeiden, bestimmen Sie die richtige Vm-Größe, um die Computinganforderungen des Kunden zu unterstützen, bevor Sie den Kauf tätigen.</span><span class="sxs-lookup"><span data-stu-id="90231-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="90231-159">Überprüfen der Reservierungsnutzung des Kunden mit der Azure-Nutzungs-API</span><span class="sxs-lookup"><span data-stu-id="90231-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="90231-160">Nur die Azure-Nutzungs-API-zeigt an, auf welchen virtuellen Computer der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="90231-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="90231-161">Sie erhalten die Reservierungsnutzungsdaten mit der Azure-Nutzungs-API, um sicherzustellen, dass der Kunde den Reservierungsrabatt erhält, und um anzuzeigen, auf welche VMs (virtuelle Computer) der Rabatt angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="90231-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="90231-162">Vergleichen Sie Beispiel A mit Beispiel B, um zu sehen, wie Sie die Reservierungsnutzung eines Kunden überprüfen.</span><span class="sxs-lookup"><span data-stu-id="90231-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Beispiele für die Reservierungsnutzung.":::

- <span data-ttu-id="90231-164">Die reservationId identifiziert die Azure-Reservierung, die verwendet wurde, um den Rabatt auf den virtuellen Computer anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="90231-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="90231-165">consumptionMeter ist die MeterId für den virtuellen Computer, auf den der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="90231-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="90231-166">ReservationMeter zeigt $0 als Kosten an, da der Reservierungsrabatt angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="90231-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="90231-167">Weitere Informationen finden Sie unter [Abrufen der Nutzungsdatensätze](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) eines Kunden für Azure in der [Partner Center-API.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="90231-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="90231-168">Kosten für Software wie etwa für Microsoft Windows Server sind derzeit nicht im Preis einer VM-Reservierung enthalten und erscheinen als separate Positionen in den Bestelldaten und auf Ihrer Rechnung.</span><span class="sxs-lookup"><span data-stu-id="90231-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="90231-169">Wenn ein Kunde über die Azure-Hybridnutzungsvorteil verfügt, werden die Softwarekosten nicht angewendet.</span><span class="sxs-lookup"><span data-stu-id="90231-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="90231-170">Weitere Informationen finden Sie unter [Nicht in reservierten Azure-VM-Instanzen enthaltene Softwarekosten](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="90231-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="90231-171">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="90231-171">Next steps</span></span>

|<span data-ttu-id="90231-172">**Informationen über**</span><span class="sxs-lookup"><span data-stu-id="90231-172">**For information about**</span></span>   |<span data-ttu-id="90231-173">**Artikel**</span><span class="sxs-lookup"><span data-stu-id="90231-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="90231-174">Azure-Reservierungen in CSP (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="90231-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="90231-175">Verkaufen von Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="90231-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="90231-176">Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="90231-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="90231-177">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="90231-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="90231-178">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="90231-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="90231-179">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="90231-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="90231-180">Erwerb von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="90231-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="90231-181">[Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="90231-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="90231-182">Verwalten von Azure-Reservierungen im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="90231-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="90231-183">[Verwalten von reservierten VM-Instanzen](/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe</span><span class="sxs-lookup"><span data-stu-id="90231-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="90231-184">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="90231-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="90231-185">[Kaufen von Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="90231-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="90231-186">Erteilen sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen aus einem Abonnement zu erwerben, das Sie für sie erworben haben.</span><span class="sxs-lookup"><span data-stu-id="90231-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="90231-187">Erteilen der Berechtigung für Kunden, ihre eigenen Azure-Reservierungen zu erwerben</span><span class="sxs-lookup"><span data-stu-id="90231-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |