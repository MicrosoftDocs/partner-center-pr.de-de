---
title: Regionale CSP-Autorisierung | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: Mithilfe der regionalen Autorisierung können international tätige Partner jetzt Kunden in verschiedenen Regionen und Ländern auf der ganzen Welt einfacher verwalten.
ms.assetid: 22F9495E-E31A-41AE-BF51-3478AB2C8E78
author: MaggiePucciEvans
ms.author: evansma
keywords: Azure AD-Mandanten, Mandanten konsolidieren, Mandantenstrategie, Mandanten in CSP, Partnerkonten in CSP, CSP-Märkte und -Gebiete, wo ich über CSP verkaufen?
ms.localizationpriority: medium
ms.openlocfilehash: 351fbad0bfc818b16ca7a40eccedefb4dfea9307
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796633"
---
# <a name="tenant-consolidation-strategies-in-csp"></a><span data-ttu-id="91487-104">Mandanten-Konsolidierungsstrategien in CSP</span><span class="sxs-lookup"><span data-stu-id="91487-104">Tenant consolidation strategies in CSP</span></span>


<span data-ttu-id="91487-105">\[Einige Informationen beziehen sich auf die Vorabversion, die vor der kommerziellen Freigabe möglicherweise wesentlichen Änderungen unterliegt.</span><span class="sxs-lookup"><span data-stu-id="91487-105">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="91487-106">Microsoft übernimmt für die hier bereitgestellten Informationen keine Garantien, weder ausdrücklicher noch impliziter Art.\]</span><span class="sxs-lookup"><span data-stu-id="91487-106">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="91487-107">Mithilfe der regionalen Autorisierung können international tätige Partner jetzt Kunden in verschiedenen Regionen und Ländern auf der ganzen Welt einfacher verwalten.</span><span class="sxs-lookup"><span data-stu-id="91487-107">With regional authorization, partners with international businesses can now more easily manage customers in different regions and countries around the world.</span></span> <span data-ttu-id="91487-108">Dies reduziert die Anzahl von Mandanten, die von Partnern verwaltet werden müssen, sowie die Abrechnungsdaten, die von Partnern verarbeitet werden müssen. Darüber hinaus erhalten Partner eine stärker konsolidierte Sicht auf ihre Verkäufe.</span><span class="sxs-lookup"><span data-stu-id="91487-108">This reduces the number of tenants that partners need to manage, reduces the billing dates that partners have to handle, and gives partners a more consolidated view of their sales.</span></span>

<span data-ttu-id="91487-109">In der Vergangenheit mussten Partner in jedem Land physisch präsent sein, in dem sie Transaktionen durchführen wollten, mit Ausnahme der Europäischen Union/EFTA.</span><span class="sxs-lookup"><span data-stu-id="91487-109">In the past, with the exception of the European Union/EFTA, partners needed to have a physical entity in each country where they wanted to transact.</span></span> <span data-ttu-id="91487-110">Das bedeutete, dass Partner mehrere Mandanten mit unterschiedlichen Abrechnungsdaten und weiteren unterschiedlichen Einstellungen in Partner Center einrichten mussten.</span><span class="sxs-lookup"><span data-stu-id="91487-110">This meant that partners needed to have multiple tenants set up in Partner Center, with multiple billing dates and other settings.</span></span> <span data-ttu-id="91487-111">In Regionen wie Lateinamerika konnten Partner nicht problemlos mit Kunden aus einer benachbarten Region oder einem benachbarten Land arbeiten. In einigen Fällen war dies völlig unmöglich.</span><span class="sxs-lookup"><span data-stu-id="91487-111">In regions such as Latin America, partners were not able to easily work with customers in a neighboring region or country, and in some cases, they were restricted completely.</span></span>

> [!NOTE]  
>  <span data-ttu-id="91487-112">Wenn Sie für [CSP für Microsoft-Cloud Deutschland](partner-center-for-microsoft-cloud-germany.md) registriert sind und Sie an Kunden in EU- und EFTA-Ländern/Regionen verkaufen, können Sie die Mandanten für Partner Center für Microsoft-Cloud Deutschland nicht mit Ihren anderen Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="91487-112">If you are enrolled in [CSP for Microsoft Cloud Germany](partner-center-for-microsoft-cloud-germany.md) and you sell to customers in the EU and EFTA countries/regions, you cannot consolidate your tenant for Partner Center for Microsoft Cloud Germany with your other tenants.</span></span>  

## <a name="planning"></a><span data-ttu-id="91487-113">Planen</span><span class="sxs-lookup"><span data-stu-id="91487-113">Planning</span></span>

<span data-ttu-id="91487-114">Partner haben mehrere Optionen für die Konsolidierung ihrer regionalen Mandanten. Diese werden im Folgenden beschrieben.</span><span class="sxs-lookup"><span data-stu-id="91487-114">Partners have multiple options for consolidating their regional tenants, as outlined below.</span></span>

### <a name="separate-tenants-for-single-regions-or-countries"></a><span data-ttu-id="91487-115">Getrennte Mandanten für die einzelnen Regionen oder Länder</span><span class="sxs-lookup"><span data-stu-id="91487-115">Separate tenants for single regions or countries</span></span>

<span data-ttu-id="91487-116">Die Mandantenkonsolidierung ist optional.</span><span class="sxs-lookup"><span data-stu-id="91487-116">Tenant consolidation is optional.</span></span> <span data-ttu-id="91487-117">Partner können internationale Kunden weiterhin über getrennte Mandanten verwalten, wie in der folgenden Tabelle gezeigt.</span><span class="sxs-lookup"><span data-stu-id="91487-117">Partners can continue to manage their international customers with separate tenants, as shown in the following table.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="91487-118">Partnerstandort(e)</span><span class="sxs-lookup"><span data-stu-id="91487-118">Partner location(s)</span></span></th>
<th><span data-ttu-id="91487-119">Abrechnungsdatum/-daten</span><span class="sxs-lookup"><span data-stu-id="91487-119">Billing Date(s)</span></span></th>
<th><span data-ttu-id="91487-120">Kundenstandort(e)</span><span class="sxs-lookup"><span data-stu-id="91487-120">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="91487-121">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="91487-121">Colombia</span></span></p></td>
<td><p><span data-ttu-id="91487-122">Abrechnungsdatum: 10. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-122">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="91487-123">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="91487-123">Colombia</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="91487-124">Chile</span><span class="sxs-lookup"><span data-stu-id="91487-124">Chile</span></span></p></td>
<td><p><span data-ttu-id="91487-125">Abrechnungsdatum: 15. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-125">Billing date 15th</span></span></p></td>
<td><p><span data-ttu-id="91487-126">Chile</span><span class="sxs-lookup"><span data-stu-id="91487-126">Chile</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="91487-127">Paraguay</span><span class="sxs-lookup"><span data-stu-id="91487-127">Paraguay</span></span></p></td>
<td><p><span data-ttu-id="91487-128">Abrechnungsdatum: 5. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-128">Billing date 5th</span></span></p></td>
<td><p><span data-ttu-id="91487-129">Paraguay</span><span class="sxs-lookup"><span data-stu-id="91487-129">Paraguay</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="91487-130">Peru</span><span class="sxs-lookup"><span data-stu-id="91487-130">Peru</span></span></p></td>
<td><p><span data-ttu-id="91487-131">Abrechnungsdatum: 2. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-131">Billing date 2nd</span></span></p></td>
<td><p><span data-ttu-id="91487-132">Peru</span><span class="sxs-lookup"><span data-stu-id="91487-132">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="one-tenant-for-multiple-regions-or-countries"></a><span data-ttu-id="91487-133">Ein einziger Mandant für mehrere Regionen oder Länder</span><span class="sxs-lookup"><span data-stu-id="91487-133">One tenant for multiple regions or countries</span></span>


<span data-ttu-id="91487-134">Partner können ihre Vorgänge aus mehreren CSP-Mandanten in einem einzigen CSP-Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="91487-134">Partners can choose to consolidate their operations from multiple CSP tenants into a single CSP tenant.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="91487-135">Partnerstandort</span><span class="sxs-lookup"><span data-stu-id="91487-135">Partner location</span></span></th>
<th><span data-ttu-id="91487-136">Abrechnungsdatum</span><span class="sxs-lookup"><span data-stu-id="91487-136">Billing Date</span></span></th>
<th><span data-ttu-id="91487-137">Kundenstandort(e)</span><span class="sxs-lookup"><span data-stu-id="91487-137">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="91487-138">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="91487-138">Colombia</span></span></p></td>
<td><p><span data-ttu-id="91487-139">Abrechnungsdatum: 10. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-139">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="91487-140">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="91487-140">Colombia</span></span></p>
<p><span data-ttu-id="91487-141">Chile</span><span class="sxs-lookup"><span data-stu-id="91487-141">Chile</span></span></p>
<p><span data-ttu-id="91487-142">Paraguay</span><span class="sxs-lookup"><span data-stu-id="91487-142">Paraguay</span></span></p>
<p><span data-ttu-id="91487-143">Peru</span><span class="sxs-lookup"><span data-stu-id="91487-143">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="some-tenants-for-some-regions-or-countries"></a><span data-ttu-id="91487-144">Einige Mandanten für einige Regionen oder Länder</span><span class="sxs-lookup"><span data-stu-id="91487-144">Some tenants for some regions or countries</span></span>


<span data-ttu-id="91487-145">Partner können ihre Vorgänge aus mehreren CSP-Mandanten auf eine kleinere Zahl von CSP-Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="91487-145">Partners can choose to consolidate their operations from multiple CSP tenants to fewer CSP tenants.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="91487-146">Partnerstandort(e)</span><span class="sxs-lookup"><span data-stu-id="91487-146">Partner location(s)</span></span></th>
<th><span data-ttu-id="91487-147">Abrechnungsdatum/-daten</span><span class="sxs-lookup"><span data-stu-id="91487-147">Billing Date(s)</span></span></th>
<th><span data-ttu-id="91487-148">Kundenstandort(e)</span><span class="sxs-lookup"><span data-stu-id="91487-148">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="91487-149">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="91487-149">Colombia</span></span></p></td>
<td><p><span data-ttu-id="91487-150">Abrechnungsdatum: 10. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-150">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="91487-151">Kolumbien</span><span class="sxs-lookup"><span data-stu-id="91487-151">Colombia</span></span></p>
<p><span data-ttu-id="91487-152">Chile</span><span class="sxs-lookup"><span data-stu-id="91487-152">Chile</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="91487-153">Paraguay</span><span class="sxs-lookup"><span data-stu-id="91487-153">Paraguay</span></span></p></td>
<td><p><span data-ttu-id="91487-154">Abrechnungsdatum: 5. des Monats</span><span class="sxs-lookup"><span data-stu-id="91487-154">Billing date 5th</span></span></p></td>
<td><p><span data-ttu-id="91487-155">Paraguay</span><span class="sxs-lookup"><span data-stu-id="91487-155">Paraguay</span></span></p>
<p><span data-ttu-id="91487-156">Peru</span><span class="sxs-lookup"><span data-stu-id="91487-156">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="consolidating-tenants"></a><span data-ttu-id="91487-157">Konsolidieren von Mandanten</span><span class="sxs-lookup"><span data-stu-id="91487-157">Consolidating tenants</span></span>


<span data-ttu-id="91487-158">Wenn Sie Mandanten konsolidieren möchten, empfehlen wir Folgendes:</span><span class="sxs-lookup"><span data-stu-id="91487-158">If you want to consolidate tenants, we recommend the following:</span></span>

-   <span data-ttu-id="91487-159">**Mehrere Regionen/Länder, Transaktionen jedoch nur in einem Land/einer Region**.</span><span class="sxs-lookup"><span data-stu-id="91487-159">**Multiple regions/countries but only one transacting**.</span></span> <span data-ttu-id="91487-160">Wenn Sie Transaktionen nur in einem Land/einer Region durchführen, jedoch eine Reihe weiterer Mandanten eingerichtet haben, verwenden Sie den Mandanten, über den Sie Transaktionen durchführen, als neuen zentralen Mandanten für dieses Land/diese Region und stornieren die übrigen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="91487-160">If you are only transacting in one country/region, but have a number of other tenants set up, use the transacting tenant as your new centralized tenant for that region and cancel your other tenants.</span></span>

-   **<span data-ttu-id="91487-161">Mehrere Länder/Regionen, Transaktionen jedoch nur in einem Land/einer Region.</span><span class="sxs-lookup"><span data-stu-id="91487-161">Multiple countries/regions but only one Transacting.</span></span>** <span data-ttu-id="91487-162">Wenn Sie Transaktionen in einer Reihe von Ländern/Regionen durchführen, empfehlen wir eine Konsolidierung auf den Mandanten mit der größten Zahl von Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="91487-162">If you are transacting in a number of countries/regions, we recommend that you centralize to the tenant with the largest number of seats.</span></span> <span data-ttu-id="91487-163">Sie sollten die Abonnements in den Ländern/Regionen stornieren, in denen Sie kleinere Mengen an Lizenzen verwalten.</span><span class="sxs-lookup"><span data-stu-id="91487-163">You should cancel the subscriptions in the countries/regions where you have smaller amounts of seats.</span></span>


## <a name="countryregion-information"></a><span data-ttu-id="91487-164">Informationen zu Ländern/Regionen</span><span class="sxs-lookup"><span data-stu-id="91487-164">Country/region information</span></span>


<span data-ttu-id="91487-165">Berücksichtigen Sie vor der Konsolidierung von Mandanten die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="91487-165">Consider the following before beginning consolidating tenants:</span></span>

-   <span data-ttu-id="91487-166">**Wenn Ihr Microsoft-Verkaufsstandort die Vereinigten Staaten sind**, umfasst Ihr Gebiet Kunden in den Vereinigten Staaten.</span><span class="sxs-lookup"><span data-stu-id="91487-166">**If your Microsoft sell-to location is the United States**, your Territory includes customers located in the United States.</span></span>

-   <span data-ttu-id="91487-167">**Wenn Ihr Microsoft-Verkaufsstandort Kanada ist**, umfasst Ihr Gebiet Kunden in Kanada.</span><span class="sxs-lookup"><span data-stu-id="91487-167">**If your Microsoft sell-to location is Canada**, your Territory includes customers located in Canada.</span></span>

-   <span data-ttu-id="91487-168">**Wenn Ihr Microsoft-Verkaufsstandort Brasilien ist**, umfasst Ihr Gebiet Kunden in Brasilien.</span><span class="sxs-lookup"><span data-stu-id="91487-168">**If your Microsoft sell-to location is Brazil**, your Territory includes customers located in Brazil.</span></span>

-   <span data-ttu-id="91487-169">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Anguilla, Antigua und Barbuda, Antarktis, Argentinien, Aruba, Bahamas, Barbados, Belize, Bermuda, Bolivien, Bonaire, Saba, St. Eustatius, Britische Jungferninseln, Kaimaninseln, Chile, Kolumbien, Costa Rica, Curacao, Dominika, Dominikanische Republik, Ecuador, El Salvador, Falklandinseln, Französisch-Guayana, Grenada, Guadeloupe, Guatemala, Guyana, Haiti, Honduras, Jamaika, Martinique, Mexiko, Montserrat, Nicaragua, Panama, Paraguay, Peru, Puerto Rico, Saba, Saint Barthélemy, St. Kitts und Nevis, St. Lucia, St. Martin, St. Vincent und die Grenadinen, Sint Maarten, Südgeorgien und die Südlichen Sandwichinseln, Suriname, Trinidad und Tobago, Turks- und Caicosinseln, Uruguay, Venezuela, Amerikanische Jungferninseln.</span><span class="sxs-lookup"><span data-stu-id="91487-169">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Anguilla, Antigua and Barbuda, Antarctica, Argentina, Aruba, Bahamas, Barbados, Belize, Bermuda, Bolivia, Bonaire, British Virgin Islands, Cayman Islands, Chile, Colombia, Costa Rica, Curacao, Dominica, Dominican Republic, Ecuador, El Salvador, Falkland Islands, French Guiana, Grenada, Guadeloupe, Guatemala, Guyana, Haiti, Honduras, Jamaica, Martinique, Mexico, Montserrat, Nicaragua, Panama, Paraguay, Peru, Puerto Rico, Saba, Saint Barthélemy, Saint Kitts and Nevis, Saint Lucia, Saint Martin, Saint Vincent and the Grenadines, Sint Eustatius, Sint Maarten, South Georgia and South Sandwich Islands, Suriname, Trinidad and Tobago, Turks and Caicos Islands, Uruguay, Venezuela, Virgin Islands.</span></span> 

-   <span data-ttu-id="91487-170">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Ålandinseln, Andorra, Österreich, Belgien, Bouvetinsel, Bulgarien, Kroatien, Zypern, Tschechische Republik, Dänemark, Estland, Färöer, Finnland, Frankreich, Deutschland, Griechenland, Gibraltar, Guernsey, Grönland, Ungarn, Island, Irland, Isle of Man, Italien, Jersey, Jan Mayen, Lettland, Liechtenstein, Litauen, Luxemburg, Madagaskar, Malawi, Mali, Malta, Mayotte, Monaco, Niederlande, Neukaledonien, Norwegen, Polen, Portugal, Rumänien, San Marino, Slowakei, Slowenien, Spanien, Svalbard, Schweden, Schweiz, Vereinigtes Königreich, Vatikanstadt.</span><span class="sxs-lookup"><span data-stu-id="91487-170">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Åland Islands, Andorra, Austria, Belgium, Bouvet Island, Bulgaria, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Faroe Islands, Finland, France, Germany, Greece, Gibraltar, Greenland, Guernsey, Hungary, Iceland, Ireland, Isle of Man, Italy, Jersey, Jan Mayen, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Monaco, Netherlands, Norway, Poland, Portugal, Romania, San Marino, Slovakia, Slovenia, Spain, Svalbard, Sweden, Switzerland, United Kingdom, Vatican City.</span></span> 

    > [!NOTE]  
>  <span data-ttu-id="91487-171">Wenn Sie für [CSP für Microsoft-Cloud Deutschland](partner-center-for-microsoft-cloud-germany.md) registriert sind und Sie an Kunden in EU- und EFTA-Ländern/Regionen verkaufen, können Sie die Mandanten für Partner Center für Microsoft-Cloud Deutschland nicht mit Ihren anderen Mandanten konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="91487-171">If you are enrolled in [CSP for Microsoft Cloud Germany](partner-center-for-microsoft-cloud-germany.md) and you sell to customers in the EU and EFTA countries/regions, you cannot consolidate your tenant for Partner Center for Microsoft Cloud Germany with your other tenants.</span></span>  


-   <span data-ttu-id="91487-172">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Afghanistan, Albanien, Algerien, Armenien, Aserbeidschan, Bahrain, Belarus, Benin, Bosnien und Herzegowina, Britisches Territorium im Indischen Ozean, Burkina Faso, Burundi, Zentralafrikanische Republik, Chad, Komoren, Kongo, Kongo (DRK), Kongo, Djibouti, Ägypten, Äquatorialguinea, Eritrea, Französisch-Polynesien, Gabon, Gambia, Guinea, Guinea-Bissau, Georgien, Irak, Israel, Jordanien, Kasachstan, Kuwait, Kirgisistan, Libanon, Liberia, Libyen, Madagaskar, Malawi, Mali, Mayotte, Republik Moldau, Mongolei, Montenegro, Marokko, Neukaledonien, Niger, Oman, Pakistan, Palästinensische Behörde, Katar, Republik von Mazedonien (FYROM), Réunion, Saudi-Arabien, Serbien, Seychellen, Sierra Leone, Somalia, Südafrika, Tadschikistan, Togo, Tunesien, Türkei, Turkmenistan, Ukraine, Vereinigte Arabische Emirate, Usbekistan, Jemen, Simbabwe.</span><span class="sxs-lookup"><span data-stu-id="91487-172">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Afghanistan, Albania, Algeria, Armenia, Azerbaijan, Bahrain, Belarus, Benin, Bosnia and Herzegovina, Burkina Faso, Burundi, Central African Republic, Chad, Comoros, Congo (DRC), Congo, Djibouti, Egypt, Equatorial Guinea, Eritrea, French Polynesia, Gabon, Gambia, Georgia, Guinea, Guinea-Bissau, Iraq, Israel, Jordan, Kazakhstan, Kuwait, Kyrgyzstan, Lebanon, Liberia, Libya, Madagascar, Malawi, Mali, Mayotte, Moldova, Mongolia, Montenegro, Morocco, New Caledonia, Niger, Oman, Pakistan, Palestinian Authority, Qatar, Republic of Macedonia (FYROM), Réunion, Saudi Arabia, Serbia, Seychelles, Sierra Leone, Somalia, South Africa, Tajikistan, Togo, Tunisia, Turkey, Turkmenistan, Ukraine, United Arab Emirates, Uzbekistan, Yemen, Zimbabwe.</span></span> 

-   <span data-ttu-id="91487-173">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Angola, Botsuana, Britisches Territorium im Indischen Ozean, Cabo Verde, Kamerun, Elfenbeinküste, Ghana, Kamerun, Kenia, Kosovo, Lesotho, Mauritius, Mosambik, Namibia, Nigeria, Ruanda, Sambia, Senegal, Swasiland, Tansania, Uganda, Yemen, Sambia.</span><span class="sxs-lookup"><span data-stu-id="91487-173">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Angola, Botswana, British Indian Ocean Territory, Cabo Verde, Cameroon, Côte d'Ivoire, Ethiopia, Ghana, Kenya, Kosovo, Lesotho, Mauritania, Mauritius, Mozambique, Namibia, Nigeria, Rwanda, Senegal, Swaziland, Tanzania, Uganda, Yemen, Zambia.</span></span> 

-   <span data-ttu-id="91487-174">**Wenn Ihr Microsoft-Verkaufsstandort Russland ist**, umfasst Ihr Gebiet Kunden in Russland.</span><span class="sxs-lookup"><span data-stu-id="91487-174">**If your Microsoft sell-to location is Russia**, your Territory includes customers located in Russia.</span></span>

-   <span data-ttu-id="91487-175">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Amerikanisch-Samoa, Bangladesch, Bhutan, Brunei Darussalam, Kambodscha, Hongkong (SAR), Indonesien, Laos, Macau SAR, Malaysia, Malediven, Marshallinseln, Myanmar, Nepal, Papua-Neuguinea, Philippinen, Saint Pierre und Miquelon, Singapur, Sri Lanka, Thailand, Timor-Leste, Tonga, Vanuatu, Vietnam.</span><span class="sxs-lookup"><span data-stu-id="91487-175">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: American Samoa, Bangladesh, Bhutan, Brunei, Darussalam, Cambodia, Hong Kong SAR, Indonesia, Laos, Macao SAR, Malaysia, Maldives, Myanmar, Nepal, Philippines, Saint Pierre and Miquelon, Samoa, Singapore, Sri Lanka, Thailand, Timor-Leste, Vanuatu, Vietnam.</span></span> 

-   <span data-ttu-id="91487-176">**Wenn Ihr Microsoft-Verkaufsstandort ein Land/Region in der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen in der folgenden Liste: Australien, Fidschi, Weihnachtsinsel, Kokosinseln, Cookinseln, Guam, Heard und McDonaldinseln, Kiribati, Marshallinseln, Mikronesien, Nauru, Niue, Norfolkinsel, Nördliche Marianen, Palau, Papua-Neuguinea, Pitcairninseln, Salomonen, Tokelau, Tonga, Tuvalu, Wallis und Futuna.</span><span class="sxs-lookup"><span data-stu-id="91487-176">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Australia, Fiji, Christmas Island, Cocos (Keeling) Islands, Cook Islands, Guam, Heard Island and McDonald Islands, Kiribati, Marshall Islands, Micronesia, Nauru, Niue, Norfolk Island, Northern Mariana Islands, Palau, Papa New Guinea, Pitcairn Islands, Solomon Islands, Tokelau, Tonga, Tuvalu, Wallis and Futuna.</span></span> 

-   <span data-ttu-id="91487-177">**Wenn Ihr Microsoft-Verkaufsstandort Neuseeland ist**, umfasst Ihr Gebiet Kunden in Neuseeland.</span><span class="sxs-lookup"><span data-stu-id="91487-177">**If your Microsoft sell-to location is New Zealand**, your Territory includes customers located in New Zealand.</span></span>

-   <span data-ttu-id="91487-178">**Wenn Ihr Microsoft-Verkaufsstandort Indien ist**, umfasst Ihr Gebiet Kunden in Indien.</span><span class="sxs-lookup"><span data-stu-id="91487-178">**If your Microsoft sell-to location is India**, your Territory includes customers located in India.</span></span>

-   <span data-ttu-id="91487-179">**Wenn Ihr Microsoft-Verkaufsstandort Japan ist**, umfasst Ihr Gebiet Kunden in Japan.</span><span class="sxs-lookup"><span data-stu-id="91487-179">**If your Microsoft sell-to location is Japan**, your Territory includes customers located in Japan.</span></span>

-   <span data-ttu-id="91487-180">**Wenn Ihr Microsoft-Verkaufsstandort Korea ist**, umfasst Ihr Gebiet Kunden in Korea.</span><span class="sxs-lookup"><span data-stu-id="91487-180">**If your Microsoft sell-to location is Korea**, your Territory includes customers located in Korea.</span></span>

-   <span data-ttu-id="91487-181">**Wenn Ihr Microsoft-Verkaufsstandort Taiwan ist**, umfasst Ihr Gebiet Kunden in Taiwan.</span><span class="sxs-lookup"><span data-stu-id="91487-181">**If your Microsoft sell-to location is Taiwan**, your Territory includes customers located in Taiwan.</span></span>

## <a name="billing-currencies-by-country"></a><span data-ttu-id="91487-182">Abrechnungswährungen nach Land</span><span class="sxs-lookup"><span data-stu-id="91487-182">Billing currencies by country</span></span>

<span data-ttu-id="91487-183">Ihr geografischer Standort bestimmt die Währung, in der Ihre Rechnungen gestellt werden, wie in der folgenden Tabelle gezeigt.</span><span class="sxs-lookup"><span data-stu-id="91487-183">Your geographic location determines the currency in which you are billed, as shown in the following table.</span></span> <span data-ttu-id="91487-184">Hinweis: Wenn Sie eine andere Abrechnungswährung verwenden möchten, müssen Sie aufgrund von steuerlichen und rechtlichen Auswirkungen einen neuen Mandanten erstellen und diese Währung angeben.</span><span class="sxs-lookup"><span data-stu-id="91487-184">Note that due to tax and legal implications, if you want to use a different billing currency, you'll need to create a new tenant and specify that currency.</span></span> 

| <span data-ttu-id="91487-185">Währung</span><span class="sxs-lookup"><span data-stu-id="91487-185">Currency</span></span> | <span data-ttu-id="91487-186">Land</span><span class="sxs-lookup"><span data-stu-id="91487-186">Country</span></span> |
| ---- | ---- |
| <span data-ttu-id="91487-187">USD</span><span class="sxs-lookup"><span data-stu-id="91487-187">USD</span></span> | <span data-ttu-id="91487-188">Albanien und St. Eustatius, Anguilla, Antarktis, Antigua und Barbuda, Argentinien, Armenien, Aruba, Aserbeidschan, Bahamas, Bahrain, Bangladesch, Barbados, Belarus, Belize, Benin, Bermuda, Bolivien, Bonaire, Brasilien, Britisches Territorium im Indischen Ozean, Brunei Darussalam, Burundi, Kamerun, Kaimaninseln, Zentralafrikanische Republik, Chile, Kolumbien, Komoren, Costa Rica, Curaçao, Dominikanische Republik, Ecuador, Ägypten, El Salvador, Äquatorialguinea, Fidschi, Französisch-Guayana, Französisch-Polynesien, Georgien, Ghana, Guatemala, Guinea-Bissau, Honduras, Hongkong (SAR), Indonesien, Irak, Israel, Jamaika, Kasachstan, Kenia, Kuwait, Kirgisistan, Libanon, Lesotho, Macau SAR, Madagaskar, Malawi, Malaysia, Mali, Mauretanien, Mauritius, Mayotte, Mexiko, Marokko, Namibia, Neukaledonien, Nicaragua, Nigeria, Oman, Pakistan, Panama, Paraguay, Peru, Philippinen, Puerto Rico, Katar, Réunion, Ruanda, Saba, St. Lucia, St. Martin, St. Vincent und die Grenadinen, Saudi-Arabien, Serbien, Seychellen, Sierra Leone, Singapur, St. Maarten, Somalia, Südafrika, Südsudan, Sri Lanka, Suriname, Swasiland, Tansania, Thailand, Timor-Leste, Togo, Trinidad und Tobago, Tunesien, Türkei, Turks- und Caicosinseln, Amerikanische Jungferninseln, Ukraine, Vereinigte Arabische Emirate, Vereinigte Staaten, Uruguay, Venezuela, Vietnam, Yemen.</span><span class="sxs-lookup"><span data-stu-id="91487-188">Albania and Sint Eustatius, Anguilla, Antarctica, Antigua and Barbuda, Argentina, Armenia, Aruba, Azerbaijan, Bahamas, Bahrain, Bangladesh, Barbados, Belarus, Belize, Benin, Bermuda, Bolivia, Bonaire, Brazil, British Indian Ocean Territory, Brunei, Burundi, Cameroon, Cayman Islands, Central African Republic, Chile, Colombia, Comoros, Costa Rica, Curaçao, Dominican Republic, Ecuador, Egypt, El Salvador, Equatorial Guinea, Eritrea, French Guiana, French Polynesia, Georgia, Ghana, Guatemala, Guinea-Bissau, Honduras, Hong Kong SAR, Indonesia, Iraq, Israel, Jamaica, Kazakhstan, Kenya, Kuwait, Kyrgyzstan, Lebanon, Lesotho, Macao SAR, Madagascar, Malawi, Malaysia, Mali, Mauritania, Mauritius, Mayotte, Mexico, Morocco, Namibia, New Caledonia, Nicaragua, Nigeria, Oman, Pakistan, Panama, Paraguay, Peru, Philippines, Puerto Rico, Qatar, Reunion, Rwanda, Saba, Saint Lucia, Saint Martin, Saint Vincent and the Grenadines, Saudi Arabia, Serbia, Seychelles, Sierra Leone, Singapore, Sint Maarten, Somalia, South Africa, South Sudan, Sri Lanka, Suriname, Swaziland, Tanzania, Thailand, Timor-Leste, Togo, Trinidad and Tobago, Tunisia, Turkey, Turks and Caicos Islands, U.S. Virgin Islands, Ukraine, United Arab Emirates, United States, Uruguay, Venezuela, Vietnam, Yemen.</span></span>| 
| <span data-ttu-id="91487-189">TWD</span><span class="sxs-lookup"><span data-stu-id="91487-189">TWD</span></span> | <span data-ttu-id="91487-190">Taiwan</span><span class="sxs-lookup"><span data-stu-id="91487-190">Taiwan</span></span> |
| <span data-ttu-id="91487-191">SEK</span><span class="sxs-lookup"><span data-stu-id="91487-191">SEK</span></span> | <span data-ttu-id="91487-192">Schweden</span><span class="sxs-lookup"><span data-stu-id="91487-192">Sweden</span></span> |
| <span data-ttu-id="91487-193">INR</span><span class="sxs-lookup"><span data-stu-id="91487-193">INR</span></span> | <span data-ttu-id="91487-194">Indien</span><span class="sxs-lookup"><span data-stu-id="91487-194">India</span></span> |
| <span data-ttu-id="91487-195">RUB</span><span class="sxs-lookup"><span data-stu-id="91487-195">RUB</span></span> | <span data-ttu-id="91487-196">Russland</span><span class="sxs-lookup"><span data-stu-id="91487-196">Russia</span></span> |
| <span data-ttu-id="91487-197">NZD</span><span class="sxs-lookup"><span data-stu-id="91487-197">NZD</span></span> | <span data-ttu-id="91487-198">Neuseeland, Vanuatu</span><span class="sxs-lookup"><span data-stu-id="91487-198">New Zealand, Vanuatu</span></span> |
| <span data-ttu-id="91487-199">NOK</span><span class="sxs-lookup"><span data-stu-id="91487-199">NOK</span></span> | <span data-ttu-id="91487-200">Jan Mayen, Norwegen, Svalbard</span><span class="sxs-lookup"><span data-stu-id="91487-200">Jan Mayen, Norway, Svalbard</span></span> |
| <span data-ttu-id="91487-201">KRW</span><span class="sxs-lookup"><span data-stu-id="91487-201">KRW</span></span> | <span data-ttu-id="91487-202">Südkorea</span><span class="sxs-lookup"><span data-stu-id="91487-202">Korea</span></span> |
| <span data-ttu-id="91487-203">JPY</span><span class="sxs-lookup"><span data-stu-id="91487-203">JPY</span></span> | <span data-ttu-id="91487-204">Japan</span><span class="sxs-lookup"><span data-stu-id="91487-204">Japan</span></span> |
| <span data-ttu-id="91487-205">GBP</span><span class="sxs-lookup"><span data-stu-id="91487-205">GBP</span></span> | <span data-ttu-id="91487-206">Isle Of Man, Jersey, Vereinigtes Königreich</span><span class="sxs-lookup"><span data-stu-id="91487-206">Isle of Man, Jersey, United Kingdom</span></span> |
| <span data-ttu-id="91487-207">EUR</span><span class="sxs-lookup"><span data-stu-id="91487-207">EUR</span></span> | <span data-ttu-id="91487-208">Andorra, Österreich, Belgien, Bouvetinsel, Kroatien, Tschechische Republik, Estland, Färöer, Finnland, Frankreich, Deutschland, Griechenland, Ungarn, Island, Irland, Italien, Lettland, Liechtenstein, Litauen, Luxemburg/Belgien, Niederlande, Polen, Portugal, Rumänien, San Marino, Slowakei, Slowenien, Spanien</span><span class="sxs-lookup"><span data-stu-id="91487-208">Andorra, Austria, Belgium, Bouvet Island, Croatia, Czech Republic, Estonia, Faroe Islands, Finland, France, Germany, Greece, Hungary, Iceland, Ireland, Italy, Latvia, Liechtenstein, Lithuania, Luxembourg/Belgium, Netherlands, Poland, Portugal, Romania, San Marino, Slovakia, Slovenia, Spain</span></span> |
| <span data-ttu-id="91487-209">DKK</span><span class="sxs-lookup"><span data-stu-id="91487-209">DKK</span></span> | <span data-ttu-id="91487-210">Dänemark</span><span class="sxs-lookup"><span data-stu-id="91487-210">Denmark</span></span> |
| <span data-ttu-id="91487-211">CHF</span><span class="sxs-lookup"><span data-stu-id="91487-211">CHF</span></span> | <span data-ttu-id="91487-212">Schweiz</span><span class="sxs-lookup"><span data-stu-id="91487-212">Switzerland</span></span> |
| <span data-ttu-id="91487-213">CAD</span><span class="sxs-lookup"><span data-stu-id="91487-213">CAD</span></span> | <span data-ttu-id="91487-214">Kanada</span><span class="sxs-lookup"><span data-stu-id="91487-214">Canada</span></span> |
| <span data-ttu-id="91487-215">AUD</span><span class="sxs-lookup"><span data-stu-id="91487-215">AUD</span></span> | <span data-ttu-id="91487-216">Australien, Weihnachtsinsel, Kokosinseln, Cookinseln, Fidschi, Heard und McDonaldinseln, Kiribati, Marshallinseln, Nauru, Niue, Norfolkinsel, Nördliche Marianen, Palau, Papua-Neuguinea, Pitcairninseln, Salomonen, Tokelau, Tonga, Tuvalu, Wallis und Futuna.</span><span class="sxs-lookup"><span data-stu-id="91487-216">Australia, Christmas Island, Cocos (Keeling) Islands, Cook Islands, Fiji, Heard Island and McDonald Islands, Kiribati, Marshall Islands, Nauru, Niue, Norfolk Island, Northern Mariana Islands, Palau, Papua New Guinea, Pitcairn Islands, Solomon Islands, Tokelau, Tonga, Tuvalu, Wallis and Futuna.</span></span> |


 



