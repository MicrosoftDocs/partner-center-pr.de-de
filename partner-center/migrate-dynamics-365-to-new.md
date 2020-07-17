---
title: Dynamics 365 Business Edition migrieren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie qualifizierte Dynamics 365 Business Edition-Angebote zu neueren Versionen migrieren, bevor Sie ablaufen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436829"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="8b86c-103">Migrieren von Dynamics 365 Business Edition-Angeboten zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="8b86c-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="8b86c-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="8b86c-104">**Applies to**</span></span>

- <span data-ttu-id="8b86c-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="8b86c-105">Partner Center</span></span>

<span data-ttu-id="8b86c-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="8b86c-106">**Appropriate roles**</span></span>
- <span data-ttu-id="8b86c-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8b86c-107">Global admin</span></span>
- <span data-ttu-id="8b86c-108">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="8b86c-108">User admin</span></span>
- <span data-ttu-id="8b86c-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="8b86c-109">Admin agent</span></span>
- <span data-ttu-id="8b86c-110">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="8b86c-110">Sales agent</span></span>

<span data-ttu-id="8b86c-111">Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 Business Edition-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="8b86c-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="8b86c-112">Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]".</span><span class="sxs-lookup"><span data-stu-id="8b86c-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="8b86c-113">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.).</span><span class="sxs-lookup"><span data-stu-id="8b86c-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="8b86c-114">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="8b86c-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="8b86c-115">Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln.</span><span class="sxs-lookup"><span data-stu-id="8b86c-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="8b86c-116">Die betreffenden Abonnements werden am 1. Januar 2019 auf „auto renew=False“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="8b86c-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="8b86c-117">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="8b86c-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="8b86c-118">Die folgenden Dynamics 365 Business Editions werden eingestellt</span><span class="sxs-lookup"><span data-stu-id="8b86c-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="8b86c-119">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="8b86c-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="8b86c-120">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="8b86c-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="8b86c-121">Dynamics Business Central – die neuen Dynamics 365 Business Edition-Angebote</span><span class="sxs-lookup"><span data-stu-id="8b86c-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="8b86c-122">Mit den neuen Dynamics Business Central-Angeboten können Ihre Kunden Bereiche wie Finanzen, Vertrieb, Service und operatives Geschäft verbinden, um Geschäftsprozesse zu optimieren, die Kundeninteraktionen zu verbessern und bessere Entscheidungen zu treffen.</span><span class="sxs-lookup"><span data-stu-id="8b86c-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="8b86c-123">Dynamics 365 Business Central ist cloudbasiert und nur über Cloud Solution Provider (CSP)-Partner erhältlich.</span><span class="sxs-lookup"><span data-stu-id="8b86c-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="8b86c-124">Dynamics 365 Business Edition-Kunden erhalten bis zum 30. Juni 2020 Migrationsrabatte für die neuen Business Central-Angebote.</span><span class="sxs-lookup"><span data-stu-id="8b86c-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8b86c-125">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="8b86c-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="8b86c-126">Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="8b86c-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="8b86c-127">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="8b86c-127">Purchase the new subscription</span></span>
- <span data-ttu-id="8b86c-128">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="8b86c-128">Reassign current user licenses</span></span>
- <span data-ttu-id="8b86c-129">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="8b86c-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="8b86c-130">Kaufen des neuen Plans für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="8b86c-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="8b86c-131">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="8b86c-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="8b86c-132">Wählen Sie **Abonnement hinzufügen**aus.</span><span class="sxs-lookup"><span data-stu-id="8b86c-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="8b86c-133">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="8b86c-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="8b86c-134">Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement.</span><span class="sxs-lookup"><span data-stu-id="8b86c-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="8b86c-135">Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="8b86c-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="8b86c-136">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="8b86c-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8b86c-137">Wählen Sie **Benutzer und Lizenzen**aus.</span><span class="sxs-lookup"><span data-stu-id="8b86c-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="8b86c-138">Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="8b86c-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="8b86c-139">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="8b86c-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="8b86c-140">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="8b86c-140">Select **Submit**.</span></span> <span data-ttu-id="8b86c-141">Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen.</span><span class="sxs-lookup"><span data-stu-id="8b86c-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="8b86c-142">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement stornieren.</span><span class="sxs-lookup"><span data-stu-id="8b86c-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="8b86c-143">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="8b86c-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8b86c-144">Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="8b86c-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="8b86c-145">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="8b86c-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="8b86c-146">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="8b86c-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8b86c-147">Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="8b86c-147">Your customer will incur no additional costs for the old subscription.</span></span>
