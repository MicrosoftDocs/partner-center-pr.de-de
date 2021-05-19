---
title: Migrieren von Kaizala Pro-Abonnements zu Microsoft 365
description: Erfahren Sie, wie Sie Kaizala Pro-Abonnements zu Microsoft 365- oder Office 365-Versionen migrieren. Weitere Informationen zum Übergang Ihrer Kunden finden Sie in diesem Artikel.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146424"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="2e04b-104">Migrieren eigenständiger Kaizala Pro-Abonnements zu Microsoft 365- oder Office 365-Versionen</span><span class="sxs-lookup"><span data-stu-id="2e04b-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="2e04b-105">**Geeignete Rollen:** Vertriebs-Agent</span><span class="sxs-lookup"><span data-stu-id="2e04b-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="2e04b-106">Ab dem 1. Juli 2020 beendet Microsoft den Umsatz des eigenständigen Kaizala Pro-Diensts.</span><span class="sxs-lookup"><span data-stu-id="2e04b-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="2e04b-107">Kunden können nach diesem Datum keine neuen Kaizala Pro-Abonnements mehr erwerben, und vorhandene Kaizala Pro-Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="2e04b-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="2e04b-108">Um die Kontinuität für Kunden sicherzustellen, sollten Sie Kunden mit ablaufenden eigenständigen Kaizala Pro-Abonnements auf eine unterstützte SKU-Option umsteigen, die unten aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="2e04b-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="2e04b-109">Es wird empfohlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienstausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="2e04b-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="2e04b-110">Wenn Sie die API verwenden (entweder DIE API oder Partner Center), können Sie ablaufende Abonnements ermitteln, indem Sie das Enddatum des Abonnements zusammen mit der Eigenschaft für die automatische Verlängerung auf FALSE festlegen: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="2e04b-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="2e04b-111">Die E4-Abonnements werden `auto renew=False` am 1. Juli 2020 auf festgelegt.</span><span class="sxs-lookup"><span data-stu-id="2e04b-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="2e04b-112">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="2e04b-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="2e04b-113">Kaizala Pro – eigenständige Ersetzungspläne</span><span class="sxs-lookup"><span data-stu-id="2e04b-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="2e04b-114">Mit den neuen Plänen können Ihre Kunden neuere Features und Funktionen in Microsoft 365 nutzen.</span><span class="sxs-lookup"><span data-stu-id="2e04b-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="2e04b-115">Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2e04b-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="2e04b-116">[**Microsoft 365 für Unternehmen,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="2e04b-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="2e04b-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="2e04b-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="2e04b-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="2e04b-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="2e04b-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="2e04b-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="2e04b-120">[**Microsoft 365 für Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="2e04b-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="2e04b-121">Microsoft 365 F3 (ehemals Microsoft 365 F1) und Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="2e04b-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="2e04b-122">[**Microsoft 365 für Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="2e04b-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="2e04b-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="2e04b-123">Office 365 E1</span></span>
   - <span data-ttu-id="2e04b-124">Microsoft 365 E3 and Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="2e04b-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="2e04b-125">Microsoft 365 E5 und Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="2e04b-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="2e04b-126">[**Microsoft 365 für Bildungseinrichtungen,**](https://www.microsoft.com/education/buy-license/microsoft365)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="2e04b-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="2e04b-127">Microsoft 365 A1 und Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="2e04b-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="2e04b-128">Microsoft 365 A3 und Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="2e04b-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="2e04b-129">Microsoft 365 A5 und Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="2e04b-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2e04b-130">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="2e04b-130">Transition customers to new product plans</span></span>

<span data-ttu-id="2e04b-131">Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an.</span><span class="sxs-lookup"><span data-stu-id="2e04b-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="2e04b-132">In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren.</span><span class="sxs-lookup"><span data-stu-id="2e04b-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="2e04b-133">Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:</span><span class="sxs-lookup"><span data-stu-id="2e04b-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="2e04b-134">A.</span><span class="sxs-lookup"><span data-stu-id="2e04b-134">A.</span></span> <span data-ttu-id="2e04b-135">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="2e04b-135">Purchase the new subscription</span></span>

<span data-ttu-id="2e04b-136">B.</span><span class="sxs-lookup"><span data-stu-id="2e04b-136">B.</span></span> <span data-ttu-id="2e04b-137">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="2e04b-137">Reassign current user licenses</span></span>

<span data-ttu-id="2e04b-138">C.</span><span class="sxs-lookup"><span data-stu-id="2e04b-138">C.</span></span> <span data-ttu-id="2e04b-139">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="2e04b-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="2e04b-140">Migrieren Ihrer Kunden zu neuen Plänen</span><span class="sxs-lookup"><span data-stu-id="2e04b-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="2e04b-141">A.</span><span class="sxs-lookup"><span data-stu-id="2e04b-141">A.</span></span> <span data-ttu-id="2e04b-142">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="2e04b-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="2e04b-143">Um das neue Abonnement zu erwerben, wählen Sie im **Menü Partner Center** die Option **Kunden** aus, wählen Sie den Kunden aus, den Sie verschieben möchten, und wählen Sie dann **Abonnements hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="2e04b-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="2e04b-144">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="2e04b-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="2e04b-145">Ihr Kunde sollte nun sowohl über alte als auch über neue Abonnements, das alte eigenständige Kaizala Pro-Abonnement und das neue Zielabonnement verfügen, z. B. Option 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="2e04b-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="2e04b-146">B.</span><span class="sxs-lookup"><span data-stu-id="2e04b-146">B.</span></span> <span data-ttu-id="2e04b-147">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="2e04b-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="2e04b-148">Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen des Kunden im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="2e04b-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="2e04b-149">Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="2e04b-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="2e04b-150">Um die Benutzerlizenz neu zuzuweisen, wählen Sie den neu zuzuweisenden Benutzer und dann **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="2e04b-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="2e04b-151">Aktivieren Sie **auf der Seite** Lizenzen verwalten das Kontrollkästchen Kaizala Pro Standalone license (Kaizala Pro Standalone-Lizenz), und wählen Sie einen neuen Serviceplan für das Abonnement aus, in das der Kunde um zieht.</span><span class="sxs-lookup"><span data-stu-id="2e04b-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="2e04b-152">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="2e04b-152">Select **Submit**.</span></span> <span data-ttu-id="2e04b-153">Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="2e04b-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="2e04b-154">Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.</span><span class="sxs-lookup"><span data-stu-id="2e04b-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="2e04b-155">C.</span><span class="sxs-lookup"><span data-stu-id="2e04b-155">C.</span></span> <span data-ttu-id="2e04b-156">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="2e04b-156">Cancel old subscription</span></span>

<span data-ttu-id="2e04b-157">Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.</span><span class="sxs-lookup"><span data-stu-id="2e04b-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="2e04b-158">Wählen Sie **Partner Center** Menü Kunden **aus.**</span><span class="sxs-lookup"><span data-stu-id="2e04b-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2e04b-159">Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.</span><span class="sxs-lookup"><span data-stu-id="2e04b-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="2e04b-160">Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.</span><span class="sxs-lookup"><span data-stu-id="2e04b-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="2e04b-161">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="2e04b-161">Select **Submit**.</span></span>

<span data-ttu-id="2e04b-162">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="2e04b-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="2e04b-163">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="2e04b-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2e04b-164">Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="2e04b-164">The customer incurs no additional costs for the old subscription.</span></span>
