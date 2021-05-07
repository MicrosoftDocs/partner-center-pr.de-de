---
title: Verwalten von Standorten im Partnerkonto
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Erfahren Sie, wie Sie einen neuen Standort hinzufügen und wie die Standort-MPN-ID in Incentive-Programmen, CSP-Geschäftsaktionen, Abonnements und anderen Transaktionen verwendet wird.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702891"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="d7ee0-103">Verwalten von MPN-Kontostandorten und Hinzufügen (Löschen) eines Standorts</span><span class="sxs-lookup"><span data-stu-id="d7ee0-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="d7ee0-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="d7ee0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d7ee0-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="d7ee0-105">Global admin</span></span>
- <span data-ttu-id="d7ee0-106">Kontoadministrator</span><span class="sxs-lookup"><span data-stu-id="d7ee0-106">Account admin</span></span>

<span data-ttu-id="d7ee0-107">Die Standort-MPN-ID identifiziert jeden spezifischen Standort Ihres Unternehmens</span><span class="sxs-lookup"><span data-stu-id="d7ee0-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="d7ee0-108">und wird für die Registrierung bei Incentive-Programmen, für die Abwicklung von Transaktionen als Cloud Solution Provider (CSP) und andere geschäftliche Transaktionen verwendet.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="d7ee0-109">Die globale MPN-ID wird für transaktionsfremde Aktivitäten verwendet (etwa für Supportanfragen).</span><span class="sxs-lookup"><span data-stu-id="d7ee0-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="d7ee0-110">Hier ein typisches Szenario:</span><span class="sxs-lookup"><span data-stu-id="d7ee0-110">The following scenario is typical:</span></span>

<span data-ttu-id="d7ee0-111">Contoso hat sein globales Partnerkonto (Partner Global Account, PGA) im Vereinigten Königreich.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="d7ee0-112">Bei dem PGA handelt es sich um das registrierte Unternehmen, und seine globale MPN-ID wird für die Verwaltung aller transaktionsfremden Angelegenheiten verwendet.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="d7ee0-113">Contoso verfügt außerdem über Partnerstandortkonten (Partner Location Account, PLA), die den Niederlassungen oder Abteilungen an anderen Standorten im Vereinigten Königreich, Frankreich und den USA entsprechen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="d7ee0-114">In der MPN-Kontostruktur werden diese PLAs als eindeutige Standort-MPN-IDs dargestellt.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="d7ee0-115">Die PLAs werden für transaktionsbezogene Angelegenheiten (beispielsweise CSP- oder Incentive-Programme) verwendet.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="d7ee0-116">Auszahlungen sind an spezifische Standorte gebunden.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="d7ee0-117">Zwischen einem CSP-Mandanten und einer MPN-Standort-ID besteht eine 1:1-Beziehung.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur von MPN-Standorten":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="d7ee0-119">Voraussetzungen für das Hinzufügen eines neuen Kontos für ein CSP-Geschäft</span><span class="sxs-lookup"><span data-stu-id="d7ee0-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="d7ee0-120">Zum Hinzufügen eines neuen CSP-Geschäftskontos müssen Sie zunächst sicherstellen, dass die Voraussetzungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="d7ee0-121">Sie müssen über eine Standort-MPN-ID in dem Land verfügen, in dem Sie CSP-Geschäfte tätigen möchten.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="d7ee0-122">Wenn Sie einen neuen MPN-Standort erstellen möchten, lesen Sie „Hinzufügen eines MPN-Standorts“ weiter unten.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="d7ee0-123">Wenn Sie eine neue CSP Indirect Reseller-Registrierung erstellen möchten, lesen Sie [Arbeiten mit indirekten Anbietern](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="d7ee0-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="d7ee0-124">Denken Sie daran, sich mit den **neuen** Anmeldeinformationen für das **neue** CSP-Konto anzumelden.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="d7ee0-125">Verwenden Sie nicht Ihre schon vorhandenen Anmeldeinformationen, da Partner Center erkennt, dass Sie bereits über ein Konto verfügen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="d7ee0-126">Stimmen Sie der Microsoft Partner-Vereinbarung zu, und aktivieren Sie das Konto.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="d7ee0-127">Wenn Sie sich als Partner mit direkter Abrechnung registrieren möchten, lesen Sie die [Anforderungen für Partner mit direkter Abrechnung](direct-partner-new-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="d7ee0-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="d7ee0-128">Anzeigen und Aktualisieren Ihrer MPN-Standorte</span><span class="sxs-lookup"><span data-stu-id="d7ee0-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="d7ee0-129">Melden Sie sich mit den Anmeldeinformationen für Ihr MPN-Konto beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home) an.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="d7ee0-130">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="d7ee0-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="d7ee0-131">Wählen Sie über das Symbol **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Rechtliche Hinweise** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="d7ee0-132">Vergewissern Sie sich, dass auf der Registerkarte **Partner** keine Fehlermeldung im Banner angezeigt wird, in der Sie dazu aufgefordert werden, von PMC migrierte Standorte zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="d7ee0-133">Wenn Ihre Standorte in PMC nicht ordnungsgemäß eingerichtet wurden und noch nicht in PC übergegangen sind, müssen Sie diese Standorte aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screenshot zum Aktualisieren des Standorts":::
 
4.  <span data-ttu-id="d7ee0-135">Wählen Sie im Bildschirm **PMC-Standorte überprüfen** die Option **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="d7ee0-136">Aktualisieren Sie die folgenden Felder:</span><span class="sxs-lookup"><span data-stu-id="d7ee0-136">Update the following fields:</span></span>

- <span data-ttu-id="d7ee0-137">**Feld „Name“** : Stellen Sie sicher, dass der Name des Unternehmensstandorts korrekt ist.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="d7ee0-138">Wenn ein Duplikatfehler angezeigt wird, versuchen Sie, den Wert z. B. von „Contoso“ in „Contoso, Inc“ zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="d7ee0-139">**Feld „Juristische Entität“** : Stellen Sie sicher, dass Sie die juristische Entität ausgewählt haben, an die der Standort gebunden ist.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="d7ee0-140">**Felder „Adresszeile 1“ und „Adresszeile 2“** : Vergewissern Sie sich, dass die Adresse richtig ist.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="d7ee0-141">**Felder „Stadt“ und „Bundesland/Kanton“** : Stellen Sie sicher, dass die Kombination von Stadt und Bundesland/Kanton richtig ist.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="d7ee0-142">Es gibt Länder, bei denen das Dropdownmenü zur Auswahl des Bundeslands/Kantons verwendet wird. Bei anderen Ländern muss der Eintrag in das Feld manuell erfolgen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="d7ee0-143">**Feld „Postleitzahl“** : Stellen Sie sicher, dass das Feld für die Postleitzahl mit dem jeweiligen Land, der Region, der Stadt oder der Adresse übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="d7ee0-144">**Felder für Informationen zum Hauptansprechpartner**: Stellen Sie sicher, dass die Felder für den Vor- und Nachnamen ausgefüllt sind und dass es sich bei der geschäftlichen E-Mail-Adresse nicht um eine private Adresse handelt (z. B. @outlook.com, @live.com usw.).</span><span class="sxs-lookup"><span data-stu-id="d7ee0-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="d7ee0-145">**Feld „Telefonnummer“** : Vergewissern Sie sich, dass die Telefonnummer keine Sonderzeichen, Leerzeichen oder die Landeskennzahl enthält.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="d7ee0-146">Der im Feld „Telefonnummer“ eingegebene Wert umfasst immer maximal zehn Zeichen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="d7ee0-147">Wird keine Fehlermeldung angezeigt, wählen Sie unter **Einstellungen** die Optionen **Kontoeinstellungen**, **Organisationsprofil**, **Bezeichner** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="d7ee0-148">Suchen Sie nach der MPN-ID mit dem Typ „Standort“, der dem Land dieses CSP-Kontos entspricht, und verwenden Sie diese, um die Zuordnung abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="d7ee0-149">Wenn Sie die Standort-MPN-ID, die dem zu verwendenden CSP-Konto entspricht, nicht finden, können Sie einen neuen Standort hinzufügen, um eine neue MPN-ID zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="d7ee0-150">Weitere Informationen finden Sie im folgenden Abschnitt **Hinzufügen eines MPN-Standorts**.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="d7ee0-151">Hinzufügen eines MPN-Standorts</span><span class="sxs-lookup"><span data-stu-id="d7ee0-151">Add an MPN location</span></span>

1. <span data-ttu-id="d7ee0-152">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="d7ee0-153">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="d7ee0-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="d7ee0-154">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="d7ee0-155">Wählen Sie über das Symbol **Einstellungen** die **Kontoeinstellungen** und dann **Organisationsprofil** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="d7ee0-156">Wählen Sie **Rechtliche Hinweise** und dann auf der Registerkarte **Partner** die Option **Geschäftsstandorte** aus. Klicken Sie anschließend auf **Standort hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="d7ee0-157">Geben Sie die erforderlichen Details einschließlich Firmenname, Adresse und Ansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="d7ee0-158">Klicken Sie auf **Standort hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-158">Click **Add location**.</span></span> <span data-ttu-id="d7ee0-159">Dadurch wird eine neue MPN-ID für den neuen Standort erstellt, die Sie für CSP-Transaktionen und -Incentives verwenden können.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Hinzufügen eines neuen Rechtsgeschäfts":::

> [!NOTE]
> <span data-ttu-id="d7ee0-161">In Partner Center hinzugefügte Standorte können nicht mehr entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="d7ee0-162">Wenn Sie die richtige MPN-ID für die Anmeldung verwendet haben, wird **MPN** im linken Menü von Partner Center angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="d7ee0-163">Hinzufügen der Registrierungs-ID</span><span class="sxs-lookup"><span data-stu-id="d7ee0-163">Add the registration number ID</span></span>

<span data-ttu-id="d7ee0-164">Wenn Sie ein indirekter Anbieter, Partner mit direkter Abrechnung oder indirekter Wiederverkäufer sind und Geschäfte mit neuen Kunden oder Bestandskunden in den folgenden Ländern tätigen, müssen Sie Registrierungs-IDs für Ihr Unternehmen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="d7ee0-165">Ist das Land, in dem Sie geschäftlich tätig sind, nachfolgend nicht aufgelistet, ist die Angabe der Registrierungs-ID optional.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="d7ee0-166">Armenien</span><span class="sxs-lookup"><span data-stu-id="d7ee0-166">Armenia</span></span> 
- <span data-ttu-id="d7ee0-167">Aserbaidschan</span><span class="sxs-lookup"><span data-stu-id="d7ee0-167">Azerbaijan</span></span> 
- <span data-ttu-id="d7ee0-168">Belarus</span><span class="sxs-lookup"><span data-stu-id="d7ee0-168">Belarus</span></span> 
- <span data-ttu-id="d7ee0-169">Brasilien</span><span class="sxs-lookup"><span data-stu-id="d7ee0-169">Brazil</span></span> 
- <span data-ttu-id="d7ee0-170">Ungarn</span><span class="sxs-lookup"><span data-stu-id="d7ee0-170">Hungary</span></span> 
- <span data-ttu-id="d7ee0-171">Indien</span><span class="sxs-lookup"><span data-stu-id="d7ee0-171">India</span></span> 
- <span data-ttu-id="d7ee0-172">Irak</span><span class="sxs-lookup"><span data-stu-id="d7ee0-172">Iraq</span></span> 
- <span data-ttu-id="d7ee0-173">Kasachstan</span><span class="sxs-lookup"><span data-stu-id="d7ee0-173">Kazakhstan</span></span> 
- <span data-ttu-id="d7ee0-174">Kirgisistan</span><span class="sxs-lookup"><span data-stu-id="d7ee0-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="d7ee0-175">Moldawien</span><span class="sxs-lookup"><span data-stu-id="d7ee0-175">Moldova</span></span> 
- <span data-ttu-id="d7ee0-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="d7ee0-176">Myanmar</span></span> 
- <span data-ttu-id="d7ee0-177">Polen</span><span class="sxs-lookup"><span data-stu-id="d7ee0-177">Poland</span></span> 
- <span data-ttu-id="d7ee0-178">Russland</span><span class="sxs-lookup"><span data-stu-id="d7ee0-178">Russia</span></span> 
- <span data-ttu-id="d7ee0-179">Saudi-Arabien</span><span class="sxs-lookup"><span data-stu-id="d7ee0-179">Saudi Arabia</span></span> 
- <span data-ttu-id="d7ee0-180">Südafrika</span><span class="sxs-lookup"><span data-stu-id="d7ee0-180">South Africa</span></span> 
- <span data-ttu-id="d7ee0-181">Südsudan</span><span class="sxs-lookup"><span data-stu-id="d7ee0-181">South Sudan</span></span>  
- <span data-ttu-id="d7ee0-182">Tadschikistan</span><span class="sxs-lookup"><span data-stu-id="d7ee0-182">Tajikistan</span></span> 
- <span data-ttu-id="d7ee0-183">Thailand</span><span class="sxs-lookup"><span data-stu-id="d7ee0-183">Thailand</span></span>
- <span data-ttu-id="d7ee0-184">Türkei</span><span class="sxs-lookup"><span data-stu-id="d7ee0-184">Turkey</span></span> 
- <span data-ttu-id="d7ee0-185">Ukraine</span><span class="sxs-lookup"><span data-stu-id="d7ee0-185">Ukraine</span></span> 
- <span data-ttu-id="d7ee0-186">Vereinigte Arabische Emirate</span><span class="sxs-lookup"><span data-stu-id="d7ee0-186">United Arab Emirates</span></span> 
- <span data-ttu-id="d7ee0-187">Usbekistan</span><span class="sxs-lookup"><span data-stu-id="d7ee0-187">Uzbekistan</span></span> 
- <span data-ttu-id="d7ee0-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="d7ee0-188">Venezuela</span></span>
- <span data-ttu-id="d7ee0-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="d7ee0-189">Vietnam</span></span> 


<span data-ttu-id="d7ee0-190">Weitere Informationen finden Sie unter [Informationen zur Registrierungs-ID](reg-number-id.md).</span><span class="sxs-lookup"><span data-stu-id="d7ee0-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="d7ee0-191">Löschen eines Standorts</span><span class="sxs-lookup"><span data-stu-id="d7ee0-191">Delete a location</span></span>

<span data-ttu-id="d7ee0-192">Um einen Standort aus Ihrem Konto zu löschen, müssen Sie sich an den [Partner-Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) wenden.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="d7ee0-193">Vergewissern Sie sich, dass Ihnen die Auswirkungen dieser Aktion bekannt sind.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="d7ee0-194">Gelöschte Standorte können nicht abgerufen werden, und alle Elemente, die mit dieser bestimmten MPN-ID verknüpft sind, werden nicht mehr erkannt oder sind für Ihr Unternehmen nicht mehr aktiv.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="d7ee0-195">Ändern des Lands für das globale Partnerkonto</span><span class="sxs-lookup"><span data-stu-id="d7ee0-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="d7ee0-196">Melden Sie sich mit dem MPN-Konto im Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="d7ee0-197">(Ihre MPN-Anmeldeinformationen können sich von Ihren CSP-Anmeldeinformationen unterscheiden.)</span><span class="sxs-lookup"><span data-stu-id="d7ee0-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="d7ee0-198">Das MPN-Konto sollte über globale Administratorrechte oder Kontoadministratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="d7ee0-199">Wechseln Sie auf der Registerkarte **Partner** zu **Geschäftsstandorte**, und prüfen Sie die Liste der Standorte, um sicherzustellen, dass der Standort, den Sie als juristische Entität wünschen, aufgeführt ist.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="d7ee0-200">Zum Hinzufügen eines Standorts klicken Sie auf **Standort hinzufügen**, und geben Sie im Flyout die erforderlichen Details einschließlich Firmenname, Adresse und Hauptansprechpartner für den Standort an, den Sie Ihrem Unternehmen hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="d7ee0-201">Wählen Sie neben der Dropdownliste **Land/Region** die Option **Land ändern** aus, und folgen Sie den angegebenen Schritten.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Flyout mit Daten des Rechtsgeschäftsprofils":::

5. <span data-ttu-id="d7ee0-203">Klicken Sie auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-203">Click **Save**.</span></span>

6. <span data-ttu-id="d7ee0-204">Das Land des globalen MPN-Kontos wird in das neue rechtsgültige Land geändert.</span><span class="sxs-lookup"><span data-stu-id="d7ee0-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="d7ee0-205">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d7ee0-205">Next steps</span></span>

- <span data-ttu-id="d7ee0-206">Erfahren Sie mehr über den [Überprüfungsprozess](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="d7ee0-206">Learn about the [verification process](verification-responses.md).</span></span>
