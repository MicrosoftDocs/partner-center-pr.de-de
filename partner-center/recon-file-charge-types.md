---
title: Gebührenarten für Abstimmungsdateien
ms.topic: article
ms.date: 06/05/2020
description: Ermitteln Sie die Arten von Gebühren (z. b. Lizenz basiert, Nutzungs basiert und einmalig), Gutschriften und Rabatte in Partner Center-Abstimmungs Dateien.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/31/2020
ms.locfileid: "87479113"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="b6b23-103">Informationen zu den verschiedenen Lade Typen in Partner Center-Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="b6b23-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="b6b23-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="b6b23-104">**Applies to**</span></span>

- <span data-ttu-id="b6b23-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="b6b23-105">Partner Center</span></span>
- <span data-ttu-id="b6b23-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="b6b23-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b6b23-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="b6b23-107">**Appropriate roles**</span></span>

- <span data-ttu-id="b6b23-108">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="b6b23-108">Admin agent</span></span>
- <span data-ttu-id="b6b23-109">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="b6b23-109">Billing admin</span></span>
- <span data-ttu-id="b6b23-110">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b6b23-110">Global admin</span></span>

<span data-ttu-id="b6b23-111">In diesem Thema werden die Zuordnungen zwischen einem Rechnungs Abschnitt und den zugehörigen Abrechnungs Typen beschrieben, die möglicherweise in der Abstimmungs Datei liegen.</span><span class="sxs-lookup"><span data-stu-id="b6b23-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="b6b23-112">Ihre Rechnung enthält eine Zusammenfassung der Gebühren.</span><span class="sxs-lookup"><span data-stu-id="b6b23-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="b6b23-113">Die Abstimmungs Datei bietet eine detaillierte Aufschlüsselung der Zeilen Element Transaktionen, einschließlich der Lade Typen.</span><span class="sxs-lookup"><span data-stu-id="b6b23-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="b6b23-114">Weitere Informationen zum Abgleich von Dateien finden [Sie unter Verwenden](use-the-reconciliation-files.md)von Abstimmungs Dateien.</span><span class="sxs-lookup"><span data-stu-id="b6b23-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="b6b23-115">Sowohl [nutzungsbasierte ababstimmungs Dateien](usage-based-recon-files.md) als auch [Lizenz basierte ababstimmungs Dateien](license-based-recon-files.md) zeigen nur nutzungsbezogene Transaktionen und Gebühren an (genutzte Einheiten und zugehörige Gebühren).</span><span class="sxs-lookup"><span data-stu-id="b6b23-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="b6b23-116">Einmalige Gutschriften, Rabatte oder Rückerstattungen, die auf der Rechnung angezeigt werden **, werden nicht** in der Abstimmungs Datei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b6b23-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="b6b23-117">Zuordnen von Gebühren Typen zu Rechnungs Gebühren</span><span class="sxs-lookup"><span data-stu-id="b6b23-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="b6b23-118">Verwenden Sie die Filteroptionen in Microsoft Excel, um die Berechnung der Kosten für einen Querverweis zwischen der Rechnung und der Abstimmungs Datei zu überschreiten.</span><span class="sxs-lookup"><span data-stu-id="b6b23-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="b6b23-119">Filtern Sie nach den Gebühren Typen in der Abstimmungs Datei, um die Rechnungs Gebühren einem Satz von Gebühren für die Abstimmungs Datei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="b6b23-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="b6b23-120">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="b6b23-120">License-based charges</span></span>

<span data-ttu-id="b6b23-121">Um diese lizenzbasierten Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b6b23-122">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="b6b23-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b6b23-123">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b6b23-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b6b23-124">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="b6b23-124">Activation fee</span></span> | <span data-ttu-id="b6b23-125">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf verwendet.</span><span class="sxs-lookup"><span data-stu-id="b6b23-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="b6b23-126">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="b6b23-126">Cancel fee</span></span> | <span data-ttu-id="b6b23-127">Anteilsmäßig an den Kunden abgezahlte Gebühren, wenn die zugeordneten Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b6b23-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b6b23-128">Instanzangleich anbrechen</span><span class="sxs-lookup"><span data-stu-id="b6b23-128">Cancel instance prorate</span></span> | <span data-ttu-id="b6b23-129">Anteilsmäßig abgeänderte Gebühren werden abgebrochen, wenn der Kunde mit monatlichem Abonnement das Abonnement angehalten hat und die zugeordneten Lizenzen innerhalb desselben Monats</span><span class="sxs-lookup"><span data-stu-id="b6b23-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="b6b23-130">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="b6b23-130">Cycle fee</span></span> | <span data-ttu-id="b6b23-131">Regelmäßige Gebühren für ein Abonnement.</span><span class="sxs-lookup"><span data-stu-id="b6b23-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="b6b23-132">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="b6b23-132">Cycle instance prorate</span></span> | <span data-ttu-id="b6b23-133">Anteilsmäßig abgeänderte Gebühren vom Kunden, wenn zugehörige Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b6b23-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b6b23-134">Gebühren bei Stornierung anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="b6b23-134">Prorate fees when cancel</span></span> | <span data-ttu-id="b6b23-135">Anteilsmäßig abgenommene Rückerstattung für den nicht genutzten Dienst Anteil nach Abbruch.</span><span class="sxs-lookup"><span data-stu-id="b6b23-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="b6b23-136">Anteilsmäßig Gebühren beim Konvertieren aus dem aktuellen Angebot</span><span class="sxs-lookup"><span data-stu-id="b6b23-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="b6b23-137">Anteilsmäßig anfallenden Gebühren nach der Umstellung des aktuellen monatlichen Abonnements in ein Jahresabonnement.</span><span class="sxs-lookup"><span data-stu-id="b6b23-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="b6b23-138">Angleichen von Gebühren beim Konvertieren in ein neues Angebot</span><span class="sxs-lookup"><span data-stu-id="b6b23-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="b6b23-139">Anteilsmäßig anfallenden Gebühren nach der Umstellung eines monatlichen Abonnements in ein neues Jahresabonnement.</span><span class="sxs-lookup"><span data-stu-id="b6b23-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="b6b23-140">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="b6b23-140">Prorate fees when purchase</span></span> | <span data-ttu-id="b6b23-141">Der Gebühr für ein Abonnement, wenn die monatliche oder jährliche Abrechnung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b6b23-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="b6b23-142">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="b6b23-142">Prorate fee when renew</span></span> | <span data-ttu-id="b6b23-143">Anteilsmäßig Kosten bei der Erneuerung des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="b6b23-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="b6b23-144">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="b6b23-144">Renew fee</span></span> | <span data-ttu-id="b6b23-145">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="b6b23-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="b6b23-146">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="b6b23-146">Prorate fees when activate</span></span> | <span data-ttu-id="b6b23-147">Anteilsmäßig an der Aktivierung bis zum Ende des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="b6b23-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="b6b23-148">Einmalige Gebühren</span><span class="sxs-lookup"><span data-stu-id="b6b23-148">One-time charges</span></span>

<span data-ttu-id="b6b23-149">Um diese einmaligen Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b6b23-150">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="b6b23-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b6b23-151">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b6b23-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b6b23-152">Neu</span><span class="sxs-lookup"><span data-stu-id="b6b23-152">New</span></span> | <span data-ttu-id="b6b23-153">Wird verwendet, wenn ein neuer Kauf erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="b6b23-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="b6b23-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b6b23-154">addQuantity</span></span> | <span data-ttu-id="b6b23-155">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Erhöhung verwendet.</span><span class="sxs-lookup"><span data-stu-id="b6b23-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="b6b23-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b6b23-156">removeQuantity</span></span> | <span data-ttu-id="b6b23-157">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Abnahme verwendet.</span><span class="sxs-lookup"><span data-stu-id="b6b23-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="b6b23-158">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="b6b23-158">Cancel</span></span> | <span data-ttu-id="b6b23-159">Wird verwendet, wenn ein Abonnement abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="b6b23-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="b6b23-160">Convert</span><span class="sxs-lookup"><span data-stu-id="b6b23-160">Convert</span></span> | <span data-ttu-id="b6b23-161">Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Lizenzen jedoch unverändert bleibt.</span><span class="sxs-lookup"><span data-stu-id="b6b23-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="b6b23-162">Usage Charges</span><span class="sxs-lookup"><span data-stu-id="b6b23-162">Usage charges</span></span>

<span data-ttu-id="b6b23-163">Um diese Nutzungsgebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b6b23-164">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="b6b23-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b6b23-165">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b6b23-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b6b23-166">Nutzungsgebühr beim Stornieren bewerten</span><span class="sxs-lookup"><span data-stu-id="b6b23-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="b6b23-167">Zugriffsnutzungsgebühr bei Abbruch für eine nicht bezahlte Nutzung im aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="b6b23-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="b6b23-168">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="b6b23-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="b6b23-169">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="b6b23-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="b6b23-170">Guthaben</span><span class="sxs-lookup"><span data-stu-id="b6b23-170">Credits</span></span>

<span data-ttu-id="b6b23-171">So ordnen Sie diese Gutschriften Ihrer Rechnung zu:</span><span class="sxs-lookup"><span data-stu-id="b6b23-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="b6b23-172">**Addieren Sie totalforcustomer** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="b6b23-173">Summieren Sie die **posttaxtotal** -Spalte aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="b6b23-174">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="b6b23-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b6b23-175">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b6b23-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b6b23-176">Ausgleichen einer Position</span><span class="sxs-lookup"><span data-stu-id="b6b23-176">Offset a line item</span></span> | <span data-ttu-id="b6b23-177">Teilweise oder vollständige Rückerstattung einer Position, einschließlich Steuern.</span><span class="sxs-lookup"><span data-stu-id="b6b23-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="b6b23-178">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="b6b23-178">Usage-based discounts</span></span>

<span data-ttu-id="b6b23-179">Um diese nutzungsbasierten Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b6b23-180">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="b6b23-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b6b23-181">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b6b23-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b6b23-182">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="b6b23-182">Activation discount</span></span> | <span data-ttu-id="b6b23-183">Der Rabatt wurde beim Aktivieren des Abonnements angewendet.</span><span class="sxs-lookup"><span data-stu-id="b6b23-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="b6b23-184">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="b6b23-184">Cycle discount</span></span> | <span data-ttu-id="b6b23-185">Der bei wiederkehrenden Gebühren gewährte Rabatt.</span><span class="sxs-lookup"><span data-stu-id="b6b23-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="b6b23-186">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="b6b23-186">Renew discount</span></span> | <span data-ttu-id="b6b23-187">Der Rabatt wurde bei erneutem Abonnement zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="b6b23-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="b6b23-188">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="b6b23-188">Cancel discount</span></span> | <span data-ttu-id="b6b23-189">Die bei Stornierung von Rabatten anfallenden Gebühren.</span><span class="sxs-lookup"><span data-stu-id="b6b23-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="b6b23-190">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="b6b23-190">License-based discounts</span></span>

<span data-ttu-id="b6b23-191">Um Lizenz basierte Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **totalotherdiscount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="b6b23-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="b6b23-192">*Lizenz basierte Rabatte können auf mehrere Lade Typen angewendet werden.*</span><span class="sxs-lookup"><span data-stu-id="b6b23-192">*License-based discounts may be applied to multiple charge types.*</span></span>
