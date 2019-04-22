---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Für eine ausführliche Zeilenelement Ansicht jeder kostenlos in einem Abrechnungszyklus Laden Sie die abstimmungsdateien von Partner Center herunter.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 7022f1e3d26751e66f90db96bf6d881cb2a694d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "59430199"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="21eb2-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="21eb2-103">Use the reconciliation files</span></span>

<span data-ttu-id="21eb2-104">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="21eb2-104">**Applies to**</span></span>

-  <span data-ttu-id="21eb2-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="21eb2-105">Partner Center</span></span>
-  <span data-ttu-id="21eb2-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="21eb2-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="21eb2-107">Für eine ausführliche Zeilenelement Ansicht jeder kostenlos in einem Abrechnungszyklus Laden Sie die abstimmungsdateien von Partner Center herunter.</span><span class="sxs-lookup"><span data-stu-id="21eb2-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="21eb2-108">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z. B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="21eb2-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="21eb2-109">Probleme bei der Formatierung</span><span class="sxs-lookup"><span data-stu-id="21eb2-109">Formatting issues</span></span>

<span data-ttu-id="21eb2-110">Gelegentlich kann die Abstimm Datei Formatierungsprobleme haben.</span><span class="sxs-lookup"><span data-stu-id="21eb2-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="21eb2-111">(Dies kann beispielsweise vorkommen, wenn das Gebietsschema EN-US nicht verwendet wird.) Gehen Sie folgendermaßen vor, um diese Probleme zu beheben.</span><span class="sxs-lookup"><span data-stu-id="21eb2-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="21eb2-112">Öffnen Sie die CSV-Datei in Excel, und wählen Sie die erste Spalte.</span><span class="sxs-lookup"><span data-stu-id="21eb2-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="21eb2-113">Wählen Sie auf dem Menüband <strong>Daten</strong>, und wählen Sie dann <strong>Text in Spalten</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="21eb2-114">Wählen Sie in Text umwandeln-Assistent, <strong>Dateityp getrennt</strong>, und wählen Sie dann <strong>Weiter</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="21eb2-115">Wählen Sie in das Feld mit Trennzeichen, <strong>Komma</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="21eb2-116">Wenn <strong>Registerkarte</strong> ist bereits ausgewählt, lassen Sie es.</span><span class="sxs-lookup"><span data-stu-id="21eb2-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="21eb2-117">Wählen Sie <strong>Weiter</strong> aus.</span><span class="sxs-lookup"><span data-stu-id="21eb2-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="21eb2-118">Wählen Sie in das Feld Spalte Daten Format <strong>Datum: MDY</strong>, und wählen Sie dann <strong>Weiter</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="21eb2-119">Wählen Sie in das Feld Spalte Daten Format <strong>Text</strong> für alle Spalten, und wählen Sie dann Betrag <strong>Fertig stellen</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="21eb2-120">Vom Partner aufschlüsseln</span><span class="sxs-lookup"><span data-stu-id="21eb2-120">Itemize by partner</span></span>


<span data-ttu-id="21eb2-121">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="21eb2-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="21eb2-122">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="21eb2-122">MPN ID</span></span></th>
<th><span data-ttu-id="21eb2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21eb2-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="21eb2-124">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="21eb2-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="21eb2-125">Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="21eb2-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-126">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="21eb2-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="21eb2-127">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="21eb2-128">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="21eb2-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="21eb2-129">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="21eb2-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="21eb2-130">eTo anzeigen oder Aktualisieren der Reseller im Partner Center-Menü wählen <strong>Kunden</strong>, wählen Sie dann aus der Liste der Kunden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="21eb2-131">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="21eb2-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="21eb2-132">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="21eb2-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="21eb2-133">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="21eb2-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="21eb2-134">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="21eb2-135">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="21eb2-136">Lizenz-Datei-Felder</span><span class="sxs-lookup"><span data-stu-id="21eb2-136">License-based file fields</span></span>


<span data-ttu-id="21eb2-137">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus Partner Center.</span><span class="sxs-lookup"><span data-stu-id="21eb2-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="21eb2-138"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-138"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="21eb2-139"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-139"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="21eb2-140"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-140"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-141">PartnerID</span><span class="sxs-lookup"><span data-stu-id="21eb2-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="21eb2-142">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="21eb2-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="21eb2-143">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="21eb2-144">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="21eb2-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="21eb2-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="21eb2-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="21eb2-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="21eb2-147">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="21eb2-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="21eb2-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="21eb2-149">OrderID</span></span></td>
<td><p><span data-ttu-id="21eb2-150">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="21eb2-151">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="21eb2-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="21eb2-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="21eb2-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="21eb2-154">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="21eb2-155">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="21eb2-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="21eb2-156">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="21eb2-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="21eb2-157">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="21eb2-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="21eb2-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="21eb2-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="21eb2-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="21eb2-160">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="21eb2-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="21eb2-161">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="21eb2-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="21eb2-162">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="21eb2-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="21eb2-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="21eb2-164">OfferID</span></span></td>
<td><p><span data-ttu-id="21eb2-165">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="21eb2-165">Unique offer ID.</span></span> <span data-ttu-id="21eb2-166">Standard-Angebot-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="21eb2-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="21eb2-167"><b>Hinweis</b>: Dieser Wert entspricht nicht den Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="21eb2-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="21eb2-168">Siehe DurableOfferID unten.</span><span class="sxs-lookup"><span data-stu-id="21eb2-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="21eb2-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="21eb2-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="21eb2-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="21eb2-171">Eindeutige dauerhafte Angebot-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="21eb2-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="21eb2-172"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="21eb2-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="21eb2-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="21eb2-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="21eb2-174">OfferName</span></span></td>
<td><p><span data-ttu-id="21eb2-175">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="21eb2-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="21eb2-176">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="21eb2-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="21eb2-178">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="21eb2-179">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="21eb2-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="21eb2-180">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="21eb2-181">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="21eb2-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="21eb2-183">Die Abonnement-Enddatum: 12 Monate + X Tage nach dem Startdatum (Partner Abrechnungsdatum in Anpassung an) oder 12 Monate ab Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="21eb2-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="21eb2-184">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="21eb2-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="21eb2-185">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21eb2-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="21eb2-186">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="21eb2-187">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="21eb2-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="21eb2-189">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="21eb2-190">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="21eb2-191">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="21eb2-192">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="21eb2-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="21eb2-194">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="21eb2-195">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="21eb2-196">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="21eb2-197">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="21eb2-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="21eb2-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="21eb2-199">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-199">The type of charge or adjustment.</span></span> <span data-ttu-id="21eb2-200">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="21eb2-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="21eb2-201">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="21eb2-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="21eb2-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="21eb2-203">Preis pro Arbeitsplatz, wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="21eb2-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="21eb2-204">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="21eb2-205">6,82</span><span class="sxs-lookup"><span data-stu-id="21eb2-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-206">Anzahl</span><span class="sxs-lookup"><span data-stu-id="21eb2-206">Quantity</span></span></td>
<td><p><span data-ttu-id="21eb2-207">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="21eb2-207">Number of seats.</span></span> <span data-ttu-id="21eb2-208">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="21eb2-209">2</span><span class="sxs-lookup"><span data-stu-id="21eb2-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-210">Betrag</span><span class="sxs-lookup"><span data-stu-id="21eb2-210">Amount</span></span></td>
<td><p><span data-ttu-id="21eb2-211">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="21eb2-211">Total of price for quantity.</span></span> <span data-ttu-id="21eb2-212">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="21eb2-213">13,32</span><span class="sxs-lookup"><span data-stu-id="21eb2-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="21eb2-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="21eb2-215">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="21eb2-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="21eb2-216">IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</span><span class="sxs-lookup"><span data-stu-id="21eb2-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="21eb2-217">2,32</span><span class="sxs-lookup"><span data-stu-id="21eb2-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-218">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="21eb2-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="21eb2-219">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="21eb2-219">Total before tax.</span></span> <span data-ttu-id="21eb2-220">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="21eb2-221">11</span><span class="sxs-lookup"><span data-stu-id="21eb2-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-222">Steuern</span><span class="sxs-lookup"><span data-stu-id="21eb2-222">Tax</span></span></td>
<td><p><span data-ttu-id="21eb2-223">Der steuerliche Aufwand basierend auf Ihren Markt&#39;steuerbestimmungen s und den jeweiligen Umständen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="21eb2-224">0</span><span class="sxs-lookup"><span data-stu-id="21eb2-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="21eb2-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="21eb2-226">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="21eb2-226">Total after tax.</span></span> <span data-ttu-id="21eb2-227">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="21eb2-228">11</span><span class="sxs-lookup"><span data-stu-id="21eb2-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-229">Währung</span><span class="sxs-lookup"><span data-stu-id="21eb2-229">Currency</span></span></td>
<td><p><span data-ttu-id="21eb2-230">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="21eb2-230">Currency type.</span></span> <span data-ttu-id="21eb2-231">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="21eb2-232">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="21eb2-233">EUR</span><span class="sxs-lookup"><span data-stu-id="21eb2-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="21eb2-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="21eb2-235">Kunden&#39;Organisationsname s, wie im Partner Center gemeldet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="21eb2-236">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="21eb2-237">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="21eb2-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-238">MPNID</span></span></td>
<td><p><span data-ttu-id="21eb2-239">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="21eb2-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="21eb2-240">4390934</span><span class="sxs-lookup"><span data-stu-id="21eb2-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="21eb2-242">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="21eb2-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="21eb2-243">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="21eb2-244">4390934</span><span class="sxs-lookup"><span data-stu-id="21eb2-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="21eb2-245">DomainName</span></span></td>
<td><p><span data-ttu-id="21eb2-246">Kunden&#39;Domain Name, die zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="21eb2-247">Dies sollte nicht verwendet werden, zur eindeutigen Identifizierung des Kunden an, wie die Kunden bzw. des Partners die Vanity/Standard-Domäne über das Office 365-Portal aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="21eb2-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="21eb2-248">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="21eb2-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="21eb2-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="21eb2-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="21eb2-251">Abonnement-Nickname.</span><span class="sxs-lookup"><span data-stu-id="21eb2-251">Subscription nickname.</span></span> <span data-ttu-id="21eb2-252">Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</span><span class="sxs-lookup"><span data-stu-id="21eb2-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="21eb2-253">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="21eb2-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="21eb2-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="21eb2-255">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="21eb2-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="21eb2-256">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="21eb2-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="21eb2-257">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="21eb2-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="21eb2-258">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="21eb2-258">Usage-based file fields</span></span>


<span data-ttu-id="21eb2-259">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="21eb2-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="21eb2-260">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="21eb2-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="21eb2-261"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-261"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="21eb2-262"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-262"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="21eb2-263"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-263"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="21eb2-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="21eb2-265">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="21eb2-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="21eb2-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="21eb2-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="21eb2-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="21eb2-268">Partnername.</span><span class="sxs-lookup"><span data-stu-id="21eb2-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="21eb2-269">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="21eb2-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="21eb2-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="21eb2-271">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="21eb2-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="21eb2-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="21eb2-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="21eb2-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="21eb2-274">Kunden&#39;Organisationsname s, wie im Partner Center gemeldet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="21eb2-275">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="21eb2-276">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="21eb2-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-277">MPNID</span></span></td>
<td><p><span data-ttu-id="21eb2-278">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="21eb2-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="21eb2-279">4390934</span><span class="sxs-lookup"><span data-stu-id="21eb2-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="21eb2-281">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="21eb2-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="21eb2-282">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="21eb2-283">4390934</span><span class="sxs-lookup"><span data-stu-id="21eb2-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="21eb2-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="21eb2-285">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="21eb2-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="21eb2-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="21eb2-288">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="21eb2-289">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="21eb2-290">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="21eb2-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="21eb2-292">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="21eb2-293">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="21eb2-294">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="21eb2-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="21eb2-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="21eb2-296">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="21eb2-297">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="21eb2-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="21eb2-298">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="21eb2-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="21eb2-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="21eb2-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="21eb2-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="21eb2-301">Nickname des Service-Angebots.</span><span class="sxs-lookup"><span data-stu-id="21eb2-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="21eb2-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="21eb2-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="21eb2-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="21eb2-304">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="21eb2-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="21eb2-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="21eb2-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="21eb2-306">OrderID</span></span></td>
<td><p><span data-ttu-id="21eb2-307">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="21eb2-308">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="21eb2-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="21eb2-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="21eb2-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="21eb2-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="21eb2-311">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="21eb2-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="21eb2-312">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="21eb2-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="21eb2-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="21eb2-314">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="21eb2-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="21eb2-315">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="21eb2-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="21eb2-316">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="21eb2-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="21eb2-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="21eb2-318">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="21eb2-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="21eb2-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="21eb2-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-320">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="21eb2-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="21eb2-321">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="21eb2-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="21eb2-322">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="21eb2-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="21eb2-323">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="21eb2-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-324">Region</span><span class="sxs-lookup"><span data-stu-id="21eb2-324">Region</span></span></td>
<td><p><span data-ttu-id="21eb2-325">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="21eb2-325">The region the usage applies to.</span></span> <span data-ttu-id="21eb2-326">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="21eb2-327">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="21eb2-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-328">SKU</span><span class="sxs-lookup"><span data-stu-id="21eb2-328">SKU</span></span></td>
<td><p><span data-ttu-id="21eb2-329">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="21eb2-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="21eb2-330">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="21eb2-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="21eb2-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="21eb2-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="21eb2-332">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="21eb2-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="21eb2-333">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="21eb2-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="21eb2-334">1</span><span class="sxs-lookup"><span data-stu-id="21eb2-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="21eb2-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="21eb2-336">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="21eb2-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="21eb2-337">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="21eb2-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="21eb2-338">11</span><span class="sxs-lookup"><span data-stu-id="21eb2-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="21eb2-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="21eb2-340">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="21eb2-340">Units included as part of the offer.</span></span> <span data-ttu-id="21eb2-341">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="21eb2-342">0</span><span class="sxs-lookup"><span data-stu-id="21eb2-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="21eb2-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="21eb2-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="21eb2-344">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="21eb2-345">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="21eb2-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="21eb2-346">11</span><span class="sxs-lookup"><span data-stu-id="21eb2-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="21eb2-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="21eb2-348">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="21eb2-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="21eb2-349">0,0808 $</span><span class="sxs-lookup"><span data-stu-id="21eb2-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="21eb2-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="21eb2-351">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="21eb2-352">0,085 $</span><span class="sxs-lookup"><span data-stu-id="21eb2-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="21eb2-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="21eb2-354">Der steuerliche Aufwand basierend auf Ihren Markt&#39;steuerbestimmungen s und den jeweiligen Umständen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="21eb2-355">0,08 $</span><span class="sxs-lookup"><span data-stu-id="21eb2-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="21eb2-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="21eb2-357">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="21eb2-358">0,93 $</span><span class="sxs-lookup"><span data-stu-id="21eb2-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-359">Währung</span><span class="sxs-lookup"><span data-stu-id="21eb2-359">Currency</span></span></td>
<td><p><span data-ttu-id="21eb2-360">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="21eb2-360">Currency type.</span></span> <span data-ttu-id="21eb2-361">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="21eb2-362">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="21eb2-363">EUR</span><span class="sxs-lookup"><span data-stu-id="21eb2-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="21eb2-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="21eb2-365">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="21eb2-365">Pretax price per unit.</span></span> <span data-ttu-id="21eb2-366">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="21eb2-367">0,08 $</span><span class="sxs-lookup"><span data-stu-id="21eb2-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="21eb2-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="21eb2-369">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="21eb2-369">Post tax price per unit.</span></span> <span data-ttu-id="21eb2-370">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="21eb2-371">0,08 $</span><span class="sxs-lookup"><span data-stu-id="21eb2-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="21eb2-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="21eb2-373">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-373">The type of charge or adjustment.</span></span> <span data-ttu-id="21eb2-374">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="21eb2-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="21eb2-375">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="21eb2-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="21eb2-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="21eb2-377">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="21eb2-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="21eb2-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="21eb2-380">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="21eb2-381">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="21eb2-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="21eb2-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="21eb2-383">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="21eb2-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="21eb2-384">Ostasien, Südostasien, Nordeuropa, Westeuropa, USA (Mitte/Norden), USA (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="21eb2-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="21eb2-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="21eb2-386">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="21eb2-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="21eb2-387">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="21eb2-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="21eb2-388">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="21eb2-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="21eb2-389">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="21eb2-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="21eb2-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="21eb2-391">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="21eb2-392">EXTERN</span><span class="sxs-lookup"><span data-stu-id="21eb2-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-393">Projekt</span><span class="sxs-lookup"><span data-stu-id="21eb2-393">Project</span></span></td>
<td><p><span data-ttu-id="21eb2-394">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="21eb2-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="21eb2-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="21eb2-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="21eb2-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="21eb2-397">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="21eb2-398">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="21eb2-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="21eb2-399">Wenn Sie ein 25-Paket von Service Bus-Verbindungen, die bereitgestellt mussten, und Sie haben 1 während des Tages verwendet, würde Ihre Anweisung zur täglichen Nutzung für diesen Tag angeben "25 Verbindungen / 30 Tage – verwendet: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="21eb2-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="21eb2-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="21eb2-401">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="21eb2-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="21eb2-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="21eb2-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="21eb2-403">DomainName</span></span></td>
<td><p><span data-ttu-id="21eb2-404">Kunden&#39;Domain Name, die zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="21eb2-405">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="21eb2-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="21eb2-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="21eb2-407">Einheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-407">Unit</span></span></td>
<td><p><span data-ttu-id="21eb2-408">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="21eb2-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="21eb2-409">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="21eb2-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="21eb2-410">Einmalige Ausführungen und zeitplanserien Dateifelder</span><span class="sxs-lookup"><span data-stu-id="21eb2-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="21eb2-411">Column</span><span class="sxs-lookup"><span data-stu-id="21eb2-411">Column</span></span></th>
<th><span data-ttu-id="21eb2-412">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21eb2-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="21eb2-413">PartnerID</span><span class="sxs-lookup"><span data-stu-id="21eb2-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="21eb2-414">Eindeutiger Bezeichner für Microsoft Azure Active Directory-Mandanten für eine bestimmte Entität Abrechnung, im GUID-Format '.</span><span class="sxs-lookup"><span data-stu-id="21eb2-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="21eb2-415">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="21eb2-416">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="21eb2-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-417">Kunden-Id</span><span class="sxs-lookup"><span data-stu-id="21eb2-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="21eb2-418">Eindeutige Microsoft Azure Active Directory-Mandanten-ID im GUID-Format, die zum Identifizieren des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-419">Kundenname</span><span class="sxs-lookup"><span data-stu-id="21eb2-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="21eb2-420">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="21eb2-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="21eb2-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="21eb2-422">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="21eb2-423">Dies sollte nicht verwendet werden, zur eindeutigen Identifizierung des Kunden an, wie die Kunden bzw. des Partners die Vanity/Standard-Domäne über das Office 365-Portal aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="21eb2-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="21eb2-424">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-425">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="21eb2-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="21eb2-426">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-427">Rechnungsnummer</span><span class="sxs-lookup"><span data-stu-id="21eb2-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="21eb2-428">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-429">MPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-429">MpnId</span></span></td>
<td><p><span data-ttu-id="21eb2-430">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="21eb2-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="21eb2-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="21eb2-432">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="21eb2-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-433">Bestellnummer</span><span class="sxs-lookup"><span data-stu-id="21eb2-433">Order ID</span></span></td>
<td><p><span data-ttu-id="21eb2-434">Eindeutiger Bezeichner für einen Auftrag in Microsoft Commerce-Plattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="21eb2-435">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-436">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="21eb2-436">Order date</span></span></td>
<td><p><span data-ttu-id="21eb2-437">Der Zeitpunkt der Auftragserstellung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-438">ProductID</span><span class="sxs-lookup"><span data-stu-id="21eb2-438">ProductId</span></span></td>
<td><p><span data-ttu-id="21eb2-439">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-440">SkuID</span><span class="sxs-lookup"><span data-stu-id="21eb2-440">SkuId</span></span></td>
<td><p><span data-ttu-id="21eb2-441">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="21eb2-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="21eb2-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="21eb2-443">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="21eb2-443">The ID for a particular Availability.</span></span> <span data-ttu-id="21eb2-444">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="21eb2-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-445">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="21eb2-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="21eb2-446">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="21eb2-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-447">Produktname</span><span class="sxs-lookup"><span data-stu-id="21eb2-447">Product name</span></span></td>
<td><p><span data-ttu-id="21eb2-448">Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="21eb2-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="21eb2-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="21eb2-450">Der Name des Verlegers des Produkts.</span><span class="sxs-lookup"><span data-stu-id="21eb2-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="21eb2-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="21eb2-452">Eindeutige ID für diesen Verleger.</span><span class="sxs-lookup"><span data-stu-id="21eb2-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-453">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="21eb2-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="21eb2-454">Der Anzeigename eines Abonnements.</span><span class="sxs-lookup"><span data-stu-id="21eb2-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-455">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="21eb2-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="21eb2-456">Eindeutiger Bezeichner für ein Abonnement in Microsoft Commerce-Plattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="21eb2-457">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="21eb2-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="21eb2-458">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="21eb2-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="21eb2-460">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-460">Start day of the charges.</span></span> <span data-ttu-id="21eb2-461">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="21eb2-463">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-463">End day of the charges.</span></span> <span data-ttu-id="21eb2-464">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-465">Begriff und Billingcycle</span><span class="sxs-lookup"><span data-stu-id="21eb2-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="21eb2-466">Die Dauer und dem Abrechnungszyklus für den Kauf.</span><span class="sxs-lookup"><span data-stu-id="21eb2-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="21eb2-467">Z. B. "1 Jahr, monatliche."</span><span class="sxs-lookup"><span data-stu-id="21eb2-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-468">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="21eb2-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="21eb2-469">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-470">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="21eb2-471">Der Preis der Pricelist zum Zeitpunkt des Kaufs, veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="21eb2-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="21eb2-472">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-473">Effektive Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="21eb2-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="21eb2-474">Der Preis nach Anpassungen vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-475">Anzahl</span><span class="sxs-lookup"><span data-stu-id="21eb2-475">Quantity</span></span></td>
<td><p><span data-ttu-id="21eb2-476">Anzahl der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="21eb2-476">Number of units.</span></span> <span data-ttu-id="21eb2-477">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-478">Unit-Typ</span><span class="sxs-lookup"><span data-stu-id="21eb2-478">Unit type</span></span></td>
<td><p><span data-ttu-id="21eb2-479">Der Typ der Einheit gekauft wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="21eb2-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="21eb2-481">Eine Erklärung der Rabatt gilt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-482">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="21eb2-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="21eb2-483">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="21eb2-483">Total before tax.</span></span> <span data-ttu-id="21eb2-484">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-485">Gesamte steuern</span><span class="sxs-lookup"><span data-stu-id="21eb2-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="21eb2-486">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="21eb2-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-487">Gesamt</span><span class="sxs-lookup"><span data-stu-id="21eb2-487">Total</span></span></td>
<td><p><span data-ttu-id="21eb2-488">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="21eb2-488">Total after tax.</span></span> <span data-ttu-id="21eb2-489">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-490">Währung</span><span class="sxs-lookup"><span data-stu-id="21eb2-490">Currency</span></span></td>
<td><p><span data-ttu-id="21eb2-491">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="21eb2-491">Currency type.</span></span> <span data-ttu-id="21eb2-492">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="21eb2-493">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="21eb2-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="21eb2-495">Ein alternativer Bezeichner, der eine Auftrags-ID.</span><span class="sxs-lookup"><span data-stu-id="21eb2-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="21eb2-496">Täglich anteilig Datei verwendungsfelder</span><span class="sxs-lookup"><span data-stu-id="21eb2-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="21eb2-497">Column</span><span class="sxs-lookup"><span data-stu-id="21eb2-497">Column</span></span></th>
<th><span data-ttu-id="21eb2-498">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21eb2-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="21eb2-499">PartnerID</span><span class="sxs-lookup"><span data-stu-id="21eb2-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="21eb2-500">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="21eb2-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="21eb2-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="21eb2-502">Partnername.</span><span class="sxs-lookup"><span data-stu-id="21eb2-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-503">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="21eb2-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="21eb2-504">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="21eb2-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="21eb2-506">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="21eb2-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="21eb2-507">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="21eb2-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="21eb2-509">Domänenname des Kunden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-509">The customer’s domain name.</span></span> <span data-ttu-id="21eb2-510">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="21eb2-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-511">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="21eb2-511">Customer country</span></span></td>
<td><p><span data-ttu-id="21eb2-512">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-513">MPNID</span></span></td>
<td><p><span data-ttu-id="21eb2-514">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="21eb2-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-515">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="21eb2-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="21eb2-516">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="21eb2-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="21eb2-517">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="21eb2-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="21eb2-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="21eb2-519">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="21eb2-520">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="21eb2-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-521">ProductID</span><span class="sxs-lookup"><span data-stu-id="21eb2-521">ProductId</span></span></td>
<td><p><span data-ttu-id="21eb2-522">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-523">SkuID</span><span class="sxs-lookup"><span data-stu-id="21eb2-523">SkuId</span></span></td>
<td><p><span data-ttu-id="21eb2-524">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="21eb2-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="21eb2-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="21eb2-526">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="21eb2-526">The ID for a particular Availability.</span></span> <span data-ttu-id="21eb2-527">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="21eb2-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-528">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="21eb2-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="21eb2-529">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="21eb2-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="21eb2-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="21eb2-531">Der Name des Verlegers.</span><span class="sxs-lookup"><span data-stu-id="21eb2-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="21eb2-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="21eb2-533">Die ID des Verlegers, im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="21eb2-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="21eb2-534">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="21eb2-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="21eb2-535">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="21eb2-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="21eb2-536">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="21eb2-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="21eb2-537">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="21eb2-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-538">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="21eb2-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="21eb2-539">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="21eb2-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="21eb2-540">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="21eb2-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="21eb2-541">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="21eb2-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="21eb2-543">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="21eb2-544">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="21eb2-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="21eb2-546">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="21eb2-547">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-548">Nutzungsdatum</span><span class="sxs-lookup"><span data-stu-id="21eb2-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="21eb2-549">Datum der Nutzung des Diensts.</span><span class="sxs-lookup"><span data-stu-id="21eb2-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-550">Typ der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="21eb2-551">Der Typ der Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="21eb2-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-552">Kategorie der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="21eb2-553">Dienst der obersten Ebene für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="21eb2-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-554">Id der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="21eb2-555">Die ID der Verbrauchseinheit, die verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-556">Unterkategorie der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="21eb2-557">Der Typ des Azure-Dienst, der auf den Tarif auswirken kann.</span><span class="sxs-lookup"><span data-stu-id="21eb2-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-558">Name der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="21eb2-559">Die Maßeinheit für die genutzte Verbrauchseinheit an.</span><span class="sxs-lookup"><span data-stu-id="21eb2-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-560">Region der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="21eb2-561">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="21eb2-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-562">Einheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-562">Unit</span></span></td>
<td><p><span data-ttu-id="21eb2-563">Die Einheit der Name der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21eb2-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-564">Verbrauchte Menge</span><span class="sxs-lookup"><span data-stu-id="21eb2-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="21eb2-565">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="21eb2-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="21eb2-566">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="21eb2-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-567">Ressourcenspeicherort</span><span class="sxs-lookup"><span data-stu-id="21eb2-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="21eb2-568">Das Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-569">Genutzter Dienst</span><span class="sxs-lookup"><span data-stu-id="21eb2-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="21eb2-570">Der Azure-Plattform-Dienst, den Sie verwendet.</span><span class="sxs-lookup"><span data-stu-id="21eb2-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-571">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="21eb2-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="21eb2-572">Die Ressourcengruppe, in der die bereitgestellte Verbrauchseinheit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-573">Ressourcen-URI</span><span class="sxs-lookup"><span data-stu-id="21eb2-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="21eb2-574">Der URI der Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-575">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="21eb2-575">Charge type</span></span></td>
<td><p><span data-ttu-id="21eb2-576">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-576">The type of charge or adjustment.</span></span> <span data-ttu-id="21eb2-577">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="21eb2-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-578">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="21eb2-578">Unit price</span></span></td>
<td><p><span data-ttu-id="21eb2-579">Preis pro-Lizenz, wie in der Pricelist zum Zeitpunkt des Kaufs veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="21eb2-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="21eb2-580">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-581">Anzahl</span><span class="sxs-lookup"><span data-stu-id="21eb2-581">Quantity</span></span></td>
<td><p><span data-ttu-id="21eb2-582">Anzahl der Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-582">Number of licenses.</span></span> <span data-ttu-id="21eb2-583">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-584">Unit-Typ</span><span class="sxs-lookup"><span data-stu-id="21eb2-584">Unit type</span></span></td>
<td><p><span data-ttu-id="21eb2-585">Der Typ der Einheit, die die Verbrauchseinheit in Rechnung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="21eb2-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="21eb2-586">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="21eb2-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-587">Die Abrechnung vor Steuern</span><span class="sxs-lookup"><span data-stu-id="21eb2-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="21eb2-588">Die Gesamtmenge vor Steuern.</span><span class="sxs-lookup"><span data-stu-id="21eb2-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-589">Rechnungswährung</span><span class="sxs-lookup"><span data-stu-id="21eb2-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="21eb2-590">Die Währung in geografischen Region des Kunden</span><span class="sxs-lookup"><span data-stu-id="21eb2-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-591">Preise vor Steuern gesamt</span><span class="sxs-lookup"><span data-stu-id="21eb2-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="21eb2-592">Die Preise, steuern hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-593">Preise von Währung</span><span class="sxs-lookup"><span data-stu-id="21eb2-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="21eb2-594">Die Währung, in der Pricelist werden soll.</span><span class="sxs-lookup"><span data-stu-id="21eb2-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-595">Dienstinformationen 1</span><span class="sxs-lookup"><span data-stu-id="21eb2-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="21eb2-596">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-597">Dienstinformationen 2</span><span class="sxs-lookup"><span data-stu-id="21eb2-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="21eb2-598">Ein legacyfeld, die optionale dienstspezifische Metadaten erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="21eb2-599">Tags</span><span class="sxs-lookup"><span data-stu-id="21eb2-599">Tags</span></span></td>
<td><p><span data-ttu-id="21eb2-600">Tags, die Sie das Messgerät in der Reihenfolge zum Gruppieren von abrechnungsdatensätzen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="21eb2-601">Beispielsweise können Sie Tags verwenden, um Kosten nach den Abteilungen zu unterteilen, die die Verbrauchseinheit nutzen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="21eb2-602">Zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="21eb2-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="21eb2-603">Zusätzliche Informationen in anderen Spalten nicht behandelt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="21eb2-604">Zuordnung der Gebühren zwischen Rechnung und abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="21eb2-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="21eb2-605">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="21eb2-606">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="21eb2-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="21eb2-607">Sowohl nutzungsbasierte als auch lizenzbasierte Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zusammenhängende Kosten).</span><span class="sxs-lookup"><span data-stu-id="21eb2-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="21eb2-608">Guthaben, Rabatte oder Erstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungsdatei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="21eb2-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="21eb2-609">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnitt und zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="21eb2-610"><strong>Beschreibung der Rechnungsgebühren</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-610"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-611"><strong>Abstimmung DateiBeschreibung (ChargeType-Spalte)</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-611"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-612"><strong>Was diese Gebühr ist?</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-612"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-613"><strong>Wie ordne ich dieser Gebührentypen zur Rechnung zu?</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-613"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="21eb2-614"><strong>Lizenzbasierte Gebühren</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-614"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-615">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="21eb2-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-616">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="21eb2-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="21eb2-617">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-618">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="21eb2-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-619">Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="21eb2-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-620">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="21eb2-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-621">Periodische Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="21eb2-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-622">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="21eb2-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-623">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</span><span class="sxs-lookup"><span data-stu-id="21eb2-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-624">Gebühren bei Abbrechen anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="21eb2-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-625">Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="21eb2-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-626">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="21eb2-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-627">Der Typ der Gebühr für ein Abonnement bei Verwendung von jährliche Abrechnung</span><span class="sxs-lookup"><span data-stu-id="21eb2-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-628">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="21eb2-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-629">Der Typ der Gebühr für ein Abonnement bei Verwendung der monatliche Abrechnung</span><span class="sxs-lookup"><span data-stu-id="21eb2-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-630">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="21eb2-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-631">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="21eb2-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="21eb2-632">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="21eb2-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-633">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="21eb2-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-634">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="21eb2-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-635">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="21eb2-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="21eb2-636"><strong>Nutzungsgebühren</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-636"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-637">Nutzungsgebühr beim Abbrechen bewerten</span><span class="sxs-lookup"><span data-stu-id="21eb2-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-638">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</span><span class="sxs-lookup"><span data-stu-id="21eb2-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="21eb2-639">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-640">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="21eb2-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-641">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="21eb2-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-642"><strong>Guthaben</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-642"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-643">Einen Artikel versetzen</span><span class="sxs-lookup"><span data-stu-id="21eb2-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-644">Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="21eb2-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-645">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="21eb2-646">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="21eb2-647"><strong>Verwendungsbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-647"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-648">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="21eb2-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-649">Rabatt auf Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="21eb2-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="21eb2-650">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-651">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="21eb2-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-652">Rabatt auf periodische Gebühren</span><span class="sxs-lookup"><span data-stu-id="21eb2-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-653">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="21eb2-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-654">Rabatt auf Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="21eb2-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-655">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="21eb2-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-656">Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="21eb2-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="21eb2-657"><strong>Lizenzbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-657"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-658"><em>Kann für mehrere gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="21eb2-658"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="21eb2-659">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="21eb2-660"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="21eb2-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-661"><em>Kann für mehrere gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="21eb2-661"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="21eb2-662"><em>Ausnahme: &quot;Ausgleich einer Position&quot; enthält bereits steuern. Finden Sie-Guthaben, oben ein.</em></span><span class="sxs-lookup"><span data-stu-id="21eb2-662"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-663">Steuern oder Umsatzsteuern (Umsatzsteuer)</span><span class="sxs-lookup"><span data-stu-id="21eb2-663">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="21eb2-664">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-664">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="21eb2-665">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="21eb2-665">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
