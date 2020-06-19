---
title: Mandantenkonsolidierung für regionale CSP-Autorisierung
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen. Dies schließt Schritte zum Migrieren von Kundenkonten und Kunden Abonnements ein.
author: LauraBrenner
ms.author: labrenne
keywords: Migrieren von Kunden, Bereitstellung, Mandantenkonto, Mandanten konsolidieren
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2e3c0bd9b50e91e02952a690cc7cbfe1601ad550
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991473"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="f4611-105">Anweisungen zur Mandantenkonsolidierung für regionale CSP-Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f4611-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="f4611-106">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="f4611-106">**Applies to**</span></span>

-  <span data-ttu-id="f4611-107">Partner Center</span><span class="sxs-lookup"><span data-stu-id="f4611-107">Partner Center</span></span>
-  <span data-ttu-id="f4611-108">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f4611-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f4611-109">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="f4611-109">**Appropriate roles**</span></span>

- <span data-ttu-id="f4611-110">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="f4611-110">Global admin</span></span>
- <span data-ttu-id="f4611-111">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="f4611-111">Admin agent</span></span>

<span data-ttu-id="f4611-112">\[Einige Informationen beziehen sich auf Vorabversionen, die vor der kommerziellen Freigabe grundlegend geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="f4611-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="f4611-113">Microsoft übernimmt keine Garantie, weder ausdrücklich noch stillschweigend, für die hier bereitgestellten Informationen.\]</span><span class="sxs-lookup"><span data-stu-id="f4611-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="f4611-114">Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.</span><span class="sxs-lookup"><span data-stu-id="f4611-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="f4611-115">Sie müssen alle Abonnements und Arbeitsplatz Zähler für Ihre Kunden kennen, die über die Übergangs Konten bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="f4611-115">You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="f4611-116">Sie werden im Rahmen des Migrationsprozesses unter dem neuen zentralen CSP-Konto genau dieselben Abonnements mit derselben Anzahl von Arbeitsplätzen erneut bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="f4611-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="f4611-117">Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f4611-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="f4611-118">Partner entscheiden sich für die Konsolidierung ihrer Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f4611-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="f4611-119">Nach Abschluss der Konsolidierung können Partner nicht den vorherigen Zustand wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="f4611-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="f4611-120">Möglicherweise ist auch eine Kunden Aktion erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4611-120">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="f4611-121">Vorbereiten der Migration</span><span class="sxs-lookup"><span data-stu-id="f4611-121">Prepare for migration</span></span>

- <span data-ttu-id="f4611-122">Melden Sie sich **mit dem Übergangs Konto (das** vorhandene Konto), das Sie übertragen werden, bei **Partner Center** an, und überprüfen Sie alle Kunden und alle Dienste, die für diese Kunden bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="f4611-122">Sign in to **Partner Center**  with the **Transitioning** (existing) account (the one you will transition) and review of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="Liste regionaler Kunden":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="f4611-124">Migrieren von Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="f4611-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="f4611-125">Melden Sie sich bei Ihrem **Partner Center** mit dem zu **migrierenden** (neuen) Konto an, und navigieren Sie von **Kunden** aus zur Liste „Kunden“.</span><span class="sxs-lookup"><span data-stu-id="f4611-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="f4611-126">Wählen Sie „Kunden“ aus.</span><span class="sxs-lookup"><span data-stu-id="f4611-126">Select Customers.</span></span>

3. <span data-ttu-id="f4611-127">Klicken Sie auf **Vertriebspartnerschaft beantragen**.</span><span class="sxs-lookup"><span data-stu-id="f4611-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="f4611-128">Ihnen wird eine Standard-E-Mail-Nachricht für die Weiterleitung an Ihre Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f4611-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="f4611-129">Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues Partner Center-Konto.</span><span class="sxs-lookup"><span data-stu-id="f4611-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="f4611-130">**Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen.</span><span class="sxs-lookup"><span data-stu-id="f4611-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="f4611-131">Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office 365-Portal aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="f4611-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="f4611-132">Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office 365 zugreift.</span><span class="sxs-lookup"><span data-stu-id="f4611-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="f4611-133">Nach der Anmeldung wird der globale Administrator für das Kundenkonto aufgefordert, eine Vereinbarung zu übermitteln, um dem neuen CSP-Konto delegierte Administratorrechte zu gewähren.</span><span class="sxs-lookup"><span data-stu-id="f4611-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="f4611-134">Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.</span><span class="sxs-lookup"><span data-stu-id="f4611-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="f4611-135">Die Kunden werden in der Kundenliste des Partners angezeigt, nachdem Sie die Vereinbarung nacheinander übermittelt haben.</span><span class="sxs-lookup"><span data-stu-id="f4611-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="f4611-136">Migrieren von nutzungsbasierten Office 365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)</span><span class="sxs-lookup"><span data-stu-id="f4611-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="f4611-137">Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.</span><span class="sxs-lookup"><span data-stu-id="f4611-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="f4611-138">Wählen Sie im **Partner Center** **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="f4611-138">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="f4611-139">Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="f4611-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="f4611-140">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="f4611-140">Select **Add subscription**.</span></span>

5. <span data-ttu-id="f4611-141">Fügen Sie die richtigen Abonnements und die korrekte Arbeitsplatzanzahl aus dem Katalog hinzu.</span><span class="sxs-lookup"><span data-stu-id="f4611-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="f4611-142">Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.</span><span class="sxs-lookup"><span data-stu-id="f4611-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Kundenliste":::

6. <span data-ttu-id="f4611-144">Klicken Sie auf **senden.**</span><span class="sxs-lookup"><span data-stu-id="f4611-144">Click **Submit.**</span></span>

   <span data-ttu-id="f4611-145">Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="f4611-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="f4611-146">Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="f4611-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="f4611-147">Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="f4611-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="f4611-148">Partner müssen Abonnements bei der **Umstellung vom** Partner Mandanten Konto in Partner Center an denselben Tag aussetzen, an dem diese Abonnements übertragen werden, und im Partner Center im Rahmen des **Übergangs zum** Partner Mandanten Konto eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="f4611-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="f4611-149">Supportanfragen in Bezug auf Kosten, die infolge sich überschneidender Abrechnungen auftreten, weil die Abonnements vom Typ **Transitioning From** nicht ordnungsgemäß deaktiviert wurden, werden abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="f4611-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="f4611-150">Deaktivieren der Office 365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“</span><span class="sxs-lookup"><span data-stu-id="f4611-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="f4611-151">Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr.</span><span class="sxs-lookup"><span data-stu-id="f4611-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="f4611-152">Azure-Abonnements müssen nicht manuell deaktiviert werden, da diese Abonnements während des Migrationsprozesses automatisch deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="f4611-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="f4611-153">Melden Sie sich im **Partner Center** mit dem CSP-Konto **Wechsel von** an, und navigieren Sie zur Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="f4611-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="f4611-154">Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.</span><span class="sxs-lookup"><span data-stu-id="f4611-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="f4611-155">Legen Sie für das Abonnement **suspended** fest, und klicken Sie anschließend auf **Übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="f4611-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="f4611-156">Durch das Anhalten des Abonnements wird sichergestellt, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="f4611-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="f4611-157">Für das Abonnement wird in der Abonnementliste **suspended** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f4611-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="f4611-158">Wiederholen Sie diese Schritte für alle Abonnements des Kunden.</span><span class="sxs-lookup"><span data-stu-id="f4611-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="f4611-159">Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f4611-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="f4611-160">Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.</span><span class="sxs-lookup"><span data-stu-id="f4611-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="f4611-161">Migrieren von nutzungsbasierten Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="f4611-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="f4611-162">Azure-Verwendungs basierte CSP-Abonnements müssen nicht manuell migriert werden, wie dies bei Office 365 CSP-Abonnements der Fall ist.</span><span class="sxs-lookup"><span data-stu-id="f4611-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="f4611-163">Der Microsoft Azure-Support kann die Azure-Abonnements sowie alle bereitgestellten Dienste oder Ressourcen von den CSP-Vertriebspartnerkonten vom Typ **Transitioning From** zum CSP-Vertriebspartnerkonto vom Typ **Transitioning To** migrieren.</span><span class="sxs-lookup"><span data-stu-id="f4611-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="f4611-164">Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.</span><span class="sxs-lookup"><span data-stu-id="f4611-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="f4611-165">Stellen Sie sicher, dass für die Kundenkonten, deren Azure-Abonnements migriert werden müssen, die Vereinbarung für das neue CSP-Konto vom Typ **Transitioning To** akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="f4611-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="f4611-166">Partner Benachrichtigen Microsoft, welche Kundenkonten, die über Azure-Abonnements verfügen, für die Migration bereit sind, und stellen diese Firmennamen für Kunden bereit.</span><span class="sxs-lookup"><span data-stu-id="f4611-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="f4611-167">Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt den Partner, wenn die Migration abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="f4611-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="f4611-168">Der Partner überprüft, ob für das Azure-Abonnement unter den CSP-Vertriebspartnerkonten vom Typ **Transitioning From** in Partner Center im Abschnitt mit den Kundenabonnements jetzt „suspended“ angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f4611-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="f4611-169">Der Partner überprüft, ob für das Azure-Abonnement unter dem CSP-Vertriebspartnerkonto vom Typ **Transitioning To** nun in Partner Center im Abschnitt mit den Kundenabonnements der Status **active** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f4611-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="f4611-170">Durch das Deaktivieren der Abonnements unter dem Kunden wird die Darstellung des Kunden in der Kundenliste nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="f4611-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="f4611-171">Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="f4611-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="f4611-172">Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.</span><span class="sxs-lookup"><span data-stu-id="f4611-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="f4611-173">Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="f4611-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="f4611-174">Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="f4611-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="f4611-175">Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.</span><span class="sxs-lookup"><span data-stu-id="f4611-175">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="f4611-176">Zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="f4611-176">Additional information</span></span>

- <span data-ttu-id="f4611-177">Das Deaktivieren des Abonnements von der **Umstellung vom** CSP-Konto wirkt sich nicht auf den Dienst des Endkunden aus, solange der Dienst vor dem Deaktivieren des Abonnements vom **Übergang zum** CSP-Konto bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f4611-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="f4611-178">Abonnements können nicht vom Kunden verwendet werden, und es werden keine Gebühren generiert, wenn Sie angehalten oder abgebrochen werden.</span><span class="sxs-lookup"><span data-stu-id="f4611-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="f4611-179">Zurzeit besteht keine Möglichkeit, einen Kunden vollständig aus der Kundenliste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="f4611-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

    >[!Note]
    > <span data-ttu-id="f4611-180">Partner müssen Abonnements bei der **Umstellung vom** Partner Mandanten Konto in Partner Center an denselben Tag aussetzen, an dem diese Abonnements umgestellt werden, und unter dem Konto des **Übergangs zum** Partner Mandanten im Partner Center eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="f4611-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="f4611-181">Microsoft unterstützt keine Kreditanforderungen aufgrund einer Überlappung bei der Abrechnung, wenn die **Umstellung von** Abonnements auf angehalten nicht ordnungsgemäß festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="f4611-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="f4611-182">Vereinfachen der Migration mithilfe der Exportfunktion</span><span class="sxs-lookup"><span data-stu-id="f4611-182">Simplify migration using Export</span></span>

<span data-ttu-id="f4611-183">Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:</span><span class="sxs-lookup"><span data-stu-id="f4611-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="f4611-184">Klicken Sie im Partner Center auf **Kunden**, um die Liste der Kunden in der vorhandenen Struktur anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f4611-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="f4611-185">Öffnen Sie den Namen des gewünschten Kunden.</span><span class="sxs-lookup"><span data-stu-id="f4611-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="f4611-186">Klicken Sie auf der Seite **Abonnements** auf **Export Subscriptions**, um Details zu Abonnements in eine Excel-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="f4611-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="f4611-187">Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f4611-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="f4611-188">API-Registrierung</span><span class="sxs-lookup"><span data-stu-id="f4611-188">API registration</span></span>

<span data-ttu-id="f4611-189">Weitere Informationen zur API-Registrierung finden [Sie unter Einrichten des API-Zugriffs in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="f4611-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
