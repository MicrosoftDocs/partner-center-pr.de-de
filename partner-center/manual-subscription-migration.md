---
title: Migrieren qualifizierter Dynamics 365-Abonnements
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie von qualifizierten, grundlegenden Dynamics 365-Abonnements zu einem neuen Abonnement migrieren, bevor vorhandene Abonnements ablaufen.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132739"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="12508-103">Migrieren von Dynamics 365 und Customer Engagement Plan von Basic (qualifizierte Angebote) zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="12508-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="12508-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="12508-104">**Appropriate roles**</span></span>

- <span data-ttu-id="12508-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="12508-105">Global admin</span></span>
- <span data-ttu-id="12508-106">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="12508-106">User management admin</span></span>
- <span data-ttu-id="12508-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="12508-107">Admin agent</span></span>
- <span data-ttu-id="12508-108">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="12508-108">Sales agent</span></span>

<span data-ttu-id="12508-109">Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 for Sales/Customer Engagement Plan von Basic (qualifizierte Angebote)-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="12508-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="12508-110">Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]".</span><span class="sxs-lookup"><span data-stu-id="12508-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="12508-111">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.).</span><span class="sxs-lookup"><span data-stu-id="12508-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="12508-112">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="12508-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="12508-113">Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln.</span><span class="sxs-lookup"><span data-stu-id="12508-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="12508-114">Die fraglichen Abonnements werden am 1. Januar 2019 auf Auto Renew = false festgelegt.</span><span class="sxs-lookup"><span data-stu-id="12508-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="12508-115">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="12508-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="12508-116">Die folgenden Dynamics 365-Angebote werden eingestellt</span><span class="sxs-lookup"><span data-stu-id="12508-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="12508-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="12508-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="12508-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="12508-120">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="12508-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="12508-124">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="12508-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="12508-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="12508-128">Dynamics 365 for Sales Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="12508-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="12508-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="12508-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) From SA for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="12508-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="12508-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="12508-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Behördenpreise) Add-On for CRM Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Studenten</span><span class="sxs-lookup"><span data-stu-id="12508-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="12508-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (qualifiziertes Angebot) für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="12508-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="12508-141">Ersatzpläne für Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="12508-142">**Eingestellte Angebote**</span><span class="sxs-lookup"><span data-stu-id="12508-142">**Retired offers**</span></span>   

- <span data-ttu-id="12508-143">Dynamics 365 for Sales from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="12508-144">Dynamics 365 Customer Engagement Plan from CRM Basic oder CRMOL Basic (qualifiziertes Angebot)</span><span class="sxs-lookup"><span data-stu-id="12508-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="12508-145">**Ersatzoptionen**</span><span class="sxs-lookup"><span data-stu-id="12508-145">**Replacement options**</span></span>
- <span data-ttu-id="12508-146">Dynamics 365 for Sales Professional (NEU)</span><span class="sxs-lookup"><span data-stu-id="12508-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="12508-147">Dynamics 365 for Sales Professional (NEU)</span><span class="sxs-lookup"><span data-stu-id="12508-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="12508-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="12508-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="12508-149">Dynamics 365 Customer Engagement Plan oder</span><span class="sxs-lookup"><span data-stu-id="12508-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="12508-150">Dynamics 365 Team Members</span><span class="sxs-lookup"><span data-stu-id="12508-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="12508-151">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="12508-151">Transition customers to new product plans</span></span>

<span data-ttu-id="12508-152">Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="12508-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="12508-153">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="12508-153">Purchase the new subscription</span></span>
- <span data-ttu-id="12508-154">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="12508-154">Reassign current user licenses</span></span>
- <span data-ttu-id="12508-155">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="12508-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="12508-156">Kaufen des neuen Plans für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="12508-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="12508-157">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="12508-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="12508-158">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="12508-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="12508-159">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="12508-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="12508-160">Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement.</span><span class="sxs-lookup"><span data-stu-id="12508-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="12508-161">Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="12508-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="12508-162">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="12508-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="12508-163">Wählen Sie **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="12508-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="12508-164">Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="12508-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="12508-165">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="12508-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="12508-166">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="12508-166">Select **Submit**.</span></span> <span data-ttu-id="12508-167">Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen.</span><span class="sxs-lookup"><span data-stu-id="12508-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="12508-168">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement kündigen.</span><span class="sxs-lookup"><span data-stu-id="12508-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="12508-169">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="12508-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="12508-170">Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="12508-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="12508-171">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="12508-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="12508-172">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="12508-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="12508-173">Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="12508-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



