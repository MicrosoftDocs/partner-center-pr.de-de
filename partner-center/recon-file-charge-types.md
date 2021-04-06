---
title: Gebührenarten für Abstimmungsdateien
ms.topic: article
ms.date: 06/05/2020
description: Ermitteln Sie die Arten von Gebühren (z. b. Lizenz basiert, Nutzungs basiert und einmalig), Gutschriften und Rabatte in Partner Center-Abstimmungs Dateien.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441594"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="acac5-103">Informationen zu den verschiedenen Lade Typen in Partner Center-Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="acac5-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="acac5-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="acac5-104">**Applies to**</span></span>

- <span data-ttu-id="acac5-105">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="acac5-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="acac5-106">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="acac5-106">**Appropriate roles**</span></span>

- <span data-ttu-id="acac5-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="acac5-107">Admin agent</span></span>
- <span data-ttu-id="acac5-108">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="acac5-108">Billing admin</span></span>
- <span data-ttu-id="acac5-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="acac5-109">Global admin</span></span>

<span data-ttu-id="acac5-110">In diesem Artikel werden die Zuordnungen zwischen einem Rechnungs Abschnitt und den zugehörigen Abrechnungs Typen beschrieben, die sich möglicherweise in der Abstimmungs Datei befinden.</span><span class="sxs-lookup"><span data-stu-id="acac5-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="acac5-111">Ihre Rechnung enthält eine Zusammenfassung der Gebühren.</span><span class="sxs-lookup"><span data-stu-id="acac5-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="acac5-112">Die Abstimmungs Datei bietet eine detaillierte Aufschlüsselung der Zeilen Element Transaktionen, einschließlich der Lade Typen.</span><span class="sxs-lookup"><span data-stu-id="acac5-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="acac5-113">Weitere Informationen zum Abgleich von Dateien finden [Sie unter Verwenden](use-the-reconciliation-files.md)von Abstimmungs Dateien.</span><span class="sxs-lookup"><span data-stu-id="acac5-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="acac5-114">Sowohl [nutzungsbasierte ababstimmungs Dateien](usage-based-recon-files.md) als auch [Lizenz basierte ababstimmungs Dateien](license-based-recon-files.md) zeigen nur nutzungsbezogene Transaktionen und Gebühren an (genutzte Einheiten und zugehörige Gebühren).</span><span class="sxs-lookup"><span data-stu-id="acac5-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="acac5-115">Einmalige Gutschriften, Rabatte oder Rückerstattungen, die auf der Rechnung angezeigt werden **, werden nicht** in der Abstimmungs Datei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="acac5-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="acac5-116">Zuordnen von Gebühren Typen zu Rechnungs Gebühren</span><span class="sxs-lookup"><span data-stu-id="acac5-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="acac5-117">Verwenden Sie die Filteroptionen in Microsoft Excel, um die Berechnung der Kosten für einen Querverweis zwischen der Rechnung und der Abstimmungs Datei zu überschreiten.</span><span class="sxs-lookup"><span data-stu-id="acac5-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="acac5-118">Filtern Sie nach den Gebühren Typen in der Abstimmungs Datei, um die Rechnungs Gebühren einem Satz von Gebühren für die Abstimmungs Datei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="acac5-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="acac5-119">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="acac5-119">License-based charges</span></span>

<span data-ttu-id="acac5-120">Um diese lizenzbasierten Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="acac5-121">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="acac5-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="acac5-122">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="acac5-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="acac5-123">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="acac5-123">Activation fee</span></span> | <span data-ttu-id="acac5-124">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf verwendet.</span><span class="sxs-lookup"><span data-stu-id="acac5-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="acac5-125">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="acac5-125">Cancel fee</span></span> | <span data-ttu-id="acac5-126">Anteilsmäßig an den Kunden abgezahlte Gebühren, wenn die zugeordneten Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="acac5-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="acac5-127">Instanzangleich anbrechen</span><span class="sxs-lookup"><span data-stu-id="acac5-127">Cancel instance prorate</span></span> | <span data-ttu-id="acac5-128">Anteilsmäßig abgeänderte Gebühren werden abgebrochen, wenn der Kunde mit monatlichem Abonnement das Abonnement angehalten hat und die zugeordneten Lizenzen innerhalb desselben Monats</span><span class="sxs-lookup"><span data-stu-id="acac5-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="acac5-129">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="acac5-129">Cycle fee</span></span> | <span data-ttu-id="acac5-130">Regelmäßige Gebühren für ein Abonnement.</span><span class="sxs-lookup"><span data-stu-id="acac5-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="acac5-131">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="acac5-131">Cycle instance prorate</span></span> | <span data-ttu-id="acac5-132">Anteilsmäßig abgeänderte Gebühren vom Kunden, wenn zugehörige Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="acac5-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="acac5-133">Gebühren bei Stornierung anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="acac5-133">Prorate fees when cancel</span></span> | <span data-ttu-id="acac5-134">Anteilsmäßig abgenommene Rückerstattung für den nicht genutzten Dienst Anteil nach Abbruch.</span><span class="sxs-lookup"><span data-stu-id="acac5-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="acac5-135">Anteilsmäßig Gebühren beim Konvertieren aus dem aktuellen Angebot</span><span class="sxs-lookup"><span data-stu-id="acac5-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="acac5-136">Anteilsmäßig anfallenden Gebühren nach der Umstellung des aktuellen monatlichen Abonnements in ein Jahresabonnement.</span><span class="sxs-lookup"><span data-stu-id="acac5-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="acac5-137">Angleichen von Gebühren beim Konvertieren in ein neues Angebot</span><span class="sxs-lookup"><span data-stu-id="acac5-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="acac5-138">Anteilsmäßig anfallenden Gebühren nach der Umstellung eines monatlichen Abonnements in ein neues Jahresabonnement.</span><span class="sxs-lookup"><span data-stu-id="acac5-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="acac5-139">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="acac5-139">Prorate fees when purchase</span></span> | <span data-ttu-id="acac5-140">Der Gebühr für ein Abonnement, wenn die monatliche oder jährliche Abrechnung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="acac5-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="acac5-141">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="acac5-141">Prorate fee when renew</span></span> | <span data-ttu-id="acac5-142">Anteilsmäßig Kosten bei der Erneuerung des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="acac5-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="acac5-143">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="acac5-143">Renew fee</span></span> | <span data-ttu-id="acac5-144">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="acac5-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="acac5-145">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="acac5-145">Prorate fees when activate</span></span> | <span data-ttu-id="acac5-146">Anteilsmäßig an der Aktivierung bis zum Ende des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="acac5-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="acac5-147">Einmalige Gebühren</span><span class="sxs-lookup"><span data-stu-id="acac5-147">One-time charges</span></span>

<span data-ttu-id="acac5-148">Um diese einmaligen Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="acac5-149">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="acac5-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="acac5-150">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="acac5-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="acac5-151">Neu</span><span class="sxs-lookup"><span data-stu-id="acac5-151">New</span></span> | <span data-ttu-id="acac5-152">Wird verwendet, wenn ein neuer Kauf erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="acac5-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="acac5-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="acac5-153">addQuantity</span></span> | <span data-ttu-id="acac5-154">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Erhöhung verwendet.</span><span class="sxs-lookup"><span data-stu-id="acac5-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="acac5-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="acac5-155">removeQuantity</span></span> | <span data-ttu-id="acac5-156">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Abnahme verwendet.</span><span class="sxs-lookup"><span data-stu-id="acac5-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="acac5-157">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="acac5-157">Cancel</span></span> | <span data-ttu-id="acac5-158">Wird verwendet, wenn ein Abonnement abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="acac5-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="acac5-159">Convert</span><span class="sxs-lookup"><span data-stu-id="acac5-159">Convert</span></span> | <span data-ttu-id="acac5-160">Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Lizenzen jedoch unverändert bleibt.</span><span class="sxs-lookup"><span data-stu-id="acac5-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="acac5-161">Usage Charges</span><span class="sxs-lookup"><span data-stu-id="acac5-161">Usage charges</span></span>

<span data-ttu-id="acac5-162">Um diese Nutzungsgebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="acac5-163">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="acac5-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="acac5-164">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="acac5-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="acac5-165">Nutzungsgebühr beim Stornieren bewerten</span><span class="sxs-lookup"><span data-stu-id="acac5-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="acac5-166">Zugriffsnutzungsgebühr bei Abbruch für eine nicht bezahlte Nutzung im aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="acac5-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="acac5-167">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="acac5-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="acac5-168">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="acac5-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="acac5-169">Mitwirkende</span><span class="sxs-lookup"><span data-stu-id="acac5-169">Credits</span></span>

<span data-ttu-id="acac5-170">So ordnen Sie diese Gutschriften Ihrer Rechnung zu:</span><span class="sxs-lookup"><span data-stu-id="acac5-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="acac5-171">**Addieren Sie totalforcustomer** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="acac5-172">Summieren Sie die **posttaxtotal** -Spalte aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="acac5-173">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="acac5-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="acac5-174">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="acac5-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="acac5-175">Ausgleichen einer Position</span><span class="sxs-lookup"><span data-stu-id="acac5-175">Offset a line item</span></span> | <span data-ttu-id="acac5-176">Teilweise oder vollständige Rückerstattung einer Position, einschließlich Steuern.</span><span class="sxs-lookup"><span data-stu-id="acac5-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="acac5-177">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="acac5-177">Usage-based discounts</span></span>

<span data-ttu-id="acac5-178">Um diese nutzungsbasierten Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="acac5-179">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="acac5-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="acac5-180">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="acac5-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="acac5-181">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="acac5-181">Activation discount</span></span> | <span data-ttu-id="acac5-182">Der Rabatt wurde beim Aktivieren des Abonnements angewendet.</span><span class="sxs-lookup"><span data-stu-id="acac5-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="acac5-183">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="acac5-183">Cycle discount</span></span> | <span data-ttu-id="acac5-184">Der bei wiederkehrenden Gebühren gewährte Rabatt.</span><span class="sxs-lookup"><span data-stu-id="acac5-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="acac5-185">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="acac5-185">Renew discount</span></span> | <span data-ttu-id="acac5-186">Der Rabatt wurde bei erneutem Abonnement zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="acac5-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="acac5-187">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="acac5-187">Cancel discount</span></span> | <span data-ttu-id="acac5-188">Die bei Stornierung von Rabatten anfallenden Gebühren.</span><span class="sxs-lookup"><span data-stu-id="acac5-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="acac5-189">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="acac5-189">License-based discounts</span></span>

<span data-ttu-id="acac5-190">Um Lizenz basierte Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **totalotherdiscount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="acac5-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="acac5-191">*Lizenz basierte Rabatte können auf mehrere Lade Typen angewendet werden.*</span><span class="sxs-lookup"><span data-stu-id="acac5-191">*License-based discounts may be applied to multiple charge types.*</span></span>
