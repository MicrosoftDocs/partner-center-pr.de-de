---
title: Mandantenkonsolidierung für regionale CSP-Autorisierung
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen. Dies umfasst schritte zum Migrieren von Kundenkonten und Kundenabonnements.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276874"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="e3176-104">Anweisungen zur Mandantenkonsolidierung für regionale CSP-Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e3176-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="e3176-105">**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e3176-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e3176-106">**Geeignete Rollen**: Globaler Administrator | Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="e3176-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="e3176-107">\[Einige Informationen beziehen sich auf Vorabversionen, die vor der kommerziellen Freigabe grundlegend geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="e3176-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="e3176-108">Microsoft übernimmt keine Garantie, weder ausdrücklich noch stillschweigend, für die hier bereitgestellten Informationen.\]</span><span class="sxs-lookup"><span data-stu-id="e3176-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="e3176-109">Sie können Mandanten für Ihr Unternehmen konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="e3176-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="e3176-110">Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.</span><span class="sxs-lookup"><span data-stu-id="e3176-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="e3176-111">Sie müssen alle bereitgestellten Abonnements und Lizenzanzahlen für jeden Ihrer Kunden in dem Konto kennen, von dem Sie den Übergang unternehmen.</span><span class="sxs-lookup"><span data-stu-id="e3176-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="e3176-112">Sie werden genau diese Abonnements mit der gleichen Lizenzanzahl im Rahmen des Migrationsprozesses unter dem neuen zentralen CSP-Konto erneut bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="e3176-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="e3176-113">Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e3176-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="e3176-114">Nach Abschluss der Konsolidierung können Sie nicht mehr auf den vorherigen Mandantenstatus zurückverwenden.</span><span class="sxs-lookup"><span data-stu-id="e3176-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="e3176-115">Möglicherweise ist auch eine Kundenaktion erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3176-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="e3176-116">Vorbereiten der Migration</span><span class="sxs-lookup"><span data-stu-id="e3176-116">Prepare for migration</span></span>

- <span data-ttu-id="e3176-117">Melden Sie sich **bei** Partner Center  mithilfe des Übergangskontos (das Konto, das Sie auf das neue Konto umstiegen) an, und überprüfen Sie alle Kunden und alle Dienste, die für diese Kunden bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e3176-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="e3176-118">Melden Sie sich von diesem Konto ab.</span><span class="sxs-lookup"><span data-stu-id="e3176-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="e3176-119">Migrieren von Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="e3176-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="e3176-120">Melden Sie sich **mit Partner Center** **(neues)** Konto (dem Konto, in das Sie Kunden umstiegen) bei ihrem Konto an.</span><span class="sxs-lookup"><span data-stu-id="e3176-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="e3176-121">Wählen Sie **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="e3176-121">Select **Customers**.</span></span>

3. <span data-ttu-id="e3176-122">Wählen Sie **Handelspartnerbeziehung anfordern aus.**</span><span class="sxs-lookup"><span data-stu-id="e3176-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="e3176-123">Ihnen wird eine Standard-E-Mail-Nachricht angezeigt, die an Ihre Kunden gesendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e3176-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="e3176-124">Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues Partner Center-Konto.</span><span class="sxs-lookup"><span data-stu-id="e3176-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="e3176-125">**Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen.</span><span class="sxs-lookup"><span data-stu-id="e3176-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="e3176-126">Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office 365-Portal aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="e3176-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="e3176-127">Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office 365 zugreift.</span><span class="sxs-lookup"><span data-stu-id="e3176-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="e3176-128">Nach der Anmeldung wird der  globale Administrator für das Kundenkonto aufgefordert, eine Vereinbarung zu übermitteln, die dem neuen CSP-Konto delegierte Administratorrechte erteilt.</span><span class="sxs-lookup"><span data-stu-id="e3176-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="e3176-129">Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.</span><span class="sxs-lookup"><span data-stu-id="e3176-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="e3176-130">Die Kunden werden in der Kundenliste des Partners angezeigt, nachdem sie die Vereinbarung 1:1 übermittelt haben.</span><span class="sxs-lookup"><span data-stu-id="e3176-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="e3176-131">Migrieren von nutzungsbasierten Office 365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)</span><span class="sxs-lookup"><span data-stu-id="e3176-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="e3176-132">Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.</span><span class="sxs-lookup"><span data-stu-id="e3176-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="e3176-133">Wählen **Partner Center** aus, und wählen **Sie Kunden aus.**</span><span class="sxs-lookup"><span data-stu-id="e3176-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="e3176-134">Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="e3176-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="e3176-135">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="e3176-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="e3176-136">Fügen Sie die richtigen Abonnements und Lizenzanzahlen aus dem Katalog hinzu.</span><span class="sxs-lookup"><span data-stu-id="e3176-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="e3176-137">Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.</span><span class="sxs-lookup"><span data-stu-id="e3176-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Kundenliste.":::

6. <span data-ttu-id="e3176-139">Wählen Sie **Senden aus.**</span><span class="sxs-lookup"><span data-stu-id="e3176-139">Select **Submit.**</span></span>

   <span data-ttu-id="e3176-140">Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="e3176-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="e3176-141">Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="e3176-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="e3176-142">Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="e3176-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="e3176-143">Partner müssen Abonnements für das Konto "Übergang vom Partner-Mandanten" in Partner Center an dem Tag  aussetzen, an dem diese Abonnements über das Konto "Übergang zum Partner-Mandanten" in der Partner Center eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt. </span><span class="sxs-lookup"><span data-stu-id="e3176-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="e3176-144">Supportanfragen für Guthaben werden aufgrund von Überschneidungen bei der Abrechnung abgelehnt, die auftreten, wenn die Umstellung von **Abonnements nicht ordnungsgemäß deaktiviert** wird.</span><span class="sxs-lookup"><span data-stu-id="e3176-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="e3176-145">Deaktivieren der Office 365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“</span><span class="sxs-lookup"><span data-stu-id="e3176-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="e3176-146">Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr.</span><span class="sxs-lookup"><span data-stu-id="e3176-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="e3176-147">Sie müssen Azure-Abonnements nicht manuell deaktivieren, da Azure-Abonnements während des Migrationsprozesses automatisch deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="e3176-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="e3176-148">Melden Sie sich im **Partner Center** mit dem CSP-Konto **Wechsel von** an, und navigieren Sie zur Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="e3176-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="e3176-149">Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.</span><span class="sxs-lookup"><span data-stu-id="e3176-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="e3176-150">Legen Sie das Abonnement auf **angehalten fest,** und wählen Sie dann **Übermitteln aus.**</span><span class="sxs-lookup"><span data-stu-id="e3176-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="e3176-151">Durch das Aussetzen des Abonnements wird sichergestellt, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="e3176-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="e3176-152">Das Abonnement wird **in der Abonnementliste** als angehalten angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e3176-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="e3176-153">Wiederholen Sie diese Schritte für alle Abonnements des Kunden.</span><span class="sxs-lookup"><span data-stu-id="e3176-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="e3176-154">Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3176-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="e3176-155">Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.</span><span class="sxs-lookup"><span data-stu-id="e3176-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="e3176-156">Migrieren von nutzungsbasierten Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="e3176-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="e3176-157">Im Gegensatz zu Office 365-CSP-Abonnements, Azure, müssen nutzungsbasierte CSP-Abonnements nicht manuell migriert werden.</span><span class="sxs-lookup"><span data-stu-id="e3176-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="e3176-158">Microsoft Azure-Support migriert die Azure-Abonnements und alle bereitgestellten  Dienste oder Ressourcen von  den CSP-Vertriebspartnerkonten in das CSP-Handelspartnerkonto.</span><span class="sxs-lookup"><span data-stu-id="e3176-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="e3176-159">Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.</span><span class="sxs-lookup"><span data-stu-id="e3176-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="e3176-160">Stellen Sie sicher, dass die Kundenkonten, für die Azure-Abonnements  migriert werden, die Vereinbarung akzeptiert haben, die dem neuen CSP-Konto für den Übergang zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e3176-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="e3176-161">Sie benachrichtigen Microsoft darüber, welche Kundenkonten migriert werden können, und geben die Unternehmensnamen dieser Kunden an.</span><span class="sxs-lookup"><span data-stu-id="e3176-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="e3176-162">Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt Sie, wenn die Migration abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="e3176-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="e3176-163">Sie müssen bestätigen, dass das Azure-Abonnement unter dem CSP-Handelspartnerkonto **"Übergang** vom CSP" jetzt im Abschnitt "Kundenabonnements" **in** der Partner Center als angehalten markiert ist.</span><span class="sxs-lookup"><span data-stu-id="e3176-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="e3176-164">Vergewissern Sie sich, dass das Azure-Abonnement unter **dem** CSP-Vertriebspartnerkonto jetzt im Abschnitt Kundenabonnements den Status aktiv **in** Partner Center angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3176-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="e3176-165">Das Deaktivieren der Abonnements unter dem Kunden ändert nicht die Darstellung des Kunden in der Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="e3176-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="e3176-166">Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="e3176-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="e3176-167">Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.</span><span class="sxs-lookup"><span data-stu-id="e3176-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="e3176-168">Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="e3176-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="e3176-169">Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="e3176-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="e3176-170">Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.</span><span class="sxs-lookup"><span data-stu-id="e3176-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="e3176-171">Zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="e3176-171">Additional information</span></span>

- <span data-ttu-id="e3176-172">Das Deaktivieren des Abonnements aus dem CSP-Konto "Übergang vom" wirkt sich nicht auf  den Dienst des Endkunden aus, solange der Dienst aus dem CSP-Konto für den Übergang bereitgestellt wurde, bevor das Abonnement deaktiviert wurde. </span><span class="sxs-lookup"><span data-stu-id="e3176-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="e3176-173">Abonnements können nicht vom Kunden verwendet werden und generieren keine Gebühren, wenn sie angehalten oder storniert werden.</span><span class="sxs-lookup"><span data-stu-id="e3176-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="e3176-174">Es gibt derzeit keine Möglichkeit, einen Kunden vollständig aus der **Kundenliste zu** entfernen.</span><span class="sxs-lookup"><span data-stu-id="e3176-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="e3176-175">Partner müssen Abonnements  für das Konto für den Übergang vom Partner-Mandanten in Partner Center dem Tag  aussetzen, an dem diese Abonnements in das Konto übergangen und unter dem Kontoübergang eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="e3176-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="e3176-176">Microsoft unterstützt keine Guthabenanforderungen aufgrund von Überschneidungen bei der Abrechnung,  die auftreten, wenn der Übergang von Abonnements auf "Angehalten" nicht ordnungsgemäß eingestellt wird.</span><span class="sxs-lookup"><span data-stu-id="e3176-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="e3176-177">Vereinfachen der Migration mithilfe der Exportfunktion</span><span class="sxs-lookup"><span data-stu-id="e3176-177">Simplify migration using Export</span></span>

<span data-ttu-id="e3176-178">Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:</span><span class="sxs-lookup"><span data-stu-id="e3176-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="e3176-179">Wählen **Sie kunden** auf Partner Center, um die Liste der Kunden zu sehen.</span><span class="sxs-lookup"><span data-stu-id="e3176-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="e3176-180">Öffnen Sie den Namen des gewünschten Kunden.</span><span class="sxs-lookup"><span data-stu-id="e3176-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="e3176-181">Wählen Sie **auf der** Seite Abonnements die Option **Abonnements exportieren** aus, um Details zu Abonnements in eine Excel-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="e3176-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="e3176-182">Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e3176-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="e3176-183">API-Registrierung</span><span class="sxs-lookup"><span data-stu-id="e3176-183">API registration</span></span>

<span data-ttu-id="e3176-184">Weitere Informationen zur API-Registrierung finden Sie unter [Einrichten des API-Zugriffs in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="e3176-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="e3176-185">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="e3176-185">Next steps</span></span>

- [<span data-ttu-id="e3176-186">Cloud Solution Provider Programm für regionale Märkte und Währungen, in denen Sie CSP-Angebote verkaufen können</span><span class="sxs-lookup"><span data-stu-id="e3176-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
