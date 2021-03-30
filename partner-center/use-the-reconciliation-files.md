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
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730080"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="7c2b9-103">Erfahren Sie, wie Sie die Zeilen Elemente in Ihren Partner Center-Abstimmungs Dateien lesen.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="7c2b9-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="7c2b9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7c2b9-105">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7c2b9-105">Billing admin</span></span>
- <span data-ttu-id="7c2b9-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7c2b9-106">Global admin</span></span>

<span data-ttu-id="7c2b9-107">Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="7c2b9-108">Zu den Zeilen Element Details zählen Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Lizenzen zu einem Abonnement).</span><span class="sxs-lookup"><span data-stu-id="7c2b9-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="7c2b9-109">Informationen zum Lesen der **Rechnung** finden Sie unter [Lesen der](read-your-bill.md)Rechnung.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="7c2b9-110">Grundlegendes zu Abstimmungs Datei Feldern</span><span class="sxs-lookup"><span data-stu-id="7c2b9-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="7c2b9-111">Grundlegendes zu den Feldern in lizenzbasierten Abstimmungsdateien von Partner Center</span><span class="sxs-lookup"><span data-stu-id="7c2b9-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="7c2b9-112">Grundlegendes zu nutzungsbasierten Abstimmungsdateien und ihren spezifischen Feldern im Partner Center</span><span class="sxs-lookup"><span data-stu-id="7c2b9-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="7c2b9-113">Abstimmungsdateien zur täglich bewerteten Nutzung: Felder</span><span class="sxs-lookup"><span data-stu-id="7c2b9-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="7c2b9-114">Felder für das einmalige kaufen von CSP-Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="7c2b9-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="7c2b9-115">Grundlegendes zu Lade Typen in Abgleich Dateien</span><span class="sxs-lookup"><span data-stu-id="7c2b9-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="7c2b9-116">Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="7c2b9-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="7c2b9-117">Beheben von Formatierungsproblemen</span><span class="sxs-lookup"><span data-stu-id="7c2b9-117">Fix formatting issues</span></span>

<span data-ttu-id="7c2b9-118">Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="7c2b9-119">Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="7c2b9-120">Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:</span><span class="sxs-lookup"><span data-stu-id="7c2b9-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="7c2b9-121">Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="7c2b9-122">Wählen Sie die erste Spalte in der Datei aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="7c2b9-123">Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="7c2b9-124">Wählen Sie im Menüband **Daten** aus, und wählen Sie dann **Text in Spalten** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="7c2b9-125">Wählen Sie im Assistenten einen **Begrenzungs Dateityp** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="7c2b9-126">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="7c2b9-127">Wählen Sie im Feld **Trenn** Zeichen die Option **Komma** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="7c2b9-128">(Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="7c2b9-129">Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="7c2b9-130">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="7c2b9-131">Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="7c2b9-132">Wählen Sie **Fertig stellen** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="7c2b9-133">Programm gesteuertes herunterladen von Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="7c2b9-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="7c2b9-134">Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="7c2b9-135">Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="7c2b9-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="7c2b9-136">Wenn die Datei das Zeilen Limit in Excel überschreitet</span><span class="sxs-lookup"><span data-stu-id="7c2b9-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="7c2b9-137">Wenn Sie eine Abstimmungs Datei herunterladen, aber nicht in Microsoft Excel öffnen können, bedeutet dies wahrscheinlich, dass die Datei mehr Zeilen enthält, als in Excel zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="7c2b9-138">Wenn dies der Fall ist, können Sie eine der folgenden Prozeduren verwenden, um die Datei zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="7c2b9-139">Öffnen Sie eine Datei für die Wiederaufnahme in Power BI</span><span class="sxs-lookup"><span data-stu-id="7c2b9-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="7c2b9-140">Laden Sie die Abstimmungs Datei wie gewohnt herunter.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="7c2b9-141">Laden Sie eine Instanz von Power BI herunter, installieren und öffnen Sie Sie.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="7c2b9-142">Wählen Sie auf der Registerkarte Power BI **Startseite** **Daten erhalten** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="7c2b9-143">Wählen Sie in der Liste der **allgemeinen Datenquellen** die Option **Text/CSV** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="7c2b9-144">Wenn Sie dazu aufgefordert werden, öffnen Sie Ihre Reconnaissance-Datei.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="7c2b9-145">Öffnen einer Datei "Reconnaissance" in einer Excel-Pivottabelle</span><span class="sxs-lookup"><span data-stu-id="7c2b9-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="7c2b9-146">Laden Sie die Abstimmungs Datei wie gewohnt herunter.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="7c2b9-147">Öffnen Sie eine neue Datei in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="7c2b9-148">Wählen Sie auf der Registerkarte **Daten** Daten **erhalten** aus, wählen Sie **aus Datei aus**, und wählen Sie dann **Text/CSV** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="7c2b9-149">Wenn Sie dazu aufgefordert werden, öffnen Sie Ihre Reconnaissance-Datei.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-149">When prompted, open your recon file.</span></span> <span data-ttu-id="7c2b9-150">Ihre Daten werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-150">Your data will appear.</span></span>
5. <span data-ttu-id="7c2b9-151">Wählen Sie im Dropdown Menü **Laden** die Option **Laden in** aus, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="7c2b9-152">Wählen Sie im Dialogfeld **Daten importieren** die Option **pivotfähiger Bericht** aus, um die Datei zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="7c2b9-153">Negativer Betrag angezeigt</span><span class="sxs-lookup"><span data-stu-id="7c2b9-153">Negative amount displayed</span></span>

<span data-ttu-id="7c2b9-154">Möglicherweise wird eine negative Menge in der Abstimmungs Datei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-154">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="7c2b9-155">Dies ist wahrscheinlich auf eine der folgenden Ursachen zurückzuführen:</span><span class="sxs-lookup"><span data-stu-id="7c2b9-155">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="7c2b9-156">Sie haben ihre Anzahl von Lizenzen vor kurzem abgebrochen oder reduziert.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-156">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="7c2b9-157">Sie haben Gutschriften für einen Service License Agreement (SLA) oder für die Azure-Nutzung erhalten.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-157">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="7c2b9-158">Weitere Informationen zu dieser Transaktion finden Sie in Ihrem Attributtyp-Attribut in der Abstimmungs Datei.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-158">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="7c2b9-159">Map-Steuern oder Mehrwertsteuer</span><span class="sxs-lookup"><span data-stu-id="7c2b9-159">Map taxes or VAT</span></span>

<span data-ttu-id="7c2b9-160">So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:</span><span class="sxs-lookup"><span data-stu-id="7c2b9-160">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="7c2b9-161">Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-161">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="7c2b9-162">Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-162">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="7c2b9-163">Abstimmungs Dateien nach Partner itemisieren</span><span class="sxs-lookup"><span data-stu-id="7c2b9-163">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="7c2b9-164">Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-164">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="7c2b9-165">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="7c2b9-165">MPN ID</span></span> | <span data-ttu-id="7c2b9-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c2b9-166">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="7c2b9-167">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="7c2b9-167">MPN ID</span></span> | <span data-ttu-id="7c2b9-168">Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="7c2b9-168">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="7c2b9-169">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="7c2b9-169">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="7c2b9-170">Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="7c2b9-170">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="7c2b9-171">Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-171">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="7c2b9-172">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-172">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="7c2b9-173">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="7c2b9-173">Reseller MPN ID</span></span>

<span data-ttu-id="7c2b9-174">Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-174">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="7c2b9-175">Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID** verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-175">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="7c2b9-176">Wenn der CSP-Partner eine **Reseller MPN-ID** entfernt, wird dieser Wert auf *-1* festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-176">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="7c2b9-177">So können Sie die **Reseller MPN-ID** anzeigen oder aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="7c2b9-177">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="7c2b9-178">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-178">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="7c2b9-179">Wählen Sie im Menü „Partner Center” **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-179">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="7c2b9-180">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-180">Choose the customer from the list.</span></span>
4. <span data-ttu-id="7c2b9-181">Wählen Sie im Menü Kunde die Option **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-181">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="7c2b9-182">Wählen Sie das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-182">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="7c2b9-183">Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.</span><span class="sxs-lookup"><span data-stu-id="7c2b9-183">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7c2b9-184">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7c2b9-184">Next steps</span></span>

- [<span data-ttu-id="7c2b9-185">Lesen Ihrer Rechnung & Datei "Reconnaissance"</span><span class="sxs-lookup"><span data-stu-id="7c2b9-185">How to read your bill & recon file</span></span>](read-your-bill.md) 