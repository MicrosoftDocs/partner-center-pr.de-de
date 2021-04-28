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
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172403"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="96ee2-104">Migrieren eigenständiger Kaizala Pro-Abonnements zu Microsoft 365- oder Office 365-Versionen</span><span class="sxs-lookup"><span data-stu-id="96ee2-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="96ee2-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="96ee2-105">**Appropriate roles**</span></span>

- <span data-ttu-id="96ee2-106">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="96ee2-106">Sales agent</span></span>

<span data-ttu-id="96ee2-107">Ab dem 1. Juli 2020 beendet Microsoft den Umsatz des eigenständigen Kaizala Pro-Diensts.</span><span class="sxs-lookup"><span data-stu-id="96ee2-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="96ee2-108">Kunden können nach diesem Datum keine neuen Kaizala Pro-Abonnements mehr erwerben, und vorhandene Kaizala Pro-Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="96ee2-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="96ee2-109">Um die Kontinuität für Kunden sicherzustellen, sollten Sie Kunden mit ablaufenden eigenständigen Kaizala Pro-Abonnements auf eine unterstützte SKU-Option umsteigen, die unten aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="96ee2-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="96ee2-110">Es wird empfohlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienstausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="96ee2-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="96ee2-111">Wenn Sie die API verwenden (entweder MIT oder Partner Center), können Sie ablaufende Abonnements ermitteln, indem Sie das Enddatum des Abonnements zusammen mit der Eigenschaft für die automatische Verlängerung auf FALSE festlegen: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="96ee2-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="96ee2-112">Die E4-Abonnements werden `auto renew=False` am 1. Juli 2020 auf festgelegt.</span><span class="sxs-lookup"><span data-stu-id="96ee2-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="96ee2-113">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="96ee2-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="96ee2-114">Kaizala Pro – eigenständige Ersetzungspläne</span><span class="sxs-lookup"><span data-stu-id="96ee2-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="96ee2-115">Mit den neuen Plänen können Ihre Kunden neuere Features und Funktionen in Microsoft 365 nutzen.</span><span class="sxs-lookup"><span data-stu-id="96ee2-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="96ee2-116">Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="96ee2-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="96ee2-117">[**Microsoft 365 für Unternehmen,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="96ee2-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="96ee2-118">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="96ee2-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="96ee2-119">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="96ee2-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="96ee2-120">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="96ee2-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="96ee2-121">[**Microsoft 365 für Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="96ee2-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="96ee2-122">Microsoft 365 F3 (ehemals Microsoft 365 F1) und Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="96ee2-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="96ee2-123">[**Microsoft 365 für Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="96ee2-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="96ee2-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="96ee2-124">Office 365 E1</span></span>
   - <span data-ttu-id="96ee2-125">Microsoft 365 E3 and Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="96ee2-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="96ee2-126">Microsoft 365 E5 und Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="96ee2-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="96ee2-127">[**Microsoft 365 für Bildungseinrichtungen,**](https://www.microsoft.com/education/buy-license/microsoft365)einschließlich:</span><span class="sxs-lookup"><span data-stu-id="96ee2-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="96ee2-128">Microsoft 365 A1 und Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="96ee2-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="96ee2-129">Microsoft 365 A3 und Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="96ee2-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="96ee2-130">Microsoft 365 A5 und Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="96ee2-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="96ee2-131">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="96ee2-131">Transition customers to new product plans</span></span>

<span data-ttu-id="96ee2-132">Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an.</span><span class="sxs-lookup"><span data-stu-id="96ee2-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="96ee2-133">In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren.</span><span class="sxs-lookup"><span data-stu-id="96ee2-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="96ee2-134">Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:</span><span class="sxs-lookup"><span data-stu-id="96ee2-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="96ee2-135">A.</span><span class="sxs-lookup"><span data-stu-id="96ee2-135">A.</span></span> <span data-ttu-id="96ee2-136">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="96ee2-136">Purchase the new subscription</span></span>

<span data-ttu-id="96ee2-137">B.</span><span class="sxs-lookup"><span data-stu-id="96ee2-137">B.</span></span> <span data-ttu-id="96ee2-138">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="96ee2-138">Reassign current user licenses</span></span>

<span data-ttu-id="96ee2-139">C.</span><span class="sxs-lookup"><span data-stu-id="96ee2-139">C.</span></span> <span data-ttu-id="96ee2-140">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="96ee2-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="96ee2-141">Migrieren Ihrer Kunden zu neuen Plänen</span><span class="sxs-lookup"><span data-stu-id="96ee2-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="96ee2-142">A.</span><span class="sxs-lookup"><span data-stu-id="96ee2-142">A.</span></span> <span data-ttu-id="96ee2-143">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="96ee2-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="96ee2-144">Um das neue Abonnement zu erwerben, wählen Sie im **Menü Partner Center** die Option **Kunden** aus, wählen Sie den Kunden aus, den Sie verschieben möchten, und wählen Sie dann **Abonnements hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="96ee2-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="96ee2-145">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="96ee2-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="96ee2-146">Ihr Kunde sollte nun sowohl über alte als auch über neue Abonnements, das alte eigenständige Kaizala Pro-Abonnement und das neue Zielabonnement verfügen, z. B. Option 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="96ee2-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="96ee2-147">B.</span><span class="sxs-lookup"><span data-stu-id="96ee2-147">B.</span></span> <span data-ttu-id="96ee2-148">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="96ee2-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="96ee2-149">Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen des Kunden im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="96ee2-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="96ee2-150">Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="96ee2-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="96ee2-151">Um die Benutzerlizenz neu zuzuweisen, wählen Sie den neu zuzuweisenden Benutzer und dann **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="96ee2-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="96ee2-152">Aktivieren Sie **auf der Seite** Lizenzen verwalten das Kontrollkästchen Kaizala Pro Standalone-Lizenz, und wählen Sie einen neuen Serviceplan für das Abonnement aus, in das der Kunde um zieht.</span><span class="sxs-lookup"><span data-stu-id="96ee2-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="96ee2-153">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="96ee2-153">Select **Submit**.</span></span> <span data-ttu-id="96ee2-154">Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="96ee2-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="96ee2-155">Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.</span><span class="sxs-lookup"><span data-stu-id="96ee2-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="96ee2-156">C.</span><span class="sxs-lookup"><span data-stu-id="96ee2-156">C.</span></span> <span data-ttu-id="96ee2-157">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="96ee2-157">Cancel old subscription</span></span>

<span data-ttu-id="96ee2-158">Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.</span><span class="sxs-lookup"><span data-stu-id="96ee2-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="96ee2-159">Wählen Sie **Partner Center** Menü Kunden **aus.**</span><span class="sxs-lookup"><span data-stu-id="96ee2-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="96ee2-160">Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.</span><span class="sxs-lookup"><span data-stu-id="96ee2-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="96ee2-161">Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.</span><span class="sxs-lookup"><span data-stu-id="96ee2-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="96ee2-162">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="96ee2-162">Select **Submit**.</span></span>

<span data-ttu-id="96ee2-163">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="96ee2-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="96ee2-164">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="96ee2-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="96ee2-165">Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="96ee2-165">The customer incurs no additional costs for the old subscription.</span></span>
