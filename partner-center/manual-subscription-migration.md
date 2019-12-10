---
title: Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierte Angebote) zu neueren Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie ein neues Abonnement erwerben können, bevor die vorhandenen ablaufen, Benutzerlizenzen neu zuweisen und dann das alte Abonnement kündigen.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365-Angebote, Angebote verlängern, neue Dynamics 365-SKUs
ms.openlocfilehash: bbb7480264a2d3d5ae6ed1f50e0f32b5ebc1c16e
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943353"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="29473-104">Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierte Angebote) zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="29473-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="29473-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="29473-105">**Applies to**</span></span>

-  <span data-ttu-id="29473-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="29473-106">Partner Center</span></span>

<span data-ttu-id="29473-107">Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 for Sales/Customer Engagement Plan von Basic (qualifizierte Angebote)-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="29473-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="29473-108">Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]".</span><span class="sxs-lookup"><span data-stu-id="29473-108">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="29473-109">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.).</span><span class="sxs-lookup"><span data-stu-id="29473-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="29473-110">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="29473-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="29473-111">Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln.</span><span class="sxs-lookup"><span data-stu-id="29473-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="29473-112">Die betreffenden Abonnements werden am 1. Januar 2019 auf „auto renew=False“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="29473-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="29473-113">Sie können Kunden jederzeit zu einem neuen Plan migrieren.</span><span class="sxs-lookup"><span data-stu-id="29473-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="29473-114">Die folgenden Dynamics 365-Angebote werden eingestellt</span><span class="sxs-lookup"><span data-stu-id="29473-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="29473-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29473-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="29473-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29473-118">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29473-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29473-122">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29473-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="29473-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29473-126">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="29473-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29473-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29473-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="29473-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29473-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29473-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="29473-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29473-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="29473-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="29473-139">Ersatzpläne für Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="29473-140">**Eingestellte Angebote**</span><span class="sxs-lookup"><span data-stu-id="29473-140">**Retired offers**</span></span>   

- <span data-ttu-id="29473-141">Dynamics 365 for Sales from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29473-142">Dynamics 365 Customer Engagement Plan from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="29473-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="29473-143">**Ersatzoptionen**</span><span class="sxs-lookup"><span data-stu-id="29473-143">**Replacement options**</span></span>
- <span data-ttu-id="29473-144">Dynamics 365 for Sales Professional (NEU)</span><span class="sxs-lookup"><span data-stu-id="29473-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="29473-145">Dynamics 365 for Sales Professional (NEU)</span><span class="sxs-lookup"><span data-stu-id="29473-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="29473-146">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="29473-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="29473-147">Dynamics 365 Customer Engagement Plan oder</span><span class="sxs-lookup"><span data-stu-id="29473-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="29473-148">Dynamics 365 Team Members</span><span class="sxs-lookup"><span data-stu-id="29473-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="29473-149">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="29473-149">Transition customers to new product plans</span></span>

<span data-ttu-id="29473-150">Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="29473-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="29473-151">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="29473-151">Purchase the new subscription</span></span>
- <span data-ttu-id="29473-152">Neuzuweisen aktueller Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="29473-152">Reassign current user licenses</span></span>
- <span data-ttu-id="29473-153">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="29473-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="29473-154">Kaufen des neuen Plans für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="29473-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="29473-155">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="29473-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="29473-156">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="29473-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="29473-157">Wählen Sie im Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die gewünschte Anzahl von Lizenzen ein, und wählen Sie anschließend **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="29473-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="29473-158">Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement.</span><span class="sxs-lookup"><span data-stu-id="29473-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="29473-159">Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="29473-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="29473-160">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="29473-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="29473-161">Wählen Sie **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="29473-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="29473-162">Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="29473-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="29473-163">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="29473-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="29473-164">Wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="29473-164">Select **Submit**.</span></span> <span data-ttu-id="29473-165">Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen.</span><span class="sxs-lookup"><span data-stu-id="29473-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="29473-166">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement stornieren.</span><span class="sxs-lookup"><span data-stu-id="29473-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="29473-167">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="29473-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="29473-168">Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="29473-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="29473-169">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="29473-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="29473-170">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="29473-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="29473-171">Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="29473-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



