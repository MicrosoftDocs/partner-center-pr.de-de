---
title: Massen Vorgänge über Excel-Dateien in verweisen
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie Co-Selling-Verkaufschancen mithilfe von Excel-Dateien herunterladen, erstellen oder aktualisieren.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 16975e78c10aeb73bf141c1a1d0a215ac885039c
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645638"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Massen Vorgänge für Co-Selling-Möglichkeiten mithilfe von CSV (Comma-Separated Value)-Dateien

**Geeignete Rollen**

- Empfehlungsadministrator
- Empfehlungsbenutzer

Massen Vorgänge in Partner Center helfen Ihrem Unternehmen beim Exportieren und Importieren von Co-Selling-Verkaufschancen Daten. Navigieren Sie zur Seite "Co-Selling-Chancen", um die Import-und Export Links oben rechts auf dem Seitentitel Banner zu finden. Benutzer, die sowohl über **Administrator** Berechtigungen als auch über **Verweise auf Benutzer** Berechtigungen verfügen, können diese Funktion verwenden.

> [!IMPORTANT]
> Die durch den Massen Import durchgeführten Aktionen zum Erstellen/aktualisieren können nicht rückgängig gemacht werden. Gehen Sie vorsichtig vor, wenn Sie eine große Anzahl von Datensätzen ändern oder erstellen. Nach dem Erstellen eines Deals können nur eine Teilmenge von Feldern geändert werden. **Es sind keine Aktionen zulässig, wenn ein beliebiges Geschäft einen Endzustand wie abgelehnt/abgelaufen/gewonnen/verloren erreicht.**

## <a name="exporting-co-sell-opportunities"></a>Exportieren von Co-Selling-Verkaufschancen

Unten sind die Details der Export Funktionalität aufgeführt.

- Sie können **maximal 5000 Datensätze** exportieren, indem Sie auf die Schaltfläche exportieren klicken.
- Die heruntergeladenen Angebote basieren auf Ihren Zugriffsebenen. Verweisadministratoren und verweisbenutzer können unterschiedliche Ergebnisse auf Grundlage ihres Umfangs und ihrer Einbindung als Teammitglieder in den Geschäften erhalten. Weitere Informationen zu [Berechtigungen](permissions-overview.md#manage-referrals)finden Sie hier.
- Mit der Exportfunktion wird die aktuelle Registerkarte auf der Seite mit den Co-Selling-Verkaufschancen und die angewendeten Filter berücksichtigt.
- Eine CSV-Datei mit allen Daten, die auf den angewendeten Filtern basieren, wird generiert.
- Es kann bis zu einer Minute dauern, bis die Datensätze heruntergeladen wurden.
- Sie müssen nicht warten, bis die Download Aktion beendet ist. Auch wenn Sie zu anderen Seiten im Partner Center navigieren, wird die Datei heruntergeladen, sobald die Exportfunktion fertig ist.
- Sie können die heruntergeladene Datei wieder verwenden, um die Details des Details und den Upload zum Aktualisieren von Datensätzen zu ändern.

## <a name="importing-co-sell-opportunities"></a>Importieren von Co-Selling-Verkaufschancen

- Sie können mit der Importfunktion **maximal 1000 Datensätze** erstellen oder aktualisieren.
- Die Vorlage kann von Grund auf neu erstellt werden, indem Sie die Vorlage auf der Seite importieren im Partner Center herunterladen.
- Sie können auch die Export-Funktion verwenden, um die vorhandenen Datensätze herunterzuladen und zu aktualisieren.
- Wenn die Datei mehr als 1000 Datensätze enthält, kann Sie nicht verarbeitet werden.
- Nachdem die Datei verarbeitet wurde, wird eine Zusammenfassung mit der Anzahl der Verweise, die erstellt, aktualisiert und nicht verarbeitet wurden, auf der letzten Prozess Datei Karte angezeigt.
- Sie können die Details der verarbeiteten Datensätze herunterladen, Fehler beheben und dieselbe Datei hochladen, um die Datensätze zu erstellen oder zu aktualisieren, die in der vorherigen Testlauf fehlgeschlagen sind. **Entfernen Sie alle erfolgreichen Datensätze aus der Datei, bevor Sie die korrigierten Datensätze hochladen, die bei der vorherigen Ausführung fehlgeschlagen sind.**
- Fügen Sie zum Hinzufügen weiterer Projektmappen Nebenprojekt Mappe 1 zusätzliche Spalten hinzu, und verwenden Sie den Spaltennamen als Projekt Mappe X, wobei X die Nummer der Projekt Mappe in der Sache darstellt. Beispiel: Lösung 2, Lösung 3.
- Sie können einer Sache bis zu 50 Lösungen hinzufügen.
- Fügen Sie zum Hinzufügen weiterer Teammitglieder zusätzliche Spalten neben Teammitglied 1 hinzu, und verwenden Sie den Spaltennamen als Teammitglied x, wobei X die Nummer des Teammitglieds in der Sache darstellt. Beispielsweise Teammitglied 2, Teammitglied 3.
- Sie können einer Sache bis zu 50 Teammitglieder hinzufügen.

> [!NOTE]
> Sie müssen nicht warten, bis die Verarbeitung beendet ist. Nachdem die Verarbeitung fertiggestellt wurde, können die Details der zuletzt verarbeiteten Datei heruntergeladen werden. **Das Hochladen von Dateien mit 1000-Datensätzen kann bis zu 10 Minuten dauern.**

> [!IMPORTANT]
> Lesen Sie alle Anweisungen sorgfältig durch, und überprüfen Sie das Format der einzelnen Spalten in der folgenden Tabelle, bevor Sie mit CSV-Dateien in Partner Center erstellen oder aktualisieren.

|**Spaltenname**|**Ist obligatorisch?**|**Beschreibung**|**Beispiel Wert (e)**|
|-----|:-----|:---------|:---|
Errors|Nein|Fehler, die sich auf die CREATE/Update-Vorgänge "w. r. t" für die Verweise beziehen, werden in diese Spalte eingefügt. Wenn mehrere Fehler vorliegen, werden alle durch ein Semikolon getrennt aufgelistet.|Obligatorische Feld Lösung 1 fehlt.|
Engagement-ID|Nein|Die Engagement-ID wird vom Microsoft Partner Center-Referenzsystem generiert. Für die Erstellung neuer Verweise nicht erforderlich. Wenn Sie einen Datensatz aktualisieren, können Sie die vorhandene Engagement-ID verwenden.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Empfehlungs-ID|Nein|Die Verweis-ID wird vom Microsoft Partner Center-Referenzsystem generiert. Für die Erstellung neuer Verweise nicht erforderlich. Geben Sie die Verweis-ID ein, wenn Sie einen vorhandenen Datensatz aktualisieren.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Name des Deals|Ja|Der Anzeige Name für den Umgang mit Ihrem Verweis.|UK Spring Deal
Customer Name|Ja|Name des Kunden Unternehmens. Verwenden Sie den rechtlichen Namen der Organisation für eine schnelle Übereinstimmung auf der Microsoft-Seite.|Contoso Corporation
Kunden Adresszeile 1|Ja|Adresszeile 1 des Kunden Unternehmens. |Eine solche Methode
Kunden Adresszeile 2|Nein|Adresszeile 2 des Kunden Unternehmens.|NE 148 Straße
Kundenort|Ja|Stadt, in der sich die Kundenorganisation befindet.|Redmond
Bundesland/Kanton des Kunden|Nein|Zustand, in dem sich die Kundenorganisation befindet.|Washington
Postleitzahl des Kunden|Nein|Postleitzahl der Region, in der sich die Kundenorganisation befindet.|98052
Land des Kunden|Ja|Das Land/die Region, in dem sich die Kundenorganisation befindet. Verwenden Sie die beiden Buchstaben Ländercodes, wie [hier]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)erwähnt.|US
ID "D-U-n-S"|Nein|Versuchen Sie, die DUNS-ID der Kundenorganisation abzurufen. Dies trägt dazu bei, dass die Kundenorganisation auf der Microsoft-Seite schneller abgeglichen wird, was eine schnellere Zuweisung von Verkäufern ermöglicht. Sie können die DUNS-ID von dieser [Website](https://www.dnb.com/duns-number/lookup.html)kostenlos erhalten.|81466849
Vorname des Kundenkontakts|Depends (Abhängig)|Der Vorname ist nur obligatorisch, wenn Sie die Microsoft-Hilfe benötigen. Der Vorname des primären Kontakts der Kundenorganisation, der an diesem Teil arbeitet.|John
Nachname des Kundenkontakts|Depends (Abhängig)|Der Nachname ist nur obligatorisch, wenn Sie Microsoft Help benötigen. Nachname des primären Kontakts der Kundenorganisation, der an diesem Teil arbeitet.|Kunde
Telefonnummer des Kundenkontakts|Depends (Abhängig)|Die Telefonnummer ist nur obligatorisch, wenn Sie Microsoft Help benötigen. Telefonnummer des primären Kontakts der Kundenorganisation, der an diesem Teil arbeitet.|9999999999
E-Mail-Adresse des Kunden|Depends (Abhängig)|E-Mail-Adresse ist nur obligatorisch, wenn Sie Microsoft-Hilfe benötigen. E-Mail-Adresse des primären Kontakts der Kundenorganisation, der an diesem Teil arbeitet.|john.customer@contoso.com
Status des Partner Verweises|Ja|Gibt den Status des Deals aus der Perspektive Ihres Unternehmens an. Erforderlich, wenn Sie versuchen, einen Verweis zu erstellen oder zu ändern. Verwenden Sie **New** , wenn Sie versuchen, ein neues zu erstellen. Akzeptierte Werte werden [hier](https://docs.microsoft.com/partner/develop/referral-resources#referralstatus)dokumentiert.|Aktiv
Unter Status des Partner Verweises|Ja|Gibt den genauen Status des Deals an. Verwenden Sie **Accepted** , wenn Sie versuchen, ein neues zu erstellen. Dies ist auch erforderlich, wenn Sie einen vorhandenen Verweis ändern. Akzeptierte Werte werden [hier](https://docs.microsoft.com/partner/develop/referral-resources#referralsubstatus)dokumentiert.|Akzeptiert
Microsoft-Referenz Status|Depends (Abhängig)|Gibt den Status der Co-Selling-Anforderung an, die Sie an Microsoft gesendet haben. Dieses Feld ist schreibgeschützt. Alle Änderungen, die an diesem Feld beim Importieren der Daten vorgenommen werden, werden ignoriert.| Ausstehend
Abgelehnter/verlorener Grund|Depends (Abhängig)| Sie müssen diese Informationen nur angeben, wenn Sie den unter Status des Felds entweder in "abgelehnt" oder "verloren" ändern. Andernfalls können Sie diese Spalte ignorieren. <br/> **Geben Sie eine Zahl auf der Grundlage der folgenden Optionen ein.** <br/><br/> **1**-das Projektbudget ist nicht ausreichend.  <br/> **2**: der Kunde hat nicht geantwortet.  <br/> **3**-Kunde hat einen anderen Hersteller gewählt  <br/> **4** : Kundenanforderung nicht erfüllt  <br/> **5** , kein Kunde <br/> **6**-vorgeschlagene zeilige Zeit ist zu kurz <br/> **7** : Melden Sie sich als Missbrauch, Spam oder Phishing an <br/> **8** -weitere |6|
Sales Stage|Nein|Dies ist das Feld, das die ausführliche Verkaufsphase des Verweises angibt. Weitere Informationen zu Verkaufsphasen [finden Sie hier](https://aka.ms/salesStages) .|40
Geschätzter Werte Wert|Ja|"Der Wert des Deals basierend auf den ersten Konversationen mit dem Kunden. Dies kann geändert werden, bis der Status eines der Terminal Zustände erreicht wird.| gewonnen oder verloren. "|12563
Währung|Ja|Die Währung, in der der Wert für den Wert eingegeben wird. Die Währungscodes finden Sie [hier](https://en.wikipedia.org/wiki/ISO_4217).|USD
Geschätztes Schluss Datum|Ja|Das geschätzte Schluss Datum des Deals basierend auf den anfänglichen Konversationen mit dem Kunden im Format mm/dd/yyyy. <br/> **Das Datum sollte in der UTC-Zeitzone liegen. Alle Datumsangaben, die in der Benutzeroberfläche von Partner Center angezeigt werden, basieren auf lokalisierten Zeitzonen. Wenn Sie sich den Verweis ansehen, für den Sie das Datum in der UTC-Zeitzone angegeben haben, gibt es möglicherweise einen Unterschied in der Partner Center-Benutzeroberfläche.**|1/30/2020
CRM-ID|Nein|Bezeichner dieses spezifischen Verweises in Ihrem CRM-System, falls vorhanden. Dies ist ein kostenloses Formular Texteingabefeld.|34234324-sdfsdf-345345-SFD
Marketing Kampagnen-ID|Nein|Dieses Feld gibt die Marketingkampagne an, die zu diesem speziellen Verweis geführt hat. Normalerweise für die ROI-Berechnung verwendet|BingSummer2020
Notizen|Nein|Ausführliche Hinweise zu den Aktualisierungen im Zusammenhang mit der Referenz|Dies ist eine Beispiel Notiz.
Microsoft-Hilfe erforderlich?|Ja|Hiermit geben Sie an, ob Microsoft Ihnen helfen soll, diese Co-Selling-Anforderung zu tätigen.|Ja
Welche spezielle Hilfe von Microsoft ist verfügbar?|Depends (Abhängig)|Eine der sechs verschiedenen Möglichkeiten, wie Microsoft Ihnen helfen kann. Dies gilt nur, wenn Sie für die Frage "die Microsoft-Hilfe ist erforderlich? " <br/> **Geben Sie eine Zahl auf der Grundlage der folgenden Optionen ein.** <br/><br/> **1**-Arbeits Auslastungs spezifischer Wert-Vorschlag  <br/> **2**: technische Kunden Architektur  <br/> **3**: Proof of Concept/Demo  <br/> **4**-Anführungszeichen und Lizenzierung  <br/> Kunden Erfolg mit **5** Kunden nach dem Verkauf  <br/> **6**-allgemein oder Sonstiges|1|
Freigeben mit dem Microsoft-Vertriebsteam|Ja|Hiermit geben Sie an, ob Sie die Details des Deals mit dem Microsoft-Vertriebsteam teilen möchten. Dies gilt nur, wenn Sie für die Frage "die Microsoft-Hilfe ist erforderlich? "|Ja
Hinweise zu Microsoft|Nein|Bestimmte Notizen von Microsoft, wenn Sie Hilfe von Microsoft benötigen|Benötigen Sie Hilfe bei einem POC für den Kunden von Microsoft.
Zustimmung zum Freigeben von Kunden/Partner Kontakten|Ja|Zustimmung zur Freigabe von Kontaktdaten des Kunden und den Kontaktinformationen Ihres Unternehmens, die an diesem Teil arbeiten. **Wenn Sie für diese Spalte Nein auswählen, werden keine Geschäfte erstellt oder aktualisiert.** |Ja
Lösung 1|Ja|Lösungs-ID (erforderlich), die Währung (optional), in der der Wert für den Wert eingegeben wird. Sie finden [hier](https://en.wikipedia.org/wiki/ISO_4217)die Währungscodes, den Preis der SKU (optional) und die Anzahl der SKU (optional).  |Sol-1234-pqrs, USD, 10, 100
Team Mitglied 1|Ja|Vorname, Nachname, Mobiltelefonnummer und e-Mail-ID des entsprechenden Teammitglieds.| Bob, Partner, 999999, Bob.partner@Contoso.com
