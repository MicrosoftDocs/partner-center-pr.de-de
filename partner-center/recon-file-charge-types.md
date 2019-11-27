---
title: Abgleich-Datei Lade Typen | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Arten von Gebühren (Lizenz basiert, Nutzungs basiert und einmalig), Gutschriften und Rabatte für Partner Center-Abstimmungs Dateien.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389808"
---
# <a name="understand-charge-types"></a><span data-ttu-id="e59e0-103">Grundlegendes zu Lade Typen</span><span class="sxs-lookup"><span data-stu-id="e59e0-103">Understand charge types</span></span>

<span data-ttu-id="e59e0-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="e59e0-104">Applies to:</span></span>

- <span data-ttu-id="e59e0-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e59e0-105">Partner Center</span></span>
- <span data-ttu-id="e59e0-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e59e0-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e59e0-107">In diesem Thema werden die Zuordnungen zwischen einem Rechnungs Abschnitt und den zugehörigen Abrechnungs Typen beschrieben, die möglicherweise in der Abstimmungs Datei liegen.</span><span class="sxs-lookup"><span data-stu-id="e59e0-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="e59e0-108">Ihre Rechnung enthält eine Zusammenfassung der Gebühren.</span><span class="sxs-lookup"><span data-stu-id="e59e0-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="e59e0-109">Die Abstimmungs Datei bietet eine detaillierte Aufschlüsselung der Zeilen Element Transaktionen, einschließlich der Lade Typen.</span><span class="sxs-lookup"><span data-stu-id="e59e0-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="e59e0-110">Weitere Informationen zum Abgleich von Dateien finden [Sie unter Verwenden](use-the-reconciliation-files.md)von Abstimmungs Dateien.</span><span class="sxs-lookup"><span data-stu-id="e59e0-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="e59e0-111">Sowohl [nutzungsbasierte ababstimmungs Dateien](usage-based-recon-files.md) als auch [Lizenz basierte ababstimmungs Dateien](license-based-recon-files.md) zeigen nur nutzungsbezogene Transaktionen und Gebühren an (genutzte Einheiten und zugehörige Gebühren).</span><span class="sxs-lookup"><span data-stu-id="e59e0-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="e59e0-112">Einmalige Gutschriften, Rabatte oder Rückerstattungen, die auf der Rechnung angezeigt werden **, werden nicht** in der Abstimmungs Datei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e59e0-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="e59e0-113">Zuordnen von Gebühren Typen zu Rechnungs Gebühren</span><span class="sxs-lookup"><span data-stu-id="e59e0-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="e59e0-114">Verwenden Sie die Filteroptionen in Microsoft Excel, um die Berechnung der Kosten für einen Querverweis zwischen der Rechnung und der Abstimmungs Datei zu überschreiten.</span><span class="sxs-lookup"><span data-stu-id="e59e0-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="e59e0-115">Filtern Sie nach den Gebühren Typen in der Abstimmungs Datei, um die Rechnungs Gebühren einem Satz von Gebühren für die Abstimmungs Datei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="e59e0-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="e59e0-116">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="e59e0-116">License-based charges</span></span>

<span data-ttu-id="e59e0-117">Um diese lizenzbasierten Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e59e0-118">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="e59e0-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e59e0-119">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e59e0-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e59e0-120">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="e59e0-120">Activation fee</span></span> | <span data-ttu-id="e59e0-121">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf verwendet.</span><span class="sxs-lookup"><span data-stu-id="e59e0-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="e59e0-122">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="e59e0-122">Cancel fee</span></span> | <span data-ttu-id="e59e0-123">Anteilsmäßig an den Kunden abgezahlte Gebühren, wenn die zugeordneten Arbeitsplätze geändert werden.</span><span class="sxs-lookup"><span data-stu-id="e59e0-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="e59e0-124">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="e59e0-124">Cycle fee</span></span> | <span data-ttu-id="e59e0-125">Regelmäßige Gebühren für ein Abonnement.</span><span class="sxs-lookup"><span data-stu-id="e59e0-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="e59e0-126">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="e59e0-126">Cycle instance prorate</span></span> | <span data-ttu-id="e59e0-127">Anteilsmäßig abgeänderte Gebühren vom Kunden, wenn die zugeordneten Arbeitsplätze geändert werden.</span><span class="sxs-lookup"><span data-stu-id="e59e0-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="e59e0-128">Gebühren bei Stornierung anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="e59e0-128">Prorate fees when cancel</span></span> | <span data-ttu-id="e59e0-129">Anteilsmäßig abgenommene Rückerstattung für den nicht genutzten Dienst Anteil nach Abbruch.</span><span class="sxs-lookup"><span data-stu-id="e59e0-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="e59e0-130">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="e59e0-130">Prorate fees when purchase</span></span> | <span data-ttu-id="e59e0-131">Der Typ der Gebühr für ein Abonnement bei Verwendung der jährlichen Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="e59e0-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="e59e0-132">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="e59e0-132">Purchase fee</span></span> | <span data-ttu-id="e59e0-133">Der Gebühr für ein Abonnement, wenn die monatliche Abrechnung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e59e0-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="e59e0-134">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="e59e0-134">Prorate fee when renew</span></span> | <span data-ttu-id="e59e0-135">Anteilsmäßig Kosten bei der Erneuerung des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="e59e0-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="e59e0-136">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="e59e0-136">Renew fee</span></span> | <span data-ttu-id="e59e0-137">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="e59e0-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="e59e0-138">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="e59e0-138">Prorate fees when activate</span></span> | <span data-ttu-id="e59e0-139">> anteilsmäßig an der Aktivierung bis zum Ende des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="e59e0-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="e59e0-140">Einmalige Gebühren</span><span class="sxs-lookup"><span data-stu-id="e59e0-140">One-time charges</span></span>

<span data-ttu-id="e59e0-141">Um diese einmaligen Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e59e0-142">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="e59e0-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e59e0-143">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e59e0-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e59e0-144">Neu</span><span class="sxs-lookup"><span data-stu-id="e59e0-144">New</span></span> | <span data-ttu-id="e59e0-145">Wird verwendet, wenn ein neuer Kauf erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e59e0-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="e59e0-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e59e0-146">addQuantity</span></span> | <span data-ttu-id="e59e0-147">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Erhöhung verwendet.</span><span class="sxs-lookup"><span data-stu-id="e59e0-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="e59e0-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e59e0-148">removeQuantity</span></span> | <span data-ttu-id="e59e0-149">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Abnahme verwendet.</span><span class="sxs-lookup"><span data-stu-id="e59e0-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="e59e0-150">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="e59e0-150">Cancel</span></span> | <span data-ttu-id="e59e0-151">Wird verwendet, wenn ein Abonnement abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="e59e0-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="e59e0-152">Konvertieren</span><span class="sxs-lookup"><span data-stu-id="e59e0-152">Convert</span></span> | <span data-ttu-id="e59e0-153">Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Arbeitsplätze jedoch unverändert bleibt.</span><span class="sxs-lookup"><span data-stu-id="e59e0-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="e59e0-154">Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="e59e0-154">Usage charges</span></span>

<span data-ttu-id="e59e0-155">Um diese Nutzungsgebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e59e0-156">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="e59e0-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e59e0-157">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e59e0-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e59e0-158">Nutzungsgebühr beim Stornieren bewerten</span><span class="sxs-lookup"><span data-stu-id="e59e0-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="e59e0-159">Der Zugriff auf die Nutzungsgebühr bei einem Abbruch für die nicht bezahlte Nutzung während des aktuellen Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="e59e0-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="e59e0-160">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="e59e0-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="e59e0-161">Zugriffs Nutzungsgebühr für den aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="e59e0-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="e59e0-162">Gutschriften</span><span class="sxs-lookup"><span data-stu-id="e59e0-162">Credits</span></span>

<span data-ttu-id="e59e0-163">So ordnen Sie diese Gutschriften Ihrer Rechnung zu:</span><span class="sxs-lookup"><span data-stu-id="e59e0-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="e59e0-164">**Addieren Sie totalforcustomer** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="e59e0-165">Summieren Sie die **posttaxtotal** -Spalte aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="e59e0-166">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="e59e0-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e59e0-167">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e59e0-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e59e0-168">Ausgleichen einer Position</span><span class="sxs-lookup"><span data-stu-id="e59e0-168">Offset a line item</span></span> | <span data-ttu-id="e59e0-169">Teilweise oder vollständige Rückerstattung eines Zeilen Elements, einschließlich Steuern.</span><span class="sxs-lookup"><span data-stu-id="e59e0-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="e59e0-170">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="e59e0-170">Usage-based discounts</span></span>

<span data-ttu-id="e59e0-171">Um diese nutzungsbasierten Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e59e0-172">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="e59e0-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e59e0-173">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e59e0-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e59e0-174">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="e59e0-174">Activation discount</span></span> | <span data-ttu-id="e59e0-175">Der Rabatt wurde beim Aktivieren des Abonnements angewendet.</span><span class="sxs-lookup"><span data-stu-id="e59e0-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="e59e0-176">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="e59e0-176">Cycle discount</span></span> | <span data-ttu-id="e59e0-177">Der Rabatt wird auf regelmäßige Gebühren angewendet.</span><span class="sxs-lookup"><span data-stu-id="e59e0-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="e59e0-178">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="e59e0-178">Renew discount</span></span> | <span data-ttu-id="e59e0-179">Der Rabatt wurde bei erneutem Abonnement zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e59e0-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="e59e0-180">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="e59e0-180">Cancel discount</span></span> | <span data-ttu-id="e59e0-181">Gebühren, die beim Abbruch von Rabatten angewendet wurden.</span><span class="sxs-lookup"><span data-stu-id="e59e0-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="e59e0-182">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="e59e0-182">License-based discounts</span></span>

<span data-ttu-id="e59e0-183">Um Lizenz basierte Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **totalotherdiscount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="e59e0-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="e59e0-184">*Lizenz basierte Rabatte können auf mehrere Lade Typen angewendet werden.*</span><span class="sxs-lookup"><span data-stu-id="e59e0-184">*License-based discounts may be applied to multiple charge types.*</span></span>
