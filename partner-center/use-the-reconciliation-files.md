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
# <a name="use-the-reconciliation-files"></a>Verwenden der Abstimmungsdateien

**Betrifft**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government


Für eine detaillierte rechnungspositionsinformationen anzuzeigen Abrechnungszyklus wird herunterladen Sie die abstimmungsdateien aus dem Partner Center. Zu diesen Informationen zählen Gebühren für die einzelnen Abonnements von Kunden und ausführliche Ereignisinformationen (wie z.B. das Hinzufügen von Arbeitsplätzen zu einem Abonnement mitten in einem Abrechnungszeitraum).

## <a href="" id="itemizebypartner"></a>Aufschlüsseln nach Partner


Partner im indirekten Modell können diese zusätzlichen Felder in den beiden lizenzbasierten und nutzungsbasierten Abstimmungsdateien verwenden, um nach Handelspartnern aufzuschlüsseln.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>MPN-ID</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>MPN-ID</td>
<td><p>Die Microsoft Partner Network (MPN)-ID des CSP-Partners (direkt oder indirekt).</p></td>
</tr>
<tr class="even">
<td>MPN-ID der Handelspartner</td>
<td><p>Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt.</p>
<p>Die MPN-ID des registrierten Handelspartners für das Abonnement. Dies entspricht der Handelspartner-ID, die für das spezifische Abonnement im Partner Center aufgeführt ist.</p>
<p>Wählen Sie zum Anzeigen oder Aktualisieren des Handelspartners im Partner Center-Menü, wählen Sie <strong>Kunden</strong>und dann den Kunden aus der Liste. Wählen Sie im Menü „Kunden” <strong>Abonnements</strong> und dann das Abonnement aus der Liste aus. Wählen Sie <strong>Aktualisieren</strong> aus, um <strong>Vertriebspartner (MPN-ID)</strong> zu ändern.</p>
<p>Wenn ein CSP-Partner das Abonnement direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners.</p>
<p>Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt.</p>
<p>Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> Lizenzbasierte Dateifelder


Um Ihre Gebühren mit den Bestellungen Ihrer Kunden abzugleichen, vergleichen Sie die Informationen unter Syndication\_Partner\_Subscription\_Number in der Abgleichungsdatei mit der Abonnement-ID aus PartnerCenter.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Spalte</strong></td>
<td><strong>Beschreibung</strong></td>
<td><strong>Beispielwert</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>Eindeutiger Bezeichner für eine spezifische Abrechnungsentität im GUID-Format. Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen. In allen Zeilen gleich.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform. Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</p>
<p>Diese ID ist nicht mit der Abonnement-ID in der Partner-Verwaltungskonsole identisch. Siehe Syndication_Partner_Subscription_Number.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>Eindeutiger Bezeichner des Abonnements. Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen, daher ist dies für die Analyse der Erstattungsdatei wichtig.</p>
<p>Dieses Feld ist der Abonnement-ID in der Partner-Administratorkonsole zugeordnet.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>Eindeutige Angebot-ID. Standard-Angebots-ID gemäß der Preisliste.</p>
<p><b>Hinweis</b>: Dieser Wert entspricht nicht der Angebots-ID aus der Preisliste. Siehe DurableOfferID unten.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>Eindeutige dauerhafte Angebots-ID gemäß Definition in der Preisliste.</p>
<p><b>Hinweis</b>: Dieser Wert entspricht der Angebots-ID aus der Preisliste.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert.</p></td>
<td>Microsoft Office 365 (Plan E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>Das Anfangsdatum des Abonnements, festgelegt auf den Tag nach Übermittlung der Bestellung. Wenn Sie das Anfangsdatum des Abonnements mit dem Enddatum vergleichen, können Sie feststellen, ob der Kunde sich noch im ersten Jahr des Abonnements befindet, oder ob das Abonnement für das folgende Jahr verlängert wurde.</p>
<p>Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</p></td>
<td>01.02.2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>Enddatum des Abonnements: 12 Monate + x Tage nach dem Anfangsdatum (entspricht dem Abrechnungsdatum für den Partner) oder 12 Monate ab dem Verlängerungsdatum.</p>
<p>Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert. Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich.</p>
<p>Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</p></td>
<td>01.02.2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>Der erste Tag, an dem Gebühren anfallen.</p>
<p>Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</p>
<p>Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</p></td>
<td>01.02.2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Letzter Tag, an dem Gebühren anfallen.</p>
<p>Wenn ein Kunde die Anzahl der Arbeitsplätze ändert, werden anhand dieser Anzahl die Kosten pro Tag (anteilsmäßig) berechnet.</p>
<p>Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</p></td>
<td>28.2.2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Art der Gebühren oder der Anpassung. Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></p></td>
<td><p>Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>Preis pro Arbeitsplatz, wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht. Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</p></td>
<td>6,82</td>
</tr>
<tr class="even">
<td>Menge</td>
<td><p>Anzahl der Arbeitsplätze Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Betrag</td>
<td><p>Gesamtpreis für die Menge Hilfreich der Überprüfung, dass die Betragsberechnung mit der Abrechnung für Ihre Kunden übereinstimmt.</p></td>
<td>13,32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Rabattbetrag auf diese Gebühren. IUR (Internal Use Rights) oder neue Abonnements, die Anspruch auf einen Bonus haben, enthalten ebenfalls einen Rabattbetrag in dieser Spalte.</p></td>
<td>2,32</td>
</tr>
<tr class="odd">
<td>Zwischensumme</td>
<td><p>Gesamtbetrag vor Steuern Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Steuern</td>
<td><p>USt.-Betrag basierend auf Ihren Market& #39; s Steuervorschriften und spezifischen gegebenheiten.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Währung</td>
<td><p>Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Customer& #39; s Organisationsnamen im Partner Center gemeldet. Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</p></td>
<td>Test für Kunde A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>MPN-ID des CSP-Partners</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>MPN-ID des registrierten Handelspartners für das Abonnement. Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Customer& #39; s-Domänennamen, wird zur Identifizierung des Kunden verwendet. Dies sollte nicht verwendet werden, um den Kunden eindeutig zu identifizieren, wie der Kunde/Partner über das Office 365-Portal Vanity/Standarddomäne aktualisieren können. Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>Abonnement-Nickname. Wenn kein Nickname angegeben ist, verwendet Partner Center den OfferName.</p></td>
<td>PROJECT ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Dies ist ein identisches Feld für den Angebotsnamen).</p></td>
<td>PROJECT ONLINE PREMIUM OHNE PROJECT-CLIENT</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>Nutzungsbasierte Dateifelder


Um Ihre Gebühren mit der Nutzung des Kunden abzugleichen, vergleichen Sie ResellerID/ResellerName/ResellerBillableAccount aus der Abgleichungsdatei, den Kundennamen und die Abonnement-ID in Partner Center.

Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Spalte</strong></td>
<td><strong>Beschreibung</strong></td>
<td><strong>Beispielwert</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>Partner-ID im GUID-Format.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>Partnername.</p></td>
<td>Acme integriert</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>Partner-Konto-ID.</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Customer& #39; s Organisationsnamen im Partner Center gemeldet. Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</p></td>
<td>Test für Kunde A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>MPN-ID des CSP-Partners.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>MPN-ID des registrierten Handelspartners für das Abonnement. Siehe <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Aufschlüsseln nach Partner</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</p>
<p>Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</p></td>
<td>01.02.2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen.</p>
<p>Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</p></td>
<td>28.02.2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken.</p>
<p>Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>Nickname des Service-Angebots.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>Branche des Service-Angebots</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform. Kann beim Kontakt zum Support zum Identifizieren des Abonnements hilfreich sein, jedoch nicht zur Abstimmung.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>Der Name des fraglichen Azure-Dienstes</p></td>
<td>VIRTUELLE COMPUTER</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Der bestimmte Typ des Windows Azure-Dienstes.</p></td>
<td><ul>
<li>Service Bus – einzeln oder als Paket</li>
<li>SQL Azure-Datenbank – Business oder Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Ressourcenname</td>
<td><p>Der Name der Azure-Ressource.</p></td>
<td><ul>
<li>Übertragung eingehender Daten (GB)</li>
<li>Übertragung ausgehender Daten (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>Die Region, auf die sich die Nutzung bezieht. Wird in erster Linie zum Zuweisen von Tarifen für die Datenübertragung verwendet, da sich die Tarife je nach Region unterscheiden.</p></td>
<td>Asien-Pazifik, Europa, Lateinamerika, Nordamerika</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>MSFT eindeutiger Bezeichner für das Angebot</p></td>
<td>7UD 00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>Eine ID und Menge für die Angabe der verschiedenen Preise für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum. Für abgestufte Raten für Azure wird möglicherweise eine Rate für eine bestimmte Menge von berechenbare Einheiten berechnet und eine andere Rate danach.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums.</p>
<p>Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>Enthaltene Einheiten als Teil des Angebots. In der Regel nicht im CSP vorhanden.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>Einheiten, die nicht Teil des Angebots sind und vom Partner bezahlt werden müssen.</p>
<p>Gleich ConsumedQuantity - IncludedQuantity.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>Gültiger Angebotspreis ab Anfangsdatum des Abonnements.</p></td>
<td>0,0808$</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrist mal OverageQuantity, auf den nächsten Cent gerundet.</p></td>
<td>0,085$</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>USt.-Betrag basierend auf Ihren Market& #39; s Steuervorschriften und spezifischen gegebenheiten.</p></td>
<td>0,08$</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Gesamtbetrag nach Steuern, wo Steuern berechnet werden.</p></td>
<td>0,93$</td>
</tr>
<tr class="odd">
<td>Währung</td>
<td><p>Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>Nettopreis pro Einheit. Gleich PretaxCharges / OverageQuantity, auf den nächsten Cent gerundet.</p></td>
<td>0,08$</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>Bruttopreis pro Einheit. Gleich PostTaxTotal / OverageQuantity oder PretaxEffectiveRate + Steuersatz pro Einheit, auf den nächsten Cent gerundet.</p></td>
<td>0,08$</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Art der Gebühren oder der Anpassung. Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></p></td>
<td><p>Siehe <a href="#charge_types">Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>Eindeutige Konto-ID auf der MSFT-Abrechnungsplattform.</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>Datum der Service-Bereitstellung.</p></td>
<td>01.02.2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</p></td>
<td>Ostasien, Südostasien, Nordeuropa, Westeuropa, Vereinigte Staaten (Mitte/Norden), Vereinigte Staaten (Mitte/Süden)</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>Diese Spalte wird verwendet, um den einzelnen Microsoft Azure-Dienst zu verfolgen, der in der Spalte mit dem Dienstnamen möglicherweise nicht eindeutig identifiziert ist. Beispielsweise werden Datenübertragungen als &quot;Microsoft Azure – Alle Dienste&quot; in der Dienstnamenspalte angegeben. In der Spalte „MeteredService“ wird angegeben, auf welchen Dienst sich die Nutzung jeweils bezieht.</p></td>
<td>AccessControl, CDN, Computing, Datenbank, ServiceBus, Speicher</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>Eine Unterüberschrift, die den einzelnen Microsoft Azure-Dienst jenseits der Stufe weiter erläutert, die im Feld „MeteredService” bereitgestellt wird.</p></td>
<td>EXTERN</td>
</tr>
<tr class="even">
<td>Projekt</td>
<td><p>Vom Kunden definierter Name für die Dienstinstanz</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</p></td>
<td>Beispiel: Wenn Sie während eines Monats mit 30 Tagen über eine individuell bereitgestellte Verbindung verfügen, wird für Service Info 1 „1,000000 Verbindungen/30 Tage” angegeben. Wenn ein Paket von 25 ServiceBus-Verbindungen bereitgestellt wurden und Sie an diesem Tag 1 genutzt haben, wird als tägliche Nutzung für diesen Tag „25 Verbindungen/30 Tage – Verwendet: 1,000000“ angegeben.</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Customer& #39; s-Domänennamen, wird zur Identifizierung des Kunden verwendet. Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>Einheit</td>
<td><p>Die Einheit des Ressourcennamens</p></td>
<td>GB oder STUNDEN</td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a>Einmalige und wiederkehrenden Dateifelder

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Spalte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td>PartnerID</td>
<td><p>Eindeutiger Bezeichner für Microsoft Azure Active Directory-Mandanten für eine spezifische abrechnungsentität im GUID-Format '. Nicht zur Abstimmung erforderlich, kann jedoch hilfreiche Informationen bereitstellen. In allen Zeilen gleich.</p></td>
</tr>

<tr class="even">
<td>Kunden-Id</td>
<td><p>Eindeutige Microsoft Azure Active Directory-Mandanten-ID im GUID-Format, die zur Identifizierung des Kunden verwendet.</p></td>
</tr>

<tr class="odd">
<td>Kundenname</td>
<td><p>Firmenname des Kunden wie im Partner Center angegeben.</p></td>
</tr>

<tr class="even">
<td>CustomerDomainName</td>
<td><p>Kundendomänenname: wird zur Identifizierung des Kunden verwendet. Dies sollte nicht verwendet werden, um den Kunden eindeutig zu identifizieren, wie der Kunde/Partner über das Office 365-Portal Vanity/Standarddomäne aktualisieren können. Dieses Feld wird bis zum zweiten Rechnungszyklus leer angezeigt.</p></td>
</tr>

<tr class="odd">
<td>Kunden Land</td>
<td><p>Land, in dem sich der Kunde befindet.</p></td>
</tr>

<tr class="even">
<td>Rechnungsnummer</td>
<td><p>Rechnungsnummer, in der die angegebene Transaktion angezeigt wird.</p></td>
</tr>

<tr class="odd">
<td>MPNID</td>
<td><p>MPN-ID des CSP-Partners.</p></td>
</tr>

<tr class="even">
<td>Händler MpnId</td>
<td><p>MPN-ID des registrierten Handelspartners für das Abonnement.</p></td>
</tr>

<tr class="odd">
<td>Bestellnummer</td>
<td><p>Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-e-Commerce-Plattform. Kann beim Kontakt zum Support zum Identifizieren der Bestellung hilfreich sein, jedoch nicht zur Abstimmung.</p></td>
</tr>

<tr class="even">
<td>Bestellungsdatum</td>
<td><p>Der Zeitpunkt der Auftragserstellung.</p></td>
</tr>

<tr class="odd">
<td>ProductId</td>
<td><p>Die ID für das Produkt.</p></td>
</tr>

<tr class="even">
<td>SkuID</td>
<td><p>Die ID für eine bestimmte SKU.</p></td>
</tr>

<tr class="odd">
<td>AvailabilityId</td>
<td><p>Die ID für eine bestimmte Verfügbarkeit. "Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</p></td>
</tr>

<tr class="even">
<td>SKU-Namen</td>
<td><p>Titel für eine bestimmte SKU.</p></td>
</tr>

<tr class="odd">
<td>Produktname</td>
<td><p>Name des Produkts.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>Der Name des Herausgebers des Produkts.</p></td>
</tr>

<tr class="odd">
<td>Des PublisherID</td>
<td><p>Eindeutige ID für diesen Herausgeber.</p></td>
</tr>

<tr class="even">
<td>Abonnement-Beschreibung</td>
<td><p>Anzeigename eines Abonnements.</p></td>
</tr>

<tr class="odd">
<td>Abonnement-ID</td>
<td><p>Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-e-Commerce-Plattform. Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken. Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Der erste Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Letzter Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</p></td>
</tr>

<tr class="even">
<td>Begriff und Billingcycle</td>
<td><p>Der Begriff Länge und Rechnungszyklus für die Bestellung. Beispielsweise "1 Jahr, monatlich."</p></td>
</tr>

<tr class="odd">
<td>Gebührenart</td>
<td><p>Art der Gebühren oder der Anpassung.</p></td>
</tr>

<tr class="even">
<td>Preis pro Einheit</td>
<td><p>Der Preis wie zum Zeitpunkt des Kaufs in der Preisliste veröffentlicht. Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</p></td>
</tr>

<tr class="odd">
<td>Preis pro Einheit effektive</td>
<td><p>Preis pro Einheit nach Korrekturen vorgenommen wurden.</p></td>
</tr>

<tr class="even">
<td>Anzahl</td>
<td><p>Anzahl der Einheiten. Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</p></td>
</tr>

<tr class="odd">
<td>Einheitentyp</td>
<td><p>Der Typ der Einheit erworben wird.</p></td>
</tr>

<tr class="even">
<td>DiscountDetails</td>
<td><p>Eine Erklärung, alle anwendbaren Rabatte.</p></td>
</tr>

<tr class="odd">
<td>Zwischensumme</td>
<td><p>Gesamtbetrag vor Steuern Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt.</p></td>
</tr>

<tr class="even">
<td>Steuern</td>
<td><p>USt.-Betrag auf der Grundlage der Steuervorschriften und spezifischen Gegebenheiten Ihres Markts.</p></td>
</tr>

<tr class="odd">
<td>Gesamt</td>
<td><p>Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden.</p></td>
</tr>

<tr class="even">
<td>Währung</td>
<td><p>Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform.</p></td>
</tr>

<tr class="odd">
<td>AlternateID</td>
<td><p>Ein alternativer Bezeichner, der eine ID ein.</p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a>Nutzung täglich bewertete Dateifelder


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Spalte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td>PartnerID</td>
<td><p>Partner-ID im GUID-Format.</p></td>
</tr>

<tr class="even">
<td>PartnerName</td>
<td><p>Partnername.</p></td>
</tr>

<tr class="odd">
<td>Kunden-ID</td>
<td><p>Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet.</p></td>
</tr>

<tr class="even">
<td>CustomerCompanyName</td>
<td><p>Firmenname des Kunden wie im Partner Center angegeben. Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen.</p></td>
</tr>

<tr class="odd">
<td>CustomerDomainName</td>
<td><p>Domänenname des Kunden. Für die aktuelle Aktivität nicht verfügbar.</p></td>
</tr>

<tr class="even">
<td>Kunden Land</td>
<td><p>Land, in dem sich der Kunde befindet.</p></td>
</tr>

<tr class="odd">
<td>MPNID</td>
<td><p>MPN-ID des CSP-Partners.</p></td>
</tr>

<tr class="even">
<td>Händler MPNID</td>
<td><p>MPN-ID des registrierten Handelspartners für das Abonnement. Für die aktuelle Aktivität nicht verfügbar.</p></td>
</tr>

<tr class="odd">
<td>InvoiceNumber</td>
<td><p>Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. Für die aktuelle Aktivität nicht verfügbar.</p></td>
</tr>

<tr class="even">
<td>ProductId</td>
<td><p>Die ID für das Produkt.</p></td>
</tr>

<tr class="odd">
<td>SkuID</td>
<td><p>Die ID für eine bestimmte SKU.</p></td>
</tr>

<tr class="even">
<td>AvailabilityId</td>
<td><p>Die ID für eine bestimmte Verfügbarkeit. "Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist.</p></td>
</tr>

<tr class="odd">
<td>SKU-Namen</td>
<td><p>Titel für eine bestimmte SKU.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>Der Name des Herausgebers.</p></td>
</tr>

<tr class="odd">
<td>Des PublisherID</td>
<td><p>Die ID des Herausgebers, im GUID-Format. Für die aktuelle Aktivität nicht verfügbar.</p></td>
</tr>

<tr class=”even">
<td>Abonnement-Beschreibung</td>
<td><p>Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Dies ist ein identisches Feld für den Angebotsnamen).</p></td>
</tr>

<tr class="odd">
<td>Abonnement-ID</td>
<td><p>Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann zum Identifizieren des Abonnements bei einer Supportanfrage nützlich sein, dient jedoch nicht zu Abstimmungszwecken. Diese unterscheidet sich von der Abonnement-ID auf der Partner-Administratorkonsole.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Anfangsdatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen. Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Enddatum des Abrechnungszeitraums, außer wenn Datumsangaben zu zuvor nicht berechneten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus) vorliegen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt.</p></td>
</tr>

<tr class="even">
<td>Nutzung Datum</td>
<td><p>Datum der Service-Nutzung.</p></td>
</tr>

<tr class="odd">
<td>Anzeige-Typ</td>
<td><p>Der Typ der Anzeige.</p></td>
</tr>

<tr class="even">
<td>Meter Kategorie</td>
<td><p>Der obersten Ebene Dienst für die Verwendung.</p></td>
</tr>

<tr class="odd">
<td>Anzeige-Id</td>
<td><p>Die ID für die Anzeige verwendet wird.</p></td>
</tr>

<tr class="even">
<td>Meter Unterkategorie</td>
<td><p>Der Typ des Azure-Dienst, der die Rate auswirken kann.</p></td>
</tr>

<tr class="odd">
<td>Meter Name</td>
<td><p>Die Maßeinheit für die Anzeige genutzt wird.</p></td>
</tr>

<tr class="even">
<td>Meter Region</td>
<td><p>Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft.</p></td>
</tr>

<tr class="odd">
<td>Einheit</td>
<td><p>Die Einheit des Ressourcennamens.</p></td>
</tr>

<tr class="even">
<td>Verbrauchten Menge</td>
<td><p>Der Betrag für genutzte Dienste (Stunden, GB usw.) während des Berichtszeitraums. Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum.</p></td>
</tr>

<tr class="odd">
<td>Speicherort der Ressource</td>
<td><p>Die Datacenter, in denen die Anzeige ausgeführt wird.</p></td>
</tr>

<tr class="even">
<td>Verbrauchten Service</td>
<td><p>Der Azure-Plattform-Dienst, den Sie verwendet.</p></td>
</tr>

<tr class="odd">
<td>Ressourcengruppe</td>
<td><p>Der Ressourcengruppe, in der die bereitgestellte Anzeige ausgeführt wird.</p></td>
</tr>

<tr class="even">
<td>Ressourcen-URI</td>
<td><p>Der URI der Ressource verwendet wird.</p></td>
</tr>

<tr class="odd">
<td>Gebührenart</td>
<td><p>Art der Gebühren oder der Anpassung. Für die aktuelle Aktivität nicht verfügbar.</p></td>
</tr>

<tr class="even">
<td>Preis pro Einheit</td>
<td><p>Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</p></td>
</tr>

<tr class="odd">
<td>Anzahl</td>
<td><p>Anzahl der Lizenzen. Stellen Sie sicher, dass dies den Informationen entspricht, die in Ihrem Abrechnungssystem während der Abstimmung gespeichert wurden.</p></td>
</tr>

<tr class="even">
<td>Einheitentyp</td>
<td><p>Der Typ der Einheit der Anzeige ist in in Rechnung gestellt. Für die aktuelle Aktivität nicht verfügbar.</p></td>
</tr>

<tr class="odd">
<td>Abrechnung vor Steuern</td>
<td><p>Gesamtbetrag vor Steuern.</p></td>
</tr>

<tr class="even">
<td>Währung der Abrechnung</td>
<td><p>Die Währung in einer geografischen Region des Kunden</p></td>
</tr>

<tr class="odd">
<td>Preise gewöhnlichen insgesamt</td>
<td><p>Die Preise vor Steuern hinzugefügt werden.</p></td>
</tr>

<tr class="even">
<td>Währung Preise</td>
<td><p>Die Währung, in der Preisliste wiedergegeben werden soll.</p></td>
</tr>

<tr class="odd">
<td>Service Info 1</td>
<td><p>Die Anzahl der ServiceBus-Verbindungen, die bereitgestellt und an einem bestimmten Tag genutzt wurden.</p></td>
</tr>

<tr class="even">
<td>Service-Informationen 2</td>
<td><p>Ein legacy-Feld, das optionale Service-spezifischen Metadaten erfasst.</p></td>
</tr>

<tr class="odd">
<td>Schilder</td>
<td><p>Tags, die Sie für die Anzeige in der Reihenfolge zum Gruppieren Abrechnung zuweisen. Beispielsweise können Sie Tags verwenden, um Kosten von der Abteilung zu verteilen, die die Anzeige verwendet.</p></td>
</tr>

<tr class="even">
<td>Zusätzliche Infos</td>
<td><p>Alle zusätzlichen Informationen, die in anderen Spalten nicht behandelt.</p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a>Siehe Zuordnung von Gebühren zwischen einer Rechnung und der Erstattungsdatei

Ihre Rechnung enthält eine Zusammenfassung der Gebühren, während die Erstattungsdatei eine detaillierte Aufschlüsselung der Positionstransaktionen bereitstellt, einschließlich der Gebührentypen.

Zum Erstellen von Querverweisen der Gebührenbeträge zwischen der Rechnung und der Abstimmungsdatei können Sie Microsoft Excel-Filteroptionen verwenden, indem Sie in der Erstattungsdatei nach Gebührentypen filtern, um die Rechnungsgebühren einer Reihe von Gebührenauflistungen in der Erstattungsdatei zuzuordnen.

Sowohl nutzungsbasierte als auch lizenzbasierte Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren an (verbrauchte Einheiten und zusammenhängende Kosten). Guthaben, Rabatte oder Erstattungen, die auf der Rechnung als "Anpassungen" angezeigt werden, werden nicht in der Abstimmungsdatei angezeigt.

Die folgende Tabelle zeigt die Zuordnungen zwischen einem Rechnungsabschnittund zugehörigen Gebührentypen, die möglicherweise auf den Erstattungsdateien angezeigt werden. 

<table>
<tbody>
<tr>
<td>
<p><strong>Beschreibung der Rechnungsgebühr</strong></p>
</td>
<td>
<p><strong>Gebührenbeschreibung der Abstimmungsdatei (ChargeType-Spalte)</strong></p>
</td>
<td>
<p><strong>Um welche Gebühr handelt es sich?</strong></p>
</td>
<td>
<p><strong>Wie ordne ich diese ChargeTypes der Rechnung zu?</strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong>Lizenzbasierte Gebühren</strong></p>
</td>
<td>
<p>Aktivierungsgebühr</p>
</td>
<td>
<p>Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf nutzt</p>
</td>
<td rowspan="10">
<p>Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Betrag</strong>.</p>
</td>
</tr>
<tr>
<td>
<p>Stornierungsgebühr</p>
</td>
<td>
<p>Anteilige Gebühren werden an den Kunden zurückerstattet, wenn verknüpfte Lizenzen geändert werden.</p>
</td>
</tr>
<tr>
<td>
<p>Gebühr für Zyklus</p>
</td>
<td>
<p>Periodische Gebühren für ein Abonnement</p>
</td>
</tr>
<tr>
<td>
<p>Anteiliger Zyklus für Instanz</p>
</td>
<td>
<p>Anteilige vom Kunden geschätzte Gebühren, wenn verknüpfte Lizenzen geändert werden</p>
</td>
</tr>
<tr>
<td>
<p>Gebühren bei Abbrechen anteilig zuordnen</p>
</td>
<td>
<p>Anteilige Erstattung für nicht verwendete Teile des Diensts bei einer Stornierung</p>
</td>
</tr>
<tr>
<td>
<p>Anteilige Gebühren beim Kauf</p>
</td>
<td>
<p>Der Typ der Abrechnung für ein Abonnement bei Verwendung der jährlichen Abrechnung</p>
</td>
</tr>
<tr>
<td>
<p>Kaufgebühr</p>
</td>
<td>
<p>Der Typ der Abrechnung für ein Abonnement bei Verwendung monatliche Abrechnung</p>
</td>
</tr>
<tr>
<td>
<p>Anteilige Gebühr bei Verlängerung</p>
</td>
<td>
<p>Anteilige Gebühren nach Verlängerung des Abonnements</p>
</td>
</tr>
<tr>

<td>
<p>Verlängerungsgebühr</p>
</td>
<td>
<p>Gebühr für Verlängerung eines Abonnements</p>
</td>
</tr>
<tr>
<td>
<p>Anteilige Gebühren beim Aktivieren</p>
</td>
<td>
<p>Anteilige Gebühren bei Aktivierung bis zum Ende des Abrechnungszeitraums</p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>Nutzungsgebühren</strong></p>
</td>
<td>
<p>Nutzungsgebühr beim Abbrechen bewerten</p>
</td>
<td>
<p>Nutzungsgebühr für Zugriffe für die nicht bezahlte Verwendung während des aktuellen Abrechnungszeitraums bei der Kündigung</p>
</td>
<td rowspan="2">
<p>Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</p>
</td>
</tr>
<tr>
<td>
<p>Nutzungsgebühr für den aktuellen Zyklus bewerten</p>
</td>
<td>
<p>Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum</p>
</td>
</tr>
<tr>
<td>
<p><strong>Guthaben</strong></p>
</td>
<td>
<p>Einen Artikel versetzen</p>
</td>
<td>
<p>Teilweise oder vollständige Erstattung an eine Position, einschließlich Steuern</p>
</td>
<td>
<p>Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalForCustomer</strong>.</p>
<p>Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PostTaxTotal</strong>.</p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong>Nutzungsbasierte Rabatte</strong></p>
</td>
<td>
<p>Aktivierungsrabatt</p>
</td>
<td>
<p>Rabatt auf Aktivierung des Abonnements</p>
</td>

<td rowspan="4">
<p>Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>PretaxCharges</strong>.</p>
</td>
</tr>
<tr>
<td>
<p>Zyklusrabatt</p>
</td>
<td>
<p>Rabatt auf periodische Gebühren</p>
</td>
</tr>
<tr>
<td>
<p>Verlängerungsrabatt</p>
</td>
<td>
<p>Rabatt auf Verlängerung des Abonnements</p>
</td>
</tr>
<tr>
<td>
<p>Stornorabatt</p>
</td>
<td>
<p>Gebühren, wenn Rabatte storniert werden</p>
</td>
</tr>


<tr>
<td>
<p><strong>Lizenzbasierte Rabatte</strong></p>
</td>
<td>
<p><em>Kann auf mehrere Gebührentypen angewendet werden</em></p>
</td>
<td>
<p></p>
</td>
<td>
<p>Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>TotalOtherDiscount</strong>.</p>
</td>
</tr>
<tr>
<td>
<p><strong>Steuern</strong>&nbsp;oder&nbsp;<strong>Umsatzsteuer</strong></p>
</td>
<td>
<p><em>Kann auf mehrere Gebührentypen angewendet werden</em></p>
<p><em>Ausnahme: &quot;einen Artikel versetzen&quot; enthält bereits steuern. Siehe Guthaben, oben.</em></p>
</td>
<td>
<p>Steuern oder Umsatzsteuern (Umsatzsteuer)</p>
</td>
<td>
<p>Erstellen Sie in der lizenzbasierten Datei die Summe der Spalte <strong>Steuern</strong>.</p>
<p>Erstellen Sie in der nutzungsbasierten Datei die Summe der Spalte <strong>TaxAmount</strong>.</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
