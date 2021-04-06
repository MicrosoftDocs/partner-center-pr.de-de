---
title: Erstellen von Kunden Abonnements im Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Abonnements an Ihre Kunden für von Microsoft veröffentlichte Produkte sowie SaaS-Produkte verkaufen, die von Drittanbieter-ISVs veröffentlicht werden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502934"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="76ab6-103">Erstellen, Aussetzen oder Stornieren von Kundenabonnements</span><span class="sxs-lookup"><span data-stu-id="76ab6-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="76ab6-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="76ab6-104">**Applies to**</span></span>

- <span data-ttu-id="76ab6-105">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="76ab6-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="76ab6-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="76ab6-106">**Appropriate roles**</span></span>

- <span data-ttu-id="76ab6-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="76ab6-107">Admin agent</span></span>
- <span data-ttu-id="76ab6-108">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="76ab6-108">Billing admin</span></span>
- <span data-ttu-id="76ab6-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="76ab6-109">Global admin</span></span>
- <span data-ttu-id="76ab6-110">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="76ab6-110">Helpdesk agent</span></span>
- <span data-ttu-id="76ab6-111">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="76ab6-111">Sales agent</span></span>

<span data-ttu-id="76ab6-112">Nachdem Sie für Ihre Kunden einen Datensatz im Partner Center erstellt haben, können Sie ihnen Abonnements für Produkte im Katalog verkaufen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="76ab6-113">Dies schließt Produkte ein, die von Microsoft und Saas-Produkten (Software-as-a-Service) veröffentlicht wurden, die von unabhängigen Softwareanbietern (ISVs) von Drittanbietern im [kommerziellen Marketplace](https://azuremarketplace.microsoft.com/marketplace)veröffentlicht wurden.</span><span class="sxs-lookup"><span data-stu-id="76ab6-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="76ab6-114">Einige Angebote sind auf ein Abonnement pro Kunde beschränkt.</span><span class="sxs-lookup"><span data-stu-id="76ab6-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="76ab6-115">Eine Liste der eingeschränkten Angebote finden Sie im Partner Center auf der Seite für Preise und Angebote.</span><span class="sxs-lookup"><span data-stu-id="76ab6-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="76ab6-116">Als Partner im CSP-Programm können Sie **Lizenz basierte** oder getaktete Saas  -Abonnements von ISV-Verlegern innerhalb von Partner Center erwerben.</span><span class="sxs-lookup"><span data-stu-id="76ab6-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="76ab6-117">Dies bedeutet, dass Sie ein **Lizenz basiertes** **oder** getaktetes SaaS-Angebot erwerben können, das der ISV-Verleger zur Verfügung gestellt hat, einschließlich [exklusiver Angebote](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , auf die Sie Zugriff haben.</span><span class="sxs-lookup"><span data-stu-id="76ab6-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="76ab6-118">Zum Erwerb oder zur Verwaltung anderer kommerzieller Marketplace-Angebote von ISVs (z. b. nutzungsbasierte Angebote mit Azure-Anwendungen, Containern oder VMS) müssen Sie zum [Azure-Portal](https://portal.azure.com/)wechseln.</span><span class="sxs-lookup"><span data-stu-id="76ab6-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="76ab6-119">Erstellen eines neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="76ab6-119">Create a new subscription</span></span>

1. <span data-ttu-id="76ab6-120">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="76ab6-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="76ab6-121">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="76ab6-122">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-122">Select **Add subscription**.</span></span> <span data-ttu-id="76ab6-123">Auf der Registerkarte **Online Dienste** werden alle verfügbaren Marketplace-SaaS-Angebote angezeigt.</span><span class="sxs-lookup"><span data-stu-id="76ab6-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="76ab6-124">Um nur bestimmte Arten von Abonnements anzuzeigen, treffen Sie eine Auswahl bei den verfügbaren Filter:</span><span class="sxs-lookup"><span data-stu-id="76ab6-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="76ab6-125">**Herausgeber**: Wählen Sie **Microsoft** aus, um nur Angebote von Microsoft oder **Partnern** anzuzeigen, um kommerzielle Marketplace-Produkte anzuzeigen, die von ISVs veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="76ab6-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="76ab6-126">**Abrechnungstyp**: Wählen Sie den Typ der Abonnement Abrechnung aus, den Sie verwenden möchten: **Lizenz** oder **Nutzung**.</span><span class="sxs-lookup"><span data-stu-id="76ab6-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="76ab6-127">Informationen, die Ihnen bei der Entscheidung zwischen monatlicher und jährlicher Abrechnungs Häufigkeit helfen, finden Sie unter [Lizenz basierte Abrechnung](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="76ab6-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="76ab6-128">**Kategorie**: Wählen Sie **Enterprise**, **Small Business** oder **Testversion** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="76ab6-129">Informationen zu Testabonnements finden Sie unter [Testversionen von Microsoft-Produkten anbieten](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="76ab6-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="76ab6-130">Wählen Sie die Produkt Abonnements aus, die Sie für Ihren Kunden erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="76ab6-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="76ab6-131">Welche Produkte Sie sehen, hängt vom Typ des Kunden Segments (Education, Government usw.) und den von Ihnen angewendeten Filtern ab.</span><span class="sxs-lookup"><span data-stu-id="76ab6-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="76ab6-132">Einige Angebote, die auf dem Marketplace angezeigt werden, sind möglicherweise nicht immer für einen bestimmten Kunden oder einen bestimmten CSP-Partner verfügbar.</span><span class="sxs-lookup"><span data-stu-id="76ab6-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="76ab6-133">Dies kann folgende Ursache haben:</span><span class="sxs-lookup"><span data-stu-id="76ab6-133">This can be because:</span></span>

   - <span data-ttu-id="76ab6-134">Der Kunde hat bereits ein Abonnement für dieses Produkt und ist nur eins zulässig.</span><span class="sxs-lookup"><span data-stu-id="76ab6-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="76ab6-135">Das Abonnement des Kunden wurde möglicherweise angehalten (in diesem Fall können Sie das Abonnement reaktivieren, anstatt ein neues zu erwerben).</span><span class="sxs-lookup"><span data-stu-id="76ab6-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="76ab6-136">Für ISV-SaaS-Angebote gibt es möglicherweise einige Gründe, warum das Angebot nicht erworben werden kann: der ISV unterstützt das Abrechnungs Land oder die Region des Kunden möglicherweise nicht. der ISV hat möglicherweise entschieden, das Angebot nicht über das CSP-Programm verfügbar zu machen. oder der ISV hat das Angebot möglicherweise nur für bestimmte CSP-Partner [exklusiv](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gestaltet.</span><span class="sxs-lookup"><span data-stu-id="76ab6-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="76ab6-137">Das ISV-Angebot kann auch nicht über das Partner Center (z. b. Container oder einige Verwendungs basierte Angebote) übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="76ab6-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="76ab6-138">Geben Sie für jedes Abonnement, das Sie hinzufügen möchten, die Anzahl der Lizenzen (falls erforderlich) ein, und wählen Sie **zum Warenkorb hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="76ab6-139">Nachdem Sie Abonnements hinzugefügt haben, wählen Sie **überprüfen** aus, und überprüfen Sie Ihre Bestellung.</span><span class="sxs-lookup"><span data-stu-id="76ab6-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="76ab6-140">Nachdem Sie Ihre Bestellungen überprüft haben und bereit sind, diese Abonnements zu erwerben, wählen Sie **kaufen** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="76ab6-141">Wenn Sie ein Abonnement für einen Kunden erworben haben, tritt Folgendes auf:</span><span class="sxs-lookup"><span data-stu-id="76ab6-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="76ab6-142">Sie können das Abonnement überprüfen oder bearbeiten, indem Sie den Abonnement Namen **auf der Abonnementseite des** Kunden auswählen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="76ab6-143">Dort können Sie Add-On-Lizenzen auswählen, falls verfügbar, die Menge der Lizenzen ändern oder das Abonnement aussetzen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="76ab6-144">**Für ISV Saas-Abonnements (Lizenz basierte und gemessene Abonnements):**</span><span class="sxs-lookup"><span data-stu-id="76ab6-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="76ab6-145">Sie erhalten einen Link zur Website des ISV-Verlegers.</span><span class="sxs-lookup"><span data-stu-id="76ab6-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="76ab6-146">Dieser Link soll Ihnen helfen, die Bereitstellung oder das Konto für das Abonnement des Kunden abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="76ab6-147">Weder Sie noch Ihr Kunde erhalten eine e-Mail mit Anweisungen zum Abschließen der Konto Einrichtung/-Bereitstellung für diese Art von ISV-Abonnement.)</span><span class="sxs-lookup"><span data-stu-id="76ab6-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="76ab6-148">Wenn Ihr Abonnement eine 30-tägige kostenlose Testversion enthält, wird der kostenlose Testzeitraum automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="76ab6-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="76ab6-149">Als Partner im CSP-Programm können Sie den kostenlosen Testzeitraum für Angebote, die Sie für Kunden erwerben, nicht aufheben.</span><span class="sxs-lookup"><span data-stu-id="76ab6-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="76ab6-150">Sobald der kostenlose Testzeitraum endet, beginnt die Abonnement Laufzeit, und das Abonnement wird in den kostenpflichtigen Status konvertiert.</span><span class="sxs-lookup"><span data-stu-id="76ab6-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="76ab6-151">Das Abonnement wird dann nach dem gleichen Zeitplan automatisch erneuert.</span><span class="sxs-lookup"><span data-stu-id="76ab6-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="76ab6-152">Aktualisieren von Abonnements mit Add-Ons</span><span class="sxs-lookup"><span data-stu-id="76ab6-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="76ab6-153">Um ein Add-on zu erwerben, muss der Kunde zuerst über ein aktives Basis Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="76ab6-154">Sie können über den Katalog keine Add-Ons erwerben.</span><span class="sxs-lookup"><span data-stu-id="76ab6-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="76ab6-155">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="76ab6-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="76ab6-156">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="76ab6-157">Wählen Sie das Abonnement aus, das Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="76ab6-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="76ab6-158">Unter dem Abschnitt **Status** finden Sie eine Liste der verfügbaren Add-ons für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="76ab6-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="76ab6-159">Aktualisieren Sie die Anzahl der Lizenzen für jedes erforderliche Add-on.</span><span class="sxs-lookup"><span data-stu-id="76ab6-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="76ab6-160">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="76ab6-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="76ab6-161">Die Möglichkeit, Add-ons über Partner Center zu erwerben, ist nur für die direkte Abrechnung und indirekte Anbieter verfügbar.</span><span class="sxs-lookup"><span data-stu-id="76ab6-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="76ab6-162">Nur berechtigte Add-ons werden basierend auf den Basis Anforderungen und der regionalen Verfügbarkeit angezeigt.</span><span class="sxs-lookup"><span data-stu-id="76ab6-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="76ab6-163">Weitere Informationen zu Preisen und Angeboten finden Sie in der Cloud Reseller offer-Matrix.</span><span class="sxs-lookup"><span data-stu-id="76ab6-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="76ab6-164">Wenn die Ausführung des Basisabonnements angehalten wird, werden auch alle zugehörigen Add-Ons angehalten.</span><span class="sxs-lookup"><span data-stu-id="76ab6-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="76ab6-165">Das Startdatum für Add-Ons richtet sich nach dem Basisabonnement, und die Gebühren werden anhand des entsprechenden Start- und Enddatums berechnet. Die erste Rechnung enthält die anteiligen Gebühren.</span><span class="sxs-lookup"><span data-stu-id="76ab6-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="76ab6-166">Weitere Informationen finden Sie unter [Lizenz basierte Abrechnung](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="76ab6-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="76ab6-167">Aussetzen oder Stornieren eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="76ab6-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="76ab6-168">Partner können ein Abonnement auf Anforderung des Kunden, bei Nichtbezahlung oder bei Betrug aussetzen oder kündigen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="76ab6-169">Aussetzen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="76ab6-169">Suspend a subscription</span></span>

<span data-ttu-id="76ab6-170">Wenn Sie den Status eines Abonnements zu **Ausgesetzt** ändern, können sich Benutzer nicht anmelden oder auf Dienste zugreifen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="76ab6-171">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="76ab6-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="76ab6-172">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="76ab6-173">Wählen Sie das Abonnement aus, das Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="76ab6-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="76ab6-174">Wählen Sie im Abschnitt **Status** die Option **Ausgesetzt** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="76ab6-175">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="76ab6-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="76ab6-176">Alle Daten werden gelöscht, solange das Abonnement nicht innerhalb von 90 Tagen oder 90 Tagen zuzüglich der Anzahl der Tage zwischen der Eröffnung des Kontos und dem ersten Abrechnungszeitraum (maximal 120 Tage) reaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="76ab6-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="76ab6-177">Wenn Sie ein Abonnement aussetzen, gibt das Datum, das unterhalb der Schaltfläche **Ausgesetzt** angezeigt wird, an, wann das Abonnement automatisch ablaufen würde, wenn Sie es nicht erneut aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76ab6-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="76ab6-178">Kündigen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="76ab6-178">Cancel a subscription</span></span>

<span data-ttu-id="76ab6-179">Sie können Lizenz basierte Saas-Abonnements von Drittanbieter-ISV-Verlegern innerhalb des [kommerziellen Marketplace](csp-commercial-marketplace-overview.md)von Partner Center kündigen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="76ab6-180">Solange Sie innerhalb des Abbruch Zeitraums abbrechen, erhalten Sie eine vollständige Rückerstattung.</span><span class="sxs-lookup"><span data-stu-id="76ab6-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="76ab6-181">Für ISV-Angebote, die monatlich abgerechnet werden:</span><span class="sxs-lookup"><span data-stu-id="76ab6-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="76ab6-182">Wenn Sie weniger als 24 Stunden abbrechen, nachdem Sie die Bestellung aufgegeben haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.</span><span class="sxs-lookup"><span data-stu-id="76ab6-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="76ab6-183">Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 24 Stunden einen Abbruch durchführen, wird der Abbruch für die Verlängerung geplant.</span><span class="sxs-lookup"><span data-stu-id="76ab6-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="76ab6-184">Für Angebote, die jährlich abgerechnet werden:</span><span class="sxs-lookup"><span data-stu-id="76ab6-184">For offers billed annually:</span></span>

- <span data-ttu-id="76ab6-185">Wenn Sie weniger als 14 Tage abbrechen, nachdem Sie die Bestellung durchgeführt haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.</span><span class="sxs-lookup"><span data-stu-id="76ab6-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="76ab6-186">Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 14 Tagen abbrechen, wird der Abbruch für die Verlängerung geplant.</span><span class="sxs-lookup"><span data-stu-id="76ab6-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="76ab6-187">Nach Ablauf dieser Zeiträume wird die Option zum Abbrechen des Abonnements nicht mehr angezeigt.</span><span class="sxs-lookup"><span data-stu-id="76ab6-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="76ab6-188">Nutzungsbasierte und gemessene ISV-Dienste von Drittanbietern (die beispielsweise virtuelle Computer oder Container verwenden) sind nicht für die Rückgabe berechtigt.</span><span class="sxs-lookup"><span data-stu-id="76ab6-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="76ab6-189">Verwendungs basierte Dienste können als Abbruch Methode deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="76ab6-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="76ab6-190">Da Gebühren nach der Verwendung abgerechnet werden, sind diese Dienste nicht für eine Rückerstattung berechtigt.</span><span class="sxs-lookup"><span data-stu-id="76ab6-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="76ab6-191">Gehen Sie zum Kündigen eines lizenzbasierten SaaS-Abonnements eines ISV-Herausgebers wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="76ab6-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="76ab6-192">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="76ab6-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="76ab6-193">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="76ab6-194">Suchen Sie das Abonnement, das Sie abbrechen möchten.</span><span class="sxs-lookup"><span data-stu-id="76ab6-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="76ab6-195">Wählen Sie in der Spalte **Status** den Wert **Abbrechen** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="76ab6-196">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="76ab6-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="76ab6-197">Wenn ein Dialogfeld angezeigt wird, füllen Sie alle relevanten Details aus, und wählen Sie dann **senden** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="76ab6-198">Um den Abbruch zu bestätigen, wählen Sie **Ja, Abbrechen** aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="76ab6-199">Sie haben auch die Möglichkeit, ein Azure Marketplace Abonnement mithilfe von APIs abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="76ab6-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="76ab6-200">Informationen hierzu finden Sie unter [Abbrechen eines Azure Marketplace Abonnements](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="76ab6-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="76ab6-201">Auswählen, ob ein Abonnement des kommerziellen Marketplace automatisch verlängert werden soll</span><span class="sxs-lookup"><span data-stu-id="76ab6-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="76ab6-202">Standardmäßig sind aktive Abonnements so festgelegt, dass sie automatisch erneuert werden, wenn der Abonnementzeitraum abläuft.</span><span class="sxs-lookup"><span data-stu-id="76ab6-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="76ab6-203">Bei [Abonnements für kommerzielle Marketplace-Produkte](csp-commercial-marketplace-overview.md)können Sie optional festlegen, dass das Abonnement nicht automatisch erneuert wird.</span><span class="sxs-lookup"><span data-stu-id="76ab6-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="76ab6-204">So beenden Sie das automatische Erneuern eines aktiven Marketplace-Abonnements:</span><span class="sxs-lookup"><span data-stu-id="76ab6-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="76ab6-205">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="76ab6-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="76ab6-206">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="76ab6-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="76ab6-207">Wählen Sie **Abonnements**.</span><span class="sxs-lookup"><span data-stu-id="76ab6-207">Select **Subscriptions**.</span></span> <span data-ttu-id="76ab6-208">Dadurch werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.</span><span class="sxs-lookup"><span data-stu-id="76ab6-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="76ab6-209">Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.</span><span class="sxs-lookup"><span data-stu-id="76ab6-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="76ab6-210">Suchen Sie auf der Seite Abonnement Details den Abschnitt **Status** , und deaktivieren Sie das Kontrollkästchen **Automatische Verlängerung** .</span><span class="sxs-lookup"><span data-stu-id="76ab6-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="76ab6-211">Klicken Sie auf **Senden**.</span><span class="sxs-lookup"><span data-stu-id="76ab6-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="76ab6-212">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="76ab6-212">Next steps</span></span>

- [<span data-ttu-id="76ab6-213">Kaufen von Produkten des kommerziellen Marketplace für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="76ab6-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="76ab6-214">Verwalten Sie kommerzielle Marketplace-Produkte für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="76ab6-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="76ab6-215">Übersicht über den kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="76ab6-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)