---
title: Auswirkungen von Steuer Richtlinien auf die Auszahlung der Azure Marketplace
description: Erfahren Sie, wie sich Steuer Richtlinien auf die Auszahlung der Azure Marketplace auswirken.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768821"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="d94b4-103">Auswirkungen von Steuer Richtlinien auf die Auszahlung der Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d94b4-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="d94b4-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="d94b4-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="d94b4-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="d94b4-105">Global admin</span></span>
-    <span data-ttu-id="d94b4-106">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="d94b4-106">User management admin</span></span>
-    <span data-ttu-id="d94b4-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="d94b4-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="d94b4-108">Einführung</span><span class="sxs-lookup"><span data-stu-id="d94b4-108">Introduction</span></span>

<span data-ttu-id="d94b4-109">Der kommerzielle Marketplace von Microsoft bietet globale Reichweite.</span><span class="sxs-lookup"><span data-stu-id="d94b4-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="d94b4-110">Transaktionen werden grenzübergreifend durchlaufen, und abhängig davon, wo sich der ISV und der Kunde befinden, können die Auswirkungen auf die Steuereffekte variieren.</span><span class="sxs-lookup"><span data-stu-id="d94b4-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="d94b4-111">Microsoft AppSource und Azure Marketplace die Partner Center-Steuer Profilinformationen verwenden, um das ISV-Land zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="d94b4-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="d94b4-112">Um das Land des Kunden zu ermitteln, verwenden Sie entweder die Abrechnungsinformationen des Kunden, oder wenn sich der Kunde in der EU befindet, verwenden wir zwei verschiedene Informationen.</span><span class="sxs-lookup"><span data-stu-id="d94b4-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="d94b4-113">Um die folgenden Szenarien besser zu verstehen, sehen Sie sich die Tabelle " [Tax Details](tax-details-marketplace.md) " an, die anzeigt, ob Microsoft Steuern im Auftrag des Verlegers erfasst und bezahlt oder ob diese Verantwortung zum Verleger gehört.</span><span class="sxs-lookup"><span data-stu-id="d94b4-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="d94b4-114">Alle Beispiele Verkaufs Werte und Steuer Prozentsätze in diesem Thema dienen nur zu Veranschaulichung, nicht zu exakten Abbildungen.</span><span class="sxs-lookup"><span data-stu-id="d94b4-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="d94b4-115">Verleger transagiert in von Microsoft verwalteten Steuer Ländern</span><span class="sxs-lookup"><span data-stu-id="d94b4-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="d94b4-116">**Szenario A** – Transaktionen, die zwischen einem Verleger und einem Kunden in einem von [Microsoft verwalteten steuerland](tax-details-marketplace.md#microsoft-managed-countries)stattfinden.</span><span class="sxs-lookup"><span data-stu-id="d94b4-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="d94b4-117">Diese Transaktionen werden zum Zeitpunkt des Verkaufs der anwendbaren Steuern hinzugefügt, und Microsoft sendet diese Steuern an das anwendbare Land.</span><span class="sxs-lookup"><span data-stu-id="d94b4-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="d94b4-118">Keine Steuern von Auszahlungs-und Auszahlungs Berechnungen sind Steuer exklusiv.</span><span class="sxs-lookup"><span data-stu-id="d94b4-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="d94b4-119">Weitere Informationen finden Sie unter [Szenario D](#foreign-publisher-transacts-with-us-customer) für Transaktionen zwischen einem nicht-US-Verleger und einem US-Kunden.</span><span class="sxs-lookup"><span data-stu-id="d94b4-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="d94b4-121">Verleger transagiert in von Microsoft verwalteten Steuer Ländern, in denen die Marketplace-Gebühr gebührenpflichtig ist</span><span class="sxs-lookup"><span data-stu-id="d94b4-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="d94b4-122">**Szenario B** – Transaktionen, die zwischen einem US-basierten Verleger (gemäß der Definition in den Steuer Profilinformationen Ihres Partner Centers) für einen Kunden in einem von Microsoft verwalteten steuerland gelten, in dem das Land eine Steuern der Marketplace-Gebühr auferlegt (ein kostenpflichtiger Dienst).</span><span class="sxs-lookup"><span data-stu-id="d94b4-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="d94b4-123">In diesem Szenario wird die Steuern der Kosten für den Store-Dienst von der Auszahlung des Herausgebers subtrahiert.</span><span class="sxs-lookup"><span data-stu-id="d94b4-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario B an.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="d94b4-125">Verleger transaagiert in vom Herausgeber verwalteten Steuer Ländern</span><span class="sxs-lookup"><span data-stu-id="d94b4-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="d94b4-126">**Szenario C** – Transaktionen, die zwischen einem Verleger und einem Kunden in einem von einem Herausgeber verwalteten steuerland stattfinden, das keine der Kunden zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="d94b4-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="d94b4-127">Kunden bezahlen zum Point of Sale keine Steuern, und es ist die Verpflichtung des Herausgebers, sämtliche anwendbaren Steuern zu bezahlen.</span><span class="sxs-lookup"><span data-stu-id="d94b4-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="d94b4-128">Weitere Informationen zu Land spezifischen Preisen (z. b. zum versetzen bevorstehender Steuern) finden Sie unter [Pläne und Preise für kommerzielle Marketplace-Angebote](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="d94b4-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="d94b4-130">Foreign Publisher transagiert mit US-Kunde</span><span class="sxs-lookup"><span data-stu-id="d94b4-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="d94b4-131">**Szenario D** – alle fremden Verleger (gemäß Definition in Ihren Partner Center-Steuer Profilinformationen) in Ländern ohne einen US-Vertrag (siehe [Szenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) Erstellen eines Verkaufs an einen US-basierten Kunden (gemäß seiner Kundenkonto Adresse).</span><span class="sxs-lookup"><span data-stu-id="d94b4-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="d94b4-132">Die US-Regierung verlangt, dass Microsoft Steuern im Auftrag des Verlegers zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="d94b4-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="d94b4-133">Die von der Auszahlung an den Verleger zurückgehaltenen Steuererklärungen werden basierend auf dem Angebotspreis berechnet.</span><span class="sxs-lookup"><span data-stu-id="d94b4-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="d94b4-135">Der fremd Verleger mit einem Vertrag wird mit dem US-Kunden abgearbeitet.</span><span class="sxs-lookup"><span data-stu-id="d94b4-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="d94b4-136">**Szenario E** – alle fremden Verleger (gemäß Definition in Ihren Partner Center-Steuer Profilinformationen) in Ländern mit einem US-Vertrag, der einen US-basierten Kunden verkauft (wie von seiner Kundenkonto Adresse definiert).</span><span class="sxs-lookup"><span data-stu-id="d94b4-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="d94b4-137">Die US-Regierung verlangt nicht, dass Microsoft Steuern im Auftrag des Verlegers zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="d94b4-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="d94b4-139">Der fremd Verleger wird an einen Kunden in einem von Microsoft verwalteten Land (außerhalb von Irland) in einem von Microsoft verwalteten Land verkauft.</span><span class="sxs-lookup"><span data-stu-id="d94b4-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="d94b4-140">**Szenario F** – alle Transaktionen zwischen fremden Verlegern und EU-Kunden in der EU (außerhalb von Irland) in einem Microsoft-Managed Land.</span><span class="sxs-lookup"><span data-stu-id="d94b4-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="d94b4-141">Der Kunde zahlt keine Steuern für den Verkauf.</span><span class="sxs-lookup"><span data-stu-id="d94b4-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario F an.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="d94b4-143">Der fremd Verleger verkauft sich in einem von Microsoft verwalteten Land in einem von Microsoft verwalteten Land (in Irland) an einen Kunden in der EU</span><span class="sxs-lookup"><span data-stu-id="d94b4-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="d94b4-144">**Szenario G** – alle Transaktionen zwischen fremden Verlegern und EU-Kunden in der EU (in Irland) in einem Microsoft-Managed Land.</span><span class="sxs-lookup"><span data-stu-id="d94b4-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="d94b4-145">Der Kunde zahlt die irische Umsatzsteuer, und Microsoft zahlt diese Steuern an die irische Regierung.</span><span class="sxs-lookup"><span data-stu-id="d94b4-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zeigt den Workflow für das Auszahlungsprozess Szenario G.":::

## <a name="next-steps"></a><span data-ttu-id="d94b4-147">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d94b4-147">Next steps</span></span>

- [<span data-ttu-id="d94b4-148">FAQ zu Verlegern</span><span class="sxs-lookup"><span data-stu-id="d94b4-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="d94b4-149">Anweisungen zum Erstellen von Zahlungs-und Steuer Profilen</span><span class="sxs-lookup"><span data-stu-id="d94b4-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)