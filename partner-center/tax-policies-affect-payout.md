---
title: Auswirkungen von Steuerrichtlinien auf die Auszahlung für Azure Marketplace
description: Erfahren Sie, wie sich Steuerrichtlinien auf die Auszahlung für Azure Marketplace auswirken.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686312"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="fa5ed-103">Auswirkungen von Steuerrichtlinien auf die Auszahlung für Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fa5ed-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="fa5ed-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="fa5ed-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fa5ed-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="fa5ed-105">Global admin</span></span>
- <span data-ttu-id="fa5ed-106">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="fa5ed-106">User management admin</span></span>
- <span data-ttu-id="fa5ed-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="fa5ed-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="fa5ed-108">Einführung</span><span class="sxs-lookup"><span data-stu-id="fa5ed-108">Introduction</span></span>

<span data-ttu-id="fa5ed-109">Der kommerzielle Microsoft-Marketplace verfügt über globale Reichweite.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="fa5ed-110">Transaktionen erfolgen über Grenzen hinweg. Je nachdem, wo sich der ISV und der Kunde befinden, können die Auswirkungen auf die Steuer variieren.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="fa5ed-111">Microsoft AppSource und Azure Marketplace die Partner Center Steuerprofilinformationen verwenden, um das Land des ISV zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="fa5ed-112">Um das Land des Kunden zu bestimmen, verwenden Sie entweder die Abrechnungsinformationen des Kunden, oder wenn sich der Kunde in der EU befindet, verwenden wir zwei verschiedene Informationen.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="fa5ed-113">Um die folgenden Szenarien besser zu verstehen, lesen Sie die Tabelle mit den [Steuerdetails,](tax-details-marketplace.md) in der angezeigt wird, ob Microsoft Steuern im Auftrag des Herausgebers einzieht und bezahlt oder ob diese Verantwortung dem Herausgeber gehört.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="fa5ed-114">Alle Beispiele für Verkaufswerte und Steuerprozentsätze in diesem Thema dienen nur zur Veranschaulichung, nicht zu genauen Zahlen.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="fa5ed-115">Herausgebertransaktionen in einem von Microsoft verwalteten Steuerland</span><span class="sxs-lookup"><span data-stu-id="fa5ed-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="fa5ed-116">**Szenario A:** Transaktionen, die zwischen einem Herausgeber und einem Kunden in einem von [Microsoft verwalteten Steuerland](tax-details-marketplace.md#microsoft-managed-countries)stattfinden.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="fa5ed-117">Für diese Transaktionen wird zum Zeitpunkt des Verkaufs die entsprechende Steuer hinzugefügt, und Microsoft sendet diese Steuer an das entsprechende Land.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="fa5ed-118">Keine Steuern werden aus Auszahlungsberechnungen zurückgehalten, und Auszahlungsberechnungen sind steuerausbesteuert.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="fa5ed-119">Informationen zu Transaktionen zwischen einem Nicht-US-Verleger und einem US-Kunden finden Sie unter [Szenario D.](#foreign-publisher-transacts-with-us-customer)</span><span class="sxs-lookup"><span data-stu-id="fa5ed-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario A an.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="fa5ed-121">Herausgebertransaktionen in einem von Microsoft verwalteten Steuerland, in dem die Marketplace-Gebühr steuerbar ist</span><span class="sxs-lookup"><span data-stu-id="fa5ed-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="fa5ed-122">**Szenario B:** Transaktionen, die zwischen einem US-basierten Herausgeber (wie durch die Partner Center Steuerprofilinformationen definiert) an einen Kunden in einem von Microsoft verwalteten Steuerland stattfinden, in dem das Land eine Steuer auf die Marketplace-Gebühr (einen steuerbaren Dienst) erhebt.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="fa5ed-123">In diesem Szenario wird die Gebühr für den Store-Dienst von der Auszahlung des Herausgebers abgezogen.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario B an.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="fa5ed-125">Verlegertransaktionen im vom Herausgeber verwalteten Steuerland</span><span class="sxs-lookup"><span data-stu-id="fa5ed-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="fa5ed-126">**Szenario C:** Transaktionen zwischen einem Herausgeber und einem Kunden in einem vom Herausgeber verwalteten Steuerland, das keine Quellensteuer für Kunden erzwingt.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="fa5ed-127">Kunden zahlen zum Zeitpunkt des Verkaufs keine Steuern, und es ist die Verpflichtung des Herausgebers, alle anwendbaren Steuern zu zahlen.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="fa5ed-128">Weitere Informationen zu landspezifischen Preisen (z. B. zum Ausgleich bevorstehender Angebote) finden Sie unter Pläne und Preise für Angebote [im kommerziellen Marketplace.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="fa5ed-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="fa5ed-130">Foreign Publisher Transacts with US Customer</span><span class="sxs-lookup"><span data-stu-id="fa5ed-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="fa5ed-131">**Szenario D** : Alle (gemäß ihren Partner Center-Steuerprofilinformationen) in Ländern ohne US-Amerikanischen Verleger (siehe Szenario [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) verkaufen einen Kunden in den USA (gemäß der Kundenkontoadresse).</span><span class="sxs-lookup"><span data-stu-id="fa5ed-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="fa5ed-132">DIE US-Regierung verlangt, dass Microsoft die Steuern im Namen des Herausgebers einbehalten muss.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="fa5ed-133">Die Steuer für die Auszahlung an den Herausgeber wird basierend auf dem Angebotspreis berechnet.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="fa5ed-135">Fremder Herausgeber mit einer Transaktionstransaktivierung mit US-Kunden</span><span class="sxs-lookup"><span data-stu-id="fa5ed-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="fa5ed-136">**Szenario E:** Alle herausgeber (gemäß ihren Partner Center-Steuerprofilinformationen) in Ländern mit einem US-Amerikanischen Kunden, der einen Verkauf an einen Kunden in den USA macht (gemäß der Kundenkontoadresse).</span><span class="sxs-lookup"><span data-stu-id="fa5ed-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="fa5ed-137">Die US-Regierung verlangt nicht, dass Microsoft die Steuern im Auftrag des Herausgebers einbehalten muss.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="fa5ed-139">Ein fremder Herausgeber verkauft an einen Kunden mit EU-Umsatzsteuer-Registrierung in einem von Microsoft verwalteten Land (außerhalb von Irland).</span><span class="sxs-lookup"><span data-stu-id="fa5ed-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="fa5ed-140">**Szenario F:** Alle Transaktionen zwischen externen Herausgebern und kunden mit EU-Umsatzsteuer (außerhalb von Irland) in einem Microsoft-Managed Land.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="fa5ed-141">Der Kunde zahlt keine Steuern für den Verkauf.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario F an.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="fa5ed-143">Ein fremder Herausgeber verkauft an einen bei der EU-Steuer registrierten Kunden in einem von Microsoft verwalteten Land (in Irland)</span><span class="sxs-lookup"><span data-stu-id="fa5ed-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="fa5ed-144">**Szenario G:** Alle Transaktionen zwischen fremden Herausgebern und Eu-Kunden mit Eu-Umsatzsteuer-Registrierung (innerhalb von Irland) in einem Microsoft-Managed Land.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="fa5ed-145">Der Kunde zahlt die gesetzliche Steuer, und Microsoft überzahlt diese Steuer an die Regierung.</span><span class="sxs-lookup"><span data-stu-id="fa5ed-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zeigt den Workflow für das Auszahlungsprozessszenario G an.":::

## <a name="next-steps"></a><span data-ttu-id="fa5ed-147">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="fa5ed-147">Next steps</span></span>

- [<span data-ttu-id="fa5ed-148">Häufig gestellte Fragen zum Herausgeber</span><span class="sxs-lookup"><span data-stu-id="fa5ed-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="fa5ed-149">Anweisungen zum Erstellen von Zahlungs- und Steuerprofilen</span><span class="sxs-lookup"><span data-stu-id="fa5ed-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)