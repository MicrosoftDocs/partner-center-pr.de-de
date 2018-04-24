---
title: Mandantenkonsolidierung für regionale CSP-Autorisierung | Partner Center
description: Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
keywords: Migrieren von Kunden, Bereitstellung, Mandantenkonto, Mandanten konsolidieren
ms.openlocfilehash: 4a8d1e993c11d379819ef9628db1f2399c6e6b49
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2018
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="00812-104">Mandantenkonsolidierung für regionale CSP-Autorisierung</span><span class="sxs-lookup"><span data-stu-id="00812-104">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="00812-105">Betrifft:</span><span class="sxs-lookup"><span data-stu-id="00812-105">Applies to</span></span>**

-  <span data-ttu-id="00812-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="00812-106">Partner Center</span></span>
-  <span data-ttu-id="00812-107">Partner Center für Microsoft Cloud für US-Behörden</span><span class="sxs-lookup"><span data-stu-id="00812-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="00812-108">Partner Center für Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="00812-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="00812-109">\[Einige Informationen beziehen sich auf die Vorabversion, die vor der kommerziellen Freigabe möglicherweise wesentlichen Änderungen unterliegt.</span><span class="sxs-lookup"><span data-stu-id="00812-109">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="00812-110">Microsoft übernimmt für die hier bereitgestellten Informationen keine Garantie, weder ausdrücklicher noch impliziter Art.\]</span><span class="sxs-lookup"><span data-stu-id="00812-110">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="00812-111">Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.</span><span class="sxs-lookup"><span data-stu-id="00812-111">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="00812-112">**Hinweis:** Sie müssen alle Abonnements und die Anzahl von Arbeitsplätzen für Ihre Kunden kennen, die über die Übergangskonten bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="00812-112">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="00812-113">Sie werden im Rahmen des Migrationsprozesses unter dem neuen zentralen CSP-Konto genau dieselben Abonnements mit derselben Anzahl von Arbeitsplätzen erneut bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="00812-113">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="00812-114">Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="00812-114">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="00812-115">Partner entscheiden sich für die Konsolidierung ihrer Mandanten.</span><span class="sxs-lookup"><span data-stu-id="00812-115">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="00812-116">Nach Abschluss der Konsolidierung können Partner nicht den vorherigen Zustand wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="00812-116">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="00812-117">Beachten Sie, dass auch Schritte vonseiten des Kunden erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="00812-117">Note that customer action may also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="00812-118">Vorbereitung auf die Migration</span><span class="sxs-lookup"><span data-stu-id="00812-118">Prepare for migration</span></span>


-   <span data-ttu-id="00812-119">Melden Sie sich im **Dashboard** mit dem zu **migrierenden** (vorhandenen) Konto an, und notieren Sie alle Kunden und alle für diese Kunden bereitgestellten Dienste.</span><span class="sxs-lookup"><span data-stu-id="00812-119">Sign in to your **Dashboard**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![Liste regionaler Kunden](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="00812-121">Migrieren von Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="00812-121">Migrate customer accounts</span></span>


1.  <span data-ttu-id="00812-122">Melden Sie sich beim **Dashboard** mit dem zu **migrierenden** (neuen) Konto an und navigieren Sie von **Kunden** aus zur Liste der Kunden.</span><span class="sxs-lookup"><span data-stu-id="00812-122">Sign in to your **Dashboard**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="00812-123">Wählen Sie die gewünschten Kunden.</span><span class="sxs-lookup"><span data-stu-id="00812-123">Select Customers.</span></span>

3.  <span data-ttu-id="00812-124">Klicken Sie auf **Vertriebspartnerschaft beantragen**.</span><span class="sxs-lookup"><span data-stu-id="00812-124">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="00812-125">Ihnen wird eine Standard-E-Mail-Nachricht für die Weiterleitung an Ihre Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="00812-125">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="00812-126">Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues PartnerCenter-Konto.</span><span class="sxs-lookup"><span data-stu-id="00812-126">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="00812-127">**Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen.</span><span class="sxs-lookup"><span data-stu-id="00812-127">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="00812-128">Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office365-Portal aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="00812-128">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="00812-129">Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office365 zugreift.</span><span class="sxs-lookup"><span data-stu-id="00812-129">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="00812-130">Nach der Anmeldung wird der globale Administrator für das Kundenkonto aufgefordert, eine Vereinbarung zu übermitteln, um dem neuen CSP-Konto delegierte Administratorrechte zu gewähren.</span><span class="sxs-lookup"><span data-stu-id="00812-130">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="00812-131">Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.</span><span class="sxs-lookup"><span data-stu-id="00812-131">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="00812-132">Die Kunden werden nach Übermittlung der Vereinbarung nacheinander in der Kundenliste des Partners angezeigt.</span><span class="sxs-lookup"><span data-stu-id="00812-132">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="00812-133">Migrieren von nutzungsbasierten Office365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)</span><span class="sxs-lookup"><span data-stu-id="00812-133">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="00812-134">Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.</span><span class="sxs-lookup"><span data-stu-id="00812-134">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="00812-135">Wählen Sie im **Dashboard** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="00812-135">From the **Dashboard** select **Customers**.</span></span>

3.  <span data-ttu-id="00812-136">Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="00812-136">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="00812-137">Klicken Sie auf **Abonnement hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="00812-137">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="00812-138">Fügen Sie die richtigen Abonnements und die korrekte Arbeitsplatzanzahl aus dem Katalog hinzu.</span><span class="sxs-lookup"><span data-stu-id="00812-138">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="00812-139">Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.</span><span class="sxs-lookup"><span data-stu-id="00812-139">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![Screenshot der Kundenliste](images/regionalcustomer2.png)

6.  <span data-ttu-id="00812-141">Klicken Sie auf **Übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="00812-141">Click **Submit.**</span></span>

<span data-ttu-id="00812-142">Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="00812-142">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="00812-143">Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="00812-143">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="00812-144">Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="00812-144">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="00812-145">**Hinweis:** Partner müssen Abonnements im Partnermandantenkonto vom Typ **Transitioning From** in Partner Center am selben Tag aussetzen, an dem diese Abonnements migriert und unter dem Partnermandantenkonto vom Typ **Transitioning To** in Partner Center eingerichtet werden, um eine doppelte Abrechnung von Kosten zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="00812-145">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="00812-146">Supportanfragen in Bezug auf Kosten, die infolge sich überschneidender Abrechnungen auftreten, weil die Abonnements vom Typ **Transitioning From** nicht ordnungsgemäß deaktiviert wurden, werden abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="00812-146">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="00812-147">Deaktivieren der Office365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“</span><span class="sxs-lookup"><span data-stu-id="00812-147">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="00812-148">Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr.</span><span class="sxs-lookup"><span data-stu-id="00812-148">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="00812-149">Azure-Abonnements müssen nicht manuell deaktiviert werden, da diese Abonnements während des Migrationsprozesses automatisch deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="00812-149">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="00812-150">Melden Sie sich im **Dashboard** mit dem **Transitioning From** CSP-Konto an, und navigieren Sie zur Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="00812-150">Sign in to the **Dashboard** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="00812-151">Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.</span><span class="sxs-lookup"><span data-stu-id="00812-151">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="00812-152">Legen Sie für das Abonnement **suspended** fest, und klicken Sie anschließend auf **Übermitteln**.</span><span class="sxs-lookup"><span data-stu-id="00812-152">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="00812-153">**Hinweis:** Durch Aussetzen des Abonnements wird sichergestellt, dass die Abrechnung nicht doppelt erfolgt.</span><span class="sxs-lookup"><span data-stu-id="00812-153">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="00812-154">Für das Abonnement wird in der Abonnementliste **suspended** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="00812-154">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="00812-155">Wiederholen Sie diese Schritte für alle Abonnements des Kunden.</span><span class="sxs-lookup"><span data-stu-id="00812-155">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="00812-156">Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="00812-156">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="00812-157">Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.</span><span class="sxs-lookup"><span data-stu-id="00812-157">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="00812-158">Migrieren von nutzungsbasierten Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="00812-158">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="00812-159">Beachten Sie, dass nutzungsbasierte Azure-CSP-Abonnements nicht wie Office365-CSP-Abonnements manuell migriert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="00812-159">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="00812-160">Der Microsoft Azure-Support kann die Azure-Abonnements sowie alle bereitgestellten Dienste oder Ressourcen von den CSP-Vertriebspartnerkonten vom Typ **Transitioning From** zum CSP-Vertriebspartnerkonto vom Typ **Transitioning To** migrieren.</span><span class="sxs-lookup"><span data-stu-id="00812-160">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="00812-161">Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.</span><span class="sxs-lookup"><span data-stu-id="00812-161">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="00812-162">Stellen Sie sicher, dass für die Kundenkonten, deren Azure-Abonnements migriert werden müssen, die Vereinbarung für das neue CSP-Konto vom Typ **Transitioning To** akzeptiert wurde.</span><span class="sxs-lookup"><span data-stu-id="00812-162">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="00812-163">Partner informieren Microsoft darüber, welche Kundenkonten mit Azure-Abonnements migriert werden können, und stellen die Firmennamen dieser Kunden bereit.</span><span class="sxs-lookup"><span data-stu-id="00812-163">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="00812-164">Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt den Partner, wenn die Migration abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="00812-164">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="00812-165">Der Partner überprüft, ob für das Azure-Abonnement unter den CSP-Vertriebspartnerkonten vom Typ **Transitioning From** in Partner Center im Abschnitt mit den Kundenabonnements jetzt „suspended“ angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="00812-165">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="00812-166">Der Partner überprüft, ob für das Azure-Abonnement unter dem CSP-Vertriebspartnerkonto vom Typ **Transitioning To** nun in Partner Center im Abschnitt mit den Kundenabonnements der Status **active** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="00812-166">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="00812-167">**Hinweis:** Durch die Deaktivierung der Abonnements im Kundeneintrag wird nicht die Darstellung des Kunden in der Kundenliste geändert.</span><span class="sxs-lookup"><span data-stu-id="00812-167">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="00812-168">Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="00812-168">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="00812-169">Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.</span><span class="sxs-lookup"><span data-stu-id="00812-169">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="00812-170">Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="00812-170">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="00812-171">Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="00812-171">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="00812-172">Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.</span><span class="sxs-lookup"><span data-stu-id="00812-172">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="00812-173">Hinweise</span><span class="sxs-lookup"><span data-stu-id="00812-173">Notes</span></span>

-   <span data-ttu-id="00812-174">Die Deaktivierung des Abonnements im CSP-Konto vom Typ **Transitioning From** wirkt sich nicht auf den Dienst des Endkunden aus, sofern der Dienst vor der Deaktivierung über das CSP-Konto vom Typ **Transitioning To** bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="00812-174">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="00812-175">Abonnements können vom Kunden nicht verwendet werden und generieren keine Gebühren, wenn sie ausgesetzt oder gekündigt wurden.</span><span class="sxs-lookup"><span data-stu-id="00812-175">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="00812-176">Zurzeit besteht keine Möglichkeit, einen Kunden vollständig aus der Kundenliste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="00812-176">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="00812-177">**Hinweis:** Partner müssen Abonnements im Partnermandantenkonto vom Typ **Transitioning From** in Partner Center am selben Tag aussetzen, an dem diese Abonnements migriert und unter dem Partnermandantenkonto vom Typ **Transitioning To** in Partner Center eingerichtet werden, um eine doppelte Abrechnung von Kosten zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="00812-177">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="00812-178">Microsoft lehnt Supportanfragen in Bezug auf Kosten ab, die infolge sich überschneidender Abrechnungen auftreten, weil Abonnements vom Typ **Transitioning From** nicht ordnungsgemäß auf „suspended“ gesetzt wurden.</span><span class="sxs-lookup"><span data-stu-id="00812-178">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="00812-179">Vereinfachen der Migration mithilfe der Exportfunktion</span><span class="sxs-lookup"><span data-stu-id="00812-179">Simplify migration using Export</span></span>

<span data-ttu-id="00812-180">Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:</span><span class="sxs-lookup"><span data-stu-id="00812-180">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="00812-181">Klicken Sie auf dem Dashboard auf **Kunden**, um die Liste der Kunden in der vorhandenen Struktur anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="00812-181">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="00812-182">Öffnen Sie den Namen des gewünschten Kunden.</span><span class="sxs-lookup"><span data-stu-id="00812-182">Open the desired customer name.</span></span>

3.  <span data-ttu-id="00812-183">Klicken Sie auf der Seite **Abonnements** auf **Export Subscriptions**, um Details zu Abonnements in eine Excel-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="00812-183">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="00812-184">Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="00812-184">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="00812-185">API-Registrierung</span><span class="sxs-lookup"><span data-stu-id="00812-185">API registration</span></span>

<span data-ttu-id="00812-186">Weitere Informationen zur API-Registrierung finden Sie in [auf dieser Seite](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="00812-186">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>


 

 



