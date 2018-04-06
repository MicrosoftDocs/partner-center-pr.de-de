---
title: Regionale CSP-Autorisierung | Partner Center
description: Mithilfe der regionalen Autorisierung können international tätige Partner jetzt Kunden in verschiedenen Regionen und Ländern auf der ganzen Welt einfacher verwalten.
ms.assetid: 22F9495E-E31A-41AE-BF51-3478AB2C8E78
author: MaggiePucciEvans
keywords: Azure AD-Mandanten, Mandanten konsolidieren, Mandantenstrategie, Mandanten in CSP, Partnerkonten in CSP, CSP-Märkte und -Gebiete, wo ich über CSP verkaufen?
ms.openlocfilehash: 45d9c6730cf3274d68915a453b1a33ed5239f68d
ms.sourcegitcommit: e56f07feb1c6748efda48a8d2cd00185331f904a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2018
---
# <a name="tenant-consolidation-strategies-in-csp"></a><span data-ttu-id="676cd-104">Mandanten-Konsolidierungsstrategien in CSP</span><span class="sxs-lookup"><span data-stu-id="676cd-104">Tenant consolidation strategies in CSP</span></span>


<span data-ttu-id="676cd-105">\[Einige Informationen beziehen sich auf die Vorabversion, die vor der kommerziellen Freigabe möglicherweise wesentlichen Änderungen unterliegt.</span><span class="sxs-lookup"><span data-stu-id="676cd-105">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="676cd-106">Microsoft übernimmt für die hier bereitgestellten Informationen keine Garantien, weder ausdrücklicher noch impliziter Art.\]</span><span class="sxs-lookup"><span data-stu-id="676cd-106">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="676cd-107">Mithilfe der regionalen Autorisierung können international tätige Partner jetzt Kunden in verschiedenen Regionen und Ländern auf der ganzen Welt einfacher verwalten.</span><span class="sxs-lookup"><span data-stu-id="676cd-107">With regional authorization, partners with international businesses can now more easily manage customers in different regions and countries around the world.</span></span> <span data-ttu-id="676cd-108">Dies reduziert die Anzahl von Mandanten, die von Partnern verwaltet werden müssen, sowie die Abrechnungsdaten, die von Partnern verarbeitet werden müssen. Darüber hinaus erhalten Partner eine stärker konsolidierte Sicht auf ihre Verkäufe.</span><span class="sxs-lookup"><span data-stu-id="676cd-108">This reduces the number of tenants that partners need to manage, reduces the billing dates that partners have to handle, and gives partners a more consolidated view of their sales.</span></span>

<span data-ttu-id="676cd-109">In der Vergangenheit mussten Partner in jedem Land physisch präsent sein, in dem sie Transaktionen durchführen wollten, mit Ausnahme der Europäischen Union/EFTA.</span><span class="sxs-lookup"><span data-stu-id="676cd-109">In the past, with the exception of the European Union/EFTA, partners needed to have a physical entity in each country where they wanted to transact.</span></span> <span data-ttu-id="676cd-110">Das bedeutete, dass Partner mehrere Mandanten mit unterschiedlichen Abrechnungsdaten und weiteren unterschiedlichen Einstellungen in Partner Center einrichten mussten.</span><span class="sxs-lookup"><span data-stu-id="676cd-110">This meant that partners needed to have multiple tenants set up in Partner Center, with multiple billing dates and other settings.</span></span> <span data-ttu-id="676cd-111">In Regionen wie Lateinamerika konnten Partner nicht problemlos mit Kunden aus einer benachbarten Region oder einem benachbarten Land arbeiten. In einigen Fällen war dies völlig unmöglich.</span><span class="sxs-lookup"><span data-stu-id="676cd-111">In regions such as Latin America, partners were not able to easily work with customers in a neighboring region or country, and in some cases, they were restricted completely.</span></span>

>**<span data-ttu-id="676cd-112">Hinweis</span><span class="sxs-lookup"><span data-stu-id="676cd-112">Note</span></span>**<br> <span data-ttu-id="676cd-113">Wenn Sie für [CSP für Microsoft-Cloud Deutschland](partner-center-for-microsoft-cloud-germany.md) registriert sind und Sie an Kunden in EU- und EFTA-Ländern/Regionen verkaufen, können Sie die Mandanten für Partner Center für Microsoft-Cloud Deutschland nicht mit Ihren anderen Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="676cd-113">If you are enrolled in [CSP for Microsoft Cloud Germany](partner-center-for-microsoft-cloud-germany.md) and you sell to customers in the EU and EFTA countries/regions, you cannot consolidate your tenant for Partner Center for Microsoft Cloud Germany with your other tenants.</span></span>  

## <a name="planning"></a><span data-ttu-id="676cd-114">Planen</span><span class="sxs-lookup"><span data-stu-id="676cd-114">Planning</span></span>

<span data-ttu-id="676cd-115">Partner haben mehrere Optionen für die Konsolidierung ihrer regionalen Mandanten. Diese werden im Folgenden beschrieben.</span><span class="sxs-lookup"><span data-stu-id="676cd-115">Partners have multiple options for consolidating their regional tenants, as outlined below.</span></span>

### <a name="separate-tenants-for-single-regions-or-countries"></a><span data-ttu-id="676cd-116">Getrennte Mandanten für die einzelnen Regionen oder Länder</span><span class="sxs-lookup"><span data-stu-id="676cd-116">Separate tenants for single regions or countries</span></span>

<span data-ttu-id="676cd-117">Die Mandantenkonsolidierung ist optional.</span><span class="sxs-lookup"><span data-stu-id="676cd-117">Tenant consolidation is optional.</span></span> <span data-ttu-id="676cd-118">Partner können internationale Kunden weiterhin über getrennte Mandanten verwalten, wie in der folgenden Tabelle gezeigt.</span><span class="sxs-lookup"><span data-stu-id="676cd-118">Partners can continue to manage their international customers with separate tenants, as shown in the following table.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="676cd-119">Partnerstandort(e)</span><span class="sxs-lookup"><span data-stu-id="676cd-119">Partner location(s)</span></span></th>
<th><span data-ttu-id="676cd-120">Abrechnungsdatum/-daten</span><span class="sxs-lookup"><span data-stu-id="676cd-120">Billing Date(s)</span></span></th>
<th><span data-ttu-id="676cd-121">Kundenstandort(e)</span><span class="sxs-lookup"><span data-stu-id="676cd-121">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="676cd-122">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="676cd-122">Colombia</span></span></p></td>
<td><p><span data-ttu-id="676cd-123">Abrechnungsdatum: 10. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-123">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="676cd-124">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="676cd-124">Colombia</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="676cd-125">Chile</span><span class="sxs-lookup"><span data-stu-id="676cd-125">Chile</span></span></p></td>
<td><p><span data-ttu-id="676cd-126">Abrechnungsdatum: 15. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-126">Billing date 15th</span></span></p></td>
<td><p><span data-ttu-id="676cd-127">Chile</span><span class="sxs-lookup"><span data-stu-id="676cd-127">Chile</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="676cd-128">Paraguay</span><span class="sxs-lookup"><span data-stu-id="676cd-128">Paraguay</span></span></p></td>
<td><p><span data-ttu-id="676cd-129">Abrechnungsdatum: 5. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-129">Billing date 5th</span></span></p></td>
<td><p><span data-ttu-id="676cd-130">Paraguay</span><span class="sxs-lookup"><span data-stu-id="676cd-130">Paraguay</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="676cd-131">Peru</span><span class="sxs-lookup"><span data-stu-id="676cd-131">Peru</span></span></p></td>
<td><p><span data-ttu-id="676cd-132">Abrechnungsdatum: 2. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-132">Billing date 2nd</span></span></p></td>
<td><p><span data-ttu-id="676cd-133">Peru</span><span class="sxs-lookup"><span data-stu-id="676cd-133">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="one-tenant-for-multiple-regions-or-countries"></a><span data-ttu-id="676cd-134">Ein einziger Mandant für mehrere Regionen oder Länder</span><span class="sxs-lookup"><span data-stu-id="676cd-134">One tenant for multiple regions or countries</span></span>


<span data-ttu-id="676cd-135">Partner können ihre Vorgänge aus mehreren CSP-Mandanten in einem einzigen CSP-Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="676cd-135">Partners can choose to consolidate their operations from multiple CSP tenants into a single CSP tenant.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="676cd-136">Partnerstandort</span><span class="sxs-lookup"><span data-stu-id="676cd-136">Partner location</span></span></th>
<th><span data-ttu-id="676cd-137">Abrechnungsdatum</span><span class="sxs-lookup"><span data-stu-id="676cd-137">Billing Date</span></span></th>
<th><span data-ttu-id="676cd-138">Kundenstandort(e)</span><span class="sxs-lookup"><span data-stu-id="676cd-138">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="676cd-139">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="676cd-139">Colombia</span></span></p></td>
<td><p><span data-ttu-id="676cd-140">Abrechnungsdatum: 10. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-140">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="676cd-141">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="676cd-141">Colombia</span></span></p>
<p><span data-ttu-id="676cd-142">Chile</span><span class="sxs-lookup"><span data-stu-id="676cd-142">Chile</span></span></p>
<p><span data-ttu-id="676cd-143">Paraguay</span><span class="sxs-lookup"><span data-stu-id="676cd-143">Paraguay</span></span></p>
<p><span data-ttu-id="676cd-144">Peru</span><span class="sxs-lookup"><span data-stu-id="676cd-144">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="some-tenants-for-some-regions-or-countries"></a><span data-ttu-id="676cd-145">Einige Mandanten für einige Regionen oder Länder</span><span class="sxs-lookup"><span data-stu-id="676cd-145">Some tenants for some regions or countries</span></span>


<span data-ttu-id="676cd-146">Partner können ihre Vorgänge aus mehreren CSP-Mandanten auf eine kleinere Zahl von CSP-Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="676cd-146">Partners can choose to consolidate their operations from multiple CSP tenants to fewer CSP tenants.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="676cd-147">Partnerstandort(e)</span><span class="sxs-lookup"><span data-stu-id="676cd-147">Partner location(s)</span></span></th>
<th><span data-ttu-id="676cd-148">Abrechnungsdatum/-daten</span><span class="sxs-lookup"><span data-stu-id="676cd-148">Billing Date(s)</span></span></th>
<th><span data-ttu-id="676cd-149">Kundenstandort(e)</span><span class="sxs-lookup"><span data-stu-id="676cd-149">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="676cd-150">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="676cd-150">Colombia</span></span></p></td>
<td><p><span data-ttu-id="676cd-151">Abrechnungsdatum: 10. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-151">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="676cd-152">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="676cd-152">Colombia</span></span></p>
<p><span data-ttu-id="676cd-153">Chile</span><span class="sxs-lookup"><span data-stu-id="676cd-153">Chile</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="676cd-154">Paraguay</span><span class="sxs-lookup"><span data-stu-id="676cd-154">Paraguay</span></span></p></td>
<td><p><span data-ttu-id="676cd-155">Abrechnungsdatum: 5. des Monats</span><span class="sxs-lookup"><span data-stu-id="676cd-155">Billing date 5th</span></span></p></td>
<td><p><span data-ttu-id="676cd-156">Paraguay</span><span class="sxs-lookup"><span data-stu-id="676cd-156">Paraguay</span></span></p>
<p><span data-ttu-id="676cd-157">Peru</span><span class="sxs-lookup"><span data-stu-id="676cd-157">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="consolidating-tenants"></a><span data-ttu-id="676cd-158">Konsolidieren von Mandanten</span><span class="sxs-lookup"><span data-stu-id="676cd-158">Consolidating tenants</span></span>


<span data-ttu-id="676cd-159">Wenn Sie Mandanten konsolidieren möchten, empfehlen wir Folgendes:</span><span class="sxs-lookup"><span data-stu-id="676cd-159">If you want to consolidate tenants, we recommend the following:</span></span>

-   <span data-ttu-id="676cd-160">**Mehrere Regionen/Länder, Transaktionen jedoch nur in einem Land/einer Region**.</span><span class="sxs-lookup"><span data-stu-id="676cd-160">**Multiple regions/countries but only one transacting**.</span></span> <span data-ttu-id="676cd-161">Wenn Sie Transaktionen nur in einem Land/einer Region durchführen, jedoch eine Reihe weiterer Mandanten eingerichtet haben, verwenden Sie den Mandanten, über den Sie Transaktionen durchführen, als neuen zentralen Mandanten für dieses Land/diese Region und stornieren die übrigen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="676cd-161">If you are only transacting in one country/region, but have a number of other tenants set up, use the transacting tenant as your new centralized tenant for that region and cancel your other tenants.</span></span>

-   **<span data-ttu-id="676cd-162">Mehrere Länder/Regionen, Transaktionen jedoch nur in einem Land/einer Region.</span><span class="sxs-lookup"><span data-stu-id="676cd-162">Multiple countries/regions but only one Transacting.</span></span>** <span data-ttu-id="676cd-163">Wenn Sie Transaktionen in einer Reihe von Ländern/Regionen durchführen, empfehlen wir eine Konsolidierung auf den Mandanten mit der größten Zahl von Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="676cd-163">If you are transacting in a number of countries/regions, we recommend that you centralize to the tenant with the largest number of seats.</span></span> <span data-ttu-id="676cd-164">Sie sollten die Abonnements in den Ländern/Regionen stornieren, in denen Sie kleinere Mengen an Lizenzen verwalten.</span><span class="sxs-lookup"><span data-stu-id="676cd-164">You should cancel the subscriptions in the countries/regions where you have smaller amounts of seats.</span></span>


## <a name="countryregion-information"></a><span data-ttu-id="676cd-165">Informationen zu Ländern/Regionen</span><span class="sxs-lookup"><span data-stu-id="676cd-165">Country/region information</span></span>


<span data-ttu-id="676cd-166">Berücksichtigen Sie vor der Konsolidierung von Mandanten die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="676cd-166">Consider the following before beginning consolidating tenants:</span></span>

-   <span data-ttu-id="676cd-167">**Wenn Ihr Microsoft-Verkaufsstandort die Vereinigten Staaten sind**, umfasst Ihr Gebiet Kunden in den Vereinigten Staaten.</span><span class="sxs-lookup"><span data-stu-id="676cd-167">**If your Microsoft sell-to location is the United States**, your Territory includes customers located in the United States.</span></span>

-   <span data-ttu-id="676cd-168">**Wenn Ihr Microsoft-Verkaufsstandort Kanada ist**, umfasst Ihr Gebiet Kunden in Kanada.</span><span class="sxs-lookup"><span data-stu-id="676cd-168">**If your Microsoft sell-to location is Canada**, your Territory includes customers located in Canada.</span></span>

-   <span data-ttu-id="676cd-169">**Wenn Ihr Microsoft-Verkaufsstandort Brasilien ist**, umfasst Ihr Gebiet Kunden in Brasilien.</span><span class="sxs-lookup"><span data-stu-id="676cd-169">**If your Microsoft sell-to location is Brazil**, your Territory includes customers located in Brazil.</span></span>

-   <span data-ttu-id="676cd-170">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Anguilla, Antigua und Barbuda, Antarktis, Argentinien, Aruba, Bahamas, Barbados, Belize, Bermuda, Bolivien, Bonaire, Saba, St. Eustatius, Britische Jungferninseln, Kaimaninseln, Chile, Kolumbien, Costa Rica, Curacao, Dominika, Dominikanische Republik, Ecuador, El Salvador, Falklandinseln, Französisch-Guayana, Grenada, Guadeloupe, Guatemala, Guyana, Haiti, Honduras, Jamaika, Martinique, Mexiko, Montserrat, Nicaragua, Panama, Paraguay, Peru, Puerto Rico, Saba, Saint Barthélemy, St. Kitts und Nevis, St. Lucia, St. Martin, St. Vincent und die Grenadinen, Sint Maarten, Südgeorgien und die Südlichen Sandwichinseln, Suriname, Trinidad und Tobago, Turks- und Caicosinseln, Uruguay, Venezuela, Amerikanische Jungferninseln.</span><span class="sxs-lookup"><span data-stu-id="676cd-170">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Anguilla, Antigua and Barbuda, Antarctica, Argentina, Aruba, Bahamas, Barbados, Belize, Bermuda, Bolivia, Bonaire, British Virgin Islands, Cayman Islands, Chile, Colombia, Costa Rica, Curacao, Dominica, Dominican Republic, Ecuador, El Salvador, Falkland Islands, French Guiana, Grenada, Guadeloupe, Guatemala, Guyana, Haiti, Honduras, Jamaica, Martinique, Mexico, Montserrat, Nicaragua, Panama, Paraguay, Peru, Puerto Rico, Saba, Saint Barthélemy, Saint Kitts and Nevis, Saint Lucia, Saint Martin, Saint Vincent and the Grenadines, Sint Eustatius, Sint Maarten, South Georgia and South Sandwich Islands, Suriname, Trinidad and Tobago, Turks and Caicos Islands, Uruguay, Venezuela, Virgin Islands.</span></span> 

-   <span data-ttu-id="676cd-171">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Ålandinseln, Andorra, Österreich, Belgien, Bouvetinsel, Bulgarien, Kroatien, Zypern, Tschechische Republik, Dänemark, Estland, Färöer, Finnland, Frankreich, Deutschland, Griechenland, Gibraltar, Guernsey, Grönland, Ungarn, Island, Irland, Isle of Man, Italien, Jersey, Jan Mayen, Lettland, Liechtenstein, Litauen, Luxemburg, Madagaskar, Malawi, Mali, Malta, Mayotte, Monaco, Niederlande, Neukaledonien, Norwegen, Polen, Portugal, Rumänien, San Marino, Slowakei, Slowenien, Spanien, Svalbard, Schweden, Schweiz, Vereinigtes Königreich, Vatikanstadt.</span><span class="sxs-lookup"><span data-stu-id="676cd-171">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Åland Islands, Andorra, Austria, Belgium, Bouvet Island, Bulgaria, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Faroe Islands, Finland, France, Germany, Greece, Gibraltar, Greenland, Guernsey, Hungary, Iceland, Ireland, Isle of Man, Italy, Jersey, Jan Mayen, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Monaco, Netherlands, Norway, Poland, Portugal, Romania, San Marino, Slovakia, Slovenia, Spain, Svalbard, Sweden, Switzerland, United Kingdom, Vatican City.</span></span> 

    >**<span data-ttu-id="676cd-172">Hinweis</span><span class="sxs-lookup"><span data-stu-id="676cd-172">Note</span></span>**<br> <span data-ttu-id="676cd-173">Wenn Sie für [CSP für Microsoft-Cloud Deutschland](partner-center-for-microsoft-cloud-germany.md) registriert sind und Sie an Kunden in EU- und EFTA-Ländern/Regionen verkaufen, können Sie die Mandanten für Partner Center für Microsoft-Cloud Deutschland nicht mit Ihren anderen Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="676cd-173">If you are enrolled in [CSP for Microsoft Cloud Germany](partner-center-for-microsoft-cloud-germany.md) and you sell to customers in the EU and EFTA countries/regions, you cannot consolidate your tenant for Partner Center for Microsoft Cloud Germany with your other tenants.</span></span>  


-   <span data-ttu-id="676cd-174">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Afghanistan, Albanien, Algerien, Armenien, Aserbeidschan, Bahrain, Belarus, Benin, Bosnien und Herzegowina, Britisches Territorium im Indischen Ozean, Burkina Faso, Burundi, Zentralafrikanische Republik, Chad, Komoren, Kongo, Kongo (DRK), Kongo, Djibouti, Ägypten, Äquatorialguinea, Eritrea, Französisch-Polynesien, Gabon, Gambia, Guinea, Guinea-Bissau, Georgien, Irak, Israel, Jordanien, Kasachstan, Kuwait, Kirgisistan, Libanon, Liberia, Libyen, Madagaskar, Malawi, Mali, Mayotte, Republik Moldau, Mongolei, Montenegro, Marokko, Neukaledonien, Niger, Oman, Pakistan, Palästinensische Behörde, Katar, Republik von Mazedonien (FYROM), Réunion, Saudi-Arabien, Serbien, Seychellen, Sierra Leone, Somalia, Südafrika, Tadschikistan, Togo, Tunesien, Türkei, Turkmenistan, Ukraine, Vereinigte Arabische Emirate, Usbekistan, Jemen, Simbabwe.</span><span class="sxs-lookup"><span data-stu-id="676cd-174">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Afghanistan, Albania, Algeria, Armenia, Azerbaijan, Bahrain, Belarus, Benin, Bosnia and Herzegovina, Burkina Faso, Burundi, Central African Republic, Chad, Comoros, Congo (DRC), Congo, Djibouti, Egypt, Equatorial Guinea, Eritrea, French Polynesia, Gabon, Gambia, Georgia, Guinea, Guinea-Bissau, Iraq, Israel, Jordan, Kazakhstan, Kuwait, Kyrgyzstan, Lebanon, Liberia, Libya, Madagascar, Malawi, Mali, Mayotte, Moldova, Mongolia, Montenegro, Morocco, New Caledonia, Niger, Oman, Pakistan, Palestinian Authority, Qatar, Republic of Macedonia (FYROM), Réunion, Saudi Arabia, Serbia, Seychelles, Sierra Leone, Somalia, South Africa, Tajikistan, Togo, Tunisia, Turkey, Turkmenistan, Ukraine, United Arab Emirates, Uzbekistan, Yemen, Zimbabwe.</span></span> 

-   <span data-ttu-id="676cd-175">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Angola, Botsuana, Britisches Territorium im Indischen Ozean, Cabo Verde, Kamerun, Elfenbeinküste, Ghana, Kamerun, Kenia, Kosovo, Lesotho, Mauritius, Mosambik, Namibia, Nigeria, Ruanda, Sambia, Senegal, Swasiland, Tansania, Uganda, Yemen, Sambia.</span><span class="sxs-lookup"><span data-stu-id="676cd-175">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Angola, Botswana, British Indian Ocean Territory, Cabo Verde, Cameroon, Côte d'Ivoire, Ethiopia, Ghana, Kenya, Kosovo, Lesotho, Mauritania, Mauritius, Mozambique, Namibia, Nigeria, Rwanda, Senegal, Swaziland, Tanzania, Uganda, Yemen, Zambia.</span></span> 

-   <span data-ttu-id="676cd-176">**Wenn Ihr Microsoft-Verkaufsstandort Russland ist**, umfasst Ihr Gebiet Kunden in Russland.</span><span class="sxs-lookup"><span data-stu-id="676cd-176">**If your Microsoft sell-to location is Russia**, your Territory includes customers located in Russia.</span></span>

-   <span data-ttu-id="676cd-177">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Amerikanisch-Samoa, Bangladesch, Bhutan, Brunei Darussalam, Kambodscha, Hongkong (SAR), Indonesien, Laos, Macau SAR, Malaysia, Malediven, Marshallinseln, Myanmar, Nepal, Papua-Neuguinea, Philippinen, Saint Pierre und Miquelon, Singapur, Sri Lanka, Thailand, Timor-Leste, Tonga, Vanuatu, Vietnam.</span><span class="sxs-lookup"><span data-stu-id="676cd-177">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: American Samoa, Bangladesh, Bhutan, Brunei, Darussalam, Cambodia, Hong Kong SAR, Indonesia, Laos, Macao SAR, Malaysia, Maldives, Myanmar, Nepal, Philippines, Saint Pierre and Miquelon, Samoa, Singapore, Sri Lanka, Thailand, Timor-Leste, Vanuatu, Vietnam.</span></span> 

-   <span data-ttu-id="676cd-178">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/Region in der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen in der folgenden Liste: Australien, Fidschi, Weihnachtsinsel, Kokosinseln, Cookinseln, Guam, Heard und McDonaldinseln, Kiribati, Marshallinseln, Mikronesien, Nauru, Niue, Norfolkinsel, Nördliche Marianen, Palau, Papua-Neuguinea, Pitcairninseln, Salomonen, Tokelau, Tonga, Tuvalu, Wallis und Futuna.</span><span class="sxs-lookup"><span data-stu-id="676cd-178">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Australia, Fiji, Christmas Island, Cocos (Keeling) Islands, Cook Islands, Guam, Heard Island and McDonald Islands, Kiribati, Marshall Islands, Micronesia, Nauru, Niue, Norfolk Island, Northern Mariana Islands, Palau, Papa New Guinea, Pitcairn Islands, Solomon Islands, Tokelau, Tonga, Tuvalu, Wallis and Futuna.</span></span> 

-   <span data-ttu-id="676cd-179">**Wenn Ihr Microsoft-Verkaufsstandort Neuseeland ist**, umfasst Ihr Gebiet Kunden in Neuseeland.</span><span class="sxs-lookup"><span data-stu-id="676cd-179">**If your Microsoft sell-to location is New Zealand**, your Territory includes customers located in New Zealand.</span></span>

-   <span data-ttu-id="676cd-180">**Wenn Ihr Microsoft-Verkaufsstandort Indien ist**, umfasst Ihr Gebiet Kunden in Indien.</span><span class="sxs-lookup"><span data-stu-id="676cd-180">**If your Microsoft sell-to location is India**, your Territory includes customers located in India.</span></span>

-   <span data-ttu-id="676cd-181">**Wenn Ihr Microsoft-Verkaufsstandort Japan ist**, umfasst Ihr Gebiet Kunden in Japan.</span><span class="sxs-lookup"><span data-stu-id="676cd-181">**If your Microsoft sell-to location is Japan**, your Territory includes customers located in Japan.</span></span>

-   <span data-ttu-id="676cd-182">**Wenn Ihr Microsoft-Verkaufsstandort Korea ist**, umfasst Ihr Gebiet Kunden in Korea.</span><span class="sxs-lookup"><span data-stu-id="676cd-182">**If your Microsoft sell-to location is Korea**, your Territory includes customers located in Korea.</span></span>

-   <span data-ttu-id="676cd-183">**Wenn Ihr Microsoft-Verkaufsstandort Taiwan ist**, umfasst Ihr Gebiet Kunden in Taiwan.</span><span class="sxs-lookup"><span data-stu-id="676cd-183">**If your Microsoft sell-to location is Taiwan**, your Territory includes customers located in Taiwan.</span></span>

## <a name="billing-currencies-by-country"></a><span data-ttu-id="676cd-184">Abrechnungswährungen nach Land</span><span class="sxs-lookup"><span data-stu-id="676cd-184">Billing currencies by country</span></span>

<span data-ttu-id="676cd-185">Ihr geografischer Standort bestimmt die Währung, in der Ihre Rechnungen gestellt werden, wie in der folgenden Tabelle gezeigt.</span><span class="sxs-lookup"><span data-stu-id="676cd-185">Your geographic location determines the currency in which you are billed, as shown in the following table.</span></span> <span data-ttu-id="676cd-186">Hinweis: Wenn Sie eine andere Abrechnungswährung verwenden möchten, müssen Sie aufgrund von steuerlichen und rechtlichen Auswirkungen einen neuen Mandanten erstellen und diese Währung angeben.</span><span class="sxs-lookup"><span data-stu-id="676cd-186">Note that due to tax and legal implications, if you want to use a different billing currency, you'll need to create a new tenant and specify that currency.</span></span> 

| <span data-ttu-id="676cd-187">Währung</span><span class="sxs-lookup"><span data-stu-id="676cd-187">Currency</span></span> | <span data-ttu-id="676cd-188">Land</span><span class="sxs-lookup"><span data-stu-id="676cd-188">Country</span></span> |
| ---- | ---- |
| <span data-ttu-id="676cd-189">USD</span><span class="sxs-lookup"><span data-stu-id="676cd-189">USD</span></span> | <span data-ttu-id="676cd-190">Albanien und St. Eustatius, Anguilla, Antarktis, Antigua und Barbuda, Argentinien, Armenien, Aruba, Aserbeidschan, Bahamas, Bahrain, Bangladesch, Barbados, Belarus, Belize, Benin, Bermuda, Bolivien, Bonaire, Brasilien, Britisches Territorium im Indischen Ozean, Brunei Darussalam, Burundi, Kamerun, Kaimaninseln, Zentralafrikanische Republik, Chile, Kolumbien, Komoren, Costa Rica, Curaçao, Dominikanische Republik, Ecuador, Ägypten, El Salvador, Äquatorialguinea, Fidschi, Französisch-Guayana, Französisch-Polynesien, Georgien, Ghana, Guatemala, Guinea-Bissau, Honduras, Hongkong (SAR), Indonesien, Irak, Israel, Jamaika, Kasachstan, Kenia, Kuwait, Kirgisistan, Libanon, Lesotho, Macau SAR, Madagaskar, Malawi, Malaysia, Mali, Mauretanien, Mauritius, Mayotte, Mexiko, Marokko, Namibia, Neukaledonien, Nicaragua, Nigeria, Oman, Pakistan, Panama, Paraguay, Peru, Philippinen, Puerto Rico, Katar, Réunion, Ruanda, Saba, St. Lucia, St. Martin, St. Vincent und die Grenadinen, Saudi-Arabien, Serbien, Seychellen, Sierra Leone, Singapur, St. Maarten, Somalia, Südafrika, Südsudan, Sri Lanka, Suriname, Swasiland, Tansania, Thailand, Timor-Leste, Togo, Trinidad und Tobago, Tunesien, Türkei, Turks- und Caicosinseln, Amerikanische Jungferninseln, Ukraine, Vereinigte Arabische Emirate, Vereinigte Staaten, Uruguay, Venezuela, Vietnam, Yemen.</span><span class="sxs-lookup"><span data-stu-id="676cd-190">Albania and Sint Eustatius, Anguilla, Antarctica, Antigua and Barbuda, Argentina, Armenia, Aruba, Azerbaijan, Bahamas, Bahrain, Bangladesh, Barbados, Belarus, Belize, Benin, Bermuda, Bolivia, Bonaire, Brazil, British Indian Ocean Territory, Brunei, Burundi, Cameroon, Cayman Islands, Central African Republic, Chile, Colombia, Comoros, Costa Rica, Curaçao, Dominican Republic, Ecuador, Egypt, El Salvador, Equatorial Guinea, Eritrea, French Guiana, French Polynesia, Georgia, Ghana, Guatemala, Guinea-Bissau, Honduras, Hong Kong SAR, Indonesia, Iraq, Israel, Jamaica, Kazakhstan, Kenya, Kuwait, Kyrgyzstan, Lebanon, Lesotho, Macao SAR, Madagascar, Malawi, Malaysia, Mali, Mauritania, Mauritius, Mayotte, Mexico, Morocco, Namibia, New Caledonia, Nicaragua, Nigeria, Oman, Pakistan, Panama, Paraguay, Peru, Philippines, Puerto Rico, Qatar, Reunion, Rwanda, Saba, Saint Lucia, Saint Martin, Saint Vincent and the Grenadines, Saudi Arabia, Serbia, Seychelles, Sierra Leone, Singapore, Sint Maarten, Somalia, South Africa, South Sudan, Sri Lanka, Suriname, Swaziland, Tanzania, Thailand, Timor-Leste, Togo, Trinidad and Tobago, Tunisia, Turkey, Turks and Caicos Islands, U.S. Virgin Islands, Ukraine, United Arab Emirates, United States, Uruguay, Venezuela, Vietnam, Yemen.</span></span>| 
| <span data-ttu-id="676cd-191">TWD</span><span class="sxs-lookup"><span data-stu-id="676cd-191">TWD</span></span> | <span data-ttu-id="676cd-192">Taiwan</span><span class="sxs-lookup"><span data-stu-id="676cd-192">Taiwan</span></span> |
| <span data-ttu-id="676cd-193">SEK</span><span class="sxs-lookup"><span data-stu-id="676cd-193">SEK</span></span> | <span data-ttu-id="676cd-194">Schweden</span><span class="sxs-lookup"><span data-stu-id="676cd-194">Sweden</span></span> |
| <span data-ttu-id="676cd-195">INR</span><span class="sxs-lookup"><span data-stu-id="676cd-195">INR</span></span> | <span data-ttu-id="676cd-196">Indien</span><span class="sxs-lookup"><span data-stu-id="676cd-196">India</span></span> |
| <span data-ttu-id="676cd-197">RUB</span><span class="sxs-lookup"><span data-stu-id="676cd-197">RUB</span></span> | <span data-ttu-id="676cd-198">Russland</span><span class="sxs-lookup"><span data-stu-id="676cd-198">Russia</span></span> |
| <span data-ttu-id="676cd-199">NZD</span><span class="sxs-lookup"><span data-stu-id="676cd-199">NZD</span></span> | <span data-ttu-id="676cd-200">Neuseeland, Vanuatu</span><span class="sxs-lookup"><span data-stu-id="676cd-200">New Zealand, Vanuatu</span></span> |
| <span data-ttu-id="676cd-201">NOK</span><span class="sxs-lookup"><span data-stu-id="676cd-201">NOK</span></span> | <span data-ttu-id="676cd-202">Jan Mayen, Norwegen, Svalbard</span><span class="sxs-lookup"><span data-stu-id="676cd-202">Jan Mayen, Norway, Svalbard</span></span> |
| <span data-ttu-id="676cd-203">KRW</span><span class="sxs-lookup"><span data-stu-id="676cd-203">KRW</span></span> | <span data-ttu-id="676cd-204">Südkorea</span><span class="sxs-lookup"><span data-stu-id="676cd-204">Korea</span></span> |
| <span data-ttu-id="676cd-205">JPY</span><span class="sxs-lookup"><span data-stu-id="676cd-205">JPY</span></span> | <span data-ttu-id="676cd-206">Japan</span><span class="sxs-lookup"><span data-stu-id="676cd-206">Japan</span></span> |
| <span data-ttu-id="676cd-207">GBP</span><span class="sxs-lookup"><span data-stu-id="676cd-207">GBP</span></span> | <span data-ttu-id="676cd-208">Isle Of Man, Jersey, Vereinigtes Königreich</span><span class="sxs-lookup"><span data-stu-id="676cd-208">Isle of Man, Jersey, United Kingdom</span></span> |
| <span data-ttu-id="676cd-209">EUR</span><span class="sxs-lookup"><span data-stu-id="676cd-209">EUR</span></span> | <span data-ttu-id="676cd-210">Andorra, Österreich, Belgien, Bouvetinsel, Kroatien, Tschechische Republik, Estland, Färöer, Finnland, Frankreich, Deutschland, Griechenland, Ungarn, Island, Irland, Italien, Lettland, Liechtenstein, Litauen, Luxemburg/Belgien, Niederlande, Polen, Portugal, Rumänien, San Marino, Slowakei, Slowenien, Spanien</span><span class="sxs-lookup"><span data-stu-id="676cd-210">Andorra, Austria, Belgium, Bouvet Island, Croatia, Czech Republic, Estonia, Faroe Islands, Finland, France, Germany, Greece, Hungary, Iceland, Ireland, Italy, Latvia, Liechtenstein, Lithuania, Luxembourg/Belgium, Netherlands, Poland, Portugal, Romania, San Marino, Slovakia, Slovenia, Spain</span></span> |
| <span data-ttu-id="676cd-211">DKK</span><span class="sxs-lookup"><span data-stu-id="676cd-211">DKK</span></span> | <span data-ttu-id="676cd-212">Dänemark</span><span class="sxs-lookup"><span data-stu-id="676cd-212">Denmark</span></span> |
| <span data-ttu-id="676cd-213">CHF</span><span class="sxs-lookup"><span data-stu-id="676cd-213">CHF</span></span> | <span data-ttu-id="676cd-214">Schweiz</span><span class="sxs-lookup"><span data-stu-id="676cd-214">Switzerland</span></span> |
| <span data-ttu-id="676cd-215">CAD</span><span class="sxs-lookup"><span data-stu-id="676cd-215">CAD</span></span> | <span data-ttu-id="676cd-216">Kanada</span><span class="sxs-lookup"><span data-stu-id="676cd-216">Canada</span></span> |
| <span data-ttu-id="676cd-217">AUD</span><span class="sxs-lookup"><span data-stu-id="676cd-217">AUD</span></span> | <span data-ttu-id="676cd-218">Australien, Weihnachtsinsel, Kokosinseln, Cookinseln, Fidschi, Heard und McDonaldinseln, Kiribati, Marshallinseln, Nauru, Niue, Norfolkinsel, Nördliche Marianen, Palau, Papua-Neuguinea, Pitcairninseln, Salomonen, Tokelau, Tonga, Tuvalu, Wallis und Futuna.</span><span class="sxs-lookup"><span data-stu-id="676cd-218">Australia, Christmas Island, Cocos (Keeling) Islands, Cook Islands, Fiji, Heard Island and McDonald Islands, Kiribati, Marshall Islands, Nauru, Niue, Norfolk Island, Northern Mariana Islands, Palau, Papua New Guinea, Pitcairn Islands, Solomon Islands, Tokelau, Tonga, Tuvalu, Wallis and Futuna.</span></span> |


 



