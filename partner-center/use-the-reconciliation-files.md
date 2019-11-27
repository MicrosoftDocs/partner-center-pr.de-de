---
title: Verwenden der Abstimmungs Dateien | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Verwenden Sie Ihre Abstimmungs Dateien, um ausführliche Informationen zu den einzelnen Aufgaben des Partner Centers zu verstehen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384801"
---
# <a name="use-your-reconciliation-files"></a><span data-ttu-id="7836d-103">Verwenden der Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="7836d-103">Use your reconciliation files</span></span>

<span data-ttu-id="7836d-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="7836d-104">Applies to:</span></span>

- <span data-ttu-id="7836d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="7836d-105">Partner Center</span></span>
- <span data-ttu-id="7836d-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="7836d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7836d-107">Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="7836d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="7836d-108">Zu den Zeilen Element Details zählen die Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Arbeitsplätzen zu einem Abonnement).</span><span class="sxs-lookup"><span data-stu-id="7836d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="7836d-109">Geeignete Rollen:</span><span class="sxs-lookup"><span data-stu-id="7836d-109">Appropriate roles:</span></span>

- <span data-ttu-id="7836d-110">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7836d-110">Billing admin</span></span>
- <span data-ttu-id="7836d-111">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7836d-111">Global admin</span></span>

<span data-ttu-id="7836d-112">Informationen zum Lesen der **Rechnung**finden Sie unter [Lesen der](read-your-bill.md)Rechnung.</span><span class="sxs-lookup"><span data-stu-id="7836d-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="7836d-113">Grundlegendes zu Abstimmungs Datei Feldern</span><span class="sxs-lookup"><span data-stu-id="7836d-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="7836d-114">Lizenz basierte Abstimmungs Datei Felder</span><span class="sxs-lookup"><span data-stu-id="7836d-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="7836d-115">Verwendungs basierte Abstimmungs Datei Felder</span><span class="sxs-lookup"><span data-stu-id="7836d-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="7836d-116">Einmalige und wiederkehrende Abstimmungs Datei Felder</span><span class="sxs-lookup"><span data-stu-id="7836d-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="7836d-117">Nutzungs Abgleich-Datei Felder für die tägliche Bewertung</span><span class="sxs-lookup"><span data-stu-id="7836d-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="7836d-118">Grundlegendes zu Lade Typen in Abgleich Dateien</span><span class="sxs-lookup"><span data-stu-id="7836d-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="7836d-119">Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="7836d-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="7836d-120">Beheben von Formatierungsproblemen</span><span class="sxs-lookup"><span data-stu-id="7836d-120">Fix formatting issues</span></span>

<span data-ttu-id="7836d-121">Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten.</span><span class="sxs-lookup"><span data-stu-id="7836d-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="7836d-122">Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="7836d-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="7836d-123">Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:</span><span class="sxs-lookup"><span data-stu-id="7836d-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="7836d-124">Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="7836d-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="7836d-125">Wählen Sie die erste Spalte in der Datei aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="7836d-126">Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**.</span><span class="sxs-lookup"><span data-stu-id="7836d-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="7836d-127">Wählen Sie im Menüband **Daten**aus, und wählen Sie dann **Text in Spalten**aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="7836d-128">Wählen Sie im Assistenten einen **Begrenzungs Dateityp**aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="7836d-129">Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="7836d-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="7836d-130">Wählen Sie im Feld **Trenn** Zeichen die Option **Komma**aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="7836d-131">(Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="7836d-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="7836d-132">Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy**aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="7836d-133">Klicken Sie dann auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="7836d-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="7836d-134">Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="7836d-135">Wählen Sie dann **Fertig**stellen aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="7836d-136">Programm gesteuertes herunterladen von Abstimmungs Dateien</span><span class="sxs-lookup"><span data-stu-id="7836d-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="7836d-137">Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="7836d-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="7836d-138">Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="7836d-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="7836d-139">Map-Steuern oder Mehrwertsteuer</span><span class="sxs-lookup"><span data-stu-id="7836d-139">Map taxes or VAT</span></span>

<span data-ttu-id="7836d-140">So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:</span><span class="sxs-lookup"><span data-stu-id="7836d-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="7836d-141">Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.</span><span class="sxs-lookup"><span data-stu-id="7836d-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="7836d-142">Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.</span><span class="sxs-lookup"><span data-stu-id="7836d-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="7836d-143">Abstimmungs Dateien nach Partner itemisieren</span><span class="sxs-lookup"><span data-stu-id="7836d-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="7836d-144">Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.</span><span class="sxs-lookup"><span data-stu-id="7836d-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="7836d-145">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="7836d-145">MPN ID</span></span> | <span data-ttu-id="7836d-146">Description</span><span class="sxs-lookup"><span data-stu-id="7836d-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="7836d-147">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="7836d-147">MPN ID</span></span> | <span data-ttu-id="7836d-148">Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="7836d-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="7836d-149">MPN-ID des Wiederverkäufers</span><span class="sxs-lookup"><span data-stu-id="7836d-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="7836d-150">Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="7836d-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="7836d-151">Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="7836d-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="7836d-152">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7836d-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="7836d-153">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="7836d-153">Reseller MPN ID</span></span>

<span data-ttu-id="7836d-154">Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="7836d-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="7836d-155">Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID**verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7836d-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="7836d-156">Wenn der CSP-Partner eine **Reseller MPN-ID**entfernt, wird dieser Wert auf *-1*festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7836d-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="7836d-157">So können Sie die **Reseller MPN-ID**anzeigen oder aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="7836d-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="7836d-158">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="7836d-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="7836d-159">Wählen Sie im Menü „Partner Center” **Kunden**.</span><span class="sxs-lookup"><span data-stu-id="7836d-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="7836d-160">Wählen Sie den Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="7836d-161">Wählen Sie im Menü Kunde die Option **Abonnements**aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="7836d-162">Wählen Sie das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="7836d-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="7836d-163">Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.</span><span class="sxs-lookup"><span data-stu-id="7836d-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
