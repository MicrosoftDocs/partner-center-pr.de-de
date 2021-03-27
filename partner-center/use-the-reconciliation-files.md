---
title: Verwenden der Abstimmungs Dateien
ms.topic: article
ms.date: 03/26/2021
description: Erfahren Sie mehr über das Abgleichen von Dateien in Partner Center und über die Interpretation der detaillierten Zeilen Element Sichten für einen bestimmten Abrechnungszeitraum.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633895"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="331ed-103">Erfahren Sie, wie Sie die Zeilen Elemente in Ihren Partner Center-Abstimmungs Dateien lesen.</span><span class="sxs-lookup"><span data-stu-id="331ed-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="331ed-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="331ed-104">**Appropriate roles**</span></span>

- <span data-ttu-id="331ed-105">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="331ed-105">Billing admin</span></span>
- <span data-ttu-id="331ed-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="331ed-106">Global admin</span></span>

<span data-ttu-id="331ed-107">Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="331ed-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="331ed-108">Zu den Zeilen Element Details zählen Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Lizenzen zu einem Abonnement).</span><span class="sxs-lookup"><span data-stu-id="331ed-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="331ed-109">Informationen zum Lesen der **Rechnung** finden Sie unter [Lesen der](read-your-bill.md)Rechnung.</span><span class="sxs-lookup"><span data-stu-id="331ed-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="331ed-110">Grundlegendes zu Abstimmungs Datei Feldern</span><span class="sxs-lookup"><span data-stu-id="331ed-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="331ed-111">Grundlegendes zu den Feldern in lizenzbasierten Abstimmungsdateien von Partner Center</span><span class="sxs-lookup"><span data-stu-id="331ed-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="331ed-112">Grundlegendes zu nutzungsbasierten Abstimmungsdateien und ihren spezifischen Feldern im Partner Center</span><span class="sxs-lookup"><span data-stu-id="331ed-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="331ed-113">Abstimmungsdateien zur täglich bewerteten Nutzung: Felder</span><span class="sxs-lookup"><span data-stu-id="331ed-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="331ed-114">Felder für das einmalige kaufen von CSP-Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="331ed-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="331ed-115">Grundlegendes zu Lade Typen in Abgleich Dateien</span><span class="sxs-lookup"><span data-stu-id="331ed-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="331ed-116">Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="331ed-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="331ed-117">Beheben von Formatierungsproblemen</span><span class="sxs-lookup"><span data-stu-id="331ed-117">Fix formatting issues</span></span>

<span data-ttu-id="331ed-118">Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten.</span><span class="sxs-lookup"><span data-stu-id="331ed-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="331ed-119">Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="331ed-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="331ed-120">Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:</span><span class="sxs-lookup"><span data-stu-id="331ed-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="331ed-121">Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="331ed-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="331ed-122">Wählen Sie die erste Spalte in der Datei aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="331ed-123">Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**.</span><span class="sxs-lookup"><span data-stu-id="331ed-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="331ed-124">Wählen Sie im Menüband **Daten** aus, und wählen Sie dann **Text in Spalten** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="331ed-125">Wählen Sie im Assistenten einen **Begrenzungs Dateityp** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="331ed-126">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="331ed-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="331ed-127">Wählen Sie im Feld **Trenn** Zeichen die Option **Komma** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="331ed-128">(Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="331ed-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="331ed-129">Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="331ed-130">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="331ed-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="331ed-131">Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="331ed-132">Wählen Sie **Fertig stellen** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="331ed-133">Programm gesteuertes herunterladen von Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="331ed-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="331ed-134">Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="331ed-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="331ed-135">Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="331ed-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="331ed-136">Wenn die Datei das Zeilen Limit in Excel überschreitet</span><span class="sxs-lookup"><span data-stu-id="331ed-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="331ed-137">Wenn Sie eine Abstimmungs Datei herunterladen, aber nicht in Microsoft Excel öffnen können, bedeutet dies wahrscheinlich, dass die Datei mehr Zeilen enthält, als in Excel zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="331ed-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="331ed-138">Wenn dies der Fall ist, können Sie eine der folgenden Prozeduren verwenden, um die Datei zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="331ed-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="331ed-139">Öffnen Sie eine Datei für die Wiederaufnahme in Power BI</span><span class="sxs-lookup"><span data-stu-id="331ed-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="331ed-140">Laden Sie die Abstimmungs Datei wie gewohnt herunter.</span><span class="sxs-lookup"><span data-stu-id="331ed-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="331ed-141">Laden Sie eine Instanz von Power BI herunter, installieren und öffnen Sie Sie.</span><span class="sxs-lookup"><span data-stu-id="331ed-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="331ed-142">Wählen Sie auf der Registerkarte Power BI **Startseite** **Daten erhalten** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="331ed-143">Wählen Sie in der Liste der **allgemeinen Datenquellen** die Option **Text/CSV** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="331ed-144">Wenn Sie dazu aufgefordert werden, öffnen Sie Ihre Reconnaissance-Datei.</span><span class="sxs-lookup"><span data-stu-id="331ed-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="331ed-145">Öffnen einer Datei "Reconnaissance" in einer Excel-Pivottabelle</span><span class="sxs-lookup"><span data-stu-id="331ed-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="331ed-146">Laden Sie die Abstimmungs Datei wie gewohnt herunter.</span><span class="sxs-lookup"><span data-stu-id="331ed-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="331ed-147">Öffnen Sie eine neue Datei in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="331ed-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="331ed-148">Wählen Sie auf der Registerkarte **Daten** Daten **erhalten** aus, wählen Sie **aus Datei aus**, und wählen Sie dann **Text/CSV** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="331ed-149">Wenn Sie dazu aufgefordert werden, öffnen Sie Ihre Reconnaissance-Datei.</span><span class="sxs-lookup"><span data-stu-id="331ed-149">When prompted, open your recon file.</span></span> <span data-ttu-id="331ed-150">Ihre Daten werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="331ed-150">Your data will appear.</span></span>
5. <span data-ttu-id="331ed-151">Wählen Sie im Dropdown Menü **Laden** die Option **Laden in** aus, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="331ed-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="331ed-152">Wählen Sie im Dialogfeld **Daten importieren** die Option **pivotfähiger Bericht** aus, um die Datei zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="331ed-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="331ed-153">Map-Steuern oder Mehrwertsteuer</span><span class="sxs-lookup"><span data-stu-id="331ed-153">Map taxes or VAT</span></span>

<span data-ttu-id="331ed-154">So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:</span><span class="sxs-lookup"><span data-stu-id="331ed-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="331ed-155">Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="331ed-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="331ed-156">Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="331ed-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="331ed-157">Abstimmungs Dateien nach Partner itemisieren</span><span class="sxs-lookup"><span data-stu-id="331ed-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="331ed-158">Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.</span><span class="sxs-lookup"><span data-stu-id="331ed-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="331ed-159">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="331ed-159">MPN ID</span></span> | <span data-ttu-id="331ed-160">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="331ed-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="331ed-161">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="331ed-161">MPN ID</span></span> | <span data-ttu-id="331ed-162">Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="331ed-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="331ed-163">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="331ed-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="331ed-164">Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="331ed-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="331ed-165">Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="331ed-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="331ed-166">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="331ed-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="331ed-167">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="331ed-167">Reseller MPN ID</span></span>

<span data-ttu-id="331ed-168">Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="331ed-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="331ed-169">Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID** verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="331ed-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="331ed-170">Wenn der CSP-Partner eine **Reseller MPN-ID** entfernt, wird dieser Wert auf *-1* festgelegt.</span><span class="sxs-lookup"><span data-stu-id="331ed-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="331ed-171">So können Sie die **Reseller MPN-ID** anzeigen oder aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="331ed-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="331ed-172">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="331ed-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="331ed-173">Wählen Sie im Menü „Partner Center” **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="331ed-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="331ed-174">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="331ed-175">Wählen Sie im Menü Kunde die Option **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="331ed-176">Wählen Sie das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="331ed-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="331ed-177">Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.</span><span class="sxs-lookup"><span data-stu-id="331ed-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="331ed-178">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="331ed-178">Next steps</span></span>

- [<span data-ttu-id="331ed-179">Lesen Ihrer Rechnung & Datei "Reconnaissance"</span><span class="sxs-lookup"><span data-stu-id="331ed-179">How to read your bill & recon file</span></span>](read-your-bill.md) 