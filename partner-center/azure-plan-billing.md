---
title: 'Azure-Plan: Abrechnung – Rechnungs- und Kontenabstimmungsdateien'
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie auf die Struktur der Rechnungs-/Abstimmungsdatei im Zusammenhang mit der Abrechnung für den Azure-Plan zugreifen und sie verstehen können.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f0246338ef8c0da06dce557573cd2811d07a0e9e
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908360"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="2b3ac-103">Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="2b3ac-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="2b3ac-104">**Geeignete Rollen:**</span><span class="sxs-lookup"><span data-stu-id="2b3ac-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="2b3ac-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="2b3ac-105">Admin agent</span></span>
- <span data-ttu-id="2b3ac-106">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="2b3ac-106">Billing admin</span></span>
- <span data-ttu-id="2b3ac-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2b3ac-107">Global admin</span></span>

<span data-ttu-id="2b3ac-108">Abrechnungen im Rahmen eines Azure-Plans bieten ein vereinfachtes Abrechnungsverfahren, das ein einheitliches Abrechnungsdatum und einen Abrechnungszeitraum auf der Grundlage von Kalendermonaten verwendet.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="2b3ac-109">Zusammenfassung der Abrechnungsgrundlagen</span><span class="sxs-lookup"><span data-stu-id="2b3ac-109">Summary of billing essentials</span></span>

- <span data-ttu-id="2b3ac-110">**Rechnungsdatum**: Die Rechnungs- und Abstimmungsdatei steht auf dem Partner Center-Dashboard bzw. über die -API am 8. des Monats zur Verfügung (Mitternacht UTC).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-110">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="2b3ac-111">**Abrechnungszeitraum der Rechnung**: Der Abrechnungszeitraum der Rechnung ist am Kalendermonat ausgerichtet, z.B. 01.10.–31.10., 01.11.–30.11.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-111">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="2b3ac-112">**Belastung von Dienstzeiträumen**: Die Gebühren richten sich nach dem Kalendermonat.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-112">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="2b3ac-113">Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-113">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="2b3ac-114">Die Rechnung des nächsten Monats, die am 08.12. generiert wird, enthält alle Gebühren für den Dienstzeitraum vom 01.11.–31.11.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-114">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="2b3ac-115">**Fälligkeit der Rechnung**: 60 Tage netto.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-115">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="2b3ac-116">**Rechnungswährung** : Partner werden weiterhin in der offiziellen Landeswährung des Kunden abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-116">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="2b3ac-117">Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-117">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="2b3ac-118">**Partnerincentives**: 45 Tage nach dem Ende des Rechnungsmonats bezahlt.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-118">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="2b3ac-119">Zugriff auf Ihre Rechnungen und Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="2b3ac-119">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="2b3ac-120">Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-120">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="2b3ac-121">**Zugriff auf die Rechnungs- und Abstimmungsdatei**</span><span class="sxs-lookup"><span data-stu-id="2b3ac-121">**To access the invoice and reconciliation file**</span></span>

1. <span data-ttu-id="2b3ac-122">Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/en-us/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-122">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/).</span></span>

2. <span data-ttu-id="2b3ac-123">Wählen Sie im Menü des Partner Center **Abrechnung** aus.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-123">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="2b3ac-124">Wählen Sie die Registerkarte für **laufende** und **einmalige** Gebühren sowie die für Sie relevante Währung aus.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-124">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

![Abrechnung](images/azure/billing3.png)

4. <span data-ttu-id="2b3ac-126">Wählen Sie **Rechnung** oder **Abstimmungsdatei** aus.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-126">Select **Invoice** or **Reconciliation file**.</span></span>  

<span data-ttu-id="2b3ac-127">Zum Anzeigen früherer Rechnungen und Abstimmungsdateien erweitern Sie die Zeile „Abrechnungsverlauf“ unten.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-127">To view historical invoices and recon files expand the Billing history row below.</span></span>


## <a name="understanding-usage-data"></a><span data-ttu-id="2b3ac-128">Grundlegendes zu Verwendungsdaten</span><span class="sxs-lookup"><span data-stu-id="2b3ac-128">Understanding usage data</span></span> 

1. <span data-ttu-id="2b3ac-129">Der Azure-Plan ist der Stammcontainer oder der Container der obersten Ebene für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-129">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="2b3ac-130">Alle Verwendungsdaten sind an einen einzelnen Azure-Plan gebunden.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-130">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="2b3ac-131">Ein Plan kann ein oder mehrere Azure-Abonnements enthalten.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-131">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="2b3ac-132">Dies sind Container, die für die Ressourcenverwaltung und -bereitstellung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-132">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="2b3ac-133">Innerhalb eines Abonnements werden Ressourcengruppen zu Gruppenressourcen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-133">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="2b3ac-134">Jede Ressource wird in einer Ressourcengruppe bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-134">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="2b3ac-135">Beispiele für Ressourcen sind virtuelle Computer und Speicherkonten.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-135">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="2b3ac-136">Ressourcen geben Verbrauchszähler aus: Verbrauchszähler sind Verbrauchsmessungen einer Ressource, und eine Ressource kann Verwendungsdaten für verschiedene Verbrauchszähler ausgeben.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-136">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="2b3ac-137">Verbrauchszähler werden durch „ProductId“-, „SKUId“- und „AvailabilityId“-Werte identifiziert.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-137">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="2b3ac-138">Hierarchie von Abonnementressourcengruppen und -messungen</span><span class="sxs-lookup"><span data-stu-id="2b3ac-138">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="2b3ac-139">**Azure-Konto (Mandant)**</span><span class="sxs-lookup"><span data-stu-id="2b3ac-139">**Azure account (tenant)**</span></span>

- <span data-ttu-id="2b3ac-140">Abonnement A</span><span class="sxs-lookup"><span data-stu-id="2b3ac-140">Subscription A</span></span>
    - <span data-ttu-id="2b3ac-141">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="2b3ac-141">ResourceGroup 1</span></span>
        - <span data-ttu-id="2b3ac-142">Virtueller Computer (Ressource)</span><span class="sxs-lookup"><span data-stu-id="2b3ac-142">Virtual machine (resource)</span></span>
            - <span data-ttu-id="2b3ac-143">Computeverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="2b3ac-143">Compute meter</span></span>
        - <span data-ttu-id="2b3ac-144">Virtuelles Netzwerk (Ressource)</span><span class="sxs-lookup"><span data-stu-id="2b3ac-144">Virtual network (resource)</span></span>
            - <span data-ttu-id="2b3ac-145">Keine Abrechnungsverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="2b3ac-145">No billing meter</span></span>

    - <span data-ttu-id="2b3ac-146">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="2b3ac-146">ResourceGroup 2</span></span>
        - <span data-ttu-id="2b3ac-147">Virtueller Computer (Ressource)</span><span class="sxs-lookup"><span data-stu-id="2b3ac-147">Virtual machine (resource)</span></span>
            - <span data-ttu-id="2b3ac-148">Computerverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="2b3ac-148">Computer meter</span></span>
        - <span data-ttu-id="2b3ac-149">Verwalteter SSD Premium-Datenträger (Ressource)</span><span class="sxs-lookup"><span data-stu-id="2b3ac-149">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="2b3ac-150">Verbrauchseinheit für Speicherkapazität</span><span class="sxs-lookup"><span data-stu-id="2b3ac-150">Storage capacity meter</span></span>
            - <span data-ttu-id="2b3ac-151">Verbrauchseinheit für Speichervorgänge</span><span class="sxs-lookup"><span data-stu-id="2b3ac-151">Storage operations meter</span></span>

- <span data-ttu-id="2b3ac-152">Abonnement B   -ResourceGroup 1       - Azure SQL (Ressource)           - DTU-Verbrauchseinheit       - VPN Gateway (Ressource)           - Verbrauchseinheit für VPN-Gateway</span><span class="sxs-lookup"><span data-stu-id="2b3ac-152">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="2b3ac-153">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="2b3ac-153">ResourceGroup 2</span></span>
        - <span data-ttu-id="2b3ac-154">Virtuelle Netzwerkschnittstelle (Ressource)</span><span class="sxs-lookup"><span data-stu-id="2b3ac-154">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="2b3ac-155">Keine Abrechnungsverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="2b3ac-155">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="2b3ac-156">Lesen der Rechnung</span><span class="sxs-lookup"><span data-stu-id="2b3ac-156">Read the invoice</span></span>

1. <span data-ttu-id="2b3ac-157">Die Rechnung steht spätestens am 8. jedes Monats zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-157">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="2b3ac-158">Partner haben 60 Tage Zeit, die Zahlung zu überweisen.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-158">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="2b3ac-159">Der Abrechnungszeitraum deckt einen bestimmten Kalendermonat ab, beispielsweise 01.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-159">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="2b3ac-160">Gebühren werden ohne Wertberichtigungen angezeigt (Betrag ohne Anrechnung von „vom Partner erworbene Gutschrift für verwaltete Dienste“).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-160">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="2b3ac-161">Weitere Abrechnungsdetails können Sie der Abstimmungsdatei zur Rechnung und der täglich ausgewerteten Nutzungsdatei entnehmen.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-161">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![Rechnung](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="2b3ac-163">Lesen der Rechnungs-/Abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="2b3ac-163">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="2b3ac-164">Jede Kombination von Azure-Plan und Verbrauchseinheit kann bis zu zwei Abrechnungszeilen in der Abstimmungsdatei aufweisen.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-164">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="2b3ac-165">Wenn die Verbrauchseinheit während des gesamten Kalendermonats zu Rabatten oder Gutschriften berechtigt – etwa die Rabatte in Schicht 1 oder das vom Partner erworbene Guthaben (PEC) für verwaltete Dienste – enthält die Abstimmungsdatei nur eine Abrechnungszeile.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-165">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="2b3ac-166">Die Spalte **PriceAdjusmentDescription** verweist auf den Rabatt oder das erworbene Guthaben.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-166">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="2b3ac-167">Wenn für eine bestimmte Verbrauchseinheit, die zu einem Rabatt oder PEC berechtigt, keine Ressourcen vorliegen, enthält die Abstimmungsdatei nur eine Abrechnungszeile, und der effektive Einzelpreis stimmt mit dem Endkundenpreis (bei dem es sich um den Einzelpreis handelt) überein.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-167">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="2b3ac-168">Wenn die Verbrauchseinheit oder eine beliebige Ressource, die diese Verbrauchseinheit ausgibt, während eines Teils des Monats für **Vom Partner erworbenes Guthaben für verwaltete Dienste** berechtigt war, enthält die Abstimmungsdatei zwei Abrechnungszeilen.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-168">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="2b3ac-169">Eine Zeile stellt die Tage dar, an denen eine Berechtigung der Verbrauchseinheit bestand, die andere die Tage, an denen diese Berechtigung nicht bestand.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-169">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="2b3ac-170">Lesen der täglichen Nutzungsdatei</span><span class="sxs-lookup"><span data-stu-id="2b3ac-170">Read the daily usage file</span></span>

- <span data-ttu-id="2b3ac-171">Verbrauchseinheiten von Abonnements im Rahmen eines Azure-Plans werden täglich bewertet und kumuliert.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-171">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="2b3ac-172">**Partner earned credit for services managed** wird auf täglicher Grundlage bestimmt und angewendet.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-172">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="2b3ac-173">Jede Verbrauchseinheit für Abonnements weist eine Zeile für jeden Tag des Monats auf, an dem ein Verbrauch angefallen ist.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-173">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="2b3ac-174">Bezogen auf das Beispiel unten:</span><span class="sxs-lookup"><span data-stu-id="2b3ac-174">In the example below:</span></span>

  - <span data-ttu-id="2b3ac-175">Die Verbrauchseinheit ist vom 01.07–3.07. für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-175">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="2b3ac-176">Die Verbrauchseinheit ist vom 04.07–07.07. nicht für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis stimmt nicht mit dem Endkundenpreis überein).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-176">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="2b3ac-177">Die Verbrauchseinheit ist vom 08.07–31.07. für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-177">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="2b3ac-179">Rechnung in Währung des Kunden</span><span class="sxs-lookup"><span data-stu-id="2b3ac-179">Invoice in customer currency</span></span> 

<span data-ttu-id="2b3ac-180">Im Rahmen eines Azure-Plans erbrachte Azure-Dienste haben Preise in USD und werden in der Landeswährung des Kunden abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-180">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="2b3ac-181">Wenn die Abrechnungswährung nicht USD ist, wird der zugrunde gelegte Wechselkurs auf der letzten Seite der Rechnung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-181">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="2b3ac-182">Wechselkurse werden monatlich bestimmt und auf die folgende Rechnung angewendet.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-182">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="2b3ac-183">Eine vollständige Liste der Landeswährungen finden Sie in der [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354) (Matrix für die Länderverfügbarkeit neuer E-Commerce-Angebote und Kundenwährungen).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-183">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span> 

<span data-ttu-id="2b3ac-184">Microsoft nutzt [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) zum Ermitteln des Wechselkurses, der für die Konvertierung aus der Preiswährung in die Abrechnungswährung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-184">Microsoft will use [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="2b3ac-185">Die Wechselkurse werden aktualisiert und stehen am Tag vor dem Ersten des Monats zur Verfügung, für den sie gelten.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-185">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="2b3ac-186">**Beispiel**:  Nutzungsgebühren für den Dienstzeitraum vom 1. August–31. August unter Verwendung des am 31. Juli veröffentlichten Wechselkurses.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-186">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="2b3ac-187">Diese Gebühren werden auf der September-Rechnung aufgeführt, und der Wechselkurs ist auf der letzten Seite der Rechnung vermerkt.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-187">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

 
## <a name="azure-reservations"></a><span data-ttu-id="2b3ac-188">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="2b3ac-188">Azure reservations</span></span> 

<span data-ttu-id="2b3ac-189">Wenn Sie [Azure-Reservierungen](https://docs.microsoft.com/partner-center/azure-reservations) im Rahmen eines Azure-Plans erwerben, ist im Partner Center anfänglich nur die Auswahl der einmaligen Abrechnung möglich.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-189">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="2b3ac-190">Die monatliche Abrechnung steht im Azure-Portal zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-190">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="2b3ac-191">Die monatliche Abrechnung ist im Partner Center zu einem späteren Termin verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-191">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-spending"></a><span data-ttu-id="2b3ac-192">Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="2b3ac-192">Azure spending</span></span> 

<span data-ttu-id="2b3ac-193">Die bestehende Azure-Kaufumgebung wird aktualisiert, um die neue Azure-Planabrechnung im Partner Center zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="2b3ac-194">Dadurch wird Partnern Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="2b3ac-194">This enables partners to:</span></span>

- <span data-ttu-id="2b3ac-195">Anzeigen, Verwalten und Empfangen von Benachrichtigungen für Budgets, die auf Kundenebene festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="2b3ac-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="2b3ac-196">Anzeigen der geschätzten Gesamtausgaben für einen Azure-Plan (aufgeschlüsselt nach Ressourcen und Verbrauchseinheitswert)</span><span class="sxs-lookup"><span data-stu-id="2b3ac-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="2b3ac-197">Da die Abrechnungsmodell für Azure-Dienste unter einem Azure-Plan nachträglich nach Verbrauch berechnet wird, können Partner ein monatliches Budget festlegen und den Prozentsatz der Nutzung nachverfolgen, um zu vermeide, dass die Rechnung höher als erwartet ausfällt.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="2b3ac-198">Ein Budget kann auf einen Kunden oder auf mehrere Kunden zugleich angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="2b3ac-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure-Ausgaben](images/azure/azurespend.png)

<span data-ttu-id="2b3ac-200">**Weitere Informationen**</span><span class="sxs-lookup"><span data-stu-id="2b3ac-200">**For more information**</span></span>

-  <span data-ttu-id="2b3ac-201">Wie das vom Partner erworbene Guthaben (PEC) berechnet wird, finden Sie in der Preisliste, die auf dem Partner Center-[Dashboard](https://partner.microsoft.com/en-us/dashboard/) verfügbar ist (Anmeldung erforderlich).</span><span class="sxs-lookup"><span data-stu-id="2b3ac-201">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/) (sign in required).</span></span> 
   
-  [<span data-ttu-id="2b3ac-202">Erwerb des Azure-Plans</span><span class="sxs-lookup"><span data-stu-id="2b3ac-202">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="2b3ac-203">Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP </span><span class="sxs-lookup"><span data-stu-id="2b3ac-203">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
