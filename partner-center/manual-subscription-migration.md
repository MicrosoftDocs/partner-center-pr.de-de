---
title: Migrieren von Dynamics 365 und Customer Engagement Plan aus Basic (qualifizierten Angebote) zu neueren Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement Plan (qualifizierten bietet) Basic Abonnements können nicht mehr verlängert werden.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968270"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="38220-103">Migrieren von Dynamics 365 und Customer Engagement Plan aus Basic (qualifizierten Angebote) zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="38220-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="38220-104">Betrifft:</span><span class="sxs-lookup"><span data-stu-id="38220-104">Applies to</span></span>**

-  <span data-ttu-id="38220-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="38220-105">Partner Center</span></span>

<span data-ttu-id="38220-106">Effektive am 1. Januar 2019 Kunden mit Dynamics 365 for Sales / Customer Engagement Plan (qualifizierten bietet) Basic Abonnements können nicht mehr erneuern, die diese älteren Angebote; vorhandene Abonnements werden bei Ablauf nicht automatisch verlängert.</span><span class="sxs-lookup"><span data-stu-id="38220-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="38220-107">Auf der Detailseite des Abonnements wird der Abonnementstatus von "Datum der automatischen [Datum]" in "Gültig bis [Datum]" ändern.</span><span class="sxs-lookup"><span data-stu-id="38220-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="38220-108">Um Kontinuität für Kunden zu gewährleisten, sollten Sie diese mit ablaufenden Abonnements auf eine unterstützte Option, die unten aufgeführten übertragen.</span><span class="sxs-lookup"><span data-stu-id="38220-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="38220-109">Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="38220-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="38220-110">Wenn Sie die API (CREST oder Partner Center) verwenden, finden Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie die automatische Verlängerung Eigenschaft "false".</span><span class="sxs-lookup"><span data-stu-id="38220-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="38220-111">Die betreffenden Abonnements werden auf auto festgelegt werden verlängern = "false" am 1. Januar 2019.</span><span class="sxs-lookup"><span data-stu-id="38220-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="38220-112">Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="38220-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="38220-113">Die Dynamics 365 bietet eingestellt wird</span><span class="sxs-lookup"><span data-stu-id="38220-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="38220-114">Dynamics 365 für Vertrieb Enterprise Edition CRMOL Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Lehrkräfte</span><span class="sxs-lookup"><span data-stu-id="38220-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="38220-116">Dynamics 365 für Vertrieb Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Schüler und Studenten</span><span class="sxs-lookup"><span data-stu-id="38220-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="38220-117">Dynamics 365 für Vertrieb Enterprise Edition (Behörden Preisgestaltung) CRMOL Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-118">Dynamics 365 for Sales Enterprise-Edition SA für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-119">Dynamics 365 for Sales Enterprise-Edition SA für CRM Basic (qualifizierten Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="38220-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="38220-120">Dynamics 365 for Sales Enterprise-Edition SA für CRM Basic (qualifizierten Angebot) für Schüler und Studenten</span><span class="sxs-lookup"><span data-stu-id="38220-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="38220-121">Dynamics 365 Sales Enterprise-Edition (Behörden Preisgestaltung) SA für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-122">Dynamics 365 for Sales Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-123">Dynamics 365 for Sales Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="38220-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="38220-124">Dynamics 365 for Sales Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Schüler und Studenten</span><span class="sxs-lookup"><span data-stu-id="38220-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="38220-125">Dynamics 365 für Vertrieb Enterprise Edition (Behörden Preisgestaltung) Add-On für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behörden Preisgestaltung) CRMOL Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Schüler und Studenten</span><span class="sxs-lookup"><span data-stu-id="38220-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="38220-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierten Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="38220-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="38220-130">Dynamics 365 Customer Engagement Plan Enterprise-Edition von SA für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-131">Dynamics 365 Kunden Engagement Plan Enterprise-Edition (Behörden Preisgestaltung) von SA für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-132">Dynamics 365 Customer Engagement Plan Enterprise-Edition von SA für CRM Basic (qualifizierten Angebot) für Schüler und Studenten</span><span class="sxs-lookup"><span data-stu-id="38220-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="38220-133">Dynamics 365 Customer Engagement Plan Enterprise-Edition von SA für CRM Basic (qualifizierten Angebot) für Lehrkräfte</span><span class="sxs-lookup"><span data-stu-id="38220-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="38220-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-135">Dynamics 365 Kunden Engagement Plan Enterprise Edition (Behörden Preisgestaltung) Add-On für CRM Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Schüler und Studenten</span><span class="sxs-lookup"><span data-stu-id="38220-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="38220-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On für CRM Basic (qualifizierten Angebot) für Lehrkräfte</span><span class="sxs-lookup"><span data-stu-id="38220-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="38220-138">Dynamics 365 for Sales / Customer Engagement Plan aus (qualifizierten bietet) Basic Ersatz-Pläne</span><span class="sxs-lookup"><span data-stu-id="38220-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="38220-139">Eingestellte Angebote</span><span class="sxs-lookup"><span data-stu-id="38220-139">Retired offers</span></span>**   

- <span data-ttu-id="38220-140">Dynamics 365 für den Verkauf von CRM Basic oder CRMOL Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="38220-141">Dynamics 365 Customer Engagement Plan von CRM Basic oder CRMOL Basic (qualifizierten Angebot)</span><span class="sxs-lookup"><span data-stu-id="38220-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="38220-142">Ersatz-Optionen</span><span class="sxs-lookup"><span data-stu-id="38220-142">Replacement options</span></span>**
- <span data-ttu-id="38220-143">Dynamics 365 for Sales Professional (neu)</span><span class="sxs-lookup"><span data-stu-id="38220-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="38220-144">Dynamics 365 for Sales Professional (neu)</span><span class="sxs-lookup"><span data-stu-id="38220-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="38220-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="38220-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="38220-146">Dynamics 365 Customer Engagement Plan oder</span><span class="sxs-lookup"><span data-stu-id="38220-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="38220-147">Dynamics 365 Team Member</span><span class="sxs-lookup"><span data-stu-id="38220-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="38220-148">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="38220-148">Transition customers to new product plans</span></span>

<span data-ttu-id="38220-149">Wechseln von Kunden von eingestellte SKUs zu neueren erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="38220-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="38220-150">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="38220-150">Purchase the new subscription</span></span>
- <span data-ttu-id="38220-151">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="38220-151">Reassign current user licenses</span></span>
- <span data-ttu-id="38220-152">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="38220-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="38220-153">Den neuen Plan für Ihre Kunden erwerben</span><span class="sxs-lookup"><span data-stu-id="38220-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="38220-154">Wählen Sie **Kunden** aus der linken Navigationsbereich, und wählen Sie dann den Kunden, die, den Sie dem neuen Abonnement verschieben möchten.</span><span class="sxs-lookup"><span data-stu-id="38220-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="38220-155">Wählen Sie das **Abonnement hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="38220-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="38220-156">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="38220-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="38220-157">Ihr Kunde wird nun das alte Abonnement und die neue Aufgabe besitzen.</span><span class="sxs-lookup"><span data-stu-id="38220-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="38220-158">Im nächste Schritt werden Lizenzen für Benutzer des Kunden neu zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="38220-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="38220-159">Wählen Sie **Kunden** aus der linken Navigationsbereich, und wählen Sie dann den Kunden, die, den Sie verschieben.</span><span class="sxs-lookup"><span data-stu-id="38220-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="38220-160">Wählen Sie **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="38220-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="38220-161">Um eine Lizenz für einen Benutzer erneut zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie dann die **Lizenzen verwalten**.</span><span class="sxs-lookup"><span data-stu-id="38220-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="38220-162">Auf der Seite " **Lizenzen verwalten** " deaktivieren Sie die Dynamics 365 for Sales / Customer Engagement Plan aus Basic (qualifizierten anbieten), Kontrollkästchen, und wählen Sie einen neuen Serviceplan für das Abonnement aus, die der Kunde in verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="38220-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="38220-163">Wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="38220-163">Select **Submit**.</span></span> <span data-ttu-id="38220-164">Sie werden für jeden Benutzer dazu, die neue Lizenz benötigt.</span><span class="sxs-lookup"><span data-stu-id="38220-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="38220-165">Nachdem Sie die Lizenzen für das neue Abonnement verschoben haben, können Sie das alte Abonnement stornieren.</span><span class="sxs-lookup"><span data-stu-id="38220-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="38220-166">Wählen Sie **Kunden** aus der linken Navigationsbereich, und wählen Sie dann den Kunden, die, den Sie verschieben.</span><span class="sxs-lookup"><span data-stu-id="38220-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="38220-167">Klicken Sie auf der Detailseite des Abonnements legen Sie das alte Abonnement auf **angehalten** , und wählen Sie **übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="38220-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="38220-168">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="38220-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="38220-169">Die Bereitstellung des ausgesetzten Abonnements wird nach 120Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="38220-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="38220-170">Ihre Kunden fallen für das alte Abonnement keine zusätzlichen Kosten.</span><span class="sxs-lookup"><span data-stu-id="38220-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



