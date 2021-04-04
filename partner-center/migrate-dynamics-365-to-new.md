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
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132637"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="a4ece-103">Migrieren von Dynamics 365 Business Edition-Angeboten zu neueren Versionen</span><span class="sxs-lookup"><span data-stu-id="a4ece-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="a4ece-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="a4ece-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a4ece-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="a4ece-105">Global admin</span></span>
- <span data-ttu-id="a4ece-106">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="a4ece-106">User management admin</span></span>
- <span data-ttu-id="a4ece-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="a4ece-107">Admin agent</span></span>
- <span data-ttu-id="a4ece-108">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="a4ece-108">Sales agent</span></span>

<span data-ttu-id="a4ece-109">Ab dem 1. Januar 2019 können Kunden mit Dynamics 365 Business Edition-Abonnements diese bisherigen Angebote nicht mehr verlängern; vorhandene Abonnements werden nicht automatisch verlängert, wenn sie ablaufen.</span><span class="sxs-lookup"><span data-stu-id="a4ece-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="a4ece-110">Auf der Detailseite des Abonnements ändert sich der Abonnement Status in "läuft am [Date]" von "Auto erneuert on [Date]".</span><span class="sxs-lookup"><span data-stu-id="a4ece-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="a4ece-111">Um die Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements eine unterstützte Option anbieten (s. u.).</span><span class="sxs-lookup"><span data-stu-id="a4ece-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="a4ece-112">Wir empfehlen, Kunden vor dem jährlichen Enddatum des Abonnements in neue Abonnements zu verschieben, um Dienst Ausfälle für Kunden zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="a4ece-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="a4ece-113">Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung (auto renew) ermitteln.</span><span class="sxs-lookup"><span data-stu-id="a4ece-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="a4ece-114">Die fraglichen Abonnements werden am 1. Januar 2019 auf Auto Renew = false festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a4ece-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="a4ece-115">Sie können Kunden jederzeit in einen neuen Plan verschieben.</span><span class="sxs-lookup"><span data-stu-id="a4ece-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="a4ece-116">Die folgenden Dynamics 365 Business Editions werden eingestellt</span><span class="sxs-lookup"><span data-stu-id="a4ece-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="a4ece-117">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="a4ece-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="a4ece-118">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="a4ece-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="a4ece-119">Dynamics Business Central – die neuen Dynamics 365 Business Edition-Angebote</span><span class="sxs-lookup"><span data-stu-id="a4ece-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="a4ece-120">Mit den neuen Dynamics Business Central-Angeboten können Ihre Kunden Bereiche wie Finanzen, Vertrieb, Service und operatives Geschäft verbinden, um Geschäftsprozesse zu optimieren, die Kundeninteraktionen zu verbessern und bessere Entscheidungen zu treffen.</span><span class="sxs-lookup"><span data-stu-id="a4ece-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="a4ece-121">Dynamics 365 Business Central ist cloudbasiert und nur über Cloud Solution Provider (CSP)-Partner erhältlich.</span><span class="sxs-lookup"><span data-stu-id="a4ece-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="a4ece-122">Dynamics 365 Business Edition-Kunden erhalten bis zum 30. Juni 2020 Migrationsrabatte für die neuen Business Central-Angebote.</span><span class="sxs-lookup"><span data-stu-id="a4ece-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="a4ece-123">Migrieren von Kunden zu neuen Produktplänen</span><span class="sxs-lookup"><span data-stu-id="a4ece-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="a4ece-124">Die Migration von Kunden von eingestellten SKUs zu neueren SKUs erfordert die folgenden Schritte in der folgenden Reihenfolge:</span><span class="sxs-lookup"><span data-stu-id="a4ece-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="a4ece-125">Kauf des neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="a4ece-125">Purchase the new subscription</span></span>
- <span data-ttu-id="a4ece-126">Neuzuweisen der aktuellen Benutzerlizenzen</span><span class="sxs-lookup"><span data-stu-id="a4ece-126">Reassign current user licenses</span></span>
- <span data-ttu-id="a4ece-127">Stornieren des alten Abonnements</span><span class="sxs-lookup"><span data-stu-id="a4ece-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="a4ece-128">Kaufen des neuen Plans für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="a4ece-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="a4ece-129">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie zum neuen Abonnement migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="a4ece-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="a4ece-130">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="a4ece-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="a4ece-131">Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall eine der oben genannten Optionen), geben Sie die nötigen Anzahl von Lizenzen ein, und wählen Sie dann **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="a4ece-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="a4ece-132">Ihre Kunden haben jetzt sowohl das alte als auch das neue Abonnement.</span><span class="sxs-lookup"><span data-stu-id="a4ece-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="a4ece-133">Der nächste Schritt besteht darin, den Benutzern des Kunden Lizenzen neu zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="a4ece-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="a4ece-134">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="a4ece-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="a4ece-135">Wählen Sie **Benutzer und Lizenzen** aus.</span><span class="sxs-lookup"><span data-stu-id="a4ece-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="a4ece-136">Um einem Benutzer eine Lizenz zuzuweisen, wählen Sie den Benutzer aus, und wählen Sie anschließend **Lizenzen verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="a4ece-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="a4ece-137">Deaktivieren Sie auf der Seite **Lizenzen verwalten** das Kontrollkästchen für die Lizenz von Dynamics 365 for Sales/ Customer Engagement Plan from Basic (qualifiziertes Angebot), und wählen Sie einen neuen Serviceplan für das Abonnement aus, auf das der Kunde umgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="a4ece-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="a4ece-138">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="a4ece-138">Select **Submit**.</span></span> <span data-ttu-id="a4ece-139">Führen Sie diese Schritte für alle Benutzer aus, die eine neue Lizenz benötigen.</span><span class="sxs-lookup"><span data-stu-id="a4ece-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="a4ece-140">Nachdem Sie die Lizenzen in das neue Abonnement verschoben haben, können Sie das alte Abonnement kündigen.</span><span class="sxs-lookup"><span data-stu-id="a4ece-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="a4ece-141">Wählen Sie in der linken Navigationsleiste **Kunden** aus, und wählen Sie anschließend den Kunden aus, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="a4ece-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="a4ece-142">Legen Sie auf der Seite mit den Abonnementdetails das alte Abonnement auf **Ausgesetzt** fest, und wählen Sie **Übermitteln** aus.</span><span class="sxs-lookup"><span data-stu-id="a4ece-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="a4ece-143">Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="a4ece-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="a4ece-144">Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben.</span><span class="sxs-lookup"><span data-stu-id="a4ece-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="a4ece-145">Für Ihren Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.</span><span class="sxs-lookup"><span data-stu-id="a4ece-145">Your customer will incur no additional costs for the old subscription.</span></span>
