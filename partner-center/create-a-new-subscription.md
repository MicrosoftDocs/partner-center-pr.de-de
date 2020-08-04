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
ms.openlocfilehash: 66c8b490e69e9b03ec0db213ca2a5baf3d42635e
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527803"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="c61de-103">Erstellen, Aussetzen oder Stornieren von Kundenabonnements</span><span class="sxs-lookup"><span data-stu-id="c61de-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="c61de-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="c61de-104">**Applies to**</span></span>

- <span data-ttu-id="c61de-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c61de-105">Partner Center</span></span>
- <span data-ttu-id="c61de-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c61de-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="c61de-107">CSP-Partner</span><span class="sxs-lookup"><span data-stu-id="c61de-107">CSP partners</span></span>

<span data-ttu-id="c61de-108">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="c61de-108">**Appropriate roles**</span></span>

- <span data-ttu-id="c61de-109">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="c61de-109">Admin agent</span></span>
- <span data-ttu-id="c61de-110">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="c61de-110">Billing admin</span></span>
- <span data-ttu-id="c61de-111">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="c61de-111">Global admin</span></span>
- <span data-ttu-id="c61de-112">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="c61de-112">Helpdesk agent</span></span>
- <span data-ttu-id="c61de-113">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="c61de-113">Sales agent</span></span>

<span data-ttu-id="c61de-114">Nachdem Sie für Ihre Kunden einen Datensatz im Partner Center erstellt haben, können Sie ihnen Abonnements für Produkte im Katalog verkaufen.</span><span class="sxs-lookup"><span data-stu-id="c61de-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="c61de-115">Dies schließt sowohl von Microsoft veröffentlichte Produkte als auch SaaS-Produkte (Software-as-a-Service) ein, die von unabhängigen Softwareanbietern (ISVs) von Drittanbietern im [kommerziellen Marketplace](https://azuremarketplace.microsoft.com/marketplace)veröffentlicht wurden.</span><span class="sxs-lookup"><span data-stu-id="c61de-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="c61de-116">Einige Angebote sind auf ein Abonnement pro Kunde beschränkt.</span><span class="sxs-lookup"><span data-stu-id="c61de-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="c61de-117">Eine Liste der eingeschränkten Angebote finden Sie im Partner Center auf der Seite für Preise und Angebote.</span><span class="sxs-lookup"><span data-stu-id="c61de-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c61de-118">Als Partner im CSP-Programm können Sie nur **Lizenz basierte Saas-** Abonnements von ISV-Verlegern innerhalb von Partner Center erwerben.</span><span class="sxs-lookup"><span data-stu-id="c61de-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="c61de-119">Dies bedeutet, dass Sie alle **lizenzbasierten Saas-** Angebote erwerben können, die der ISV-Verleger Ihnen zur Verfügung gestellt hat, einschließlich [exklusiver Angebote](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , auf die Sie Zugriff haben.</span><span class="sxs-lookup"><span data-stu-id="c61de-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="c61de-120">Zum Erwerb oder zur Verwaltung anderer kommerzieller Marketplace-Angebote von ISVs (z. b. **nutzungsbasierte**, gemessene oder Verbrauchs basierte Angebote mit Azure-Anwendungen, Containern oder VMS) müssen Sie das Azure- [Verwaltungs Portal](https://portal.azure.com/)aufrufen.</span><span class="sxs-lookup"><span data-stu-id="c61de-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="c61de-121">Weitere Informationen finden Sie unter [erwerben kommerzieller Marketplace-Produkte](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="c61de-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="c61de-122">Erstellen eines neuen Abonnements</span><span class="sxs-lookup"><span data-stu-id="c61de-122">Create a new subscription</span></span>

1. <span data-ttu-id="c61de-123">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="c61de-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c61de-124">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c61de-125">Wählen Sie **Abonnement hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-125">Select **Add subscription**.</span></span> <span data-ttu-id="c61de-126">Auf der Registerkarte **Online Dienste** werden alle verfügbaren Marketplace-SaaS-Angebote angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c61de-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="c61de-127">Um nur bestimmte Arten von Abonnements anzuzeigen, treffen Sie eine Auswahl bei den verfügbaren Filter:</span><span class="sxs-lookup"><span data-stu-id="c61de-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="c61de-128">**Herausgeber**: Wählen Sie **Microsoft** aus, um nur Angebote von Microsoft oder **Partnern** anzuzeigen, um kommerzielle Marketplace-Produkte anzuzeigen, die von ISVs veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="c61de-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="c61de-129">**Abrechnungstyp**: Wählen Sie den Typ der Abonnement Abrechnung aus, den Sie verwenden möchten: **Lizenz** oder **Nutzung**.</span><span class="sxs-lookup"><span data-stu-id="c61de-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="c61de-130">Informationen, die Ihnen bei der Entscheidung zwischen monatlicher und jährlicher Abrechnungs Häufigkeit helfen, finden Sie unter [Lizenz basierte Abrechnung](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="c61de-130">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="c61de-131">**Kategorie**: Wählen Sie **Enterprise**, **Small Business**oder **Testversion**aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="c61de-132">Informationen zu Testabonnements finden Sie unter [Testversionen von Microsoft-Produkten anbieten](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="c61de-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="c61de-133">Wählen Sie die Produkt Abonnements aus, die Sie für Ihren Kunden erwerben möchten.</span><span class="sxs-lookup"><span data-stu-id="c61de-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="c61de-134">Welche Produkte Sie sehen, hängt vom Typ des Kunden Segments (Education, Government usw.) und den von Ihnen angewendeten Filtern ab.</span><span class="sxs-lookup"><span data-stu-id="c61de-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="c61de-135">Einige Angebote, die auf dem Marketplace angezeigt werden, sind möglicherweise nicht immer für einen bestimmten Kunden oder einen bestimmten CSP-Partner verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c61de-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="c61de-136">Dies kann folgende Ursache haben:</span><span class="sxs-lookup"><span data-stu-id="c61de-136">This can be because:</span></span>

   - <span data-ttu-id="c61de-137">Der Kunde hat bereits ein Abonnement für dieses Produkt und ist nur eins zulässig.</span><span class="sxs-lookup"><span data-stu-id="c61de-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="c61de-138">Das Abonnement des Kunden wurde möglicherweise angehalten (in diesem Fall können Sie das Abonnement reaktivieren, anstatt ein neues zu erwerben).</span><span class="sxs-lookup"><span data-stu-id="c61de-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="c61de-139">Für ISV-SaaS-Angebote gibt es möglicherweise einige Gründe, warum das Angebot nicht erworben werden kann: der ISV unterstützt das Abrechnungs Land oder die Region des Kunden möglicherweise nicht. der ISV hat möglicherweise entschieden, das Angebot nicht über das CSP-Programm verfügbar zu machen. oder der ISV hat das Angebot möglicherweise nur für bestimmte CSP-Partner [exklusiv](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gestaltet.</span><span class="sxs-lookup"><span data-stu-id="c61de-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="c61de-140">Das ISV-Angebot kann auch nicht über das Partner Center (z. b. Container oder einige Verwendungs basierte Angebote) übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="c61de-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="c61de-141">Geben Sie für jedes Abonnement, das Sie hinzufügen möchten, die Anzahl der Lizenzen (falls erforderlich) ein, und wählen Sie **zum Warenkorb hinzufügen**aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="c61de-142">Nachdem Sie Abonnements hinzugefügt haben, wählen Sie **überprüfen** aus, und überprüfen Sie Ihre Bestellung.</span><span class="sxs-lookup"><span data-stu-id="c61de-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="c61de-143">Nachdem Sie Ihre Bestellungen überprüft haben und bereit sind, diese Abonnements zu erwerben, wählen Sie **kaufen**aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="c61de-144">Wenn Sie ein Abonnement für einen Kunden erworben haben, tritt Folgendes auf:</span><span class="sxs-lookup"><span data-stu-id="c61de-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="c61de-145">Sie können das Abonnement überprüfen oder bearbeiten, indem Sie den Abonnement Namen **auf der Abonnementseite des** Kunden auswählen.</span><span class="sxs-lookup"><span data-stu-id="c61de-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="c61de-146">Dort können Sie Add-On-Lizenzen auswählen, falls verfügbar, die Menge der Lizenzen ändern oder das Abonnement aussetzen.</span><span class="sxs-lookup"><span data-stu-id="c61de-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="c61de-147">**Für ISV Saas-Abonnements (Lizenz basiert):**</span><span class="sxs-lookup"><span data-stu-id="c61de-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="c61de-148">Sie erhalten einen Link zur Website des ISV-Verlegers.</span><span class="sxs-lookup"><span data-stu-id="c61de-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="c61de-149">Dieser Link soll Ihnen helfen, die Bereitstellung oder das Konto für das Abonnement des Kunden abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="c61de-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="c61de-150">Weder Sie noch Ihr Kunde erhalten eine e-Mail mit Anweisungen zum Abschließen der Konto Einrichtung/-Bereitstellung für diese Art von ISV-Abonnement.)</span><span class="sxs-lookup"><span data-stu-id="c61de-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="c61de-151">Wenn Ihr Abonnement eine 30-tägige kostenlose Testversion enthält, wird der kostenlose Testzeitraum automatisch angewendet.</span><span class="sxs-lookup"><span data-stu-id="c61de-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="c61de-152">Als Partner im CSP-Programm können Sie den kostenlosen Testzeitraum für Angebote, die Sie für Kunden erwerben, nicht aufheben.</span><span class="sxs-lookup"><span data-stu-id="c61de-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="c61de-153">Sobald der kostenlose Testzeitraum endet, beginnt die Abonnement Laufzeit, und das Abonnement wird in den kostenpflichtigen Status konvertiert.</span><span class="sxs-lookup"><span data-stu-id="c61de-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="c61de-154">Das Abonnement wird dann nach dem gleichen Zeitplan automatisch erneuert.</span><span class="sxs-lookup"><span data-stu-id="c61de-154">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="c61de-155">Aktualisieren von Abonnements mit Add-ons</span><span class="sxs-lookup"><span data-stu-id="c61de-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="c61de-156">Um ein Add-on zu erwerben, muss der Kunde zuerst über ein aktives Basis Abonnement verfügen.</span><span class="sxs-lookup"><span data-stu-id="c61de-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="c61de-157">Sie können keine Add-ons über den Katalog erwerben.</span><span class="sxs-lookup"><span data-stu-id="c61de-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="c61de-158">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="c61de-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c61de-159">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-159">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c61de-160">Wählen Sie das Abonnement aus, das Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="c61de-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c61de-161">Unter dem Abschnitt **Status** finden Sie eine Liste der verfügbaren Add-ons für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c61de-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="c61de-162">Aktualisieren Sie die Anzahl der Lizenzen für jedes erforderliche Add-on.</span><span class="sxs-lookup"><span data-stu-id="c61de-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="c61de-163">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="c61de-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="c61de-164">Die Möglichkeit, Add-ons über Partner Center zu erwerben, ist nur für die direkte Abrechnung und indirekte Anbieter verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c61de-164">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="c61de-165">Nur berechtigte Add-ons werden basierend auf den Basis Anforderungen und der regionalen Verfügbarkeit angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c61de-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="c61de-166">Weitere Informationen zu Preisen und Angeboten finden Sie in der Cloud Reseller offer-Matrix.</span><span class="sxs-lookup"><span data-stu-id="c61de-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="c61de-167">Durch das Anhalten des Basisabonnements werden auch alle zugehörigen Add-ons angehalten.</span><span class="sxs-lookup"><span data-stu-id="c61de-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="c61de-168">Startdatums Angaben für Add-ons richten sich an das Basis Abonnement, und die Gebühren werden aus dem Startdatum der Gebühr und dem Abrechnungsdatum für die ersten Rechnung berechnet.</span><span class="sxs-lookup"><span data-stu-id="c61de-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="c61de-169">Weitere Informationen finden Sie unter [Lizenz basierte Abrechnung](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="c61de-169">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="c61de-170">Aussetzen oder Stornieren eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="c61de-170">Suspend or cancel a subscription</span></span>

<span data-ttu-id="c61de-171">Partner können ein Abonnement auf Anforderung des Kunden, bei Nichtbezahlung oder bei Betrug aussetzen oder kündigen.</span><span class="sxs-lookup"><span data-stu-id="c61de-171">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="c61de-172">Aussetzen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="c61de-172">Suspend a subscription</span></span>

<span data-ttu-id="c61de-173">Wenn Sie den Status eines Abonnements zu **Ausgesetzt** ändern, können sich Benutzer nicht anmelden oder auf Dienste zugreifen.</span><span class="sxs-lookup"><span data-stu-id="c61de-173">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="c61de-174">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="c61de-174">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c61de-175">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-175">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c61de-176">Wählen Sie das Abonnement aus, das Sie verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="c61de-176">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c61de-177">Wählen Sie im Abschnitt **Status** die Option **Ausgesetzt** aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-177">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="c61de-178">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="c61de-178">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c61de-179">Alle Daten werden gelöscht, solange das Abonnement nicht innerhalb von 90 Tagen oder 90 Tagen zuzüglich der Anzahl der Tage zwischen der Eröffnung des Kontos und dem ersten Abrechnungszeitraum (maximal 120 Tage) reaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="c61de-179">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="c61de-180">Wenn Sie ein Abonnement aussetzen, gibt das Datum, das unterhalb der Schaltfläche **Ausgesetzt** angezeigt wird, an, wann das Abonnement automatisch ablaufen würde, wenn Sie es nicht erneut aktivieren.</span><span class="sxs-lookup"><span data-stu-id="c61de-180">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="c61de-181">Kündigen eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="c61de-181">Cancel a subscription</span></span>

<span data-ttu-id="c61de-182">Sie haben die Möglichkeit, Lizenz basierte Saas-Abonnements von Drittanbieter-ISV-Verlegern innerhalb des [kommerziellen Marketplace](csp-commercial-marketplace-overview.md)von Partner Center abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="c61de-182">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="c61de-183">Solange Sie innerhalb des Abbruch Zeitraums abbrechen, erhalten Sie eine vollständige Rückerstattung.</span><span class="sxs-lookup"><span data-stu-id="c61de-183">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="c61de-184">Für ISV-Angebote, die monatlich abgerechnet werden:</span><span class="sxs-lookup"><span data-stu-id="c61de-184">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="c61de-185">Wenn Sie weniger als 24 Stunden abbrechen, nachdem Sie die Bestellung aufgegeben haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.</span><span class="sxs-lookup"><span data-stu-id="c61de-185">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c61de-186">Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 24 Stunden einen Abbruch durchführen, wird der Abbruch für die Verlängerung geplant.</span><span class="sxs-lookup"><span data-stu-id="c61de-186">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c61de-187">Für Angebote, die jährlich abgerechnet werden:</span><span class="sxs-lookup"><span data-stu-id="c61de-187">For offers billed annually:</span></span>

- <span data-ttu-id="c61de-188">Wenn Sie weniger als 14 Tage abbrechen, nachdem Sie die Bestellung durchgeführt haben, erhalten Sie eine vollständige Gutschrift für die nächste Rechnung.</span><span class="sxs-lookup"><span data-stu-id="c61de-188">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c61de-189">Wenn Sie nach dem Platzieren der Bestellung nach einem Abbruch nach 14 Tagen abbrechen, wird der Abbruch für die Verlängerung geplant.</span><span class="sxs-lookup"><span data-stu-id="c61de-189">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c61de-190">Nach Ablauf dieser Zeiträume wird die Option zum Abbrechen des Abonnements nicht mehr angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c61de-190">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="c61de-191">Nutzungsbasierte und gemessene ISV-Dienste von Drittanbietern (die beispielsweise virtuelle Computer oder Container verwenden) sind nicht für die Rückgabe berechtigt.</span><span class="sxs-lookup"><span data-stu-id="c61de-191">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="c61de-192">Verwendungs basierte Dienste können als Abbruch Methode deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="c61de-192">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="c61de-193">Da Gebühren nach der Verwendung abgerechnet werden, sind diese Dienste nicht für eine Rückerstattung berechtigt.</span><span class="sxs-lookup"><span data-stu-id="c61de-193">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="c61de-194">Gehen Sie zum Kündigen eines lizenzbasierten SaaS-Abonnements eines ISV-Herausgebers wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="c61de-194">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="c61de-195">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="c61de-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c61de-196">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c61de-197">Suchen Sie das Abonnement, das Sie abbrechen möchten.</span><span class="sxs-lookup"><span data-stu-id="c61de-197">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="c61de-198">Wählen Sie in der Spalte **Status** den Wert **Abbrechen**aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-198">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="c61de-199">Wählen Sie anschließend **Übermitteln** aus, um Ihre Änderungen zu übermitteln.</span><span class="sxs-lookup"><span data-stu-id="c61de-199">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c61de-200">Wenn ein Dialogfeld angezeigt wird, füllen Sie alle relevanten Details aus, und wählen Sie dann **senden**aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-200">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="c61de-201">Um den Abbruch zu bestätigen, wählen Sie **Ja, Abbrechen**aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-201">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="c61de-202">Sie haben auch die Möglichkeit, ein Azure Marketplace Abonnement mithilfe von APIs abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="c61de-202">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="c61de-203">Informationen hierzu finden Sie unter [Abbrechen eines Azure Marketplace Abonnements](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="c61de-203">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="c61de-204">Auswählen, ob ein Abonnement des kommerziellen Marketplace automatisch verlängert werden soll</span><span class="sxs-lookup"><span data-stu-id="c61de-204">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="c61de-205">Standardmäßig sind aktive Abonnements so festgelegt, dass sie automatisch erneuert werden, wenn der Abonnementzeitraum abläuft.</span><span class="sxs-lookup"><span data-stu-id="c61de-205">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="c61de-206">Bei [Abonnements für kommerzielle Marketplace-Produkte](csp-commercial-marketplace-overview.md)können Sie optional festlegen, dass das Abonnement nicht automatisch erneuert wird.</span><span class="sxs-lookup"><span data-stu-id="c61de-206">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="c61de-207">So beenden Sie das automatische Erneuern eines aktiven Marketplace-Abonnements:</span><span class="sxs-lookup"><span data-stu-id="c61de-207">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="c61de-208">Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard) an.</span><span class="sxs-lookup"><span data-stu-id="c61de-208">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c61de-209">Wählen Sie im Menü „Partner Center“ die Option **Kunden** aus, und wählen Sie dann einen Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c61de-209">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c61de-210">Wählen Sie **Abonnements**.</span><span class="sxs-lookup"><span data-stu-id="c61de-210">Select **Subscriptions**.</span></span> <span data-ttu-id="c61de-211">Dadurch werden alle lizenzbasierten Abonnements aufgelistet, die Sie für den Kunden erworben haben.</span><span class="sxs-lookup"><span data-stu-id="c61de-211">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="c61de-212">Wählen Sie in der Spalte **Abonnement** das Abonnement aus, das Sie ändern möchten.</span><span class="sxs-lookup"><span data-stu-id="c61de-212">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="c61de-213">Suchen Sie auf der Seite Abonnement Details den Abschnitt **Status** , und deaktivieren Sie das Kontrollkästchen **Automatische Verlängerung** .</span><span class="sxs-lookup"><span data-stu-id="c61de-213">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="c61de-214">Klicken Sie auf **Submit** (Senden).</span><span class="sxs-lookup"><span data-stu-id="c61de-214">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c61de-215">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="c61de-215">Next steps</span></span>

- [<span data-ttu-id="c61de-216">Kaufen von Produkten des kommerziellen Marketplace für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="c61de-216">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="c61de-217">Verwalten Sie kommerzielle Marketplace-Produkte für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="c61de-217">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="c61de-218">Übersicht über den kommerziellen Marketplace</span><span class="sxs-lookup"><span data-stu-id="c61de-218">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
