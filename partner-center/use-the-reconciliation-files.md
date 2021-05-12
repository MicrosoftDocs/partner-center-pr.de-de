---
title: Verwenden Ihrer Abstimmungsdateien
ms.topic: article
ms.date: 03/26/2021
description: Erfahren Sie mehr über Abstimmungsdateien in Partner Center und wie Sie die detaillierten Zeilenansichten der Gebühren für einen bestimmten Abrechnungszyklus interpretieren.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794954"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="f8966-103">Erfahren Sie, wie Sie die Zeilenelemente in Ihren Partner Center Abstimmungsdateien lesen.</span><span class="sxs-lookup"><span data-stu-id="f8966-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="f8966-104">**Geeignete Rollen:** Abrechnungsadministrator | Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="f8966-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="f8966-105">Sie können Ihre Abstimmungsdateien aus Partner Center herunterladen, um eine detaillierte Zeilenansicht der einzelnen Gebühren in einem Abrechnungszyklus zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="f8966-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="f8966-106">Die Details der Einzelnen enthalten Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. B. das kurzfristige Hinzufügen von Lizenzen zu einem Abonnement).</span><span class="sxs-lookup"><span data-stu-id="f8966-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="f8966-107">Informationen zum Lesen Ihrer **Rechnung** finden Sie unter [Lesen Ihrer Rechnung.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="f8966-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="f8966-108">Grundlegendes zu Abstimmungsdateifeldern</span><span class="sxs-lookup"><span data-stu-id="f8966-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="f8966-109">Grundlegendes zu den Feldern in lizenzbasierten Abstimmungsdateien von Partner Center</span><span class="sxs-lookup"><span data-stu-id="f8966-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="f8966-110">Grundlegendes zu nutzungsbasierten Abstimmungsdateien und ihren spezifischen Feldern im Partner Center</span><span class="sxs-lookup"><span data-stu-id="f8966-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="f8966-111">Abstimmungsdateien zur täglich bewerteten Nutzung: Felder</span><span class="sxs-lookup"><span data-stu-id="f8966-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="f8966-112">Felder für die CSP-Abstimmungsdatei für einmaligen Kauf</span><span class="sxs-lookup"><span data-stu-id="f8966-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="f8966-113">Grundlegendes zu Gebührentypen in Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="f8966-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="f8966-114">Informationen zu den Gebührentypen in Abstimmungsdateien (Spalte **ChargeType)** finden Sie unter Gebührentypen für [Abstimmungsdateien.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="f8966-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="f8966-115">Beheben von Formatierungsproblemen</span><span class="sxs-lookup"><span data-stu-id="f8966-115">Fix formatting issues</span></span>

<span data-ttu-id="f8966-116">Gelegentlich kann eine Abstimmungsdatei Formatierungsprobleme enthalten.</span><span class="sxs-lookup"><span data-stu-id="f8966-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="f8966-117">Dieses Problem kann beispielsweise auftreten, wenn das Gebietsschema "en-US" nicht verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f8966-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="f8966-118">Führen Sie die folgenden Schritte aus, um Formatierungsprobleme in Ihren Abstimmungsdateien zu beheben:</span><span class="sxs-lookup"><span data-stu-id="f8966-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="f8966-119">Öffnen Sie die Abstimmungsdatei (im CSV-Format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="f8966-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="f8966-120">Wählen Sie die erste Spalte in der Datei aus.</span><span class="sxs-lookup"><span data-stu-id="f8966-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="f8966-121">Öffnen Sie den **Assistenten zum Konvertieren von Text in Spalten.**</span><span class="sxs-lookup"><span data-stu-id="f8966-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="f8966-122">Wählen Sie im Menüband **Daten** und dann **Text in Spalten aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="f8966-123">Wählen Sie im Assistenten **Dateityp mit Trennzeichen aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="f8966-124">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="f8966-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="f8966-125">Wählen Sie **im Feld Trennzeichen** die Option **Komma aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="f8966-126">(Wenn **tab** bereits ausgewählt ist, können Sie diese Option aktivieren.) Wählen Sie dann Weiter **aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="f8966-127">Wählen Sie **im Feld Spaltendatenformat** die Option **Date:MDY aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="f8966-128">Klicken Sie anschließend auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="f8966-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="f8966-129">Wählen Sie **im Feld Spaltendatenformat** die Option **Text für** alle Betragsspalten aus.</span><span class="sxs-lookup"><span data-stu-id="f8966-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="f8966-130">Wählen Sie **Fertig stellen** aus.</span><span class="sxs-lookup"><span data-stu-id="f8966-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="f8966-131">Programmgesteuertes Herunterladen von Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="f8966-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="f8966-132">Abstimmungsdateien können sehr groß sein und sind manchmal schwierig herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="f8966-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="f8966-133">Informationen zum programmgesteuerten Herunterladen von Abstimmungsdateien finden Sie unter [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="f8966-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="f8966-134">Wenn Ihre Datei das Zeilenlimit in Excel überschreitet</span><span class="sxs-lookup"><span data-stu-id="f8966-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="f8966-135">Wenn Sie eine Abstimmungsdatei herunterladen, aber nicht in Microsoft Excel öffnen können, bedeutet dies wahrscheinlich, dass die Datei mehr Zeilen enthält, als Excel erlaubt.</span><span class="sxs-lookup"><span data-stu-id="f8966-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="f8966-136">In diesem Fall können Sie eine der folgenden Verfahren verwenden, um die Datei zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="f8966-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="f8966-137">Öffnen Sie eine Recon-Datei in Power BI</span><span class="sxs-lookup"><span data-stu-id="f8966-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="f8966-138">Laden Sie die Abstimmungsdatei wie gewohnt herunter.</span><span class="sxs-lookup"><span data-stu-id="f8966-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="f8966-139">Laden Sie eine Instanz von herunter, installieren Sie sie, und öffnen Power BI.</span><span class="sxs-lookup"><span data-stu-id="f8966-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="f8966-140">Wählen Sie Power BI **Registerkarte Start** die Option **Daten erhalten aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="f8966-141">Wählen Sie in der Liste **common data sources (Allgemeine Datenquellen)** die Option **Text/CSV aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="f8966-142">Öffnen Sie ihre Recon-Datei, wenn Sie dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="f8966-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="f8966-143">Öffnen einer Recon-Datei in einer Excel-Pivottabelle</span><span class="sxs-lookup"><span data-stu-id="f8966-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="f8966-144">Laden Sie die Abstimmungsdatei wie gewohnt herunter.</span><span class="sxs-lookup"><span data-stu-id="f8966-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="f8966-145">Öffnen Sie eine neue Datei in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="f8966-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="f8966-146">Wählen Sie **auf der** Registerkarte Daten die Option **Daten herunterladen** aus, wählen Sie Aus **Datei** aus, und wählen Sie **dann Text/CSV aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="f8966-147">Öffnen Sie ihre Recon-Datei, wenn Sie dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="f8966-147">When prompted, open your recon file.</span></span> <span data-ttu-id="f8966-148">Ihre Daten werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f8966-148">Your data will appear.</span></span>
5. <span data-ttu-id="f8966-149">Wählen **Sie** im Dropdownmenü Laden die Option **Laden in** und dann **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="f8966-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="f8966-150">Wählen **Sie** im Dialogfeld Daten importieren die Option **PivotTable-Bericht** aus, um die Datei zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="f8966-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="f8966-151">Negativer Betrag angezeigt</span><span class="sxs-lookup"><span data-stu-id="f8966-151">Negative amount displayed</span></span>

<span data-ttu-id="f8966-152">Möglicherweise wird in Ihrer Abstimmungsdatei ein negativer Betrag angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f8966-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="f8966-153">Dieses Problem hat häufig eine der folgenden Ursachen:</span><span class="sxs-lookup"><span data-stu-id="f8966-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="f8966-154">Sie haben ihre Anzahl von Lizenzen vor Kurzem gekündigt oder reduziert.</span><span class="sxs-lookup"><span data-stu-id="f8966-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="f8966-155">Sie haben entweder eine Gutschrift für einen Dienstlizenzvertrag (Service License Agreement, SLA) oder für die Azure-Nutzung erhalten.</span><span class="sxs-lookup"><span data-stu-id="f8966-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="f8966-156">Um weitere Informationen über diese Transaktion zu erhalten, überprüfen Sie das Attribut „Gebührentyp“ in Ihrer Abstimmungsdatei.</span><span class="sxs-lookup"><span data-stu-id="f8966-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="f8966-157">Zuordnen von Steuern oder Steuern</span><span class="sxs-lookup"><span data-stu-id="f8966-157">Map taxes or VAT</span></span>

<span data-ttu-id="f8966-158">So ordnen Sie Steuern oder Mehrwertsteuer (USt) Ihrer Rechnung zu:</span><span class="sxs-lookup"><span data-stu-id="f8966-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="f8966-159">Addiert die Spalte **Steuern** aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="f8966-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="f8966-160">Addiert die **Spalte TaxAmount** aus der nutzungsbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="f8966-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="f8966-161">Itemize reconciliation files by partner (Abstimmungsdateien nach Partner auf itemisieren)</span><span class="sxs-lookup"><span data-stu-id="f8966-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="f8966-162">Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch in nutzungsbasierten Abstimmungsdateien verwenden, um die Dateien nach Handelspartner aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="f8966-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="f8966-163">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="f8966-163">MPN ID</span></span> | <span data-ttu-id="f8966-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8966-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="f8966-165">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="f8966-165">MPN ID</span></span> | <span data-ttu-id="f8966-166">Der MPN-Bezeichner (Microsoft Partner Network) des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="f8966-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="f8966-167">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="f8966-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="f8966-168">Der [MPN-Bezeichner des Datensatzhändlers für das Abonnement.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="f8966-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="f8966-169">Dieses Feld entspricht der Reseller-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="f8966-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="f8966-170">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f8966-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="f8966-171">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="f8966-171">Reseller MPN ID</span></span>

<span data-ttu-id="f8966-172">Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird seine **MPN-ID** zweimal aufgeführt, sowohl als **MPN-ID** als auch als **Reseller MPN ID**.</span><span class="sxs-lookup"><span data-stu-id="f8966-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="f8966-173">Wenn ein CSP-Partner über einen Handelspartner ohne **MPN-ID** verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f8966-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="f8966-174">Wenn der CSP-Partner eine **Reseller-MPN-ID** entfernt, wird dieser Wert auf *-1* festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f8966-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="f8966-175">So zeigen Sie die **MPN-ID des Wiederverkäufers an oder aktualisieren sie:**</span><span class="sxs-lookup"><span data-stu-id="f8966-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="f8966-176">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="f8966-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="f8966-177">Wählen Sie im Menü „Partner Center” **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="f8966-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="f8966-178">Wählen Sie den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="f8966-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="f8966-179">Wählen Sie im Kundenmenü Abonnements **aus.**</span><span class="sxs-lookup"><span data-stu-id="f8966-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="f8966-180">Wählen Sie das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="f8966-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="f8966-181">Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.</span><span class="sxs-lookup"><span data-stu-id="f8966-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f8966-182">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f8966-182">Next steps</span></span>

- [<span data-ttu-id="f8966-183">Lesen der Rechnungs- &-Recon-Datei</span><span class="sxs-lookup"><span data-stu-id="f8966-183">How to read your bill & recon file</span></span>](read-your-bill.md) 