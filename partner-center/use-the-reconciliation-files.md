---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Für eine detaillierte rechnungspositionsinformationen Ansicht der einzelnen Gebühren Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 4b5fbab84c30743e4d91b32bf4cbd2bb8b950992
ms.sourcegitcommit: b433061dff8f667c81b623c33417fb490d8e3b4a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/04/2018
ms.locfileid: "6022240"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="d9458-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="d9458-103">Use the reconciliation files</span></span>

**<span data-ttu-id="d9458-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="d9458-104">Applies to</span></span>**

-  <span data-ttu-id="d9458-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="d9458-105">Partner Center</span></span>
-  <span data-ttu-id="d9458-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d9458-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="d9458-107">Partner Center für Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="d9458-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="d9458-108">Für eine detaillierte rechnungspositionsinformationen Ansicht der einzelnen Gebühren Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d9458-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="d9458-109">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z.B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="d9458-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="d9458-110">Aufschlüsseln nach Partner</span><span class="sxs-lookup"><span data-stu-id="d9458-110">Itemize by partner</span></span>


<span data-ttu-id="d9458-111">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="d9458-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="d9458-112">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="d9458-112">MPN ID</span></span></th>
<th><span data-ttu-id="d9458-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9458-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="d9458-114">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="d9458-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="d9458-115">Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="d9458-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-116">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="d9458-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="d9458-117">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d9458-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="d9458-118">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="d9458-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="d9458-119">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="d9458-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="d9458-120">Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Menü "Partner Center", wählen Sie <strong>Kunden</strong>, und wählen Sie den Kunden aus der Liste.</span><span class="sxs-lookup"><span data-stu-id="d9458-120">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="d9458-121">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="d9458-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="d9458-122">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d9458-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="d9458-123">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="d9458-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="d9458-124">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="d9458-125">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="d9458-126">Lizenzbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="d9458-126">License-based file fields</span></span>


<span data-ttu-id="d9458-127">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus PartnerCenter.</span><span class="sxs-lookup"><span data-stu-id="d9458-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="d9458-128">Spalte</span><span class="sxs-lookup"><span data-stu-id="d9458-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="d9458-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9458-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="d9458-130">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="d9458-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-131">PartnerID</span><span class="sxs-lookup"><span data-stu-id="d9458-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="d9458-132">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="d9458-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="d9458-133">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="d9458-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="d9458-134">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="d9458-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="d9458-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="d9458-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="d9458-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="d9458-137">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="d9458-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="d9458-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="d9458-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="d9458-139">OrderID</span></span></td>
<td><p><span data-ttu-id="d9458-140">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="d9458-141">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="d9458-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="d9458-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="d9458-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="d9458-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="d9458-144">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="d9458-145">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="d9458-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="d9458-146">Diese ID ist nicht mit der Abonnement-ID in der Partner-Verwaltungskonsole identisch.</span><span class="sxs-lookup"><span data-stu-id="d9458-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="d9458-147">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="d9458-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="d9458-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="d9458-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="d9458-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="d9458-150">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d9458-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="d9458-151">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="d9458-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="d9458-152">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="d9458-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="d9458-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="d9458-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="d9458-154">OfferID</span></span></td>
<td><p><span data-ttu-id="d9458-155">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="d9458-155">Unique offer ID.</span></span> <span data-ttu-id="d9458-156">Standard-Angebots-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="d9458-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="d9458-157"><b>Hinweis</b>: Dieser Wert entspricht nicht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="d9458-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="d9458-158">Siehe DurableOfferID unten.</span><span class="sxs-lookup"><span data-stu-id="d9458-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="d9458-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="d9458-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="d9458-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="d9458-161">Eindeutige dauerhafte Angebots-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="d9458-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="d9458-162"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="d9458-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="d9458-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="d9458-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="d9458-164">OfferName</span></span></td>
<td><p><span data-ttu-id="d9458-165">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="d9458-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="d9458-166">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="d9458-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="d9458-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="d9458-168">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="d9458-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="d9458-169">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="d9458-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="d9458-170">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d9458-171">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="d9458-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="d9458-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="d9458-173">Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="d9458-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="d9458-174">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d9458-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="d9458-175">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9458-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="d9458-176">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d9458-177">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="d9458-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="d9458-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="d9458-179">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="d9458-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="d9458-180">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="d9458-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="d9458-181">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d9458-182">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="d9458-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="d9458-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="d9458-184">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="d9458-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="d9458-185">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="d9458-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="d9458-186">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="d9458-187">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="d9458-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="d9458-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="d9458-189">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="d9458-189">The type of charge or adjustment.</span></span> <span data-ttu-id="d9458-190">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="d9458-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="d9458-191">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="d9458-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="d9458-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="d9458-193">Preis pro Arbeitsplatz, wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="d9458-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="d9458-194">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="d9458-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="d9458-195">6,82</span><span class="sxs-lookup"><span data-stu-id="d9458-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-196">Menge</span><span class="sxs-lookup"><span data-stu-id="d9458-196">Quantity</span></span></td>
<td><p><span data-ttu-id="d9458-197">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="d9458-197">Number of seats.</span></span> <span data-ttu-id="d9458-198">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="d9458-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="d9458-199">2</span><span class="sxs-lookup"><span data-stu-id="d9458-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-200">Betrag</span><span class="sxs-lookup"><span data-stu-id="d9458-200">Amount</span></span></td>
<td><p><span data-ttu-id="d9458-201">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="d9458-201">Total of price for quantity.</span></span> <span data-ttu-id="d9458-202">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="d9458-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="d9458-203">13,32</span><span class="sxs-lookup"><span data-stu-id="d9458-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="d9458-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="d9458-205">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="d9458-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="d9458-206">IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</span><span class="sxs-lookup"><span data-stu-id="d9458-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="d9458-207">2,32</span><span class="sxs-lookup"><span data-stu-id="d9458-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-208">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="d9458-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="d9458-209">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="d9458-209">Total before tax.</span></span> <span data-ttu-id="d9458-210">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="d9458-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="d9458-211">11</span><span class="sxs-lookup"><span data-stu-id="d9458-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-212">Steuern</span><span class="sxs-lookup"><span data-stu-id="d9458-212">Tax</span></span></td>
<td><p><span data-ttu-id="d9458-213">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="d9458-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="d9458-214">0</span><span class="sxs-lookup"><span data-stu-id="d9458-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="d9458-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="d9458-216">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="d9458-216">Total after tax.</span></span> <span data-ttu-id="d9458-217">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="d9458-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="d9458-218">11</span><span class="sxs-lookup"><span data-stu-id="d9458-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-219">Währung</span><span class="sxs-lookup"><span data-stu-id="d9458-219">Currency</span></span></td>
<td><p><span data-ttu-id="d9458-220">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="d9458-220">Currency type.</span></span> <span data-ttu-id="d9458-221">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="d9458-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="d9458-222">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="d9458-223">EUR</span><span class="sxs-lookup"><span data-stu-id="d9458-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="d9458-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="d9458-225">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="d9458-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="d9458-226">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="d9458-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="d9458-227">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="d9458-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="d9458-228">MPNID</span></span></td>
<td><p><span data-ttu-id="d9458-229">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="d9458-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="d9458-230">4390934</span><span class="sxs-lookup"><span data-stu-id="d9458-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="d9458-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="d9458-232">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="d9458-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="d9458-233">Siehe [Aufschlüsseln nach Partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="d9458-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="d9458-234">4390934</span><span class="sxs-lookup"><span data-stu-id="d9458-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="d9458-235">DomainName</span></span></td>
<td><p><span data-ttu-id="d9458-236">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="d9458-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="d9458-237">Dies sollte nicht verwendet werden, um den Kunden eindeutig zu identifizieren, wie der Kunde/Partner über das Office 365-Portal Vanity/Standarddomäne aktualisieren können.</span><span class="sxs-lookup"><span data-stu-id="d9458-237">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="d9458-238">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d9458-238">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="d9458-239">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d9458-239">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-240">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="d9458-240">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="d9458-241">Abonnement-Nickname.</span><span class="sxs-lookup"><span data-stu-id="d9458-241">Subscription nickname.</span></span> <span data-ttu-id="d9458-242">Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</span><span class="sxs-lookup"><span data-stu-id="d9458-242">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="d9458-243">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="d9458-243">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-244">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="d9458-244">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="d9458-245">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="d9458-245">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="d9458-246">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="d9458-246">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="d9458-247">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="d9458-247">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="d9458-248">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="d9458-248">Usage-based file fields</span></span>


<span data-ttu-id="d9458-249">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d9458-249">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="d9458-250">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="d9458-250">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="d9458-251">Spalte</span><span class="sxs-lookup"><span data-stu-id="d9458-251">Column</span></span></strong></td>
<td><strong><span data-ttu-id="d9458-252">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9458-252">Description</span></span></strong></td>
<td><strong><span data-ttu-id="d9458-253">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="d9458-253">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-254">PartnerID</span><span class="sxs-lookup"><span data-stu-id="d9458-254">PartnerID</span></span></td>
<td><p><span data-ttu-id="d9458-255">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="d9458-255">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="d9458-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="d9458-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-257">PartnerName</span><span class="sxs-lookup"><span data-stu-id="d9458-257">PartnerName</span></span></td>
<td><p><span data-ttu-id="d9458-258">Partnername.</span><span class="sxs-lookup"><span data-stu-id="d9458-258">Partner Name.</span></span></p></td>
<td><span data-ttu-id="d9458-259">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="d9458-259">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-260">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="d9458-260">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="d9458-261">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="d9458-261">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="d9458-262">1010578050</span><span class="sxs-lookup"><span data-stu-id="d9458-262">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-263">CustomerName</span><span class="sxs-lookup"><span data-stu-id="d9458-263">CustomerName</span></span></td>
<td><p><span data-ttu-id="d9458-264">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="d9458-264">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="d9458-265">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="d9458-265">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="d9458-266">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="d9458-266">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-267">MPNID</span><span class="sxs-lookup"><span data-stu-id="d9458-267">MPNID</span></span></td>
<td><p><span data-ttu-id="d9458-268">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="d9458-268">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="d9458-269">4390934</span><span class="sxs-lookup"><span data-stu-id="d9458-269">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-270">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="d9458-270">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="d9458-271">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="d9458-271">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="d9458-272">Siehe [Aufschlüsseln nach Partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="d9458-272">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="d9458-273">4390934</span><span class="sxs-lookup"><span data-stu-id="d9458-273">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-274">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="d9458-274">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="d9458-275">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d9458-275">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="d9458-276">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="d9458-276">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-277">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="d9458-277">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="d9458-278">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="d9458-278">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="d9458-279">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-279">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="d9458-280">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="d9458-280">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-281">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="d9458-281">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="d9458-282">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="d9458-282">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="d9458-283">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-283">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="d9458-284">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="d9458-284">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-285">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="d9458-285">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="d9458-286">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-286">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="d9458-287">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="d9458-287">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="d9458-288">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="d9458-288">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="d9458-289">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="d9458-289">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-290">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="d9458-290">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="d9458-291">Nickname des Service-Angebots.</span><span class="sxs-lookup"><span data-stu-id="d9458-291">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="d9458-292">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d9458-292">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-293">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="d9458-293">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="d9458-294">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="d9458-294">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="d9458-295">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d9458-295">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-296">OrderID</span><span class="sxs-lookup"><span data-stu-id="d9458-296">OrderID</span></span></td>
<td><p><span data-ttu-id="d9458-297">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-297">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="d9458-298">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="d9458-298">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="d9458-299">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="d9458-299">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-300">ServiceName</span><span class="sxs-lookup"><span data-stu-id="d9458-300">ServiceName</span></span></td>
<td><p><span data-ttu-id="d9458-301">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="d9458-301">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="d9458-302">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="d9458-302">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-303">ServiceType</span><span class="sxs-lookup"><span data-stu-id="d9458-303">ServiceType</span></span></td>
<td><p><span data-ttu-id="d9458-304">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="d9458-304">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="d9458-305">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="d9458-305">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="d9458-306">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="d9458-306">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-307">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="d9458-307">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="d9458-308">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="d9458-308">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="d9458-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="d9458-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-310">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="d9458-310">Resource Name</span></span></td>
<td><p><span data-ttu-id="d9458-311">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d9458-311">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="d9458-312">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="d9458-312">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="d9458-313">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="d9458-313">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-314">Region</span><span class="sxs-lookup"><span data-stu-id="d9458-314">Region</span></span></td>
<td><p><span data-ttu-id="d9458-315">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="d9458-315">The region the usage applies to.</span></span> <span data-ttu-id="d9458-316">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="d9458-316">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="d9458-317">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="d9458-317">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-318">SKU</span><span class="sxs-lookup"><span data-stu-id="d9458-318">SKU</span></span></td>
<td><p><span data-ttu-id="d9458-319">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="d9458-319">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="d9458-320">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="d9458-320">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="d9458-321">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="d9458-321">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="d9458-322">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="d9458-322">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="d9458-323">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="d9458-323">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="d9458-324">1</span><span class="sxs-lookup"><span data-stu-id="d9458-324">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-325">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="d9458-325">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="d9458-326">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="d9458-326">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="d9458-327">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="d9458-327">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="d9458-328">11</span><span class="sxs-lookup"><span data-stu-id="d9458-328">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-329">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="d9458-329">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="d9458-330">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="d9458-330">Units included as part of the offer.</span></span> <span data-ttu-id="d9458-331">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="d9458-331">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="d9458-332">0</span><span class="sxs-lookup"><span data-stu-id="d9458-332">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="d9458-333">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="d9458-333">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="d9458-334">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="d9458-334">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="d9458-335">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="d9458-335">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="d9458-336">11</span><span class="sxs-lookup"><span data-stu-id="d9458-336">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-337">ListPrice</span><span class="sxs-lookup"><span data-stu-id="d9458-337">ListPrice</span></span></td>
<td><p><span data-ttu-id="d9458-338">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="d9458-338">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="d9458-339">0,0808$</span><span class="sxs-lookup"><span data-stu-id="d9458-339">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-340">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="d9458-340">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="d9458-341">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="d9458-341">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="d9458-342">0,085$</span><span class="sxs-lookup"><span data-stu-id="d9458-342">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-343">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="d9458-343">TaxAmount</span></span></td>
<td><p><span data-ttu-id="d9458-344">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="d9458-344">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="d9458-345">0,08$</span><span class="sxs-lookup"><span data-stu-id="d9458-345">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-346">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="d9458-346">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="d9458-347">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="d9458-347">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="d9458-348">0,93$</span><span class="sxs-lookup"><span data-stu-id="d9458-348">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-349">Währung</span><span class="sxs-lookup"><span data-stu-id="d9458-349">Currency</span></span></td>
<td><p><span data-ttu-id="d9458-350">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="d9458-350">Currency type.</span></span> <span data-ttu-id="d9458-351">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="d9458-351">Each billing entity has only one currency.</span></span> <span data-ttu-id="d9458-352">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-352">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="d9458-353">EUR</span><span class="sxs-lookup"><span data-stu-id="d9458-353">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-354">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="d9458-354">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="d9458-355">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="d9458-355">Pretax price per unit.</span></span> <span data-ttu-id="d9458-356">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="d9458-356">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="d9458-357">0,08$</span><span class="sxs-lookup"><span data-stu-id="d9458-357">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-358">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="d9458-358">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="d9458-359">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="d9458-359">Post tax price per unit.</span></span> <span data-ttu-id="d9458-360">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="d9458-360">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="d9458-361">0,08$</span><span class="sxs-lookup"><span data-stu-id="d9458-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-362">ChargeType</span><span class="sxs-lookup"><span data-stu-id="d9458-362">ChargeType</span></span></td>
<td><p><span data-ttu-id="d9458-363">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="d9458-363">The type of charge or adjustment.</span></span> <span data-ttu-id="d9458-364">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="d9458-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="d9458-365">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="d9458-365">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-366">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="d9458-366">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="d9458-367">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-367">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="d9458-368">1280018095</span><span class="sxs-lookup"><span data-stu-id="d9458-368">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-369">UsageDate</span><span class="sxs-lookup"><span data-stu-id="d9458-369">UsageDate</span></span></td>
<td><p><span data-ttu-id="d9458-370">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="d9458-370">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="d9458-371">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="d9458-371">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-372">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="d9458-372">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="d9458-373">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="d9458-373">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="d9458-374">Ostasien, Südostasien, Nordeuropa, Westeuropa, Vereinigte Staaten (Mitte/Norden), Vereinigte Staaten (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="d9458-374">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-375">MeteredService</span><span class="sxs-lookup"><span data-stu-id="d9458-375">MeteredService</span></span></td>
<td><p><span data-ttu-id="d9458-376">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="d9458-376">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="d9458-377">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="d9458-377">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="d9458-378">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="d9458-378">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="d9458-379">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="d9458-379">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-380">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="d9458-380">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="d9458-381">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="d9458-381">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="d9458-382">EXTERN</span><span class="sxs-lookup"><span data-stu-id="d9458-382">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-383">Projekt</span><span class="sxs-lookup"><span data-stu-id="d9458-383">Project</span></span></td>
<td><p><span data-ttu-id="d9458-384">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="d9458-384">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="d9458-385">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="d9458-385">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-386">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="d9458-386">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="d9458-387">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="d9458-387">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="d9458-388">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="d9458-388">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="d9458-389">Wenn ein Paket von 25 ServiceBus-Verbindungen bereitgestellt wurden und Sie an diesem Tag 1 genutzt haben, wird als tägliche Nutzung für diesen Tag „25 Verbindungen/30 Tage – Verwendet: 1,000000“ angegeben.</span><span class="sxs-lookup"><span data-stu-id="d9458-389">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-390">CustomerID</span><span class="sxs-lookup"><span data-stu-id="d9458-390">CustomerID</span></span></td>
<td><p><span data-ttu-id="d9458-391">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="d9458-391">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="d9458-392">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="d9458-392">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d9458-393">DomainName</span><span class="sxs-lookup"><span data-stu-id="d9458-393">DomainName</span></span></td>
<td><p><span data-ttu-id="d9458-394">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="d9458-394">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="d9458-395">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d9458-395">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="d9458-396">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d9458-396">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="d9458-397">Einheit</span><span class="sxs-lookup"><span data-stu-id="d9458-397">Unit</span></span></td>
<td><p><span data-ttu-id="d9458-398">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="d9458-398">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="d9458-399">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="d9458-399">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="d9458-400">Feld für das einmalige Erwerben der Datei</span><span class="sxs-lookup"><span data-stu-id="d9458-400">One-time purchase file fields</span></span>

|**<span data-ttu-id="d9458-401">Feld</span><span class="sxs-lookup"><span data-stu-id="d9458-401">Field</span></span>** |**<span data-ttu-id="d9458-402">Definition</span><span class="sxs-lookup"><span data-stu-id="d9458-402">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="d9458-403">PartnerID</span><span class="sxs-lookup"><span data-stu-id="d9458-403">PartnerId</span></span> |<span data-ttu-id="d9458-404">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="d9458-404">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="d9458-405">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="d9458-405">CustomerId</span></span> |<span data-ttu-id="d9458-406">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="d9458-406">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="d9458-407">CustomerName</span><span class="sxs-lookup"><span data-stu-id="d9458-407">CustomerName</span></span> |<span data-ttu-id="d9458-408">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="d9458-408">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="d9458-409">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="d9458-409">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="d9458-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="d9458-410">CustomerDomainName</span></span> |<span data-ttu-id="d9458-411">Domänenname des Kunden.</span><span class="sxs-lookup"><span data-stu-id="d9458-411">The customer’s domain name.</span></span> |
|<span data-ttu-id="d9458-412">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="d9458-412">CustomerCountry</span></span> |<span data-ttu-id="d9458-413">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="d9458-413">The country in which the customer is located.</span></span> |
|<span data-ttu-id="d9458-414">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="d9458-414">InvoiceNumber</span></span> |<span data-ttu-id="d9458-415">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d9458-415">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="d9458-416">MPNID</span><span class="sxs-lookup"><span data-stu-id="d9458-416">MpnId</span></span> |<span data-ttu-id="d9458-417">Die MPN-ID des CSP Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="d9458-417">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="d9458-418">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="d9458-418">Reseller MPN ID</span></span> |<span data-ttu-id="d9458-419">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d9458-419">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="d9458-420">Die MPN-ID des registrierten Handelspartners für die Reservierung.</span><span class="sxs-lookup"><span data-stu-id="d9458-420">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="d9458-421">Dies entspricht der Handelspartner-ID, die für die spezifische Reservierung im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="d9458-421">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="d9458-422">Wenn ein CSP-Partner die Reservierung direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="d9458-422">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="d9458-423">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-423">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="d9458-424">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d9458-424">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="d9458-425">OrderID</span><span class="sxs-lookup"><span data-stu-id="d9458-425">OrderId</span></span> |<span data-ttu-id="d9458-426">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-426">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="d9458-427">Kann beim Kontakt zum Support zum Identifizieren von Azur Reservations hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="d9458-427">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="d9458-428">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="d9458-428">OrderDate</span></span> |<span data-ttu-id="d9458-429">Der Zeitpunkt der Auftragserstellung.</span><span class="sxs-lookup"><span data-stu-id="d9458-429">The date the order was placed.</span></span> |
|<span data-ttu-id="d9458-430">ProductId</span><span class="sxs-lookup"><span data-stu-id="d9458-430">ProductId</span></span> |<span data-ttu-id="d9458-431">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="d9458-431">The ID for the product.</span></span> |
|<span data-ttu-id="d9458-432">SkuID</span><span class="sxs-lookup"><span data-stu-id="d9458-432">SkuId</span></span>  |<span data-ttu-id="d9458-433">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="d9458-433">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="d9458-434">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="d9458-434">AvailabilityId</span></span> |<span data-ttu-id="d9458-435">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="d9458-435">The ID for a particular Availability.</span></span> <span data-ttu-id="d9458-436">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="d9458-436">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="d9458-437">SkuName</span><span class="sxs-lookup"><span data-stu-id="d9458-437">SkuName</span></span>  |<span data-ttu-id="d9458-438">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="d9458-438">The title for a particular SKU.</span></span> |
|<span data-ttu-id="d9458-439">ProductName</span><span class="sxs-lookup"><span data-stu-id="d9458-439">ProductName</span></span> |<span data-ttu-id="d9458-440">Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="d9458-440">The name of the product.</span></span> |
|<span data-ttu-id="d9458-441">ChargeType</span><span class="sxs-lookup"><span data-stu-id="d9458-441">ChargeType</span></span> |<span data-ttu-id="d9458-442">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="d9458-442">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="d9458-443">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="d9458-443">UnitPrice</span></span> |<span data-ttu-id="d9458-444">Preis pro bestelltem Produkt.</span><span class="sxs-lookup"><span data-stu-id="d9458-444">Price per product ordered.</span></span> |
|<span data-ttu-id="d9458-445">Anzahl</span><span class="sxs-lookup"><span data-stu-id="d9458-445">Quantity</span></span> |<span data-ttu-id="d9458-446">Anzahl der bestellten Produkte.</span><span class="sxs-lookup"><span data-stu-id="d9458-446">Number of products ordered.</span></span> |
|<span data-ttu-id="d9458-447">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="d9458-447">Subtotal</span></span> |<span data-ttu-id="d9458-448">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="d9458-448">Total before tax.</span></span> <span data-ttu-id="d9458-449">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="d9458-449">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="d9458-450">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="d9458-450">TaxTotal</span></span> |<span data-ttu-id="d9458-451">Die Summe aller anwendbaren Steuern.</span><span class="sxs-lookup"><span data-stu-id="d9458-451">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="d9458-452">Gesamt</span><span class="sxs-lookup"><span data-stu-id="d9458-452">Total</span></span> |<span data-ttu-id="d9458-453">Dies ist die Gesamtanzahl der Käufe.</span><span class="sxs-lookup"><span data-stu-id="d9458-453">The total amount of this purchase.</span></span> |
|<span data-ttu-id="d9458-454">Währung</span><span class="sxs-lookup"><span data-stu-id="d9458-454">Currency</span></span> |<span data-ttu-id="d9458-455">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="d9458-455">Currency type.</span></span> <span data-ttu-id="d9458-456">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="d9458-456">Each billing entity has only one currency.</span></span> <span data-ttu-id="d9458-457">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="d9458-457">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="d9458-458">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="d9458-458">DiscountDetails</span></span> |<span data-ttu-id="d9458-459">Detaillierte Liste der relevanten Rabatte.</span><span class="sxs-lookup"><span data-stu-id="d9458-459">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="d9458-460">Siehe Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</span><span class="sxs-lookup"><span data-stu-id="d9458-460">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="d9458-461">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="d9458-461">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="d9458-462">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="d9458-462">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="d9458-463">Sowohl nutzungsbasierte als auch lizenzbasierte Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zusammenhängende Kosten).</span><span class="sxs-lookup"><span data-stu-id="d9458-463">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="d9458-464">Guthaben, Rabatte oder Erstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungsdatei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d9458-464">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="d9458-465">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnittund zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="d9458-465">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="d9458-466">Beschreibung der Rechnungsgebühr</span><span class="sxs-lookup"><span data-stu-id="d9458-466">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="d9458-467">Gebührenbeschreibung der Abstimmungsdatei (ChargeType-Spalte)</span><span class="sxs-lookup"><span data-stu-id="d9458-467">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="d9458-468">Um welche Gebühr handelt es sich?</span><span class="sxs-lookup"><span data-stu-id="d9458-468">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="d9458-469">Wie ordne ich diese ChargeTypes der Rechnung zu?</span><span class="sxs-lookup"><span data-stu-id="d9458-469">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="d9458-470">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="d9458-470">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d9458-471">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="d9458-471">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-472">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="d9458-472">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="d9458-473">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-473">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-474">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="d9458-474">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-475">Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d9458-475">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-476">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="d9458-476">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-477">Periodische Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="d9458-477">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-478">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="d9458-478">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-479">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</span><span class="sxs-lookup"><span data-stu-id="d9458-479">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-480">Gebühren bei Abbrechen anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="d9458-480">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-481">Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="d9458-481">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-482">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="d9458-482">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-483">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="d9458-483">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-484">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="d9458-484">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-485">Anfängliche Gebühr für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="d9458-485">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-486">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="d9458-486">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-487">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="d9458-487">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="d9458-488">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="d9458-488">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-489">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="d9458-489">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-490">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="d9458-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-491">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="d9458-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="d9458-492">Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="d9458-492">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d9458-493">Nutzungsgebühr beim Abbrechen bewerten</span><span class="sxs-lookup"><span data-stu-id="d9458-493">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-494">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</span><span class="sxs-lookup"><span data-stu-id="d9458-494">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="d9458-495">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-495">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-496">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="d9458-496">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-497">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="d9458-497">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="d9458-498">Guthaben</span><span class="sxs-lookup"><span data-stu-id="d9458-498">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d9458-499">Einen Artikel versetzen</span><span class="sxs-lookup"><span data-stu-id="d9458-499">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-500">Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="d9458-500">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-501">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-501">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="d9458-502">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-502">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="d9458-503">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="d9458-503">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="d9458-504">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="d9458-504">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-505">Rabatt auf Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="d9458-505">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="d9458-506">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-506">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-507">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="d9458-507">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-508">Rabatt auf periodische Gebühren</span><span class="sxs-lookup"><span data-stu-id="d9458-508">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-509">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="d9458-509">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-510">Rabatt auf Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="d9458-510">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-511">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="d9458-511">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-512">Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="d9458-512">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="d9458-513">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="d9458-513">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="d9458-514">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="d9458-514">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="d9458-515">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-515">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="d9458-516"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="d9458-516"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="d9458-517">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="d9458-517">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="d9458-518">Ausnahme: "Einen Artikel versetzen" enthält bereits Steuern.</span><span class="sxs-lookup"><span data-stu-id="d9458-518">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="d9458-519">Siehe Guthaben, oben.</span><span class="sxs-lookup"><span data-stu-id="d9458-519">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="d9458-520">Steuern oder Umsatzsteuern (Umsatzsteuer)</span><span class="sxs-lookup"><span data-stu-id="d9458-520">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="d9458-521">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-521">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="d9458-522">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="d9458-522">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
