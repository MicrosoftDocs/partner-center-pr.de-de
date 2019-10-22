---
title: 'Azure-Plan: Abrechnung | Partner Center'
ms.topic: article
ms.date: 10/04/2019
description: Beschreibt die Dateistruktur für Rechnungen und Abstimmungen
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171302"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="b31ed-103">Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b31ed-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="b31ed-104">Abrechnungen im Rahmen eines Azure-Plans bieten ein vereinfachtes Abrechnungsverfahren, das ein einheitliches Abrechnungsdatum und einen Abrechnungszeitraum auf der Grundlage von Kalendermonaten verwendet.</span><span class="sxs-lookup"><span data-stu-id="b31ed-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="b31ed-105">Informationen zur Abrechnungsplattform finden Sie unter [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (Partner Center Modern Commerce – Betriebshandbuch).</span><span class="sxs-lookup"><span data-stu-id="b31ed-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="b31ed-106">Zusammenfassung der Abrechnungsgrundlagen</span><span class="sxs-lookup"><span data-stu-id="b31ed-106">Summary of billing essentials</span></span>

- <span data-ttu-id="b31ed-107">**Rechnungsdatum**: Die Rechnungs- und Abstimmungsdatei steht auf dem Partner Center-Dashboard bzw. über die -API am 8. des Monats zur Verfügung (Mitternacht UTC).</span><span class="sxs-lookup"><span data-stu-id="b31ed-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="b31ed-108">**Abrechnungszeitraum der Rechnung**: Der Abrechnungszeitraum der Rechnung ist am Kalendermonat ausgerichtet, z.B. 01.10.–31.10., 01.11.–30.11.</span><span class="sxs-lookup"><span data-stu-id="b31ed-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="b31ed-109">**Belastung von Dienstzeiträumen**: Die Gebühren richten sich nach dem Kalendermonat.</span><span class="sxs-lookup"><span data-stu-id="b31ed-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="b31ed-110">Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="b31ed-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="b31ed-111">Die Rechnung des nächsten Monats, die am 08.12. generiert wird, enthält alle Gebühren für den Dienstzeitraum vom 01.11.–30.11.</span><span class="sxs-lookup"><span data-stu-id="b31ed-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="b31ed-112">**Fälligkeit der Rechnung**: 60 Tage netto.</span><span class="sxs-lookup"><span data-stu-id="b31ed-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="b31ed-113">**Rechnungswährung** : Partner werden weiterhin in der offiziellen Landeswährung des Kunden abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="b31ed-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="b31ed-114">Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.</span><span class="sxs-lookup"><span data-stu-id="b31ed-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="b31ed-115">**Partnerincentives**: 45 Tage nach dem Ende des Rechnungsmonats bezahlt.</span><span class="sxs-lookup"><span data-stu-id="b31ed-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="b31ed-116">Zugriff auf Ihre Rechnungen und Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="b31ed-116">Access your invoices and recon files</span></span>

<span data-ttu-id="b31ed-117">Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist.</span><span class="sxs-lookup"><span data-stu-id="b31ed-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="b31ed-118">**Zugriff auf die Rechnung und Abstimmungsdatei**</span><span class="sxs-lookup"><span data-stu-id="b31ed-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="b31ed-119">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="b31ed-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="b31ed-120">Wählen Sie im Menü des Partner Center **Abrechnung** aus.</span><span class="sxs-lookup"><span data-stu-id="b31ed-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="b31ed-121">Wählen Sie die Registerkarte für die **kalenderbasierte** Abrechnung und die Sie interessierende Währung aus.</span><span class="sxs-lookup"><span data-stu-id="b31ed-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![Abrechnung](images/azure/billing1.png)

4. <span data-ttu-id="b31ed-123">Wählen Sie **Rechnung und Abstimmungsdatei** aus.</span><span class="sxs-lookup"><span data-stu-id="b31ed-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="b31ed-124">Zum Anzeigen früherer Rechnungen und Abstimmungsdateien erweitern Sie die Zeile „Abrechnungsverlauf“ unten.</span><span class="sxs-lookup"><span data-stu-id="b31ed-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="b31ed-125">Lesen der Rechnung</span><span class="sxs-lookup"><span data-stu-id="b31ed-125">Read the invoice</span></span>

1. <span data-ttu-id="b31ed-126">Die Rechnung steht spätestens am 8. jedes Monats zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="b31ed-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="b31ed-127">Partner haben 60 Tage Zeit, die Zahlung zu überweisen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="b31ed-128">Der Abrechnungszeitraum deckt einen bestimmten Kalendermonat ab, beispielsweise 01.10–31.10.</span><span class="sxs-lookup"><span data-stu-id="b31ed-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="b31ed-129">Gebühren werden ohne Wertberichtigungen angezeigt (Betrag ohne Anrechnung von „Partner earned credit for services managed“).</span><span class="sxs-lookup"><span data-stu-id="b31ed-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="b31ed-130">Weitere Abrechnungsdetails können Sie der Abstimmungsdatei zur Rechnung und der täglich ausgewerteten Nutzungsdatei entnehmen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![Rechnung](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="b31ed-132">Lesen der Abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="b31ed-132">Read the recon file</span></span>

1. <span data-ttu-id="b31ed-133">Jede Verbrauchseinheit von Azure-Abonnements kann bis zu zwei Abrechnungszeilen in der Abstimmungsdatei aufweisen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="b31ed-134">Wenn die Verbrauchseinheit während des gesamten Kalendermonats zu Rabatten oder Gutschriften berechtigt (etwa die Rabatte in Schicht 1 oder die „Partner earned credit for managed services“), enthält die Abstimmungsdatei nur eine Abrechnungszeile.</span><span class="sxs-lookup"><span data-stu-id="b31ed-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="b31ed-135">Die Spalte **PriceAdjusmentDescription** weist den Rabatt oder die erworbene Gutschrift aus; der effektive Preis pro Einheit ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift oder anderer Rabatte.</span><span class="sxs-lookup"><span data-stu-id="b31ed-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="b31ed-136">Wenn die Verbrauchseinheit während des gesamten Kalendermonats nicht zu Gutschriften für die „Partner earned credit for managed services“ berechtigt war, enthält die Abstimmungsdatei nur eine Abrechnungszeile, und der effektive Einzelpreis stimmt mit dem Endkundenpreis (bei dem es sich um den Einzelpreis handelt) überein.</span><span class="sxs-lookup"><span data-stu-id="b31ed-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="b31ed-137">Wenn die Verbrauchseinheit während eines Teils des Monats für **Partner earned credit for services managed** berechtigt war, enthält die Abstimmungsdatei zwei Abrechnungszeilen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="b31ed-138">Eine Zeile stellt die Tage dar, an denen eine Berechtigung der Verbrauchseinheit bestand, die andere die Tage, an denen diese Berechtigung nicht bestand.</span><span class="sxs-lookup"><span data-stu-id="b31ed-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="b31ed-139">Lesen der täglichen Nutzungsdatei</span><span class="sxs-lookup"><span data-stu-id="b31ed-139">Read the daily usage file</span></span>

- <span data-ttu-id="b31ed-140">Verbrauchseinheiten von Abonnements im Rahmen eines Azure-Plans werden täglich bewertet und kumuliert.</span><span class="sxs-lookup"><span data-stu-id="b31ed-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="b31ed-141">**Partner earned credit for services managed** wird auf täglicher Grundlage bestimmt und angewendet.</span><span class="sxs-lookup"><span data-stu-id="b31ed-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="b31ed-142">Jede Verbrauchseinheit für Abonnements weist eine Zeile für jeden Tag des Monats auf, an dem ein Verbrauch angefallen ist.</span><span class="sxs-lookup"><span data-stu-id="b31ed-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="b31ed-143">Bezogen auf das Beispiel unten:</span><span class="sxs-lookup"><span data-stu-id="b31ed-143">In the example below:</span></span>

  - <span data-ttu-id="b31ed-144">Die Verbrauchseinheit ist vom 01.07–03.07. für **Partner earned credit for services managed** qualifiziert (beachten Sie, dass der effektive Einzelpreis sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift ergibt).</span><span class="sxs-lookup"><span data-stu-id="b31ed-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="b31ed-145">Die Verbrauchseinheit ist vom 04.07–07.07. nicht für **Partner earned credit for services managed** qualifiziert (beachten Sie, dass der effektive Einzelpreis mit dem Endkundenpreis übereinstimmt).</span><span class="sxs-lookup"><span data-stu-id="b31ed-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="b31ed-146">Die Verbrauchseinheit ist vom 08.07–31.07. für **Partner earned credit for services managed** qualifiziert (beachten Sie, dass der effektive Einzelpreis sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift ergibt).</span><span class="sxs-lookup"><span data-stu-id="b31ed-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="b31ed-148">Rechnung in Währung des Kunden</span><span class="sxs-lookup"><span data-stu-id="b31ed-148">Invoice in customer currency</span></span> 

<span data-ttu-id="b31ed-149">Im Rahmen eines Azure-Plans erbrachte Azure-Dienste haben Preise in USD und werden in der Landeswährung des Kunden abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="b31ed-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="b31ed-150">Wenn die Abrechnungswährung nicht USD ist, wird der zugrunde gelegte Wechselkurs auf der letzten Seite der Rechnung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b31ed-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="b31ed-151">Wechselkurse werden monatlich bestimmt und auf die folgende Rechnung angewendet.</span><span class="sxs-lookup"><span data-stu-id="b31ed-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="b31ed-152">Eine vollständige Liste der Landeswährungen finden Sie in der [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V) (Matrix für die Länderverfügbarkeit neuer E-Commerce-Angebote und Kundenwährungen).</span><span class="sxs-lookup"><span data-stu-id="b31ed-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="b31ed-153">Microsoft nutzt [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) zum Ermitteln des Wechselkurses, der für die Konvertierung aus der Preiswährung in die Rechnungswährung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b31ed-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="b31ed-154">Der Wechselkurs wird aktualisiert und steht am Tag vor dem Ersten des Monats zur Verfügung, für den er gilt.</span><span class="sxs-lookup"><span data-stu-id="b31ed-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="b31ed-155">**Beispiel**:  Nutzungsgebühren für den Dienstzeitraum vom 1. August–31. August unter Verwendung des am 1. August veröffentlichten Wechselkurses.</span><span class="sxs-lookup"><span data-stu-id="b31ed-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="b31ed-156">Diese Gebühren werden auf der September-Rechnung aufgeführt, und der Wechselkurs ist auf der letzten Seite der Rechnung vermerkt.</span><span class="sxs-lookup"><span data-stu-id="b31ed-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="b31ed-157">Benutzer von Partnermandanten sehen auch weiterhin rollenspezifische Informationen zu allen Kunden und Bestellungen, unabhängig von der Rechnungswährung.</span><span class="sxs-lookup"><span data-stu-id="b31ed-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="b31ed-158">Darüber hinaus kann der Benutzer alle Rechnungen in allen Währungen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="b31ed-159">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="b31ed-159">Azure reservations</span></span> 

<span data-ttu-id="b31ed-160">Wenn Sie [Azure-Reservierungen](https://docs.microsoft.com/partner-center/azure-reservations) im Rahmen eines Azure-Plans erwerben, ist im Partner Center anfänglich nur die Auswahl der einmaligen Abrechnung möglich.</span><span class="sxs-lookup"><span data-stu-id="b31ed-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="b31ed-161">Die monatliche Abrechnung steht im Azure-Portal zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="b31ed-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="b31ed-162">Die monatliche Abrechnung ist im Partner Center zu einem späteren Termin verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b31ed-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="b31ed-163">Azure-Kostenmanagement</span><span class="sxs-lookup"><span data-stu-id="b31ed-163">Azure cost management</span></span> 

<span data-ttu-id="b31ed-164">Mithilfe der Azure-Tools für Kostenmanagement können Organisationen Kosten überall in Microsoft Azure visualisieren, verwalten und optimieren.</span><span class="sxs-lookup"><span data-stu-id="b31ed-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="b31ed-165">Diese Funktion soll im Azure-Portal verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="b31ed-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="b31ed-166">Partner verfügen über eine Always-On-Lösung mit geringer Latenz, die folgende Features unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b31ed-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="b31ed-167">Umfangreichere Analyse- und Budgetwarnungen</span><span class="sxs-lookup"><span data-stu-id="b31ed-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="b31ed-168">APIs und Power BI-Connectors</span><span class="sxs-lookup"><span data-stu-id="b31ed-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="b31ed-169">Ansicht für mehrere Kunden</span><span class="sxs-lookup"><span data-stu-id="b31ed-169">Multi-customer view</span></span> 
- <span data-ttu-id="b31ed-170">Kostenlose Verwaltung von Azure-Kosten</span><span class="sxs-lookup"><span data-stu-id="b31ed-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="b31ed-171">Erweiterung von Rollen/Benutzern</span><span class="sxs-lookup"><span data-stu-id="b31ed-171">Expansion of roles/users</span></span> 

<span data-ttu-id="b31ed-172">Weitere Informationen zu diesem Feature, das für Enterprise-Verträge seit Februar 2019 verfügbar ist, finden Sie unter [Azure-Kostenmanagement](https://azure.microsoft.com/services/cost-management).</span><span class="sxs-lookup"><span data-stu-id="b31ed-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="b31ed-173">Es steht nur für Azure-Dienste zur Verfügung, die im Rahmen dieser neuen Azure-E-Commerce-Benutzeroberfläche in CSP erworben wurden.</span><span class="sxs-lookup"><span data-stu-id="b31ed-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="b31ed-174">Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="b31ed-174">Azure spending</span></span> 

<span data-ttu-id="b31ed-175">Ein Azure-Ausgabentool soll im Partner Center für die neue E-Commerce-Benutzeroberfläche in CSP zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="b31ed-176">Wenn es angewendet wird, können Partner mit dieser Funktion Folgendes anzeigen:</span><span class="sxs-lookup"><span data-stu-id="b31ed-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="b31ed-177">Das Gesamtbudget für einen Kunden</span><span class="sxs-lookup"><span data-stu-id="b31ed-177">Total budget on a customer</span></span> 
- <span data-ttu-id="b31ed-178">Geschätzte Gesamtausgaben für einen vorhandenen Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="b31ed-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="b31ed-179">Prozentsatz der Nutzung durch den Kunden in jedem Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="b31ed-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="b31ed-180">Da das Abrechnungsmodell für Azure-Dienste im Rahmen eines Azure-Plans die Nutzung nach Vorkasse vorsieht, können Partner zum Vermeiden einer höher als erwarteten Rechnung ein monatliches Budget zuweisen und den Prozentsatz seiner Nutzung nachverfolgen.</span><span class="sxs-lookup"><span data-stu-id="b31ed-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="b31ed-181">Ein Budget kann auf einen Kunden oder auf mehrere Kunden zugleich angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="b31ed-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure-Ausgaben](images/azure/azurespend.png)

<span data-ttu-id="b31ed-183">**Weitere Informationen**</span><span class="sxs-lookup"><span data-stu-id="b31ed-183">**For more information**</span></span>

-  <span data-ttu-id="b31ed-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard (Art der Berechnung der vom Partner erworbenen Gutschriften (PEC) und ihre Position in der Preisliste, die auf dem Partner Center-Dashboard verfügbar ist).</span><span class="sxs-lookup"><span data-stu-id="b31ed-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="b31ed-185">Erwerb des Azure-Plans</span><span class="sxs-lookup"><span data-stu-id="b31ed-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="b31ed-186">Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP </span><span class="sxs-lookup"><span data-stu-id="b31ed-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
