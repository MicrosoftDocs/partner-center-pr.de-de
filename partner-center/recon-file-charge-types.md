---
title: Abgleich-Datei Lade Typen | Partner Center
ms.topic: article
ms.date: 01/06/2020
description: Arten von Gebühren (Lizenz basiert, Nutzungs basiert und einmalig), Gutschriften und Rabatte für Partner Center-Abstimmungs Dateien.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b18a2a7d53e2f9d35baac2412c1710c21d6d98eb
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716871"
---
# <a name="understand-charge-types"></a><span data-ttu-id="067e9-103">Grundlegendes zu Lade Typen</span><span class="sxs-lookup"><span data-stu-id="067e9-103">Understand charge types</span></span>

<span data-ttu-id="067e9-104">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="067e9-104">**Applies to**</span></span>

- <span data-ttu-id="067e9-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="067e9-105">Partner Center</span></span>
- <span data-ttu-id="067e9-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="067e9-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="067e9-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="067e9-107">**Appropriate roles**</span></span>

- <span data-ttu-id="067e9-108">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="067e9-108">Admin agent</span></span>
- <span data-ttu-id="067e9-109">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="067e9-109">Billing admin</span></span>
- <span data-ttu-id="067e9-110">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="067e9-110">Global admin</span></span>

<span data-ttu-id="067e9-111">In diesem Thema werden die Zuordnungen zwischen einem Rechnungs Abschnitt und den zugehörigen Abrechnungs Typen beschrieben, die möglicherweise in der Abstimmungs Datei liegen.</span><span class="sxs-lookup"><span data-stu-id="067e9-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="067e9-112">Ihre Rechnung enthält eine Zusammenfassung der Gebühren.</span><span class="sxs-lookup"><span data-stu-id="067e9-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="067e9-113">Die Abstimmungs Datei bietet eine detaillierte Aufschlüsselung der Zeilen Element Transaktionen, einschließlich der Lade Typen.</span><span class="sxs-lookup"><span data-stu-id="067e9-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="067e9-114">Weitere Informationen zum Abgleich von Dateien finden [Sie unter Verwenden](use-the-reconciliation-files.md)von Abstimmungs Dateien.</span><span class="sxs-lookup"><span data-stu-id="067e9-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="067e9-115">Sowohl [nutzungsbasierte ababstimmungs Dateien](usage-based-recon-files.md) als auch [Lizenz basierte ababstimmungs Dateien](license-based-recon-files.md) zeigen nur nutzungsbezogene Transaktionen und Gebühren an (genutzte Einheiten und zugehörige Gebühren).</span><span class="sxs-lookup"><span data-stu-id="067e9-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="067e9-116">Einmalige Gutschriften, Rabatte oder Rückerstattungen, die auf der Rechnung angezeigt werden **, werden nicht** in der Abstimmungs Datei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="067e9-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="067e9-117">Zuordnen von Gebühren Typen zu Rechnungs Gebühren</span><span class="sxs-lookup"><span data-stu-id="067e9-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="067e9-118">Verwenden Sie die Filteroptionen in Microsoft Excel, um die Berechnung der Kosten für einen Querverweis zwischen der Rechnung und der Abstimmungs Datei zu überschreiten.</span><span class="sxs-lookup"><span data-stu-id="067e9-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="067e9-119">Filtern Sie nach den Gebühren Typen in der Abstimmungs Datei, um die Rechnungs Gebühren einem Satz von Gebühren für die Abstimmungs Datei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="067e9-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="067e9-120">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="067e9-120">License-based charges</span></span>

<span data-ttu-id="067e9-121">Um diese lizenzbasierten Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="067e9-122">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="067e9-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="067e9-123">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="067e9-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="067e9-124">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="067e9-124">Activation fee</span></span> | <span data-ttu-id="067e9-125">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf verwendet.</span><span class="sxs-lookup"><span data-stu-id="067e9-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="067e9-126">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="067e9-126">Cancel fee</span></span> | <span data-ttu-id="067e9-127">Anteilsmäßig an den Kunden abgezahlte Gebühren, wenn die zugeordneten Arbeitsplätze geändert werden.</span><span class="sxs-lookup"><span data-stu-id="067e9-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="067e9-128">Instanz anteilig stornieren</span><span class="sxs-lookup"><span data-stu-id="067e9-128">Cancel instance prorate</span></span> | <span data-ttu-id="067e9-129">Anteilsmäßig abgeänderte Gebühren, die abgebrochen wurden, wenn der Kunde mit monatlichem Abonnement das Abonnement angehalten hat und die zugeordneten Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="067e9-129">Prorated charges cancelled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="067e9-130">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="067e9-130">Cycle fee</span></span> | <span data-ttu-id="067e9-131">Regelmäßige Gebühren für ein Abonnement.</span><span class="sxs-lookup"><span data-stu-id="067e9-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="067e9-132">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="067e9-132">Cycle instance prorate</span></span> | <span data-ttu-id="067e9-133">Anteilsmäßig abgeänderte Gebühren vom Kunden, wenn die zugeordneten Arbeitsplätze geändert werden.</span><span class="sxs-lookup"><span data-stu-id="067e9-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="067e9-134">Gebühren bei Stornierung anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="067e9-134">Prorate fees when cancel</span></span> | <span data-ttu-id="067e9-135">Anteilsmäßig abgenommene Rückerstattung für den nicht genutzten Dienst Anteil nach Abbruch.</span><span class="sxs-lookup"><span data-stu-id="067e9-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="067e9-136">Anteilsmäßig Gebühren beim Konvertieren aus dem aktuellen Angebot</span><span class="sxs-lookup"><span data-stu-id="067e9-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="067e9-137">Anteilsmäßig anfallenden Gebühren nach der Umstellung des aktuellen monatlichen Abonnements in ein Jahresabonnement.</span><span class="sxs-lookup"><span data-stu-id="067e9-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="067e9-138">Angleichen von Gebühren beim Konvertieren in ein neues Angebot</span><span class="sxs-lookup"><span data-stu-id="067e9-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="067e9-139">Anteilsmäßig anfallenden Gebühren nach der Umstellung eines monatlichen Abonnements in ein neues Jahresabonnement.</span><span class="sxs-lookup"><span data-stu-id="067e9-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="067e9-140">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="067e9-140">Prorate fees when purchase</span></span> | <span data-ttu-id="067e9-141">Der Typ der Gebühr für ein Abonnement bei Verwendung der jährlichen Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="067e9-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="067e9-142">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="067e9-142">Purchase fee</span></span> | <span data-ttu-id="067e9-143">Der Gebühr für ein Abonnement, wenn die monatliche Abrechnung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="067e9-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="067e9-144">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="067e9-144">Prorate fee when renew</span></span> | <span data-ttu-id="067e9-145">Anteilsmäßig Kosten bei der Erneuerung des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="067e9-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="067e9-146">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="067e9-146">Renew fee</span></span> | <span data-ttu-id="067e9-147">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="067e9-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="067e9-148">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="067e9-148">Prorate fees when activate</span></span> | <span data-ttu-id="067e9-149">> anteilsmäßig an der Aktivierung bis zum Ende des Abrechnungszeitraums.</span><span class="sxs-lookup"><span data-stu-id="067e9-149">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="067e9-150">Einmalige Gebühren</span><span class="sxs-lookup"><span data-stu-id="067e9-150">One-time charges</span></span>

<span data-ttu-id="067e9-151">Um diese einmaligen Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="067e9-152">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="067e9-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="067e9-153">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="067e9-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="067e9-154">„Neu“,</span><span class="sxs-lookup"><span data-stu-id="067e9-154">New</span></span> | <span data-ttu-id="067e9-155">Wird verwendet, wenn ein neuer Kauf erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="067e9-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="067e9-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="067e9-156">addQuantity</span></span> | <span data-ttu-id="067e9-157">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Erhöhung verwendet.</span><span class="sxs-lookup"><span data-stu-id="067e9-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="067e9-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="067e9-158">removeQuantity</span></span> | <span data-ttu-id="067e9-159">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Abnahme verwendet.</span><span class="sxs-lookup"><span data-stu-id="067e9-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="067e9-160">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="067e9-160">Cancel</span></span> | <span data-ttu-id="067e9-161">Wird verwendet, wenn ein Abonnement abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="067e9-161">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="067e9-162">Konvertieren</span><span class="sxs-lookup"><span data-stu-id="067e9-162">Convert</span></span> | <span data-ttu-id="067e9-163">Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Arbeitsplätze jedoch unverändert bleibt.</span><span class="sxs-lookup"><span data-stu-id="067e9-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="067e9-164">Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="067e9-164">Usage charges</span></span>

<span data-ttu-id="067e9-165">Um diese Nutzungsgebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="067e9-166">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="067e9-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="067e9-167">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="067e9-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="067e9-168">Nutzungsgebühr beim Stornieren bewerten</span><span class="sxs-lookup"><span data-stu-id="067e9-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="067e9-169">Zugriffsnutzungsgebühr bei Abbruch für eine nicht bezahlte Nutzung im aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="067e9-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="067e9-170">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="067e9-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="067e9-171">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="067e9-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="067e9-172">Gutschriften</span><span class="sxs-lookup"><span data-stu-id="067e9-172">Credits</span></span>

<span data-ttu-id="067e9-173">So ordnen Sie diese Gutschriften Ihrer Rechnung zu:</span><span class="sxs-lookup"><span data-stu-id="067e9-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="067e9-174">**Addieren Sie totalforcustomer** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="067e9-175">Summieren Sie die **posttaxtotal** -Spalte aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="067e9-176">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="067e9-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="067e9-177">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="067e9-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="067e9-178">Ausgleichen einer Position</span><span class="sxs-lookup"><span data-stu-id="067e9-178">Offset a line item</span></span> | <span data-ttu-id="067e9-179">Teilweise oder vollständige Rückerstattung einer Position, einschließlich Steuern.</span><span class="sxs-lookup"><span data-stu-id="067e9-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="067e9-180">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="067e9-180">Usage-based discounts</span></span>

<span data-ttu-id="067e9-181">Um diese nutzungsbasierten Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="067e9-182">Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei)</span><span class="sxs-lookup"><span data-stu-id="067e9-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="067e9-183">Erklärung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="067e9-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="067e9-184">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="067e9-184">Activation discount</span></span> | <span data-ttu-id="067e9-185">Der Rabatt wurde beim Aktivieren des Abonnements angewendet.</span><span class="sxs-lookup"><span data-stu-id="067e9-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="067e9-186">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="067e9-186">Cycle discount</span></span> | <span data-ttu-id="067e9-187">Der bei wiederkehrenden Gebühren gewährte Rabatt.</span><span class="sxs-lookup"><span data-stu-id="067e9-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="067e9-188">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="067e9-188">Renew discount</span></span> | <span data-ttu-id="067e9-189">Der Rabatt wurde bei erneutem Abonnement zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="067e9-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="067e9-190">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="067e9-190">Cancel discount</span></span> | <span data-ttu-id="067e9-191">Gebühren, die beim Abbruch von Rabatten angewendet wurden.</span><span class="sxs-lookup"><span data-stu-id="067e9-191">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="067e9-192">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="067e9-192">License-based discounts</span></span>

<span data-ttu-id="067e9-193">Um Lizenz basierte Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **totalotherdiscount** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="067e9-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="067e9-194">*Lizenz basierte Rabatte können auf mehrere Lade Typen angewendet werden.*</span><span class="sxs-lookup"><span data-stu-id="067e9-194">*License-based discounts may be applied to multiple charge types.*</span></span>
