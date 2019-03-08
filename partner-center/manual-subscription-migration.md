---
title: Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierter Angebote) auf neuere Versionen | Partner Center
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement Plan aus Basic (qualifizierter bietet) Abonnements kann nicht mehr erneuert werden.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Verlängern Sie Dynamics 365 bietet, Angebote, neue Dynamics 365-SKUs
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586943"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="41079-104">Migrieren von Dynamics 365 und Customer Engagement Plan von „Standard“ (qualifizierte Angebote) zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="41079-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="41079-105">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="41079-105">**Applies to**</span></span>

-  <span data-ttu-id="41079-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="41079-106">Partner Center</span></span>

<span data-ttu-id="41079-107">Effektive am 1. Januar 2019-Kunden mit Dynamics 365 for Sales / Customer Engagement Plan aus Basic (qualifizierter bietet) Abonnements kann diese älteren Angebote; nicht mehr verlängern vorhandene Abonnements werden nicht automatisch verlängert werden, wenn diese ablaufen.</span><span class="sxs-lookup"><span data-stu-id="41079-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="41079-108">Auf der Detailseite des Abonnements ändert der Abonnementstatus zu "Läuft ab am [Datum]" sich von "erneuert automatisch am [Datum]".</span><span class="sxs-lookup"><span data-stu-id="41079-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="41079-109">Zur Sicherstellung der Kontinuität für Kunden, sollten Sie mit dem abgelaufene Abonnements für eine unterstützte Option, die unten aufgeführten übergehen.</span><span class="sxs-lookup"><span data-stu-id="41079-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="41079-110">Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="41079-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="41079-111">Wenn Sie die API (CREST oder Partner Center) verwenden, finden Sie Verlängerung von ablaufenden Abonnements durch die das Enddatum des Abonnements sowie die automatische Auswertung = "false"-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="41079-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="41079-112">Die betreffenden Abonnements auf auto festgelegt erneuern = False auf 1. Januar 2019.</span><span class="sxs-lookup"><span data-stu-id="41079-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="41079-113">Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="41079-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="41079-114">Die Dynamics 365 bietet eingestellt</span><span class="sxs-lookup"><span data-stu-id="41079-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="41079-115">Dynamics 365 für Sales, Enterprise Edition CRMOL Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-116">Dynamics 365 für Sales, Enterprise Edition CRMOL Basic (qualifizierter Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="41079-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="41079-117">Dynamics 365 für Sales, Enterprise Edition CRMOL Basic (qualifizierter Angebot) für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="41079-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="41079-118">Dynamics 365 für Sales, Enterprise Edition (Behördenpreise) CRMOL Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-119">Dynamics 365 für die Sales, Enterprise Edition von SA für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-120">Dynamics 365 für die Sales, Enterprise Edition von SA für CRM Basic (qualifizierter Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="41079-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="41079-121">Dynamics 365 für die Sales, Enterprise Edition von SA für CRM Basic (qualifizierter Angebot) für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="41079-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="41079-122">Dynamics 365 für Sales, Enterprise Edition (Behördenpreise), die von SA für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-123">Dynamics 365 für Sales, Enterprise Edition-Add-On für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-124">Dynamics 365 für Sales, Enterprise Edition-Add-On für CRM Basic (qualifizierter Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="41079-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="41079-125">Dynamics 365 für Sales, Enterprise Edition-Add-On für CRM Basic (qualifizierter Angebot) für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="41079-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="41079-126">Dynamics 365 für Sales, Enterprise Edition (Behördenpreise)-Add-On für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) CRMOL Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierter Angebot) für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="41079-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="41079-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifizierter Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="41079-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="41079-131">Dynamics 365 Customer Engagement Plan Enterprise Edition von SA für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) von SA für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-133">Dynamics 365 Customer Engagement Plan Enterprise Edition von SA für CRM Basic (qualifizierter Angebot) für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="41079-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="41079-134">Dynamics 365 Customer Engagement Plan Enterprise Edition von SA für CRM Basic (qualifizierter Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="41079-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="41079-135">Dynamics 365 Customer Engagement Plan Enterprise Edition-Add-On für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise)-Add-On für CRM Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-137">Dynamics 365 Customer Engagement Plan Enterprise Edition-Add-On für CRM Basic (qualifizierter Angebot) für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="41079-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="41079-138">Dynamics 365 Customer Engagement Plan Enterprise Edition-Add-On für CRM Basic (qualifizierter Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="41079-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="41079-139">Dynamics 365 for Sales / Customer Engagement Planen von Basic (qualifizierter bietet) Ersatz-Pläne</span><span class="sxs-lookup"><span data-stu-id="41079-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="41079-140">**Abgelaufene Angebote**</span><span class="sxs-lookup"><span data-stu-id="41079-140">**Retired offers**</span></span>   

- <span data-ttu-id="41079-141">Dynamics 365 für den Vertrieb von CRM-Basic oder CRMOL Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="41079-142">Dynamics 365 Customer Engagement-Plan aus CRM Basic "oder" CRMOL Basic (qualifizierter Angebot)</span><span class="sxs-lookup"><span data-stu-id="41079-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="41079-143">**Optionen für das Ersetzen**</span><span class="sxs-lookup"><span data-stu-id="41079-143">**Replacement options**</span></span>
- <span data-ttu-id="41079-144">Dynamics 365 für Sales Professional (neu)</span><span class="sxs-lookup"><span data-stu-id="41079-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="41079-145">Dynamics 365 für Sales Professional (neu)</span><span class="sxs-lookup"><span data-stu-id="41079-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="41079-146">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="41079-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="41079-147">Dynamics 365 Customer Engagement-Plan oder</span><span class="sxs-lookup"><span data-stu-id="41079-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="41079-148">Dynamics 365-Team-Mitglieder</span><span class="sxs-lookup"><span data-stu-id="41079-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="41079-149">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="41079-149">Transition customers to new product plans</span></span>

<span data-ttu-id="41079-150">Verschieben von Kunden aus deaktivierten SKUs in neuere erfordert die folgenden Schritte aus, in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="41079-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="41079-151">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="41079-151">Purchase the new subscription</span></span>
- <span data-ttu-id="41079-152">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="41079-152">Reassign current user licenses</span></span>
- <span data-ttu-id="41079-153">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="41079-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="41079-154">Den neuen Plan für Ihre Kunden erwerben</span><span class="sxs-lookup"><span data-stu-id="41079-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="41079-155">Wählen Sie **Kunden** aus den linken Navigationsbereich, und wählen Sie dann den Kunden, die Sie in das neue Abonnement verschieben möchten.</span><span class="sxs-lookup"><span data-stu-id="41079-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="41079-156">Wählen Sie **-Abonnement hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="41079-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="41079-157">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="41079-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="41079-158">Ihre Kunden haben jetzt sowohl das alte Abonnement und den neuen Wert.</span><span class="sxs-lookup"><span data-stu-id="41079-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="41079-159">Der nächste Schritt ist für die neuzuweisung von Lizenzen, um den Kunden eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="41079-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="41079-160">Wählen Sie **Kunden** aus den linken Navigationsbereich, und wählen Sie dann den Kunden möchten verschieben.</span><span class="sxs-lookup"><span data-stu-id="41079-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="41079-161">Wählen Sie **Benutzer und Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="41079-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="41079-162">Um eine Lizenz zu einem Benutzer neu zuweisen möchten, wählen Sie den Benutzer aus, und wählen Sie dann **Verwalten von Lizenzen**.</span><span class="sxs-lookup"><span data-stu-id="41079-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="41079-163">Auf der **Verwalten von Lizenzen** Seite, deaktivieren Sie die Dynamics 365 for Sales / Customer Engagement-Plan von Basic (qualifizierter bieten) lizenzieren Sie das Kontrollkästchen, und wählen Sie einen neuen Dienstplan für das Abonnement des Kunden auf verschoben wurde.</span><span class="sxs-lookup"><span data-stu-id="41079-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="41079-164">Wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="41079-164">Select **Submit**.</span></span> <span data-ttu-id="41079-165">Sie werden für jeden Benutzer so vorgehen, die die neue Lizenz benötigt.</span><span class="sxs-lookup"><span data-stu-id="41079-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="41079-166">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement Abbrechen.</span><span class="sxs-lookup"><span data-stu-id="41079-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="41079-167">Wählen Sie **Kunden** aus den linken Navigationsbereich, und wählen Sie dann den Kunden möchten verschieben.</span><span class="sxs-lookup"><span data-stu-id="41079-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="41079-168">Legen Sie auf der Detailseite des Abonnements, auf das alte Abonnement **Suspended** , und wählen Sie **senden**.</span><span class="sxs-lookup"><span data-stu-id="41079-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="41079-169">Das alte Abonnement ist jetzt angehalten, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="41079-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="41079-170">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="41079-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="41079-171">Ihre Kunden fallen keine zusätzlichen Kosten für das alte Abonnement auf.</span><span class="sxs-lookup"><span data-stu-id="41079-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



