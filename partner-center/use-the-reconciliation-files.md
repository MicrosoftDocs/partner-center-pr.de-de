---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Für eine ausführliche Zeilenelement Ansicht jeder kostenlos in einem Abrechnungszyklus Laden Sie die abstimmungsdateien von Partner Center herunter.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 9997b01c76dacb736baa33f458def0b820753f1d
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682508"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="f9c5d-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="f9c5d-103">Use the reconciliation files</span></span>

<span data-ttu-id="f9c5d-104">**Gilt für**</span><span class="sxs-lookup"><span data-stu-id="f9c5d-104">**Applies to**</span></span>

-  <span data-ttu-id="f9c5d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="f9c5d-105">Partner Center</span></span>
-  <span data-ttu-id="f9c5d-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f9c5d-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="f9c5d-107">Für eine ausführliche Zeilenelement Ansicht jeder kostenlos in einem Abrechnungszyklus Laden Sie die abstimmungsdateien von Partner Center herunter.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="f9c5d-108">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z. B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="f9c5d-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="f9c5d-109">Vom Partner aufschlüsseln</span><span class="sxs-lookup"><span data-stu-id="f9c5d-109">Itemize by partner</span></span>


<span data-ttu-id="f9c5d-110">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f9c5d-111">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-111">MPN ID</span></span></th>
<th><span data-ttu-id="f9c5d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f9c5d-113">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="f9c5d-114">Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="f9c5d-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-115">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="f9c5d-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="f9c5d-116">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="f9c5d-117">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f9c5d-118">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="f9c5d-119">eTo anzeigen oder Aktualisieren der Reseller im Partner Center-Menü wählen <strong>Kunden</strong>, wählen Sie dann aus der Liste der Kunden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="f9c5d-120">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="f9c5d-121">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="f9c5d-122">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="f9c5d-123">Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="f9c5d-124">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="f9c5d-125">Lizenz-Datei-Felder</span><span class="sxs-lookup"><span data-stu-id="f9c5d-125">License-based file fields</span></span>


<span data-ttu-id="f9c5d-126">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f9c5d-127"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="f9c5d-128"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="f9c5d-129"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-130">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="f9c5d-131">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f9c5d-132">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f9c5d-133">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="f9c5d-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="f9c5d-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="f9c5d-136">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f9c5d-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="f9c5d-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-138">OrderID</span></span></td>
<td><p><span data-ttu-id="f9c5d-139">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f9c5d-140">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f9c5d-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f9c5d-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f9c5d-143">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f9c5d-144">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f9c5d-145">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="f9c5d-146">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="f9c5d-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f9c5d-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="f9c5d-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="f9c5d-149">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="f9c5d-150">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="f9c5d-151">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f9c5d-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="f9c5d-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-153">OfferID</span></span></td>
<td><p><span data-ttu-id="f9c5d-154">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-154">Unique offer ID.</span></span> <span data-ttu-id="f9c5d-155">Standard-Angebot-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="f9c5d-156"><b>Hinweis</b>: Dieser Wert entspricht nicht den Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="f9c5d-157">Siehe DurableOfferID unten.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="f9c5d-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="f9c5d-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="f9c5d-160">Eindeutige dauerhafte Angebot-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="f9c5d-161"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="f9c5d-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="f9c5d-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-163">OfferName</span></span></td>
<td><p><span data-ttu-id="f9c5d-164">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="f9c5d-165">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="f9c5d-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-167">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="f9c5d-168">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="f9c5d-169">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f9c5d-170">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f9c5d-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-172">Die Abonnement-Enddatum: 12 Monate + X Tage nach dem Startdatum (Partner Abrechnungsdatum in Anpassung an) oder 12 Monate ab Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="f9c5d-173">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="f9c5d-174">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="f9c5d-175">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f9c5d-176">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f9c5d-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-178">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="f9c5d-179">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f9c5d-180">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f9c5d-181">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f9c5d-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-183">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="f9c5d-184">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f9c5d-185">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f9c5d-186">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="f9c5d-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f9c5d-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="f9c5d-188">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-188">The type of charge or adjustment.</span></span> <span data-ttu-id="f9c5d-189">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="f9c5d-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f9c5d-190">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="f9c5d-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="f9c5d-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="f9c5d-192">Preis pro Arbeitsplatz, wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f9c5d-193">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f9c5d-194">6,82</span><span class="sxs-lookup"><span data-stu-id="f9c5d-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-195">Anzahl</span><span class="sxs-lookup"><span data-stu-id="f9c5d-195">Quantity</span></span></td>
<td><p><span data-ttu-id="f9c5d-196">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="f9c5d-196">Number of seats.</span></span> <span data-ttu-id="f9c5d-197">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f9c5d-198">2</span><span class="sxs-lookup"><span data-stu-id="f9c5d-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-199">Betrag</span><span class="sxs-lookup"><span data-stu-id="f9c5d-199">Amount</span></span></td>
<td><p><span data-ttu-id="f9c5d-200">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="f9c5d-200">Total of price for quantity.</span></span> <span data-ttu-id="f9c5d-201">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="f9c5d-202">13,32</span><span class="sxs-lookup"><span data-stu-id="f9c5d-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="f9c5d-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="f9c5d-204">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="f9c5d-205">IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="f9c5d-206">2,32</span><span class="sxs-lookup"><span data-stu-id="f9c5d-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-207">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="f9c5d-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="f9c5d-208">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="f9c5d-208">Total before tax.</span></span> <span data-ttu-id="f9c5d-209">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="f9c5d-210">11</span><span class="sxs-lookup"><span data-stu-id="f9c5d-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-211">Steuern</span><span class="sxs-lookup"><span data-stu-id="f9c5d-211">Tax</span></span></td>
<td><p><span data-ttu-id="f9c5d-212">Der steuerliche Aufwand basierend auf Ihren Markt&#39;steuerbestimmungen s und den jeweiligen Umständen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f9c5d-213">0</span><span class="sxs-lookup"><span data-stu-id="f9c5d-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="f9c5d-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="f9c5d-215">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-215">Total after tax.</span></span> <span data-ttu-id="f9c5d-216">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="f9c5d-217">11</span><span class="sxs-lookup"><span data-stu-id="f9c5d-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-218">Währung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-218">Currency</span></span></td>
<td><p><span data-ttu-id="f9c5d-219">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="f9c5d-219">Currency type.</span></span> <span data-ttu-id="f9c5d-220">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="f9c5d-221">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f9c5d-222">EUR</span><span class="sxs-lookup"><span data-stu-id="f9c5d-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="f9c5d-224">Kunden&#39;Organisationsname s, wie im Partner Center gemeldet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f9c5d-225">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f9c5d-226">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="f9c5d-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-227">MPNID</span></span></td>
<td><p><span data-ttu-id="f9c5d-228">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="f9c5d-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="f9c5d-229">4390934</span><span class="sxs-lookup"><span data-stu-id="f9c5d-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f9c5d-231">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f9c5d-232">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f9c5d-233">4390934</span><span class="sxs-lookup"><span data-stu-id="f9c5d-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-234">DomainName</span></span></td>
<td><p><span data-ttu-id="f9c5d-235">Kunden&#39;Domain Name, die zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f9c5d-236">Dies sollte nicht verwendet werden, zur eindeutigen Identifizierung des Kunden an, wie die Kunden bzw. des Partners die Vanity/Standard-Domäne über das Office 365-Portal aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f9c5d-237">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f9c5d-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f9c5d-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f9c5d-240">Abonnement-Nickname.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-240">Subscription nickname.</span></span> <span data-ttu-id="f9c5d-241">Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="f9c5d-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="f9c5d-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f9c5d-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f9c5d-244">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f9c5d-245">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="f9c5d-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="f9c5d-246">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="f9c5d-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="f9c5d-247">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="f9c5d-247">Usage-based file fields</span></span>


<span data-ttu-id="f9c5d-248">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="f9c5d-249">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f9c5d-250"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="f9c5d-251"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="f9c5d-252"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="f9c5d-254">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="f9c5d-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f9c5d-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="f9c5d-257">Partnername.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="f9c5d-258">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="f9c5d-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="f9c5d-260">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="f9c5d-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="f9c5d-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="f9c5d-263">Kunden&#39;Organisationsname s, wie im Partner Center gemeldet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f9c5d-264">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f9c5d-265">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="f9c5d-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-266">MPNID</span></span></td>
<td><p><span data-ttu-id="f9c5d-267">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="f9c5d-268">4390934</span><span class="sxs-lookup"><span data-stu-id="f9c5d-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f9c5d-270">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f9c5d-271">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f9c5d-272">4390934</span><span class="sxs-lookup"><span data-stu-id="f9c5d-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f9c5d-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f9c5d-274">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="f9c5d-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="f9c5d-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-277">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f9c5d-278">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f9c5d-279">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f9c5d-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-281">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f9c5d-282">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f9c5d-283">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="f9c5d-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f9c5d-285">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f9c5d-286">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f9c5d-287">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f9c5d-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f9c5d-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f9c5d-290">Nickname des Service-Angebots.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="f9c5d-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f9c5d-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f9c5d-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f9c5d-293">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="f9c5d-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="f9c5d-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f9c5d-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-295">OrderID</span></span></td>
<td><p><span data-ttu-id="f9c5d-296">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f9c5d-297">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f9c5d-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f9c5d-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="f9c5d-300">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="f9c5d-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="f9c5d-301">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="f9c5d-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="f9c5d-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="f9c5d-303">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f9c5d-304">Service Bus – einzeln oder als Paket</span><span class="sxs-lookup"><span data-stu-id="f9c5d-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="f9c5d-305">SQL Azure-Datenbank – Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="f9c5d-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="f9c5d-307">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="f9c5d-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f9c5d-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-309">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="f9c5d-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="f9c5d-310">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f9c5d-311">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="f9c5d-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="f9c5d-312">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="f9c5d-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-313">Region</span><span class="sxs-lookup"><span data-stu-id="f9c5d-313">Region</span></span></td>
<td><p><span data-ttu-id="f9c5d-314">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-314">The region the usage applies to.</span></span> <span data-ttu-id="f9c5d-315">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="f9c5d-316">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="f9c5d-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-317">SKU</span><span class="sxs-lookup"><span data-stu-id="f9c5d-317">SKU</span></span></td>
<td><p><span data-ttu-id="f9c5d-318">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="f9c5d-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="f9c5d-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="f9c5d-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="f9c5d-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="f9c5d-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="f9c5d-321">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="f9c5d-322">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="f9c5d-323">1</span><span class="sxs-lookup"><span data-stu-id="f9c5d-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="f9c5d-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="f9c5d-325">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="f9c5d-326">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="f9c5d-327">11</span><span class="sxs-lookup"><span data-stu-id="f9c5d-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="f9c5d-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="f9c5d-329">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-329">Units included as part of the offer.</span></span> <span data-ttu-id="f9c5d-330">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="f9c5d-331">0</span><span class="sxs-lookup"><span data-stu-id="f9c5d-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f9c5d-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="f9c5d-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="f9c5d-333">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="f9c5d-334">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="f9c5d-335">11</span><span class="sxs-lookup"><span data-stu-id="f9c5d-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="f9c5d-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="f9c5d-337">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="f9c5d-338">0,0808 $</span><span class="sxs-lookup"><span data-stu-id="f9c5d-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="f9c5d-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="f9c5d-340">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f9c5d-341">0,085 $</span><span class="sxs-lookup"><span data-stu-id="f9c5d-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="f9c5d-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="f9c5d-343">Der steuerliche Aufwand basierend auf Ihren Markt&#39;steuerbestimmungen s und den jeweiligen Umständen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f9c5d-344">0,08 $</span><span class="sxs-lookup"><span data-stu-id="f9c5d-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="f9c5d-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="f9c5d-346">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="f9c5d-347">0,93 $</span><span class="sxs-lookup"><span data-stu-id="f9c5d-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-348">Währung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-348">Currency</span></span></td>
<td><p><span data-ttu-id="f9c5d-349">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="f9c5d-349">Currency type.</span></span> <span data-ttu-id="f9c5d-350">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="f9c5d-351">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f9c5d-352">EUR</span><span class="sxs-lookup"><span data-stu-id="f9c5d-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f9c5d-354">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-354">Pretax price per unit.</span></span> <span data-ttu-id="f9c5d-355">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f9c5d-356">0,08 $</span><span class="sxs-lookup"><span data-stu-id="f9c5d-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f9c5d-358">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-358">Post tax price per unit.</span></span> <span data-ttu-id="f9c5d-359">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f9c5d-360">0,08 $</span><span class="sxs-lookup"><span data-stu-id="f9c5d-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f9c5d-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="f9c5d-362">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-362">The type of charge or adjustment.</span></span> <span data-ttu-id="f9c5d-363">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="f9c5d-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f9c5d-364">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="f9c5d-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="f9c5d-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="f9c5d-366">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="f9c5d-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="f9c5d-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-369">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="f9c5d-370">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f9c5d-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="f9c5d-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="f9c5d-372">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="f9c5d-373">Ostasien, Südostasien, Nordeuropa, Westeuropa, USA (Mitte/Norden), USA (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="f9c5d-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="f9c5d-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="f9c5d-375">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="f9c5d-376">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="f9c5d-377">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="f9c5d-378">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="f9c5d-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="f9c5d-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="f9c5d-380">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="f9c5d-381">EXTERN</span><span class="sxs-lookup"><span data-stu-id="f9c5d-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-382">Projekt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-382">Project</span></span></td>
<td><p><span data-ttu-id="f9c5d-383">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="f9c5d-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="f9c5d-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f9c5d-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="f9c5d-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="f9c5d-386">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="f9c5d-387">Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="f9c5d-388">Wenn Sie ein 25-Paket von Service Bus-Verbindungen, die bereitgestellt mussten, und Sie haben 1 während des Tages verwendet, würde Ihre Anweisung zur täglichen Nutzung für diesen Tag angeben "25 Verbindungen / 30 Tage – verwendet: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="f9c5d-390">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f9c5d-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f9c5d-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f9c5d-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-392">DomainName</span></span></td>
<td><p><span data-ttu-id="f9c5d-393">Kunden&#39;Domain Name, die zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f9c5d-394">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f9c5d-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f9c5d-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="f9c5d-396">Einheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-396">Unit</span></span></td>
<td><p><span data-ttu-id="f9c5d-397">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="f9c5d-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="f9c5d-398">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="f9c5d-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="f9c5d-399">Einmalige Ausführungen und zeitplanserien Dateifelder</span><span class="sxs-lookup"><span data-stu-id="f9c5d-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f9c5d-400">Column</span><span class="sxs-lookup"><span data-stu-id="f9c5d-400">Column</span></span></th>
<th><span data-ttu-id="f9c5d-401">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="f9c5d-402">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="f9c5d-403">Eindeutiger Bezeichner für Microsoft Azure Active Directory-Mandanten für eine bestimmte Entität Abrechnung, im GUID-Format '.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f9c5d-404">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f9c5d-405">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-406">Kunden-Id</span><span class="sxs-lookup"><span data-stu-id="f9c5d-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="f9c5d-407">Eindeutige Microsoft Azure Active Directory-Mandanten-ID im GUID-Format, die zum Identifizieren des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-408">Kundenname</span><span class="sxs-lookup"><span data-stu-id="f9c5d-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="f9c5d-409">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f9c5d-411">Kundendomänenname: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="f9c5d-412">Dies sollte nicht verwendet werden, zur eindeutigen Identifizierung des Kunden an, wie die Kunden bzw. des Partners die Vanity/Standard-Domäne über das Office 365-Portal aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f9c5d-413">Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-414">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="f9c5d-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="f9c5d-415">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-416">Rechnungsnummer</span><span class="sxs-lookup"><span data-stu-id="f9c5d-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="f9c5d-417">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-418">MPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-418">MpnId</span></span></td>
<td><p><span data-ttu-id="f9c5d-419">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-420">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="f9c5d-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="f9c5d-421">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-422">Bestellnummer</span><span class="sxs-lookup"><span data-stu-id="f9c5d-422">Order ID</span></span></td>
<td><p><span data-ttu-id="f9c5d-423">Eindeutiger Bezeichner für einen Auftrag in Microsoft Commerce-Plattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="f9c5d-424">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-425">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="f9c5d-425">Order date</span></span></td>
<td><p><span data-ttu-id="f9c5d-426">Der Zeitpunkt der Auftragserstellung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-427">ProductID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-427">ProductId</span></span></td>
<td><p><span data-ttu-id="f9c5d-428">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-429">SkuID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-429">SkuId</span></span></td>
<td><p><span data-ttu-id="f9c5d-430">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f9c5d-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f9c5d-432">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-432">The ID for a particular Availability.</span></span> <span data-ttu-id="f9c5d-433">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-434">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="f9c5d-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="f9c5d-435">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-436">Produktname</span><span class="sxs-lookup"><span data-stu-id="f9c5d-436">Product name</span></span></td>
<td><p><span data-ttu-id="f9c5d-437">Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="f9c5d-439">Der Name des Verlegers des Produkts.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="f9c5d-441">Eindeutige ID für diesen Verleger.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-442">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f9c5d-443">Der Anzeigename eines Abonnements.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-444">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f9c5d-445">Eindeutiger Bezeichner für ein Abonnement in Microsoft Commerce-Plattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="f9c5d-446">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f9c5d-447">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-449">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-449">Start day of the charges.</span></span> <span data-ttu-id="f9c5d-450">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-452">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-452">End day of the charges.</span></span> <span data-ttu-id="f9c5d-453">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-454">Begriff und Billingcycle</span><span class="sxs-lookup"><span data-stu-id="f9c5d-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="f9c5d-455">Die Dauer und dem Abrechnungszyklus für den Kauf.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="f9c5d-456">Z. B. "1 Jahr, monatliche."</span><span class="sxs-lookup"><span data-stu-id="f9c5d-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-457">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="f9c5d-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="f9c5d-458">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-459">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="f9c5d-460">Der Preis der Pricelist zum Zeitpunkt des Kaufs, veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f9c5d-461">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-462">Effektive Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="f9c5d-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="f9c5d-463">Der Preis nach Anpassungen vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-464">Anzahl</span><span class="sxs-lookup"><span data-stu-id="f9c5d-464">Quantity</span></span></td>
<td><p><span data-ttu-id="f9c5d-465">Anzahl der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-465">Number of units.</span></span> <span data-ttu-id="f9c5d-466">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-467">Unit-Typ</span><span class="sxs-lookup"><span data-stu-id="f9c5d-467">Unit type</span></span></td>
<td><p><span data-ttu-id="f9c5d-468">Der Typ der Einheit gekauft wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="f9c5d-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="f9c5d-470">Eine Erklärung der Rabatt gilt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-471">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="f9c5d-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="f9c5d-472">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="f9c5d-472">Total before tax.</span></span> <span data-ttu-id="f9c5d-473">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-474">Gesamte steuern</span><span class="sxs-lookup"><span data-stu-id="f9c5d-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="f9c5d-475">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-476">Gesamt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-476">Total</span></span></td>
<td><p><span data-ttu-id="f9c5d-477">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-477">Total after tax.</span></span> <span data-ttu-id="f9c5d-478">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-479">Währung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-479">Currency</span></span></td>
<td><p><span data-ttu-id="f9c5d-480">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="f9c5d-480">Currency type.</span></span> <span data-ttu-id="f9c5d-481">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="f9c5d-482">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="f9c5d-484">Ein alternativer Bezeichner, der eine Auftrags-ID.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-484">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="f9c5d-485">Täglich anteilig Datei verwendungsfelder</span><span class="sxs-lookup"><span data-stu-id="f9c5d-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f9c5d-486">Column</span><span class="sxs-lookup"><span data-stu-id="f9c5d-486">Column</span></span></th>
<th><span data-ttu-id="f9c5d-487">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="f9c5d-488">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="f9c5d-489">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="f9c5d-491">Partnername.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-492">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="f9c5d-493">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="f9c5d-495">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="f9c5d-496">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f9c5d-498">Domänenname des Kunden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-498">The customer’s domain name.</span></span> <span data-ttu-id="f9c5d-499">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-500">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="f9c5d-500">Customer country</span></span></td>
<td><p><span data-ttu-id="f9c5d-501">Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-502">MPNID</span></span></td>
<td><p><span data-ttu-id="f9c5d-503">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-504">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="f9c5d-505">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f9c5d-506">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f9c5d-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f9c5d-508">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="f9c5d-509">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-510">ProductID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-510">ProductId</span></span></td>
<td><p><span data-ttu-id="f9c5d-511">Die ID für das Produkt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-512">SkuID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-512">SkuId</span></span></td>
<td><p><span data-ttu-id="f9c5d-513">Die ID für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f9c5d-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f9c5d-515">Die ID für eine bestimmte Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-515">The ID for a particular Availability.</span></span> <span data-ttu-id="f9c5d-516">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-517">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="f9c5d-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="f9c5d-518">Titel für eine bestimmte SKU.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f9c5d-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="f9c5d-520">Der Name des Verlegers.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="f9c5d-522">Die ID des Verlegers, im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="f9c5d-523">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="f9c5d-524">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f9c5d-525">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f9c5d-526">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="f9c5d-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-527">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="f9c5d-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f9c5d-528">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f9c5d-529">Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f9c5d-530">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-532">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f9c5d-533">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f9c5d-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f9c5d-535">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f9c5d-536">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-537">Nutzungsdatum</span><span class="sxs-lookup"><span data-stu-id="f9c5d-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="f9c5d-538">Datum der Nutzung des Diensts.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-539">Typ der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="f9c5d-540">Der Typ der Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-541">Kategorie der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="f9c5d-542">Dienst der obersten Ebene für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-543">Id der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="f9c5d-544">Die ID der Verbrauchseinheit, die verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-545">Unterkategorie der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="f9c5d-546">Der Typ des Azure-Dienst, der auf den Tarif auswirken kann.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-547">Name der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="f9c5d-548">Die Maßeinheit für die genutzte Verbrauchseinheit an.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-549">Region der abrechnungseinheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="f9c5d-550">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-551">Einheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-551">Unit</span></span></td>
<td><p><span data-ttu-id="f9c5d-552">Die Einheit der Name der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-553">Verbrauchte Menge</span><span class="sxs-lookup"><span data-stu-id="f9c5d-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="f9c5d-554">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="f9c5d-555">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-556">Ressourcenspeicherort</span><span class="sxs-lookup"><span data-stu-id="f9c5d-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="f9c5d-557">Das Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-558">Genutzter Dienst</span><span class="sxs-lookup"><span data-stu-id="f9c5d-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="f9c5d-559">Der Azure-Plattform-Dienst, den Sie verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-560">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="f9c5d-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="f9c5d-561">Die Ressourcengruppe, in der die bereitgestellte Verbrauchseinheit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-562">Ressourcen-URI</span><span class="sxs-lookup"><span data-stu-id="f9c5d-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="f9c5d-563">Der URI der Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-564">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="f9c5d-564">Charge type</span></span></td>
<td><p><span data-ttu-id="f9c5d-565">Art der Gebühren oder der Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-565">The type of charge or adjustment.</span></span> <span data-ttu-id="f9c5d-566">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-567">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="f9c5d-567">Unit price</span></span></td>
<td><p><span data-ttu-id="f9c5d-568">Preis pro-Lizenz, wie in der Pricelist zum Zeitpunkt des Kaufs veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f9c5d-569">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-570">Anzahl</span><span class="sxs-lookup"><span data-stu-id="f9c5d-570">Quantity</span></span></td>
<td><p><span data-ttu-id="f9c5d-571">Anzahl der Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-571">Number of licenses.</span></span> <span data-ttu-id="f9c5d-572">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-573">Unit-Typ</span><span class="sxs-lookup"><span data-stu-id="f9c5d-573">Unit type</span></span></td>
<td><p><span data-ttu-id="f9c5d-574">Der Typ der Einheit, die die Verbrauchseinheit in Rechnung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="f9c5d-575">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-576">Die Abrechnung vor Steuern</span><span class="sxs-lookup"><span data-stu-id="f9c5d-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="f9c5d-577">Die Gesamtmenge vor Steuern.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-578">Rechnungswährung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="f9c5d-579">Die Währung in geografischen Region des Kunden</span><span class="sxs-lookup"><span data-stu-id="f9c5d-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-580">Preise vor Steuern gesamt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="f9c5d-581">Die Preise, steuern hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-582">Preise von Währung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="f9c5d-583">Die Währung, in der Pricelist werden soll.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-584">Dienstinformationen 1</span><span class="sxs-lookup"><span data-stu-id="f9c5d-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="f9c5d-585">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-586">Dienstinformationen 2</span><span class="sxs-lookup"><span data-stu-id="f9c5d-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="f9c5d-587">Ein legacyfeld, die optionale dienstspezifische Metadaten erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f9c5d-588">Tags</span><span class="sxs-lookup"><span data-stu-id="f9c5d-588">Tags</span></span></td>
<td><p><span data-ttu-id="f9c5d-589">Tags, die Sie das Messgerät in der Reihenfolge zum Gruppieren von abrechnungsdatensätzen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="f9c5d-590">Beispielsweise können Sie Tags verwenden, um Kosten nach den Abteilungen zu unterteilen, die die Verbrauchseinheit nutzen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f9c5d-591">Zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="f9c5d-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="f9c5d-592">Zusätzliche Informationen in anderen Spalten nicht behandelt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="f9c5d-593">Zuordnung der Gebühren zwischen Rechnung und abstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="f9c5d-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="f9c5d-594">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="f9c5d-595">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="f9c5d-596">Sowohl nutzungsbasierte als auch lizenzbasierte Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zusammenhängende Kosten).</span><span class="sxs-lookup"><span data-stu-id="f9c5d-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="f9c5d-597">Guthaben, Rabatte oder Erstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungsdatei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="f9c5d-598">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnitt und zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="f9c5d-599"><strong>Beschreibung der Rechnungsgebühren</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-600"><strong>Abstimmung DateiBeschreibung (ChargeType-Spalte)</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-601"><strong>Was diese Gebühr ist?</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-602"><strong>Wie ordne ich dieser Gebührentypen zur Rechnung zu?</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="f9c5d-603"><strong>Lizenzbasierte Gebühren</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-604">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="f9c5d-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-605">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="f9c5d-606">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-607">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="f9c5d-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-608">Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-609">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="f9c5d-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-610">Periodische Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="f9c5d-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-611">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="f9c5d-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-612">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</span><span class="sxs-lookup"><span data-stu-id="f9c5d-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-613">Gebühren bei Abbrechen anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="f9c5d-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-614">Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-615">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="f9c5d-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-616">Der Typ der Gebühr für ein Abonnement bei Verwendung von jährliche Abrechnung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-617">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="f9c5d-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-618">Der Typ der Gebühr für ein Abonnement bei Verwendung der monatliche Abrechnung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-619">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-620">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="f9c5d-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="f9c5d-621">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="f9c5d-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-622">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="f9c5d-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-623">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="f9c5d-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-624">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="f9c5d-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="f9c5d-625"><strong>Nutzungsgebühren</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-626">Nutzungsgebühr beim Abbrechen bewerten</span><span class="sxs-lookup"><span data-stu-id="f9c5d-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-627">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</span><span class="sxs-lookup"><span data-stu-id="f9c5d-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="f9c5d-628">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-629">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="f9c5d-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-630">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="f9c5d-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-631"><strong>Guthaben</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-632">Einen Artikel versetzen</span><span class="sxs-lookup"><span data-stu-id="f9c5d-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-633">Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="f9c5d-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-634">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="f9c5d-635">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="f9c5d-636"><strong>Verwendungsbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-637">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-638">Rabatt auf Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="f9c5d-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="f9c5d-639">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-640">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-641">Rabatt auf periodische Gebühren</span><span class="sxs-lookup"><span data-stu-id="f9c5d-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-642">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-643">Rabatt auf Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="f9c5d-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-644">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="f9c5d-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-645">Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="f9c5d-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="f9c5d-646"><strong>Lizenzbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-647"><em>Kann für mehrere gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="f9c5d-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-648">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f9c5d-649"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="f9c5d-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-650"><em>Kann für mehrere gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="f9c5d-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="f9c5d-651"><em>Ausnahme: &quot;Ausgleich einer Position&quot; enthält bereits steuern. Finden Sie-Guthaben, oben ein.</em></span><span class="sxs-lookup"><span data-stu-id="f9c5d-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-652">Steuern oder Umsatzsteuern (Umsatzsteuer)</span><span class="sxs-lookup"><span data-stu-id="f9c5d-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="f9c5d-653">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="f9c5d-654">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="f9c5d-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
