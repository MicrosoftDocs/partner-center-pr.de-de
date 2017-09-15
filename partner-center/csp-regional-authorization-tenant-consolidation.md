---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="be04e-103">CSP regional authorization tenant consolidation</span><span class="sxs-lookup"><span data-stu-id="be04e-103">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="be04e-104">Applies to</span><span class="sxs-lookup"><span data-stu-id="be04e-104">Applies to</span></span>**

-  <span data-ttu-id="be04e-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="be04e-105">Partner Center</span></span>
-  <span data-ttu-id="be04e-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="be04e-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="be04e-107">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="be04e-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="be04e-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span><span class="sxs-lookup"><span data-stu-id="be04e-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="be04e-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span><span class="sxs-lookup"><span data-stu-id="be04e-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="be04e-110">Use these instructions to consolidate tenants for different country/regions.</span><span class="sxs-lookup"><span data-stu-id="be04e-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="be04e-111">**Hinweis:** Sie müssen alle Abonnements und die Anzahl von Arbeitsplätzen für Ihre Kunden kennen, die über die Übergangskonten bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="be04e-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="be04e-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span><span class="sxs-lookup"><span data-stu-id="be04e-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="be04e-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span><span class="sxs-lookup"><span data-stu-id="be04e-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="be04e-114">Partners choose to consolidate their tenants.</span><span class="sxs-lookup"><span data-stu-id="be04e-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="be04e-115">Once consolidation is complete, Partners cannot revert to their previous state.</span><span class="sxs-lookup"><span data-stu-id="be04e-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="be04e-116">Note that customer action is also be required.</span><span class="sxs-lookup"><span data-stu-id="be04e-116">Note that customer action is also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="be04e-117">Prepare for migration</span><span class="sxs-lookup"><span data-stu-id="be04e-117">Prepare for migration</span></span>


-   <span data-ttu-id="be04e-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span><span class="sxs-lookup"><span data-stu-id="be04e-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="be04e-120">Migrate customer accounts</span><span class="sxs-lookup"><span data-stu-id="be04e-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="be04e-121">Melden Sie sich mit dem zu migrierenden (vorhandenen) Konto unter <https://partnercenter.microsoft.com> an, und navigieren Sie auf dem Partner Center-Dashboard zur Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="be04e-121">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="be04e-122">Select Customer.</span><span class="sxs-lookup"><span data-stu-id="be04e-122">Select Customer.</span></span>

3.  <span data-ttu-id="be04e-123">Klicken Sie auf **Vertriebspartnerschaft beantragen**.</span><span class="sxs-lookup"><span data-stu-id="be04e-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="be04e-124">You are presented with a default email message to present to your customers.</span><span class="sxs-lookup"><span data-stu-id="be04e-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="be04e-125">This message contains a URL with the org ID unique to your new Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="be04e-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="be04e-126">**Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen.</span><span class="sxs-lookup"><span data-stu-id="be04e-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="be04e-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span><span class="sxs-lookup"><span data-stu-id="be04e-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="be04e-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span><span class="sxs-lookup"><span data-stu-id="be04e-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="be04e-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span><span class="sxs-lookup"><span data-stu-id="be04e-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="be04e-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span><span class="sxs-lookup"><span data-stu-id="be04e-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="be04e-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span><span class="sxs-lookup"><span data-stu-id="be04e-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="be04e-132">Migrating Office 365 and non-Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="be04e-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="be04e-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span><span class="sxs-lookup"><span data-stu-id="be04e-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="be04e-134">Klicken Sie auf dem PartnerCenter-Dashboard im linken Navigationsmenü auf **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="be04e-134">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="be04e-135">Open the company name for the customer you want to migrate.</span><span class="sxs-lookup"><span data-stu-id="be04e-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="be04e-136">Klicken Sie auf **Abonnement hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="be04e-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="be04e-137">Add the correct subscriptions and seat counts from the catalog.</span><span class="sxs-lookup"><span data-stu-id="be04e-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="be04e-138">Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.</span><span class="sxs-lookup"><span data-stu-id="be04e-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  <span data-ttu-id="be04e-140">Klicken Sie auf **Übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="be04e-140">Click **Submit.**</span></span>

<span data-ttu-id="be04e-141">Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="be04e-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="be04e-142">Repeat these steps to migrate subscriptions for all additional customers.</span><span class="sxs-lookup"><span data-stu-id="be04e-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="be04e-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span><span class="sxs-lookup"><span data-stu-id="be04e-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="be04e-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="be04e-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="be04e-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span><span class="sxs-lookup"><span data-stu-id="be04e-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="be04e-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span><span class="sxs-lookup"><span data-stu-id="be04e-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="be04e-147">Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr.</span><span class="sxs-lookup"><span data-stu-id="be04e-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="be04e-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span><span class="sxs-lookup"><span data-stu-id="be04e-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="be04e-149">Melden Sie sich mit dem CSP-Konto vom Typ **Transitioning From** unter <https://partnercenter.microsoft.com> an, und navigieren Sie zur Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="be04e-149">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="be04e-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span><span class="sxs-lookup"><span data-stu-id="be04e-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="be04e-151">Legen Sie für das Abonnement **suspended** fest, und klicken Sie anschließend auf **Übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="be04e-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="be04e-152">**Hinweis:** Durch Aussetzen des Abonnements wird sichergestellt, dass die Abrechnung nicht doppelt erfolgt.</span><span class="sxs-lookup"><span data-stu-id="be04e-152">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="be04e-153">Für das Abonnement wird in der Abonnementliste **suspended** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="be04e-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="be04e-154">Repeat these steps for all subscriptions under the customer.</span><span class="sxs-lookup"><span data-stu-id="be04e-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="be04e-155">Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="be04e-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="be04e-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span><span class="sxs-lookup"><span data-stu-id="be04e-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="be04e-157">Migrating Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="be04e-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="be04e-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span><span class="sxs-lookup"><span data-stu-id="be04e-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="be04e-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span><span class="sxs-lookup"><span data-stu-id="be04e-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="be04e-160">There will be no disruption of service to the customer during this transition.</span><span class="sxs-lookup"><span data-stu-id="be04e-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="be04e-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span><span class="sxs-lookup"><span data-stu-id="be04e-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="be04e-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span><span class="sxs-lookup"><span data-stu-id="be04e-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="be04e-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span><span class="sxs-lookup"><span data-stu-id="be04e-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="be04e-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="be04e-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="be04e-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="be04e-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="be04e-166">**Hinweis:** Durch die Deaktivierung der Abonnements im Kundeneintrag wird nicht die Darstellung des Kunden in der Kundenliste geändert.</span><span class="sxs-lookup"><span data-stu-id="be04e-166">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="be04e-167">There is currently no option to remove customers from the list.</span><span class="sxs-lookup"><span data-stu-id="be04e-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="be04e-168">Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.</span><span class="sxs-lookup"><span data-stu-id="be04e-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="be04e-169">Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="be04e-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="be04e-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span><span class="sxs-lookup"><span data-stu-id="be04e-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="be04e-171">No future invoices will generate after that final billing period.</span><span class="sxs-lookup"><span data-stu-id="be04e-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="be04e-172">Notes</span><span class="sxs-lookup"><span data-stu-id="be04e-172">Notes</span></span>

-   <span data-ttu-id="be04e-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span><span class="sxs-lookup"><span data-stu-id="be04e-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="be04e-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span><span class="sxs-lookup"><span data-stu-id="be04e-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="be04e-175">There is currently no way to remove a customer from the Customers list completely.</span><span class="sxs-lookup"><span data-stu-id="be04e-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="be04e-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="be04e-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="be04e-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span><span class="sxs-lookup"><span data-stu-id="be04e-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="be04e-178">Simplify migration using Export</span><span class="sxs-lookup"><span data-stu-id="be04e-178">Simplify migration using Export</span></span>

<span data-ttu-id="be04e-179">Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:</span><span class="sxs-lookup"><span data-stu-id="be04e-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="be04e-180">Klicken Sie auf dem Dashboard auf **Kunden**, um die Liste der Kunden in der vorhandenen Struktur anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="be04e-180">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="be04e-181">Open the desired customer name.</span><span class="sxs-lookup"><span data-stu-id="be04e-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="be04e-182">Klicken Sie auf der Seite **Abonnements** auf **Export Subscriptions**, um Details zu Abonnements in eine Excel-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="be04e-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="be04e-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span><span class="sxs-lookup"><span data-stu-id="be04e-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="be04e-184">API registration</span><span class="sxs-lookup"><span data-stu-id="be04e-184">API registration</span></span>

<span data-ttu-id="be04e-185">Weitere Informationen zur API-Registrierung finden Sie in [auf dieser Seite](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="be04e-185">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="be04e-186">Partner Center Activity log</span><span class="sxs-lookup"><span data-stu-id="be04e-186">Partner Center Activity log</span></span>


<span data-ttu-id="be04e-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span><span class="sxs-lookup"><span data-stu-id="be04e-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="be04e-188">This helps partners track changes on a customer tenant.</span><span class="sxs-lookup"><span data-stu-id="be04e-188">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="be04e-189">View the Activity log</span><span class="sxs-lookup"><span data-stu-id="be04e-189">View the Activity log</span></span>**

1.  <span data-ttu-id="be04e-190">Klicken Sie auf dem Partner Center-Dashboard auf den Link **Aktivitätsprotokoll**.</span><span class="sxs-lookup"><span data-stu-id="be04e-190">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="be04e-191">Sehen Sie sich auf der Seite **Aktivitätsprotokoll** die Änderungen an, die an Kundenkonten vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="be04e-191">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="be04e-192">Wählen Sie zum Filtern des Aktivitätsprotokolls nach **Datum Start-** und **Enddatum** aus, um die ausgewählten Einträge im Protokoll einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="be04e-192">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="be04e-193">Verwenden Sie das Suchfeld, um im **Aktivitätsprotokoll** nach Kunde zu filtern.</span><span class="sxs-lookup"><span data-stu-id="be04e-193">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="be04e-194">Export the Activity log</span><span class="sxs-lookup"><span data-stu-id="be04e-194">Export the Activity log</span></span>**

-   <span data-ttu-id="be04e-195">Klicken Sie auf **Export log**, um die Daten Ihres Aktivitätsprotokolls in eine CSV-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="be04e-195">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="be04e-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span><span class="sxs-lookup"><span data-stu-id="be04e-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



