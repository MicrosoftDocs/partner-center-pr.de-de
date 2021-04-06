---
title: Mandantenkonsolidierung für regionale CSP-Autorisierung
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen. Dies schließt Schritte zum Migrieren von Kundenkonten und Kunden Abonnements ein.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502569"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="acff3-104">Anweisungen zur Mandantenkonsolidierung für regionale CSP-Autorisierung</span><span class="sxs-lookup"><span data-stu-id="acff3-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="acff3-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="acff3-105">**Applies to**</span></span>

- <span data-ttu-id="acff3-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="acff3-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="acff3-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="acff3-107">**Appropriate roles**</span></span>

- <span data-ttu-id="acff3-108">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="acff3-108">Global admin</span></span>
- <span data-ttu-id="acff3-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="acff3-109">Admin agent</span></span>

<span data-ttu-id="acff3-110">\[Einige Informationen beziehen sich auf Vorabversionen, die vor der kommerziellen Freigabe grundlegend geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="acff3-110">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="acff3-111">Microsoft übernimmt keine Garantie, weder ausdrücklich noch stillschweigend, für die hier bereitgestellten Informationen.\]</span><span class="sxs-lookup"><span data-stu-id="acff3-111">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="acff3-112">Mandanten können für Ihr Unternehmen konsolidiert werden.</span><span class="sxs-lookup"><span data-stu-id="acff3-112">You can consolidate tenants for your business.</span></span> <span data-ttu-id="acff3-113">Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.</span><span class="sxs-lookup"><span data-stu-id="acff3-113">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="acff3-114">Sie müssen alle bereitgestellten Abonnements und Lizenz Anzahlen für die einzelnen Kunden in dem Konto beachten, von dem aus Sie wechseln.</span><span class="sxs-lookup"><span data-stu-id="acff3-114">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="acff3-115">Sie werden im Rahmen des Migrationsprozesses dieselben exakten Abonnements mit der gleichen Anzahl von Lizenzen unter dem neuen zentralen CSP-Konto bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="acff3-115">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="acff3-116">Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="acff3-116">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="acff3-117">Wenn die Konsolidierung fertiggestellt ist, können Sie nicht mehr auf den vorherigen Mandanten Status zurückgreifen.</span><span class="sxs-lookup"><span data-stu-id="acff3-117">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="acff3-118">Möglicherweise ist auch eine Kunden Aktion erforderlich.</span><span class="sxs-lookup"><span data-stu-id="acff3-118">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="acff3-119">Vorbereiten der Migration</span><span class="sxs-lookup"><span data-stu-id="acff3-119">Prepare for migration</span></span>

- <span data-ttu-id="acff3-120">Melden Sie sich mit dem **transitionskonto** , das Sie zum neuen Konto wechseln, bei **Partner Center** an, und überprüfen Sie alle Kunden und alle Dienste, die für diese Kunden bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="acff3-120">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="acff3-121">Melden Sie sich von diesem Konto ab.</span><span class="sxs-lookup"><span data-stu-id="acff3-121">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="acff3-122">Migrieren von Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="acff3-122">Migrate customer accounts</span></span>

1. <span data-ttu-id="acff3-123">Melden Sie sich bei **Partner Center**  mit dem **transitionskonto** (neu) an (das Konto, in das Sie die Kunden wechseln).</span><span class="sxs-lookup"><span data-stu-id="acff3-123">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="acff3-124">Wählen Sie **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="acff3-124">Select **Customers**.</span></span>

3. <span data-ttu-id="acff3-125">Wählen Sie **Reseller Relationship anfordern** aus.</span><span class="sxs-lookup"><span data-stu-id="acff3-125">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="acff3-126">Ihnen wird eine Standard-e-Mail-Nachricht angezeigt, die an Ihre Kunden gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="acff3-126">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="acff3-127">Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues Partner Center-Konto.</span><span class="sxs-lookup"><span data-stu-id="acff3-127">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="acff3-128">**Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen.</span><span class="sxs-lookup"><span data-stu-id="acff3-128">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="acff3-129">Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office 365-Portal aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="acff3-129">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="acff3-130">Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office 365 zugreift.</span><span class="sxs-lookup"><span data-stu-id="acff3-130">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="acff3-131">Nach der Anmeldung wird der globale Administrator für das **Kundenkonto** aufgefordert, eine Vereinbarung zu übermitteln, die dem neuen CSP-Konto Delegierte Administratorrechte erteilt.</span><span class="sxs-lookup"><span data-stu-id="acff3-131">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="acff3-132">Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.</span><span class="sxs-lookup"><span data-stu-id="acff3-132">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="acff3-133">Die Kunden werden in der Kundenliste des Partners angezeigt, nachdem Sie die Vereinbarung nacheinander übermittelt haben.</span><span class="sxs-lookup"><span data-stu-id="acff3-133">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="acff3-134">Migrieren von nutzungsbasierten Office 365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)</span><span class="sxs-lookup"><span data-stu-id="acff3-134">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="acff3-135">Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.</span><span class="sxs-lookup"><span data-stu-id="acff3-135">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="acff3-136">Wählen Sie im **Partner Center** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="acff3-136">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="acff3-137">Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.</span><span class="sxs-lookup"><span data-stu-id="acff3-137">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="acff3-138">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="acff3-138">Select **Add subscription**.</span></span>

5. <span data-ttu-id="acff3-139">Fügen Sie die richtigen Abonnements und Lizenz Anzahl aus dem Katalog hinzu.</span><span class="sxs-lookup"><span data-stu-id="acff3-139">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="acff3-140">Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.</span><span class="sxs-lookup"><span data-stu-id="acff3-140">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Kundenliste":::

6. <span data-ttu-id="acff3-142">Wählen Sie **senden aus.**</span><span class="sxs-lookup"><span data-stu-id="acff3-142">Select **Submit.**</span></span>

   <span data-ttu-id="acff3-143">Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="acff3-143">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="acff3-144">Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="acff3-144">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="acff3-145">Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="acff3-145">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="acff3-146">Partner müssen Abonnements bei der **Umstellung vom** Partner Mandanten Konto in Partner Center an denselben Tag aussetzen, an dem diese Abonnements übertragen werden, und im Partner Center im Rahmen des **Übergangs zum** Partner Mandanten Konto eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="acff3-146">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="acff3-147">Support Anfragen werden aufgrund von Überlappungen bei der Abrechnung verweigert, wenn der **Übergang von** Abonnements nicht ordnungsgemäß deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="acff3-147">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="acff3-148">Deaktivieren der Office 365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“</span><span class="sxs-lookup"><span data-stu-id="acff3-148">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="acff3-149">Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr.</span><span class="sxs-lookup"><span data-stu-id="acff3-149">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="acff3-150">Azure-Abonnements müssen nicht manuell deaktiviert werden, da Azure-Abonnements während des Migrations Vorgangs automatisch deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="acff3-150">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="acff3-151">Melden Sie sich im **Partner Center** mit dem CSP-Konto **Wechsel von** an, und navigieren Sie zur Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="acff3-151">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="acff3-152">Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.</span><span class="sxs-lookup"><span data-stu-id="acff3-152">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="acff3-153">Legen **Sie das Abonnement auf angeh** alten fest, und wählen Sie dann **senden** aus.</span><span class="sxs-lookup"><span data-stu-id="acff3-153">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="acff3-154">Durch das Anhalten des Abonnements wird sichergestellt, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="acff3-154">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="acff3-155">Das Abonnement **wird** in der Liste Abonnements angezeigt.</span><span class="sxs-lookup"><span data-stu-id="acff3-155">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="acff3-156">Wiederholen Sie diese Schritte für alle Abonnements des Kunden.</span><span class="sxs-lookup"><span data-stu-id="acff3-156">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="acff3-157">Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="acff3-157">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="acff3-158">Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.</span><span class="sxs-lookup"><span data-stu-id="acff3-158">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="acff3-159">Migrieren von nutzungsbasierten Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="acff3-159">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="acff3-160">Im Gegensatz zu den Office 365 CSP-Abonnements müssen Azure und Verwendungs basierte CSP-Abonnements nicht manuell migriert werden.</span><span class="sxs-lookup"><span data-stu-id="acff3-160">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="acff3-161">Microsoft Azure-Unterstützung migriert die Azure-Abonnements und alle bereitgestellten Dienste oder Ressourcen von der **Umstellung von** CSP-Reseller-Konten zum **Übergang in** das CSP-Reseller-Konto.</span><span class="sxs-lookup"><span data-stu-id="acff3-161">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="acff3-162">Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.</span><span class="sxs-lookup"><span data-stu-id="acff3-162">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="acff3-163">Stellen Sie sicher, dass das Kundenkonto, für das Azure-Abonnements migriert werden sollen, die Vereinbarung zum neuen **Übergang zum** CSP-Konto zugeordnet haben.</span><span class="sxs-lookup"><span data-stu-id="acff3-163">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="acff3-164">Sie benachrichtigen Microsoft, welche Kundenkonten für die Migration bereit sind, und geben die Firmennamen dieser Kunden an.</span><span class="sxs-lookup"><span data-stu-id="acff3-164">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="acff3-165">Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt Sie, wenn die Migration beendet ist.</span><span class="sxs-lookup"><span data-stu-id="acff3-165">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="acff3-166">Sie müssen sicherstellen, dass das Azure-Abonnement im Rahmen des **Übergangs von** CSP-Reseller-Konto jetzt im Partner Center im Abschnitt Kunden Abonnements als angeh **alten gekennzeichnet ist** .</span><span class="sxs-lookup"><span data-stu-id="acff3-166">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="acff3-167">Vergewissern Sie sich, dass das Azure-Abonnement unter der **Umstellung auf** das CSP-Reseller-Konto jetzt den Status **aktiv** im Partner Center im Abschnitt Kunden Abonnements anzeigt.</span><span class="sxs-lookup"><span data-stu-id="acff3-167">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="acff3-168">Durch das Deaktivieren der Abonnements unter dem Kunden wird die Darstellung des Kunden in der Kundenliste nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="acff3-168">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="acff3-169">Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="acff3-169">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="acff3-170">Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.</span><span class="sxs-lookup"><span data-stu-id="acff3-170">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="acff3-171">Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="acff3-171">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="acff3-172">Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="acff3-172">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="acff3-173">Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.</span><span class="sxs-lookup"><span data-stu-id="acff3-173">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="acff3-174">Zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="acff3-174">Additional information</span></span>

- <span data-ttu-id="acff3-175">Das Deaktivieren des Abonnements von der **Umstellung vom** CSP-Konto wirkt sich nicht auf den Dienst des Endkunden aus, solange der Dienst vor dem Deaktivieren des Abonnements vom **Übergang zum** CSP-Konto bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="acff3-175">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="acff3-176">Abonnements können nicht vom Kunden verwendet werden, und es werden keine Gebühren generiert, wenn Sie angehalten oder abgebrochen werden.</span><span class="sxs-lookup"><span data-stu-id="acff3-176">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="acff3-177">Es gibt derzeit keine Möglichkeit, einen Kunden vollständig aus der **Kunden** Liste zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="acff3-177">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="acff3-178">Partner müssen Abonnements bei der **Umstellung vom** Partner Mandanten Konto in Partner Center an denselben Tag, an dem diese Abonnements umgestellt werden, und bei der Umstellung **auf** das Konto sperren, um sicherzustellen, dass keine doppelte Abrechnung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="acff3-178">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="acff3-179">Microsoft unterstützt keine Kreditanforderungen aufgrund einer Überlappung bei der Abrechnung, wenn die **Umstellung von** Abonnements auf angehalten nicht ordnungsgemäß festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="acff3-179">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="acff3-180">Vereinfachen der Migration mithilfe der Exportfunktion</span><span class="sxs-lookup"><span data-stu-id="acff3-180">Simplify migration using Export</span></span>

<span data-ttu-id="acff3-181">Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:</span><span class="sxs-lookup"><span data-stu-id="acff3-181">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="acff3-182">Wählen Sie **Kunden** im Partner Center aus, um die Kundenliste anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="acff3-182">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="acff3-183">Öffnen Sie den Namen des gewünschten Kunden.</span><span class="sxs-lookup"><span data-stu-id="acff3-183">Open the desired customer name.</span></span>

3. <span data-ttu-id="acff3-184">Wählen Sie auf der Seite **Abonnements** die Option **Abonnements exportieren** aus, um die Details von Abonnements in eine Excel-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="acff3-184">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="acff3-185">Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="acff3-185">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="acff3-186">API-Registrierung</span><span class="sxs-lookup"><span data-stu-id="acff3-186">API registration</span></span>

<span data-ttu-id="acff3-187">Weitere Informationen zur API-Registrierung finden [Sie unter Einrichten des API-Zugriffs in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="acff3-187">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="acff3-188">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="acff3-188">Next steps</span></span>

- [<span data-ttu-id="acff3-189">Cloud Solution Provider Program (regionale Märkte und Währungen), in denen Sie CSP-Angebote verkaufen können</span><span class="sxs-lookup"><span data-stu-id="acff3-189">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
