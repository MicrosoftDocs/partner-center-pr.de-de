---
title: Verwenden der Abstimmungs Dateien
ms.topic: article
ms.date: 06/08/2020
description: Erfahren Sie mehr über das Abgleichen von Dateien in Partner Center und über die Interpretation der detaillierten Zeilen Element Sichten für einen bestimmten Abrechnungszeitraum.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999704"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="8fb6d-103">Erfahren Sie, wie Sie die Zeilen Elemente in Ihren Partner Center-Abstimmungs Dateien lesen.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="8fb6d-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="8fb6d-104">Applies to:</span></span>

- <span data-ttu-id="8fb6d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="8fb6d-105">Partner Center</span></span>
- <span data-ttu-id="8fb6d-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="8fb6d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8fb6d-107">Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="8fb6d-108">Zu den Zeilen Element Details zählen Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Lizenzen zu einem Abonnement).</span><span class="sxs-lookup"><span data-stu-id="8fb6d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="8fb6d-109">Geeignete Rollen:</span><span class="sxs-lookup"><span data-stu-id="8fb6d-109">Appropriate roles:</span></span>

- <span data-ttu-id="8fb6d-110">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="8fb6d-110">Billing admin</span></span>
- <span data-ttu-id="8fb6d-111">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8fb6d-111">Global admin</span></span>

<span data-ttu-id="8fb6d-112">Informationen zum Lesen der **Rechnung**finden Sie unter [Lesen der](read-your-bill.md)Rechnung.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="8fb6d-113">Grundlegendes zu Abstimmungs Datei Feldern</span><span class="sxs-lookup"><span data-stu-id="8fb6d-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="8fb6d-114">Lizenz basierte Abstimmungs Datei Felder</span><span class="sxs-lookup"><span data-stu-id="8fb6d-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="8fb6d-115">Verwendungs basierte Abstimmungs Datei Felder</span><span class="sxs-lookup"><span data-stu-id="8fb6d-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="8fb6d-116">Nutzungs Abgleich-Datei Felder für die tägliche Bewertung</span><span class="sxs-lookup"><span data-stu-id="8fb6d-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="8fb6d-117">Grundlegendes zu Lade Typen in Abgleich Dateien</span><span class="sxs-lookup"><span data-stu-id="8fb6d-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="8fb6d-118">Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="8fb6d-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="8fb6d-119">Beheben von Formatierungsproblemen</span><span class="sxs-lookup"><span data-stu-id="8fb6d-119">Fix formatting issues</span></span>

<span data-ttu-id="8fb6d-120">Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="8fb6d-121">Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="8fb6d-122">Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:</span><span class="sxs-lookup"><span data-stu-id="8fb6d-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="8fb6d-123">Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="8fb6d-124">Wählen Sie die erste Spalte in der Datei aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="8fb6d-125">Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="8fb6d-126">Wählen Sie im Menüband **Daten**aus, und wählen Sie dann **Text in Spalten**aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="8fb6d-127">Wählen Sie im Assistenten einen **Begrenzungs Dateityp**aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="8fb6d-128">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="8fb6d-129">Wählen Sie im Feld **Trenn** Zeichen die Option **Komma**aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="8fb6d-130">(Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="8fb6d-131">Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy**aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="8fb6d-132">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="8fb6d-133">Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="8fb6d-134">Wählen Sie anschließend **Fertig stellen** aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="8fb6d-135">Programm gesteuertes herunterladen von Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="8fb6d-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="8fb6d-136">Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="8fb6d-137">Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="8fb6d-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="8fb6d-138">Map-Steuern oder Mehrwertsteuer</span><span class="sxs-lookup"><span data-stu-id="8fb6d-138">Map taxes or VAT</span></span>

<span data-ttu-id="8fb6d-139">So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:</span><span class="sxs-lookup"><span data-stu-id="8fb6d-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="8fb6d-140">Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="8fb6d-141">Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="8fb6d-142">Abstimmungs Dateien nach Partner itemisieren</span><span class="sxs-lookup"><span data-stu-id="8fb6d-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="8fb6d-143">Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="8fb6d-144">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="8fb6d-144">MPN ID</span></span> | <span data-ttu-id="8fb6d-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb6d-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="8fb6d-146">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="8fb6d-146">MPN ID</span></span> | <span data-ttu-id="8fb6d-147">Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="8fb6d-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="8fb6d-148">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="8fb6d-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="8fb6d-149">Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="8fb6d-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="8fb6d-150">Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="8fb6d-151">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="8fb6d-152">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="8fb6d-152">Reseller MPN ID</span></span>

<span data-ttu-id="8fb6d-153">Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="8fb6d-154">Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID**verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="8fb6d-155">Wenn der CSP-Partner eine **Reseller MPN-ID**entfernt, wird dieser Wert auf *-1*festgelegt.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="8fb6d-156">So können Sie die **Reseller MPN-ID**anzeigen oder aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="8fb6d-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="8fb6d-157">Melden Sie sich beim Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="8fb6d-158">Wählen Sie im Menü „Partner Center” **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="8fb6d-159">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="8fb6d-160">Wählen Sie im Menü Kunde die Option **Abonnements**aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="8fb6d-161">Wählen Sie das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="8fb6d-162">Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.</span><span class="sxs-lookup"><span data-stu-id="8fb6d-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>