---
title: Verwenden der Abstimmungs Dateien
ms.topic: article
ms.date: 03/10/2021
description: Erfahren Sie mehr über das Abgleichen von Dateien in Partner Center und über die Interpretation der detaillierten Zeilen Element Sichten für einen bestimmten Abrechnungszeitraum.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022773"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="30c09-103">Erfahren Sie, wie Sie die Zeilen Elemente in Ihren Partner Center-Abstimmungs Dateien lesen.</span><span class="sxs-lookup"><span data-stu-id="30c09-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="30c09-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="30c09-104">**Appropriate roles**</span></span>

- <span data-ttu-id="30c09-105">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="30c09-105">Billing admin</span></span>
- <span data-ttu-id="30c09-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="30c09-106">Global admin</span></span>

<span data-ttu-id="30c09-107">Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="30c09-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="30c09-108">Zu den Zeilen Element Details zählen Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Lizenzen zu einem Abonnement).</span><span class="sxs-lookup"><span data-stu-id="30c09-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="30c09-109">Informationen zum Lesen der **Rechnung** finden Sie unter [Lesen der](read-your-bill.md)Rechnung.</span><span class="sxs-lookup"><span data-stu-id="30c09-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="30c09-110">Grundlegendes zu Abstimmungs Datei Feldern</span><span class="sxs-lookup"><span data-stu-id="30c09-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="30c09-111">Grundlegendes zu den Feldern in lizenzbasierten Abstimmungsdateien von Partner Center</span><span class="sxs-lookup"><span data-stu-id="30c09-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="30c09-112">Grundlegendes zu nutzungsbasierten Abstimmungsdateien und ihren spezifischen Feldern im Partner Center</span><span class="sxs-lookup"><span data-stu-id="30c09-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="30c09-113">Abstimmungsdateien zur täglich bewerteten Nutzung: Felder</span><span class="sxs-lookup"><span data-stu-id="30c09-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="30c09-114">Felder für das einmalige kaufen von CSP-Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="30c09-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="30c09-115">Grundlegendes zu Lade Typen in Abgleich Dateien</span><span class="sxs-lookup"><span data-stu-id="30c09-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="30c09-116">Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="30c09-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="30c09-117">Beheben von Formatierungsproblemen</span><span class="sxs-lookup"><span data-stu-id="30c09-117">Fix formatting issues</span></span>

<span data-ttu-id="30c09-118">Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten.</span><span class="sxs-lookup"><span data-stu-id="30c09-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="30c09-119">Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="30c09-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="30c09-120">Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:</span><span class="sxs-lookup"><span data-stu-id="30c09-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="30c09-121">Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="30c09-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="30c09-122">Wählen Sie die erste Spalte in der Datei aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="30c09-123">Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**.</span><span class="sxs-lookup"><span data-stu-id="30c09-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="30c09-124">Wählen Sie im Menüband **Daten** aus, und wählen Sie dann **Text in Spalten** aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="30c09-125">Wählen Sie im Assistenten einen **Begrenzungs Dateityp** aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="30c09-126">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="30c09-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="30c09-127">Wählen Sie im Feld **Trenn** Zeichen die Option **Komma** aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="30c09-128">(Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="30c09-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="30c09-129">Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy** aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="30c09-130">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="30c09-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="30c09-131">Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="30c09-132">Wählen Sie **Fertig stellen** aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="30c09-133">Programm gesteuertes herunterladen von Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="30c09-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="30c09-134">Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="30c09-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="30c09-135">Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="30c09-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="30c09-136">Map-Steuern oder Mehrwertsteuer</span><span class="sxs-lookup"><span data-stu-id="30c09-136">Map taxes or VAT</span></span>

<span data-ttu-id="30c09-137">So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:</span><span class="sxs-lookup"><span data-stu-id="30c09-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="30c09-138">Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="30c09-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="30c09-139">Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="30c09-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="30c09-140">Abstimmungs Dateien nach Partner itemisieren</span><span class="sxs-lookup"><span data-stu-id="30c09-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="30c09-141">Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.</span><span class="sxs-lookup"><span data-stu-id="30c09-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="30c09-142">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="30c09-142">MPN ID</span></span> | <span data-ttu-id="30c09-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30c09-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="30c09-144">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="30c09-144">MPN ID</span></span> | <span data-ttu-id="30c09-145">Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="30c09-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="30c09-146">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="30c09-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="30c09-147">Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="30c09-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="30c09-148">Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="30c09-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="30c09-149">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="30c09-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="30c09-150">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="30c09-150">Reseller MPN ID</span></span>

<span data-ttu-id="30c09-151">Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="30c09-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="30c09-152">Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID** verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="30c09-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="30c09-153">Wenn der CSP-Partner eine **Reseller MPN-ID** entfernt, wird dieser Wert auf *-1* festgelegt.</span><span class="sxs-lookup"><span data-stu-id="30c09-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="30c09-154">So können Sie die **Reseller MPN-ID** anzeigen oder aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="30c09-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="30c09-155">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="30c09-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="30c09-156">Wählen Sie im Menü „Partner Center” **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="30c09-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="30c09-157">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="30c09-158">Wählen Sie im Menü Kunde die Option **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="30c09-159">Wählen Sie das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="30c09-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="30c09-160">Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.</span><span class="sxs-lookup"><span data-stu-id="30c09-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="30c09-161">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="30c09-161">Next steps</span></span>

- [<span data-ttu-id="30c09-162">Lesen Ihrer Rechnung & Datei "Reconnaissance"</span><span class="sxs-lookup"><span data-stu-id="30c09-162">How to read your bill & recon file</span></span>](read-your-bill.md) 