---
title: Dynamics 365 Business Edition migrieren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie qualifizierte Dynamics 365 Business Edition-Angebote zu neueren Versionen migrieren, bevor Sie ablaufen.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365-Angebote, Angebote verlängern, neue Dynamics 365-SKUs
ms.openlocfilehash: d49966db4a2c9de50b0723abf9ccd0fe589a442a
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795968"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="b3c45-104">Migrieren von Dynamics 365 Business Edition-Angeboten zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="b3c45-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="b3c45-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="b3c45-105">**Applies to**</span></span>

- <span data-ttu-id="b3c45-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="b3c45-106">Partner Center</span></span>

<span data-ttu-id="b3c45-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="b3c45-107">**Appropriate roles**</span></span>
- <span data-ttu-id="b3c45-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b3c45-108">Global admin</span></span>
- <span data-ttu-id="b3c45-109">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="b3c45-109">User admin</span></span>
- <span data-ttu-id="b3c45-110">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="b3c45-110">Admin agent</span></span>
- <span data-ttu-id="b3c45-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="b3c45-111">Sales agent</span></span>

<span data-ttu-id="b3c45-112">Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 Business Edition-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="b3c45-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="b3c45-113">Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]".</span><span class="sxs-lookup"><span data-stu-id="b3c45-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="b3c45-114">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.).</span><span class="sxs-lookup"><span data-stu-id="b3c45-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="b3c45-115">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="b3c45-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b3c45-116">Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln.</span><span class="sxs-lookup"><span data-stu-id="b3c45-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b3c45-117">Die betreffenden Abonnements werden am 1. Januar 2019 auf „auto renew=False“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b3c45-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="b3c45-118">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="b3c45-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="b3c45-119">Die folgenden Dynamics 365 Business Editions werden eingestellt</span><span class="sxs-lookup"><span data-stu-id="b3c45-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="b3c45-120">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="b3c45-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="b3c45-121">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="b3c45-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="b3c45-122">Dynamics Business Central – die neuen Dynamics 365 Business Edition-Angebote</span><span class="sxs-lookup"><span data-stu-id="b3c45-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="b3c45-123">Mit den neuen Dynamics Business Central-Angeboten können Ihre Kunden Bereiche wie Finanzen, Vertrieb, Service und operatives Geschäft verbinden, um Geschäftsprozesse zu optimieren, die Kundeninteraktionen zu verbessern und bessere Entscheidungen zu treffen.</span><span class="sxs-lookup"><span data-stu-id="b3c45-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="b3c45-124">Dynamics 365 Business Central ist cloudbasiert und nur über Cloud Solution Provider (CSP)-Partner erhältlich.</span><span class="sxs-lookup"><span data-stu-id="b3c45-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="b3c45-125">Dynamics 365 Business Edition-Kunden erhalten bis zum 30. Juni 2020 Migrationsrabatte für die neuen Business Central-Angebote.</span><span class="sxs-lookup"><span data-stu-id="b3c45-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b3c45-126">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="b3c45-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="b3c45-127">Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="b3c45-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="b3c45-128">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="b3c45-128">Purchase the new subscription</span></span>
- <span data-ttu-id="b3c45-129">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="b3c45-129">Reassign current user licenses</span></span>
- <span data-ttu-id="b3c45-130">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="b3c45-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="b3c45-131">Kaufen des neuen Plans für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="b3c45-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="b3c45-132">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="b3c45-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="b3c45-133">Wählen Sie **Abonnement hinzufügen**aus.</span><span class="sxs-lookup"><span data-stu-id="b3c45-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="b3c45-134">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="b3c45-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b3c45-135">Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement.</span><span class="sxs-lookup"><span data-stu-id="b3c45-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="b3c45-136">Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="b3c45-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="b3c45-137">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="b3c45-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b3c45-138">Wählen Sie **Benutzer und Lizenzen**aus.</span><span class="sxs-lookup"><span data-stu-id="b3c45-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="b3c45-139">Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="b3c45-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="b3c45-140">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="b3c45-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="b3c45-141">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="b3c45-141">Select **Submit**.</span></span> <span data-ttu-id="b3c45-142">Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen.</span><span class="sxs-lookup"><span data-stu-id="b3c45-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="b3c45-143">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement stornieren.</span><span class="sxs-lookup"><span data-stu-id="b3c45-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="b3c45-144">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="b3c45-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b3c45-145">Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="b3c45-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="b3c45-146">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="b3c45-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="b3c45-147">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="b3c45-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b3c45-148">Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="b3c45-148">Your customer will incur no additional costs for the old subscription.</span></span>
