---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Für eine detaillierte rechnungspositionsinformationen anzuzeigen Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 081afc547a0ff86010e06fcb5224a615a0075e34
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122277"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="c43de-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="c43de-103">Use the reconciliation files</span></span>

**<span data-ttu-id="c43de-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="c43de-104">Applies to</span></span>**

-  <span data-ttu-id="c43de-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c43de-105">Partner Center</span></span>
-  <span data-ttu-id="c43de-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c43de-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="c43de-107">Für eine detaillierte rechnungspositionsinformationen anzuzeigen Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c43de-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="c43de-108">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z.B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="c43de-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="c43de-109">Aufschlüsseln nach Partner</span><span class="sxs-lookup"><span data-stu-id="c43de-109">Itemize by partner</span></span>


<span data-ttu-id="c43de-110">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="c43de-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c43de-111">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="c43de-111">MPN ID</span></span></th>
<th><span data-ttu-id="c43de-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="c43de-113">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="c43de-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="c43de-114">Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="c43de-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-115">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="c43de-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="c43de-116">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c43de-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="c43de-117">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c43de-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c43de-118">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="c43de-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="c43de-119">Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Partner Center-Menü, wählen Sie <strong>Kunden</strong>und dann den Kunden aus der Liste.</span><span class="sxs-lookup"><span data-stu-id="c43de-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="c43de-120">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c43de-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="c43de-121">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="c43de-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="c43de-122">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="c43de-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="c43de-123">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="c43de-124">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="c43de-125">Lizenzbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="c43de-125">License-based file fields</span></span>


<span data-ttu-id="c43de-126">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus PartnerCenter.</span><span class="sxs-lookup"><span data-stu-id="c43de-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="c43de-127">Spalte</span><span class="sxs-lookup"><span data-stu-id="c43de-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="c43de-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="c43de-129">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="c43de-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-130">PartnerID</span><span class="sxs-lookup"><span data-stu-id="c43de-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="c43de-131">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="c43de-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="c43de-132">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="c43de-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="c43de-133">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="c43de-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="c43de-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="c43de-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="c43de-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="c43de-136">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="c43de-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="c43de-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="c43de-138">OrderID</span></span></td>
<td><p><span data-ttu-id="c43de-139">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="c43de-140">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="c43de-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="c43de-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="c43de-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="c43de-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="c43de-143">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="c43de-144">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="c43de-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="c43de-145">Diese ID ist nicht mit der Abonnement-ID in der Partner-Verwaltungskonsole identisch.</span><span class="sxs-lookup"><span data-stu-id="c43de-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="c43de-146">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="c43de-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="c43de-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="c43de-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="c43de-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="c43de-149">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="c43de-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="c43de-150">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="c43de-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="c43de-151">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="c43de-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="c43de-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="c43de-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="c43de-153">OfferID</span></span></td>
<td><p><span data-ttu-id="c43de-154">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="c43de-154">Unique offer ID.</span></span> <span data-ttu-id="c43de-155">Standard-Angebots-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="c43de-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="c43de-156"><b>Hinweis</b>: Dieser Wert entspricht nicht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="c43de-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="c43de-157">Siehe DurableOfferID unten.</span><span class="sxs-lookup"><span data-stu-id="c43de-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="c43de-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="c43de-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="c43de-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="c43de-160">Eindeutige dauerhafte Angebots-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="c43de-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="c43de-161"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="c43de-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="c43de-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="c43de-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="c43de-163">OfferName</span></span></td>
<td><p><span data-ttu-id="c43de-164">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="c43de-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="c43de-165">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="c43de-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="c43de-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="c43de-167">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="c43de-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="c43de-168">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="c43de-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="c43de-169">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c43de-170">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="c43de-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="c43de-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="c43de-172">Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="c43de-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="c43de-173">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c43de-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="c43de-174">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c43de-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="c43de-175">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c43de-176">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="c43de-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="c43de-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="c43de-178">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="c43de-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="c43de-179">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="c43de-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="c43de-180">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c43de-181">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="c43de-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="c43de-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="c43de-183">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="c43de-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="c43de-184">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="c43de-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="c43de-185">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="c43de-186">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="c43de-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="c43de-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="c43de-188">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="c43de-188">The type of charge or adjustment.</span></span> <span data-ttu-id="c43de-189">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="c43de-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="c43de-190">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="c43de-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="c43de-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="c43de-192">Preis pro Arbeitsplatz, wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="c43de-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="c43de-193">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="c43de-194">6,82</span><span class="sxs-lookup"><span data-stu-id="c43de-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-195">Menge</span><span class="sxs-lookup"><span data-stu-id="c43de-195">Quantity</span></span></td>
<td><p><span data-ttu-id="c43de-196">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="c43de-196">Number of seats.</span></span> <span data-ttu-id="c43de-197">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="c43de-198">2</span><span class="sxs-lookup"><span data-stu-id="c43de-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-199">Betrag</span><span class="sxs-lookup"><span data-stu-id="c43de-199">Amount</span></span></td>
<td><p><span data-ttu-id="c43de-200">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="c43de-200">Total of price for quantity.</span></span> <span data-ttu-id="c43de-201">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="c43de-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="c43de-202">13,32</span><span class="sxs-lookup"><span data-stu-id="c43de-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="c43de-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="c43de-204">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="c43de-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="c43de-205">IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</span><span class="sxs-lookup"><span data-stu-id="c43de-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="c43de-206">2,32</span><span class="sxs-lookup"><span data-stu-id="c43de-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-207">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="c43de-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="c43de-208">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="c43de-208">Total before tax.</span></span> <span data-ttu-id="c43de-209">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="c43de-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="c43de-210">11</span><span class="sxs-lookup"><span data-stu-id="c43de-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-211">Steuern</span><span class="sxs-lookup"><span data-stu-id="c43de-211">Tax</span></span></td>
<td><p><span data-ttu-id="c43de-212">USt.-Betrag basierend auf Ihren Market& #39; s Steuervorschriften und spezifischen gegebenheiten.</span><span class="sxs-lookup"><span data-stu-id="c43de-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="c43de-213">0</span><span class="sxs-lookup"><span data-stu-id="c43de-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="c43de-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="c43de-215">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="c43de-215">Total after tax.</span></span> <span data-ttu-id="c43de-216">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="c43de-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="c43de-217">11</span><span class="sxs-lookup"><span data-stu-id="c43de-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-218">Währung</span><span class="sxs-lookup"><span data-stu-id="c43de-218">Currency</span></span></td>
<td><p><span data-ttu-id="c43de-219">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="c43de-219">Currency type.</span></span> <span data-ttu-id="c43de-220">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="c43de-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="c43de-221">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="c43de-222">EUR</span><span class="sxs-lookup"><span data-stu-id="c43de-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="c43de-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="c43de-224">Customer& #39; s Organisationsnamen im Partner Center gemeldet.</span><span class="sxs-lookup"><span data-stu-id="c43de-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="c43de-225">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="c43de-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="c43de-226">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="c43de-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-227">MPNID</span></span></td>
<td><p><span data-ttu-id="c43de-228">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="c43de-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="c43de-229">4390934</span><span class="sxs-lookup"><span data-stu-id="c43de-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="c43de-231">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c43de-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c43de-232">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="c43de-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="c43de-233">4390934</span><span class="sxs-lookup"><span data-stu-id="c43de-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="c43de-234">DomainName</span></span></td>
<td><p><span data-ttu-id="c43de-235">Customer& #39; s-Domänennamen, wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="c43de-236">Dies sollte nicht verwendet werden, um den Kunden eindeutig zu identifizieren, wie der Kunde/Partner über das Office 365-Portal Vanity/Standarddomäne aktualisieren können.</span><span class="sxs-lookup"><span data-stu-id="c43de-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="c43de-237">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c43de-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="c43de-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c43de-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="c43de-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="c43de-240">Abonnement-Nickname.</span><span class="sxs-lookup"><span data-stu-id="c43de-240">Subscription nickname.</span></span> <span data-ttu-id="c43de-241">Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</span><span class="sxs-lookup"><span data-stu-id="c43de-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="c43de-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="c43de-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="c43de-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="c43de-244">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="c43de-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="c43de-245">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="c43de-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="c43de-246">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="c43de-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="c43de-247">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="c43de-247">Usage-based file fields</span></span>


<span data-ttu-id="c43de-248">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c43de-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="c43de-249">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="c43de-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="c43de-250">Spalte</span><span class="sxs-lookup"><span data-stu-id="c43de-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="c43de-251">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="c43de-252">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="c43de-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="c43de-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="c43de-254">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="c43de-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="c43de-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="c43de-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="c43de-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="c43de-257">Partnername.</span><span class="sxs-lookup"><span data-stu-id="c43de-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="c43de-258">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="c43de-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="c43de-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="c43de-260">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="c43de-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="c43de-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="c43de-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="c43de-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="c43de-263">Customer& #39; s Organisationsnamen im Partner Center gemeldet.</span><span class="sxs-lookup"><span data-stu-id="c43de-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="c43de-264">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="c43de-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="c43de-265">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="c43de-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-266">MPNID</span></span></td>
<td><p><span data-ttu-id="c43de-267">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="c43de-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="c43de-268">4390934</span><span class="sxs-lookup"><span data-stu-id="c43de-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="c43de-270">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c43de-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c43de-271">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="c43de-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="c43de-272">4390934</span><span class="sxs-lookup"><span data-stu-id="c43de-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="c43de-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="c43de-274">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="c43de-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="c43de-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="c43de-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="c43de-277">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="c43de-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="c43de-278">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="c43de-279">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="c43de-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="c43de-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="c43de-281">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="c43de-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="c43de-282">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="c43de-283">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="c43de-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="c43de-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="c43de-285">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="c43de-286">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="c43de-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="c43de-287">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="c43de-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="c43de-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="c43de-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="c43de-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="c43de-290">Nickname des Service-Angebots.</span><span class="sxs-lookup"><span data-stu-id="c43de-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="c43de-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="c43de-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="c43de-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="c43de-293">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="c43de-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="c43de-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="c43de-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="c43de-295">OrderID</span></span></td>
<td><p><span data-ttu-id="c43de-296">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="c43de-297">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="c43de-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="c43de-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="c43de-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="c43de-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="c43de-300">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="c43de-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="c43de-301">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="c43de-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="c43de-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="c43de-303">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="c43de-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="c43de-304">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="c43de-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="c43de-305">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="c43de-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="c43de-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="c43de-307">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="c43de-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="c43de-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="c43de-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-309">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="c43de-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="c43de-310">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="c43de-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="c43de-311">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="c43de-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="c43de-312">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="c43de-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-313">Region</span><span class="sxs-lookup"><span data-stu-id="c43de-313">Region</span></span></td>
<td><p><span data-ttu-id="c43de-314">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="c43de-314">The region the usage applies to.</span></span> <span data-ttu-id="c43de-315">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="c43de-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="c43de-316">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="c43de-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-317">SKU</span><span class="sxs-lookup"><span data-stu-id="c43de-317">SKU</span></span></td>
<td><p><span data-ttu-id="c43de-318">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="c43de-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="c43de-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="c43de-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="c43de-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="c43de-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="c43de-321">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="c43de-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="c43de-322">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="c43de-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="c43de-323">1</span><span class="sxs-lookup"><span data-stu-id="c43de-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="c43de-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="c43de-325">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="c43de-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="c43de-326">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="c43de-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="c43de-327">11</span><span class="sxs-lookup"><span data-stu-id="c43de-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="c43de-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="c43de-329">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="c43de-329">Units included as part of the offer.</span></span> <span data-ttu-id="c43de-330">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="c43de-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="c43de-331">0</span><span class="sxs-lookup"><span data-stu-id="c43de-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="c43de-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="c43de-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="c43de-333">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="c43de-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="c43de-334">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="c43de-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="c43de-335">11</span><span class="sxs-lookup"><span data-stu-id="c43de-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="c43de-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="c43de-337">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="c43de-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="c43de-338">0,0808$</span><span class="sxs-lookup"><span data-stu-id="c43de-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="c43de-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="c43de-340">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="c43de-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="c43de-341">0,085$</span><span class="sxs-lookup"><span data-stu-id="c43de-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="c43de-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="c43de-343">USt.-Betrag basierend auf Ihren Market& #39; s Steuervorschriften und spezifischen gegebenheiten.</span><span class="sxs-lookup"><span data-stu-id="c43de-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="c43de-344">0,08$</span><span class="sxs-lookup"><span data-stu-id="c43de-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="c43de-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="c43de-346">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="c43de-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="c43de-347">0,93$</span><span class="sxs-lookup"><span data-stu-id="c43de-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-348">Währung</span><span class="sxs-lookup"><span data-stu-id="c43de-348">Currency</span></span></td>
<td><p><span data-ttu-id="c43de-349">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="c43de-349">Currency type.</span></span> <span data-ttu-id="c43de-350">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="c43de-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="c43de-351">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="c43de-352">EUR</span><span class="sxs-lookup"><span data-stu-id="c43de-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="c43de-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="c43de-354">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="c43de-354">Pretax price per unit.</span></span> <span data-ttu-id="c43de-355">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="c43de-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="c43de-356">0,08$</span><span class="sxs-lookup"><span data-stu-id="c43de-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="c43de-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="c43de-358">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="c43de-358">Post tax price per unit.</span></span> <span data-ttu-id="c43de-359">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="c43de-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="c43de-360">0,08$</span><span class="sxs-lookup"><span data-stu-id="c43de-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="c43de-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="c43de-362">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="c43de-362">The type of charge or adjustment.</span></span> <span data-ttu-id="c43de-363">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="c43de-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="c43de-364">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="c43de-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="c43de-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="c43de-366">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="c43de-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="c43de-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="c43de-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="c43de-369">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="c43de-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="c43de-370">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="c43de-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="c43de-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="c43de-372">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c43de-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="c43de-373">Ostasien, Südostasien, Nordeuropa, Westeuropa, Vereinigte Staaten (Mitte/Norden), Vereinigte Staaten (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="c43de-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="c43de-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="c43de-375">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="c43de-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="c43de-376">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="c43de-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="c43de-377">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="c43de-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="c43de-378">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="c43de-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="c43de-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="c43de-380">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="c43de-381">EXTERN</span><span class="sxs-lookup"><span data-stu-id="c43de-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-382">Projekt</span><span class="sxs-lookup"><span data-stu-id="c43de-382">Project</span></span></td>
<td><p><span data-ttu-id="c43de-383">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="c43de-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="c43de-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="c43de-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="c43de-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="c43de-386">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="c43de-387">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="c43de-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="c43de-388">Wenn ein Paket von 25 ServiceBus-Verbindungen bereitgestellt wurden und Sie an diesem Tag 1 genutzt haben, wird als tägliche Nutzung für diesen Tag „25 Verbindungen/30 Tage – Verwendet: 1,000000“ angegeben.</span><span class="sxs-lookup"><span data-stu-id="c43de-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="c43de-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="c43de-390">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="c43de-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="c43de-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="c43de-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="c43de-392">DomainName</span></span></td>
<td><p><span data-ttu-id="c43de-393">Customer& #39; s-Domänennamen, wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="c43de-394">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c43de-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="c43de-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c43de-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="c43de-396">Einheit</span><span class="sxs-lookup"><span data-stu-id="c43de-396">Unit</span></span></td>
<td><p><span data-ttu-id="c43de-397">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="c43de-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="c43de-398">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="c43de-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="c43de-399">Einmalige und wiederkehrenden Dateifelder</span><span class="sxs-lookup"><span data-stu-id="c43de-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c43de-400">Spalte</span><span class="sxs-lookup"><span data-stu-id="c43de-400">Column</span></span></th>
<th><span data-ttu-id="c43de-401">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="c43de-402">PartnerID</span><span class="sxs-lookup"><span data-stu-id="c43de-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="c43de-403">Eindeutiger Bezeichner für Microsoft Azure Active Directory-Mandanten für eine spezifische abrechnungsentität im GUID-Format '.</span><span class="sxs-lookup"><span data-stu-id="c43de-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="c43de-404">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="c43de-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="c43de-405">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="c43de-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-406">Kunden-Id</span><span class="sxs-lookup"><span data-stu-id="c43de-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="c43de-407">Eindeutige Microsoft Azure Active Directory-Mandanten-ID im GUID-Format, die zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-408">Kundenname</span><span class="sxs-lookup"><span data-stu-id="c43de-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="c43de-409">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="c43de-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="c43de-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="c43de-411">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="c43de-412">Dies sollte nicht verwendet werden, um den Kunden eindeutig zu identifizieren, wie der Kunde/Partner über das Office 365-Portal Vanity/Standarddomäne aktualisieren können.</span><span class="sxs-lookup"><span data-stu-id="c43de-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="c43de-413">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c43de-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-414">Kunden Land</span><span class="sxs-lookup"><span data-stu-id="c43de-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="c43de-415">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="c43de-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-416">Rechnungsnummer</span><span class="sxs-lookup"><span data-stu-id="c43de-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="c43de-417">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-418">MPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-418">MpnId</span></span></td>
<td><p><span data-ttu-id="c43de-419">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="c43de-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-420">Händler MpnId</span><span class="sxs-lookup"><span data-stu-id="c43de-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="c43de-421">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c43de-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-422">Bestellnummer</span><span class="sxs-lookup"><span data-stu-id="c43de-422">Order ID</span></span></td>
<td><p><span data-ttu-id="c43de-423">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-e-Commerce-Plattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="c43de-424">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="c43de-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-425">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="c43de-425">Order date</span></span></td>
<td><p><span data-ttu-id="c43de-426">Der Zeitpunkt der Auftragserstellung.</span><span class="sxs-lookup"><span data-stu-id="c43de-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="c43de-427">ProductId</span></span></td>
<td><p><span data-ttu-id="c43de-428">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="c43de-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-429">SkuID</span><span class="sxs-lookup"><span data-stu-id="c43de-429">SkuId</span></span></td>
<td><p><span data-ttu-id="c43de-430">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="c43de-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="c43de-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="c43de-432">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="c43de-432">The ID for a particular Availability.</span></span> <span data-ttu-id="c43de-433">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="c43de-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-434">SKU-Namen</span><span class="sxs-lookup"><span data-stu-id="c43de-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="c43de-435">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="c43de-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-436">Produktname</span><span class="sxs-lookup"><span data-stu-id="c43de-436">Product name</span></span></td>
<td><p><span data-ttu-id="c43de-437">Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="c43de-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="c43de-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="c43de-439">Der Name des Herausgebers des Produkts.</span><span class="sxs-lookup"><span data-stu-id="c43de-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-440">Des PublisherID</span><span class="sxs-lookup"><span data-stu-id="c43de-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="c43de-441">Eindeutige ID für diesen Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="c43de-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-442">Abonnement-Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="c43de-443">Anzeigename eines Abonnements.</span><span class="sxs-lookup"><span data-stu-id="c43de-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-444">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="c43de-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="c43de-445">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-e-Commerce-Plattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="c43de-446">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="c43de-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="c43de-447">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="c43de-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="c43de-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="c43de-449">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="c43de-449">Start day of the charges.</span></span> <span data-ttu-id="c43de-450">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="c43de-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="c43de-452">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="c43de-452">End day of the charges.</span></span> <span data-ttu-id="c43de-453">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-454">Begriff und Billingcycle</span><span class="sxs-lookup"><span data-stu-id="c43de-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="c43de-455">Der Begriff Länge und Rechnungszyklus für die Bestellung.</span><span class="sxs-lookup"><span data-stu-id="c43de-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="c43de-456">Beispielsweise "1 Jahr, monatlich."</span><span class="sxs-lookup"><span data-stu-id="c43de-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-457">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="c43de-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="c43de-458">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="c43de-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-459">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="c43de-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="c43de-460">Der Preis wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="c43de-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="c43de-461">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-462">Preis pro Einheit effektive</span><span class="sxs-lookup"><span data-stu-id="c43de-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="c43de-463">Preis pro Einheit nach Korrekturen vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-464">Anzahl</span><span class="sxs-lookup"><span data-stu-id="c43de-464">Quantity</span></span></td>
<td><p><span data-ttu-id="c43de-465">Anzahl der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="c43de-465">Number of units.</span></span> <span data-ttu-id="c43de-466">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-467">Einheitentyp</span><span class="sxs-lookup"><span data-stu-id="c43de-467">Unit type</span></span></td>
<td><p><span data-ttu-id="c43de-468">Der Typ der Einheit erworben wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="c43de-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="c43de-470">Eine Erklärung, alle anwendbaren Rabatte.</span><span class="sxs-lookup"><span data-stu-id="c43de-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-471">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="c43de-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="c43de-472">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="c43de-472">Total before tax.</span></span> <span data-ttu-id="c43de-473">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="c43de-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-474">Steuern</span><span class="sxs-lookup"><span data-stu-id="c43de-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="c43de-475">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="c43de-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-476">Gesamt</span><span class="sxs-lookup"><span data-stu-id="c43de-476">Total</span></span></td>
<td><p><span data-ttu-id="c43de-477">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="c43de-477">Total after tax.</span></span> <span data-ttu-id="c43de-478">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="c43de-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-479">Währung</span><span class="sxs-lookup"><span data-stu-id="c43de-479">Currency</span></span></td>
<td><p><span data-ttu-id="c43de-480">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="c43de-480">Currency type.</span></span> <span data-ttu-id="c43de-481">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="c43de-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="c43de-482">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="c43de-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="c43de-484">Ein alternativer Bezeichner, der eine ID ein.</span><span class="sxs-lookup"><span data-stu-id="c43de-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="c43de-485">Nutzung täglich bewertete Dateifelder</span><span class="sxs-lookup"><span data-stu-id="c43de-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="c43de-486">Spalte</span><span class="sxs-lookup"><span data-stu-id="c43de-486">Column</span></span></th>
<th><span data-ttu-id="c43de-487">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="c43de-488">PartnerID</span><span class="sxs-lookup"><span data-stu-id="c43de-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="c43de-489">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="c43de-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="c43de-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="c43de-491">Partnername.</span><span class="sxs-lookup"><span data-stu-id="c43de-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-492">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="c43de-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="c43de-493">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="c43de-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="c43de-495">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="c43de-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="c43de-496">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="c43de-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="c43de-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="c43de-498">Domänenname des Kunden.</span><span class="sxs-lookup"><span data-stu-id="c43de-498">The customer’s domain name.</span></span> <span data-ttu-id="c43de-499">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c43de-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-500">Kunden Land</span><span class="sxs-lookup"><span data-stu-id="c43de-500">Customer country</span></span></td>
<td><p><span data-ttu-id="c43de-501">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="c43de-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-502">MPNID</span></span></td>
<td><p><span data-ttu-id="c43de-503">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="c43de-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-504">Händler MPNID</span><span class="sxs-lookup"><span data-stu-id="c43de-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="c43de-505">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="c43de-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="c43de-506">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c43de-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="c43de-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="c43de-508">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="c43de-509">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c43de-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="c43de-510">ProductId</span></span></td>
<td><p><span data-ttu-id="c43de-511">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="c43de-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-512">SkuID</span><span class="sxs-lookup"><span data-stu-id="c43de-512">SkuId</span></span></td>
<td><p><span data-ttu-id="c43de-513">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="c43de-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="c43de-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="c43de-515">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="c43de-515">The ID for a particular Availability.</span></span> <span data-ttu-id="c43de-516">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="c43de-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-517">SKU-Namen</span><span class="sxs-lookup"><span data-stu-id="c43de-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="c43de-518">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="c43de-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="c43de-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="c43de-520">Der Name des Herausgebers.</span><span class="sxs-lookup"><span data-stu-id="c43de-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-521">Des PublisherID</span><span class="sxs-lookup"><span data-stu-id="c43de-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="c43de-522">Die ID des Herausgebers, im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="c43de-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="c43de-523">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c43de-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="c43de-524">Abonnement-Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43de-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="c43de-525">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="c43de-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="c43de-526">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="c43de-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-527">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="c43de-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="c43de-528">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="c43de-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="c43de-529">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="c43de-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="c43de-530">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="c43de-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="c43de-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="c43de-532">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="c43de-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="c43de-533">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="c43de-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="c43de-535">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="c43de-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="c43de-536">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c43de-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-537">Nutzung Datum</span><span class="sxs-lookup"><span data-stu-id="c43de-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="c43de-538">Datum der Service-Nutzung.</span><span class="sxs-lookup"><span data-stu-id="c43de-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-539">Anzeige-Typ</span><span class="sxs-lookup"><span data-stu-id="c43de-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="c43de-540">Der Typ der Anzeige.</span><span class="sxs-lookup"><span data-stu-id="c43de-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-541">Meter Kategorie</span><span class="sxs-lookup"><span data-stu-id="c43de-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="c43de-542">Der obersten Ebene Dienst für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="c43de-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-543">Anzeige-Id</span><span class="sxs-lookup"><span data-stu-id="c43de-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="c43de-544">Die ID für die Anzeige verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-545">Meter Unterkategorie</span><span class="sxs-lookup"><span data-stu-id="c43de-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="c43de-546">Der Typ des Azure-Dienst, der die Rate auswirken kann.</span><span class="sxs-lookup"><span data-stu-id="c43de-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-547">Meter Name</span><span class="sxs-lookup"><span data-stu-id="c43de-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="c43de-548">Die Maßeinheit für die Anzeige genutzt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-549">Meter Region</span><span class="sxs-lookup"><span data-stu-id="c43de-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="c43de-550">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c43de-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-551">Einheit</span><span class="sxs-lookup"><span data-stu-id="c43de-551">Unit</span></span></td>
<td><p><span data-ttu-id="c43de-552">Die Einheit des Ressourcennamens.</span><span class="sxs-lookup"><span data-stu-id="c43de-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-553">Verbrauchten Menge</span><span class="sxs-lookup"><span data-stu-id="c43de-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="c43de-554">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="c43de-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="c43de-555">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="c43de-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-556">Speicherort der Ressource</span><span class="sxs-lookup"><span data-stu-id="c43de-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="c43de-557">Die Datacenter, in denen die Anzeige ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-558">Verbrauchten Service</span><span class="sxs-lookup"><span data-stu-id="c43de-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="c43de-559">Der Azure-Plattform-Dienst, den Sie verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-560">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="c43de-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="c43de-561">Der Ressourcengruppe, in der die bereitgestellte Anzeige ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-562">Ressourcen-URI</span><span class="sxs-lookup"><span data-stu-id="c43de-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="c43de-563">Der URI der Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c43de-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-564">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="c43de-564">Charge type</span></span></td>
<td><p><span data-ttu-id="c43de-565">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="c43de-565">The type of charge or adjustment.</span></span> <span data-ttu-id="c43de-566">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c43de-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-567">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="c43de-567">Unit price</span></span></td>
<td><p><span data-ttu-id="c43de-568">Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="c43de-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="c43de-569">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-570">Anzahl</span><span class="sxs-lookup"><span data-stu-id="c43de-570">Quantity</span></span></td>
<td><p><span data-ttu-id="c43de-571">Anzahl der Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c43de-571">Number of licenses.</span></span> <span data-ttu-id="c43de-572">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-573">Einheitentyp</span><span class="sxs-lookup"><span data-stu-id="c43de-573">Unit type</span></span></td>
<td><p><span data-ttu-id="c43de-574">Der Typ der Einheit der Anzeige ist in in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="c43de-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="c43de-575">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c43de-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-576">Abrechnung vor Steuern</span><span class="sxs-lookup"><span data-stu-id="c43de-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="c43de-577">Gesamtbetrag vor Steuern.</span><span class="sxs-lookup"><span data-stu-id="c43de-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-578">Währung der Abrechnung</span><span class="sxs-lookup"><span data-stu-id="c43de-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="c43de-579">Die Währung in einer geografischen Region des Kunden</span><span class="sxs-lookup"><span data-stu-id="c43de-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-580">Preise gewöhnlichen insgesamt</span><span class="sxs-lookup"><span data-stu-id="c43de-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="c43de-581">Die Preise vor Steuern hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="c43de-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-582">Währung Preise</span><span class="sxs-lookup"><span data-stu-id="c43de-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="c43de-583">Die Währung, in der Preisliste wiedergegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="c43de-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-584">Service Info 1</span><span class="sxs-lookup"><span data-stu-id="c43de-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="c43de-585">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="c43de-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-586">Service-Informationen 2</span><span class="sxs-lookup"><span data-stu-id="c43de-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="c43de-587">Ein legacy-Feld, das optionale Service-spezifischen Metadaten erfasst.</span><span class="sxs-lookup"><span data-stu-id="c43de-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="c43de-588">Schilder</span><span class="sxs-lookup"><span data-stu-id="c43de-588">Tags</span></span></td>
<td><p><span data-ttu-id="c43de-589">Tags, die Sie für die Anzeige in der Reihenfolge zum Gruppieren Abrechnung zuweisen.</span><span class="sxs-lookup"><span data-stu-id="c43de-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="c43de-590">Beispielsweise können Sie Tags verwenden, um Kosten von der Abteilung zu verteilen, die die Anzeige verwendet.</span><span class="sxs-lookup"><span data-stu-id="c43de-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="c43de-591">Zusätzliche Infos</span><span class="sxs-lookup"><span data-stu-id="c43de-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="c43de-592">Alle zusätzlichen Informationen, die in anderen Spalten nicht behandelt.</span><span class="sxs-lookup"><span data-stu-id="c43de-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="c43de-593">Siehe Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</span><span class="sxs-lookup"><span data-stu-id="c43de-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="c43de-594">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="c43de-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="c43de-595">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="c43de-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="c43de-596">Sowohl nutzungsbasierte als auch lizenzbasierte Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zusammenhängende Kosten).</span><span class="sxs-lookup"><span data-stu-id="c43de-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="c43de-597">Guthaben, Rabatte oder Erstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungsdatei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c43de-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="c43de-598">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnittund zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c43de-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="c43de-599">Beschreibung der Rechnungsgebühr</span><span class="sxs-lookup"><span data-stu-id="c43de-599">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="c43de-600">Gebührenbeschreibung der Abstimmungsdatei (ChargeType-Spalte)</span><span class="sxs-lookup"><span data-stu-id="c43de-600">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="c43de-601">Um welche Gebühr handelt es sich?</span><span class="sxs-lookup"><span data-stu-id="c43de-601">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="c43de-602">Wie ordne ich diese ChargeTypes der Rechnung zu?</span><span class="sxs-lookup"><span data-stu-id="c43de-602">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="c43de-603">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="c43de-603">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="c43de-604">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="c43de-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-605">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="c43de-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="c43de-606">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-607">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="c43de-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-608">Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="c43de-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-609">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="c43de-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-610">Periodische Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="c43de-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-611">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="c43de-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-612">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</span><span class="sxs-lookup"><span data-stu-id="c43de-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-613">Gebühren bei Abbrechen anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="c43de-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-614">Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="c43de-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-615">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="c43de-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-616">Der Typ der Abrechnung für ein Abonnement bei Verwendung der jährlichen Abrechnung</span><span class="sxs-lookup"><span data-stu-id="c43de-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-617">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="c43de-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-618">Der Typ der Abrechnung für ein Abonnement bei Verwendung monatliche Abrechnung</span><span class="sxs-lookup"><span data-stu-id="c43de-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-619">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="c43de-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-620">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="c43de-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="c43de-621">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="c43de-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-622">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="c43de-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-623">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="c43de-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-624">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="c43de-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="c43de-625">Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="c43de-625">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="c43de-626">Nutzungsgebühr beim Abbrechen bewerten</span><span class="sxs-lookup"><span data-stu-id="c43de-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-627">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</span><span class="sxs-lookup"><span data-stu-id="c43de-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="c43de-628">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-629">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="c43de-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-630">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="c43de-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="c43de-631">Guthaben</span><span class="sxs-lookup"><span data-stu-id="c43de-631">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="c43de-632">Einen Artikel versetzen</span><span class="sxs-lookup"><span data-stu-id="c43de-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-633">Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="c43de-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-634">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="c43de-635">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="c43de-636">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="c43de-636">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="c43de-637">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="c43de-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-638">Rabatt auf Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="c43de-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="c43de-639">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-640">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="c43de-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-641">Rabatt auf periodische Gebühren</span><span class="sxs-lookup"><span data-stu-id="c43de-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-642">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="c43de-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-643">Rabatt auf Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="c43de-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-644">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="c43de-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-645">Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="c43de-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="c43de-646">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="c43de-646">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="c43de-647">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="c43de-647">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="c43de-648">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="c43de-649"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="c43de-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="c43de-650">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="c43de-650">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="c43de-651">Ausnahme: &quot;einen Artikel versetzen&quot; enthält bereits steuern.</span><span class="sxs-lookup"><span data-stu-id="c43de-651">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="c43de-652">Siehe Guthaben, oben.</span><span class="sxs-lookup"><span data-stu-id="c43de-652">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="c43de-653">Steuern oder Umsatzsteuern (Umsatzsteuer)</span><span class="sxs-lookup"><span data-stu-id="c43de-653">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="c43de-654">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-654">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="c43de-655">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="c43de-655">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
