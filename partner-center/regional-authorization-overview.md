---
title: Regionale CSP-Autorisierung | Partner Center
description: "Mithilfe der regionalen Autorisierung können international tätige Partner jetzt Kunden in verschiedenen Regionen und Ländern auf der ganzen Welt einfacher verwalten."
ms.assetid: 22F9495E-E31A-41AE-BF51-3478AB2C8E78
author: MaggiePucciEvans
ms.openlocfilehash: f79c2f0a56f88faf554543fa2bb0a0ab504e0614
ms.sourcegitcommit: a905afc18ffc20e3469933fa005336f1e9b520f4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2017
---
# <a name="csp-regional-authorization"></a>Regionale CSP-Autorisierung


\[Einige Informationen beziehen sich auf die Vorabversion, die vor der kommerziellen Freigabe möglicherweise wesentlichen Änderungen unterliegt. Microsoft übernimmt für die hier bereitgestellten Informationen keine Garantien, weder ausdrücklicher noch impliziter Art.\]

Mithilfe der regionalen Autorisierung können international tätige Partner jetzt Kunden in verschiedenen Regionen und Ländern auf der ganzen Welt einfacher verwalten. Dies reduziert die Anzahl von Mandanten, die von Partnern verwaltet werden müssen, sowie die Abrechnungsdaten, die von Partnern verarbeitet werden müssen. Darüber hinaus erhalten Partner eine stärker konsolidierte Sicht auf ihre Verkäufe.

In der Vergangenheit mussten Partner in jedem Land physisch präsent sein, in dem sie Transaktionen durchführen wollten, mit Ausnahme der Europäischen Union/EFTA. Das bedeutete, dass Partner mehrere Mandanten mit unterschiedlichen Abrechnungsdaten und weiteren unterschiedlichen Einstellungen in Partner Center einrichten mussten. In Regionen wie Lateinamerika konnten Partner nicht problemlos mit Kunden aus einer benachbarten Region oder einem benachbarten Land arbeiten. In einigen Fällen war dies völlig unmöglich.

>**Hinweis**<br> Wenn Sie für [CSP für Microsoft-Cloud Deutschland](partner-center-for-microsoft-cloud-germany.md) registriert sind und Sie an Kunden in EU- und EFTA-Ländern/Regionen verkaufen, können Sie die Mandanten für Partner Center für Microsoft-Cloud Deutschland nicht mit Ihren anderen Mandanten konsolidieren.  

## <a name="planning"></a>Planen

Partner haben mehrere Optionen für die Konsolidierung ihrer regionalen Mandanten. Diese werden im Folgenden beschrieben.

### <a name="separate-tenants-for-single-regions-or-countries"></a>Getrennte Mandanten für die einzelnen Regionen oder Länder

Die Mandantenkonsolidierung ist optional. Partner können internationale Kunden weiterhin über getrennte Mandanten verwalten, wie in der folgenden Tabelle gezeigt.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Partnerstandort(e)</th>
<th>Abrechnungsdatum/-daten</th>
<th>Kundenstandort(e)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Kolumbien</p></td>
<td><p>Abrechnungsdatum: 10. des Monats</p></td>
<td><p>Kolumbien</p></td>
</tr>
<tr class="even">
<td><p>Chile</p></td>
<td><p>Abrechnungsdatum: 15. des Monats</p></td>
<td><p>Chile</p></td>
</tr>
<tr class="odd">
<td><p>Paraguay</p></td>
<td><p>Abrechnungsdatum: 5. des Monats</p></td>
<td><p>Paraguay</p></td>
</tr>
<tr class="even">
<td><p>Peru</p></td>
<td><p>Abrechnungsdatum: 2. des Monats</p></td>
<td><p>Peru</p></td>
</tr>
</tbody>
</table>

 

## <a name="one-tenant-for-multiple-regions-or-countries"></a>Ein einziger Mandant für mehrere Regionen oder Länder


Partner können ihre Vorgänge aus mehreren CSP-Mandanten auf einen einzigen CSP-Mandanten konsolidieren.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Partnerstandort</th>
<th>Abrechnungsdatum</th>
<th>Kundenstandort(e)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Kolumbien</p></td>
<td><p>Abrechnungsdatum: 10. des Monats</p></td>
<td><p>Kolumbien</p>
<p>Chile</p>
<p>Paraguay</p>
<p>Peru</p></td>
</tr>
</tbody>
</table>

 

## <a name="some-tenants-for-some-regions-or-countries"></a>Einige Mandanten für einige Regionen oder Länder


Partner können ihre Vorgänge aus mehreren CSP-Mandanten auf eine kleinere Zahl von CSP-Mandanten konsolidieren.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Partnerstandort(e)</th>
<th>Abrechnungsdatum/-daten</th>
<th>Kundenstandort(e)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Kolumbien</p></td>
<td><p>Abrechnungsdatum: 10. des Monats</p></td>
<td><p>Kolumbien</p>
<p>Chile</p></td>
</tr>
<tr class="even">
<td><p>Paraguay</p></td>
<td><p>Abrechnungsdatum: 5. des Monats</p></td>
<td><p>Paraguay</p>
<p>Peru</p></td>
</tr>
</tbody>
</table>

 

## <a name="consolidating-tenants"></a>Konsolidieren von Mandanten


Wenn Sie Mandanten konsolidieren möchten, empfehlen wir Folgendes:

-   **Mehrere Regionen/Länder, Transaktionen jedoch nur in einem Land/einer Region**. Wenn Sie Transaktionen nur in einem Land/einer Region durchführen, jedoch eine Reihe weiterer Mandanten eingerichtet haben, verwenden Sie den Mandanten, über den Sie Transaktionen durchführen, als neuen zentralen Mandanten für dieses Land/diese Region und stornieren die übrigen Mandanten.

-   **Mehrere Länder/Regionen, Transaktionen jedoch nur in einem Land/einer Region.** Wenn Sie Transaktionen in einer Reihe von Ländern/Regionen durchführen, empfehlen wir eine Konsolidierung auf den Mandanten mit der größten Zahl von Lizenzen. Sie sollten die Abonnements in den Ländern/Regionen stornieren, in denen Sie kleinere Mengen an Lizenzen verwalten.


## <a name="countryregion-information"></a>Informationen zu Ländern/Regionen


Berücksichtigen Sie vor der Konsolidierung von Mandanten die folgenden Punkte:

-   **Wenn Ihr Microsoft-Verkaufsstandort die Vereinigten Staaten sind**, umfasst Ihr Gebiet Kunden in den Vereinigten Staaten.

-   **Wenn Ihr Microsoft-Verkaufsstandort Kanada ist**, umfasst Ihr Gebiet Kunden in Kanada.

-   **Wenn Ihr Microsoft-Verkaufsstandort Brasilien ist**, umfasst Ihr Gebiet Kunden in Brasilien.

-   **Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Anguilla, Antigua und Barbuda, Argentinien, Aruba, Bahamas, Barbados, Belize, Bermuda, Bolivien, Bonaire, Kaimaninseln, Chile, Kolumbien, Costa Rica, Curacao, Dominikanische Republik, Ecuador, El Salvador, Französisch-Guayana, Guadeloupe, Guatemala, Honduras, Jamaika, Martinique, Mexiko, Nicaragua, Panama, Paraguay, Peru, Puerto Rico, St. Kitts und Nevis, St. Lucia, St. Martin, St. Vincent und die Grenadinen, Sint Maarten, Suriname, Trinidad und Tobago, Turks- und Caicosinseln, Uruguay, Venezuela, Amerikanische Jungferninseln.

-   **Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Andorra, Österreich, Belgien, Bulgarien, Kroatien, Zypern, Tschechische Republik, Dänemark, Estland, Färöer, Finnland, Frankreich, Deutschland, Griechenland, Grönland, Ungarn, Island, Irland, Isle of Man, Italien, Jersey, Lettland, Liechtenstein, Litauen, Luxemburg, Madagaskar, Malawi, Mali, Malta, Mayotte, Monaco, Niederlande, Neukaledonien, Norwegen, Polen, Portugal, Rumänien, San Marino, Slowakei, Slowenien, Spanien, Schweden, Schweiz, Vereinigtes Königreich, Vatikanstadt.

    >**Hinweis**<br> Wenn Sie für [CSP für Microsoft-Cloud Deutschland](partner-center-for-microsoft-cloud-germany.md) registriert sind und Sie an Kunden in EU- und EFTA-Ländern/Regionen verkaufen, können Sie die Mandanten für Partner Center für Microsoft-Cloud Deutschland nicht mit Ihren anderen Mandanten konsolidieren.  


-   **Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Afghanistan, Albanien, Algerien, Armenien, Aserbeidschan, Bahrain, Belarus, Benin, Bosnien und Herzegowina, Burundi, Komoren, Ägypten, Französisch-Polynesien, Georgien, Irak, Israel, Jordanien, Kasachstan, Kuwait, Kirgisistan, Libanon, Libyen, Republik Mazedonien (Ehemalige jugoslawische Republik Mazedonien), Republik Moldau, Mongolei, Montenegro, Marokko, Mosambik, Oman, Pakistan, Palästinensische Behörde, Katar, Réunion, Saudi-Arabien, Serbien, Seychellen, Südafrika, Tadschikistan, Togo, Tunesien, Türkei, Turkmenistan, Ukraine, Vereinigte Arabische Emirate, Usbekistan, Jemen, Simbabwe.

-   **Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Äthiopien, Angola, Botsuana, Cabo Verde, Elfenbeinküste, Ghana, Kamerun, Kenia, Mauritius, Namibia, Nigeria, Ruanda, Sambia, Senegal, Tansania, Uganda.

-   **Wenn Ihr Microsoft-Verkaufsstandort Russland ist**, umfasst Ihr Gebiet Kunden in Russland.

-   **Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Bangladesch, Bhutan, Brunei Darussalam, Kambodscha, Hongkong (SAR), Indonesien, Laos, Macau SAR, Malaysia, Malediven, Marshallinseln, Myanmar, Nepal, Papua-Neuguinea, Philippinen, Singapur, Sri Lanka, Thailand, Timor-Leste, Tonga, Vietnam.

-   **Wenn Ihr Microsoft-Verkaufsstandort ein Land/eine Region aus der folgenden Liste ist**, umfasst Ihr Gebiet Kunden in den Ländern/Regionen aus der folgenden Liste: Australien oder Fidschi.

-   **Wenn Ihr Microsoft-Verkaufsstandort Neuseeland ist**, umfasst Ihr Gebiet Kunden in Neuseeland.

-   **Wenn Ihr Microsoft-Verkaufsstandort Indien ist**, umfasst Ihr Gebiet Kunden in Indien.

-   **Wenn Ihr Microsoft-Verkaufsstandort Japan ist**, umfasst Ihr Gebiet Kunden in Japan.

-   **Wenn Ihr Microsoft-Verkaufsstandort Korea ist**, umfasst Ihr Gebiet Kunden in Korea.

-   **Wenn Ihr Microsoft-Verkaufsstandort Taiwan ist**, umfasst Ihr Gebiet Kunden in Taiwan.

## <a name="billing-currencies-by-country"></a>Abrechnungswährungen nach Land

Ihr geografischer Standort bestimmt die Währung, in der Ihre Rechnungen gestellt werden, wie in der folgenden Tabelle gezeigt. Hinweis: Wenn Sie eine andere Abrechnungswährung verwenden möchten, müssen Sie aufgrund von steuerlichen und rechtlichen Auswirkungen einen neuen Mandanten erstellen und diese Währung angeben. 

| Währung | Land |
| ---- | ---- |
| USD | Albanien, Anguilla, Antigua und Barbuda, Argentinien, Armenien, Aruba, Aserbeidschan, Bahamas, Bahrain, Bangladesch, Barbados, Belarus, Belize, Benin, Bermuda, Bolivien, Bonaire, Brasilien, Brunei Darussalam, Burundi, Kamerun, Kaimaninseln, Chile, Kolumbien, Komoren, Costa Rica, Curaçao, Dominikanische Republik, Ecuador, Ägypten, El Salvador, Fidschi, Französisch-Guayana, Französisch-Polynesien, Georgien, Ghana, Guatemala, Honduras, Hongkong (SAR), Indonesien, Irak, Israel, Jamaika, Kasachstan, Kenia, Kuwait, Kirgisistan, Libanon, Macau SAR, Madagaskar, Malawi, Malaysia, Mali, Mauritius, Mayotte, Mexiko, Marokko, Namibia, Neukaledonien, Nicaragua, Nigeria, Oman, Pakistan, Panama, Paraguay, Peru, Philippinen, Puerto Rico, Katar, Réunion, Ruanda, St. Lucia, St. Martin, St. Vincent und die Grenadinen, Saudi-Arabien, Serbien, Seychellen, Singapur, Sint Maarten, Südafrika, Sri Lanka, Suriname, Tansania, Thailand, Timor-Leste, Togo, Trinidad und Tobago, Tunesien, Türkei, Turks- und Caicosinseln, Amerikanische Jungferninseln, Ukraine, Vereinigte Arabische Emirate, Vereinigte Staaten, Uruguay, Venezuela, Vietnam  | 
| TWD | Taiwan |
| SEK | Schweden |
| INR | Indien |
| RUB | Russland |
| NZD | Neuseeland |
| NOK | Norwegen |
| KRW | Südkorea |
| JPY | Japan |
| GBP | Isle Of Man, Jersey, Vereinigtes Königreich |
| EUR | Andorra, Österreich, Belgien, Kroatien, Tschechische Republik, Estland, Färöer, Finnland, Frankreich, Deutschland, Griechenland, Ungarn, Island, Irland, Italien, Lettland, Liechtenstein, Litauen, Luxemburg/Belgien, Niederlande, Polen, Portugal, Rumänien, San Marino, Slowakei, Slowenien, Spanien |
| DKK | Dänemark |
| CHF | Schweiz |
| CAD | Kanada |
| AUD | Australien, Marshallinseln, Papua-Neuguinea, Tonga |


 



