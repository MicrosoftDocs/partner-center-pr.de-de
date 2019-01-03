---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Für eine detaillierte rechnungspositionsinformationen anzuzeigen Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 50af14ab0e8edf6cd4576be6615cd7238b23bd99
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990992"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="003f0-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="003f0-103">Use the reconciliation files</span></span>

**<span data-ttu-id="003f0-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="003f0-104">Applies to</span></span>**

-  <span data-ttu-id="003f0-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="003f0-105">Partner Center</span></span>
-  <span data-ttu-id="003f0-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="003f0-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="003f0-107">Für eine detaillierte rechnungspositionsinformationen anzuzeigen Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center.</span><span class="sxs-lookup"><span data-stu-id="003f0-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="003f0-108">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z.B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="003f0-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="003f0-109">Aufschlüsseln nach Partner</span><span class="sxs-lookup"><span data-stu-id="003f0-109">Itemize by partner</span></span>


<span data-ttu-id="003f0-110">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="003f0-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="003f0-111">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="003f0-111">MPN ID</span></span></th>
<th><span data-ttu-id="003f0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003f0-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="003f0-113">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="003f0-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="003f0-114">Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="003f0-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-115">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="003f0-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="003f0-116">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="003f0-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="003f0-117">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="003f0-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="003f0-118">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="003f0-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="003f0-119">Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Partner Center-Menü wählen <strong>Kunden</strong>aus, und wählen Sie den Kunden aus der Liste.</span><span class="sxs-lookup"><span data-stu-id="003f0-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="003f0-120">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="003f0-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="003f0-121">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="003f0-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="003f0-122">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="003f0-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="003f0-123">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="003f0-124">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="003f0-125">Lizenzbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="003f0-125">License-based file fields</span></span>


<span data-ttu-id="003f0-126">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus PartnerCenter.</span><span class="sxs-lookup"><span data-stu-id="003f0-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="003f0-127">Spalte</span><span class="sxs-lookup"><span data-stu-id="003f0-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="003f0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003f0-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="003f0-129">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="003f0-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-130">PartnerID</span><span class="sxs-lookup"><span data-stu-id="003f0-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="003f0-131">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="003f0-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="003f0-132">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="003f0-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="003f0-133">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="003f0-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="003f0-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="003f0-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="003f0-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="003f0-136">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="003f0-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="003f0-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="003f0-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="003f0-138">OrderID</span></span></td>
<td><p><span data-ttu-id="003f0-139">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="003f0-140">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="003f0-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="003f0-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="003f0-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="003f0-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="003f0-143">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="003f0-144">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="003f0-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="003f0-145">Diese ID ist nicht mit der Abonnement-ID in der Partner-Verwaltungskonsole identisch.</span><span class="sxs-lookup"><span data-stu-id="003f0-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="003f0-146">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="003f0-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="003f0-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="003f0-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="003f0-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="003f0-149">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="003f0-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="003f0-150">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="003f0-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="003f0-151">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="003f0-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="003f0-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="003f0-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="003f0-153">OfferID</span></span></td>
<td><p><span data-ttu-id="003f0-154">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="003f0-154">Unique offer ID.</span></span> <span data-ttu-id="003f0-155">Standard-Angebots-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="003f0-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="003f0-156"><b>Hinweis</b>: Dieser Wert entspricht nicht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="003f0-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="003f0-157">Siehe DurableOfferID unten.</span><span class="sxs-lookup"><span data-stu-id="003f0-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="003f0-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="003f0-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="003f0-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="003f0-160">Eindeutige dauerhafte Angebots-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="003f0-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="003f0-161"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="003f0-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="003f0-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="003f0-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="003f0-163">OfferName</span></span></td>
<td><p><span data-ttu-id="003f0-164">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="003f0-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="003f0-165">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="003f0-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="003f0-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="003f0-167">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="003f0-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="003f0-168">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="003f0-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="003f0-169">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="003f0-170">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="003f0-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="003f0-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="003f0-172">Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="003f0-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="003f0-173">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="003f0-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="003f0-174">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="003f0-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="003f0-175">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="003f0-176">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="003f0-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="003f0-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="003f0-178">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="003f0-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="003f0-179">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="003f0-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="003f0-180">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="003f0-181">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="003f0-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="003f0-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="003f0-183">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="003f0-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="003f0-184">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="003f0-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="003f0-185">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="003f0-186">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="003f0-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="003f0-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="003f0-188">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="003f0-188">The type of charge or adjustment.</span></span> <span data-ttu-id="003f0-189">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="003f0-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="003f0-190">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="003f0-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="003f0-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="003f0-192">Preis pro Arbeitsplatz, wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="003f0-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="003f0-193">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="003f0-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="003f0-194">6,82</span><span class="sxs-lookup"><span data-stu-id="003f0-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-195">Menge</span><span class="sxs-lookup"><span data-stu-id="003f0-195">Quantity</span></span></td>
<td><p><span data-ttu-id="003f0-196">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="003f0-196">Number of seats.</span></span> <span data-ttu-id="003f0-197">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="003f0-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="003f0-198">2</span><span class="sxs-lookup"><span data-stu-id="003f0-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-199">Betrag</span><span class="sxs-lookup"><span data-stu-id="003f0-199">Amount</span></span></td>
<td><p><span data-ttu-id="003f0-200">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="003f0-200">Total of price for quantity.</span></span> <span data-ttu-id="003f0-201">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="003f0-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="003f0-202">13,32</span><span class="sxs-lookup"><span data-stu-id="003f0-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="003f0-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="003f0-204">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="003f0-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="003f0-205">IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</span><span class="sxs-lookup"><span data-stu-id="003f0-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="003f0-206">2,32</span><span class="sxs-lookup"><span data-stu-id="003f0-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-207">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="003f0-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="003f0-208">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="003f0-208">Total before tax.</span></span> <span data-ttu-id="003f0-209">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="003f0-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="003f0-210">11</span><span class="sxs-lookup"><span data-stu-id="003f0-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-211">Steuern</span><span class="sxs-lookup"><span data-stu-id="003f0-211">Tax</span></span></td>
<td><p><span data-ttu-id="003f0-212">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="003f0-212">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="003f0-213">0</span><span class="sxs-lookup"><span data-stu-id="003f0-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="003f0-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="003f0-215">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="003f0-215">Total after tax.</span></span> <span data-ttu-id="003f0-216">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="003f0-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="003f0-217">11</span><span class="sxs-lookup"><span data-stu-id="003f0-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-218">Währung</span><span class="sxs-lookup"><span data-stu-id="003f0-218">Currency</span></span></td>
<td><p><span data-ttu-id="003f0-219">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="003f0-219">Currency type.</span></span> <span data-ttu-id="003f0-220">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="003f0-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="003f0-221">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="003f0-222">EUR</span><span class="sxs-lookup"><span data-stu-id="003f0-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="003f0-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="003f0-224">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="003f0-224">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="003f0-225">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="003f0-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="003f0-226">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="003f0-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="003f0-227">MPNID</span></span></td>
<td><p><span data-ttu-id="003f0-228">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="003f0-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="003f0-229">4390934</span><span class="sxs-lookup"><span data-stu-id="003f0-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="003f0-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="003f0-231">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="003f0-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="003f0-232">Siehe [Aufschlüsseln nach Partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="003f0-232">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="003f0-233">4390934</span><span class="sxs-lookup"><span data-stu-id="003f0-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="003f0-234">DomainName</span></span></td>
<td><p><span data-ttu-id="003f0-235">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="003f0-235">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="003f0-236">Dies sollte nicht verwendet werden, um den Kunden eindeutig zu identifizieren, wie der Kunde/Partner über das Office 365-Portal Vanity/Standarddomäne aktualisieren können.</span><span class="sxs-lookup"><span data-stu-id="003f0-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="003f0-237">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="003f0-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="003f0-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="003f0-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="003f0-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="003f0-240">Abonnement-Nickname.</span><span class="sxs-lookup"><span data-stu-id="003f0-240">Subscription nickname.</span></span> <span data-ttu-id="003f0-241">Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</span><span class="sxs-lookup"><span data-stu-id="003f0-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="003f0-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="003f0-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="003f0-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="003f0-244">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="003f0-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="003f0-245">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="003f0-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="003f0-246">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="003f0-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="003f0-247">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="003f0-247">Usage-based file fields</span></span>


<span data-ttu-id="003f0-248">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="003f0-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="003f0-249">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="003f0-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="003f0-250">Spalte</span><span class="sxs-lookup"><span data-stu-id="003f0-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="003f0-251">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003f0-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="003f0-252">Beispielwert</span><span class="sxs-lookup"><span data-stu-id="003f0-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="003f0-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="003f0-254">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="003f0-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="003f0-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="003f0-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="003f0-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="003f0-257">Partnername.</span><span class="sxs-lookup"><span data-stu-id="003f0-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="003f0-258">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="003f0-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="003f0-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="003f0-260">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="003f0-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="003f0-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="003f0-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="003f0-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="003f0-263">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="003f0-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="003f0-264">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="003f0-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="003f0-265">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="003f0-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="003f0-266">MPNID</span></span></td>
<td><p><span data-ttu-id="003f0-267">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="003f0-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="003f0-268">4390934</span><span class="sxs-lookup"><span data-stu-id="003f0-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="003f0-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="003f0-270">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="003f0-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="003f0-271">Siehe [Aufschlüsseln nach Partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="003f0-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="003f0-272">4390934</span><span class="sxs-lookup"><span data-stu-id="003f0-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="003f0-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="003f0-274">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="003f0-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="003f0-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="003f0-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="003f0-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="003f0-277">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="003f0-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="003f0-278">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="003f0-279">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="003f0-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="003f0-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="003f0-281">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="003f0-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="003f0-282">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="003f0-283">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="003f0-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="003f0-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="003f0-285">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="003f0-286">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="003f0-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="003f0-287">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="003f0-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="003f0-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="003f0-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="003f0-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="003f0-290">Nickname des Service-Angebots.</span><span class="sxs-lookup"><span data-stu-id="003f0-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="003f0-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="003f0-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="003f0-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="003f0-293">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="003f0-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="003f0-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="003f0-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="003f0-295">OrderID</span></span></td>
<td><p><span data-ttu-id="003f0-296">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="003f0-297">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="003f0-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="003f0-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="003f0-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="003f0-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="003f0-300">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="003f0-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="003f0-301">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="003f0-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="003f0-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="003f0-303">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="003f0-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="003f0-304">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="003f0-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="003f0-305">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="003f0-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="003f0-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="003f0-307">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="003f0-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="003f0-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="003f0-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-309">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="003f0-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="003f0-310">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="003f0-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="003f0-311">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="003f0-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="003f0-312">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="003f0-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-313">Region</span><span class="sxs-lookup"><span data-stu-id="003f0-313">Region</span></span></td>
<td><p><span data-ttu-id="003f0-314">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="003f0-314">The region the usage applies to.</span></span> <span data-ttu-id="003f0-315">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="003f0-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="003f0-316">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="003f0-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-317">SKU</span><span class="sxs-lookup"><span data-stu-id="003f0-317">SKU</span></span></td>
<td><p><span data-ttu-id="003f0-318">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="003f0-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="003f0-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="003f0-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="003f0-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="003f0-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="003f0-321">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="003f0-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="003f0-322">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="003f0-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="003f0-323">1</span><span class="sxs-lookup"><span data-stu-id="003f0-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="003f0-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="003f0-325">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="003f0-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="003f0-326">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="003f0-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="003f0-327">11</span><span class="sxs-lookup"><span data-stu-id="003f0-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="003f0-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="003f0-329">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="003f0-329">Units included as part of the offer.</span></span> <span data-ttu-id="003f0-330">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="003f0-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="003f0-331">0</span><span class="sxs-lookup"><span data-stu-id="003f0-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="003f0-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="003f0-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="003f0-333">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="003f0-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="003f0-334">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="003f0-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="003f0-335">11</span><span class="sxs-lookup"><span data-stu-id="003f0-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="003f0-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="003f0-337">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="003f0-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="003f0-338">0,0808$</span><span class="sxs-lookup"><span data-stu-id="003f0-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="003f0-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="003f0-340">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="003f0-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="003f0-341">0,085$</span><span class="sxs-lookup"><span data-stu-id="003f0-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="003f0-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="003f0-343">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="003f0-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="003f0-344">0,08$</span><span class="sxs-lookup"><span data-stu-id="003f0-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="003f0-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="003f0-346">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="003f0-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="003f0-347">0,93$</span><span class="sxs-lookup"><span data-stu-id="003f0-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-348">Währung</span><span class="sxs-lookup"><span data-stu-id="003f0-348">Currency</span></span></td>
<td><p><span data-ttu-id="003f0-349">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="003f0-349">Currency type.</span></span> <span data-ttu-id="003f0-350">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="003f0-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="003f0-351">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="003f0-352">EUR</span><span class="sxs-lookup"><span data-stu-id="003f0-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="003f0-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="003f0-354">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="003f0-354">Pretax price per unit.</span></span> <span data-ttu-id="003f0-355">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="003f0-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="003f0-356">0,08$</span><span class="sxs-lookup"><span data-stu-id="003f0-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="003f0-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="003f0-358">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="003f0-358">Post tax price per unit.</span></span> <span data-ttu-id="003f0-359">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="003f0-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="003f0-360">0,08$</span><span class="sxs-lookup"><span data-stu-id="003f0-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="003f0-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="003f0-362">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="003f0-362">The type of charge or adjustment.</span></span> <span data-ttu-id="003f0-363">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="003f0-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="003f0-364">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="003f0-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="003f0-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="003f0-366">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="003f0-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="003f0-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="003f0-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="003f0-369">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="003f0-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="003f0-370">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="003f0-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="003f0-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="003f0-372">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="003f0-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="003f0-373">Ostasien, Südostasien, Nordeuropa, Westeuropa, Vereinigte Staaten (Mitte/Norden), Vereinigte Staaten (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="003f0-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="003f0-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="003f0-375">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="003f0-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="003f0-376">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="003f0-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="003f0-377">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="003f0-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="003f0-378">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="003f0-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="003f0-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="003f0-380">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="003f0-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="003f0-381">EXTERN</span><span class="sxs-lookup"><span data-stu-id="003f0-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-382">Projekt</span><span class="sxs-lookup"><span data-stu-id="003f0-382">Project</span></span></td>
<td><p><span data-ttu-id="003f0-383">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="003f0-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="003f0-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="003f0-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="003f0-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="003f0-386">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="003f0-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="003f0-387">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="003f0-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="003f0-388">Wenn ein Paket von 25 ServiceBus-Verbindungen bereitgestellt wurden und Sie an diesem Tag 1 genutzt haben, wird als tägliche Nutzung für diesen Tag „25 Verbindungen/30 Tage – Verwendet: 1,000000“ angegeben.</span><span class="sxs-lookup"><span data-stu-id="003f0-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="003f0-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="003f0-390">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="003f0-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="003f0-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="003f0-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="003f0-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="003f0-392">DomainName</span></span></td>
<td><p><span data-ttu-id="003f0-393">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="003f0-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="003f0-394">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="003f0-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="003f0-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="003f0-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="003f0-396">Einheit</span><span class="sxs-lookup"><span data-stu-id="003f0-396">Unit</span></span></td>
<td><p><span data-ttu-id="003f0-397">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="003f0-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="003f0-398">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="003f0-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="003f0-399">Feld für das einmalige Erwerben der Datei</span><span class="sxs-lookup"><span data-stu-id="003f0-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="003f0-400">Feld</span><span class="sxs-lookup"><span data-stu-id="003f0-400">Field</span></span>** |**<span data-ttu-id="003f0-401">Definition</span><span class="sxs-lookup"><span data-stu-id="003f0-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="003f0-402">PartnerID</span><span class="sxs-lookup"><span data-stu-id="003f0-402">PartnerId</span></span> |<span data-ttu-id="003f0-403">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="003f0-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="003f0-404">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="003f0-404">CustomerId</span></span> |<span data-ttu-id="003f0-405">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="003f0-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="003f0-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="003f0-406">CustomerName</span></span> |<span data-ttu-id="003f0-407">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="003f0-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="003f0-408">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="003f0-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="003f0-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="003f0-409">CustomerDomainName</span></span> |<span data-ttu-id="003f0-410">Domänenname des Kunden.</span><span class="sxs-lookup"><span data-stu-id="003f0-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="003f0-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="003f0-411">CustomerCountry</span></span> |<span data-ttu-id="003f0-412">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="003f0-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="003f0-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="003f0-413">InvoiceNumber</span></span> |<span data-ttu-id="003f0-414">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="003f0-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="003f0-415">MPNID</span><span class="sxs-lookup"><span data-stu-id="003f0-415">MpnId</span></span> |<span data-ttu-id="003f0-416">Die MPN-ID des CSP Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="003f0-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="003f0-417">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="003f0-417">Reseller MPN ID</span></span> |<span data-ttu-id="003f0-418">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="003f0-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="003f0-419">Die MPN-ID des registrierten Handelspartners für die Reservierung.</span><span class="sxs-lookup"><span data-stu-id="003f0-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="003f0-420">Dies entspricht der Handelspartner-ID, die für die spezifische Reservierung im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="003f0-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="003f0-421">Wenn ein CSP-Partner die Reservierung direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="003f0-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="003f0-422">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="003f0-423">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="003f0-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="003f0-424">OrderID</span><span class="sxs-lookup"><span data-stu-id="003f0-424">OrderId</span></span> |<span data-ttu-id="003f0-425">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="003f0-426">Kann beim Kontakt zum Support zum Identifizieren von Azur Reservations hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="003f0-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="003f0-427">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="003f0-427">OrderDate</span></span> |<span data-ttu-id="003f0-428">Der Zeitpunkt der Auftragserstellung.</span><span class="sxs-lookup"><span data-stu-id="003f0-428">The date the order was placed.</span></span> |
|<span data-ttu-id="003f0-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="003f0-429">ProductId</span></span> |<span data-ttu-id="003f0-430">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="003f0-430">The ID for the product.</span></span> |
|<span data-ttu-id="003f0-431">SkuID</span><span class="sxs-lookup"><span data-stu-id="003f0-431">SkuId</span></span>  |<span data-ttu-id="003f0-432">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="003f0-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="003f0-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="003f0-433">AvailabilityId</span></span> |<span data-ttu-id="003f0-434">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="003f0-434">The ID for a particular Availability.</span></span> <span data-ttu-id="003f0-435">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="003f0-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="003f0-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="003f0-436">SkuName</span></span>  |<span data-ttu-id="003f0-437">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="003f0-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="003f0-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="003f0-438">ProductName</span></span> |<span data-ttu-id="003f0-439">Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="003f0-439">The name of the product.</span></span> |
|<span data-ttu-id="003f0-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="003f0-440">ChargeType</span></span> |<span data-ttu-id="003f0-441">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="003f0-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="003f0-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="003f0-442">UnitPrice</span></span> |<span data-ttu-id="003f0-443">Preis pro bestelltem Produkt.</span><span class="sxs-lookup"><span data-stu-id="003f0-443">Price per product ordered.</span></span> |
|<span data-ttu-id="003f0-444">Anzahl</span><span class="sxs-lookup"><span data-stu-id="003f0-444">Quantity</span></span> |<span data-ttu-id="003f0-445">Anzahl der bestellten Produkte.</span><span class="sxs-lookup"><span data-stu-id="003f0-445">Number of products ordered.</span></span> |
|<span data-ttu-id="003f0-446">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="003f0-446">Subtotal</span></span> |<span data-ttu-id="003f0-447">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="003f0-447">Total before tax.</span></span> <span data-ttu-id="003f0-448">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="003f0-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="003f0-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="003f0-449">TaxTotal</span></span> |<span data-ttu-id="003f0-450">Die Summe aller anwendbaren Steuern.</span><span class="sxs-lookup"><span data-stu-id="003f0-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="003f0-451">Gesamt</span><span class="sxs-lookup"><span data-stu-id="003f0-451">Total</span></span> |<span data-ttu-id="003f0-452">Dies ist die Gesamtanzahl der Käufe.</span><span class="sxs-lookup"><span data-stu-id="003f0-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="003f0-453">Währung</span><span class="sxs-lookup"><span data-stu-id="003f0-453">Currency</span></span> |<span data-ttu-id="003f0-454">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="003f0-454">Currency type.</span></span> <span data-ttu-id="003f0-455">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="003f0-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="003f0-456">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="003f0-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="003f0-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="003f0-457">DiscountDetails</span></span> |<span data-ttu-id="003f0-458">Detaillierte Liste der relevanten Rabatte.</span><span class="sxs-lookup"><span data-stu-id="003f0-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="003f0-459">Siehe Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</span><span class="sxs-lookup"><span data-stu-id="003f0-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="003f0-460">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="003f0-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="003f0-461">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="003f0-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="003f0-462">Sowohl nutzungsbasierte als auch lizenzbasierte Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zusammenhängende Kosten).</span><span class="sxs-lookup"><span data-stu-id="003f0-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="003f0-463">Guthaben, Rabatte oder Erstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungsdatei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="003f0-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="003f0-464">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnittund zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="003f0-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="003f0-465">Beschreibung der Rechnungsgebühr</span><span class="sxs-lookup"><span data-stu-id="003f0-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="003f0-466">Gebührenbeschreibung der Abstimmungsdatei (ChargeType-Spalte)</span><span class="sxs-lookup"><span data-stu-id="003f0-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="003f0-467">Um welche Gebühr handelt es sich?</span><span class="sxs-lookup"><span data-stu-id="003f0-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="003f0-468">Wie ordne ich diese ChargeTypes der Rechnung zu?</span><span class="sxs-lookup"><span data-stu-id="003f0-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="003f0-469">Lizenzbasierte Gebühren</span><span class="sxs-lookup"><span data-stu-id="003f0-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="003f0-470">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="003f0-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-471">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="003f0-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="003f0-472">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-473">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="003f0-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-474">Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="003f0-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-475">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="003f0-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-476">Periodische Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="003f0-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-477">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="003f0-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-478">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</span><span class="sxs-lookup"><span data-stu-id="003f0-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-479">Gebühren bei Abbrechen anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="003f0-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-480">Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="003f0-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-481">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="003f0-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-482">Der Typ der Abrechnung für ein Abonnement bei Verwendung der jährlichen Abrechnung</span><span class="sxs-lookup"><span data-stu-id="003f0-482">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-483">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="003f0-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-484">Der Typ der Abrechnung für ein Abonnement Verwendung monatliche Abrechnung</span><span class="sxs-lookup"><span data-stu-id="003f0-484">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-485">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="003f0-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-486">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="003f0-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="003f0-487">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="003f0-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-488">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="003f0-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-489">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="003f0-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-490">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="003f0-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="003f0-491">Nutzungsgebühren</span><span class="sxs-lookup"><span data-stu-id="003f0-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="003f0-492">Nutzungsgebühr beim Abbrechen bewerten</span><span class="sxs-lookup"><span data-stu-id="003f0-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-493">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</span><span class="sxs-lookup"><span data-stu-id="003f0-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="003f0-494">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-495">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="003f0-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-496">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="003f0-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="003f0-497">Guthaben</span><span class="sxs-lookup"><span data-stu-id="003f0-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="003f0-498">Einen Artikel versetzen</span><span class="sxs-lookup"><span data-stu-id="003f0-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-499">Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="003f0-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-500">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="003f0-501">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="003f0-502">Nutzungsbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="003f0-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="003f0-503">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="003f0-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-504">Rabatt auf Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="003f0-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="003f0-505">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-506">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="003f0-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-507">Rabatt auf periodische Gebühren</span><span class="sxs-lookup"><span data-stu-id="003f0-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-508">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="003f0-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-509">Rabatt auf Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="003f0-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-510">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="003f0-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-511">Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="003f0-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="003f0-512">Lizenzbasierte Rabatte</span><span class="sxs-lookup"><span data-stu-id="003f0-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="003f0-513">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="003f0-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="003f0-514">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="003f0-515"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="003f0-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="003f0-516">Kann auf mehrere Gebührentypen angewendet werden</span><span class="sxs-lookup"><span data-stu-id="003f0-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="003f0-517">Ausnahme: "Einen Artikel versetzen" enthält bereits Steuern.</span><span class="sxs-lookup"><span data-stu-id="003f0-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="003f0-518">Siehe Guthaben, oben.</span><span class="sxs-lookup"><span data-stu-id="003f0-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="003f0-519">Steuern oder Umsatzsteuern (Umsatzsteuer)</span><span class="sxs-lookup"><span data-stu-id="003f0-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="003f0-520">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="003f0-521">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="003f0-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
