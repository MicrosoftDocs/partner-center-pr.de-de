---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 07/08/2019
description: Laden Sie die Kontenabstimmungsdateien aus dem Partner Center herunter, um ausführliche Informationen zu den einzelnen Rechnungspositionen der Gebühren in einem Abrechnungszyklus anzuzeigen.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8fae84790aa84b3c5a006d65a632668a33ac24a7
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820566"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="cb91f-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="cb91f-103">Use the reconciliation files</span></span>

<span data-ttu-id="cb91f-104">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="cb91f-104">**Applies to**</span></span>

-  <span data-ttu-id="cb91f-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="cb91f-105">Partner Center</span></span>
-  <span data-ttu-id="cb91f-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="cb91f-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="cb91f-107">Laden Sie die Kontenabstimmungsdateien aus dem Partner Center herunter, um ausführliche Informationen zu den einzelnen Rechnungspositionen der Gebühren in einem Abrechnungszyklus anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="cb91f-108">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z. B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="cb91f-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="cb91f-109">Formatierungsprobleme</span><span class="sxs-lookup"><span data-stu-id="cb91f-109">Formatting issues</span></span>

<span data-ttu-id="cb91f-110">Gelegentlich kann die Kontenabstimmungsdatei Formatierungsprobleme aufweisen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="cb91f-111">(Dies kann beispielsweise vorkommen, wenn das Gebietsschema EN-US nicht verwendet wird.) Gehen Sie folgendermaßen vor, um diese Probleme zu beheben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="cb91f-112">Öffnen Sie die CSV-Datei in Excel, und wählen Sie die erste Spalte aus.</span><span class="sxs-lookup"><span data-stu-id="cb91f-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="cb91f-113">Klicken Sie auf dem Menüband auf <strong>Daten</strong> und dann auf <strong>Text in Spalten</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="cb91f-114">Wählen Sie im Textkonvertierungs-Assistenten <strong>Dateityp „Getrennt“</strong> aus, und klicken Sie dann auf <strong>Weiter</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="cb91f-115">Wählen Sie im Feld „Trennzeichen“ <strong>Komma</strong> aus.</span><span class="sxs-lookup"><span data-stu-id="cb91f-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="cb91f-116">Wenn <strong>Tabstopp</strong> bereits ausgewählt ist, übernehmen Sie diese Einstellung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="cb91f-117">Wählen Sie <strong>Weiter</strong> aus.</span><span class="sxs-lookup"><span data-stu-id="cb91f-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="cb91f-118">Wählen Sie <strong>im Feld Spaltendaten Format die Option Date: Und klicken Sie dann auf <strong>Weiter.</strong></strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="cb91f-119">Wählen Sie im Feld „Datenformat der Spalten“ für alle Betragsspalten <strong>Text</strong> aus, und klicken Sie dann auf <strong>Fertig stellen</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="cb91f-120">Herunterladen einer großen Datei für das herunterladen</span><span class="sxs-lookup"><span data-stu-id="cb91f-120">Downloading a large recon file</span></span>

<span data-ttu-id="cb91f-121">Das Herunterladen von Dateien kann sehr groß werden und ist manchmal schwierig.</span><span class="sxs-lookup"><span data-stu-id="cb91f-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="cb91f-122">Ein PowerShell-Skript, das Sie beim Herunterladen umfangreicher Datei Dateien unterstützt, finden Sie unter [Get Rechnungs Items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="cb91f-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="cb91f-123">Aufschlüsseln nach Partner</span><span class="sxs-lookup"><span data-stu-id="cb91f-123">Itemize by partner</span></span>


<span data-ttu-id="cb91f-124">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="cb91f-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cb91f-125">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-125">MPN ID</span></span></th>
<th><span data-ttu-id="cb91f-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb91f-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cb91f-127">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="cb91f-128">Die Microsoft Partner Network-ID (MPN) des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="cb91f-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-129">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="cb91f-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="cb91f-130">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="cb91f-131">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb91f-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cb91f-132">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="cb91f-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="cb91f-133">Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Partner Center-Menü <strong>Kunden</strong> und dann den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="cb91f-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="cb91f-134">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="cb91f-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="cb91f-135">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="cb91f-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="cb91f-136">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="cb91f-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="cb91f-137">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="cb91f-138">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="cb91f-139">Lizenzbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="cb91f-139">License-based file fields</span></span>


<span data-ttu-id="cb91f-140">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cb91f-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cb91f-141"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="cb91f-142"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="cb91f-143"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-144">PartnerID</span><span class="sxs-lookup"><span data-stu-id="cb91f-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="cb91f-145">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="cb91f-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="cb91f-146">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="cb91f-147">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="cb91f-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="cb91f-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="cb91f-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-149">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="cb91f-150">Eindeutige Microsoft-ID im GUID-Format, die zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="cb91f-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="cb91f-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="cb91f-152">OrderID</span></span></td>
<td><p><span data-ttu-id="cb91f-153">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="cb91f-154">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="cb91f-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="cb91f-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="cb91f-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="cb91f-157">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cb91f-158">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="cb91f-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="cb91f-159">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="cb91f-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="cb91f-160">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="cb91f-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="cb91f-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="cb91f-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="cb91f-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="cb91f-163">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="cb91f-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="cb91f-164">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="cb91f-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="cb91f-165">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="cb91f-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="cb91f-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="cb91f-167">OfferID</span></span></td>
<td><p><span data-ttu-id="cb91f-168">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="cb91f-168">Unique offer ID.</span></span> <span data-ttu-id="cb91f-169">Standard-Angebot-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="cb91f-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="cb91f-170"><b>Hinweis:</b> Dieser Wert entspricht nicht der Angebots-ID in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="cb91f-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="cb91f-171">Siehe „DurableOfferID“ unten.</span><span class="sxs-lookup"><span data-stu-id="cb91f-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="cb91f-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="cb91f-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="cb91f-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="cb91f-174">Eindeutige dauerhafte Angebot-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="cb91f-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="cb91f-175"><b>Hinweis:</b> Dieser Wert entspricht der Angebots-ID in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="cb91f-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="cb91f-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="cb91f-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="cb91f-177">OfferName</span></span></td>
<td><p><span data-ttu-id="cb91f-178">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="cb91f-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="cb91f-179">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="cb91f-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="cb91f-181">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="cb91f-182">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="cb91f-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="cb91f-183">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cb91f-184">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cb91f-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="cb91f-186">Das Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="cb91f-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="cb91f-187">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cb91f-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="cb91f-188">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb91f-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="cb91f-189">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cb91f-190">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cb91f-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cb91f-192">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="cb91f-193">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="cb91f-194">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cb91f-195">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cb91f-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cb91f-197">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="cb91f-198">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="cb91f-199">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="cb91f-200">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="cb91f-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="cb91f-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="cb91f-202">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-202">The type of charge or adjustment.</span></span> <span data-ttu-id="cb91f-203">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="cb91f-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="cb91f-204">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="cb91f-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="cb91f-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="cb91f-206">Preis pro Arbeitsplatz entsprechend der Preisliste zum Kaufzeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cb91f-207">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="cb91f-208">6,82</span><span class="sxs-lookup"><span data-stu-id="cb91f-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-209">Anzahl</span><span class="sxs-lookup"><span data-stu-id="cb91f-209">Quantity</span></span></td>
<td><p><span data-ttu-id="cb91f-210">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="cb91f-210">Number of seats.</span></span> <span data-ttu-id="cb91f-211">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="cb91f-212">2</span><span class="sxs-lookup"><span data-stu-id="cb91f-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-213">Betrag</span><span class="sxs-lookup"><span data-stu-id="cb91f-213">Amount</span></span></td>
<td><p><span data-ttu-id="cb91f-214">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="cb91f-214">Total of price for quantity.</span></span> <span data-ttu-id="cb91f-215">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="cb91f-216">13,32</span><span class="sxs-lookup"><span data-stu-id="cb91f-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="cb91f-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="cb91f-218">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="cb91f-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="cb91f-219">Produktlizenzen, die in einer Kompetenz oder in Karten oder neuen Abonnements enthalten sind, die für einen Anreiz geeignet sind, enthalten in dieser Spalte ebenfalls einen Rabatt Betrag.</span><span class="sxs-lookup"><span data-stu-id="cb91f-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="cb91f-220">2,32</span><span class="sxs-lookup"><span data-stu-id="cb91f-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-221">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="cb91f-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="cb91f-222">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="cb91f-222">Total before tax.</span></span> <span data-ttu-id="cb91f-223">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="cb91f-224">11</span><span class="sxs-lookup"><span data-stu-id="cb91f-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-225">Steuern</span><span class="sxs-lookup"><span data-stu-id="cb91f-225">Tax</span></span></td>
<td><p><span data-ttu-id="cb91f-226">Steuerbetrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="cb91f-227">0</span><span class="sxs-lookup"><span data-stu-id="cb91f-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="cb91f-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="cb91f-229">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="cb91f-229">Total after tax.</span></span> <span data-ttu-id="cb91f-230">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="cb91f-231">11</span><span class="sxs-lookup"><span data-stu-id="cb91f-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-232">Währung</span><span class="sxs-lookup"><span data-stu-id="cb91f-232">Currency</span></span></td>
<td><p><span data-ttu-id="cb91f-233">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="cb91f-233">Currency type.</span></span> <span data-ttu-id="cb91f-234">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="cb91f-235">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="cb91f-236">EUR</span><span class="sxs-lookup"><span data-stu-id="cb91f-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="cb91f-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="cb91f-238">Name der Organisation des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="cb91f-239">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="cb91f-240">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="cb91f-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="cb91f-241">MPNID</span></span></td>
<td><p><span data-ttu-id="cb91f-242">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="cb91f-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="cb91f-243">4390934</span><span class="sxs-lookup"><span data-stu-id="cb91f-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="cb91f-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="cb91f-245">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb91f-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cb91f-246">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="cb91f-247">4390934</span><span class="sxs-lookup"><span data-stu-id="cb91f-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="cb91f-248">DomainName</span></span></td>
<td><p><span data-ttu-id="cb91f-249">Name der Domäne des Kunden, der zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="cb91f-250">Dieser Name darf nicht verwendet werden, um den Kunden eindeutig zu identifizieren, da der Kunde/Partner die Vanity-/Standarddomäne über das Office 365-Portal aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="cb91f-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="cb91f-251">Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="cb91f-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cb91f-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="cb91f-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="cb91f-254">Spitzname des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="cb91f-254">Subscription nickname.</span></span> <span data-ttu-id="cb91f-255">Wenn kein Spitzname angegeben ist, verwendet Partner Center „OfferName“.</span><span class="sxs-lookup"><span data-stu-id="cb91f-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="cb91f-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="cb91f-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="cb91f-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="cb91f-258">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="cb91f-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="cb91f-259">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="cb91f-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="cb91f-260">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="cb91f-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="cb91f-261">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="cb91f-261">Usage-based file fields</span></span>


<span data-ttu-id="cb91f-262">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="cb91f-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="cb91f-263">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="cb91f-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cb91f-264"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="cb91f-265"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="cb91f-266"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="cb91f-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="cb91f-268">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="cb91f-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="cb91f-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="cb91f-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="cb91f-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="cb91f-271">Partnername.</span><span class="sxs-lookup"><span data-stu-id="cb91f-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="cb91f-272">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="cb91f-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="cb91f-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="cb91f-274">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="cb91f-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="cb91f-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="cb91f-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="cb91f-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="cb91f-277">Name der Organisation des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="cb91f-278">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="cb91f-279">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="cb91f-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="cb91f-280">MPNID</span></span></td>
<td><p><span data-ttu-id="cb91f-281">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="cb91f-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="cb91f-282">4390934</span><span class="sxs-lookup"><span data-stu-id="cb91f-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="cb91f-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="cb91f-284">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb91f-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cb91f-285">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="cb91f-286">4390934</span><span class="sxs-lookup"><span data-stu-id="cb91f-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="cb91f-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="cb91f-288">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="cb91f-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="cb91f-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cb91f-291">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="cb91f-292">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cb91f-293">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="cb91f-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cb91f-295">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="cb91f-296">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="cb91f-297">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="cb91f-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="cb91f-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="cb91f-299">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cb91f-300">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="cb91f-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="cb91f-301">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="cb91f-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="cb91f-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="cb91f-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="cb91f-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="cb91f-304">Spitzname des Dienstangebots.</span><span class="sxs-lookup"><span data-stu-id="cb91f-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="cb91f-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cb91f-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="cb91f-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="cb91f-307">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="cb91f-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="cb91f-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cb91f-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="cb91f-309">OrderID</span></span></td>
<td><p><span data-ttu-id="cb91f-310">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="cb91f-311">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="cb91f-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="cb91f-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="cb91f-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="cb91f-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="cb91f-314">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="cb91f-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="cb91f-315">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="cb91f-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="cb91f-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="cb91f-317">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="cb91f-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="cb91f-318">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="cb91f-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="cb91f-319">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="cb91f-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="cb91f-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="cb91f-321">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="cb91f-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="cb91f-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="cb91f-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-323">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="cb91f-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="cb91f-324">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb91f-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="cb91f-325">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="cb91f-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="cb91f-326">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="cb91f-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-327">Region</span><span class="sxs-lookup"><span data-stu-id="cb91f-327">Region</span></span></td>
<td><p><span data-ttu-id="cb91f-328">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="cb91f-328">The region the usage applies to.</span></span> <span data-ttu-id="cb91f-329">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="cb91f-330">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="cb91f-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-331">SKU</span><span class="sxs-lookup"><span data-stu-id="cb91f-331">SKU</span></span></td>
<td><p><span data-ttu-id="cb91f-332">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="cb91f-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="cb91f-333">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="cb91f-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="cb91f-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="cb91f-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="cb91f-335">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb91f-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="cb91f-336">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="cb91f-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="cb91f-337">1</span><span class="sxs-lookup"><span data-stu-id="cb91f-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="cb91f-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="cb91f-339">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="cb91f-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="cb91f-340">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb91f-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="cb91f-341">11</span><span class="sxs-lookup"><span data-stu-id="cb91f-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="cb91f-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="cb91f-343">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="cb91f-343">Units included as part of the offer.</span></span> <span data-ttu-id="cb91f-344">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="cb91f-345">0</span><span class="sxs-lookup"><span data-stu-id="cb91f-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="cb91f-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="cb91f-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="cb91f-347">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="cb91f-348">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="cb91f-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="cb91f-349">11</span><span class="sxs-lookup"><span data-stu-id="cb91f-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="cb91f-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="cb91f-351">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="cb91f-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="cb91f-352">0,0808 $</span><span class="sxs-lookup"><span data-stu-id="cb91f-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="cb91f-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="cb91f-354">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cb91f-355">0,085 $</span><span class="sxs-lookup"><span data-stu-id="cb91f-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="cb91f-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="cb91f-357">Steuerbetrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="cb91f-358">0,08 $</span><span class="sxs-lookup"><span data-stu-id="cb91f-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="cb91f-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="cb91f-360">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="cb91f-361">0,93 $</span><span class="sxs-lookup"><span data-stu-id="cb91f-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-362">Währung</span><span class="sxs-lookup"><span data-stu-id="cb91f-362">Currency</span></span></td>
<td><p><span data-ttu-id="cb91f-363">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="cb91f-363">Currency type.</span></span> <span data-ttu-id="cb91f-364">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="cb91f-365">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="cb91f-366">EUR</span><span class="sxs-lookup"><span data-stu-id="cb91f-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="cb91f-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="cb91f-368">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-368">Pretax price per unit.</span></span> <span data-ttu-id="cb91f-369">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cb91f-370">0,08 $</span><span class="sxs-lookup"><span data-stu-id="cb91f-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="cb91f-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="cb91f-372">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-372">Post tax price per unit.</span></span> <span data-ttu-id="cb91f-373">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cb91f-374">0,08 $</span><span class="sxs-lookup"><span data-stu-id="cb91f-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="cb91f-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="cb91f-376">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-376">The type of charge or adjustment.</span></span> <span data-ttu-id="cb91f-377">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="cb91f-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="cb91f-378">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="cb91f-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="cb91f-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="cb91f-380">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="cb91f-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="cb91f-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="cb91f-383">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="cb91f-384">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="cb91f-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="cb91f-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="cb91f-386">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="cb91f-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="cb91f-387">Ostasien, Südostasien, Nordeuropa, Westeuropa, USA (Mitte/Norden), USA (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="cb91f-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="cb91f-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="cb91f-389">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="cb91f-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="cb91f-390">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="cb91f-391">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="cb91f-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="cb91f-392">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="cb91f-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="cb91f-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="cb91f-394">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="cb91f-395">EXTERN</span><span class="sxs-lookup"><span data-stu-id="cb91f-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-396">Projekt</span><span class="sxs-lookup"><span data-stu-id="cb91f-396">Project</span></span></td>
<td><p><span data-ttu-id="cb91f-397">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="cb91f-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="cb91f-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="cb91f-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="cb91f-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="cb91f-400">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="cb91f-401">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="cb91f-402">Wenn Sie über ein 25-Service-Paket mit Service Bus-Verbindungen verfügen und an diesem Tag 1 verwendet haben, gibt Ihre tägliche Nutzungs Erklärung für diesen Tag "25 Verbindungen/30 Tage – verwendet: 1,000000 ".</span><span class="sxs-lookup"><span data-stu-id="cb91f-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="cb91f-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="cb91f-404">Eindeutige Microsoft-ID im GUID-Format, die zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="cb91f-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="cb91f-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cb91f-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="cb91f-406">DomainName</span></span></td>
<td><p><span data-ttu-id="cb91f-407">Name der Domäne des Kunden, der zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="cb91f-408">Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="cb91f-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cb91f-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="cb91f-410">Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-410">Unit</span></span></td>
<td><p><span data-ttu-id="cb91f-411">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="cb91f-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="cb91f-412">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="cb91f-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="cb91f-413">Einmalige und wiederkehrende Dateifelder</span><span class="sxs-lookup"><span data-stu-id="cb91f-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cb91f-414">Spalte</span><span class="sxs-lookup"><span data-stu-id="cb91f-414">Column</span></span></th>
<th><span data-ttu-id="cb91f-415">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb91f-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="cb91f-416">PartnerID</span><span class="sxs-lookup"><span data-stu-id="cb91f-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="cb91f-417">Eindeutiger Bezeichner für Microsoft Azure Active Directory-Mandanten für eine bestimmte Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="cb91f-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="cb91f-418">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="cb91f-419">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="cb91f-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-420">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="cb91f-421">Eindeutige Microsoft Azure Active Directory-Mandanten-ID im GUID-Format, die zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-422">Kundenname</span><span class="sxs-lookup"><span data-stu-id="cb91f-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="cb91f-423">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="cb91f-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="cb91f-425">Name der Domäne des Kunden, der zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="cb91f-426">Dieser Name darf nicht verwendet werden, um den Kunden eindeutig zu identifizieren, da der Kunde/Partner die Vanity-/Standarddomäne über das Office 365-Portal aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="cb91f-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="cb91f-427">Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-428">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="cb91f-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="cb91f-429">Das Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-430">Rechnungsnummer</span><span class="sxs-lookup"><span data-stu-id="cb91f-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="cb91f-431">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-432">MPNID</span><span class="sxs-lookup"><span data-stu-id="cb91f-432">MpnId</span></span></td>
<td><p><span data-ttu-id="cb91f-433">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="cb91f-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-434">MPN-ID des Handelspartners</span><span class="sxs-lookup"><span data-stu-id="cb91f-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="cb91f-435">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb91f-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-436">Bestellnummer</span><span class="sxs-lookup"><span data-stu-id="cb91f-436">Order ID</span></span></td>
<td><p><span data-ttu-id="cb91f-437">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft Commerce Platform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="cb91f-438">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-439">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="cb91f-439">Order date</span></span></td>
<td><p><span data-ttu-id="cb91f-440">Das Datum, an dem die Bestellung aufgegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="cb91f-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-441">ProductID</span><span class="sxs-lookup"><span data-stu-id="cb91f-441">ProductId</span></span></td>
<td><p><span data-ttu-id="cb91f-442">Die ID des Produkts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="cb91f-443">SkuId</span></span></td>
<td><p><span data-ttu-id="cb91f-444">Die ID einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="cb91f-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="cb91f-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="cb91f-446">Die ID einer bestimmten Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-446">The ID for a particular Availability.</span></span> <span data-ttu-id="cb91f-447">„Verfügbarkeit“ bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, eine Währung, ein Branchensegment usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="cb91f-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-448">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="cb91f-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="cb91f-449">Der Titel einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="cb91f-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-450">Produktname</span><span class="sxs-lookup"><span data-stu-id="cb91f-450">Product name</span></span></td>
<td><p><span data-ttu-id="cb91f-451">Der Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="cb91f-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="cb91f-453">Der Name des Herausgebers des Produkts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="cb91f-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="cb91f-455">Eindeutige ID dieses Herausgebers.</span><span class="sxs-lookup"><span data-stu-id="cb91f-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-456">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="cb91f-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="cb91f-457">Anzeigename eines Abonnements.</span><span class="sxs-lookup"><span data-stu-id="cb91f-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-458">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="cb91f-459">Eindeutiger Bezeichner eines Abonnements auf der Microsoft Commerce Platform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="cb91f-460">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="cb91f-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="cb91f-461">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="cb91f-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cb91f-463">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-463">Start day of the charges.</span></span> <span data-ttu-id="cb91f-464">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cb91f-466">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-466">End day of the charges.</span></span> <span data-ttu-id="cb91f-467">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-468">Laufzeit und Abrechnungszyklus</span><span class="sxs-lookup"><span data-stu-id="cb91f-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="cb91f-469">Die Laufzeitlänge und der Abrechnungszyklus für den Kauf.</span><span class="sxs-lookup"><span data-stu-id="cb91f-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="cb91f-470">Beispiel: 1 Jahr, monatlich.</span><span class="sxs-lookup"><span data-stu-id="cb91f-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-471">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="cb91f-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="cb91f-472">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-473">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="cb91f-474">Der Preis entsprechend der Preisliste zum Kaufzeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cb91f-475">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-476">Effektiver Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="cb91f-477">Der Preis pro Einheit, nachdem Anpassungen vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-478">Anzahl</span><span class="sxs-lookup"><span data-stu-id="cb91f-478">Quantity</span></span></td>
<td><p><span data-ttu-id="cb91f-479">Anzahl der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="cb91f-479">Number of units.</span></span> <span data-ttu-id="cb91f-480">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-481">Typ der Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-481">Unit type</span></span></td>
<td><p><span data-ttu-id="cb91f-482">Der Typ der Einheit, die gekauft wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="cb91f-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="cb91f-484">Eine Erklärung der geltenden Rabatte.</span><span class="sxs-lookup"><span data-stu-id="cb91f-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-485">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="cb91f-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="cb91f-486">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="cb91f-486">Total before tax.</span></span> <span data-ttu-id="cb91f-487">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-488">Steuern gesamt</span><span class="sxs-lookup"><span data-stu-id="cb91f-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="cb91f-489">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-490">Gesamt</span><span class="sxs-lookup"><span data-stu-id="cb91f-490">Total</span></span></td>
<td><p><span data-ttu-id="cb91f-491">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="cb91f-491">Total after tax.</span></span> <span data-ttu-id="cb91f-492">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-493">Währung</span><span class="sxs-lookup"><span data-stu-id="cb91f-493">Currency</span></span></td>
<td><p><span data-ttu-id="cb91f-494">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="cb91f-494">Currency type.</span></span> <span data-ttu-id="cb91f-495">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="cb91f-496">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="cb91f-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="cb91f-498">Ein alternativer Bezeichner für eine Bestellungs-ID.</span><span class="sxs-lookup"><span data-stu-id="cb91f-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="cb91f-499">Dateifelder zur bewerteten täglichen Nutzung</span><span class="sxs-lookup"><span data-stu-id="cb91f-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cb91f-500">Spalte</span><span class="sxs-lookup"><span data-stu-id="cb91f-500">Column</span></span></th>
<th><span data-ttu-id="cb91f-501">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb91f-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="cb91f-502">PartnerID</span><span class="sxs-lookup"><span data-stu-id="cb91f-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="cb91f-503">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="cb91f-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="cb91f-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="cb91f-505">Partnername.</span><span class="sxs-lookup"><span data-stu-id="cb91f-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-506">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="cb91f-507">Eindeutige Microsoft-ID im GUID-Format, die zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="cb91f-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="cb91f-509">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="cb91f-510">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="cb91f-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="cb91f-512">Der Name der Domäne des Kunden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-512">The customer’s domain name.</span></span> <span data-ttu-id="cb91f-513">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cb91f-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-514">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="cb91f-514">Customer country</span></span></td>
<td><p><span data-ttu-id="cb91f-515">Das Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="cb91f-516">MPNID</span></span></td>
<td><p><span data-ttu-id="cb91f-517">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="cb91f-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-518">MPN-ID des Handelspartners</span><span class="sxs-lookup"><span data-stu-id="cb91f-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="cb91f-519">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb91f-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cb91f-520">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cb91f-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="cb91f-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="cb91f-522">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="cb91f-523">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cb91f-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-524">ProductID</span><span class="sxs-lookup"><span data-stu-id="cb91f-524">ProductId</span></span></td>
<td><p><span data-ttu-id="cb91f-525">Die ID des Produkts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="cb91f-526">SkuId</span></span></td>
<td><p><span data-ttu-id="cb91f-527">Die ID einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="cb91f-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="cb91f-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="cb91f-529">Die ID einer bestimmten Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-529">The ID for a particular Availability.</span></span> <span data-ttu-id="cb91f-530">„Verfügbarkeit“ bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, eine Währung, ein Branchensegment usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="cb91f-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-531">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="cb91f-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="cb91f-532">Der Titel einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="cb91f-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="cb91f-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="cb91f-534">Der Name des Herausgebers.</span><span class="sxs-lookup"><span data-stu-id="cb91f-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="cb91f-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="cb91f-536">Die ID des Herausgebers im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="cb91f-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="cb91f-537">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cb91f-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="cb91f-538">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="cb91f-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="cb91f-539">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="cb91f-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="cb91f-540">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="cb91f-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-541">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="cb91f-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="cb91f-542">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="cb91f-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cb91f-543">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="cb91f-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="cb91f-544">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="cb91f-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cb91f-546">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="cb91f-547">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cb91f-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cb91f-549">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="cb91f-550">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-551">Nutzungsdatum</span><span class="sxs-lookup"><span data-stu-id="cb91f-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="cb91f-552">Datum der Nutzung des Diensts.</span><span class="sxs-lookup"><span data-stu-id="cb91f-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-553">Typ der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="cb91f-554">Der Typ der Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-555">Kategorie der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="cb91f-556">Der Dienst der obersten Ebene für die Nutzung.</span><span class="sxs-lookup"><span data-stu-id="cb91f-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-557">ID der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="cb91f-558">Die ID der verwendeten Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-559">Unterkategorie der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="cb91f-560">Der Typ des Azure-Diensts, der sich auf die Rate auswirken kann.</span><span class="sxs-lookup"><span data-stu-id="cb91f-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-561">Name der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="cb91f-562">Die Maßeinheit für die genutzte Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="cb91f-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-563">Region der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="cb91f-564">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="cb91f-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-565">Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-565">Unit</span></span></td>
<td><p><span data-ttu-id="cb91f-566">Die Einheit des Ressourcennamens.</span><span class="sxs-lookup"><span data-stu-id="cb91f-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-567">Verbrauchte Menge</span><span class="sxs-lookup"><span data-stu-id="cb91f-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="cb91f-568">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="cb91f-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="cb91f-569">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb91f-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-570">Ressourcenspeicherort</span><span class="sxs-lookup"><span data-stu-id="cb91f-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="cb91f-571">Das Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-572">Genutzter Dienst</span><span class="sxs-lookup"><span data-stu-id="cb91f-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="cb91f-573">Der Azure-Plattformdienst, den Sie verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="cb91f-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="cb91f-574">Ressourcen-URI</span><span class="sxs-lookup"><span data-stu-id="cb91f-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="cb91f-575">Der URI der verwendeten Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb91f-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-576">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="cb91f-576">Charge type</span></span></td>
<td><p><span data-ttu-id="cb91f-577">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-577">The type of charge or adjustment.</span></span> <span data-ttu-id="cb91f-578">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cb91f-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-579">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-579">Unit price</span></span></td>
<td><p><span data-ttu-id="cb91f-580">Preis pro Lizenz entsprechend der Preisliste zum Kaufzeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cb91f-581">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-582">Anzahl</span><span class="sxs-lookup"><span data-stu-id="cb91f-582">Quantity</span></span></td>
<td><p><span data-ttu-id="cb91f-583">Anzahl der Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-583">Number of licenses.</span></span> <span data-ttu-id="cb91f-584">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-585">Typ der Einheit</span><span class="sxs-lookup"><span data-stu-id="cb91f-585">Unit type</span></span></td>
<td><p><span data-ttu-id="cb91f-586">Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="cb91f-587">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cb91f-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-588">Abrechnung vor Steuern</span><span class="sxs-lookup"><span data-stu-id="cb91f-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="cb91f-589">Gesamtbetrag vor Steuern.</span><span class="sxs-lookup"><span data-stu-id="cb91f-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-590">Abrechnungswährung</span><span class="sxs-lookup"><span data-stu-id="cb91f-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="cb91f-591">Die Währung in der geografischen Region des Kunden</span><span class="sxs-lookup"><span data-stu-id="cb91f-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-592">Preise vor Steuern gesamt</span><span class="sxs-lookup"><span data-stu-id="cb91f-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="cb91f-593">Die Preise vor Hinzufügen von Steuern.</span><span class="sxs-lookup"><span data-stu-id="cb91f-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-594">Währung der Preise</span><span class="sxs-lookup"><span data-stu-id="cb91f-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="cb91f-595">Die Währung in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="cb91f-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cb91f-596">Dienstinformationen 1</span><span class="sxs-lookup"><span data-stu-id="cb91f-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="cb91f-597">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-598">Dienstinformationen 2</span><span class="sxs-lookup"><span data-stu-id="cb91f-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="cb91f-599">Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cb91f-600">Zusätzliche Infos</span><span class="sxs-lookup"><span data-stu-id="cb91f-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="cb91f-601">Zusätzliche Informationen, die von anderen Spalten nicht abgedeckt werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="cb91f-602">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="cb91f-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="cb91f-603">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Kontenabstimmungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="cb91f-604">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen Rechnung und Kontenabstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie die Kontenabstimmungsdatei nach Gebührentypen filtern, um die Abrechnungsgebühren einer Reihe von Gebührenaufschlüsselungen in der Kontenabstimmungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="cb91f-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="cb91f-605">Sowohl nutzungsbasierte als auch lizenzbasierte Kontenabstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zugehörige Kosten).</span><span class="sxs-lookup"><span data-stu-id="cb91f-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="cb91f-606">Guthaben, Rabatte oder Rückerstattungen, die auf der Rechnung als „Anpassungen“ angezeigt werden, werden nicht in der Kontenabstimmungsdatei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="cb91f-607">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnitt und zugehörigen Gebührentypen, die möglicherweise in den Kontenabstimmungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="cb91f-608"><strong>Beschreibung der Rechnungsgebühr</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-609"><strong>Gebührenbeschreibung der Abstimmungsdatei (Spalte „ChargeType“)</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-610"><strong>Was ist diese Gebühr?</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-611"><strong>Wie ordne ich diese Gebührentypen der Rechnung zu?</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="cb91f-612"><strong>Lizenzbasierte Gebühren</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-613">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="cb91f-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-614">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="cb91f-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="cb91f-615">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-616">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="cb91f-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-617">Anteilige Gebühren werden dem Kunden zurückerstattet, wenn verknüpfte Arbeitsplätze geändert werden.</span><span class="sxs-lookup"><span data-stu-id="cb91f-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-618">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="cb91f-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-619">Regelmäßige Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="cb91f-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-620">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="cb91f-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-621">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Arbeitsplätze geändert werden</span><span class="sxs-lookup"><span data-stu-id="cb91f-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-622">Gebühren bei Stornierung anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="cb91f-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-623">Anteilige Rückerstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="cb91f-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-624">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="cb91f-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-625">Der Typ der Gebühr für ein Abonnement bei Verwendung der jährlichen Abrechnung</span><span class="sxs-lookup"><span data-stu-id="cb91f-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-626">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="cb91f-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-627">Der Typ der Gebühr für ein Abonnement bei Verwendung der monatlichen Abrechnung</span><span class="sxs-lookup"><span data-stu-id="cb91f-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-628">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="cb91f-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-629">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="cb91f-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="cb91f-630">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="cb91f-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-631">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="cb91f-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-632">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="cb91f-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-633">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="cb91f-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="cb91f-634"><strong>Einmalige Gebühren</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="cb91f-635">Neu</span><span class="sxs-lookup"><span data-stu-id="cb91f-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-636">Wird verwendet, wenn ein neuer Kauf erstellt wird</span><span class="sxs-lookup"><span data-stu-id="cb91f-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-637">addmenge</span><span class="sxs-lookup"><span data-stu-id="cb91f-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-638">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach der Erhöhung verwendet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-639">removemenge</span><span class="sxs-lookup"><span data-stu-id="cb91f-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-640">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach der Abnahme verwendet.</span><span class="sxs-lookup"><span data-stu-id="cb91f-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-641">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="cb91f-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-642">Wird verwendet, wenn ein Abonnement abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="cb91f-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-643">Konvertieren</span><span class="sxs-lookup"><span data-stu-id="cb91f-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-644">Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Arbeitsplätze jedoch unverändert bleibt.</span><span class="sxs-lookup"><span data-stu-id="cb91f-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="cb91f-645"><strong>Nutzungsgebühren</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-646">Nutzungsgebühr beim Stornieren bewerten</span><span class="sxs-lookup"><span data-stu-id="cb91f-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-647">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei Kündigung</span><span class="sxs-lookup"><span data-stu-id="cb91f-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="cb91f-648">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-649">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="cb91f-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-650">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="cb91f-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="cb91f-651"><strong>Guthaben</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-652">Ausgleichen einer Position</span><span class="sxs-lookup"><span data-stu-id="cb91f-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-653">Teilweise oder vollständige Rückerstattung für eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="cb91f-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-654">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="cb91f-655">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="cb91f-656"><strong>Nutzungsbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-657">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="cb91f-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-658">Rabatt bei Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="cb91f-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="cb91f-659">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-660">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="cb91f-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-661">Rabatt auf regelmäßige Gebühren</span><span class="sxs-lookup"><span data-stu-id="cb91f-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-662">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="cb91f-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-663">Rabatt bei Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="cb91f-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-664">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="cb91f-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-665">Anfallende Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="cb91f-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="cb91f-666"><strong>Lizenzbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-667"><em>Können auf mehrere Gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="cb91f-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="cb91f-668">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cb91f-669"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="cb91f-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-670"><em>Können auf mehrere Gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="cb91f-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="cb91f-671"><em>Ausnahme: &quot;Ausgleichen einer Position&quot; schließt Steuern bereits ein. Siehe „Guthaben“ oben.</em></span><span class="sxs-lookup"><span data-stu-id="cb91f-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-672">Steuern oder Umsatzsteuern (MwSt.)</span><span class="sxs-lookup"><span data-stu-id="cb91f-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="cb91f-673">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="cb91f-674">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="cb91f-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
