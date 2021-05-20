---
title: Massenexport und -import von Co-Sell-Verkaufschancen über Excel-/CSV-Dateien in Empfehlungen
description: Erfahren Sie, wie Sie Co-Sell-Verkaufschancen mithilfe von Excel-Dateien (CSV) in Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: af567b9b8b36841b6e6fd7e18a34e1c4b6b81f2e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149161"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Massenvorgänge für Co-Sell-Verkaufschancen mithilfe von CSV-Dateien (Durch Komma getrennte Werte)

**Geeignete Rollen:** Administratorberechtigungen für Empfehlungen | Empfehlungsbenutzer

Massenvorgänge in Partner Center Ihrem Unternehmen beim Exportieren und Importieren von Co-Sell-Verkaufschancendaten. Navigieren Sie zur **Seite co-sell opportunities (Co-Sell-Verkaufschancen),** um die Import- und **Exportlinks** oben rechts im Titelbanner der Seite zu finden.  Benutzer mit **berechtigungen Empfehlungsadministratoren** **und Empfehlungsbenutzern** können diese Funktion verwenden.

> [!IMPORTANT]
> Die über den Massenimport durchgeführten Erstellungs-/Aktualisierungsaktionen sind nicht umkehrbar. Seien Sie vorsichtig, wenn Sie eine große Anzahl von Datensätzen ändern oder erstellen. Nach dem Erstellen eines Deal kann nur eine Teilmenge der Felder geändert werden. **Es sind keine Aktionen zulässig, sobald ein Deal einen Endzustand wie "Abgelehnt", "Abgelaufen", "Gewonnen" oder "Verloren" erreicht hat.**

## <a name="export-co-sell-opportunities"></a>Exportieren von Co-Sell-Verkaufschancen

Die folgenden Informationen beschreiben die Exportfunktionalität:

- Sie können maximal **5.000** Datensätze exportieren, indem Sie auf die Schaltfläche **Exportieren** klicken.
- Die heruntergeladenen Angebote basieren auf Ihren Zugriffsebenen. Empfehlungsadministratoren und Empfehlungsbenutzer erhalten je nach Umfang und Einbindung als Teammitglieder in den Deals möglicherweise unterschiedliche Ergebnisse. Erfahren Sie mehr über [Berechtigungen für Empfehlungen.](permissions-overview.md#manage-referrals)
- Die Exportfunktion übernimmt , um die aktuelle Registerkarte auf der Seite co-sell opportunities (Co-Sell-Verkaufschancen) und die angewendeten Filter zu berücksichtigen.
- Eine CSV-Datei mit allen Daten, die auf den angewendeten Filtern basieren, wird generiert.
- Das Herunterladen der Datensätze kann bis zu einer Minute dauern.
- Sie müssen nicht warten, bis die Downloadaktion abgeschlossen ist. Auch wenn Sie zu anderen Seiten in Partner Center navigieren, wird die Datei heruntergeladen, sobald die Exportfunktion abgeschlossen ist.
- Sie können die heruntergeladene Datei wiederverwenden, um die Dealdetails zu ändern, und hochladen, um Datensätze zu aktualisieren.

## <a name="import-co-sell-opportunities"></a>Importieren von Co-Selling-Verkaufschancen

- Sie können mithilfe der Importfunktion **maximal 1.000 Datensätze** erstellen oder aktualisieren.
- Sie können die Vorlage von Grund auf neu erstellen, indem Sie sie auf der Seite Importieren auf Partner Center herunterladen.
- Sie können auch die Exportfunktion verwenden, um die vorhandenen Datensätze herunterzuladen und zu aktualisieren.
- Wenn die Datei mehr als 1.000 Datensätze enthält, kann sie nicht verarbeitet werden.
- Nachdem die Datei verarbeitet wurde, wird eine Zusammenfassung mit der Anzahl der Empfehlungen, die erstellt, aktualisiert und nicht verarbeitet wurden, auf der Letzten Prozessdateikarte angezeigt.
- Sie können die Details der verarbeiteten Datensätze herunterladen, Fehler beheben und dieselbe Datei hochladen, um die Datensätze zu erstellen oder zu aktualisieren, die bei der vorherigen Ausführung fehlgeschlagen sind. **Entfernen Sie alle erfolgreichen Datensätze aus der Datei, bevor Sie die korrigierten Datensätze hochladen, bei denen bei der vorherigen Ausführung ein Fehler aufgetreten ist.**
- Um weitere Lösungen hinzuzufügen, fügen Sie zusätzliche Spalten neben Lösung 1 hinzu, und verwenden Sie den Spaltennamen als Projektmappe X, wobei X die Nummer der Lösung im Deal darstellt. Beispiel: Lösung 2, Lösung 3.
- Sie können einem Deal bis zu 50 Lösungen hinzufügen.
- Um weitere Teammitglieder hinzuzufügen, fügen Sie zusätzliche Spalten neben Teammitglied 1 hinzu, und verwenden Sie den Spaltennamen als Teammitglied X, wobei X die Nummer des Teammitglieds im Deal darstellt. Beispiel: Teammitglied 2, Teammitglied 3.
- Sie können einem Deal bis zu 50 Teammitglieder hinzufügen.

> [!NOTE]
> Sie müssen nicht warten, bis die Verarbeitung abgeschlossen ist. Die Details der zuletzt verarbeiteten Datei können heruntergeladen werden, sobald die Verarbeitung abgeschlossen ist. **Es kann bis zu 10 Minuten dauern, wenn Sie Dateien mit 1000 Datensätzen hochladen.**

> [!IMPORTANT]
> Lesen Sie alle Anweisungen sorgfältig durch, und überprüfen Sie das Format der einzelnen Spalten aus der folgenden Tabelle, bevor Sie Deals mithilfe von CSV-Dateien in Partner Center.

|**Spaltenname**|**Ist obligatorisch?**|**Beschreibung**|**Beispielwerte**|
|-----|:-----|:---------|:---|
Errors|Nein|Fehler im Zusammenhang mit den Erstellungs-/Aktualisierungsvorgängen w.r.t zu den Empfehlungen werden in dieser Spalte enthalten sein. Wenn mehrere Fehler auftreten, werden alle durch ein Semikolon getrennt aufgelistet.|Pflichtfeld Lösung 1 fehlt|
Engagement-ID|Nein|Die Engagement-ID wird vom Microsoft Partner Center-Empfehlungssystem generiert. Für die Erstellung neuer Empfehlungen nicht erforderlich. Sie können die vorhandene Engagement-ID verwenden, wenn Sie einen Datensatz aktualisieren.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Empfehlungs-ID|Nein|Die Empfehlungs-ID wird vom Microsoft Partner Center-Empfehlungssystem generiert. Für die Erstellung neuer Empfehlungen nicht erforderlich. Geben Sie die Empfehlungs-ID ein, wenn Sie einen vorhandenen Datensatz aktualisieren.|csdkdc-0b84-4ac4-b4ea-5b2587d42cee
DealName|Ja|Der Benutzername für den Deal als Referenz.|Uk spring deal
Customer Name|Ja|Name des Kundenunternehmens. Verwenden Sie den rechtlichen Namen der Organisation für den schnellen Abgleich auf Microsoft-Seite.|Contoso Corporation
Kundenadressenzeile 1|Ja|Adresszeile 1 des Kundenunternehmens. |One Contoso Way
Kundenadressenzeile 2|Nein|Adresszeile 2 des Kundenunternehmens.|NE 148 Street
Kundenort|Ja|Ort, in dem sich die Kundenorganisation befindet.|Redmond
Bundesland/Kanton des Kunden|Nein|Geben Sie an, wo sich die Kundenorganisation befindet.|Washington
Postleitzahl des Kunden|Nein|Postleitzahl der Region, in der sich die Kundenorganisation befindet.|98052
Land des Kunden|Ja|Land/Region, in dem sich die Kundenorganisation befindet. Verwenden Sie die zweistelligen Ländercodes, wie [hier]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)erwähnt.|US
D-U-N-S-ID des Kunden|Nein|Versuchen Sie, die DUNS-ID der Kundenorganisation abzurufen. Dies hilft bei der schnelleren Abstimmung der Kundenorganisation auf Microsoft-Seite, was eine schnellere Verkäuferzuweisung unterstützt. Sie können die DUNS-ID kostenlos von dieser [Website](https://www.dnb.com/duns-number/lookup.html)abrufen.|81466849
Vorname des Kundenkontakts|Depends (Abhängig)|Der Vorname ist nur obligatorisch, wenn Sie Microsoft-Hilfe benötigen. Der Vorname des primären Kontakts aus der Kundenorganisation, die an diesem Deal arbeitet.|John
Nachname des Kundenkontakts|Depends (Abhängig)|Der Nachname ist nur obligatorisch, wenn Sie Microsoft-Hilfe benötigen. Nachname des primären Kontakts aus der Kundenorganisation, die an diesem Deal arbeitet.|Kunde
Telefonnummer des Kundenkontakts|Depends (Abhängig)|Die Telefonnummer ist nur obligatorisch, wenn Sie Microsoft-Hilfe benötigen. Telefonnummer des primären Kontakts der Kundenorganisation, die an diesem Deal arbeitet.|9999999999
E-Mail-Adresse des Kundenkontakts|Depends (Abhängig)|Die E-Mail-Adresse ist nur obligatorisch, wenn Sie Microsoft-Hilfe benötigen. E-Mail-Adresse des primären Kontakts der Kundenorganisation, die an diesem Deal arbeitet.|john.customer@contoso.com
Partnerempfehlungsstatus|Ja|Gibt den Status des Deal aus Sicht Ihres Unternehmens an. Erforderlich, wenn Sie versuchen, eine Empfehlung zu erstellen oder zu ändern. Verwenden **Sie Neu,** wenn Sie versuchen, einen neuen Deal zu erstellen. Akzeptierte Werte sind hier [dokumentiert.](/partner/develop/referral-resources#referralstatus)|Aktiv
Partner Referral Substatus|Ja|Gibt den genauen Status des Deal an. Verwenden **Sie Akzeptiert,** wenn Sie versuchen, einen neuen Deal zu erstellen. Dies ist auch erforderlich, wenn Sie eine vorhandene Empfehlung ändern. Akzeptierte Werte sind hier [dokumentiert.](/partner/develop/referral-resources#referralsubstatus)|Akzeptiert
Microsoft-Empfehlungsstatus|Depends (Abhängig)|Gibt den Status der Co-Selling-Anforderung an, die Sie an Microsoft gesendet haben, um Hilfe zu erhalten. Dieses Feld ist schreibgeschützt. Alle Änderungen, die beim Importieren der Daten an diesem Feld vorgenommen werden, werden ignoriert.| Ausstehend
Abgelehnte/verlorene Ursache|Depends (Abhängig)| Sie müssen diese Informationen nur angeben, wenn Sie den Unterstatus Ihres Felds in Abgelehnt oder Verloren ändern. Sie können diese Spalte andernfalls ignorieren. <br/> **Geben Sie basierend auf den folgenden Optionen eine Zahl ein.** <br/><br/> **1–** Projektbudget ist nicht ausreichend  <br/> **2**– Kunde hat nicht reagiert  <br/> **3–** Kunde hat einen anderen Anbieter ausgewählt  <br/> **4–** Kundenanforderung nicht erfüllt  <br/> **5 –** Kein Kunde <br/> **6.** Vorgeschlagene Zeitlinie war zu kurz <br/> **7:** Melden als Missbrauch, Spam oder Phishing <br/> **8** – Andere |6|
Sales Stage|Nein|Dies ist das Feld, in dem die detaillierte Verkaufsphase der Empfehlung angegeben wird. Weitere Informationen zu Vertriebsphasen finden Sie [hier.](./manage-co-sell-opportunities.md)|40
Geschätzter Dealwert|Ja|Der Wert des Geschäfts, der auf den ersten Konversationen mit dem Kunden basiert. Dies kann geändert werden, bis der Deal einen der Terminalzustände **gewonnen** oder **verloren hat.**|12563
Währung|Ja|Die Währung, in der der Dealwert eingegeben wird. Die Währungscodes finden Sie [hier.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Geschätztes Schließdatum|Ja|Das geschätzte Abschlussdatum des Geschäfts basierend auf den ersten Konversationen mit dem Kunden im Format MM/TT/YYYY. <br/> **Das Datum sollte in der UTC-Zeitzone liegen. Alle Datumsangaben, die auf Partner Center Benutzeroberfläche angezeigt werden, basieren auf lokalisierten Zeitzonen. Möglicherweise gibt es einen Tag Unterschied in der Partner Center Ui, wenn Sie sich die Empfehlung ansehen, für die Sie das Datum in der UTC-Zeitzone angegeben haben.**|1/30/2020
CRM-ID|Nein|Bezeichner dieser spezifischen Empfehlung in Ihrem CRM-System, falls vorhanden. Dies ist ein Freiformtexteingabefeld.|34234324-sdfsdf-345345-sfd
Marketingkampagnen-ID|Nein|Dieses Feld gibt die Marketingkampagne an, die zu dieser spezifischen Empfehlung geführt hat. Wird in der Regel für die ROI-Berechnung verwendet.|BingSummer2020
Notizen|Nein|Ausführliche Hinweise, die die Aktualisierungen im Zusammenhang mit der Empfehlung angeben|Dies ist ein Beispielhinweis.
Microsoft-Hilfe erforderlich?|Ja|Dies bedeutet, dass Sie angeben möchten, ob Microsoft Ihnen bei der Erstellung dieser Co-Selling-Anforderung helfen soll.|Ja
Welche spezifische Hilfe von Microsoft?|Depends (Abhängig)|Eine der sechs verschiedenen Möglichkeiten, mit denen Microsoft Sie unterstützen kann. Dies gilt nur, wenn Sie ja für die Frage "Microsoft-Hilfe erforderlich? auswählen. " <br/> **Geben Sie basierend auf den folgenden Optionen eine Zahl ein.** <br/><br/> **1–** Workload – spezifisches Wertversprechen  <br/> **2–** Technische Architektur des Kunden  <br/> **3–** Proof of Concept /Demo  <br/> **4:** Anführungszeichen und Lizenzierung  <br/> **5**– Post – Kundenerfolg im Vertrieb  <br/> **6–** Allgemein oder sonstige|1|
Freigeben für das Microsoft-Vertriebsteam|Ja|Dies soll angeben, ob Sie die Details des Deals mit dem Microsoft-Vertriebsteam teilen möchten oder nicht. Dies gilt nur, wenn Sie nein für die Frage "Microsoft-Hilfe erforderlich? auswählen. "|Ja
Hinweise für Microsoft|Nein|Alle spezifischen Hinweise für Microsoft, wenn Sie Hilfe von Microsoft benötigen|Benötigen Sie Hilfe bei einem POC für den Contoso-Kunden
Zustimmung zur Freigabe des Kunden-/Partnerkontakts|Ja|Stimmen Sie der Freigabe von Kundenkontaktdetails zu, und wenden Sie sich an die Kontaktdetails Ihrer Unternehmensmitarbeiter, die an dem Deal arbeiten. **Angebote werden nicht erstellt oder aktualisiert, wenn Sie für diese Spalte Nein auswählen.** |Ja
Lösung 1|Ja|Lösungs-ID (erforderlich), Die Währung (optional), in die der Dealwert eingegeben wird. Die Währungscodes finden Sie [hier,](https://en.wikipedia.org/wiki/ISO_4217)Preis der SKU (optional) und Menge der SKU (optional).  |SOL-1234-PQRS, USD, 10, 100
Teammitglied 1|Ja|Vorname, Nachname, Mobiltelefonnummer und E-Mail-ID des jeweiligen Teammitglieds.| Bob, Partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Nächste Schritte

Sie können diese Partner Center Co-Sell-Connectors verwenden, um in Ihren CRM-Systemen co-sell mit Microsoft zu verkaufen.

- [Co-Sell-Connector für Dynamics 365 CRM – Übersicht](connector-dynamics.md)
- [Co-Selling-Connector für Salesforce CRM – Übersicht](connector-salesforce.md)
