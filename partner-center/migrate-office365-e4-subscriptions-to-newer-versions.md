---
title: Migrieren von Office 365 E4-Abonnements
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Die Enterprise E4-Edition von Microsoft Office 365 wurde am 7. April 2017 eingestellt. Hier erfahren Sie, wie Sie Ihre Kundenabonnements zu neueren Versionen von Office 365 migrieren.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132620"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="72752-104">Migrieren von Abonnements für Office 365 E4 auf neuere Versionen von Office 365</span><span class="sxs-lookup"><span data-stu-id="72752-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="72752-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="72752-105">**Appropriate roles**</span></span>

- <span data-ttu-id="72752-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="72752-106">Global admin</span></span>
- <span data-ttu-id="72752-107">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="72752-107">User management admin</span></span>
- <span data-ttu-id="72752-108">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="72752-108">Admin agent</span></span>
- <span data-ttu-id="72752-109">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="72752-109">Sales agent</span></span>

<span data-ttu-id="72752-110">Der Enterprise E4-Plan für Office 365 wurde am 7. April 2017 eingestellt.</span><span class="sxs-lookup"><span data-stu-id="72752-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="72752-111">Nach diesem Datum können keine neuen Office 365 E4-Abonnements mehr erworben werden, und bereits vorhandene E4-Abonnements werden bei Ablauf nicht automatisch verlängert.</span><span class="sxs-lookup"><span data-stu-id="72752-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="72752-112">Wenn E4-Abonnements enden, werden sie storniert.</span><span class="sxs-lookup"><span data-stu-id="72752-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="72752-113">Zur Gewährleistung von Kontinuität für betroffene Kunden sollten Sie Kunden mit ablaufenden E4-Abonnements zu einer unterstützten SKU-Option (nachfolgend aufgeführt) migrieren.</span><span class="sxs-lookup"><span data-stu-id="72752-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="72752-114">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="72752-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="72752-115">Sowohl kommerzielle SKUs als auch Behörden-SKUs für Office 365 Enterprise E4 wurden eingestellt.</span><span class="sxs-lookup"><span data-stu-id="72752-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="72752-116">Auf der Detailseite des Abonnements wurde der E4-Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert.</span><span class="sxs-lookup"><span data-stu-id="72752-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="72752-117">Bei Verwendung der API (CREST oder Partner Center) können Sie ablaufende Abonnements anhand des Enddatums des Abonnements sowie anhand der Eigenschaft „auto renew = False“ erkennen.</span><span class="sxs-lookup"><span data-stu-id="72752-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="72752-118">Für E4-Abonnements wird die automatische Verlängerung am 7. April 2017 automatisch auf „False“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="72752-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="72752-119">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="72752-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="72752-120">Ersatzpläne für die Enterprise E4-Edition von Office 365</span><span class="sxs-lookup"><span data-stu-id="72752-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="72752-121">Sie können wählen, ob die gleichen Funktionen wie in E4 bereitgestellt werden oder ob Ihre Kunden in Office 365 und Skype for Business Online in den Genuss neuerer Features und Funktionen kommen sollen.</span><span class="sxs-lookup"><span data-stu-id="72752-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="72752-122">Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="72752-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="72752-123">Secure Productive Enterprise E3 bzw. Secure Productive Enterprise E5 kann durch die folgenden Optionen für Office 365 Enterprise E3 bzw. Office 365 Enterprise E5 ersetzt werden:</span><span class="sxs-lookup"><span data-stu-id="72752-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="72752-124">Option 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="72752-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="72752-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="72752-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="72752-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (Preis-und Funktionalitäts Parität mit E4)</span><span class="sxs-lookup"><span data-stu-id="72752-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="72752-127">Option 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="72752-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="72752-128">Funktion</span><span class="sxs-lookup"><span data-stu-id="72752-128">Feature</span></span> | <span data-ttu-id="72752-129">Option 1:</span><span class="sxs-lookup"><span data-stu-id="72752-129">Option 1</span></span> | <span data-ttu-id="72752-130">Option 2:</span><span class="sxs-lookup"><span data-stu-id="72752-130">Option 2</span></span> | <span data-ttu-id="72752-131">Option 3</span><span class="sxs-lookup"><span data-stu-id="72752-131">Option 3</span></span> | <span data-ttu-id="72752-132">Option 4</span><span class="sxs-lookup"><span data-stu-id="72752-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="72752-133">Alle in Office 365 Enterprise E4 enthaltenen Features verfügbar?</span><span class="sxs-lookup"><span data-stu-id="72752-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="72752-134">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-134">Yes</span></span> | <span data-ttu-id="72752-135">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-135">Yes</span></span> | <span data-ttu-id="72752-136">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-136">Yes</span></span> | <span data-ttu-id="72752-137">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-137">No</span></span> |
| <span data-ttu-id="72752-138">Verwaltung von Telefonnummern in Office 365?</span><span class="sxs-lookup"><span data-stu-id="72752-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="72752-139">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-139">Yes</span></span> | <span data-ttu-id="72752-140">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-140">Yes</span></span> | <span data-ttu-id="72752-141">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-141">No</span></span> | <span data-ttu-id="72752-142">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-142">No</span></span> |
| <span data-ttu-id="72752-143">Verwaltung von Telefonnummern sowohl lokal als auch in Office 365 (Hybridbereitstellung)?</span><span class="sxs-lookup"><span data-stu-id="72752-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="72752-144">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-144">Yes</span></span> | <span data-ttu-id="72752-145">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-145">Yes</span></span> | <span data-ttu-id="72752-146">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-146">No</span></span> | <span data-ttu-id="72752-147">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-147">No</span></span> |
| <span data-ttu-id="72752-148">Option zum Hinzufügen eines PSTN-Sprachanrufplans?</span><span class="sxs-lookup"><span data-stu-id="72752-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="72752-149">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-149">Yes</span></span> | <span data-ttu-id="72752-150">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-150">Yes</span></span> | <span data-ttu-id="72752-151">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-151">No</span></span> | <span data-ttu-id="72752-152">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-152">No</span></span> |
| <span data-ttu-id="72752-153">PSTN-Konferenzen?</span><span class="sxs-lookup"><span data-stu-id="72752-153">PSTN Conferencing?</span></span> | <span data-ttu-id="72752-154">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-154">Yes</span></span> | <span data-ttu-id="72752-155">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-155">No</span></span> | <span data-ttu-id="72752-156">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-156">No</span></span> | <span data-ttu-id="72752-157">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-157">No</span></span> |
| <span data-ttu-id="72752-158">Erweiterte Tools für Zusammenarbeit, Analysen und Sicherheit?</span><span class="sxs-lookup"><span data-stu-id="72752-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="72752-159">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-159">Yes</span></span> | <span data-ttu-id="72752-160">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-160">No</span></span> | <span data-ttu-id="72752-161">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-161">No</span></span> | <span data-ttu-id="72752-162">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-162">No</span></span> |
| <span data-ttu-id="72752-163">Interaktive Berichte, Dashboards und Datenvisualisierungen?</span><span class="sxs-lookup"><span data-stu-id="72752-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="72752-164">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-164">Yes</span></span> | <span data-ttu-id="72752-165">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-165">No</span></span> | <span data-ttu-id="72752-166">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-166">No</span></span> | <span data-ttu-id="72752-167">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-167">No</span></span> | 
| <span data-ttu-id="72752-168">Mehr Kontrolle über die Datensicherheit und Compliance mit integriertem Datenschutz, Transparenz und optimierten Benutzersteuerelementen?</span><span class="sxs-lookup"><span data-stu-id="72752-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="72752-169">Ja</span><span class="sxs-lookup"><span data-stu-id="72752-169">Yes</span></span> | <span data-ttu-id="72752-170">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-170">No</span></span> | <span data-ttu-id="72752-171">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-171">No</span></span> | <span data-ttu-id="72752-172">Nein</span><span class="sxs-lookup"><span data-stu-id="72752-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="72752-173">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="72752-173">Transition customers to new product plans</span></span>

<span data-ttu-id="72752-174">Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an.</span><span class="sxs-lookup"><span data-stu-id="72752-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="72752-175">In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren.</span><span class="sxs-lookup"><span data-stu-id="72752-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="72752-176">Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:</span><span class="sxs-lookup"><span data-stu-id="72752-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="72752-177">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="72752-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="72752-178">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="72752-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="72752-179">Stornieren des alten Abonnements.</span><span class="sxs-lookup"><span data-stu-id="72752-179">Cancel the old subscription</span></span>

<span data-ttu-id="72752-180">Führen Sie diese Schritte aus, um das Office 365 Enterprise E4-Abonnement eines Kunden zu einer der Optionen in der obigen Tabelle zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="72752-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="72752-181">Schritt 1: Kaufen des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="72752-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="72752-182">Wählen Sie im Menü **Partner Center** die Option **Kunden** und anschließend den Kunden aus, den Sie migrieren möchten. Wählen Sie dann **Abonnements hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="72752-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="72752-183">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="72752-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="72752-184">Ihr Kunde sollte nun sowohl alte als auch neue Abonnements haben, das alte Office 365 Enterprise E4-Abonnement und das neue Abonnement "target", z. b. Option 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="72752-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="72752-185">Schritt 2: Neuzuweisen der Benutzerlizenzen des Kunden</span><span class="sxs-lookup"><span data-stu-id="72752-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="72752-186">Wählen Sie im Menü **Partner Center** die Option **Kunden** und anschließend den Kunden aus, den Sie migrieren möchten. Wählen Sie dann **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="72752-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="72752-187">Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="72752-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="72752-188">Wählen Sie zum erneuten Zuweisen von Benutzerlizenzen den Benutzer aus, der neu zugewiesen werden soll, und wählen Sie dann **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="72752-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="72752-189">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Lizenzkontrollkästchen für **Office 365 Enterprise E4**, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="72752-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="72752-190">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="72752-190">Select **Submit**.</span></span> <span data-ttu-id="72752-191">Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="72752-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="72752-192">Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.</span><span class="sxs-lookup"><span data-stu-id="72752-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="72752-193">Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.</span><span class="sxs-lookup"><span data-stu-id="72752-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="72752-194">Schritt 3: Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="72752-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="72752-195">Wählen Sie im **Partner Center** -Menü die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="72752-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="72752-196">Wählen Sie den Kunden aus, den Sie migrieren möchten, und wählen Sie anschließend das Abonnement aus, das Sie stornieren möchten.</span><span class="sxs-lookup"><span data-stu-id="72752-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="72752-197">Legen Sie auf der Seite mit den Abonnementdetails den Abonnementstatus auf **Ausgesetzt** fest.</span><span class="sxs-lookup"><span data-stu-id="72752-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="72752-198">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="72752-198">Select **Submit**.</span></span>

<span data-ttu-id="72752-199">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="72752-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="72752-200">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="72752-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="72752-201">Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="72752-201">The customer incurs no additional costs for the old subscription.</span></span>



 



