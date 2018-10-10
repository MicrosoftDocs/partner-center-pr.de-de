---
title: Informationen zu Ihrer Rechnung | Partner Center
description: Ihre Rechnung stellt eine Zusammenfassung aller Gebühren (programm-, produkt- und kundenübergreifend) für den aktuellen Monatszeitraum dar. Es ist im Partner Center verfügbar.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
keywords: Abonnementabrechnungen, Abrechnung, Abrechnung im Partner Center, Partner Center-Abrechnung, meine Rechnung lesen, Rechnung, Rechnung für Partner Center, CSP-Abrechnung, wo ist meine Rechnung?
ms.localizationpriority: medium
ms.openlocfilehash: 81262c11ab402dcd1748f9f8fde5cdeceac0f4f9
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489406"
---
# <a name="read-your-bill"></a>Informationen zu Ihrer Rechnung

**Betrifft**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government
-  Partner Center für Microsoft Cloud Deutschland

Ihre Rechnung wechseln Sie zum Menü " **Partner Center** ", und wählen Sie dann, **Abrechnung** , um Ihren Abrechnungsverlauf und -Trend, Links zu Ihrer Rechnung und abstimmungsdatei sowie Ihre letzte Zahlung anzeigen anzuzeigen.

Partner im Cloud Solution Provider-Programm mit monatlicher Rechnung bezahlen Microsoft rückwirkend für 60Tage für das Abonnement ihres Kunden (sowohl lizenzbasierte und die nutzungsbasierte Abonnements).

> [!NOTE]  
> Ihre Rechnung stellt eine Zusammenfassung aller Gebühren (programm-, produkt- und Kundenübergreifend) für den aktuellen Monatszeitraum dar und ist innerhalb von vier (4) Tagen nach Ablauf des ausgewählten Abrechnungsdatums verfügbar.

Sie erhalten eine Rechnung für lizenzbasierte (Office 365) und Gebühren für nutzungsbasierte (Azure) und eine separate Rechnung für einmalige (Azure reserved VM Instances) Gebühren.

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
<td>Die Adresse, an die wir Ihre Rechnung senden. Um diese Adresse zu ändern, wechseln Sie zu Einstellungen > Partnerabrechnungsprofil. </td>
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
<td>Beispielsweise der Rabatt, den der Kunde auf den normalen Preis des Abonnements erhält. Dies wird als Pauschbetrag und nicht als Preis pro Einheit oder Lizenz aufgeführt.</td>
</tr>
<tr class="odd">
<td>Guthaben</td>
<td>Guthaben oder Anpassungen für Änderungen an Abonnements (Beispiel: Erhöhung oder Reduzierung der Lizenzzahl).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Zwischensumme</td>
<td>Gesamtbetrag vor Steuern und Gebühren exklusive und Guthaben.</td>
</tr>
<td>Steuern</td>
<td>Die gesamten Steuern für die aktuellen Gebühren, wie im Abschnitt „Details“ auf Seite 2 der Rechnung summiert. Diese Zahl ist die Summe aller Gebühren in folgenden Spalten:
<ul>
<li>Spalte &quot;TaxAmount&quot; der nutzungsbasierten Abstimmungsdatei (Spalte AA) und</li>
<li>Spalte &quot;Steuern&quot; der lizenzbasierten Abgleichungsdatei (Spalte U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Andere Guthaben</td>
<td>Exklusive Guthaben.</td>
</tr>
<tr class="even">
<td>Aktuelle Gebühren insgesamt</td>
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
<td>Für CSP-Partner erfolgt die Abrechnung monatlich oder jährlich.</td>
</tr>
<tr class="even">
<td>Rechnungsdatum</td>
<td>Das Ausstellungsdatum Ihrer Rechnung.</td>
</tr>
<tr class="odd">
<td>Zahlungsbedingungen</td>
<td>Für einmalige Einkäufe wird dies immer 60Tage sein.</td>
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
<td>Die Adresse, an der der Dienst verwendet wird. (Dies ist die rechtlich gültige Unternehmensadresse. Sie ist mit der Unternehmensprüfung verknüpft und kann nicht geändert werden.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Detaillierte Liste einmaliger Gebühren

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|Datum |Kaufdatum. |
|Beschreibung |Produktname. |
|Anzahl |Die Anzahl von erworbenen Produkten (Reservierungen etc). |
|Preis pro Einheit |Preis pro Produkt (Reservierungen etc). |
|Rabatte |Alle anwendbaren Rabatte. |
|Vorsteuerbetrag |Zwischensumme vor Steuern. |
|Mehrwertsteuer |Steuerbetrag. |
|Gesamt |Zahlungen gesamt. |
 



