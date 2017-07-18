---
title: Verwenden der Abstimmungsdateien | Partner Center
description: "Laden Sie die Abgleichungsdateien aus dem PartnerCenter-Dashboard herunter, um detaillierte Rechnungspositionsinformationen für einen Abrechnungszyklus anzuzeigen."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 61e71d4207d9e8ac68ee4fcfc1f0d04282474032
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/19/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="de71f-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="de71f-103">Use the reconciliation files</span></span>

**<span data-ttu-id="de71f-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="de71f-104">Applies to</span></span>**

-  <span data-ttu-id="de71f-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="de71f-105">Partner Center</span></span>
-  <span data-ttu-id="de71f-106">Partner Center für Microsoft Cloud für US-Behörden</span><span class="sxs-lookup"><span data-stu-id="de71f-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="de71f-107">Partner Center für Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="de71f-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="de71f-108">Laden Sie die Abgleichungsdateien aus dem PartnerCenter-Dashboard herunter, um detaillierte Rechnungspositionsinformationen für einen Abrechnungszyklus anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="de71f-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="de71f-109">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z.B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="de71f-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <span data-ttu-id="de71f-110"><a href="" id="itemizebypartner"></a>Aufschlüsseln nach Partner</span><span class="sxs-lookup"><span data-stu-id="de71f-110"><a href="" id="itemizebypartner"></a>Itemize by partner</span></span>


<span data-ttu-id="de71f-111">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="de71f-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="de71f-112">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="de71f-112">MPN ID</span></span></th>
<th><span data-ttu-id="de71f-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de71f-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="de71f-114">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="de71f-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="de71f-115">Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="de71f-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-116">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="de71f-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="de71f-117">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="de71f-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="de71f-118">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="de71f-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="de71f-119">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="de71f-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="de71f-120">Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Menü „Partner Center” <strong>Kunden</strong> aus, und wählen Sie dann den Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="de71f-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="de71f-121">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="de71f-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="de71f-122">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="de71f-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="de71f-123">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="de71f-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="de71f-124">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="de71f-125">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <span data-ttu-id="de71f-126"><a href="" id="licencebasedfiles"></a> Lizenzbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="de71f-126"><a href="" id="licencebasedfiles"></a> License-based file fields</span></span>


<span data-ttu-id="de71f-127">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus PartnerCenter.</span><span class="sxs-lookup"><span data-stu-id="de71f-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="de71f-128">Spalte</span><span class="sxs-lookup"><span data-stu-id="de71f-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="de71f-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de71f-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="de71f-130">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="de71f-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-131">OperatingUnit</span><span class="sxs-lookup"><span data-stu-id="de71f-131">OperatingUnit</span></span></td>
<td><p><span data-ttu-id="de71f-132">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="de71f-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="de71f-133">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="de71f-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="de71f-134">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="de71f-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="de71f-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="de71f-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="de71f-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="de71f-137">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="de71f-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="de71f-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="de71f-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="de71f-139">OrderID</span></span></td>
<td><p><span data-ttu-id="de71f-140">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="de71f-141">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="de71f-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="de71f-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="de71f-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="de71f-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="de71f-144">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="de71f-145">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="de71f-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="de71f-146">Diese ID ist nicht mit der Abonnement-ID in der Partner-Verwaltungskonsole identisch.</span><span class="sxs-lookup"><span data-stu-id="de71f-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="de71f-147">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="de71f-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="de71f-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="de71f-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="de71f-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="de71f-150">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="de71f-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="de71f-151">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="de71f-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="de71f-152">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="de71f-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="de71f-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="de71f-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="de71f-154">OfferID</span></span></td>
<td><p><span data-ttu-id="de71f-155">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="de71f-155">Unique offer ID.</span></span> <span data-ttu-id="de71f-156">Standard-Angebots-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="de71f-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="de71f-157"><b>Hinweis</b>: Dieser Wert entspricht nicht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="de71f-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="de71f-158">Siehe DurableOfferID unten.</span><span class="sxs-lookup"><span data-stu-id="de71f-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="de71f-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="de71f-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="de71f-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="de71f-161">Eindeutige dauerhafte Angebots-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="de71f-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="de71f-162"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="de71f-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="de71f-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="de71f-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="de71f-164">OfferName</span></span></td>
<td><p><span data-ttu-id="de71f-165">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="de71f-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="de71f-166">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="de71f-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="de71f-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="de71f-168">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="de71f-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="de71f-169">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="de71f-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="de71f-170">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="de71f-171">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="de71f-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="de71f-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="de71f-173">Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="de71f-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="de71f-174">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="de71f-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="de71f-175">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de71f-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="de71f-176">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="de71f-177">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="de71f-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="de71f-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="de71f-179">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="de71f-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="de71f-180">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="de71f-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="de71f-181">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="de71f-182">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="de71f-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="de71f-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="de71f-184">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="de71f-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="de71f-185">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="de71f-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="de71f-186">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="de71f-187">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="de71f-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="de71f-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="de71f-189">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="de71f-189">The type of charge or adjustment.</span></span> <span data-ttu-id="de71f-190">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="de71f-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="de71f-191">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="de71f-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="de71f-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="de71f-193">Preis pro Lizenz.</span><span class="sxs-lookup"><span data-stu-id="de71f-193">Price per seat.</span></span> <span data-ttu-id="de71f-194">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="de71f-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="de71f-195">6,82</span><span class="sxs-lookup"><span data-stu-id="de71f-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-196">Menge</span><span class="sxs-lookup"><span data-stu-id="de71f-196">Quantity</span></span></td>
<td><p><span data-ttu-id="de71f-197">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="de71f-197">Number of seats.</span></span> <span data-ttu-id="de71f-198">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="de71f-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="de71f-199">2</span><span class="sxs-lookup"><span data-stu-id="de71f-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-200">Betrag</span><span class="sxs-lookup"><span data-stu-id="de71f-200">Amount</span></span></td>
<td><p><span data-ttu-id="de71f-201">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="de71f-201">Total of price for quantity.</span></span> <span data-ttu-id="de71f-202">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="de71f-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="de71f-203">13,32</span><span class="sxs-lookup"><span data-stu-id="de71f-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="de71f-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="de71f-205">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="de71f-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="de71f-206">IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</span><span class="sxs-lookup"><span data-stu-id="de71f-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="de71f-207">2,32</span><span class="sxs-lookup"><span data-stu-id="de71f-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-208">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="de71f-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="de71f-209">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="de71f-209">Total before tax.</span></span> <span data-ttu-id="de71f-210">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="de71f-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="de71f-211">11</span><span class="sxs-lookup"><span data-stu-id="de71f-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-212">Steuern</span><span class="sxs-lookup"><span data-stu-id="de71f-212">Tax</span></span></td>
<td><p><span data-ttu-id="de71f-213">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="de71f-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="de71f-214">0</span><span class="sxs-lookup"><span data-stu-id="de71f-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="de71f-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="de71f-216">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="de71f-216">Total after tax.</span></span> <span data-ttu-id="de71f-217">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="de71f-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="de71f-218">11</span><span class="sxs-lookup"><span data-stu-id="de71f-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-219">Währung</span><span class="sxs-lookup"><span data-stu-id="de71f-219">Currency</span></span></td>
<td><p><span data-ttu-id="de71f-220">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="de71f-220">Currency type.</span></span> <span data-ttu-id="de71f-221">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="de71f-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="de71f-222">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="de71f-223">EUR</span><span class="sxs-lookup"><span data-stu-id="de71f-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="de71f-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="de71f-225">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="de71f-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="de71f-226">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="de71f-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="de71f-227">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="de71f-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="de71f-228">MPNID</span></span></td>
<td><p><span data-ttu-id="de71f-229">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="de71f-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="de71f-230">4390934</span><span class="sxs-lookup"><span data-stu-id="de71f-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="de71f-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="de71f-232">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="de71f-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="de71f-233">Siehe [Aufschlüsseln nach Partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="de71f-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="de71f-234">4390934</span><span class="sxs-lookup"><span data-stu-id="de71f-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="de71f-235">DomainName</span></span></td>
<td><p><span data-ttu-id="de71f-236">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="de71f-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="de71f-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="de71f-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="de71f-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="de71f-239">Abonnement-Nickname.</span><span class="sxs-lookup"><span data-stu-id="de71f-239">Subscription nickname.</span></span> <span data-ttu-id="de71f-240">Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</span><span class="sxs-lookup"><span data-stu-id="de71f-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="de71f-241">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="de71f-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="de71f-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="de71f-243">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="de71f-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="de71f-244">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="de71f-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="de71f-245">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="de71f-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <span data-ttu-id="de71f-246"><a href="" id="usagebasedfiles"></a>Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="de71f-246"><a href="" id="usagebasedfiles"></a>Usage-based file fields</span></span>


<span data-ttu-id="de71f-247">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="de71f-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="de71f-248">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="de71f-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="de71f-249">Spalte</span><span class="sxs-lookup"><span data-stu-id="de71f-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="de71f-250">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de71f-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="de71f-251">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="de71f-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="de71f-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="de71f-253">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="de71f-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="de71f-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="de71f-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="de71f-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="de71f-256">Partnername.</span><span class="sxs-lookup"><span data-stu-id="de71f-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="de71f-257">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="de71f-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="de71f-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="de71f-259">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="de71f-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="de71f-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="de71f-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="de71f-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="de71f-262">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="de71f-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="de71f-263">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="de71f-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="de71f-264">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="de71f-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="de71f-265">MPNID</span></span></td>
<td><p><span data-ttu-id="de71f-266">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="de71f-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="de71f-267">4390934</span><span class="sxs-lookup"><span data-stu-id="de71f-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="de71f-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="de71f-269">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="de71f-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="de71f-270">Siehe [Aufschlüsseln nach Partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="de71f-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="de71f-271">4390934</span><span class="sxs-lookup"><span data-stu-id="de71f-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="de71f-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="de71f-273">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="de71f-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="de71f-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="de71f-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="de71f-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="de71f-276">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="de71f-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="de71f-277">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="de71f-278">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="de71f-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="de71f-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="de71f-280">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="de71f-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="de71f-281">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="de71f-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="de71f-282">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="de71f-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="de71f-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="de71f-284">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="de71f-285">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="de71f-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="de71f-286">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="de71f-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="de71f-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="de71f-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="de71f-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="de71f-289">Nickname des Service-Angebots.</span><span class="sxs-lookup"><span data-stu-id="de71f-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="de71f-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="de71f-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="de71f-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="de71f-292">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="de71f-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="de71f-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="de71f-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="de71f-294">OrderID</span></span></td>
<td><p><span data-ttu-id="de71f-295">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="de71f-296">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="de71f-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="de71f-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="de71f-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="de71f-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="de71f-299">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="de71f-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="de71f-300">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="de71f-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="de71f-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="de71f-302">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="de71f-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="de71f-303">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="de71f-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="de71f-304">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="de71f-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="de71f-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="de71f-306">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="de71f-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="de71f-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="de71f-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-308">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="de71f-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="de71f-309">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="de71f-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="de71f-310">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="de71f-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="de71f-311">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="de71f-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-312">Region</span><span class="sxs-lookup"><span data-stu-id="de71f-312">Region</span></span></td>
<td><p><span data-ttu-id="de71f-313">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="de71f-313">The region the usage applies to.</span></span> <span data-ttu-id="de71f-314">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="de71f-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="de71f-315">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="de71f-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-316">SKU</span><span class="sxs-lookup"><span data-stu-id="de71f-316">SKU</span></span></td>
<td><p><span data-ttu-id="de71f-317">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="de71f-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="de71f-318">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="de71f-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="de71f-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="de71f-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="de71f-320">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="de71f-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="de71f-321">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="de71f-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="de71f-322">1</span><span class="sxs-lookup"><span data-stu-id="de71f-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="de71f-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="de71f-324">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="de71f-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="de71f-325">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="de71f-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="de71f-326">11</span><span class="sxs-lookup"><span data-stu-id="de71f-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="de71f-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="de71f-328">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="de71f-328">Units included as part of the offer.</span></span> <span data-ttu-id="de71f-329">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="de71f-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="de71f-330">0</span><span class="sxs-lookup"><span data-stu-id="de71f-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="de71f-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="de71f-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="de71f-332">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="de71f-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="de71f-333">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="de71f-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="de71f-334">11</span><span class="sxs-lookup"><span data-stu-id="de71f-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="de71f-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="de71f-336">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="de71f-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="de71f-337">0,0808$</span><span class="sxs-lookup"><span data-stu-id="de71f-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="de71f-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="de71f-339">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="de71f-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="de71f-340">0,085$</span><span class="sxs-lookup"><span data-stu-id="de71f-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="de71f-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="de71f-342">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="de71f-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="de71f-343">0,08$</span><span class="sxs-lookup"><span data-stu-id="de71f-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="de71f-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="de71f-345">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="de71f-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="de71f-346">0,93$</span><span class="sxs-lookup"><span data-stu-id="de71f-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-347">Währung</span><span class="sxs-lookup"><span data-stu-id="de71f-347">Currency</span></span></td>
<td><p><span data-ttu-id="de71f-348">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="de71f-348">Currency type.</span></span> <span data-ttu-id="de71f-349">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="de71f-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="de71f-350">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="de71f-351">EUR</span><span class="sxs-lookup"><span data-stu-id="de71f-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="de71f-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="de71f-353">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="de71f-353">Pretax price per unit.</span></span> <span data-ttu-id="de71f-354">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="de71f-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="de71f-355">0,08$</span><span class="sxs-lookup"><span data-stu-id="de71f-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="de71f-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="de71f-357">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="de71f-357">Post tax price per unit.</span></span> <span data-ttu-id="de71f-358">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="de71f-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="de71f-359">0,08$</span><span class="sxs-lookup"><span data-stu-id="de71f-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="de71f-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="de71f-361">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="de71f-361">The type of charge or adjustment.</span></span> <span data-ttu-id="de71f-362">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="de71f-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="de71f-363">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="de71f-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="de71f-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="de71f-365">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="de71f-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="de71f-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="de71f-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="de71f-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="de71f-368">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="de71f-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="de71f-369">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="de71f-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="de71f-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="de71f-371">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="de71f-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="de71f-372">Ostasien, Südostasien, Nordeuropa, Westeuropa, Vereinigte Staaten (Mitte/Norden), Vereinigte Staaten (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="de71f-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="de71f-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="de71f-374">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="de71f-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="de71f-375">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="de71f-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="de71f-376">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="de71f-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="de71f-377">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="de71f-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="de71f-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="de71f-379">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="de71f-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="de71f-380">EXTERN</span><span class="sxs-lookup"><span data-stu-id="de71f-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-381">Projekt</span><span class="sxs-lookup"><span data-stu-id="de71f-381">Project</span></span></td>
<td><p><span data-ttu-id="de71f-382">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="de71f-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="de71f-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="de71f-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="de71f-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="de71f-385">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="de71f-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="de71f-386">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="de71f-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="de71f-387">Wenn ein Paket von 25 ServiceBus-Verbindungen bereitgestellt wurden und Sie an diesem Tag 1 genutzt haben, wird als tägliche Nutzung für diesen Tag „25 Verbindungen/30 Tage – Verwendet: 1,000000“ angegeben.</span><span class="sxs-lookup"><span data-stu-id="de71f-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="de71f-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="de71f-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="de71f-389">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="de71f-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="de71f-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="de71f-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="de71f-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="de71f-391">DomainName</span></span></td>
<td><p><span data-ttu-id="de71f-392">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="de71f-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="de71f-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="de71f-393">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <span data-ttu-id="de71f-394"><a href="" id="charge_types"></a>Siehe Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</span><span class="sxs-lookup"><span data-stu-id="de71f-394"><a href="" id="charge_types"></a>Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="de71f-395">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="de71f-395">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="de71f-396">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="de71f-396">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="de71f-397">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnittund zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="de71f-397">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="de71f-398">Beschreibung der Rechnungsgebühr</span><span class="sxs-lookup"><span data-stu-id="de71f-398">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="de71f-399">Gebührenbeschreibung der Abstimmungsdatei (ChargeType-Spalte)</span><span class="sxs-lookup"><span data-stu-id="de71f-399">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="de71f-400">Um welche Gebühr handelt es sich?</span><span class="sxs-lookup"><span data-stu-id="de71f-400">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="de71f-401">Wie ordne ich diese ChargeTypes der Rechnung zu?</span><span class="sxs-lookup"><span data-stu-id="de71f-401">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="de71f-402">Laufende Gebühren</span><span class="sxs-lookup"><span data-stu-id="de71f-402">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="de71f-403">Instanz anteilig stornieren</span><span class="sxs-lookup"><span data-stu-id="de71f-403">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-404">Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="de71f-404">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="de71f-405">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-405">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-406">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="de71f-406">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-407">Periodische Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="de71f-407">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-408">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="de71f-408">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-409">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</span><span class="sxs-lookup"><span data-stu-id="de71f-409">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-410">Gebühren bei Abbrechen anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="de71f-410">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-411">Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="de71f-411">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-412">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="de71f-412">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-413">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="de71f-413">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-414">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="de71f-414">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-415">Anfängliche Gebühr für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="de71f-415">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-416">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="de71f-416">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-417">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="de71f-417">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-418">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="de71f-418">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-419">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="de71f-419">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="de71f-420">Weitere Produkte und Dienste</span><span class="sxs-lookup"><span data-stu-id="de71f-420">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="de71f-421">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="de71f-421">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-422">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="de71f-422">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-423">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-423">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="de71f-424">Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="de71f-424">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="de71f-425">Nutzungsgebühr beim Abbrechen bewerten</span><span class="sxs-lookup"><span data-stu-id="de71f-425">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-426">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</span><span class="sxs-lookup"><span data-stu-id="de71f-426">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="de71f-427">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-427">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-428">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="de71f-428">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-429">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="de71f-429">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="de71f-430">Guthaben und Anpassungen</span><span class="sxs-lookup"><span data-stu-id="de71f-430">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="de71f-431">Einen Artikel versetzen</span><span class="sxs-lookup"><span data-stu-id="de71f-431">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-432">Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="de71f-432">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-433">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-433">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="de71f-434">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-434">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="de71f-435">Andere Rabatte</span><span class="sxs-lookup"><span data-stu-id="de71f-435">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="de71f-436">(nutzungsbasiert)</span><span class="sxs-lookup"><span data-stu-id="de71f-436">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="de71f-437">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="de71f-437">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-438">Rabatt auf Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="de71f-438">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="de71f-439">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-439">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-440">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="de71f-440">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-441">Rabatt auf periodische Gebühren</span><span class="sxs-lookup"><span data-stu-id="de71f-441">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="de71f-442">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="de71f-442">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-443">Rabatt auf Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="de71f-443">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="de71f-444">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="de71f-444">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-445">Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="de71f-445">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="de71f-446">Andere Rabatte</span><span class="sxs-lookup"><span data-stu-id="de71f-446">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="de71f-447">(lizenzbasiert)</span><span class="sxs-lookup"><span data-stu-id="de71f-447">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="de71f-448">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="de71f-448">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="de71f-449">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-449">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="de71f-450"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="de71f-450"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="de71f-451">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="de71f-451">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="de71f-452">Ausnahme: "Einen Artikel versetzen" enthält bereits Steuern.</span><span class="sxs-lookup"><span data-stu-id="de71f-452">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="de71f-453">Siehe "Guthaben und Anpassungen" oben.</span><span class="sxs-lookup"><span data-stu-id="de71f-453">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="de71f-454">Steuern oder Umsatzsteuern (Umsatzsteuer)</span><span class="sxs-lookup"><span data-stu-id="de71f-454">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="de71f-455">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-455">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="de71f-456">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="de71f-456">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
