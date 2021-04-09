---
title: Ankündigungen für März 2021
description: Ankündigungen für März 2021 zum Microsoft Partner Center, einschließlich neuer Funktionen, Promotions, Angebote, Märkte oder Änderungen an bestehenden Angeboten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374386"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="10d1e-103">Ankündigungen für März 2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-103">March 2021 announcements</span></span>

<span data-ttu-id="10d1e-104">Auf dieser Seite finden Sie die Ankündigungen vom März 2021 für Microsoft Partner Center.</span><span class="sxs-lookup"><span data-stu-id="10d1e-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="10d1e-105">Aktualisierte API zur Überprüfung von Kundenadressen im CSP-Programm jetzt zum Testen verfügbar</span><span class="sxs-lookup"><span data-stu-id="10d1e-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-106">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-106">Categories</span></span>

- <span data-ttu-id="10d1e-107">Datum: 31.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="10d1e-108">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-109">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-109">Summary</span></span>

<span data-ttu-id="10d1e-110">Im Rahmen unserer Verpflichtung, Partner und Kunden bei der Ausführung ihrer Geschäfte auf Vertrauensbasis zu unterstützen, laden wir Partner weltweit ein, die Änderungen an der ValidateAddress-API zu testen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-111">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-111">Impacted audience</span></span>

<span data-ttu-id="10d1e-112">Alle CSP-Partner mit direkter Abrechnung und indirekte Anbieter, die neue Adressdetails für Kunden erstellen oder bestehende Details aktualisieren</span><span class="sxs-lookup"><span data-stu-id="10d1e-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-113">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-113">Details</span></span>

<span data-ttu-id="10d1e-114">Microsoft setzt auf Vertrauen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-114">Microsoft runs on trust.</span></span> <span data-ttu-id="10d1e-115">Wir haben uns verpflichtet, eine kompatible und sichere Methode der Überprüfung von Kundenadressen zur Abwicklung von Kundenabonnements im CSP-Programm bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="10d1e-116">Heute, am 31. März 2021, haben wir Änderungen an der ValidateAddress-API eingeführt, die wir gerne von Ihnen testen lassen möchten, bevor die Änderungen im Juni 2021 umgesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="10d1e-117">Beachten Sie, dass diese Änderungen nur die ValidateAddress-API betreffen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="10d1e-118">Die CreateCustomer-API and UpdateBillingProfile-API sind nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="10d1e-119">Die Antwort gibt eine der folgenden Statusmeldungen zurück:</span><span class="sxs-lookup"><span data-stu-id="10d1e-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="10d1e-120">Status</span><span class="sxs-lookup"><span data-stu-id="10d1e-120">Status</span></span> | <span data-ttu-id="10d1e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10d1e-121">Description</span></span> | <span data-ttu-id="10d1e-122">Anzahl der zurückgegebenen vorgeschlagenen Adressen</span><span class="sxs-lookup"><span data-stu-id="10d1e-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="10d1e-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="10d1e-123">VerifiedShippable</span></span> | <span data-ttu-id="10d1e-124">Die Adresse ist überprüft und für den Versand geeignet.</span><span class="sxs-lookup"><span data-stu-id="10d1e-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="10d1e-125">Eine</span><span class="sxs-lookup"><span data-stu-id="10d1e-125">Single</span></span> |
| <span data-ttu-id="10d1e-126">Verified</span><span class="sxs-lookup"><span data-stu-id="10d1e-126">Verified</span></span> | <span data-ttu-id="10d1e-127">Die Adresse ist überprüft.</span><span class="sxs-lookup"><span data-stu-id="10d1e-127">Address is verified.</span></span> | <span data-ttu-id="10d1e-128">Eine</span><span class="sxs-lookup"><span data-stu-id="10d1e-128">Single</span></span> |
| <span data-ttu-id="10d1e-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="10d1e-129">InteractionRequired</span></span> | <span data-ttu-id="10d1e-130">Die vorgeschlagene Adresse wurde erheblich geändert und muss vom Benutzer bestätigt werden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="10d1e-131">Eine</span><span class="sxs-lookup"><span data-stu-id="10d1e-131">Single</span></span> |
| <span data-ttu-id="10d1e-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="10d1e-132">StreetPartial</span></span> | <span data-ttu-id="10d1e-133">Die angegebene Straße in der Adresse ist unvollständig und erfordert weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="10d1e-134">Mehrere – maximal drei</span><span class="sxs-lookup"><span data-stu-id="10d1e-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="10d1e-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="10d1e-135">PremisesPartial</span></span> | <span data-ttu-id="10d1e-136">Die angegebenen Räumlichkeiten (Gebäudenummer, Suitenummer usw.) sind unvollständig und erfordern weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="10d1e-137">Mehrere – maximal drei</span><span class="sxs-lookup"><span data-stu-id="10d1e-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="10d1e-138">Multiple</span><span class="sxs-lookup"><span data-stu-id="10d1e-138">Multiple</span></span> | <span data-ttu-id="10d1e-139">Mehrere Felder in der Adresse sind unvollständig (möglicherweise StreetPartial and PremisesPartial eingeschlossen).</span><span class="sxs-lookup"><span data-stu-id="10d1e-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="10d1e-140">Mehrere – maximal drei</span><span class="sxs-lookup"><span data-stu-id="10d1e-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="10d1e-141">None</span><span class="sxs-lookup"><span data-stu-id="10d1e-141">None</span></span> | <span data-ttu-id="10d1e-142">Die Adresse ist falsch.</span><span class="sxs-lookup"><span data-stu-id="10d1e-142">Address is incorrect.</span></span> | <span data-ttu-id="10d1e-143">Keine</span><span class="sxs-lookup"><span data-stu-id="10d1e-143">None</span></span> |
| <span data-ttu-id="10d1e-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="10d1e-144">NotValidated</span></span> | <span data-ttu-id="10d1e-145">Die Adresse konnte den Überprüfungsprozess nicht durchlaufen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="10d1e-146">Keine</span><span class="sxs-lookup"><span data-stu-id="10d1e-146">None</span></span> |

<span data-ttu-id="10d1e-147">Nachdem eine Adresse über die ValidateAddress-API übermittelt wurde, wird das folgende Antwortschema zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="10d1e-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="10d1e-148">Sehen Sie sich die folgende Beispielantwort an.</span><span class="sxs-lookup"><span data-stu-id="10d1e-148">Take a look at this sample response.</span></span> <span data-ttu-id="10d1e-149">Beachten Sie, dass die Antwort für die USA ein zusätzliches vierstelliges Suffix für die Postleitzahl zurückgibt, wenn Sie nur fünf Ziffern für die Postleitzahl eingeben.</span><span class="sxs-lookup"><span data-stu-id="10d1e-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="10d1e-150">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-150">Next steps</span></span>

- <span data-ttu-id="10d1e-151">Teilen Sie unserem Fachexperten (SME), Ali Khaki, Ihre Sandbox-Mandanten-ID mit, damit Sie in die Testphase einbezogen werden und mit der Vorbereitung für die Aktualisierung beginnen können.</span><span class="sxs-lookup"><span data-stu-id="10d1e-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="10d1e-152">Wenden Sie sich an Ihren CPV (Control Panel Vendor), wenn Sie eine CPV-Lösung verwenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-153">Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-153">Questions?</span></span>

<span data-ttu-id="10d1e-154">Wenn Sie Fragen haben oder Unterstützung hinsichtlich des Geschäftsbetriebs mit Microsoft benötigen, wenden Sie sich an Ihre Yammer-Gruppe beim Partner-Support.</span><span class="sxs-lookup"><span data-stu-id="10d1e-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="10d1e-155">Neue Benutzeroberfläche des Exchange Admin Center (EAC)</span><span class="sxs-lookup"><span data-stu-id="10d1e-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-156">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-156">Categories</span></span>

- <span data-ttu-id="10d1e-157">Datum: 29.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="10d1e-158">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-159">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-159">Summary</span></span>

<span data-ttu-id="10d1e-160">Ab dem 27. April 2021 führt das Exchange Admin Center (EAC) eine neue Benutzeroberfläche ein, mit der die tägliche Effizienz für Benutzer verbessert wird.</span><span class="sxs-lookup"><span data-stu-id="10d1e-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-161">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-161">Impacted audience</span></span>

<span data-ttu-id="10d1e-162">Delegierte Administratoren, die über Partner Center auf Exchange zugreifen</span><span class="sxs-lookup"><span data-stu-id="10d1e-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-163">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-163">Details</span></span>

<span data-ttu-id="10d1e-164">Ab dem 27. April 2021 werden Partner, die über Partner Center zu Exchange navigieren, zum neuen EAC umgeleitet.</span><span class="sxs-lookup"><span data-stu-id="10d1e-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="10d1e-165">Diese neue Oberfläche ist derzeit als Vorschau verfügbar, und Administratoren können sie aktivieren, indem sie im klassischen EAC die Umschaltfläche in der oberen rechten Ecke auswählen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="10d1e-166">Administratoren können auch zum neuen EAC navigieren, indem sie auf das Banner „Jetzt ausprobieren“ klicken, das auf allen Seiten angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="10d1e-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="10d1e-167">Das neue EAC bietet unter anderem folgende Vorteile:</span><span class="sxs-lookup"><span data-stu-id="10d1e-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="10d1e-168">Zusätzliche Einblicke, Berichte und Warnmechanismen für Probleme im Zusammenhang mit dem Nachrichtenfluss</span><span class="sxs-lookup"><span data-stu-id="10d1e-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="10d1e-169">Personalisierte Dashboards zur Steigerung der Produktivität</span><span class="sxs-lookup"><span data-stu-id="10d1e-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="10d1e-170">Als Hilfe beim Navigieren durch die neue Benutzeroberfläche stehen Videos im Abschnitt **Schulung und Leitfaden** auf der neuen EAC-Oberfläche bereit.</span><span class="sxs-lookup"><span data-stu-id="10d1e-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="10d1e-171">Diese vermitteln Ihnen einen Überblick darüber, wie Sie das neue Portal optimal verwenden können.</span><span class="sxs-lookup"><span data-stu-id="10d1e-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="10d1e-172">Durch diese Änderung ist die klassische EAC-Oberfläche nicht veraltet.</span><span class="sxs-lookup"><span data-stu-id="10d1e-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="10d1e-173">Sie werden rechtzeitig benachrichtigt, bevor eine Änderung implementiert wird.</span><span class="sxs-lookup"><span data-stu-id="10d1e-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-174">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-174">Next steps</span></span>

- <span data-ttu-id="10d1e-175">Sehen Sie sich die [Ressourcen zu diesem Thema](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/) an, die Screenshots der neuen Benutzeroberfläche enthalten.</span><span class="sxs-lookup"><span data-stu-id="10d1e-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="10d1e-176">Leiten Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrem Unternehmen weiter.</span><span class="sxs-lookup"><span data-stu-id="10d1e-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="10d1e-177">Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-177">Questions?</span></span>

<span data-ttu-id="10d1e-178">Bei Fragen zu diesen Änderungen können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="10d1e-179">Microsoft Operations: Neuer Produkteinführungskalender</span><span class="sxs-lookup"><span data-stu-id="10d1e-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-180">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-180">Categories</span></span>

- <span data-ttu-id="10d1e-181">Datum: 25.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="10d1e-182">Angebote | Moderner Arbeitsplatz</span><span class="sxs-lookup"><span data-stu-id="10d1e-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-183">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-183">Summary</span></span>

<span data-ttu-id="10d1e-184">Als Reaktion auf das Feedback von Partnern optimiert Microsoft Operations seine Vorgehensweise für Mitteilungen über Produkteinführungen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-185">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-185">Impacted audience</span></span>

<span data-ttu-id="10d1e-186">CSP-Partner (Cloud Solution Provider)</span><span class="sxs-lookup"><span data-stu-id="10d1e-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-187">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-187">Details</span></span>

<span data-ttu-id="10d1e-188">Microsoft ist bestrebt, die Erfahrungen für seine Partner kontinuierlich zu verbessern.</span><span class="sxs-lookup"><span data-stu-id="10d1e-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="10d1e-189">Wir haben Feedback von Ihnen erhalten, dass Ihnen zu viele Mitteilungen von Microsoft zugestellt werden, einschließlich doppelter Ankündigungen von Produkteinführungen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="10d1e-190">Als Reaktion auf Ihr Feedback hat Microsoft die Readiness-Oberfläche für Produkteinführungen für neue und vorhandene Angebote optimiert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="10d1e-191">Wir stellen Ihnen jetzt eine einzige monatliche Ansicht der Produkteinführungen bereit, die im Operations Readiness-Ressourcenkatalog veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="10d1e-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="10d1e-192">Dieser monatliche [Produkteinführungskalender](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) ersetzt einzelne Mitteilungen über Produkteinführungen im Operations Readiness-Ressourcenkatalog und in Partner Center-Ankündigungen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="10d1e-193">Sie können auf diesen [Produkteinführungskalender](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) auch über [Communitysammlungen](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [Kalenderansichten](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) und [CSP-Newsletter](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) zugreifen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="10d1e-194">Wir benachrichtigen Sie, wenn wir den Produkteinführungskalender für einen Monat veröffentlichen, mit einer Ankündigung im Operations Readiness-Ressourcenkatalog.</span><span class="sxs-lookup"><span data-stu-id="10d1e-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="10d1e-195">Informationen zu neuen und vorhandenen Angeboten stehen Ihnen weiterhin in der Preislistenvorschau und den Preislisten-Änderungsprotokollen sowie in Produktblogs, Lizenzierungsleitfäden und auf den Seiten des Produktmarketing zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="10d1e-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="10d1e-196">Die Änderung betrifft Einführungen für die folgenden Produkte:</span><span class="sxs-lookup"><span data-stu-id="10d1e-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="10d1e-197">Lokales Dynamics</span><span class="sxs-lookup"><span data-stu-id="10d1e-197">Dynamics on-premises</span></span>
- <span data-ttu-id="10d1e-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="10d1e-198">Microsoft 365</span></span>
- <span data-ttu-id="10d1e-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="10d1e-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="10d1e-200">Windows</span><span class="sxs-lookup"><span data-stu-id="10d1e-200">Windows</span></span>
- <span data-ttu-id="10d1e-201">Server</span><span class="sxs-lookup"><span data-stu-id="10d1e-201">Server</span></span>  
- <span data-ttu-id="10d1e-202">Tools</span><span class="sxs-lookup"><span data-stu-id="10d1e-202">Tools</span></span>
- <span data-ttu-id="10d1e-203">Teams und Telco</span><span class="sxs-lookup"><span data-stu-id="10d1e-203">Teams and Telco</span></span>

<span data-ttu-id="10d1e-204">Wir senden weiterhin spezifische Ankündigungen für Produkteinführungen, für die Operations Readiness-Details erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="10d1e-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-205">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-205">Next steps</span></span>

<span data-ttu-id="10d1e-206">Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.</span><span class="sxs-lookup"><span data-stu-id="10d1e-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-207">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-207">Questions?</span></span>

<span data-ttu-id="10d1e-208">Bei weiteren Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="10d1e-209">Änderungen der Anforderungen für das Onboarding von Kunden im CSP-Programm</span><span class="sxs-lookup"><span data-stu-id="10d1e-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-210">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-210">Categories</span></span>

- <span data-ttu-id="10d1e-211">Datum: 25.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="10d1e-212">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-213">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-213">Summary</span></span>

<span data-ttu-id="10d1e-214">Im Rahmen unserer Verpflichtung, Partner und Kunden bei der Ausführung ihrer Geschäfte auf Vertrauensbasis zu unterstützen, werden wir ab dem 25. März 2021 zusätzliche Kundeninformationen anfordern.</span><span class="sxs-lookup"><span data-stu-id="10d1e-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-215">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-215">Impacted audience</span></span>

<span data-ttu-id="10d1e-216">CSP-Partner (Cloud Solution Provider) mit direkter Abrechnung und indirekte Anbieter mit neuen Kunden oder Bestandskunden in den im nächsten Abschnitt aufgeführten Ländern</span><span class="sxs-lookup"><span data-stu-id="10d1e-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-217">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-217">Details</span></span>

<span data-ttu-id="10d1e-218">Microsoft setzt auf Vertrauen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-218">Microsoft runs on trust.</span></span> <span data-ttu-id="10d1e-219">Wir haben uns verpflichtet, eine kompatible und sichere Methode der Kundenüberprüfung zur Abwicklung von Kundenabonnements im CSP-Programm bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="10d1e-220">Am 25. März 2021 werden wir Verbesserungen der Partner Center-API und -Benutzeroberfläche (UI) einführen, die sich auf Partner auswirken, die die beiden folgenden Kriterien erfüllen:</span><span class="sxs-lookup"><span data-stu-id="10d1e-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="10d1e-221">Der Partner hat eine direkte Abrechnungsbeziehung mit Microsoft (das heißt, er ist ein Partner mit direkter Abrechnung oder ein indirekter Anbieter).</span><span class="sxs-lookup"><span data-stu-id="10d1e-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="10d1e-222">Der Partner tätigt Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern:</span><span class="sxs-lookup"><span data-stu-id="10d1e-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="10d1e-223">Thailand</span><span class="sxs-lookup"><span data-stu-id="10d1e-223">Thailand</span></span>
    - <span data-ttu-id="10d1e-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="10d1e-224">Vietnam</span></span>
    - <span data-ttu-id="10d1e-225">Türkei</span><span class="sxs-lookup"><span data-stu-id="10d1e-225">Turkey</span></span>
    - <span data-ttu-id="10d1e-226">Polen</span><span class="sxs-lookup"><span data-stu-id="10d1e-226">Poland</span></span>
    - <span data-ttu-id="10d1e-227">Südafrika</span><span class="sxs-lookup"><span data-stu-id="10d1e-227">South Africa</span></span>
    - <span data-ttu-id="10d1e-228">Indien</span><span class="sxs-lookup"><span data-stu-id="10d1e-228">India</span></span>
    - <span data-ttu-id="10d1e-229">Brasilien</span><span class="sxs-lookup"><span data-stu-id="10d1e-229">Brazil</span></span>
    - <span data-ttu-id="10d1e-230">Irak</span><span class="sxs-lookup"><span data-stu-id="10d1e-230">Iraq</span></span>
    - <span data-ttu-id="10d1e-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="10d1e-231">Myanmar</span></span>
    - <span data-ttu-id="10d1e-232">Südsudan</span><span class="sxs-lookup"><span data-stu-id="10d1e-232">South Sudan</span></span>
    - <span data-ttu-id="10d1e-233">Saudi-Arabien</span><span class="sxs-lookup"><span data-stu-id="10d1e-233">Saudi Arabia</span></span>
    - <span data-ttu-id="10d1e-234">Vereinigte Arabische Emirate</span><span class="sxs-lookup"><span data-stu-id="10d1e-234">United Arab Emirates</span></span>
    - <span data-ttu-id="10d1e-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="10d1e-235">Venezuela</span></span>

<span data-ttu-id="10d1e-236">Partner, die diese Kriterien erfüllen, müssen beim Onboarding neuer Kunden oder beim Ändern von Bestandskundendetails die **Firmenregistrierungs-ID** des Kunden (auch als **Organisations-INN** des Kunden bezeichnet) und dessen **Telefonnummer** übermitteln.</span><span class="sxs-lookup"><span data-stu-id="10d1e-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="10d1e-237">Diese Partner können auch einen optionalen **zweiten Vornamen** für den Kunden eingeben.</span><span class="sxs-lookup"><span data-stu-id="10d1e-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="10d1e-238">Beachten Sie, dass Sie beim Hinzufügen Ihrer Firmenregistrierungs-ID Ihre Unternehmenssteuer-ID und nicht die persönliche ID des Kunden verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="10d1e-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="10d1e-239">Für Partner, die Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern tätigen, erfolgte bereits ein Onboarding mit einer früheren Version im November 2020.</span><span class="sxs-lookup"><span data-stu-id="10d1e-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="10d1e-240">Armenien</span><span class="sxs-lookup"><span data-stu-id="10d1e-240">Armenia</span></span>
- <span data-ttu-id="10d1e-241">Aserbaidschan</span><span class="sxs-lookup"><span data-stu-id="10d1e-241">Azerbaijan</span></span>
- <span data-ttu-id="10d1e-242">Belarus</span><span class="sxs-lookup"><span data-stu-id="10d1e-242">Belarus</span></span>
- <span data-ttu-id="10d1e-243">Ungarn</span><span class="sxs-lookup"><span data-stu-id="10d1e-243">Hungary</span></span>
- <span data-ttu-id="10d1e-244">Kasachstan</span><span class="sxs-lookup"><span data-stu-id="10d1e-244">Kazakhstan</span></span>
- <span data-ttu-id="10d1e-245">Kirgisistan</span><span class="sxs-lookup"><span data-stu-id="10d1e-245">Kyrgyzstan</span></span>
- <span data-ttu-id="10d1e-246">Moldawien</span><span class="sxs-lookup"><span data-stu-id="10d1e-246">Moldova</span></span>
- <span data-ttu-id="10d1e-247">Russland</span><span class="sxs-lookup"><span data-stu-id="10d1e-247">Russia</span></span>
- <span data-ttu-id="10d1e-248">Tadschikistan</span><span class="sxs-lookup"><span data-stu-id="10d1e-248">Tajikistan</span></span>
- <span data-ttu-id="10d1e-249">Ukraine</span><span class="sxs-lookup"><span data-stu-id="10d1e-249">Ukraine</span></span>
- <span data-ttu-id="10d1e-250">Usbekistan</span><span class="sxs-lookup"><span data-stu-id="10d1e-250">Uzbekistan</span></span>

<span data-ttu-id="10d1e-251">Partner mit Kunden in anderen Ländern weltweit haben am 25. März 2021 die Möglichkeit, die **Firmenregistrierungs-ID**, die **Telefonnummer** und den **zweiten Vornamen** für Kunden als optionale Details einzugeben.</span><span class="sxs-lookup"><span data-stu-id="10d1e-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-252">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-252">Next steps</span></span>

- <span data-ttu-id="10d1e-253">Ausführlichere Anleitungen finden Sie in der technischen Dokumentation und unter den häufig gestellten Fragen in der [jeweiligen Sammlung für Partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).</span><span class="sxs-lookup"><span data-stu-id="10d1e-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="10d1e-254">Bereiten Sie die Einbindung der Änderungen mithilfe der Partner Center-API und der Webbenutzeroberfläche vor.</span><span class="sxs-lookup"><span data-stu-id="10d1e-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="10d1e-255">API/SDKs werden zu Testzwecken bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="10d1e-256">Stellen Sie sicher, dass Sie beim Onboarding neuer Kunden oder beim Ändern von Bestandskundendetails die zusätzlichen Daten übermitteln.</span><span class="sxs-lookup"><span data-stu-id="10d1e-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="10d1e-257">Wenden Sie sich an Ihren CPV (Control Panel Vendor), wenn Sie eine CPV-Lösung verwenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-258">Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-258">Questions?</span></span>

<span data-ttu-id="10d1e-259">Wenn Sie Fragen im Bezug auf die rechtliche Identifizierung (auch INN oder TIN genannt) haben, wenden Sie sich an Ihren Steuerberater oder das örtliche Finanzamt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="10d1e-260">Microsoft kann in Steuerfragen keine Hilfestellung bieten.</span><span class="sxs-lookup"><span data-stu-id="10d1e-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="10d1e-261">Wenn Sie Unterstützung hinsichtlich des Geschäftsbetriebs mit Microsoft benötigen, [erstellen Sie eine Serviceanfrage](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="10d1e-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="10d1e-262">Korrekturen an der Preisliste für unbefristete Software vom 1. März 2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-263">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-263">Categories</span></span>

- <span data-ttu-id="10d1e-264">Datum: 23.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="10d1e-265">Angebote/Märkte</span><span class="sxs-lookup"><span data-stu-id="10d1e-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-266">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-266">Impacted audience</span></span>

<span data-ttu-id="10d1e-267">Indirekte Anbieter und Partner mit direkter Abrechnung, die Transaktionen für unbefristete Software im Cloud Solution Provider-Programm durchführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="10d1e-268">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-268">Details</span></span>

<span data-ttu-id="10d1e-269">Die Preisliste für unbefristete Software, die am 1. März 2021 veröffentlicht wurde, umfasste Märkte, die nicht hätten enthalten sein dürfen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="10d1e-270">Die Preisliste für unbefristete Software wurde am 17. März 2021 mit Korrekturen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="10d1e-271">Diese Korrekturen betrafen ausschließlich Folgendes:</span><span class="sxs-lookup"><span data-stu-id="10d1e-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="10d1e-272">Produkt-ID: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="10d1e-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="10d1e-273">Produktname: Upgrade von Windows 10 Home auf Pro für Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="10d1e-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="10d1e-274">Entfernte oder nicht unterstützte Märkte: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="10d1e-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="10d1e-275">Diese Änderungen gelten nur für das oben genannte Produkt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-275">These changes only apply to the above product.</span></span> <span data-ttu-id="10d1e-276">Für andere Produkte wurden keine Korrekturen vorgenommen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="10d1e-277">Nächste Schritte und zusätzliche Ressourcen</span><span class="sxs-lookup"><span data-stu-id="10d1e-277">Next steps and resources</span></span>

- <span data-ttu-id="10d1e-278">Partner, die Transaktionen für unbefristete Software durchführen, sollten die neueste Preisliste für unbefristete Software herunterladen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="10d1e-279">Eine übersichtliche Zuordnung der Abkürzungen mit zwei Buchstaben zu Ländern finden Sie unter den [Länder- und Regionscodes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries).</span><span class="sxs-lookup"><span data-stu-id="10d1e-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="10d1e-280">SDK-Release für .NET Standard (v1.17.0)</span><span class="sxs-lookup"><span data-stu-id="10d1e-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-281">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-281">Categories</span></span>

- <span data-ttu-id="10d1e-282">Datum: 23.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="10d1e-283">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="10d1e-284">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-284">Impacted audience</span></span>

<span data-ttu-id="10d1e-285">Partner mit direkter Abrechnung und indirekte Anbieter, die am CSP-Programm teilnehmen und das Partner Center .NET SDK verwenden</span><span class="sxs-lookup"><span data-stu-id="10d1e-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-286">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-286">Details</span></span>

<span data-ttu-id="10d1e-287">Ab dem 23. März 2020 können Partner mit dem Herunterladen der Version von [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) zusammen mit aktualisierten [GitHub-Beispielen](https://github.com/Microsoft/Partner-Center-DotNet-Samples) für das öffentliche Partner Center SDK beginnen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="10d1e-288">Diese Version enthält Updates für die folgenden Methoden:</span><span class="sxs-lookup"><span data-stu-id="10d1e-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="10d1e-289">Überwachung aktualisiert: Neue Vorgangstypen</span><span class="sxs-lookup"><span data-stu-id="10d1e-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="10d1e-290">Es wurden neue [Vorgangstypen](https://docs.microsoft.com/partner-center/develop/auditing-resources) hinzugefügt, um zu wissen, wann der Kunde DAP genehmigt und beendet hat.</span><span class="sxs-lookup"><span data-stu-id="10d1e-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="10d1e-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="10d1e-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="10d1e-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="10d1e-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="10d1e-293">Überwachung aktualisiert: Neue Ressourcen- und Vorgangstypen</span><span class="sxs-lookup"><span data-stu-id="10d1e-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="10d1e-294">Es wurden neue [Ressourcen- und Vorgangstypen](https://docs.microsoft.com/partner-center/develop/auditing-resources) zur Unterstützung des Szenarios „Kundenverzeichnisrolle“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="10d1e-295">Neuer Ressourcentyp „CustomerDirectoryRole“</span><span class="sxs-lookup"><span data-stu-id="10d1e-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="10d1e-296">Vorgangstypen „AddUserMember“ and „RemoveUserMember“</span><span class="sxs-lookup"><span data-stu-id="10d1e-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="10d1e-297">SDK-Updates für Kundenkonten</span><span class="sxs-lookup"><span data-stu-id="10d1e-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="10d1e-298">Unterstützung für GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="10d1e-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="10d1e-299">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="10d1e-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="10d1e-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="10d1e-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="10d1e-301">Weitere Änderungen</span><span class="sxs-lookup"><span data-stu-id="10d1e-301">Additional changes</span></span>

<span data-ttu-id="10d1e-302">Die folgenden Änderungen werden im Rahmen des neuen E-Commerce-Verfahrens eingeführt und stehen derzeit nur per Einladung für Partner zur Verfügung, die an der Technical Preview des neuen E-Commerce-Verfahrens für M365/D365 teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="10d1e-303">Partner, die nicht an der Technical Preview des neuen E-Commerce-Verfahrens teilnehmen, sollten keine Auswirkungen bemerken, und es sollte Abwärtskompatibilität bestehen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="10d1e-304">Katalogänderungen:</span><span class="sxs-lookup"><span data-stu-id="10d1e-304">Catalog Changes:</span></span>

  - <span data-ttu-id="10d1e-305">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="10d1e-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="10d1e-306">Erwerb und Verwaltung:</span><span class="sxs-lookup"><span data-stu-id="10d1e-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="10d1e-307">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="10d1e-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="10d1e-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="10d1e-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="10d1e-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="10d1e-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="10d1e-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="10d1e-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="10d1e-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="10d1e-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="10d1e-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="10d1e-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-313">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-313">Next Steps</span></span>

- <span data-ttu-id="10d1e-314">Herunterladen der neuesten Version von [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="10d1e-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="10d1e-315">Herunterladen und Überprüfen der [GitHub-Beispiele](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="10d1e-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><span data-ttu-id="10d1e-316"><a name="12">Angebot im kommerziellen CSP-Marketplace und CSP-Incentives im Geschäftsjahr 2021 für berechtigte Angebote</a></span><span class="sxs-lookup"><span data-stu-id="10d1e-316"><a name="12"></a>CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-317">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-317">Categories</span></span>

- <span data-ttu-id="10d1e-318">Datum: 18.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="10d1e-319">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-320">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-320">Impacted audience</span></span>

<span data-ttu-id="10d1e-321">Indirekte Anbieter und Partner mit direkter Abrechnung im Cloud Solution Provider-Programm</span><span class="sxs-lookup"><span data-stu-id="10d1e-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="10d1e-322">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-322">Details</span></span>

<span data-ttu-id="10d1e-323">Indirekte Anbieter und Partner mit direkter Abrechnung im Cloud Solution Provider-Programm können Angebote von Drittanbietern verkaufen und ein Rabattincentive für jedes berechtigte Angebot eines Drittanbieters erhalten, für das Transaktionen in Partner Center oder im Azure-Portal durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="10d1e-324">Das Incentive erfolgt in Form eines Rabatts auf die in Rechnung gestellten Verkäufe für berechtigte Angebote und ist **bis zum 30. Juni 2021 verfügbar**.</span><span class="sxs-lookup"><span data-stu-id="10d1e-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="10d1e-325">Weitere Informationen zu diesem Angebot im kommerziellen CSP-Marketplace finden Sie weiter unten. Nehmen Sie noch heute Kontakt zu Ihren Kunden auf, um die richtigen Angebote für deren weiteren Erfolg und die digitale Transformationen zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="10d1e-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="10d1e-326">Wir arbeiten eng mit unabhängigen Softwareanbietern (Independent Software Vendors, ISVs) zusammen, um für Microsoft-Kunden die neuesten IaaS-und SaaS-Lösungen auf den Markt zu bringen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="10d1e-327">ISV-Herausgeber können den Vertrieb ihrer Angebote über den Microsoft-Partnerkanal ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="10d1e-328">Unsere für Incentives berechtigten Angebote fallen unter zwei Kategorien:</span><span class="sxs-lookup"><span data-stu-id="10d1e-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="10d1e-329">Ausgewählte SaaS- und IaaS-Angebote von Drittanbietern mit Incentivestatus für Azure-IP-Co-Selling</span><span class="sxs-lookup"><span data-stu-id="10d1e-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="10d1e-330">SaaS-Anwendungen, die in Teams oder mindestens zwei Microsoft 365-Produktivitäts-Apps integriert sind, z. B. PowerPoint, Word, Excel, Outlook oder SharePoint</span><span class="sxs-lookup"><span data-stu-id="10d1e-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="10d1e-331">Nächste Schritte und zusätzliche Ressourcen</span><span class="sxs-lookup"><span data-stu-id="10d1e-331">Next steps and resources</span></span>

- <span data-ttu-id="10d1e-332">Erfahren Sie, wie Sie [Partnerincentives](https://partner.microsoft.com/membership/partner-incentives) für den Verkauf berechtigter Marketplace-Apps (für Incentive-berechtigte Apps) erhalten.</span><span class="sxs-lookup"><span data-stu-id="10d1e-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="10d1e-333">Es werden monatlich neue Angebote hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="10d1e-334">Incentiveressourcen für Partner mit direkter Abrechnung im Cloud Solution Provider-Programm</span><span class="sxs-lookup"><span data-stu-id="10d1e-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="10d1e-335">Incentiveressourcen für indirekte Anbieter im Cloud Solution Provider-Programm</span><span class="sxs-lookup"><span data-stu-id="10d1e-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="10d1e-336">Sehen Sie sich diese [Präsentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) an, um mehr über das Verkaufen von Apps im kommerziellen Marketplace zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="10d1e-337">Weitere Ressourcen finden Sie [hier](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="10d1e-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="10d1e-338">Erkunden Sie den Katalog des kommerziellen Marketplace in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) oder im [Azure-Portal](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="10d1e-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="10d1e-339">Verwenden Sie [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) zum Integrieren von Apps in den Marketplace Ihres Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="10d1e-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="10d1e-340">Wenden Sie sich an ISVs, mit denen Sie geschäftlich tätig werden möchten.</span><span class="sxs-lookup"><span data-stu-id="10d1e-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="10d1e-341">Indirekte Anbieter müssen über APIs integriert werden und Wiederverkäufern Anleitungen dazu geben, welche Apps verkauft werden sollen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-342">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-342">Questions?</span></span>  

<span data-ttu-id="10d1e-343">In [diesem Artikel](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) finden Sie eine Übersicht über den kommerziellen Marketplace in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="10d1e-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="10d1e-344">Wenn Sie weitere Unterstützung benötigen, können Sie eine Supportanfrage in Partner Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="10d1e-345">Weitere Informationen finden Sie unter [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span><span class="sxs-lookup"><span data-stu-id="10d1e-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><span data-ttu-id="10d1e-346"><a name="11">Aktualisierung der Benennung und erforderlichen Komponenten für Power BI Premium-Angebote</a></span><span class="sxs-lookup"><span data-stu-id="10d1e-346"><a name="11"></a>Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-347">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-347">Categories</span></span>

- <span data-ttu-id="10d1e-348">Datum: 18.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="10d1e-349">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-350">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-350">Summary</span></span>

<span data-ttu-id="10d1e-351">Die endgültige Preisliste für den 1. April 2021 wird aktualisiert, um für Klarheit bei der Benennung und/oder den erforderlichen Komponenten für Angebote der Power BI Premium-Einzelbenutzerlizenz zu sorgen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-352">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-352">Impacted audience</span></span>

<span data-ttu-id="10d1e-353">Direkte und indirekte CSP-Partner (Cloud Solution Provider)</span><span class="sxs-lookup"><span data-stu-id="10d1e-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-354">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-354">Details</span></span>

<span data-ttu-id="10d1e-355">Die endgültige Preisliste für den 1. April 2021 wird aktualisiert, um für Klarheit bei der Benennung und/oder den erforderlichen Komponenten für Angebote der Power BI Premium-Einzelbenutzerlizenz zu sorgen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="10d1e-356">Verwenden Sie bis zur Aktualisierung der endgültigen Preisliste die Informationen in diesem Abschnitt, um sicherzustellen, dass das richtige Produkt bestellt wird.</span><span class="sxs-lookup"><span data-stu-id="10d1e-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="10d1e-357">Die folgenden Angaben umfassen die betroffene SKU und Informationen zu den erforderlichen Komponenten.</span><span class="sxs-lookup"><span data-stu-id="10d1e-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="10d1e-358">Angebotsanzeigename in der Preislistenvorschau vom 1. März</span><span class="sxs-lookup"><span data-stu-id="10d1e-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="10d1e-359">Aktualisierter Angebotsanzeigename in der endgültigen Preisliste für den 1. April</span><span class="sxs-lookup"><span data-stu-id="10d1e-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="10d1e-360">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="10d1e-361">Power BI Premium-Einzelbenutzerlizenz-Add-On (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="10d1e-362">Power BI Premium-Einzelbenutzerlizenz-Add-On **(Office)** (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="10d1e-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="10d1e-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="10d1e-364">Für den Erwerb dieses Angebots benötigen Kunden eine der folgenden erforderlichen Komponenten:</span><span class="sxs-lookup"><span data-stu-id="10d1e-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="10d1e-365">Angebotsanzeigename</span><span class="sxs-lookup"><span data-stu-id="10d1e-365">Offer display name</span></span> | <span data-ttu-id="10d1e-366">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="10d1e-367">Microsoft 365 E5 (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="10d1e-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="10d1e-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="10d1e-369">Microsoft 365 E5 ohne Audiokonferenz (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="10d1e-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="10d1e-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="10d1e-371">Office 365 E5 (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="10d1e-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="10d1e-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="10d1e-373">Office 365 E5-Testversion (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="10d1e-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="10d1e-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="10d1e-375">Office 365 E5 ohne Audiokonferenz (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="10d1e-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="10d1e-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="10d1e-377">Für den Erwerb des folgenden Power BI Premium-Angebots muss eine erforderliche Komponente vorhanden sein:</span><span class="sxs-lookup"><span data-stu-id="10d1e-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="10d1e-378">Angebotsanzeigename</span><span class="sxs-lookup"><span data-stu-id="10d1e-378">Offer display name</span></span> | <span data-ttu-id="10d1e-379">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="10d1e-380">Power BI Premium-Einzelbenutzerlizenz-Add-On (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="10d1e-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="10d1e-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="10d1e-382">Für den Erwerb dieses Angebots benötigen Kunden die folgende erforderliche Komponente:</span><span class="sxs-lookup"><span data-stu-id="10d1e-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="10d1e-383">Angebotsanzeigename</span><span class="sxs-lookup"><span data-stu-id="10d1e-383">Offer display name</span></span> | <span data-ttu-id="10d1e-384">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="10d1e-385">Power BI Pro (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="10d1e-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="10d1e-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="10d1e-387">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-387">Next steps</span></span>

<span data-ttu-id="10d1e-388">Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.</span><span class="sxs-lookup"><span data-stu-id="10d1e-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="10d1e-389">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-389">Questions?</span></span>

<span data-ttu-id="10d1e-390">Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><span data-ttu-id="10d1e-391"><a name="10"> Aktualisierungen der Preise im März für Microsoft 365 F3</a></span><span class="sxs-lookup"><span data-stu-id="10d1e-391"><a name="10"></a> March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-392">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-392">Categories</span></span>

- <span data-ttu-id="10d1e-393">Datum: 16.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="10d1e-394">Angebote/Märkte</span><span class="sxs-lookup"><span data-stu-id="10d1e-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-395">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-395">Summary</span></span>

<span data-ttu-id="10d1e-396">Falsche Preise für Microsoft 365 F3 in britischen Pfund (GBP) und Euro (EUR) im März 2021 wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-397">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-397">Impacted audience</span></span>

<span data-ttu-id="10d1e-398">Partner, die zwischen dem 1. und 17. März 2021 Microsoft 365 F3 in GBP oder EUR über das CSP-Programm (Cloud Solution Provider) erworben haben</span><span class="sxs-lookup"><span data-stu-id="10d1e-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-399">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-399">Details</span></span>

<span data-ttu-id="10d1e-400">Microsoft hat falsche Preise für Microsoft 365 F3 korrigiert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="10d1e-401">Die falschen Preise betreffen die Währungen GBP und EUR und nur Angebote, die zwischen dem 1. und 17. März 2021 erworben wurden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="10d1e-402">Die betroffenen Angebote und die entsprechenden Währungen sind nachfolgend aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="10d1e-403">Angebotsname</span><span class="sxs-lookup"><span data-stu-id="10d1e-403">Offer name</span></span> | <span data-ttu-id="10d1e-404">Währung</span><span class="sxs-lookup"><span data-stu-id="10d1e-404">Currency</span></span> | <span data-ttu-id="10d1e-405">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-405">Offer ID</span></span> | <span data-ttu-id="10d1e-406">Materialkennung</span><span class="sxs-lookup"><span data-stu-id="10d1e-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="10d1e-407">Microsoft 365 F3 (Wohltätigkeitsorganisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="10d1e-408">GBP</span><span class="sxs-lookup"><span data-stu-id="10d1e-408">GBP</span></span> | <span data-ttu-id="10d1e-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="10d1e-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="10d1e-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="10d1e-410">AAD-11626</span></span> |
| <span data-ttu-id="10d1e-411">Microsoft 365 F3 (Kommerziell)</span><span class="sxs-lookup"><span data-stu-id="10d1e-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="10d1e-412">EUR</span><span class="sxs-lookup"><span data-stu-id="10d1e-412">EUR</span></span>| <span data-ttu-id="10d1e-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="10d1e-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="10d1e-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="10d1e-414">AAA-89898</span></span> |
 
<span data-ttu-id="10d1e-415">Die lizenzbasierten Vorschaupreislisten für März und April wurden am 16. März um 17:00 Uhr (PST) aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-416">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-416">Next steps</span></span>

- <span data-ttu-id="10d1e-417">Partner sollten die aktuellen lizenzbasierten Preislisten (sowohl die Vorschaupreisliste für März als auch April) mit diesen Preiskorrekturen ggf. erneut herunterladen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="10d1e-418">Microsoft wird in den kommenden Wochen per E-Mail Kontakt mit den betroffenen Partnern aufnehmen, um sie über die weiteren Schritte zur Korrektur betroffener Transaktionen zu informieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-419">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-419">Questions?</span></span>

<span data-ttu-id="10d1e-420">Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="10d1e-421">Aktualisieren eines rechtlichen Firmennamens über Partner Center</span><span class="sxs-lookup"><span data-stu-id="10d1e-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-422">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-422">Categories</span></span>

- <span data-ttu-id="10d1e-423">Datum: 16.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="10d1e-424">Fördern von Effizienz und Skalierung</span><span class="sxs-lookup"><span data-stu-id="10d1e-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-425">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-425">Summary</span></span>

<span data-ttu-id="10d1e-426">Ab März 2021 können MPN-Partner (Microsoft Partner Network) und indirekte Wiederverkäufer im CSP-Programm (CSP Indirect Reseller) ihren rechtlichen Firmennamen über Partner Center aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-427">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-427">Impacted audience</span></span>

<span data-ttu-id="10d1e-428">MPN-Partner und indirekte Wiederverkäufer im CSP-Programm (gilt nicht für CSP-Partner mit direkter Abrechnung)</span><span class="sxs-lookup"><span data-stu-id="10d1e-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-429">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-429">Details</span></span>

<span data-ttu-id="10d1e-430">Ab März 2021 können MPN-Partner und indirekte Wiederverkäufer im CSP-Programm ihren rechtlichen Firmennamen über Partner Center auf konforme, selbstständige Weise aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="10d1e-431">Aufgrund dieser neuen Funktion müssen Partner kein Partner Center-Supportticket mehr einreichen, um ihren Firmennamen zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="10d1e-432">So können Partner bei diesen Aktivitäten viel Zeit einsparen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="10d1e-433">Weitere Informationen finden Sie unter [Aktualisieren des rechtlichen Geschäftsprofils](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="10d1e-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="10d1e-434">Vergewissern Sie sich, dass der Firmenname in Ihrem Rechtsgeschäftsprofil keine Rechtschreibfehler und Abkürzungen enthält und den formalen Geschäftsregistrierungsdatensätzen Ihres Unternehmens exakt entspricht.</span><span class="sxs-lookup"><span data-stu-id="10d1e-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="10d1e-435">Weitere Informationen zum Aktualisieren Ihres Organisationsprofils finden Sie unter [Überprüfen von Organisationsprofilen](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="10d1e-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-436">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-436">Next steps</span></span>

<span data-ttu-id="10d1e-437">Leiten Sie diese Informationen an das geeignete Team in Ihrem Unternehmen weiter, damit es seine Prozesse überprüfen und aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="10d1e-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-438">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-438">Questions?</span></span>

<span data-ttu-id="10d1e-439">Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="10d1e-440">Neuerungen bei der Weiterentwicklung des CSP-Programms (Cloud Solution Provider) und Änderungen des Open License-Programms</span><span class="sxs-lookup"><span data-stu-id="10d1e-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-441">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-441">Categories</span></span>

- <span data-ttu-id="10d1e-442">Datum: 15.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="10d1e-443">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-444">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-444">Summary</span></span>

<span data-ttu-id="10d1e-445">Das CSP-Programm (Cloud Solution Provider) wird um neue Angebote für unbefristete Software für den kommerziellen und öffentlichen Sektor erweitert, und es werden Änderungen am Open Licensing-Programm vorgenommen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-446">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-446">Impacted audience</span></span>

<span data-ttu-id="10d1e-447">Vertriebshändler und verwaltete Vertriebspartner, die Verkäufe über das Open License-Programm tätigen, sowie alle CSP-Partner, die Transaktionen für unbefristete Software durchführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-448">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-448">Details</span></span>

<span data-ttu-id="10d1e-449">Im September 2020 [kündigte Microsoft eine Reihe von Schritten auf einem Weg der digitalen Transformation an](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/), um die Verkaufschancen für Partner im CSP-Programm zu erweitern, einschließlich der Verfügbarkeit lokaler Software für Partner.</span><span class="sxs-lookup"><span data-stu-id="10d1e-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="10d1e-450">Diese Änderungen ermöglichen es Partnern, ihre Geschäfte auszubauen und ihre Reichweite auszudehnen, indem sie Softwarelizenzen in CSP nutzen und sich so erfolgreich in der heutigen cloudzentrierten Welt positionieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="10d1e-451">Darüber hinaus wird den Kunden der Übergang in die Cloud erleichtert, während Partner die Flexibilität erhalten, die sie für Hybrid Cloud-Umgebungen der Kunden benötigen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="10d1e-452">In Fortführung dieser digitalen Transformation kündigen wir die folgenden Änderungen an:</span><span class="sxs-lookup"><span data-stu-id="10d1e-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="10d1e-453">1\. Juli 2021: Der Preisliste für das Open License-Programm werden keine neuen SKUs, Produkte oder Promotions hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="10d1e-454">7\. Juli 2021: Zwei kommerzielle Angebote, Get Genuine Windows und Visual Studio Professional, sowie Angebote für den öffentlichen Sektor (Behörden, Bildungseinrichtungen und gemeinnützige Organisationen – siehe [Ankündigung](./2020-december.md#9)) werden der CSP-Preisliste für unbefristete Software hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="10d1e-455">Die Preisliste ist im Abschnitt „Software“ der Seite [Verkaufen > Preise und Angebote](https://partnercenter.microsoft.com/pcv/sales) in Partner Center zu finden und wird an diesem Datum neu veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="10d1e-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="10d1e-456">Ausführliche Informationen zur Weiterentwicklung des CSP-Programms und den Änderungen des Open License-Programms sind im folgenden Abschnitt **Nächste Schritte** angegeben.</span><span class="sxs-lookup"><span data-stu-id="10d1e-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-457">Nächste Schritte:</span><span class="sxs-lookup"><span data-stu-id="10d1e-457">Next Steps:</span></span>

- <span data-ttu-id="10d1e-458">Weiterentwicklung des CSP-Programms: Sehen Sie sich die Readiness-Materialien für [unbefristete Software im Cloud Solution Provider-Programm](https://partner.microsoft.com/resources/collection/software-in-csp#/) an.</span><span class="sxs-lookup"><span data-stu-id="10d1e-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="10d1e-459">Verwenden Sie diese [Readiness-Karte](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf), um schnell die richtigen Informationen für Ihre Rolle zu finden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="10d1e-460">Änderungen des Open License-Programms: Sehen Sie sich die Readiness-Materialien zur [Weiterentwicklung des CSP-Programms und Änderungen des Open License-Programms](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) an.</span><span class="sxs-lookup"><span data-stu-id="10d1e-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="10d1e-461">Verwenden Sie diese [Readiness-Karte](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf), um schnell die richtigen Informationen für Ihre Rolle zu finden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-462">Fragen</span><span class="sxs-lookup"><span data-stu-id="10d1e-462">Questions</span></span>

<span data-ttu-id="10d1e-463">Bei weiteren Fragen können Sie sich an die entsprechende CSP-Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="10d1e-464">Aktualisierung einer früheren Ankündigung: Premiumbewertungen, ein Add-On für Compliance Manager</span><span class="sxs-lookup"><span data-stu-id="10d1e-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-465">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-465">Categories</span></span>

- <span data-ttu-id="10d1e-466">Datum: 15.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="10d1e-467">Umsatzsteigerung</span><span class="sxs-lookup"><span data-stu-id="10d1e-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-468">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-468">Summary</span></span>

<span data-ttu-id="10d1e-469">Die Testangebote hätten nicht in der Preisliste aufgeführt werden sollen und werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-470">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-470">Impacted audience</span></span>

<span data-ttu-id="10d1e-471">Partner, die Transaktionen im Rahmen des Cloud Solution Provider-Programms ausführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-472">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-472">Details</span></span>

<span data-ttu-id="10d1e-473">Die Testangebote hätten nicht in die Preisliste aufgenommen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="10d1e-474">Sie werden aus der Preisliste für den 1. Mai 2021 entfernt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="10d1e-475">Die ursprüngliche Ankündigung finden Sie [hier](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="10d1e-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="10d1e-476">Zusätzliche Ressourcen</span><span class="sxs-lookup"><span data-stu-id="10d1e-476">Additional resources</span></span>

- [<span data-ttu-id="10d1e-477">Microsoft 365 E5 Security & Compliance</span><span class="sxs-lookup"><span data-stu-id="10d1e-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="10d1e-478">Erstellen und Verwalten von Bewertungen in Microsoft Compliance Manager – Microsoft 365 Compliance</span><span class="sxs-lookup"><span data-stu-id="10d1e-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="10d1e-479">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-479">Next steps</span></span>

<span data-ttu-id="10d1e-480">Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.</span><span class="sxs-lookup"><span data-stu-id="10d1e-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-481">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-481">Questions?</span></span>

<span data-ttu-id="10d1e-482">Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="10d1e-483">Migrieren Ihrer Lösungen von der OCP-Markteinführung (One Commercial Partner GTM) zum kommerziellen Microsoft-Marketplace</span><span class="sxs-lookup"><span data-stu-id="10d1e-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-484">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-484">Categories</span></span>

- <span data-ttu-id="10d1e-485">Datum: 12.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="10d1e-486">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-487">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-487">Summary</span></span>

<span data-ttu-id="10d1e-488">Ab dem 29. März 2021 können Sie nur eingeschränkte Markteinführungsfunktionen (GTM) in One Commercial Partner (OCP) nutzen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="10d1e-489">Es wird empfohlen, Ihre Lösungen zum kommerziellen Marketplace in Partner Center zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-490">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-490">Impacted audience</span></span>

<span data-ttu-id="10d1e-491">Organisationen, die Co-Selling-Aktivitäten für Lösungen in OCP GTM durchführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-492">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-492">Details</span></span>

<span data-ttu-id="10d1e-493">Im Dezember 2020 haben wir unseren Weg vom Microsoft OCP GTM-Tool zum kommerziellen Microsoft-Marketplace in Partner Center begonnen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="10d1e-494">Durch diese Umstellung werden die Funktionen des kommerziellen Marketplace erweitert, in dem Sie Ihre Lösungen Millionen von Kunden präsentieren, Verkaufschancen mit anderen Verkäufern von Microsoft und Partnern gemeinsam nutzen sowie innovative Lösungen gemeinsam anbieten können.</span><span class="sxs-lookup"><span data-stu-id="10d1e-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="10d1e-495">Der nächste Meilenstein dieser Umstellung erfolgt am 29. März 2021.</span><span class="sxs-lookup"><span data-stu-id="10d1e-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="10d1e-496">Ab diesem Zeitpunkt können Sie nur eingeschränkte GTM-Funktionen in OCP nutzen, wobei dann einige Felder schreibgeschützt sind.</span><span class="sxs-lookup"><span data-stu-id="10d1e-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="10d1e-497">Wenn Sie derzeit Co-Selling-Aktivitäten für Lösungen in OCP GTM durchführen, wird empfohlen, Ihre Lösungen zum kommerziellen Marketplace zu migrieren, um von den dessen Funktionen zu profitieren und ihre Veröffentlichungsvorgänge zu vereinfachen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="10d1e-498">Durch den Wechsel zum kommerziellen Marketplace wird Partner Center das primäre Ziel für Co-Selling-Veröffentlichungen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="10d1e-499">Dort können Sie Ihr Geschäft weiter ausbauen, indem Sie Ihre Lösungen mit unseren gemeinsam Kunden über dieselben Kanäle und produktinternen Funktionen verbinden, die wir für Microsoft-Produkte nutzen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="10d1e-500">[Weitere Informationen zum kommerziellen Marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="10d1e-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-501">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-501">Next steps</span></span>

- <span data-ttu-id="10d1e-502">Wenn Sie Ihre Lösungen noch nicht verschoben haben, befolgen Sie die Anweisungen im [Leitfaden für den Übergang](/azure/marketplace/co-sell-solution-migration), oder sehen Sie sich das [Videotutorial mit Schritt-für-Schritt-Anleitungen](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) an, um alle Migrationsaktivitäten durchzuführen und mit der Veröffentlichung Ihrer Lösungen im kommerziellen Marketplace zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="10d1e-503">Fragen zur eingeschränkten Funktionsweise von OCP GTM finden Sie unter den [häufig gestellten Fragen zu Co-Selling-Anforderungen für die Veröffentlichung im kommerziellen Microsoft-Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="10d1e-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="10d1e-504">(Siehe Abschnitt „Eingeschränkte GTM-Funktionen in OCP ab 29. März 2021“.)</span><span class="sxs-lookup"><span data-stu-id="10d1e-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-505">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-505">Questions?</span></span>

<span data-ttu-id="10d1e-506">Wenn Sie Fragen haben oder weitere Informationen benötigen, wenden Sie sich an den [Support](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="10d1e-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="10d1e-507">Ausweitung des neuen E-Commerce-Verfahrens im CSP-Programm (Cloud Solution Provider) für Azure auf Russland</span><span class="sxs-lookup"><span data-stu-id="10d1e-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-508">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-508">Categories</span></span>

- <span data-ttu-id="10d1e-509">Datum: 10.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="10d1e-510">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-511">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-511">Impacted audience</span></span>

<span data-ttu-id="10d1e-512">Alle Partner in Russland, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-513">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-513">Details</span></span>

<span data-ttu-id="10d1e-514">Wir freuen uns, die Verfügbarkeit des **neuen E-Commerce-Verfahrens in CSP für Azure in Russland** ab dem 10. März 2021 ankündigen zu können.</span><span class="sxs-lookup"><span data-stu-id="10d1e-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="10d1e-515">Dieses Verfahren optimiert die Art und Weise, wie Kunden Azure-Dienste kaufen und nutzen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="10d1e-516">Außerdem erhalten Partner im CSP-Programm einen konsistenten Überblick über Azure-Preise in allen Vertriebsprozessen, Preise in USD für globale Konsistenz, Anpassung des Abrechnungsdatums und Zugriff auf Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="10d1e-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-517">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-517">Next steps</span></span>

<span data-ttu-id="10d1e-518">Es stehen mehrere Ressourcen zur Einführung des neuen E-Commerce-Verfahrens für Azure sowie zusätzliche Informationen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="10d1e-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="10d1e-519">Im [Ressourcenkatalog für CSP-Programmupdates](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/) finden Sie die neuesten häufig gestellten Fragen, Foliensätze, Videos und mehr.</span><span class="sxs-lookup"><span data-stu-id="10d1e-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="10d1e-520">Softwarelizenzschlüssel und Softwaredownload in Partner Center</span><span class="sxs-lookup"><span data-stu-id="10d1e-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-521">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-521">Categories</span></span>

- <span data-ttu-id="10d1e-522">Datum: 04.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="10d1e-523">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-524">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-524">Summary</span></span>

<span data-ttu-id="10d1e-525">Die Partner Center-Funktionen für den Download von Software und Lizenzschlüssel wurden reaktiviert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-526">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-526">Impacted audience</span></span>

<span data-ttu-id="10d1e-527">Alle CSP-Partner (Cloud Solution Provider), die Transaktionen für Bestellungen von unbefristeter Software und Serverabonnementsoftware über Partner Center durchführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-528">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-528">Details</span></span>

<span data-ttu-id="10d1e-529">Als Reaktion auf Partnerfeedback werden die Partner Center-Funktionen zum Abrufen von Software und Lizenzschlüsseln für Bestellungen von unbefristeter Software und Serverabonnementsoftware reaktiviert.</span><span class="sxs-lookup"><span data-stu-id="10d1e-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="10d1e-530">Sie werden im vorherigen Zustand vor dem Entfernen am 19. Januar 2021 wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="10d1e-531">(Weitere Informationen finden Sie in der [Ankündigung](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="10d1e-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="10d1e-532">Beachten Sie, dass Lizenzschlüssel und Downloadlinks für Software wertvolle und sehr gefragte Ressourcen geistigen Eigentums sind.</span><span class="sxs-lookup"><span data-stu-id="10d1e-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="10d1e-533">Wenn diese kompromittiert werden, können die Aktivierungslimits schnell ausgeschöpft sein und eine negative Erfahrung für Kunden und Partner bewirken.</span><span class="sxs-lookup"><span data-stu-id="10d1e-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-534">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-534">Next steps</span></span>

<span data-ttu-id="10d1e-535">In den folgenden Ressourcen finden Sie Hinweise zur Verwendung und wichtige Anleitungen zur Verteilung von Softwareschlüsseln:</span><span class="sxs-lookup"><span data-stu-id="10d1e-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="10d1e-536">Verkaufen lokaler Software über das CSP-Programm</span><span class="sxs-lookup"><span data-stu-id="10d1e-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="10d1e-537">[Leitfaden zum neuen E-Commerce-Verfahren in Partner Center](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Abschnitt mit **Anleitungen zur Verteilung von Softwareschlüsseln**)</span><span class="sxs-lookup"><span data-stu-id="10d1e-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-538">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-538">Questions?</span></span>

<span data-ttu-id="10d1e-539">Wenn Sie weitere Fragen zu diesem Hinweis haben, können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="10d1e-540">Migrieren Ihrer Deals aus Partner Sales Connect (PSC) in Partner Center</span><span class="sxs-lookup"><span data-stu-id="10d1e-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-541">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-541">Categories</span></span>

- <span data-ttu-id="10d1e-542">Datum: 04.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="10d1e-543">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-544">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-544">Summary</span></span>

<span data-ttu-id="10d1e-545">Partner Sales Connect (PSC) wird ab dem 31. März 2021 auf den schreibgeschützten Zugriff umgestellt. Wir empfehlen daher dringend, mit der Migration Ihrer Deals aus PSC in Partner Center zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-546">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-546">Impacted audience</span></span>

<span data-ttu-id="10d1e-547">Partner mit Deals in PSC</span><span class="sxs-lookup"><span data-stu-id="10d1e-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-548">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-548">Details</span></span>

<span data-ttu-id="10d1e-549">Im Rahmen unserer gemeinsamen Verpflichtung zum Wachstum bietet Ihnen **Co-Selling mit Microsoft** die Möglichkeit, **entdeckt zu werden, ihr Fachwissen bereitzustellen und ihre Kundenbasis zu erweitern**, um somit positive Kundenergebnisse zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="10d1e-550">Bei einem durchschnittlichen Angebot, das **3,5-mal schneller** erfolgt als üblich, ermöglicht Ihnen die Verwaltung Ihrer Co-Selling-Aktivitäten in Partner Center den Verkauf über die Kanäle direkter Kunde, Partner und Microsoft-Verkäufer sowie die Verwaltung der gesamten Empfehlungspipeline an einem Ort.</span><span class="sxs-lookup"><span data-stu-id="10d1e-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="10d1e-551">**PSC** wird ab dem **31. März 2021** auf den **schreibgeschützten Zugriff** umgestellt. Wir empfehlen daher dringend, mit dem Wechsel zu Partner Center zu beginnen und dadurch Zugriff auf folgende Funktionsverbesserungen zu erhalten:</span><span class="sxs-lookup"><span data-stu-id="10d1e-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="10d1e-552">**Genauere Weiterleitung** der gemeinsam mit Microsoft genutzten Angebote an den richtigen Verkäufer, basierend auf der Art der benötigten Unterstützung</span><span class="sxs-lookup"><span data-stu-id="10d1e-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="10d1e-553">**Vorabprüfung von Angeboten** auf für Incentives-berechtigte Lösungen und Erfüllung der Kriterien für das ISV Connect-Programm, um den Genehmigungsprozess und den abschließenden Ausführungsnachweis zu vereinfachen</span><span class="sxs-lookup"><span data-stu-id="10d1e-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="10d1e-554">**Nahtlose Benutzeroberfläche** zum Verwalten all Ihrer Co-Selling-Verkaufschancen und qualifizierten Vertriebsleads an einem Ort</span><span class="sxs-lookup"><span data-stu-id="10d1e-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="10d1e-555">Darüber hinaus wurden kürzlich neue Features in Partner Center hinzugefügt, die Ihnen bei der Umstellung helfen:</span><span class="sxs-lookup"><span data-stu-id="10d1e-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="10d1e-556">Massenvorgänge für Co-Selling-Verkaufschancen</span><span class="sxs-lookup"><span data-stu-id="10d1e-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="10d1e-557">[Funktion für die Dealmigration](../psc-to-pc.md) (Abschnitt zur **Migration von PSC-Deals**)</span><span class="sxs-lookup"><span data-stu-id="10d1e-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="10d1e-558">Durch Verwendung der Co-Selling-Funktionalität in Partner Center haben Ihre Vertriebsteams mehr Zeit, sich auf die Pflege von Leads und Verkaufschancen, den Abschluss von Deals und den Aufbau dauerhafter Kundenbeziehungen zu konzentrieren.</span><span class="sxs-lookup"><span data-stu-id="10d1e-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="10d1e-559">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-559">Next steps</span></span>

<span data-ttu-id="10d1e-560">Im [Leitfaden für den Übergang zu Partner Center](../psc-to-pc.md) werden Sie durch die Schritte zum Migrieren Ihrer Deals von PSC zu Partner Center geführt.</span><span class="sxs-lookup"><span data-stu-id="10d1e-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-561">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-561">Questions?</span></span>

<span data-ttu-id="10d1e-562">Bei weiteren Fragen wenden Sie sich an den [Support](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="10d1e-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="10d1e-563">Neue Microsoft Dynamics 365-Produkte und -Angebote ab 1. April 2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-564">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-564">Categories</span></span>

- <span data-ttu-id="10d1e-565">Datum: 04.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="10d1e-566">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-567">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-567">Summary</span></span>

<span data-ttu-id="10d1e-568">Am 1. April 2021 führt Microsoft mehrere neue Produkte und Angebote für das CSP-Programm (Cloud Solution Provider) ein.</span><span class="sxs-lookup"><span data-stu-id="10d1e-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-569">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-569">Impacted audience</span></span>

<span data-ttu-id="10d1e-570">Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-571">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-571">Details</span></span>

<span data-ttu-id="10d1e-572">Am 1. April 2021 führt Microsoft die folgenden neuen Produkte und Angebote ein:</span><span class="sxs-lookup"><span data-stu-id="10d1e-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="10d1e-573">Power BI Premium-Einzelbenutzerlizenz</span><span class="sxs-lookup"><span data-stu-id="10d1e-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="10d1e-574">Geografische und Segmenterweiterung der USL für Customer Voice und Marketing</span><span class="sxs-lookup"><span data-stu-id="10d1e-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="10d1e-575">**Power BI Premium-Einzelbenutzerlizenz**</span><span class="sxs-lookup"><span data-stu-id="10d1e-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="10d1e-576">Microsoft führt die ersten Power BI Premium-Angebote mit Einzelbenutzerlizenz ein.</span><span class="sxs-lookup"><span data-stu-id="10d1e-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="10d1e-577">Power BI Premium wird derzeit nur in einem Kapazitätskonstrukt verkauft.</span><span class="sxs-lookup"><span data-stu-id="10d1e-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="10d1e-578">Die Power BI Premium-Einzelbenutzerlizenz bietet Zugriff auf Enterprise Business Intelligence (BI) und Analysefunktionen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="10d1e-579">Diese flexible Einzelplatzlizenzierung eignet sich für kleine bis mittelständische Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="10d1e-580">Weitere Informationen zu diesem Angebot finden Sie in den [Details zum Power BI-Release](/power-platform-release-plan/2020wave2/power-bi/planned-features).</span><span class="sxs-lookup"><span data-stu-id="10d1e-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="10d1e-581">**Angebotsdetails**</span><span class="sxs-lookup"><span data-stu-id="10d1e-581">**Offer details**</span></span>

<span data-ttu-id="10d1e-582">Beachten Sie, dass der Angebotsname leicht von der Preislistenvorschau abweicht.</span><span class="sxs-lookup"><span data-stu-id="10d1e-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="10d1e-583">Angebotsname</span><span class="sxs-lookup"><span data-stu-id="10d1e-583">Offer name</span></span> | <span data-ttu-id="10d1e-584">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="10d1e-585">Power BI Premium-Einzelbenutzerlizenz</span><span class="sxs-lookup"><span data-stu-id="10d1e-585">Power BI Premium Per User</span></span> | <span data-ttu-id="10d1e-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="10d1e-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="10d1e-587">Power BI Premium-Einzelbenutzerlizenz für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="10d1e-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="10d1e-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="10d1e-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="10d1e-589">Power BI Premium-Einzelbenutzerlizenz für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="10d1e-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="10d1e-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="10d1e-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="10d1e-591">Power BI Premium-Einzelbenutzerlizenz (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="10d1e-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="10d1e-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="10d1e-593">Power BI Premium-Einzelbenutzerlizenz-Add-On</span><span class="sxs-lookup"><span data-stu-id="10d1e-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="10d1e-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="10d1e-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="10d1e-595">Power BI Premium-Einzelbenutzerlizenz-Add-On für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="10d1e-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="10d1e-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="10d1e-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="10d1e-597">Power BI Premium-Einzelbenutzerlizenz-Add-On für Schüler/Studenten</span><span class="sxs-lookup"><span data-stu-id="10d1e-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="10d1e-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="10d1e-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="10d1e-599">Power BI Premium-Einzelbenutzerlizenz-Add-On (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="10d1e-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="10d1e-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="10d1e-601">**Geografische und Segmenterweiterung der USL für Customer Voice und Marketing**</span><span class="sxs-lookup"><span data-stu-id="10d1e-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="10d1e-602">Im Anschluss an die Einführung im Dezember 2020 wurden die USL-Angebote für Dynamics 365 Customer Voice und Marketing geändert, um neue Länder und weitere SKUs für gemeinnützige Organisationen und Bildungseinrichtungen hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="10d1e-603">Angebotsname</span><span class="sxs-lookup"><span data-stu-id="10d1e-603">Offer name</span></span> | <span data-ttu-id="10d1e-604">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="10d1e-605">USL für Dynamics 365 Customer Voice (Preise für Mitarbeiter gemeinnütziger Organisationen)</span><span class="sxs-lookup"><span data-stu-id="10d1e-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="10d1e-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="10d1e-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="10d1e-607">USL für Dynamics 365 Customer Voice für Lehrpersonal</span><span class="sxs-lookup"><span data-stu-id="10d1e-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="10d1e-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="10d1e-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="10d1e-609">Weitere Informationen zu diesen Angeboten finden Sie auf den folgenden Seiten:</span><span class="sxs-lookup"><span data-stu-id="10d1e-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="10d1e-610">Homepage von Dynamics 365 Customer Voice</span><span class="sxs-lookup"><span data-stu-id="10d1e-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="10d1e-611">Homepage von Dynamics 365 Marketing</span><span class="sxs-lookup"><span data-stu-id="10d1e-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="10d1e-612">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-612">Next steps</span></span>

<span data-ttu-id="10d1e-613">Sehen Sie sich die Ressourcen zu diesem Thema an, und geben Sie diese Informationen an die entsprechenden Mitarbeiter in Ihrer Organisation weiter.</span><span class="sxs-lookup"><span data-stu-id="10d1e-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="10d1e-614">Haben Sie Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-614">Questions?</span></span>

<span data-ttu-id="10d1e-615">Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="10d1e-616">Microsoft-Lösung für universelles Drucken jetzt in einigen Suites verfügbar</span><span class="sxs-lookup"><span data-stu-id="10d1e-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="10d1e-617">Kategorien</span><span class="sxs-lookup"><span data-stu-id="10d1e-617">Categories</span></span>

- <span data-ttu-id="10d1e-618">Datum: 03.03.2021</span><span class="sxs-lookup"><span data-stu-id="10d1e-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="10d1e-619">Funktionen</span><span class="sxs-lookup"><span data-stu-id="10d1e-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="10d1e-620">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="10d1e-620">Summary</span></span>

<span data-ttu-id="10d1e-621">Die Microsoft-Lösung für universelles Drucken steht ab dem 1. März 2021 für Transaktionen innerhalb ausgewählter Microsoft 365-Suites und als eigenständiges Add-On zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="10d1e-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="10d1e-622">Zielgruppe</span><span class="sxs-lookup"><span data-stu-id="10d1e-622">Impacted audience</span></span>

<span data-ttu-id="10d1e-623">Alle Partner, die Transaktionen im Rahmen des CSP-Programms (Cloud Solution Provider) ausführen</span><span class="sxs-lookup"><span data-stu-id="10d1e-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="10d1e-624">Details</span><span class="sxs-lookup"><span data-stu-id="10d1e-624">Details</span></span>

<span data-ttu-id="10d1e-625">[Universelles Drucken](https://aka.ms/universalprint) ist ein Microsoft 365-Druckdienst, durch den keine lokalen Druckerserver mehr benötigt werden und der Windows-Geräten das Drucken an Azure-registrierte Drucker ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="10d1e-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="10d1e-626">Er steht ab dem 1. März 2021 für Transaktionen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="10d1e-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="10d1e-627">Worker profitieren von treiberlosem Drucken, einer optimierten standortbasierten Druckerermittlung und einem intuitiven Druckvorgang ohne Lernkurve.</span><span class="sxs-lookup"><span data-stu-id="10d1e-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="10d1e-628">Geräte, die mit Azure Active Directory (Azure AD) verknüpft sind, nutzen vorhandene Azure AD-Anmeldeinformationen für sicheres Drucken.</span><span class="sxs-lookup"><span data-stu-id="10d1e-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="10d1e-629">Administratoren verwalten das Drucken über das Azure-Portal und können Drucker mit nativer Unterstützung für universelles Drucken problemlos verbinden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="10d1e-630">Universelles Drucken kann bei nicht kompatiblen Druckern mithilfe von Konnektorsoftware für universelles Drucken bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="10d1e-631">Universelles Drucken wird bei Einführung in Windows E3, A3, E5 und A5 sowie Microsoft 365 BP, F3, E3, A3, E5 und A5 aufgenommen.</span><span class="sxs-lookup"><span data-stu-id="10d1e-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="10d1e-632">**Angebotsdetails**</span><span class="sxs-lookup"><span data-stu-id="10d1e-632">**Offer details**</span></span>

<span data-ttu-id="10d1e-633">Beachten Sie, dass der Angebotsname leicht von der Preislistenvorschau abweicht.</span><span class="sxs-lookup"><span data-stu-id="10d1e-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="10d1e-634">Angebotsname</span><span class="sxs-lookup"><span data-stu-id="10d1e-634">Offer name</span></span> | <span data-ttu-id="10d1e-635">Angebots-ID</span><span class="sxs-lookup"><span data-stu-id="10d1e-635">Offer ID</span></span> | <span data-ttu-id="10d1e-636">Materialkennung</span><span class="sxs-lookup"><span data-stu-id="10d1e-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="10d1e-637">Universelles Drucken – Volumen-Add-On (500 Aufträge) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="10d1e-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="10d1e-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="10d1e-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="10d1e-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="10d1e-639">9BI-00004</span></span>   |
| <span data-ttu-id="10d1e-640">Universelles Drucken – Volumen-Add-On (500 Aufträge) für Lehrpersonal – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="10d1e-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="10d1e-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="10d1e-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="10d1e-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="10d1e-642">9BK-00004</span></span>   |
| <span data-ttu-id="10d1e-643">Universelles Drucken – Volumen-Add-On (500 Aufträge) – Windows</span><span class="sxs-lookup"><span data-stu-id="10d1e-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="10d1e-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="10d1e-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="10d1e-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="10d1e-645">9BI-00002</span></span>   |
| <span data-ttu-id="10d1e-646">Universelles Drucken – Volumen-Add-On (500 Aufträge) für Lehrpersonal – Windows</span><span class="sxs-lookup"><span data-stu-id="10d1e-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="10d1e-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="10d1e-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="10d1e-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="10d1e-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="10d1e-649">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="10d1e-649">Next steps</span></span>

<span data-ttu-id="10d1e-650">Machen Sie sich mit der Preisliste und der [Übersicht über universelles Drucken](/universal-print/fundamentals/universal-print-whatis) vertraut.</span><span class="sxs-lookup"><span data-stu-id="10d1e-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="10d1e-651">Geben Sie diese Informationen an die entsprechenden Kontakte in Ihrer Organisation weiter.</span><span class="sxs-lookup"><span data-stu-id="10d1e-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="10d1e-652">Noch Fragen?</span><span class="sxs-lookup"><span data-stu-id="10d1e-652">Questions?</span></span>

<span data-ttu-id="10d1e-653">Bei Fragen zu diesen Angeboten können Sie sich an die entsprechende Yammer-Community wenden.</span><span class="sxs-lookup"><span data-stu-id="10d1e-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
