---
title: Allgemeine Abrechnungsszenarien | Partner Center
description: "In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Arbeitsplätze für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 5ac69f33ca78be1eca2af439a48d6d0904a4cfc5
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="common-billing-scenarios"></a>Allgemeine Abrechnungsszenarien

**Betrifft**

-  Partner Center
-  Partner Center für Microsoft-Cloud Deutschland

In diesem Thema wird erläutert, was auf Ihrer Rechnung nach dem Hinzufügen neuer Abonnements, dem Anpassen der Arbeitsplätze für ein Abonnement oder dem Kündigen eines Abonnements angezeigt werden sollte. Die Auswirkungen fallen für nutzungsbasierte und lizenzbasierte Abonnements unterschiedlich aus.

## <a name="in-this-section"></a>Inhalt dieses Abschnitts


-   [Nutzungsbasierte Abrechnung](#usagebased)

-   [Lizenzbasierte Abrechnung](#licensebased)

## <a href="" id="usagebased"></a>Nutzungsbasierte Abrechnung


Es werden Ihnen nur Dienste berechnet, die im vorherigen Abrechnungszeitraums genutzt wurden. Alle Azure-Dienste oder -Anwendungen, die während des Abrechnungszeitraums aktiviert und genutzt werden, erscheinen in der nächsten Rechnung.

-   Die erste Rechnung enthält den Anfangszeitraum vom Abonnementstartdatum bis zum ersten Abrechnungsdatum.
-   Getaktete Dienstleistungspreise können sich innerhalb des Abrechnungszyklus ändern.
    -   Preiserhöhungen werden 30 Tage zuvor bekanntgegeben.
    -   Preissenkungen werden am Tag der Änderung angezeigt.
    -   Vorhandene Abonnements verwenden den zum Anfang des Abrechnungszyklus gültigen Preis.
    -   Neue Abonnements (im Abrechnungszyklus erstellt) verwenden den zum Erstellungsdatum gültigen Preis.
-   Wenn Sie ein Abonnement vor der ersten Abrechnung oder während eines Rechnungszyklus kündigen, erscheinen die Nutzungsgebühren in der Abstimmungsdatei für den Zeitraum, in dem das Abonnement aktiv war.

## <a href="" id="licensebased"></a>Lizenzbasierte Abrechnung


Für Monate ohne Änderungen an lizenzbasierten Abonnements sehen Sie einen einzelnen Eintrag für jedes Abonnement in der Abstimmungsdatei und in der Rechnung – die Vorausgebühren für den nächsten Monat.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Szenario</td>
<td>Beschreibung</td>
<td>Beispiel</td>
</tr>
<tr class="even">
<td>Neues Abonnement</td>
<td><p>Der Zeitraum zwischen dem Startdatum des Abonnements und dem ersten Abrechnungsdatum ist KOSTENLOS.</p>
<p>Ihre Erstattungsdatei enthält einen einzelnen Posten:</p>
<ul>
<li>Im Voraus anfallende Gebühr für den nächsten Monat</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Neues Abonnement: vor dem ersten Abrechnungstermin gekündigt</td>
<td>Das Konto wird nicht mit Gebühren belastet. Das Abonnement wird nicht in der Erstattungsdatei aufgeführt. Dies ist hilfreich, wenn Sie Tests ohne zusätzliche Abonnementgebühren ausführen möchten.</td>
<td></td>
</tr>
<tr class="even">
<td>Neues Abonnement: mit Anpassungen der Lizenzmenge während der kostenlosen Testphase</td>
<td><p>Die Erstattungsdatei enthält mehrere Positionen:</p>
<ul>
<li>Änderungen der Lizenzmenge zum Einheitenpreis von 0 US-Dollar. (Während der kostenlosen Testphase fallen keine Kosten für Arbeitsplatzänderungen an.)</li>
<li>Die im Voraus anfallende Gebühr für den nächsten Monat spiegelt die neue Menge wider.</li>
</ul></td>
<td>Anteilige Nutzung:
<ul>
<li>3. Juni bis 7. Juni für 10 Arbeitsplätze = KEINE Gebühr</li>
<li>8. Juni bis 11. Juni für 20 Arbeitsplätze = KEINE Gebühr</li>
<li>12. Juni bis 14. Juni für 15 Arbeitsplätze = KEINE Gebühr</li>
</ul>
<p>Abrechnungstermin: im Voraus anfallende Gebühr für den ganzen Monatszeitraum vom 15. Juni bis 14. Juli für 15 Arbeitsplätze. Wenn die Gebühren pro Abonnement und Monat beispielsweise 10 US-Dollar betragen, ist die Gebühr 10 US-Dollar x 15 Arbeitsplätze = 150 US-Dollar.</p></td>
</tr>
<tr class="odd">
<td>Bestehendes Abonnement: Erhöhung oder Verringerung der Lizenzmenge</td>
<td><p>Die Erstattungsdatei enthält mehrere Positionen:</p>
<ul>
<li>Erstattung der im Voraus anfallenden Gebühren</li>
<li>Gebühren für die anteilige Nutzung</li>
<li>Im Voraus anfallende Gebühr für den nächsten Monat</li>
</ul></td>
<td><p>Anteilige Nutzung:</p>
<ul>
<li>15. Juli bis 19. Juli für 15 Arbeitsplätze = 26,61 US-Dollar</li>
<li>20. Juli bis 30. Juli für 12 Arbeitsplätze = 46,84 US-Dollar</li>
<li>31. Juli bis 9. August für 18 Arbeitsplätze = 63,87 US-Dollar</li>
<li>10. August bis 14. August für 10 Arbeitsplätze = 17,74 US-Dollar</li>
</ul>
Rückerstattung der im Voraus anfallenden Gebühren für den gesamten Monatszeitraum vom 15. Juli bis 14. August = -165 US-Dollar.
<p>Abrechnungstermin: im Voraus anfallende Gebühr für den ganzen Monatszeitraum vom 15. August bis 14. September für 10 Arbeitsplätze = 110 US-Dollar.</p></td>
</tr>
<tr class="even">
<td>Kündigung: keine vorherigen Arbeitsplatzänderungen</td>
<td><p>Ihre Erstattungsdatei enthält einen einzelnen Posten:</p>
<ul>
<li>Erstattung für nicht genutzte Tage, da der gesamte Zeitraum in der vorherigen Abrechnung im Voraus in Rechnung gestellt wurde. Dieser Betrag wird basierend auf dem Abonnementenddatum berechnet.</li>
</ul></td>
<td>Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.
<p>Verbrauchter Teil der im Voraus anfallenden Gebühr vom 15. August bis 24. August.</p>
<p>Erstattung für nicht genutzte Tage: 25. August bis 14. September für 10 Arbeitsplätze = -74,51 US-Dollar.</p></td>
</tr>
<tr class="odd">
<td>Kündigung: mit vorherigen Arbeitsplatzänderungen</td>
<td><p>Die Erstattungsdatei enthält mehrere Positionen:</p>
<ul>
<li>Erstattung der im Voraus anfallenden Gebühren</li>
<li>Gebühren für die anteilige Nutzung</li>
<li>Erstattung für alle nicht genutzten Tage</li>
</ul></td>
<td>Zuvor in Rechnung gestellte im Voraus anfallende Gebühren: 15. August bis 14. September für 10 Arbeitsplätze = 100 US-Dollar.
<p>Anteilige Nutzung:</p>
<ul>
<li>15. August bis 24. August für 10 Arbeitsplätze</li>
<li>25. August bis 14. September für 5 Arbeitsplätze</li>
</ul>
<p>Erstattung für nicht genutzte Tage: 1. September bis 14. September für 5 Arbeitsplätze.</p>
<p>Rückerstattung der im Voraus anfallenden Gebühren für den gesamten Monatszeitraum vom 15. August bis 14. September = -100 US-Dollar.</p></td>
</tr>
</tbody>
</table>

 

 

 



