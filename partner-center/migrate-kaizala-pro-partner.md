---
title: Migrieren von kaizala pro-Abonnements zu Microsoft365
description: Erfahren Sie, wie Sie kaizala pro-Abonnements zu Microsoft365-oder Office 365-Versionen migrieren.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611236"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="23013-103">Migrieren von eigenständigen kaizala pro-Abonnements zu Microsoft365-oder Office 365-Versionen</span><span class="sxs-lookup"><span data-stu-id="23013-103">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="23013-104">Ab dem 1. Juli 2020 beendet Microsoft den Umsatz des eigenständigen kaizala pro-Dienstanbieter.</span><span class="sxs-lookup"><span data-stu-id="23013-104">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="23013-105">Kunden können nach diesem Datum keine neuen kaizala pro-Abonnements mehr erwerben, und vorhandene kaizala pro-Abonnements werden nicht automatisch erneuert, wenn Sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="23013-105">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="23013-106">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit abgelaufenen, eigenständigen kaizala pro-Abonnements auf eine unterstützte SKU-Option umstellen, die unten aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="23013-106">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="23013-107">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="23013-107">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="23013-108">Wenn Sie die API (entweder "Kamm" oder "Partner Center") verwenden, können Sie ablaufende Abonnements ermitteln, indem Sie das Enddatum des Abonnements und die Eigenschaft "automatisch erneuern" auf "false" festlegen `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="23013-108">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="23013-109">Die E4-Abonnements werden auf den `auto renew=False` 1. Juli 2020 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="23013-109">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="23013-110">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="23013-110">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="23013-111">Eigenständige "kaizala pro"-Ersetzungs Pläne</span><span class="sxs-lookup"><span data-stu-id="23013-111">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="23013-112">Mit den neuen Plänen können Ihre Kunden in Microsoft 365 neuere Features und Funktionen nutzen.</span><span class="sxs-lookup"><span data-stu-id="23013-112">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="23013-113">Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="23013-113">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="23013-114">[**Microsoft 365 für Unternehmen**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), einschließlich:</span><span class="sxs-lookup"><span data-stu-id="23013-114">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="23013-115">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="23013-115">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="23013-116">Standard Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="23013-116">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="23013-117">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="23013-117">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="23013-118">[**Microsoft 365 für Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), einschließlich:</span><span class="sxs-lookup"><span data-stu-id="23013-118">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="23013-119">Microsoft 365 F3 (früher Microsoft 365 F1) und Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="23013-119">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="23013-120">[**Microsoft 365 für Unternehmen**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), einschließlich:</span><span class="sxs-lookup"><span data-stu-id="23013-120">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="23013-121">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="23013-121">Office 365 E1</span></span>
   - <span data-ttu-id="23013-122">Microsoft 365 E3 und Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="23013-122">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="23013-123">Microsoft 365 E5 und Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="23013-123">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="23013-124">[**Microsoft 365 für Bildungseinrichtungen**](https://www.microsoft.com/education/buy-license/microsoft365), einschließlich:</span><span class="sxs-lookup"><span data-stu-id="23013-124">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="23013-125">Microsoft 365 a1 und Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="23013-125">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="23013-126">Microsoft 365 a3 und Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="23013-126">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="23013-127">Microsoft 365 a5 und Office 365 a5</span><span class="sxs-lookup"><span data-stu-id="23013-127">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="23013-128">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="23013-128">Transition customers to new product plans</span></span>

<span data-ttu-id="23013-129">Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an.</span><span class="sxs-lookup"><span data-stu-id="23013-129">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="23013-130">In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren.</span><span class="sxs-lookup"><span data-stu-id="23013-130">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="23013-131">Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:</span><span class="sxs-lookup"><span data-stu-id="23013-131">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="23013-132">A.</span><span class="sxs-lookup"><span data-stu-id="23013-132">A.</span></span> <span data-ttu-id="23013-133">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="23013-133">Purchase the new subscription</span></span>

<span data-ttu-id="23013-134">B.</span><span class="sxs-lookup"><span data-stu-id="23013-134">B.</span></span> <span data-ttu-id="23013-135">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="23013-135">Reassign current user licenses</span></span>

<span data-ttu-id="23013-136">C.</span><span class="sxs-lookup"><span data-stu-id="23013-136">C.</span></span> <span data-ttu-id="23013-137">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="23013-137">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="23013-138">Migrieren Ihrer Kunden zu neuen Plänen</span><span class="sxs-lookup"><span data-stu-id="23013-138">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="23013-139">A.</span><span class="sxs-lookup"><span data-stu-id="23013-139">A.</span></span> <span data-ttu-id="23013-140">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="23013-140">Purchase the new subscription</span></span>

1. <span data-ttu-id="23013-141">Wenn Sie das neue Abonnement erwerben möchten, wählen Sie im **Partner Center** -Menü **Kunden**aus, wählen Sie den zu verschiebenden Kunden aus, und klicken Sie dann auf **Abonnements hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="23013-141">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="23013-142">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="23013-142">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="23013-143">Ihr Kunde sollte nun sowohl alte als auch neue Abonnements haben, das alte, eigenständige kaizala pro-Abonnement und das neue Abonnement "target", z. b. Option 1-Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="23013-143">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="23013-144">B.</span><span class="sxs-lookup"><span data-stu-id="23013-144">B.</span></span> <span data-ttu-id="23013-145">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="23013-145">Reassign current user licenses</span></span>

1. <span data-ttu-id="23013-146">Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen des Kunden im Menü **Partner Center** die Option **Kunden** aus. Wählen Sie dann den zu verschiebenden Kunden und die Option **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="23013-146">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="23013-147">Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="23013-147">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="23013-148">Um die Benutzerlizenz erneut zuzuweisen, wählen Sie den neu zuzuweisenden Benutzer aus, und wählen Sie dann **Lizenzen verwalten**aus.</span><span class="sxs-lookup"><span data-stu-id="23013-148">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="23013-149">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die eigenständige kaizala pro-Lizenz, und wählen Sie einen neuen Dienstplan für das Abonnement aus, zu dem der Kunde wechselt.</span><span class="sxs-lookup"><span data-stu-id="23013-149">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="23013-150">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="23013-150">Select **Submit**.</span></span> <span data-ttu-id="23013-151">Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="23013-151">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="23013-152">Führen Sie denselben Prozess für andere Benutzer durch, die Lizenzzuweisungen benötigen.</span><span class="sxs-lookup"><span data-stu-id="23013-152">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="23013-153">C.</span><span class="sxs-lookup"><span data-stu-id="23013-153">C.</span></span> <span data-ttu-id="23013-154">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="23013-154">Cancel old subscription</span></span>

<span data-ttu-id="23013-155">Nachdem Sie die Benutzerlizenz zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.</span><span class="sxs-lookup"><span data-stu-id="23013-155">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="23013-156">Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="23013-156">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="23013-157">Wählen Sie den Kunden, dessen Abonnement Sie stornieren möchten.</span><span class="sxs-lookup"><span data-stu-id="23013-157">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="23013-158">Legen Sie auf der Seite mit den Abonnementdetails das Abonnement auf **Ausgesetzt** fest.</span><span class="sxs-lookup"><span data-stu-id="23013-158">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="23013-159">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="23013-159">Select **Submit**.</span></span>

<span data-ttu-id="23013-160">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="23013-160">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="23013-161">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="23013-161">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="23013-162">Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="23013-162">The customer incurs no additional costs for the old subscription.</span></span>
