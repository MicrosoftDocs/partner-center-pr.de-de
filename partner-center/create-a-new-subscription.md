---
title: Erstellen von Kunden Abonnements im Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Ihre Kunden Abonnements sowohl für von Microsoft veröffentlichte Produkte als auch für SaaS-Produkte verkaufen, die von Drittanbieter-ISVs veröffentlicht werden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038879"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="8e1a1-103">Erstellen, Aussetzen oder Stornieren von Kundenabonnements</span><span class="sxs-lookup"><span data-stu-id="8e1a1-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="8e1a1-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="8e1a1-104">**Applies to**</span></span>

- <span data-ttu-id="8e1a1-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="8e1a1-105">Partner Center</span></span>
- <span data-ttu-id="8e1a1-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="8e1a1-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="8e1a1-107">CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="8e1a1-107">CSP partners</span></span>

<span data-ttu-id="8e1a1-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="8e1a1-108">**Appropriate roles**</span></span>

- <span data-ttu-id="8e1a1-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="8e1a1-109">Admin agent</span></span>
- <span data-ttu-id="8e1a1-110">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="8e1a1-110">Billing admin</span></span>
- <span data-ttu-id="8e1a1-111">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8e1a1-111">Global admin</span></span>
- <span data-ttu-id="8e1a1-112">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="8e1a1-112">Helpdesk agent</span></span>
- <span data-ttu-id="8e1a1-113">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="8e1a1-113">Sales agent</span></span>

<span data-ttu-id="8e1a1-114">Nachdem Sie für Ihre Kunden einen Datensatz im Partner Center erstellt haben, können Sie ihnen Abonnements für Produkte im Katalog verkaufen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="8e1a1-115">Dies schließt sowohl von Microsoft veröffentlichte Produkte als auch SaaS-Produkte (Software-as-a-Service) ein, die von unabhängigen Softwareanbietern (ISVs) von Drittanbietern im [kommerziellen Marketplace](https://azuremarketplace.microsoft.com/marketplace)veröffentlicht wurden.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="8e1a1-116">Einige Angebote sind auf ein Abonnement pro Kunde beschränkt.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="8e1a1-117">Eine Liste der eingeschränkten Angebote finden Sie im Partner Center auf der Seite für Preise und Angebote.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="8e1a1-118">Als Partner im CSP-Programm können Sie **Lizenz basierte** oder getaktete Saas **metered** -Abonnements von ISV-Verlegern innerhalb von Partner Center erwerben.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="8e1a1-119">Dies bedeutet, dass Sie ein **Lizenz basiertes** **oder** getaktetes SaaS-Angebot erwerben können, das der ISV-Verleger zur Verfügung gestellt hat, einschließlich [exklusiver Angebote](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , auf die Sie Zugriff haben.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="8e1a1-120">Zum Erwerb oder zur Verwaltung anderer kommerzieller Marketplace-Angebote von ISVs (z. b. nutzungsbasierte Angebote mit Azure-Anwendungen, Containern oder VMS) müssen Sie zum [Azure-Portal](https://portal.azure.com/)wechseln.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="8e1a1-121">Erstellen eines neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="8e1a1-121">Create a new subscription</span></span>

1. <span data-ttu-id="8e1a1-122">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-122">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8e1a1-123">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-123">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8e1a1-124">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-124">Select **Add subscription**.</span></span> <span data-ttu-id="8e1a1-125">Auf der Registerkarte **Online Dienste** werden alle verfügbaren Marketplace-SaaS-Angebote angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-125">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="8e1a1-126">Um nur bestimmte Arten von Abonnements anzuzeigen, treffen Sie eine Auswahl bei den verfügbaren Filter:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-126">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="8e1a1-127">**Herausgeber**: Wählen Sie **Microsoft** aus, um nur Angebote von Microsoft oder **Partnern** anzuzeigen, um kommerzielle Marketplace-Produkte anzuzeigen, die von ISVs veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-127">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="8e1a1-128">**Abrechnungstyp**: Wählen Sie den Typ der Abonnement Abrechnung aus, den Sie verwenden möchten: **Lizenz** oder **Nutzung**.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-128">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="8e1a1-129">Informationen, die Ihnen bei der Entscheidung zwischen monatlicher und jährlicher Abrechnungs Häufigkeit helfen, finden Sie unter [Lizenz basierte Abrechnung](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="8e1a1-129">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="8e1a1-130">**Kategorie**: Wählen Sie **Enterprise**, **Small Business** oder **Testversion** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-130">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="8e1a1-131">Informationen zu Testabonnements finden Sie unter [Testversionen von Microsoft-Produkten anbieten](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="8e1a1-131">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="8e1a1-132">Wählen Sie die Produkt Abonnements aus, die Sie für Ihren Kunden erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-132">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="8e1a1-133">Welche Produkte Sie sehen, hängt vom Typ des Kunden Segments (Education, Government usw.) und den von Ihnen angewendeten Filtern ab.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-133">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="8e1a1-134">Einige Angebote, die auf dem Marketplace angezeigt werden, sind möglicherweise nicht immer für einen bestimmten Kunden oder einen bestimmten CSP-Partner verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-134">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="8e1a1-135">Dies kann folgende Ursache haben:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-135">This can be because:</span></span>

   - <span data-ttu-id="8e1a1-136">Der Kunde hat bereits ein Abonnement für dieses Produkt und ist nur eins zulässig.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-136">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="8e1a1-137">Das Abonnement des Kunden wurde möglicherweise angehalten (in diesem Fall können Sie das Abonnement reaktivieren, anstatt ein neues zu erwerben).</span><span class="sxs-lookup"><span data-stu-id="8e1a1-137">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="8e1a1-138">Für ISV-SaaS-Angebote gibt es möglicherweise einige Gründe, warum das Angebot nicht erworben werden kann: der ISV unterstützt das Abrechnungs Land oder die Region des Kunden möglicherweise nicht. der ISV hat möglicherweise entschieden, das Angebot nicht über das CSP-Programm verfügbar zu machen. oder der ISV hat das Angebot möglicherweise nur für bestimmte CSP-Partner [exklusiv](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gestaltet.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-138">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="8e1a1-139">Das ISV-Angebot kann auch nicht über das Partner Center (z. b. Container oder einige Verwendungs basierte Angebote) übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-139">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="8e1a1-140">Geben Sie für jedes Abonnement, das Sie hinzufügen möchten, die Anzahl der Lizenzen (falls erforderlich) ein, und wählen Sie **zum Warenkorb hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-140">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="8e1a1-141">Nachdem Sie Abonnements hinzugefügt haben, wählen Sie **überprüfen** aus, und überprüfen Sie Ihre Bestellung.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-141">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="8e1a1-142">Nachdem Sie Ihre Bestellungen überprüft haben und bereit sind, diese Abonnements zu erwerben, wählen Sie **kaufen** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-142">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="8e1a1-143">Wenn Sie ein Abonnement für einen Kunden erworben haben, tritt Folgendes auf:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-143">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="8e1a1-144">Sie können das Abonnement überprüfen oder bearbeiten, indem Sie den Abonnement Namen **auf der Abonnementseite des** Kunden auswählen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-144">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="8e1a1-145">Dort können Sie Add-On-Lizenzen auswählen, falls verfügbar, die Menge der Lizenzen ändern oder das Abonnement aussetzen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-145">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="8e1a1-146">**Für ISV Saas-Abonnements (Lizenz basierte und gemessene Abonnements):**</span><span class="sxs-lookup"><span data-stu-id="8e1a1-146">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="8e1a1-147">Sie erhalten einen Link zur Website des ISV-Verlegers.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-147">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="8e1a1-148">Dieser Link soll Ihnen helfen, die Bereitstellung oder das Konto für das Abonnement des Kunden abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-148">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="8e1a1-149">Weder Sie noch Ihr Kunde erhalten eine e-Mail mit Anweisungen zum Abschließen der Konto Einrichtung/-Bereitstellung für diese Art von ISV-Abonnement.)</span><span class="sxs-lookup"><span data-stu-id="8e1a1-149">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="8e1a1-150">Wenn Ihr Abonnement eine 30-tägige kostenlose Testversion enthält, wird der kostenlose Testzeitraum automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-150">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="8e1a1-151">Als Partner im CSP-Programm können Sie den kostenlosen Testzeitraum für Angebote, die Sie für Kunden erwerben, nicht aufheben.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-151">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="8e1a1-152">Sobald der kostenlose Testzeitraum endet, beginnt die Abonnement Laufzeit, und das Abonnement wird in den kostenpflichtigen Status konvertiert.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-152">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="8e1a1-153">Das Abonnement wird dann nach dem gleichen Zeitplan automatisch erneuert.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-153">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="8e1a1-154">Aktualisieren von Abonnements mit Add-Ons</span><span class="sxs-lookup"><span data-stu-id="8e1a1-154">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="8e1a1-155">Zum Erwerben eines Add-Ons muss der Kunde zunächst über ein aktives Basisabonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-155">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="8e1a1-156">Sie können über den Katalog keine Add-Ons erwerben.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-156">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="8e1a1-157">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-157">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8e1a1-158">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-158">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8e1a1-159">Wählen Sie das Abonnement aus, das Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-159">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="8e1a1-160">Unter dem Abschnitt **Status** finden Sie eine Liste der verfügbaren Add-ons für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-160">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="8e1a1-161">Aktualisieren Sie die Anzahl der Lizenzen für jedes erforderliche Add-on.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-161">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="8e1a1-162">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-162">Then **Submit** your changes.</span></span>

<span data-ttu-id="8e1a1-163">Die Möglichkeit, Add-ons über Partner Center zu erwerben, ist nur für die direkte Abrechnung und indirekte Anbieter verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-163">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="8e1a1-164">Nur berechtigte Add-ons werden basierend auf den Basis Anforderungen und der regionalen Verfügbarkeit angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-164">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="8e1a1-165">Weitere Informationen zu Preisen und Angeboten finden Sie in der Cloud Reseller-Angebotsmatrix.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-165">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="8e1a1-166">Wenn die Ausführung des Basisabonnements angehalten wird, werden auch alle zugehörigen Add-Ons angehalten.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-166">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="8e1a1-167">Das Startdatum für Add-Ons richtet sich nach dem Basisabonnement, und die Gebühren werden anhand des entsprechenden Start- und Enddatums berechnet. Die erste Rechnung enthält die anteiligen Gebühren.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-167">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="8e1a1-168">Weitere Informationen finden Sie unter [Lizenz basierte Abrechnung](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="8e1a1-168">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="8e1a1-169">Aussetzen oder Stornieren eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="8e1a1-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="8e1a1-170">Partner können ein Abonnement auf Anforderung des Kunden, bei Nichtbezahlung oder bei Betrug aussetzen oder kündigen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="8e1a1-171">Aussetzen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="8e1a1-171">Suspend a subscription</span></span>

<span data-ttu-id="8e1a1-172">Wenn Sie den Status eines Abonnements zu **Ausgesetzt** ändern, können sich Benutzer nicht anmelden oder auf Dienste zugreifen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="8e1a1-173">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8e1a1-174">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8e1a1-175">Wählen Sie das Abonnement aus, das Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="8e1a1-176">Wählen Sie im Abschnitt **Status** die Option **Ausgesetzt** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="8e1a1-177">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="8e1a1-178">Alle Daten werden gelöscht, solange das Abonnement nicht innerhalb von 90 Tagen oder 90 Tagen zuzüglich der Anzahl der Tage zwischen der Eröffnung des Kontos und dem ersten Abrechnungszeitraum (maximal 120 Tage) reaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="8e1a1-179">Wenn Sie ein Abonnement aussetzen, gibt das Datum, das unterhalb der Schaltfläche **Ausgesetzt** angezeigt wird, an, wann das Abonnement automatisch ablaufen würde, wenn Sie es nicht erneut aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="8e1a1-180">Kündigen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="8e1a1-180">Cancel a subscription</span></span>

<span data-ttu-id="8e1a1-181">Sie haben die Möglichkeit, Lizenz basierte Saas-Abonnements von Drittanbieter-ISV-Verlegern innerhalb des [kommerziellen Marketplace](csp-commercial-marketplace-overview.md)von Partner Center abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="8e1a1-182">Solange Sie innerhalb des Abbruch Zeitraums abbrechen, erhalten Sie eine vollständige Rückerstattung.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="8e1a1-183">Für ISV-Angebote, die monatlich abgerechnet werden:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="8e1a1-184">Wenn Sie weniger als 24 Stunden abbrechen, nachdem Sie die Bestellung aufgegeben haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="8e1a1-185">Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 24 Stunden einen Abbruch durchführen, wird der Abbruch für die Verlängerung geplant.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="8e1a1-186">Für Angebote, die jährlich abgerechnet werden:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-186">For offers billed annually:</span></span>

- <span data-ttu-id="8e1a1-187">Wenn Sie weniger als 14 Tage abbrechen, nachdem Sie die Bestellung durchgeführt haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="8e1a1-188">Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 14 Tagen abbrechen, wird der Abbruch für die Verlängerung geplant.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="8e1a1-189">Nach Ablauf dieser Zeiträume wird die Option zum Abbrechen des Abonnements nicht mehr angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="8e1a1-190">Nutzungsbasierte und gemessene ISV-Dienste von Drittanbietern (die beispielsweise virtuelle Computer oder Container verwenden) sind nicht für die Rückgabe berechtigt.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="8e1a1-191">Verwendungs basierte Dienste können als Abbruch Methode deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="8e1a1-192">Da Gebühren nach der Verwendung abgerechnet werden, sind diese Dienste nicht für eine Rückerstattung berechtigt.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="8e1a1-193">Gehen Sie zum Kündigen eines lizenzbasierten SaaS-Abonnements eines ISV-Herausgebers wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="8e1a1-194">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8e1a1-195">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8e1a1-196">Suchen Sie das Abonnement, das Sie abbrechen möchten.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="8e1a1-197">Wählen Sie in der Spalte **Status** den Wert **Abbrechen** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="8e1a1-198">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="8e1a1-199">Wenn ein Dialogfeld angezeigt wird, füllen Sie alle relevanten Details aus, und wählen Sie dann **senden** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="8e1a1-200">Um den Abbruch zu bestätigen, wählen Sie **Ja, Abbrechen** aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="8e1a1-201">Sie haben auch die Möglichkeit, ein Azure Marketplace Abonnement mithilfe von APIs abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="8e1a1-202">Informationen hierzu finden Sie unter [Abbrechen eines Azure Marketplace Abonnements](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="8e1a1-202">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="8e1a1-203">Auswählen, ob ein Abonnement des kommerziellen Marketplace automatisch verlängert werden soll</span><span class="sxs-lookup"><span data-stu-id="8e1a1-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="8e1a1-204">Standardmäßig sind aktive Abonnements so festgelegt, dass sie automatisch erneuert werden, wenn der Abonnementzeitraum abläuft.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="8e1a1-205">Bei [Abonnements für kommerzielle Marketplace-Produkte](csp-commercial-marketplace-overview.md)können Sie optional festlegen, dass das Abonnement nicht automatisch erneuert wird.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="8e1a1-206">So beenden Sie das automatische Erneuern eines aktiven Marketplace-Abonnements:</span><span class="sxs-lookup"><span data-stu-id="8e1a1-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="8e1a1-207">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8e1a1-208">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8e1a1-209">Wählen Sie **Abonnements**.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-209">Select **Subscriptions**.</span></span> <span data-ttu-id="8e1a1-210">Dadurch werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="8e1a1-211">Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.</span><span class="sxs-lookup"><span data-stu-id="8e1a1-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="8e1a1-212">Suchen Sie auf der Seite Abonnement Details den Abschnitt **Status** , und deaktivieren Sie das Kontrollkästchen **Automatische Verlängerung** .</span><span class="sxs-lookup"><span data-stu-id="8e1a1-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="8e1a1-213">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="8e1a1-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8e1a1-214">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="8e1a1-214">Next steps</span></span>

- [<span data-ttu-id="8e1a1-215">Kaufen von Produkten des kommerziellen Marketplace für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="8e1a1-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="8e1a1-216">Verwalten Sie kommerzielle Marketplace-Produkte für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="8e1a1-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="8e1a1-217">Übersicht über den kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="8e1a1-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)