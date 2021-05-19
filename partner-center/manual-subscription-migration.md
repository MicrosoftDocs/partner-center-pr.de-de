---
title: Migrieren von qualifizierten Dynamics 365-Abonnements
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie von qualifizierten, grundlegenden Dynamics 365-Abonnements zu einem neuen Abonnement migrieren, bevor vorhandene Abonnements ablaufen.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151643"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="5f41d-103">Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierte Angebote) zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="5f41d-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="5f41d-104">**Geeignete Rollen:** globale | Benutzerverwaltungsadministrator | | des Administrator-Agents Vertriebsmitarbeiter</span><span class="sxs-lookup"><span data-stu-id="5f41d-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="5f41d-105">Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 for Sales/Customer Engagement Plan von Basic (qualifizierte Angebote)-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="5f41d-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="5f41d-106">Auf der Detailseite des Abonnements ändert sich der Abonnementstatus von "Automatische Verlängerung am [Datum]" in "Läuft am [Datum]" ab.</span><span class="sxs-lookup"><span data-stu-id="5f41d-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="5f41d-107">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.).</span><span class="sxs-lookup"><span data-stu-id="5f41d-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="5f41d-108">Es wird empfohlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienstausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="5f41d-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="5f41d-109">Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln.</span><span class="sxs-lookup"><span data-stu-id="5f41d-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="5f41d-110">Die betreffenden Abonnements werden am 1. Januar 2019 auf Auto Renew=False festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f41d-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="5f41d-111">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="5f41d-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="5f41d-112">Die folgenden Dynamics 365-Angebote werden eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f41d-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="5f41d-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5f41d-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="5f41d-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5f41d-116">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5f41d-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5f41d-120">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5f41d-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="5f41d-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5f41d-124">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="5f41d-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5f41d-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5f41d-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="5f41d-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5f41d-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5f41d-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="5f41d-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5f41d-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="5f41d-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="5f41d-137">Ersatzpläne für Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="5f41d-138">**Eingestellte Angebote**</span><span class="sxs-lookup"><span data-stu-id="5f41d-138">**Retired offers**</span></span>   

- <span data-ttu-id="5f41d-139">Dynamics 365 for Sales from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5f41d-140">Dynamics 365 Customer Engagement Plan from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="5f41d-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="5f41d-141">**Ersatzoptionen**</span><span class="sxs-lookup"><span data-stu-id="5f41d-141">**Replacement options**</span></span>
- <span data-ttu-id="5f41d-142">Dynamics 365 for Sales Professional (NEU)</span><span class="sxs-lookup"><span data-stu-id="5f41d-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="5f41d-143">Dynamics 365 for Sales Professional (NEU)</span><span class="sxs-lookup"><span data-stu-id="5f41d-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="5f41d-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="5f41d-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="5f41d-145">Dynamics 365 Customer Engagement Plan oder</span><span class="sxs-lookup"><span data-stu-id="5f41d-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="5f41d-146">Dynamics 365 Team Members</span><span class="sxs-lookup"><span data-stu-id="5f41d-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5f41d-147">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="5f41d-147">Transition customers to new product plans</span></span>

<span data-ttu-id="5f41d-148">Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="5f41d-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="5f41d-149">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="5f41d-149">Purchase the new subscription</span></span>
- <span data-ttu-id="5f41d-150">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="5f41d-150">Reassign current user licenses</span></span>
- <span data-ttu-id="5f41d-151">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="5f41d-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="5f41d-152">Kaufen des neuen Plans für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="5f41d-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="5f41d-153">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="5f41d-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="5f41d-154">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="5f41d-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="5f41d-155">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="5f41d-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="5f41d-156">Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement.</span><span class="sxs-lookup"><span data-stu-id="5f41d-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="5f41d-157">Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="5f41d-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="5f41d-158">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="5f41d-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="5f41d-159">Wählen Sie **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="5f41d-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="5f41d-160">Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="5f41d-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="5f41d-161">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="5f41d-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="5f41d-162">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="5f41d-162">Select **Submit**.</span></span> <span data-ttu-id="5f41d-163">Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen.</span><span class="sxs-lookup"><span data-stu-id="5f41d-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="5f41d-164">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement kündigen.</span><span class="sxs-lookup"><span data-stu-id="5f41d-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="5f41d-165">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="5f41d-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="5f41d-166">Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="5f41d-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="5f41d-167">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="5f41d-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="5f41d-168">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="5f41d-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="5f41d-169">Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="5f41d-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



