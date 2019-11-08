---
title: Verwenden der Abstimmungsdateien | Partner Center
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Laden Sie die Kontenabstimmungsdateien aus dem Partner Center herunter, um ausführliche Informationen zu den einzelnen Rechnungspositionen der Gebühren in einem Abrechnungszyklus anzuzeigen.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753851"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="63c57-103">Verwenden der Abstimmungsdateien</span><span class="sxs-lookup"><span data-stu-id="63c57-103">Use the reconciliation files</span></span>

<span data-ttu-id="63c57-104">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="63c57-104">**Applies to**</span></span>

-  <span data-ttu-id="63c57-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="63c57-105">Partner Center</span></span>
-  <span data-ttu-id="63c57-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="63c57-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="63c57-107">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="63c57-107">**Appropriate roles**</span></span>

- <span data-ttu-id="63c57-108">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="63c57-108">Billing admin</span></span>
- <span data-ttu-id="63c57-109">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="63c57-109">Global admin</span></span>

<span data-ttu-id="63c57-110">Laden Sie die Kontenabstimmungsdateien aus dem Partner Center herunter, um ausführliche Informationen zu den einzelnen Rechnungspositionen der Gebühren in einem Abrechnungszyklus anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="63c57-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="63c57-111">Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z. B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).</span><span class="sxs-lookup"><span data-stu-id="63c57-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="63c57-112">Formatierungsprobleme</span><span class="sxs-lookup"><span data-stu-id="63c57-112">Formatting issues</span></span>

<span data-ttu-id="63c57-113">Gelegentlich kann die Kontenabstimmungsdatei Formatierungsprobleme aufweisen.</span><span class="sxs-lookup"><span data-stu-id="63c57-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="63c57-114">(Dies kann beispielsweise der Fall sein, wenn das Gebiets Schema "en-US" nicht verwendet wird.) Führen Sie die folgenden Schritte aus, um diese Probleme zu beheben.</span><span class="sxs-lookup"><span data-stu-id="63c57-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="63c57-115">Öffnen Sie die CSV-Datei in Excel, und wählen Sie die erste Spalte aus.</span><span class="sxs-lookup"><span data-stu-id="63c57-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="63c57-116">Klicken Sie auf dem Menüband auf <strong>Daten</strong> und dann auf <strong>Text in Spalten</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="63c57-117">Wählen Sie im Textkonvertierungs-Assistenten <strong>Dateityp „Getrennt“</strong> aus, und klicken Sie dann auf <strong>Weiter</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="63c57-118">Wählen Sie im Feld „Trennzeichen“ <strong>Komma</strong> aus.</span><span class="sxs-lookup"><span data-stu-id="63c57-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="63c57-119">Wenn <strong>Tabstopp</strong> bereits ausgewählt ist, übernehmen Sie diese Einstellung.</span><span class="sxs-lookup"><span data-stu-id="63c57-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="63c57-120">Wählen Sie <strong>Weiter</strong> aus.</span><span class="sxs-lookup"><span data-stu-id="63c57-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="63c57-121">Wählen Sie im Feld Spaltendaten Format die Option <strong>Date: mdy</strong>aus, und klicken Sie dann auf <strong>weiter</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="63c57-122">Wählen Sie im Feld „Datenformat der Spalten“ für alle Betragsspalten <strong>Text</strong> aus, und klicken Sie dann auf <strong>Fertig stellen</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="63c57-123">Herunterladen einer großen Datei für das herunterladen</span><span class="sxs-lookup"><span data-stu-id="63c57-123">Downloading a large recon file</span></span>

<span data-ttu-id="63c57-124">Das Herunterladen von Dateien kann sehr groß werden und ist manchmal schwierig.</span><span class="sxs-lookup"><span data-stu-id="63c57-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="63c57-125">Ein PowerShell-Skript, das Sie beim Herunterladen umfangreicher Datei Dateien unterstützt, finden Sie unter [Get Rechnungs Items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="63c57-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="63c57-126">Aufschlüsseln nach Partner</span><span class="sxs-lookup"><span data-stu-id="63c57-126">Itemize by partner</span></span>


<span data-ttu-id="63c57-127">Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="63c57-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="63c57-128">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-128">MPN ID</span></span></th>
<th><span data-ttu-id="63c57-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="63c57-130">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="63c57-131">Die Microsoft Partner Network-ID (MPN) des CSP-Partners (direkt oder indirekt).</span><span class="sxs-lookup"><span data-stu-id="63c57-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-132">MPN-ID der Handelspartner</span><span class="sxs-lookup"><span data-stu-id="63c57-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="63c57-133">Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</span><span class="sxs-lookup"><span data-stu-id="63c57-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="63c57-134">Die MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="63c57-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="63c57-135">Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="63c57-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="63c57-136">Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Partner Center-Menü <strong>Kunden</strong> und dann den Kunden in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="63c57-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="63c57-137">Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="63c57-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="63c57-138">Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</span><span class="sxs-lookup"><span data-stu-id="63c57-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="63c57-139">Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</span><span class="sxs-lookup"><span data-stu-id="63c57-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="63c57-140">Wenn ein CSP-Partner über einen Reseller ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="63c57-141">Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="63c57-142">Lizenzbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="63c57-142">License-based file fields</span></span>


<span data-ttu-id="63c57-143">Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus Partner Center.</span><span class="sxs-lookup"><span data-stu-id="63c57-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="63c57-144"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="63c57-145"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="63c57-146"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-147">PartnerID</span><span class="sxs-lookup"><span data-stu-id="63c57-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="63c57-148">Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="63c57-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="63c57-149">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="63c57-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="63c57-150">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="63c57-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="63c57-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="63c57-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-152">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="63c57-153">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="63c57-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="63c57-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="63c57-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="63c57-155">OrderID</span></span></td>
<td><p><span data-ttu-id="63c57-156">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="63c57-157">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="63c57-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="63c57-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="63c57-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="63c57-160">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="63c57-161">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="63c57-162">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="63c57-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="63c57-163">Siehe Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="63c57-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="63c57-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="63c57-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="63c57-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="63c57-166">Eindeutiger Bezeichner des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="63c57-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="63c57-167">Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</span><span class="sxs-lookup"><span data-stu-id="63c57-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="63c57-168">Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="63c57-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="63c57-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="63c57-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="63c57-170">OfferID</span></span></td>
<td><p><span data-ttu-id="63c57-171">Eindeutige Angebot-ID.</span><span class="sxs-lookup"><span data-stu-id="63c57-171">Unique offer ID.</span></span> <span data-ttu-id="63c57-172">Standard-Angebots-ID gemäß der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="63c57-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="63c57-173"><b>Hinweis</b>: Dieser Wert entspricht nicht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="63c57-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="63c57-174">Siehe „DurableOfferID“ unten.</span><span class="sxs-lookup"><span data-stu-id="63c57-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="63c57-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="63c57-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="63c57-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="63c57-177">Eindeutige dauerhafte Angebots-ID gemäß Definition in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="63c57-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="63c57-178"><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="63c57-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="63c57-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="63c57-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="63c57-180">OfferName</span></span></td>
<td><p><span data-ttu-id="63c57-181">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="63c57-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="63c57-182">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="63c57-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="63c57-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="63c57-184">Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung.</span><span class="sxs-lookup"><span data-stu-id="63c57-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="63c57-185">Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</span><span class="sxs-lookup"><span data-stu-id="63c57-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="63c57-186">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="63c57-187">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="63c57-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="63c57-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="63c57-189">Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</span><span class="sxs-lookup"><span data-stu-id="63c57-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="63c57-190">Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="63c57-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="63c57-191">Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63c57-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="63c57-192">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="63c57-193">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="63c57-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="63c57-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="63c57-195">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="63c57-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="63c57-196">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="63c57-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="63c57-197">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="63c57-198">01.02.2015 0:00</span><span class="sxs-lookup"><span data-stu-id="63c57-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="63c57-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="63c57-200">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="63c57-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="63c57-201">Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</span><span class="sxs-lookup"><span data-stu-id="63c57-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="63c57-202">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="63c57-203">28.2.2015 23:59</span><span class="sxs-lookup"><span data-stu-id="63c57-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="63c57-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="63c57-205">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="63c57-205">The type of charge or adjustment.</span></span> <span data-ttu-id="63c57-206">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="63c57-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="63c57-207">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="63c57-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="63c57-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="63c57-209">Preis pro Arbeitsplatz entsprechend der Preisliste zum Kaufzeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="63c57-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="63c57-210">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="63c57-211">6,82</span><span class="sxs-lookup"><span data-stu-id="63c57-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-212">Anzahl</span><span class="sxs-lookup"><span data-stu-id="63c57-212">Quantity</span></span></td>
<td><p><span data-ttu-id="63c57-213">Anzahl der Arbeitsplätze</span><span class="sxs-lookup"><span data-stu-id="63c57-213">Number of seats.</span></span> <span data-ttu-id="63c57-214">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="63c57-215">2</span><span class="sxs-lookup"><span data-stu-id="63c57-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-216">Betrag</span><span class="sxs-lookup"><span data-stu-id="63c57-216">Amount</span></span></td>
<td><p><span data-ttu-id="63c57-217">Gesamtpreis für die Menge</span><span class="sxs-lookup"><span data-stu-id="63c57-217">Total of price for quantity.</span></span> <span data-ttu-id="63c57-218">Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="63c57-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="63c57-219">13,32</span><span class="sxs-lookup"><span data-stu-id="63c57-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="63c57-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="63c57-221">Rabattbetrag auf diese Gebühren.</span><span class="sxs-lookup"><span data-stu-id="63c57-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="63c57-222">Produktlizenzen, die in einer Kompetenz oder in Karten oder neuen Abonnements enthalten sind, die für einen Anreiz geeignet sind, enthalten in dieser Spalte ebenfalls einen Rabatt Betrag.</span><span class="sxs-lookup"><span data-stu-id="63c57-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="63c57-223">2,32</span><span class="sxs-lookup"><span data-stu-id="63c57-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-224">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="63c57-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="63c57-225">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="63c57-225">Total before tax.</span></span> <span data-ttu-id="63c57-226">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="63c57-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="63c57-227">11</span><span class="sxs-lookup"><span data-stu-id="63c57-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-228">Steuern</span><span class="sxs-lookup"><span data-stu-id="63c57-228">Tax</span></span></td>
<td><p><span data-ttu-id="63c57-229">Steuerbetrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="63c57-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="63c57-230">0</span><span class="sxs-lookup"><span data-stu-id="63c57-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="63c57-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="63c57-232">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="63c57-232">Total after tax.</span></span> <span data-ttu-id="63c57-233">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="63c57-234">11</span><span class="sxs-lookup"><span data-stu-id="63c57-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-235">Währung</span><span class="sxs-lookup"><span data-stu-id="63c57-235">Currency</span></span></td>
<td><p><span data-ttu-id="63c57-236">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="63c57-236">Currency type.</span></span> <span data-ttu-id="63c57-237">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="63c57-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="63c57-238">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="63c57-239">EUR</span><span class="sxs-lookup"><span data-stu-id="63c57-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="63c57-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="63c57-241">Name der Organisation des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="63c57-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="63c57-242">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="63c57-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="63c57-243">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="63c57-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="63c57-244">MPNID</span></span></td>
<td><p><span data-ttu-id="63c57-245">MPN-ID des CSP-Partners</span><span class="sxs-lookup"><span data-stu-id="63c57-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="63c57-246">4390934</span><span class="sxs-lookup"><span data-stu-id="63c57-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="63c57-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="63c57-248">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="63c57-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="63c57-249">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="63c57-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="63c57-250">4390934</span><span class="sxs-lookup"><span data-stu-id="63c57-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="63c57-251">DomainName</span></span></td>
<td><p><span data-ttu-id="63c57-252">Name der Domäne des Kunden, der zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="63c57-253">Dieser Name darf nicht verwendet werden, um den Kunden eindeutig zu identifizieren, da der Kunde/Partner die Vanity-/Standarddomäne über das Office 365-Portal aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="63c57-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="63c57-254">Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="63c57-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="63c57-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="63c57-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="63c57-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="63c57-257">Spitzname des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="63c57-257">Subscription nickname.</span></span> <span data-ttu-id="63c57-258">Wenn kein Spitzname angegeben ist, verwendet Partner Center „OfferName“.</span><span class="sxs-lookup"><span data-stu-id="63c57-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="63c57-259">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="63c57-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="63c57-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="63c57-261">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="63c57-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="63c57-262">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="63c57-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="63c57-263">PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</span><span class="sxs-lookup"><span data-stu-id="63c57-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="63c57-264">Nutzungsbasierte Dateifelder</span><span class="sxs-lookup"><span data-stu-id="63c57-264">Usage-based file fields</span></span>


<span data-ttu-id="63c57-265">Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="63c57-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="63c57-266">Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.</span><span class="sxs-lookup"><span data-stu-id="63c57-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="63c57-267"><strong>Spalte</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="63c57-268"><strong>Beschreibung</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="63c57-269"><strong>Beispielwert</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="63c57-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="63c57-271">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="63c57-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="63c57-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="63c57-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="63c57-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="63c57-274">Partnername.</span><span class="sxs-lookup"><span data-stu-id="63c57-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="63c57-275">Acme integriert</span><span class="sxs-lookup"><span data-stu-id="63c57-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="63c57-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="63c57-277">Partner-Konto-ID.</span><span class="sxs-lookup"><span data-stu-id="63c57-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="63c57-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="63c57-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="63c57-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="63c57-280">Name der Organisation des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="63c57-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="63c57-281">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="63c57-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="63c57-282">Test für Kunde A</span><span class="sxs-lookup"><span data-stu-id="63c57-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="63c57-283">MPNID</span></span></td>
<td><p><span data-ttu-id="63c57-284">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="63c57-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="63c57-285">4390934</span><span class="sxs-lookup"><span data-stu-id="63c57-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="63c57-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="63c57-287">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="63c57-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="63c57-288">Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</span><span class="sxs-lookup"><span data-stu-id="63c57-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="63c57-289">4390934</span><span class="sxs-lookup"><span data-stu-id="63c57-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="63c57-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="63c57-291">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="63c57-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="63c57-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="63c57-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="63c57-294">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="63c57-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="63c57-295">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="63c57-296">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="63c57-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="63c57-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="63c57-298">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="63c57-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="63c57-299">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="63c57-300">28.02.2014 23:59</span><span class="sxs-lookup"><span data-stu-id="63c57-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="63c57-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="63c57-302">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="63c57-303">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="63c57-304">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="63c57-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="63c57-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="63c57-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="63c57-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="63c57-307">Spitzname des Dienstangebots.</span><span class="sxs-lookup"><span data-stu-id="63c57-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="63c57-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="63c57-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="63c57-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="63c57-310">Branche des Service-Angebots</span><span class="sxs-lookup"><span data-stu-id="63c57-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="63c57-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="63c57-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="63c57-312">OrderID</span></span></td>
<td><p><span data-ttu-id="63c57-313">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="63c57-314">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="63c57-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="63c57-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="63c57-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="63c57-317">Der Name des fraglichen Azure-Dienstes</span><span class="sxs-lookup"><span data-stu-id="63c57-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="63c57-318">VIRTUELLE COMPUTER</span><span class="sxs-lookup"><span data-stu-id="63c57-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="63c57-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="63c57-320">Der bestimmte Typ des Windows Azure-Dienstes.</span><span class="sxs-lookup"><span data-stu-id="63c57-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="63c57-321">Service Bus einzeln oder Paket</span><span class="sxs-lookup"><span data-stu-id="63c57-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="63c57-322">SQL Azure Datenbank-Business oder Web Edition</span><span class="sxs-lookup"><span data-stu-id="63c57-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="63c57-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="63c57-324">Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</span><span class="sxs-lookup"><span data-stu-id="63c57-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="63c57-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="63c57-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-326">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="63c57-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="63c57-327">Der Name der Azure-Ressource.</span><span class="sxs-lookup"><span data-stu-id="63c57-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="63c57-328">Übertragung eingehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="63c57-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="63c57-329">Übertragung ausgehender Daten (GB)</span><span class="sxs-lookup"><span data-stu-id="63c57-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-330">Region</span><span class="sxs-lookup"><span data-stu-id="63c57-330">Region</span></span></td>
<td><p><span data-ttu-id="63c57-331">Die Region, auf die sich die Nutzung bezieht.</span><span class="sxs-lookup"><span data-stu-id="63c57-331">The region the usage applies to.</span></span> <span data-ttu-id="63c57-332">Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="63c57-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="63c57-333">Asien-Pazifik, Europa, Lateinamerika, Nordamerika</span><span class="sxs-lookup"><span data-stu-id="63c57-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-334">SKU</span><span class="sxs-lookup"><span data-stu-id="63c57-334">SKU</span></span></td>
<td><p><span data-ttu-id="63c57-335">MSFT eindeutiger Bezeichner für das Angebot</span><span class="sxs-lookup"><span data-stu-id="63c57-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="63c57-336">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="63c57-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="63c57-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="63c57-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="63c57-338">Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum.</span><span class="sxs-lookup"><span data-stu-id="63c57-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="63c57-339">Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</span><span class="sxs-lookup"><span data-stu-id="63c57-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="63c57-340">1</span><span class="sxs-lookup"><span data-stu-id="63c57-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="63c57-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="63c57-342">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="63c57-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="63c57-343">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="63c57-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="63c57-344">11</span><span class="sxs-lookup"><span data-stu-id="63c57-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="63c57-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="63c57-346">Enthaltene Einheiten als Teil des Angebots.</span><span class="sxs-lookup"><span data-stu-id="63c57-346">Units included as part of the offer.</span></span> <span data-ttu-id="63c57-347">In der Regel nicht im CSP vorhanden.</span><span class="sxs-lookup"><span data-stu-id="63c57-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="63c57-348">0</span><span class="sxs-lookup"><span data-stu-id="63c57-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="63c57-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="63c57-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="63c57-350">Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="63c57-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="63c57-351">Gleich ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="63c57-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="63c57-352">11</span><span class="sxs-lookup"><span data-stu-id="63c57-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="63c57-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="63c57-354">Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="63c57-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="63c57-355">0,0808 $</span><span class="sxs-lookup"><span data-stu-id="63c57-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="63c57-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="63c57-357">ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="63c57-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="63c57-358">0,085 $</span><span class="sxs-lookup"><span data-stu-id="63c57-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="63c57-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="63c57-360">Steuerbetrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="63c57-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="63c57-361">0,08 $</span><span class="sxs-lookup"><span data-stu-id="63c57-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="63c57-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="63c57-363">Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="63c57-364">0,93 $</span><span class="sxs-lookup"><span data-stu-id="63c57-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-365">Währung</span><span class="sxs-lookup"><span data-stu-id="63c57-365">Currency</span></span></td>
<td><p><span data-ttu-id="63c57-366">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="63c57-366">Currency type.</span></span> <span data-ttu-id="63c57-367">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="63c57-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="63c57-368">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="63c57-369">EUR</span><span class="sxs-lookup"><span data-stu-id="63c57-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="63c57-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="63c57-371">Nettopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="63c57-371">Pretax price per unit.</span></span> <span data-ttu-id="63c57-372">Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="63c57-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="63c57-373">0,08 $</span><span class="sxs-lookup"><span data-stu-id="63c57-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="63c57-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="63c57-375">Bruttopreis pro Einheit.</span><span class="sxs-lookup"><span data-stu-id="63c57-375">Post tax price per unit.</span></span> <span data-ttu-id="63c57-376">Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</span><span class="sxs-lookup"><span data-stu-id="63c57-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="63c57-377">0,08 $</span><span class="sxs-lookup"><span data-stu-id="63c57-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="63c57-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="63c57-379">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="63c57-379">The type of charge or adjustment.</span></span> <span data-ttu-id="63c57-380">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="63c57-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="63c57-381">Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</a></span><span class="sxs-lookup"><span data-stu-id="63c57-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="63c57-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="63c57-383">Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="63c57-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="63c57-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="63c57-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="63c57-386">Datum der Service-Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="63c57-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="63c57-387">01.02.2014 0:00</span><span class="sxs-lookup"><span data-stu-id="63c57-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="63c57-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="63c57-389">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="63c57-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="63c57-390">Ostasien, Südostasien, Nordeuropa, Westeuropa, Vereinigte Staaten (Mitte/Norden), Vereinigte Staaten (Mitte/Süden)</span><span class="sxs-lookup"><span data-stu-id="63c57-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="63c57-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="63c57-392">Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist.</span><span class="sxs-lookup"><span data-stu-id="63c57-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="63c57-393">Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben.</span><span class="sxs-lookup"><span data-stu-id="63c57-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="63c57-394">In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</span><span class="sxs-lookup"><span data-stu-id="63c57-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="63c57-395">AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</span><span class="sxs-lookup"><span data-stu-id="63c57-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="63c57-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="63c57-397">Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="63c57-398">EXTERN</span><span class="sxs-lookup"><span data-stu-id="63c57-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-399">Projizieren</span><span class="sxs-lookup"><span data-stu-id="63c57-399">Project</span></span></td>
<td><p><span data-ttu-id="63c57-400">Vom Kunden definierter Name für die Dienstinstanz</span><span class="sxs-lookup"><span data-stu-id="63c57-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="63c57-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="63c57-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="63c57-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="63c57-403">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="63c57-404">Wenn Sie z. b. während eines 30-tägigen Monats eine einzeln bereitgestellte Verbindung haben, lesen Dienst Info 1 "1,000000 Connections/30 Days".</span><span class="sxs-lookup"><span data-stu-id="63c57-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="63c57-405">Wenn Sie über ein 25-Service-Paket mit Service Bus-Verbindungen verfügen und während des Tages 1 verwendet haben, würde Ihre tägliche Nutzungs Erklärung für diesen Tag "25 Verbindungen/30 Tage verwendet: 1,000000" lauten.</span><span class="sxs-lookup"><span data-stu-id="63c57-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-406">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="63c57-407">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="63c57-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="63c57-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="63c57-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="63c57-409">DomainName</span></span></td>
<td><p><span data-ttu-id="63c57-410">Name der Domäne des Kunden, der zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="63c57-411">Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="63c57-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="63c57-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="63c57-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-413">Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-413">Unit</span></span></td>
<td><p><span data-ttu-id="63c57-414">Die Einheit des Ressourcennamens</span><span class="sxs-lookup"><span data-stu-id="63c57-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="63c57-415">GB oder STUNDEN</span><span class="sxs-lookup"><span data-stu-id="63c57-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="63c57-416">Einmalige und wiederkehrende Dateifelder</span><span class="sxs-lookup"><span data-stu-id="63c57-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="63c57-417">Column</span><span class="sxs-lookup"><span data-stu-id="63c57-417">Column</span></span></th>
<th><span data-ttu-id="63c57-418">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="63c57-419">PartnerID</span><span class="sxs-lookup"><span data-stu-id="63c57-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="63c57-420">Eindeutiger Bezeichner für Microsoft Azure Active Directory-Mandanten für eine bestimmte Abrechnungsentität im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="63c57-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="63c57-421">Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="63c57-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="63c57-422">In allen Zeilen gleich.</span><span class="sxs-lookup"><span data-stu-id="63c57-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-423">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="63c57-424">Eindeutige Microsoft Azure Active Directory-Mandanten-ID im GUID-Format, die zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-425">Kundenname</span><span class="sxs-lookup"><span data-stu-id="63c57-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="63c57-426">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="63c57-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="63c57-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="63c57-428">Name der Domäne des Kunden, der zur Identifizierung des Kunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="63c57-429">Dieser Name darf nicht verwendet werden, um den Kunden eindeutig zu identifizieren, da der Kunde/Partner die Vanity-/Standarddomäne über das Office 365-Portal aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="63c57-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="63c57-430">Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="63c57-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-431">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="63c57-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="63c57-432">Das Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="63c57-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-433">Rechnungsnummer</span><span class="sxs-lookup"><span data-stu-id="63c57-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="63c57-434">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-435">MPNID</span><span class="sxs-lookup"><span data-stu-id="63c57-435">MpnId</span></span></td>
<td><p><span data-ttu-id="63c57-436">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="63c57-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-437">MPN-ID des Handelspartners</span><span class="sxs-lookup"><span data-stu-id="63c57-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="63c57-438">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="63c57-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-439">Bestellnummer</span><span class="sxs-lookup"><span data-stu-id="63c57-439">Order ID</span></span></td>
<td><p><span data-ttu-id="63c57-440">Eindeutiger Bezeichner für eine Bestellung auf der Microsoft Commerce Platform.</span><span class="sxs-lookup"><span data-stu-id="63c57-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="63c57-441">Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-442">Bestellungsdatum</span><span class="sxs-lookup"><span data-stu-id="63c57-442">Order date</span></span></td>
<td><p><span data-ttu-id="63c57-443">Das Datum, an dem die Bestellung aufgegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="63c57-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-444">ProductID</span><span class="sxs-lookup"><span data-stu-id="63c57-444">ProductId</span></span></td>
<td><p><span data-ttu-id="63c57-445">Die ID des Produkts.</span><span class="sxs-lookup"><span data-stu-id="63c57-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="63c57-446">SkuId</span></span></td>
<td><p><span data-ttu-id="63c57-447">Die ID einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="63c57-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="63c57-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="63c57-449">Die ID einer bestimmten Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="63c57-449">The ID for a particular Availability.</span></span> <span data-ttu-id="63c57-450">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für das jeweilige Land, die Währung, das Branchensegment usw. für den Erwerb verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="63c57-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-451">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="63c57-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="63c57-452">Der Titel einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="63c57-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-453">Produktname</span><span class="sxs-lookup"><span data-stu-id="63c57-453">Product name</span></span></td>
<td><p><span data-ttu-id="63c57-454">Name des Produkts.</span><span class="sxs-lookup"><span data-stu-id="63c57-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="63c57-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="63c57-456">Der Name des Herausgebers des Produkts.</span><span class="sxs-lookup"><span data-stu-id="63c57-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="63c57-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="63c57-458">Eindeutige ID dieses Herausgebers.</span><span class="sxs-lookup"><span data-stu-id="63c57-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-459">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="63c57-460">Anzeigename eines Abonnements.</span><span class="sxs-lookup"><span data-stu-id="63c57-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-461">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="63c57-462">Eindeutiger Bezeichner eines Abonnements auf der Microsoft Commerce Platform.</span><span class="sxs-lookup"><span data-stu-id="63c57-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="63c57-463">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="63c57-464">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="63c57-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="63c57-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="63c57-466">Der erste Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="63c57-466">Start day of the charges.</span></span> <span data-ttu-id="63c57-467">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="63c57-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="63c57-469">Letzter Tag, an dem Gebühren anfallen.</span><span class="sxs-lookup"><span data-stu-id="63c57-469">End day of the charges.</span></span> <span data-ttu-id="63c57-470">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-471">Laufzeit und Abrechnungszyklus</span><span class="sxs-lookup"><span data-stu-id="63c57-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="63c57-472">Die Laufzeitlänge und der Abrechnungszyklus für den Kauf.</span><span class="sxs-lookup"><span data-stu-id="63c57-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="63c57-473">Beispiel: "1 Jahr, monatlich".</span><span class="sxs-lookup"><span data-stu-id="63c57-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-474">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="63c57-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="63c57-475">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="63c57-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-476">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="63c57-477">Der Preis entsprechend der Preisliste zum Kaufzeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="63c57-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="63c57-478">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-479">Effektiver Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="63c57-480">Der Preis pro Einheit, nachdem Anpassungen vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-481">Anzahl</span><span class="sxs-lookup"><span data-stu-id="63c57-481">Quantity</span></span></td>
<td><p><span data-ttu-id="63c57-482">Anzahl der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="63c57-482">Number of units.</span></span> <span data-ttu-id="63c57-483">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-484">Typ der Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-484">Unit type</span></span></td>
<td><p><span data-ttu-id="63c57-485">Der Typ der Einheit, die gekauft wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-486">Preis Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="63c57-487">Eine Erklärung der geltenden Rabatte.</span><span class="sxs-lookup"><span data-stu-id="63c57-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-488">Zwischensumme</span><span class="sxs-lookup"><span data-stu-id="63c57-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="63c57-489">Gesamtbetrag vor Steuern</span><span class="sxs-lookup"><span data-stu-id="63c57-489">Total before tax.</span></span> <span data-ttu-id="63c57-490">Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="63c57-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-491">Steuern gesamt</span><span class="sxs-lookup"><span data-stu-id="63c57-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="63c57-492">USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</span><span class="sxs-lookup"><span data-stu-id="63c57-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-493">Gesamt</span><span class="sxs-lookup"><span data-stu-id="63c57-493">Total</span></span></td>
<td><p><span data-ttu-id="63c57-494">Gesamtsumme nach Steuern.</span><span class="sxs-lookup"><span data-stu-id="63c57-494">Total after tax.</span></span> <span data-ttu-id="63c57-495">Überprüft, ob in der Rechnung Steuern berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-496">Währung</span><span class="sxs-lookup"><span data-stu-id="63c57-496">Currency</span></span></td>
<td><p><span data-ttu-id="63c57-497">Währungstyp</span><span class="sxs-lookup"><span data-stu-id="63c57-497">Currency type.</span></span> <span data-ttu-id="63c57-498">Jede Abrechnungsentität verfügt nur über eine Währung.</span><span class="sxs-lookup"><span data-stu-id="63c57-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="63c57-499">Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="63c57-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="63c57-501">Ein alternativer Bezeichner für eine Bestellungs-ID.</span><span class="sxs-lookup"><span data-stu-id="63c57-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-502">Billingfrequency</span><span class="sxs-lookup"><span data-stu-id="63c57-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="63c57-503">Wird monatlich angezeigt, wenn die monatliche Abrechnung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="63c57-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="63c57-504">Andernfalls leer.</span><span class="sxs-lookup"><span data-stu-id="63c57-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-505">Billablemenge</span><span class="sxs-lookup"><span data-stu-id="63c57-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="63c57-506">Stellt die Gesamtanzahl erworbener oder genutzter Einheiten dar.</span><span class="sxs-lookup"><span data-stu-id="63c57-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-507">Pricingcurrency</span><span class="sxs-lookup"><span data-stu-id="63c57-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="63c57-508">Listet den Preis für die Ressource oder das Angebot auf.</span><span class="sxs-lookup"><span data-stu-id="63c57-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-509">Pctobcexchangerate</span><span class="sxs-lookup"><span data-stu-id="63c57-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="63c57-510">Wechselkurs für Preiswährung (Kunden) Abrechnungswährung</span><span class="sxs-lookup"><span data-stu-id="63c57-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-511">Pctobcexchangeratedate</span><span class="sxs-lookup"><span data-stu-id="63c57-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="63c57-512">Das Datum, an dem die Preiswährung für den Abrechnungs Währungsaustausch festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-513">Meterbeschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="63c57-514">Verbrauchseinheit für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="63c57-515">Dateifelder zur bewerteten täglichen Nutzung</span><span class="sxs-lookup"><span data-stu-id="63c57-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="63c57-516">Column</span><span class="sxs-lookup"><span data-stu-id="63c57-516">Column</span></span></th>
<th><span data-ttu-id="63c57-517">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="63c57-518">PartnerID</span><span class="sxs-lookup"><span data-stu-id="63c57-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="63c57-519">Partner-ID im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="63c57-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="63c57-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="63c57-521">Partnername.</span><span class="sxs-lookup"><span data-stu-id="63c57-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-522">Kunden-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="63c57-523">Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</span><span class="sxs-lookup"><span data-stu-id="63c57-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="63c57-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="63c57-525">Firmenname des Kunden wie im Partner Center angegeben.</span><span class="sxs-lookup"><span data-stu-id="63c57-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="63c57-526">Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</span><span class="sxs-lookup"><span data-stu-id="63c57-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="63c57-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="63c57-528">Der Domänen Name des Kunden.</span><span class="sxs-lookup"><span data-stu-id="63c57-528">The customer's domain name.</span></span> <span data-ttu-id="63c57-529">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="63c57-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-530">Land des Kunden</span><span class="sxs-lookup"><span data-stu-id="63c57-530">Customer country</span></span></td>
<td><p><span data-ttu-id="63c57-531">Das Land, in dem sich der Kunde befindet.</span><span class="sxs-lookup"><span data-stu-id="63c57-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="63c57-532">MPNID</span></span></td>
<td><p><span data-ttu-id="63c57-533">MPN-ID des CSP-Partners.</span><span class="sxs-lookup"><span data-stu-id="63c57-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-534">MPN-ID des Handelspartners</span><span class="sxs-lookup"><span data-stu-id="63c57-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="63c57-535">MPN-ID des registrierten Handelspartners für das Abonnement.</span><span class="sxs-lookup"><span data-stu-id="63c57-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="63c57-536">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="63c57-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="63c57-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="63c57-538">Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="63c57-539">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="63c57-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-540">ProductID</span><span class="sxs-lookup"><span data-stu-id="63c57-540">ProductId</span></span></td>
<td><p><span data-ttu-id="63c57-541">Die ID des Produkts.</span><span class="sxs-lookup"><span data-stu-id="63c57-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="63c57-542">SkuId</span></span></td>
<td><p><span data-ttu-id="63c57-543">Die ID einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="63c57-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="63c57-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="63c57-545">Die ID einer bestimmten Verfügbarkeit.</span><span class="sxs-lookup"><span data-stu-id="63c57-545">The ID for a particular Availability.</span></span> <span data-ttu-id="63c57-546">"Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für das jeweilige Land, die Währung, das Branchensegment usw. für den Erwerb verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="63c57-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-547">SKU-Name</span><span class="sxs-lookup"><span data-stu-id="63c57-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="63c57-548">Der Titel einer bestimmten SKU.</span><span class="sxs-lookup"><span data-stu-id="63c57-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="63c57-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="63c57-550">Der Name des Herausgebers.</span><span class="sxs-lookup"><span data-stu-id="63c57-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="63c57-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="63c57-552">Die ID des Herausgebers im GUID-Format.</span><span class="sxs-lookup"><span data-stu-id="63c57-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="63c57-553">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="63c57-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-554">Abonnementbeschreibung</span><span class="sxs-lookup"><span data-stu-id="63c57-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="63c57-555">Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</span><span class="sxs-lookup"><span data-stu-id="63c57-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="63c57-556">(Dies ist ein identisches Feld für den Angebotsnamen).</span><span class="sxs-lookup"><span data-stu-id="63c57-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-557">Abonnement-ID</span><span class="sxs-lookup"><span data-stu-id="63c57-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="63c57-558">Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform.</span><span class="sxs-lookup"><span data-stu-id="63c57-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="63c57-559">Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</span><span class="sxs-lookup"><span data-stu-id="63c57-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="63c57-560">Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</span><span class="sxs-lookup"><span data-stu-id="63c57-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="63c57-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="63c57-562">Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="63c57-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="63c57-563">Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="63c57-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="63c57-565">Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</span><span class="sxs-lookup"><span data-stu-id="63c57-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="63c57-566">Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</span><span class="sxs-lookup"><span data-stu-id="63c57-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-567">Nutzungsdatum</span><span class="sxs-lookup"><span data-stu-id="63c57-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="63c57-568">Datum der Nutzung des Diensts.</span><span class="sxs-lookup"><span data-stu-id="63c57-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-569">Typ der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="63c57-570">Der Typ der Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="63c57-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-571">Kategorie der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="63c57-572">Der Dienst der obersten Ebene für die Nutzung.</span><span class="sxs-lookup"><span data-stu-id="63c57-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-573">ID der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="63c57-574">Die ID der verwendeten Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="63c57-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-575">Unterkategorie der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="63c57-576">Der Typ des Azure-Diensts, der sich auf die Rate auswirken kann.</span><span class="sxs-lookup"><span data-stu-id="63c57-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-577">Name der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="63c57-578">Die Maßeinheit für die genutzte Verbrauchseinheit.</span><span class="sxs-lookup"><span data-stu-id="63c57-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-579">Region der Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="63c57-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="63c57-580">Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</span><span class="sxs-lookup"><span data-stu-id="63c57-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-581">Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-581">Unit</span></span></td>
<td><p><span data-ttu-id="63c57-582">Die Einheit des Ressourcennamens.</span><span class="sxs-lookup"><span data-stu-id="63c57-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-583">Verbrauchte Menge</span><span class="sxs-lookup"><span data-stu-id="63c57-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="63c57-584">Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</span><span class="sxs-lookup"><span data-stu-id="63c57-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="63c57-585">Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</span><span class="sxs-lookup"><span data-stu-id="63c57-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-586">Ressourcenspeicherort</span><span class="sxs-lookup"><span data-stu-id="63c57-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="63c57-587">Das Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-588">Genutzter Dienst</span><span class="sxs-lookup"><span data-stu-id="63c57-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="63c57-589">Der Azure-Plattformdienst, den Sie verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="63c57-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="63c57-590">Ressourcen-URI</span><span class="sxs-lookup"><span data-stu-id="63c57-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="63c57-591">Der URI der verwendeten Ressource.</span><span class="sxs-lookup"><span data-stu-id="63c57-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-592">Gebührenart</span><span class="sxs-lookup"><span data-stu-id="63c57-592">Charge type</span></span></td>
<td><p><span data-ttu-id="63c57-593">Art der Gebühren oder der Anpassung.</span><span class="sxs-lookup"><span data-stu-id="63c57-593">The type of charge or adjustment.</span></span> <span data-ttu-id="63c57-594">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="63c57-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-595">Preis pro Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-595">Unit price</span></span></td>
<td><p><span data-ttu-id="63c57-596">Preis pro Lizenz entsprechend der Preisliste zum Kaufzeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="63c57-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="63c57-597">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-598">Anzahl</span><span class="sxs-lookup"><span data-stu-id="63c57-598">Quantity</span></span></td>
<td><p><span data-ttu-id="63c57-599">Anzahl der Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="63c57-599">Number of licenses.</span></span> <span data-ttu-id="63c57-600">Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-601">Typ der Einheit</span><span class="sxs-lookup"><span data-stu-id="63c57-601">Unit type</span></span></td>
<td><p><span data-ttu-id="63c57-602">Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="63c57-603">Für die aktuelle Aktivität nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="63c57-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-604">Abrechnung vor Steuern</span><span class="sxs-lookup"><span data-stu-id="63c57-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="63c57-605">Gesamtbetrag vor Steuern.</span><span class="sxs-lookup"><span data-stu-id="63c57-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-606">Abrechnungswährung</span><span class="sxs-lookup"><span data-stu-id="63c57-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="63c57-607">Die Währung in der geografischen Region des Kunden</span><span class="sxs-lookup"><span data-stu-id="63c57-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-608">Preise vor Steuern gesamt</span><span class="sxs-lookup"><span data-stu-id="63c57-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="63c57-609">Die Preise vor Hinzufügen von Steuern.</span><span class="sxs-lookup"><span data-stu-id="63c57-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-610">Währung der Preise</span><span class="sxs-lookup"><span data-stu-id="63c57-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="63c57-611">Die Währung in der Preisliste.</span><span class="sxs-lookup"><span data-stu-id="63c57-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-612">Dienstinformationen 1</span><span class="sxs-lookup"><span data-stu-id="63c57-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="63c57-613">Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</span><span class="sxs-lookup"><span data-stu-id="63c57-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="63c57-614">Dienstinformationen 2</span><span class="sxs-lookup"><span data-stu-id="63c57-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="63c57-615">Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="63c57-616">Zusätzliche Infos</span><span class="sxs-lookup"><span data-stu-id="63c57-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="63c57-617">Zusätzliche Informationen, die von anderen Spalten nicht abgedeckt werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-618">Effectiveunitprice</span><span class="sxs-lookup"><span data-stu-id="63c57-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="63c57-619">Tatsächlicher Wert pro Einheit (Dies umfasst Rabatte, Gutschriften usw.).</span><span class="sxs-lookup"><span data-stu-id="63c57-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-620">Pctobcexchangerate</span><span class="sxs-lookup"><span data-stu-id="63c57-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="63c57-621">Wechselkurs für Preiswährung (Kunden), Abrechnungswährung.</span><span class="sxs-lookup"><span data-stu-id="63c57-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-622">Pctobcexchangeratedate</span><span class="sxs-lookup"><span data-stu-id="63c57-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="63c57-623">Das Datum, an dem die Preiswährung für den Abrechnungs Währungsaustausch festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="63c57-624">Berelementid</span><span class="sxs-lookup"><span data-stu-id="63c57-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="63c57-625">Stellt Azure-Abonnement-ID dar.</span><span class="sxs-lookup"><span data-stu-id="63c57-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="63c57-626">Berelementdescription</span><span class="sxs-lookup"><span data-stu-id="63c57-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="63c57-627">Steht für den Namen des Azure-Abonnements.</span><span class="sxs-lookup"><span data-stu-id="63c57-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="63c57-628">Zuordnung von Gebühren zwischen einer Rechnung und der Kontenabstimmungsdatei</span><span class="sxs-lookup"><span data-stu-id="63c57-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="63c57-629">Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Kontenabstimmungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.</span><span class="sxs-lookup"><span data-stu-id="63c57-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="63c57-630">Zum Erstellen von Querverweisen der Gebührenbeträge zwischen Rechnung und Kontenabstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie die Kontenabstimmungsdatei nach Gebührentypen filtern, um die Abrechnungsgebühren einer Reihe von Gebührenaufschlüsselungen in der Kontenabstimmungsdatei zuzuordnen.</span><span class="sxs-lookup"><span data-stu-id="63c57-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="63c57-631">Sowohl nutzungsbasierte als auch lizenzbasierte Kontenabstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zugehörige Kosten).</span><span class="sxs-lookup"><span data-stu-id="63c57-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="63c57-632">Ein Guthaben, Rabatte oder Rückerstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungs Datei angezeigt.</span><span class="sxs-lookup"><span data-stu-id="63c57-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="63c57-633">Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnitt und zugehörigen Gebührentypen, die möglicherweise in den Kontenabstimmungsdateien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="63c57-634"><strong>Beschreibung der Rechnungsgebühr</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-635"><strong>Gebührenbeschreibung der Abstimmungsdatei (Spalte „ChargeType“)</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-636"><strong>Was ist diese Gebühr?</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-637"><strong>Wie ordne ich diese Gebührentypen der Rechnung zu?</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="63c57-638"><strong>Lizenzbasierte Gebühren</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-639">Aktivierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="63c57-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-640">Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</span><span class="sxs-lookup"><span data-stu-id="63c57-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="63c57-641">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-642">Stornierungsgebühr</span><span class="sxs-lookup"><span data-stu-id="63c57-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-643">Anteilige Gebühren werden dem Kunden zurückerstattet, wenn verknüpfte Arbeitsplätze geändert werden.</span><span class="sxs-lookup"><span data-stu-id="63c57-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-644">Gebühr für Zyklus</span><span class="sxs-lookup"><span data-stu-id="63c57-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-645">Regelmäßige Gebühren für ein Abonnement</span><span class="sxs-lookup"><span data-stu-id="63c57-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-646">Anteiliger Zyklus für Instanz</span><span class="sxs-lookup"><span data-stu-id="63c57-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-647">Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Arbeitsplätze geändert werden</span><span class="sxs-lookup"><span data-stu-id="63c57-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-648">Gebühren bei Stornierung anteilig zuordnen</span><span class="sxs-lookup"><span data-stu-id="63c57-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-649">Anteilige Rückerstattung für nicht verwendete Teile des Diensts bei einer Stornierung</span><span class="sxs-lookup"><span data-stu-id="63c57-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-650">Anteilige Gebühren beim Kauf</span><span class="sxs-lookup"><span data-stu-id="63c57-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-651">Der Typ der Gebühr für ein Abonnement bei Verwendung der jährlichen Abrechnung</span><span class="sxs-lookup"><span data-stu-id="63c57-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-652">Kaufgebühr</span><span class="sxs-lookup"><span data-stu-id="63c57-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-653">Der Typ der Gebühr für ein Abonnement bei Verwendung der monatlichen Abrechnung</span><span class="sxs-lookup"><span data-stu-id="63c57-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-654">Anteilige Gebühr bei Verlängerung</span><span class="sxs-lookup"><span data-stu-id="63c57-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-655">Anteilige Gebühren nach Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="63c57-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="63c57-656">Verlängerungsgebühr</span><span class="sxs-lookup"><span data-stu-id="63c57-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-657">Gebühr für Verlängerung eines Abonnements</span><span class="sxs-lookup"><span data-stu-id="63c57-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-658">Anteilige Gebühren beim Aktivieren</span><span class="sxs-lookup"><span data-stu-id="63c57-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-659">Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</span><span class="sxs-lookup"><span data-stu-id="63c57-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="63c57-660"><strong>Einmalige Gebühren</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="63c57-661">Neu</span><span class="sxs-lookup"><span data-stu-id="63c57-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-662">Wird verwendet, wenn ein neuer Kauf erstellt wird</span><span class="sxs-lookup"><span data-stu-id="63c57-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="63c57-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-664">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach der Erhöhung verwendet.</span><span class="sxs-lookup"><span data-stu-id="63c57-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="63c57-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-666">Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach der Abnahme verwendet.</span><span class="sxs-lookup"><span data-stu-id="63c57-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-667">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="63c57-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-668">Wird verwendet, wenn ein Abonnement abgebrochen wird.</span><span class="sxs-lookup"><span data-stu-id="63c57-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-669">Konvertieren</span><span class="sxs-lookup"><span data-stu-id="63c57-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-670">Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Arbeitsplätze jedoch unverändert bleibt.</span><span class="sxs-lookup"><span data-stu-id="63c57-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="63c57-671"><strong>Nutzungsgebühren</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-672">Nutzungsgebühr beim Stornieren bewerten</span><span class="sxs-lookup"><span data-stu-id="63c57-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-673">Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei Kündigung</span><span class="sxs-lookup"><span data-stu-id="63c57-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="63c57-674">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-675">Nutzungsgebühr für den aktuellen Zyklus bewerten</span><span class="sxs-lookup"><span data-stu-id="63c57-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-676">Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</span><span class="sxs-lookup"><span data-stu-id="63c57-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="63c57-677"><strong>Guthaben</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-678">Ausgleichen einer Position</span><span class="sxs-lookup"><span data-stu-id="63c57-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-679">Teilweise oder vollständige Rückerstattung für eine Position, einschließlich Steuern</span><span class="sxs-lookup"><span data-stu-id="63c57-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-680">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="63c57-681">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="63c57-682"><strong>Nutzungsbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-683">Aktivierungsrabatt</span><span class="sxs-lookup"><span data-stu-id="63c57-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-684">Rabatt bei Aktivierung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="63c57-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="63c57-685">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-686">Zyklusrabatt</span><span class="sxs-lookup"><span data-stu-id="63c57-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-687">Rabatt auf regelmäßige Gebühren</span><span class="sxs-lookup"><span data-stu-id="63c57-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-688">Verlängerungsrabatt</span><span class="sxs-lookup"><span data-stu-id="63c57-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-689">Rabatt bei Verlängerung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="63c57-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-690">Stornorabatt</span><span class="sxs-lookup"><span data-stu-id="63c57-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-691">Anfallende Gebühren, wenn Rabatte storniert werden</span><span class="sxs-lookup"><span data-stu-id="63c57-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="63c57-692"><strong>Lizenzbasierte Rabatte</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-693"><em>Können auf mehrere Gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="63c57-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="63c57-694">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="63c57-695"><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></span><span class="sxs-lookup"><span data-stu-id="63c57-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-696"><em>Können auf mehrere Gebührentypen angewendet werden</em></span><span class="sxs-lookup"><span data-stu-id="63c57-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="63c57-697"><em>Ausnahme: &quot;Offset ein Zeilen Element &quot; bereits Steuern enthält. Siehe Guthaben weiter oben.</em></span><span class="sxs-lookup"><span data-stu-id="63c57-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-698">Steuern oder Umsatzsteuern (MwSt.)</span><span class="sxs-lookup"><span data-stu-id="63c57-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="63c57-699">Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="63c57-700">Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="63c57-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
