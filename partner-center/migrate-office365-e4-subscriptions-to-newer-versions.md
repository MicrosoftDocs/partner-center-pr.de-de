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
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949045"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="5db7d-104">Migrieren von Abonnements für Office 365 E4 auf neuere Versionen von Office 365</span><span class="sxs-lookup"><span data-stu-id="5db7d-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="5db7d-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="5db7d-105">**Applies to**</span></span>

-  <span data-ttu-id="5db7d-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="5db7d-106">Partner Center</span></span>

<span data-ttu-id="5db7d-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="5db7d-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="5db7d-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="5db7d-108">Global admin</span></span>
-   <span data-ttu-id="5db7d-109">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="5db7d-109">User admin</span></span>
-   <span data-ttu-id="5db7d-110">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="5db7d-110">Admin agent</span></span>
-   <span data-ttu-id="5db7d-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="5db7d-111">Sales agent</span></span>

<span data-ttu-id="5db7d-112">Der Enterprise E4-Plan für Office 365 wurde am 7. April 2017 eingestellt.</span><span class="sxs-lookup"><span data-stu-id="5db7d-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="5db7d-113">Nach diesem Datum können keine neuen Office 365 E4-Abonnements mehr erworben werden, und bereits vorhandene E4-Abonnements werden bei Ablauf nicht automatisch verlängert.</span><span class="sxs-lookup"><span data-stu-id="5db7d-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="5db7d-114">Wenn E4-Abonnements enden, werden sie storniert.</span><span class="sxs-lookup"><span data-stu-id="5db7d-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="5db7d-115">Zur Gewährleistung von Kontinuität für betroffene Kunden sollten Sie Kunden mit ablaufenden E4-Abonnements zu einer unterstützten SKU-Option (nachfolgend aufgeführt) migrieren.</span><span class="sxs-lookup"><span data-stu-id="5db7d-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="5db7d-116">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="5db7d-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="5db7d-117">Sowohl kommerzielle SKUs als auch Behörden-SKUs für Office 365 Enterprise E4 wurden eingestellt.</span><span class="sxs-lookup"><span data-stu-id="5db7d-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="5db7d-118">Auf der Detailseite des Abonnements wurde der E4-Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert.</span><span class="sxs-lookup"><span data-stu-id="5db7d-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="5db7d-119">Bei Verwendung der API (CREST oder Partner Center) können Sie ablaufende Abonnements anhand des Enddatums des Abonnements sowie anhand der Eigenschaft „auto renew = False“ erkennen.</span><span class="sxs-lookup"><span data-stu-id="5db7d-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="5db7d-120">Für E4-Abonnements wird die automatische Verlängerung am 7. April 2017 automatisch auf „False“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5db7d-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="5db7d-121">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="5db7d-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="5db7d-122">Ersatzpläne für die Enterprise E4-Edition von Office 365</span><span class="sxs-lookup"><span data-stu-id="5db7d-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="5db7d-123">Sie können wählen, ob die gleichen Funktionen wie in E4 bereitgestellt werden oder ob Ihre Kunden in Office 365 und Skype for Business Online in den Genuss neuerer Features und Funktionen kommen sollen.</span><span class="sxs-lookup"><span data-stu-id="5db7d-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="5db7d-124">Preisdetails finden Sie in der Preisliste und der Angebotslistenmatrix in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5db7d-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="5db7d-125">Secure Productive Enterprise E3 bzw. Secure Productive Enterprise E5 kann durch die folgenden Optionen für Office 365 Enterprise E3 bzw. Office 365 Enterprise E5 ersetzt werden:</span><span class="sxs-lookup"><span data-stu-id="5db7d-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="5db7d-126">Option 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="5db7d-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="5db7d-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="5db7d-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="5db7d-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (Preis-und Funktionalitäts Parität mit E4)</span><span class="sxs-lookup"><span data-stu-id="5db7d-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="5db7d-129">Option 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="5db7d-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="5db7d-130">Feature</span><span class="sxs-lookup"><span data-stu-id="5db7d-130">Feature</span></span> | <span data-ttu-id="5db7d-131">Option 1:</span><span class="sxs-lookup"><span data-stu-id="5db7d-131">Option 1</span></span> | <span data-ttu-id="5db7d-132">Option 2:</span><span class="sxs-lookup"><span data-stu-id="5db7d-132">Option 2</span></span> | <span data-ttu-id="5db7d-133">Option 3</span><span class="sxs-lookup"><span data-stu-id="5db7d-133">Option 3</span></span> | <span data-ttu-id="5db7d-134">Option 4</span><span class="sxs-lookup"><span data-stu-id="5db7d-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="5db7d-135">Alle in Office 365 Enterprise E4 enthaltenen Features verfügbar?</span><span class="sxs-lookup"><span data-stu-id="5db7d-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="5db7d-136">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-136">Yes</span></span> | <span data-ttu-id="5db7d-137">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-137">Yes</span></span> | <span data-ttu-id="5db7d-138">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-138">Yes</span></span> | <span data-ttu-id="5db7d-139">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-139">No</span></span> |
| <span data-ttu-id="5db7d-140">Verwaltung von Telefonnummern in Office 365?</span><span class="sxs-lookup"><span data-stu-id="5db7d-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="5db7d-141">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-141">Yes</span></span> | <span data-ttu-id="5db7d-142">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-142">Yes</span></span> | <span data-ttu-id="5db7d-143">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-143">No</span></span> | <span data-ttu-id="5db7d-144">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-144">No</span></span> |
| <span data-ttu-id="5db7d-145">Verwaltung von Telefonnummern sowohl lokal als auch in Office 365 (Hybridbereitstellung)?</span><span class="sxs-lookup"><span data-stu-id="5db7d-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="5db7d-146">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-146">Yes</span></span> | <span data-ttu-id="5db7d-147">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-147">Yes</span></span> | <span data-ttu-id="5db7d-148">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-148">No</span></span> | <span data-ttu-id="5db7d-149">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-149">No</span></span> |
| <span data-ttu-id="5db7d-150">Option zum Hinzufügen eines PSTN-Sprachanrufplans?</span><span class="sxs-lookup"><span data-stu-id="5db7d-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="5db7d-151">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-151">Yes</span></span> | <span data-ttu-id="5db7d-152">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-152">Yes</span></span> | <span data-ttu-id="5db7d-153">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-153">No</span></span> | <span data-ttu-id="5db7d-154">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-154">No</span></span> |
| <span data-ttu-id="5db7d-155">PSTN-Konferenzen?</span><span class="sxs-lookup"><span data-stu-id="5db7d-155">PSTN Conferencing?</span></span> | <span data-ttu-id="5db7d-156">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-156">Yes</span></span> | <span data-ttu-id="5db7d-157">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-157">No</span></span> | <span data-ttu-id="5db7d-158">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-158">No</span></span> | <span data-ttu-id="5db7d-159">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-159">No</span></span> |
| <span data-ttu-id="5db7d-160">Erweiterte Tools für Zusammenarbeit, Analysen und Sicherheit?</span><span class="sxs-lookup"><span data-stu-id="5db7d-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="5db7d-161">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-161">Yes</span></span> | <span data-ttu-id="5db7d-162">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-162">No</span></span> | <span data-ttu-id="5db7d-163">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-163">No</span></span> | <span data-ttu-id="5db7d-164">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-164">No</span></span> |
| <span data-ttu-id="5db7d-165">Interaktive Berichte, Dashboards und Datenvisualisierungen?</span><span class="sxs-lookup"><span data-stu-id="5db7d-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="5db7d-166">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-166">Yes</span></span> | <span data-ttu-id="5db7d-167">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-167">No</span></span> | <span data-ttu-id="5db7d-168">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-168">No</span></span> | <span data-ttu-id="5db7d-169">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-169">No</span></span> | 
| <span data-ttu-id="5db7d-170">Mehr Kontrolle über die Datensicherheit und Compliance mit integriertem Datenschutz, Transparenz und optimierten Benutzersteuerelementen?</span><span class="sxs-lookup"><span data-stu-id="5db7d-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="5db7d-171">Ja</span><span class="sxs-lookup"><span data-stu-id="5db7d-171">Yes</span></span> | <span data-ttu-id="5db7d-172">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-172">No</span></span> | <span data-ttu-id="5db7d-173">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-173">No</span></span> | <span data-ttu-id="5db7d-174">Nein</span><span class="sxs-lookup"><span data-stu-id="5db7d-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5db7d-175">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="5db7d-175">Transition customers to new product plans</span></span>

<span data-ttu-id="5db7d-176">Microsoft bietet Partnern kontinuierlich neue Produkte und Dienste an.</span><span class="sxs-lookup"><span data-stu-id="5db7d-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="5db7d-177">In diesen Fällen müssen Sie Kunden möglicherweise auf neue Dienste upgraden oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren.</span><span class="sxs-lookup"><span data-stu-id="5db7d-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="5db7d-178">Die Migration von Kunden mit eingestellten SKUs zu neueren SKUs umfasst folgende Schritte:</span><span class="sxs-lookup"><span data-stu-id="5db7d-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="5db7d-179">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="5db7d-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="5db7d-180">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="5db7d-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="5db7d-181">Stornieren des alten Abonnements.</span><span class="sxs-lookup"><span data-stu-id="5db7d-181">Cancel the old subscription</span></span>

<span data-ttu-id="5db7d-182">Führen Sie diese Schritte aus, um das Office 365 Enterprise E4-Abonnement eines Kunden zu einer der Optionen in der obigen Tabelle zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="5db7d-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="5db7d-183">Schritt 1: Kaufen des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="5db7d-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="5db7d-184">Wählen Sie im Menü **Partner Center** die Option **Kunden** und anschließend den Kunden aus, den Sie migrieren möchten. Wählen Sie dann **Abonnements hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="5db7d-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="5db7d-185">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="5db7d-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="5db7d-186">Ihr Kunde sollte nun sowohl alte als auch neue Abonnements haben, das alte Office 365 Enterprise E4-Abonnement und das neue Abonnement "target", z. b. Option 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="5db7d-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="5db7d-187">Schritt 2: Neuzuweisen der Benutzerlizenzen des Kunden</span><span class="sxs-lookup"><span data-stu-id="5db7d-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="5db7d-188">Wählen Sie im Menü **Partner Center** die Option **Kunden** und anschließend den Kunden aus, den Sie migrieren möchten. Wählen Sie dann **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="5db7d-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="5db7d-189">Die Seite Benutzer und Lizenzen des Kunden wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="5db7d-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="5db7d-190">Um Benutzerlizenzen neu zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="5db7d-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="5db7d-191">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Lizenzkontrollkästchen für **Office 365 Enterprise E4**, und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="5db7d-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="5db7d-192">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="5db7d-192">Select **Submit**.</span></span> <span data-ttu-id="5db7d-193">Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="5db7d-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="5db7d-194">Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.</span><span class="sxs-lookup"><span data-stu-id="5db7d-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="5db7d-195">Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das eingestellte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.</span><span class="sxs-lookup"><span data-stu-id="5db7d-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="5db7d-196">Schritt 3: Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="5db7d-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="5db7d-197">Wählen Sie im **Partner Center** -Menü die Option **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="5db7d-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="5db7d-198">Wählen Sie den Kunden aus, den Sie migrieren möchten, und wählen Sie anschließend das Abonnement aus, das Sie stornieren möchten.</span><span class="sxs-lookup"><span data-stu-id="5db7d-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="5db7d-199">Legen Sie auf der Seite mit den Abonnementdetails den Abonnementstatus auf **Ausgesetzt** fest.</span><span class="sxs-lookup"><span data-stu-id="5db7d-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="5db7d-200">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="5db7d-200">Select **Submit**.</span></span>

<span data-ttu-id="5db7d-201">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="5db7d-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="5db7d-202">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="5db7d-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="5db7d-203">Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="5db7d-203">The customer incurs no additional costs for the old subscription.</span></span>



 



