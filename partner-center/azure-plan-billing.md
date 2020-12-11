---
title: 'Azure-Plan: Abrechnung – Rechnungs- und Kontenabstimmungsdateien'
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie auf die Struktur der Rechnungs-/Abstimmungsdatei im Zusammenhang mit der Abrechnung für den Azure-Plan zugreifen und sie verstehen können.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 1dc683c194de158dc7a4dac541b37631f3be1f1e
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534691"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="657e2-103">Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="657e2-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="657e2-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="657e2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="657e2-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="657e2-105">Admin agent</span></span>
- <span data-ttu-id="657e2-106">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="657e2-106">Billing admin</span></span>
- <span data-ttu-id="657e2-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="657e2-107">Global admin</span></span>

<span data-ttu-id="657e2-108">In diesem Artikel wird erläutert, wie Sie auf die Struktur der Rechnungs-/Abstimmungsdatei im Zusammenhang mit der Abrechnung für den Azure-Plan zugreifen und sie verstehen können.</span><span class="sxs-lookup"><span data-stu-id="657e2-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="657e2-109">Abrechnungen im Rahmen eines Azure-Plans bieten ein vereinfachtes Abrechnungsverfahren, das ein einheitliches Abrechnungsdatum und einen Abrechnungszeitraum auf der Grundlage von Kalendermonaten verwendet.</span><span class="sxs-lookup"><span data-stu-id="657e2-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="657e2-110">Zusammenfassung der Abrechnungsgrundlagen</span><span class="sxs-lookup"><span data-stu-id="657e2-110">Summary of billing essentials</span></span>

- <span data-ttu-id="657e2-111">**Rechnungsdatum**: Die Rechnungs- und Abstimmungsdatei steht auf dem Partner Center-Dashboard bzw. über die -API am 8. des Monats zur Verfügung (Mitternacht UTC).</span><span class="sxs-lookup"><span data-stu-id="657e2-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="657e2-112">**Abrechnungszeitraum der Rechnung**: Der Abrechnungszeitraum der Rechnung ist am Kalendermonat ausgerichtet, z.B. 01.10.–31.10., 01.11.–30.11.</span><span class="sxs-lookup"><span data-stu-id="657e2-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="657e2-113">**Belastung von Dienstzeiträumen**: Die Gebühren richten sich nach dem Kalendermonat.</span><span class="sxs-lookup"><span data-stu-id="657e2-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="657e2-114">Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="657e2-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="657e2-115">Die Rechnung des nächsten Monats, die am 08.12. generiert wird, enthält alle Gebühren für den Dienstzeitraum vom 01.11.–31.11.</span><span class="sxs-lookup"><span data-stu-id="657e2-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="657e2-116">**Fälligkeit der Rechnung**: 60 Tage netto.</span><span class="sxs-lookup"><span data-stu-id="657e2-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="657e2-117">**Rechnungswährung** : Partner werden weiterhin in der offiziellen Landeswährung des Kunden abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="657e2-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="657e2-118">Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.</span><span class="sxs-lookup"><span data-stu-id="657e2-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="657e2-119">**Partnerincentives**: 45 Tage nach dem Ende des Rechnungsmonats bezahlt.</span><span class="sxs-lookup"><span data-stu-id="657e2-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="657e2-120">Zugriff auf Ihre Rechnungen und Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="657e2-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="657e2-121">Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist.</span><span class="sxs-lookup"><span data-stu-id="657e2-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="657e2-122">So greifen Sie auf die Rechnungs- und Abstimmungsdatei zu:</span><span class="sxs-lookup"><span data-stu-id="657e2-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="657e2-123">Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="657e2-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="657e2-124">Wählen Sie im Menü des Partner Center **Abrechnung** aus.</span><span class="sxs-lookup"><span data-stu-id="657e2-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="657e2-125">Wählen Sie die Registerkarte für **laufende** und **einmalige** Gebühren sowie die für Sie relevante Währung aus.</span><span class="sxs-lookup"><span data-stu-id="657e2-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Abrechnung":::

4. <span data-ttu-id="657e2-127">Wählen Sie **Rechnung** oder **Abstimmungsdatei** aus.</span><span class="sxs-lookup"><span data-stu-id="657e2-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="657e2-128">Zum Anzeigen früherer Rechnungen und Abstimmungsdateien erweitern Sie die Zeile „Abrechnungsverlauf“ unten.</span><span class="sxs-lookup"><span data-stu-id="657e2-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="657e2-129">Grundlegendes zu Verwendungsdaten</span><span class="sxs-lookup"><span data-stu-id="657e2-129">Understanding usage data</span></span> 

1. <span data-ttu-id="657e2-130">Der Azure-Plan ist der Stammcontainer oder der Container der obersten Ebene für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="657e2-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="657e2-131">Alle Verwendungsdaten sind an einen einzelnen Azure-Plan gebunden.</span><span class="sxs-lookup"><span data-stu-id="657e2-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="657e2-132">Ein Plan kann ein oder mehrere Azure-Abonnements enthalten.</span><span class="sxs-lookup"><span data-stu-id="657e2-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="657e2-133">Dies sind Container, die für die Ressourcenverwaltung und -bereitstellung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="657e2-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="657e2-134">Innerhalb eines Abonnements werden Ressourcengruppen zu Gruppenressourcen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="657e2-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="657e2-135">Jede Ressource wird in einer Ressourcengruppe bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="657e2-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="657e2-136">Beispiele für Ressourcen sind virtuelle Computer und Speicherkonten.</span><span class="sxs-lookup"><span data-stu-id="657e2-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="657e2-137">Ressourcen geben Verbrauchszähler aus: Verbrauchszähler sind Verbrauchsmessungen einer Ressource, und eine Ressource kann Verwendungsdaten für verschiedene Verbrauchszähler ausgeben.</span><span class="sxs-lookup"><span data-stu-id="657e2-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="657e2-138">Verbrauchszähler werden durch „ProductId“-, „SKUId“- und „AvailabilityId“-Werte identifiziert.</span><span class="sxs-lookup"><span data-stu-id="657e2-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="657e2-139">Hierarchie von Abonnementressourcengruppen und -messungen</span><span class="sxs-lookup"><span data-stu-id="657e2-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="657e2-140">**Azure-Konto (Mandant)**</span><span class="sxs-lookup"><span data-stu-id="657e2-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="657e2-141">Abonnement A</span><span class="sxs-lookup"><span data-stu-id="657e2-141">Subscription A</span></span>
    - <span data-ttu-id="657e2-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="657e2-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="657e2-143">Virtueller Computer (Ressource)</span><span class="sxs-lookup"><span data-stu-id="657e2-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="657e2-144">Computeverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="657e2-144">Compute meter</span></span>
        - <span data-ttu-id="657e2-145">Virtuelles Netzwerk (Ressource)</span><span class="sxs-lookup"><span data-stu-id="657e2-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="657e2-146">Keine Abrechnungsverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="657e2-146">No billing meter</span></span>

    - <span data-ttu-id="657e2-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="657e2-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="657e2-148">Virtueller Computer (Ressource)</span><span class="sxs-lookup"><span data-stu-id="657e2-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="657e2-149">Computerverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="657e2-149">Computer meter</span></span>
        - <span data-ttu-id="657e2-150">Verwalteter SSD Premium-Datenträger (Ressource)</span><span class="sxs-lookup"><span data-stu-id="657e2-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="657e2-151">Verbrauchseinheit für Speicherkapazität</span><span class="sxs-lookup"><span data-stu-id="657e2-151">Storage capacity meter</span></span>
            - <span data-ttu-id="657e2-152">Verbrauchseinheit für Speichervorgänge</span><span class="sxs-lookup"><span data-stu-id="657e2-152">Storage operations meter</span></span>

- <span data-ttu-id="657e2-153">Abonnement B   -ResourceGroup 1       - Azure SQL (Ressource)           - DTU-Verbrauchseinheit       - VPN Gateway (Ressource)           - Verbrauchseinheit für VPN-Gateway</span><span class="sxs-lookup"><span data-stu-id="657e2-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="657e2-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="657e2-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="657e2-155">Virtuelle Netzwerkschnittstelle (Ressource)</span><span class="sxs-lookup"><span data-stu-id="657e2-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="657e2-156">Keine Abrechnungsverbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="657e2-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="657e2-157">Lesen der Rechnung</span><span class="sxs-lookup"><span data-stu-id="657e2-157">Read the invoice</span></span>

1. <span data-ttu-id="657e2-158">Die Rechnung steht spätestens am 8. jedes Monats zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="657e2-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="657e2-159">Partner haben 60 Tage Zeit, die Zahlung zu überweisen.</span><span class="sxs-lookup"><span data-stu-id="657e2-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="657e2-160">Der Abrechnungszeitraum deckt einen bestimmten Kalendermonat ab, beispielsweise 01.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="657e2-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="657e2-161">Gebühren werden ohne Wertberichtigungen angezeigt (Betrag ohne Anrechnung von „vom Partner erworbene Gutschrift für verwaltete Dienste“).</span><span class="sxs-lookup"><span data-stu-id="657e2-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="657e2-162">Weitere Abrechnungsdetails können Sie der Abstimmungsdatei zur Rechnung und der täglich ausgewerteten Nutzungsdatei entnehmen.</span><span class="sxs-lookup"><span data-stu-id="657e2-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Rechnung":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="657e2-164">Lesen der Rechnungs-/Abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="657e2-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="657e2-165">Jede Kombination von Azure-Plan und Verbrauchseinheit kann bis zu zwei Abrechnungszeilen in der Abstimmungsdatei aufweisen.</span><span class="sxs-lookup"><span data-stu-id="657e2-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="657e2-166">Wenn die Verbrauchseinheit während des gesamten Kalendermonats zu Rabatten oder Gutschriften berechtigt – etwa die Rabatte in Schicht 1 oder das vom Partner erworbene Guthaben (PEC) für verwaltete Dienste – enthält die Abstimmungsdatei nur eine Abrechnungszeile.</span><span class="sxs-lookup"><span data-stu-id="657e2-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="657e2-167">Die Spalte **PriceAdjusmentDescription** verweist auf den Rabatt oder das erworbene Guthaben.</span><span class="sxs-lookup"><span data-stu-id="657e2-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="657e2-168">Wenn für eine bestimmte Verbrauchseinheit, die zu einem Rabatt oder PEC berechtigt, keine Ressourcen vorliegen, enthält die Abstimmungsdatei nur eine Abrechnungszeile, und der effektive Einzelpreis stimmt mit dem Endkundenpreis (bei dem es sich um den Einzelpreis handelt) überein.</span><span class="sxs-lookup"><span data-stu-id="657e2-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="657e2-169">Wenn die Verbrauchseinheit oder eine beliebige Ressource, die diese Verbrauchseinheit ausgibt, während eines Teils des Monats für **Vom Partner erworbenes Guthaben für verwaltete Dienste** berechtigt war, enthält die Abstimmungsdatei zwei Abrechnungszeilen.</span><span class="sxs-lookup"><span data-stu-id="657e2-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="657e2-170">Eine Zeile stellt die Tage dar, an denen eine Berechtigung der Verbrauchseinheit bestand, die andere die Tage, an denen diese Berechtigung nicht bestand.</span><span class="sxs-lookup"><span data-stu-id="657e2-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="657e2-171">Lesen der täglichen Nutzungsdatei</span><span class="sxs-lookup"><span data-stu-id="657e2-171">Read the daily usage file</span></span>

- <span data-ttu-id="657e2-172">Verbrauchseinheiten von Abonnements im Rahmen eines Azure-Plans werden täglich bewertet und kumuliert.</span><span class="sxs-lookup"><span data-stu-id="657e2-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="657e2-173">**Partner earned credit for services managed** wird auf täglicher Grundlage bestimmt und angewendet.</span><span class="sxs-lookup"><span data-stu-id="657e2-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="657e2-174">Jede Verbrauchseinheit für Abonnements weist eine Zeile für jeden Tag des Monats auf, an dem ein Verbrauch angefallen ist.</span><span class="sxs-lookup"><span data-stu-id="657e2-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="657e2-175">Bezogen auf das Beispiel unten:</span><span class="sxs-lookup"><span data-stu-id="657e2-175">In the example below:</span></span>

  - <span data-ttu-id="657e2-176">Die Verbrauchseinheit ist vom 01.07–3.07. für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift).</span><span class="sxs-lookup"><span data-stu-id="657e2-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="657e2-177">Die Verbrauchseinheit ist vom 04.07–07.07. nicht für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis stimmt nicht mit dem Endkundenpreis überein).</span><span class="sxs-lookup"><span data-stu-id="657e2-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="657e2-178">Die Verbrauchseinheit ist vom 08.07–31.07. für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift).</span><span class="sxs-lookup"><span data-stu-id="657e2-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="657e2-180">Rechnung in Währung des Kunden</span><span class="sxs-lookup"><span data-stu-id="657e2-180">Invoice in customer currency</span></span>

<span data-ttu-id="657e2-181">Im Rahmen eines Azure-Plans erbrachte Azure-Dienste haben Preise in USD und werden in der Landeswährung des Kunden abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="657e2-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="657e2-182">Wenn die Abrechnungswährung nicht USD ist, wird der zugrunde gelegte Wechselkurs auf der letzten Seite der Rechnung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="657e2-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="657e2-183">Wechselkurse werden monatlich bestimmt und auf die folgende Rechnung angewendet.</span><span class="sxs-lookup"><span data-stu-id="657e2-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="657e2-184">Eine vollständige Liste der Landeswährungen finden Sie in der [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354) (Matrix für die Länderverfügbarkeit neuer E-Commerce-Angebote und Kundenwährungen).</span><span class="sxs-lookup"><span data-stu-id="657e2-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="657e2-185">Microsoft nutzt Thompson Reuters zum Ermitteln des Wechselkurses, der für die Konvertierung aus der Preiswährung in die Abrechnungswährung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="657e2-185">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="657e2-186">Die Wechselkurse werden aktualisiert und stehen am Tag vor dem Ersten des Monats zur Verfügung, für den sie gelten.</span><span class="sxs-lookup"><span data-stu-id="657e2-186">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="657e2-187">**Beispiel**:  Nutzungsgebühren für den Dienstzeitraum vom 1. August–31. August unter Verwendung des am 31. Juli veröffentlichten Wechselkurses.</span><span class="sxs-lookup"><span data-stu-id="657e2-187">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="657e2-188">Diese Gebühren werden auf der September-Rechnung aufgeführt, und der Wechselkurs ist auf der letzten Seite der Rechnung vermerkt.</span><span class="sxs-lookup"><span data-stu-id="657e2-188">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="657e2-189">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="657e2-189">Azure reservations</span></span>


<span data-ttu-id="657e2-190">Wenn Sie [Azure-Reservierungen](azure-reservations.md) über einen Azure-Plan erwerben, können Sie eine einmalige oder monatliche Abrechnung wählen.</span><span class="sxs-lookup"><span data-stu-id="657e2-190">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="657e2-191">Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="657e2-191">Azure spending</span></span>

<span data-ttu-id="657e2-192">Die bestehende Azure-Kaufumgebung wird aktualisiert, um die neue Azure-Planabrechnung im Partner Center zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="657e2-192">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="657e2-193">Dadurch wird Partnern Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="657e2-193">This enables partners to:</span></span>

- <span data-ttu-id="657e2-194">Anzeigen, Verwalten und Empfangen von Benachrichtigungen für Budgets, die auf Kundenebene festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="657e2-194">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="657e2-195">Anzeigen der geschätzten Gesamtausgaben für einen Azure-Plan (aufgeschlüsselt nach Ressourcen und Verbrauchseinheitswert)</span><span class="sxs-lookup"><span data-stu-id="657e2-195">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="657e2-196">Da die Abrechnungsmodell für Azure-Dienste unter einem Azure-Plan nachträglich nach Verbrauch berechnet wird, können Partner ein monatliches Budget festlegen und den Prozentsatz der Nutzung nachverfolgen, um zu vermeide, dass die Rechnung höher als erwartet ausfällt.</span><span class="sxs-lookup"><span data-stu-id="657e2-196">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="657e2-197">Ein Budget kann auf einen Kunden oder auf mehrere Kunden zugleich angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="657e2-197">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-Ausgaben":::

## <a name="next-steps"></a><span data-ttu-id="657e2-199">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="657e2-199">Next steps</span></span>

- <span data-ttu-id="657e2-200">Informieren Sie sich, wie von Partnern erworbene Guthaben (Partner Earned Credit, PEC) berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="657e2-200">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="657e2-201">Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/) an, und suchen Sie die verfügbare Preisliste.</span><span class="sxs-lookup"><span data-stu-id="657e2-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="657e2-202">Erfahren Sie mehr über den [Erwerb des Azure-Plans](purchase-azure-plan.md).</span><span class="sxs-lookup"><span data-stu-id="657e2-202">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="657e2-203">Sehen Sie sich die [Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP](azure-plan-price-list.md) an.</span><span class="sxs-lookup"><span data-stu-id="657e2-203">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
