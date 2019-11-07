---
title: Informationen zu Ihrer Rechnung | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ihre Rechnung stellt eine Zusammenfassung aller Gebühren (programm-, produkt- und kundenübergreifend) für den aktuellen Monatszeitraum dar. Sie steht im Partner Center zur Verfügung.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: Abonnementabrechnungen, Abrechnung, Abrechnung im Partner Center, Partner Center-Abrechnung, meine Rechnung lesen, Rechnung, Rechnung für Partner Center, CSP-Abrechnung, wo ist meine Rechnung?
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652174"
---
# <a name="read-your-bill"></a>Informationen zu Ihrer Rechnung

**Zielgruppe**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government


Die Abrechnung befindet sich im Menü **Partner Center** unter **Abrechnung**. Dort können Sie Ihren Abrechnungsverlauf und -trends, Links zu Ihrer Rechnung und zur Kontenabstimmungsdatei sowie Ihre letzte Zahlung anzeigen.

Partner im Cloud Solution Provider-Programm mit monatlicher Rechnung bezahlen Microsoft rückwirkend für 60 Tage für das Abonnement ihres Kunden (sowohl lizenzbasierte und die nutzungsbasierte Abonnements).

> [!NOTE]  
> Ihre Rechnung stellt eine Zusammenfassung aller Gebühren (programm-, produkt- und kundenübergreifend) für den aktuellen Monatszeitraum dar und ist innerhalb von zwei (2) Tagen nach Ablauf des ausgewählten Abrechnungsdatums (in UTC-Zeit) verfügbar. Wenn beispielsweise das Abrechnungsdatum der 12. September ist, beginnt der Prozess zur Rechnungsgenerierung am 13. September um 12:00 Uhr UTC und endet am 14. September um 12:00 Uhr UTC. Wenn Ihre Rechnung nicht um 11:59uhr UTC am 15. September angezeigt wird, sind Sie nicht mehr in Ihrem Vereinbarung zum Servicelevel und sollten eine Service Request. 

Sie erhalten eine Rechnung für lizenzbasierte (Office 365) und nutzungsbasierte (Azure) Gebühren und eine separate Rechnung für einmalige Gebühren (Azure Reserved VM Instances).

Aufgeschlüsselte Einzelheiten zu den Gebühren finden Sie in den zugehörigen Abstimmungsdateien. Die Abstimmungsdateien enthalten die Kunden-IDs und Abonnement-IDs, mit deren Hilfe Sie Kundenrechnungen erstellen. Weitere Informationen finden Sie unter [So wird's gemacht: Verwenden der Abstimmungsdateien](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Definitionen zur Rechnungsdatei


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Feld</strong></td>
<td><strong>Beschreibung</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>Ihre Steuernummer.</td>
</tr>
<tr class="odd">
<td>Kundennummer</td>
<td>Ihre Kundennummer.</td>
</tr>
<tr class="even">
<td>Rechnungsempfänger</td>
<td>Die Adresse, an die wir Ihre Rechnung senden. Zum Ändern von Firmenname oder Adresse bearbeiten Sie Ihr Partner Center-Abrechnungsprofil. </td>
</tr>
<tr class="odd">
<td>Lizenzbasierte Gebühren</td>
<td>Die monatlichen (oder jährlichen) pauschalen Gebühren für die gekauften nutzungsbasierten Lizenzen, die im Voraus in Rechnung gestellt werden. Diese Zahl ist die Summe aller Gebühren in der Spalte &quot;Zwischensumme&quot; der lizenzbasierten Abgleichungsdatei (Spalte T).</td>
</tr>
<tr class="even">
<td>Nutzungsbasierte Gebühren</td>
<td>Azure-Nutzung, einschließlich neuer Dienste oder Anwendungen, die während des Abrechnungsmonats aktiviert und verwendet wurden. Diese Zahl ist die Summe aller Gebühren in der Spalte &quot;PretaxCharges&quot; der nutzungsbasierten Abgleichungsdatei (Spalte Z).</td>
</tr>
<tr class="odd">
<td>Rabatte</td>
<td>Beispielsweise der Rabatt, den der Kunde auf den normalen Preis des Abonnements erhält. Dies wird als Pauschalbetrag und nicht als Preis pro Einheit oder Lizenz aufgeführt.</td>
</tr>
<tr class="odd">
<td>Gutschriften</td>
<td>Guthaben oder Anpassungen für Änderungen an Abonnements (Beispiel: Erhöhung oder Reduzierung der Lizenzzahl).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Zwischensumme</td>
<td>Gesamtbetrag vor Steuern und Gebühren und Guthaben exklusive Steuern</td>
</tr>
<td>Steuern</td>
<td>Die gesamten Steuern für die aktuellen Gebühren, wie im Abschnitt "Details" auf Seite 2 der Rechnung summiert. Diese Zahl ist die Summe aller Gebühren in folgenden Spalten:
<ul>
<li>Spalte &quot;TaxAmount&quot; der nutzungsbasierten Abstimmungsdatei (Spalte AA) und</li>
<li>Spalte &quot;Steuern&quot; der lizenzbasierten Abgleichungsdatei (Spalte U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Andere Guthaben</td>
<td>Guthaben exklusive Steuern</td>
</tr>
<tr class="even">
<td>Gesamtsumme der aktuellen Gebühren</td>
<td>Der in Ihrer Abrechnungswährung für den Abrechnungszeitraum zum angegebenen Termin fällige Betrag.</td>
</tr>
<tr class="odd">
<td>Zahlungsanweisungen</td>
<td>Beschreibt, wie Ihre Rechnung auf der Grundlage Ihrer Region bezahlt wird. Geben Sie bei einer Zahlung stets die Rechnungsnummer an.</td>
</tr>
<tr class="even">
<td>Rechnungsnummer</td>
<td>Die Nummer Ihrer Rechnung.</td>
</tr>
<tr class="odd">
<td>Abrechnungszeitraum</td>
<td>Der monatliche Zeitraum bis zum Rechnungsdatum. Dies ist der Zeitraum, in dem nutzungsbasierte Dienste verbraucht und lizenzbasierte Dienste auf Guthabenanpassungen oder Änderungen in der Lizenzanzahl abgestimmt werden.</td>
</tr>
<tr class="even">
<td>Rechnungsdatum</td>
<td>Ihr Rechnungsdatum oder Jahrestag, an dem Ihre Rechnung jeden Monat erstellt wird.</td>
</tr>
<tr class="odd">
<td>Zahlungsbedingungen</td>
<td>Für einmalige Einkäufe wird dies immer 60 Tage sein.</td>
</tr>
<tr class="even">
<td>Fälligkeitsdatum der Zahlung</td>
<td>Ihre Zahlung muss bis zu diesem Datum eingegangen sein.</td>
</tr>
<tr class="odd">
<td>Name des Kunden</td>
<td>Ihre Bestellnummer.</td>
</tr>
<tr class="even">
<td>Kundendienst</td>
<td>Die Adresse der Kundendienst-Website.</td>
</tr>
<tr class="odd">
<td>Dienstempfänger</td>
<td>Die Adresse, an der der Dienst verwendet wird. (Dies ist die rechtlich gültige Unternehmensadresse. Sie ist mit der Unternehmensprüfung verknüpft.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Detaillierte Liste einmaliger Gebühren

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|Datum |Kaufdatum. |
|Beschreibung |Produktname. |
|Anzahl |Die Anzahl von erworbenen Produkten (z. B. Reservierungen). |
|Preis pro Einheit |Preis pro Produkt (z. B. Reservierung). |
|Rabatte |Alle anwendbaren Rabatte. |
|Vorsteuerbetrag |Zwischensumme der Einkäufe vor Steuern. |
|Mehrwertsteuer |Steuerbetrag. |
|Gesamt |Zahlungen gesamt. |
 



