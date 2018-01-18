---
title: "Häufig gestellte Fragen zu neuen Abrechnungsfunktionen | Partner Center"
Description: The following are frequently asked questions about Partner Center's annual billing and free trial features.
ms.assetid: 
author: MaggiePucciEvans
ms.openlocfilehash: ddd10efe487effdd2571869f2a4231118f946b8b
ms.sourcegitcommit: 4b697e2e18426edc95b9165f380b784bb10937ed
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2017
---
# <a name="faq-about-new-billing-features"></a>Häufig gestellte Fragen zu neuen Abrechnungsfunktionen

**Betrifft:**

-  Partner Center
-  Partner Center für Microsoft Cloud für US-Behörden
-  Partner Center für Microsoft Cloud Deutschland

Im folgende sind häufig gestellte Fragen zur jährlichen Abrechnung und kostenlose Testphase von Partner Center aufgeführt. 

## <a name="in-this-section"></a>In diesem Abschnitt

-   [Jährliche Abrechnung – häufig gestellte Fragen](#annualbillingfaq)

-   [Kostenlose Testversionen – häufig gestellte Fragen](#freetrialsfaq)

-   [Rechnungsanpassung – häufig gestellte Fragen](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Jährliche Abrechnung – häufig gestellte Fragen

Abschnitte:

[Übersicht und Vorteile der jährlichen Abrechnung](#overviewandbenefits)

[Bestellungs- und Abrechnungsszenarien](#placingyourorder)

[Abonnement wechseln](#changingyoursubscription)

[Preisberechnung](#pricingcalculation)

[Berichterstellung](#reporting)

[Vorteile](#incentives)


<a href="" id="overviewandbenefits"></a>**Übersicht und Vorteile der jährlichen Abrechnung**

**F:** Was hat sich geändert?

-   **A:** Als Reaktion auf Ihre Anfragen haben wir die Option zum Bezahlen von bestimmten CSP-Abonnements auf monatlicher oder jährlicher Basis eingeführt. Diese neue Option ist seit dem 17. Oktober 2017 verfügbar.

**F:** Wer kann daran teilnehmen?

-   **A:** Alle Partner und Partnertypen können die jährliche Abrechnung verwenden. Die jährliche Abrechnung ist in allen Märkten verfügbar, in denen CSP derzeit verfügbar ist. 

**F:** Was muss ich berücksichtigen, wenn ich die jährliche Abrechnung verwenden möchte?    

-   **A: **Sie sollten berücksichtigen, wie dies ihren Verkaufsvorgang beeinträchtigt. Hier einige Tipps zur effektiven Nutzung der jährlichen Abrechnung. 
    - Aktualisieren Sie APIs, um ggf. der jährlichen Abrechnungsfunktion gerecht zu werden. 
    - Überprüfen Sie die Änderungen an der Rechnung und der lizenzbasierten Abstimmungsdatei.
    - Stellen Sie sicher, dass Ihr Team darüber informiert wird.
    - Aktualisieren Sie Ihre interne Prozesse nach Bedarf.

**F:** Welche Vorteile bietet die jährliche Abrechnung? 

-   **A:** Eine jährliche Abrechnung bietet folgende Vorteile:

    - Verbesserte Flexibilität im Hinblick auf Zahlungsoptionen.

    - Bessere Übereinstimmung mit der Fakturierung Ihrer Kunden.

    - Weniger Einfluss der Währungsfluktuationen.

    - Reduzierte Betriebskosten bei der Abrechnung.

**F:** Welche Angebote sind für die jährliche Abrechnung berechtigt?

-   **A:** Die meisten lizenzbasierten Abonnements können monatlich oder jährlich abgerechnet werden. Für nutzungsbasierte Abonnements ist nur die monatliche Abrechnung verfügbar. In Spalte J der Angebotsmatrix finden sie den verfügbaren Abrechnungszeitrum für jedes Angebot. Die Angebotsmatrix finden Sie im Abschnitt „Anzeigen von Angeboten und Preisen” im Partner Center. .

**F:** Erfolgt die jährliche Abrechnung pro Abonnement oder pro Lizenz?       

-   **A:** Sowohl die jährliche als auch die monatliche Abrechnung erfolgt pro Abonnement.

**F:** Gibt es zur Unterstützung der jährlichen Abrechnung Änderungen an den APIs?    

-   **A:** Zur Nutzung der jährliche Abrechnung sind einige Änderungen an Ihren APIs erforderlich. Weitere Informationen finden Sie in den folgenden Artikeln:

    - https://partnercenter.microsoft.com/de-de/partner/developer

    - https://msdn.microsoft.com/en-us/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Beispielcode: https://msdn.microsoft.com/en-us/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Bestellungs- und Abrechnungsszenarien**

**F:** Gibt es spezielle Angebote für Aufträge mit jährlicher Abrechnung?   

-   **A:** Nein. Alle Abrechnungshäufigkeiten, einschließlich der jährlichen Abrechnungsoption, werden dem Angebot als Attribut zugewiesen. Sie können allerdings ein Angebot zur Differenzierung umbenennen und einen benutzerfreundlichen Namen verwenden.

**F:** Wie wähle ich die jährliche Abrechnung aus?

-   **A:** Wenn Sie ein neues Abonnement hinzufügen, werden Sie aufgefordert, die Abrechnungshäufigkeit auszuwählen. Dabei können Sie die Option für jährliche Abrechnung auswählen. Nach dem Auswählen der jährlichen Abrechnung werden alle verfügbaren Angebote angezeigt.

**F:** Wenn ich mich für die jährliche Abrechnung entscheide, wann erfolgt die Abrechnung?    

-   **A:** Die Abrechnung erfolgt am folgenden Rechnungsdatum. Wenn beispielsweise Ihr Abrechnungsdatum der 1. Februar ist, erfolgt die Abrechnung immer am 1. Februar. Wenn Sie also ein jährlich abgerechnetes Abonnement am 29. Oktober 2017 oder am 15. Januar 2018 erwerben, wird Ihnen in beiden Fällen ein Jahresabonnement ab dem 1. Februar 2018 in Rechnung gestellt. 

**F:** Kann ich ein Abonnement so aufteilen, dass ein Teil monatlich und der andere jährlich abgerechnet wird?  

-   **A:** Nein. Für das gesamte Abonnement muss derselbe Abrechnungszeitraum gelten. Das gesamte Abonnement muss entweder monatlich oder jährlich abgerechnet werden.

**F:** Wann erfolgt die Verlängerung für ein Abonnement mit Jahresabrechnung?     

-   **A:** Das Verlängerungsdatum liegt zwölf Monate nach dem Startdatum des Diensts. Der Dienstzeitraum beginnt mit dem Datum, an dem das Abonnement abgeschlossen wird.  Beispielsweise wird ein am 10. Januar 2018 abgeschlossenes Abonnement am 10. Januar 2019 verlängert.

**F:** Wann wird mir die Verlängerung eines Abonnements mit jährlicher Abrechnung in Rechnung gestellt? 

-   **A:** Die Abrechnung erfolgt am nächsten Rechnungsdatum nach dem Verlängerungsdatum des Abonnements. Wenn Sie ein jährlich in Rechnung gestelltes Abonnement am 15.Januar2018 erwerben und Ihr Abrechnungsdatum der 20.Januar ist, wird Ihr Abonnement am 15.Januar2019 verlängert. Die Verlängerung wird am 20.Januar 2019 in Rechnung gestellt.

**F:** Erhalten Abonnements mit jährlicher Abrechnung einen „kostenlosen Zeitraum”?

-   **A: **Nein, Abonnement mit jährlicher Abrechnungsfrequenz erhalten keinen „kostenlosen Zeitraum”. Der kostenpflichtige 12-Monats-Zahlungszeitraum beginnt mit dem Kaufdatum. Dies ist anders als bei Abonnements mit monatlicher Abrechnung, die nach dem Kauf einen „kostenlosen Zeitraum” bis zum nächsten Abrechnungsdatum erhalten.

**F:** Kann ein Kunde mehrere Abonnements für das gleiche Angebot mit unterschiedlichen Abrechnungsintervallen besitzen?    

-   **A:** Das hängt vom Angebot ab. Bestimmte Angebote sind auf ein Abonnement pro Kunde beschränkt. Wenn das Angebot nicht beschränkt ist, kann ein Kunde mehrere Abonnements für das gleiche Angebot mit unterschiedlichen Abrechnungsintervallen besitzen. Die Details für alle Angebotseinschränkungen finden Sie in der Spalte I der Angebotsmatrix. Die Angebotsmatrix finden Sie im Abschnitt „Anzeigen von Angeboten und Preisen” im Partner Center.

<a href="" id="changingyoursubscription"></a>**Abonnement wechseln**

**F:** Kann ich eine neue Lizenz zu einem vorhandenen Abonnement mit jährlicher Abrechnung hinzufügen?    

-   **A:** Ja. Sie können die Anzahl der Lizenzen für Ihre Abonnements jederzeit ändern. Das Hinzufügen von zusätzlichen Lizenzen wirkt sich nicht auf die Abrechnungshäufigkeit aus. 

**F:**Kann ich Lizenzen mit monatlicher Abrechnung zu einem vorhandenen Abonnement mit jährlicher Abrechnung hinzufügen? 

-   **A:** Nach dem Kauf eines Abonnement mit jährlicher Abrechnung gilt dieser Abrechnungsrhythmus für alle zusätzlichen Lizenzen. Wenn Sie Lizenzen mit einem monatlichen Abonnement benötigen, müssen Sie ein neues Abonnement kaufen.

**F:** Kann ich zwischen einem monatlichen und einem jährlichen Abrechnungsintervall für ein Abonnement (und umgekehrt) wechseln? 

-   **A:** Nein. Nachdem Sie das Abrechnungsintervall ausgewählt haben, können Sie dieses nicht mehr ändern. 

**F:** Steht die jährliche Abrechnung für Add-On-Angebote zur Verfügung?   

-   **A:** Ja. Das Add-On-Abonnement erhält das gleiche Abrechnungsintervall wie das übergeordnete Abonnement.

**F:** Wie funktioniert die jährliche Abrechnung, wenn ich Lizenzen hinzufügen oder entfernen möchte? 

-   **A:** Sie können Lizenzen jederzeit hinzufügen oder entfernen. Nach dem Ändern der Anzahl der Lizenzen erhalten Sie am nächsten Rechnungsdatum eine Gutschrift und eine anteilige Rückbuchung. 

**F:** Was geschieht, wenn ich ein Abonnement mit jährliche Abrechnung kündige?    

-   **A:** Die Kündigungsbedingungen sind für alle Abrechnungsintervalle identisch. Wenn das Abonnement in den ersten 30Tagen des kostenpflichtigen 12-Monats-Zahlungszeitraums abgebrochen wird, erhalten Sie eine Erstattung von 100 Prozent zum nächsten Abrechnungsdatum. Wenn das Abonnement nach 30Tagen des kostenpflichtigen 12-Monats-Zahlungszeitraums abgebrochen wird, erhalten Sie eine anteilige Gutschrift für das nächste Abrechnungsdatum.

**F:** Kann ein Kunde ein Abonnement mit jährlicher Abrechnung von einem Partner auf einen anderen übertragen?  

-   **A:** Nein. Abonnements können nicht zwischen Partnern übertagen werden. Der neue Partner muss im Auftrag des Kunden ein neues Abonnement erwerben. Dies gilt für monatlich und jährlich in Rechnung gestellte Abonnements.

**F:** Kann ich ein Abonnement mit einer jährlichen Abrechnung neu aktivieren?

-   **A:** Ja, Sie haben ab dem Datum der Stornierung 90 Tage Zeit, das Abonnement wieder zu aktivieren. Die anteilige Abrechnung erfolgt am folgenden Rechnungsdatum. Das Verlängerungsdatum des Abonnements bleibt unverändert.

<a href="" id="pricingcalculation"></a>**Preisberechnung**

**F:** Was geschieht, wenn ein Angebotspreis für ein jährlich in Rechnung gestelltes Abonnements während der 12-monatigen Abonnementdauer geändert wird?    

-   **A:** Der Angebotspreis zum Zeitpunkt des Kaufs ist für die 12-monatige Laufzeit des Abonnements garantiert. 

**F:** Welcher Preis gilt für ein Abonnement, wenn es nach 12 Monaten automatisch erneuert wird?    

-   **A:** Wenn ein Abonnement erneuert wird, gilt der Preis in der aktuellen Preisliste zum Zeitpunkt der Verlängerung. Der neue Preis ist für den nächsten 12-monatigen Abonnementzeitraum garantiert.

**F:** Wie wird die Gutschrift für die Stornierung einer Lizenz oder eines Abonnements ermittelt? Wird sie pro Tag oder pro Monat berechnet?   

-   **A:** Ein Stornierungsguthaben wird wie folgt berechnet:

    - Stornierungsguthaben = ((Monatspreis*12)/365) * verbleibende Tage im 12-monatlichen Abozeitraum * Anzahl der stornierten Lizenzen

**F:** Was geschieht, wenn ein Angebotspreis während der 12-monatigen Laufzeit eines jährlich in Rechnung gestellten Abonnements gesenkt wird? 

-   **A:** Eine Änderung findet nicht statt. Der Preis gilt für den gesamten 12-monatigen Zeitraum. Dies entspricht der monatlichen Abrechnung.


<a href="" id="reporting"></a>**Berichterstellung**

**F:** Wo finde ich heraus, ob ein Abonnement jährlich oder monatlich abgerechnet wird?   

-   **A:** Die lizenzbasierte Abstimmungsdatei enthält die Abrechnungshäufigkeit. Sie finden sie in Spalte AA.

**F:** Welche Änderungen enthält die lizenzbasierte Abstimmungsdatei, wenn ein Abonnement mit jährlicher Abrechnung erworben oder erneuert wird?  

-   **A:** Die erste Änderung ist eine neue Zeile in der lizenzbasierten Abstimmungsdatei am ersten Rechnungsdatum mit dem Kauf oder einem neuen Abonnement. ein. Wenn keine Änderungen am Abonnement vorgenommen wurden, enthält die Abstimmungsdatei keine Zeilen für die Monate zwei bis zwölf des Abonnementzeitraums. Die nächste Änderung der Abstimmungsdatei erfolgt, wenn das Abonnement erneuert wird. Die Änderung wird am ersten Abrechnungsdatum nach der Verlängerung angezeigt. Wenn während der 12-monatigen Laufzeit eine Änderung am Abonnement vorgenommen wird, erscheint nach der Änderung eine Gutschrift und eine anteilige Rückbuchung in der nächsten Abstimmungsdatei.

**F:** Wie werden Kauf, Änderung oder Stornierung eines Jahresabonnements in Spalte P der Nutzungsdateien angezeigt?

-   **A:** Die anfängliche Gebühr wird als „Anteilige Gebühren bei Erwerb” angezeigt. Lizenzänderungen, die zur Gutschrift und Neuberechnung führen, werden als „Anteilige Zyklusinstanz” angezeigt. Stornierungsgutschriften werden als „Stornierungsgebühr” angezeigt.

**F:** Was wird in der Abstimmungsdatei angezeigt, wenn ein Jahresabonnement storniert wird?   

-   **A:** Die Abstimmungsdatei enthält ein Positionselement für die Gutschrift der Kündigung. Wird das Abonnement in den ersten 30 Tagen des 12-monatigen Abonnementzeitraums storniert, wird es zu 100 Prozent gutgeschrieben. Wird das Abonnement nach den ersten 30Tagen storniert, wird der anteilige Betrag gutgeschrieben

**F:** Was wird in der Abstimmungsdatei angezeigt, wenn Lizenzen zu einem Abonnement mit jährlicher Abrechnung hinzugefügt werden?  

-   **A:** Die Abstimmungsdatei enthält eine Gutschrift und eine anteilige Rückbuchung. Dies gilt auch für ein Abonnement mit monatlicher Abrechnung.

**F:** Was wird in der Abstimmungsdatei angezeigt, wenn Lizenzen aus einem Abonnement mit jährlicher Abrechnung entfernt werden? 

-   **A:** Die Abstimmungsdatei enthält eine Gutschrift und eine anteilige Rückbuchung.  Dies gilt auch für ein Abonnement mit monatlicher Abrechnung.

**F:** Wird der jährliche Preis in der Preisliste angezeigt? 

-   **A:** Nein. Die Preisliste enthält den monatlichen Preis. Sie können die jährlichen Preis berechnen, indem Sie den monatlichen Preis mit zwölf multiplizieren.

**F:** Enthält die Angebotsmatrix unterschiedliche Einträge für Angebote, die jährlich in Rechnung gestellt werden können?   

-   **A:**  Nein. Der Angebots-IDs sind für alle Abrechnungsperioden identisch. Es gibt keine speziellen Angebots-IDs für jährliche Abrechnung.


<a href="" id="incentives"></a>**Anreize (Incentives)**

**F:** Wie oft werden Incentives für Jahresabonnements berechnet? 

-   **A:** Wir rechnen mit dem fakturierten Umsatz. Erzielte Incentive-Zahlungen werden im Einklang mit unserer Richtlinien gezahlt, wie in den CSP-Handbüchern für Incentives aufgeführt. 

**F:** Wie werden die Incentives für jährlich abgerechnete Abonnements bezahlt?  

-   **A:** Derzeit erfolgen alle Incentive-Zahlungen zweimal pro Jahr. Diese Zahlungen erfolgen 45 Tage nach Semesterende.

**F:** Wenn ein jährlich abgerechnetes Abonnement verkauft wird, wie werden die Einnahmen dieses Abonnements für die Berechnung der Incentives verbucht? Erfolgt die Berechnung auf der Grundlage von fakturierten oder angepassten Erlösen? 

-   **A:** Incentive-Berechnungen basieren auf dem in Rechnung gestellten Umsatz.

**F:** Wie werden die Incentive-Einnahmen für das förderfähige jährlich abgerechnete Abonnement bezüglich der verschiedenen CSP-Incentive-Raten (globale Incentive-Raten, lokale Beschleunigungsraten und lokale Kampagnen) berechnet?

-   **A:** Unabhängig davon, wie ein Abonnement abgerechnet wird, ob monatlich oder jährlich, erhalten die Partner Incentives für alle zulässigen Transaktionen. Dazu gehören die globale Incentive-Rate, die auf den fakturierten Umsatz der Periode angewendet wird, der lokale Beschleuniger für alle Regionen, in denen es lokale Beschleuniger gibt, und ggf. globale Kampagnen.

**F:** An wen können Sie sich bei Fragen zu Incentives wenden?

-   **A:** Wenden Sie sich an das jeweilige regionale Supportteam für Incentives.

    - Nordamerika: ocina@microsoft.com

    - Lateinamerika & Brasilien: ocilatam@microsoft.com

    - EMEA: ociemea@microsoft.com

    - APOAC (ausgenommen Japan): ociapgc@microsoft.com

    - Japan: ocijp@microsoft.com


**F:** Was geschieht, wenn ich mein Abonnement storniere? 

-   **A:** Wenn Sie ein Abonnement entweder im Partner Center oder über API innerhalb von 30Tagen nach dem Kauf anhalten, erhalten Sie eine Erstattung von 100%, unabhängig von der Abrechnungsfrequenz. 

    Mit einer jährlichen Abrechnung würde es wie folgt aussehen:

    - Der Partner kauft ein Abonnement am 1.Januar = Rechnungsposition der Gebühr für den Aktivierungszeitraum 1.1 – 31.12.
    - Der Partner kauft ein Abonnement am 1.Januar = Rechnungsposition der Gebühr für den Aktivierungszeitraum 01.01 – 31.12.
    - Der Partner kauft ein Abonnement am 1.Januar = Rechnungsposition der Gebühr für den Aktivierungszeitraum 29.01 – 31.12.

    Mit einer monatlichen Abrechnung würde es wie folgt aussehen:

    - Der Partner kauft ein Abonnement am 1.Januar = Rechnungsposition der Gebühr für den Aktivierungszeitraum 1.1 – 31.12.
    - Der Partner kauft ein Abonnement am 1.Januar = Rechnungsposition der Gebühr für den Aktivierungszeitraum 01.01 – 31.12.
    - Der Partner kauft ein Abonnement am 1.Januar = Rechnungsposition der Gebühr für den Aktivierungszeitraum 29.01 – 31.01.



## <a href="" id="freetrialsfaq"></a>FAQ zu kostenlosen Testversionen

**F:** Was sind kostenlose Testversionen?

-   **A:** Sie können Ihren Kunden eine 30-tägige kostenlose Testversion von bestimmten Produkten anbieten. Dadurch können Ihre Kunden das Produkt vor dem Kauf bewerten. Kostenlose Testversionen sind für folgende Produkte verfügbar: 

    - Office 365 Business Premium  
    - Office 365 E3  
    - Office 365 E5 mit PSTN  
    - Office 365 E5 ohne PSTN  
    - Enterprise Mobility & Security E5  
    - Dynamics 365 Customer Engagement Plan 1  
    - Dynamics 365 for Financials  
    
**F:** Wird die kostenlose Testphase durch die Bereitstellung einer kostenlosen Testversionen entfernt?

-   **A:** Nein, Abonnements mit monatlicher Rechnung erhalten auch weiterhin einen „kostenlosen Zeitraum”. Es steht jedoch kein kostenloser Zeitraum für die jährliche Abrechnung zur Verfügung.

**F:** Die Abrechnungsanpassung wird bis zum ersten Quartal des Geschäftsjahrs 2018 verzögert. Wie wirkt sich dies auf den kostenlosen Zeitraum und die Abrechnung im Allgemeinen aus?

-   **A:** Neue Abonnements mit monatlichen Abrechnungen erhalten auch weiterhin eine Rechnung und werden am Abrechnungsdatum des Partners ausgerichtet. Abonnements mit jährlicher Abrechnung bieten diesen kostenlosen nicht an und sind am Kaufdatum ausgerichtet. Partner erhalten auch weiterhin ihre Rechnung und Erstattungsdateien an ihrem monatlichem Abrechnungsdatum, das die Abrechnungsaktivität für die monatlichen und jährlichen Abonnements enthält.

**F:** Wann wird die kostenlose Testphase für Abonnements mit monatlicher Abrechnungsfrequenz entfernt?

-   **A:** im ersten Quartal des Geschäftsjahrs 2018.

**F:** Sind jährliche Abrechnungen und kostenlose Testphasen unterschiedliche in der unabhängiger Cloud im Vergleich zur öffentlichen Cloud?

-   **A:** Nein. Sie sind identisch. Der einzige Unterschied liegt in den Testversions-SKUs, die zum Zeitpunkt des Starts verfügbar sind.

**F:** Wenn wird dies für die oben aufgeführten SKUs verfügbar sein?

-   **A:** 17. Oktober 2017.

**F:** Wer kann teilnehmen?

-   **A:** Alle Partner können teilnehmen. Allerdings sind in China derzeit keine Testversionen verfügbar. Die kostenlosen Testversionen stehen für chinesische Partner und Kunden Ende 2017 zur Verfügung. 

**F:** Was muss ich unternehmen, um von diesen kostenlosen Testversionen profitieren zu können?

-   **A:** Überlegen Sie, wie die kostenlose Testversion in Ihren Verkaufsprozess integriert werden kann und welchen Einfluss sie auf interne Vorgänge hat. Sie müssen außerdem möglicherweise die APIs ändern, um die Umwandlung einer kostenlosen Testversion in ein kostenpflichtiges Abonnement zu ermöglichen. Im Ankündigungsbereich des Partner Centers werden detaillierte technische Spezifikationen für diese API-Änderungen zur Verfügung gestellt.

**F:** Wird die kostenlose Testversion in meiner Rechnung und Abstimmungsdatei angezeigt?

-   **A:** Nein, die kostenlose Testversion wird nicht in Ihrer Rechnung oder der lizenzbasierten Abstimmungsdatei angezeigt. Erst nach der Umwandlung einer kostenlosen Testversion in ein kostenpflichtiges Abonnement erscheint sie auf Ihrer Rechnung und in der lizenzbasierten Abstimmungsdatei. Das konvertierte Abonnement wird in gleicher Weise wie jedes andere neue Abonnement in Ihrer Rechnung und der lizenzbasierten Abstimmungsdatei angezeigt. 

**F:** Hat die kostenlose Testversion Auswirkungen auf Incentives?

-   **A:** Nein. Die kostenlose Testversion hat keine Auswirkung auf Anreize.

**Q:** Werden kostenlose Testversionen für zusätzliche Office-Produkte und CSPs in Zukunft zur Verfügung gestellt?

-   **A:** Wir wissen es noch nicht. Wir bieten kostenlose Testversionen für diese Produkte an, da sie die umfassendsten und beliebtesten geschäftlichen Angebote sind. Wir werden in Zukunft möglicherweise weitere kostenlose Testangebote hinzufügen.

**F:** Kann ein Kunde mehr als eine kostenlose Testversion erhalten?

-   **A:** Jeder Kunde erhält eine kostenlose Testversion pro Angebot.

**F:** Gibt es Beschränkungen für eine kostenlose Testversion?

-   **A:** Ja. Die Testversion gilt für maximal 25 Lizenzen. Die Anzahl der Lizenzen kann während des Testzeitraums nicht geändert werden. Nachdem die Testversion in ein kostenpflichtiges Abonnement umgewandelt wurde, können Sie zusätzliche Lizenzen für das Abonnement hinzufügen.

**F:** Wird eine kostenlose Testversion automatisch in ein kostenpflichtiges Abonnement umgewandelt?

-   **A:** Nein. Sie müssen das Abonnement selbst umwandeln, entweder im Partner Center oder über die API.

**F:** Können kostenlose Testversionen sowohl für monatlich als auch für jährliche in Rechnung gestellte Abonnements verwendet werden?

-   **A:** Ja. Sie können die Abrechnungshäufigkeit auswählen, wenn Sie die Testversion in ein kostenpflichtiges Abonnement umwandeln.

**F:** Wird das Startdatum des Abonnements basierend auf dem Datum der kostenlosen Testversion bestimmt, oder basierend auf dem Datum, an dem es in ein kostenpflichtiges Abonnement umgewandelt wird? 

-   **A:** Das Startdatum basiert auf dem Datum der Konvertierung. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit jährlicher Abrechnung umgewandelt wird, ist zwölf Monate nach dem Datum der Umwandlung das Verlängerungsdatum erreicht. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit monatlicher Abrechnung umgewandelt, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem Verlängerungsdatum der Konvertierung.

**F:** Können während der kostenlosen Testphase Plätze hinzugefügt oder entfernt werden?

-   **A:** Nein. Kostenlose Testversionen umfassen standardmäßig 25Lizenzen und können nicht erhöht werden.

**F:** Gibt es Testversionen für Add-On-Angebote wie ATP und PSTN?

-   **A:** Es gibt keine kostenlosen Testversionen für Add-On-Angebote.

**F:** Kann ich eine Testphase für ein Angebot anbieten, das ein Kunde bereits besitzt?

-   **A:** Nein. Nein, wenn der Kunde das Angebot bereits besitzt kann, dafür keine kostenlose Testversion bereitgestellt werden.

**F:** Kann ich meine ausstehenden Testangebote anzeigen?

-   **A:** Ja. Auf der Kundenseite sind alle Abonnements aufgeführt. Es werden sowohl die kostenlosen Testabonnements als auch die kostenpflichtigen Abonnements angezeigt.

**F:** Werde ich über ablaufende kostenlose Testversionen benachrichtigt?

-   **A:** Nein. Sie können anstehende Ablaufdaten im Partner Center verfolgen oder die API zum Abrufen des Datums nutzen. Sie sollten diese Daten häufig überwachen, damit die entsprechende Transaktion zusammen mit dem Kunden durchgeführt werden kann.

**F:** Kann ein Kunde, der bereits eine kostenlose Testversion für ein Angebot besitzt, zusätzlich Testversionen für andere Angebote erhalten? 

-   **A:** Ja. Kunden können sich für ein Testabonnement pro Angebot registrieren. Sie können z.B. eine kostenlose Testversion für Office365 Business Premium und eine kostenlose Testversion für Office365 E3 erhalten.

**F:** Was geschieht, wenn die Testversion abläuft? Erhalten ich und der Kunde eine Benachrichtigung? Welche Benachrichtigungen werden angezeigt, wenn ich versuche, mich bei einer abgelaufenen Testversion anzumelden?

-   **A: **Nachdem die Testversion abgelaufen ist und der Kunde versucht, sich anzumelden, wird eine Nachricht auf der Testversion angezeigt, dass die Testversion abgelaufen ist. Es gibt keine Benachrichtigungen, dass die Testversion abläuft. Als Partner können dies allerdings über die Kundenansicht oder API-Abfragen nachverfolgen.

**F:** Kann eine Testversion verlängert werden?

-   **A:** Nein. Die Testversion muss entweder umgewandelt werden oder läuft nach 30 Tagen ab.

**Q:** Kann auf die Informationen der Testversion zugegriffen werden, wenn sie abgelaufen ist?

-   **A:** Ja. Die Informationen werden entsprechend den Standards für die Aufbewahrung von Daten gespeichert. Nachdem Sie ein neues Abonnement mit den gleichen Serviceplänen erworben haben, können Sie über das neu aktivierte Abonnement auf die Daten zugreifen.

**F:** Gibt es kostenlose Testversionen für Behörden und Bildungseinrichtungen?

-   **A:** Es gibt im Moment noch keine kostenlosen Testversionen für Behörden und Bildungseinrichtungen.

**F:** Können Testversionen für Kunden im Cloud Solution Provider (CSP)-Programm auf andere Programm-Mandanten wie EA, Open oder MOSP übertragen werden? 

-   **A:** Nein. Abonnements können nicht vom CSP auf andere Programme übertragen werden.

**F:** Wie erhalte ich Support für kostenlose Testversionen? 

-   **A:** Bitte übermitteln Sie eine Serviceanfrage über das Partner Center.

## <a href="" id="billingalignmentfaq"></a>Anpassung des Abrechnungsdatums – kein freier Zeitraum mehr

Am 20. Februar wird im CSP-Programm eine „Anpassung des Abrechnungsdatums” für neue Abonnements mit monatlicher Abrechnung implementiert. Diese „Anpassung des Abrechnungsdatums” wird den Partnern mehr Flexibilität und Vorhersagbarkeit für Vertrieb, Abrechnung, Bereitstellung und Verwaltung von Kundenabonnements bieten. Abonnements, die vor dem 20. Februar gekauft wurden, erhalten einen kostenlosen Zeitraum vom Kaufdatum bis zum Rechnungsdatum des Partners. Abonnements, die nach dem 20. Februar gekauft wurden, erhalten keinen kostenlosen Zeitraum mehr. Die 12-monatige Zahlungsfrist beginnt mit dem Kaufdatum auf der Partnerabrechnung. Partnern wird keine Rechnungszeile mehr mit einem Nullbetrag angezeigt, die den kostenlosen Zeitraum in der Abstimmungsdatei darstellt. Es gibt keine Änderungen an APIs, Fakturierung oder Incentives.  Partner sollten ihre Verkaufs- und Buchhaltungsteams über diese neue Abrechnungslogik informieren und sicherstellen, dass alle Vorgänge bei Bedarf angepasst werden.  

Vor der Anpassung des Abrechnungsdatums sind wir bei der Rechnungsstellung vom dem Datum ausgegangen, an dem der Partner dem CSP-Programm beigetreten ist, und nicht von dem Jahrestag, an dem der Kunde sein Abonnement erworben hat. Der daraus resultierende kostenlose Zeitraum entfällt nach dem 20. Februar, da die Abrechnung mit einem Partner ab dann auf dem Jahrestag seines Abonnements basiert.  Partner erhalten weiterhin Rechnungen zu ihrem Abrechnungsdatum, aber das effektive Rechnungsdatum wird der Jahrestag des Kundenabonnements sein. 

Abonnements, deren kostenloser Zeitraum den 20. Februar umfasst, werden im Zeitraum zwischen Kaufdatum und dem Abrechnungsdatum für den Partner nicht berechnet. Zudem sind sie im Monat 1 des 12-monatigen Abrechnungszeitraums kostenlos. Wenn Sie eine Abstimmungsdatei für die Überprüfung verwenden, beachten Sie, dass die Gebühren für diesen ersten Monat nicht mehr angezeigt werden.  


**F:** Was ändert sich?

-   **A:** Für lizenzbasierte Abonnements gibt es keinen kostenlosen Zeitraum mehr zwischen Kaufdatum und Rechnungsdatum des Partners.

**F:** Wann entfällt der kostenlose Zeitraum?

- **A:** Ab dem 20. Februar 2018 gibt es für neue Abonnements keinen freien Zeitraum mehr.

**F:** Sind Abonnements betroffen, deren kostenloser Zeitraum den 20. Februar 2018 umfasst?

- **A:** Der kostenlose Zeitraum wird bis zum Partnerabrechnungsdatum für Abonnements fortgesetzt, die sich bereits am 20. Februar 2018 im kostenlosen Zeitraum befinden. Zudem sind sie im Monat 1 des 12-monatigen Abrechnungszeitraums kostenlos. Wenn Sie die Abstimmungsdatei für die Überprüfung verwenden, beachten Sie, dass die Gebühren für diesen ersten Monat nicht mehr angezeigt werden. Die nachstehenden Szenarien enthalten eine genauere Beschreibung.

**F:** Wann beginnt der kostenpflichtig Zeitraum von 12 Monaten?

- **A:** Derzeit beginnt die bezahlte Periode an dem auf das Kaufdatum folgenden Partnerabrechnungsdatum. Nach Abschaffung des kostenlosen Zeitraums beginnt der bezahlte Zeitraum für neue Abonnements mit dem Kaufdatum.

**F:** Wann werden Abonnements automatisch verlängert?

- **A:** Derzeit verlängern sich Abonnements automatisch 12 Monate nach dem auf das Kaufdatum folgende Partnerabrechnungsdatum. Nach Abschaffung des kostenlosen Zeitraums verlängern sich Abonnements automatisch nach 12 Monaten ab dem Kaufdatum.

**F:** Was geschieht, wenn ich das Abonnement am 29., 30. oder 31. erwerbe?

- **A:** Das Abonnement wird ab Kaufdatum bereitgestellt, aber der kostenpflichtige 12-Monatszeitraum beginnt erst mit dem Folgemonat.

**F:** Welche Angebote sind von dieser Änderung betroffen?

- **A:** Es sind alle lizenzbasierten CSP-Abonnements betroffen.

**F:** Wie wirkt sich diese Änderung auf die Rechnung und die Abstimmungsdatei aus?

- **A:** Partnern wird keine Rechnungszeile mehr mit einem Nullbetrag angezeigt, die den kostenlosen Zeitraum in der Abstimmungsdatei darstellt.

**F:** Ändert sich mein Abrechnungsdatum?

- **A:** Nein, Sie erhalten die Rechnung und die Abstimmungsdatei weiterhin an Ihrem bisherigen Abrechnungsdatum.

**F:** Ändern sich das monatliche Anfangs- und Enddatum für bestehende Abonnements?

- **A:** Nein, das monatliche Anfangs- und Enddatum für bestehende Abonnements entspricht weiterhin Ihrem Abrechnungsdatum. Neue Abonnements werden jedoch nach dem Kaufdatum berechnet. Siehe Beispiel unten.

**F**: Ändert sich die Berechnung der Incentives?

- **A:** Nein.

**F:** Ändern sich die APIs?

- **A:** Nein.

### <a name="common-scenarios"></a>Häufige Szenarien


|**Szenarien**   |**Szenario 1: Der kostenlose Zeitraum des Abonnement endet vor dem 20. Februar 2018.**   |**Szenario 2: Der kostenlose Zeitraum des Abonnement umfasst den 20. Februar 2018.**  | **Szenario 3: Das Abonnement wurde am oder nach dem 20. Februar 2018 erworben.**   |
|----------|:------------|:--------------------|:------------|
|Kaufdatum |1. Februar    | 1. Februar    | 1. Juni     |
|Bereitstellungsdatum | 1. Februar   |1. Februar   |1. Juni   |
|Abrechnungsdatum   | 15   |25   | 15|
|Kostenloser Zeitraum   | 1. Februar – 15. Februar|1. Februar – 24. Februar   |Kein kostenloser Zeitraum|
|Gebühr für Monat 1   | 15.Februar – 14. März | 25.Februar2018 – 24.März2018 keine Belastung, nicht in Abstimmungsdatei aufgeführt|1.Juni – 30.Juni   |
|Gebühr für Monat 2   | 15.März – 14. April|25.März – 24. April   |1. Juli – 31. Juli|
|Beginn des kostenpflichtigen Zeitraums   | 15. Februar 2018 | 25. März 2018| 1. Juni 2018| 
|Ende des kostenpflichtigen Zeitraums | 14. Februar 2019   |24. Februar 2019   | 31. Mai 2019  |
|Verlängerungsdatum | 15. Februar 2019 |25. Februar 2019   |1.Juni2019|

### <a name="scenario---new-purchase"></a>Szenario: Neuer Kauf

Das Abrechnungsdatum des Partners ist der 15. Am 1. Juni kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Die Abstimmungsdatei vom 15. Juni wird Folgendes enthalten:

- 30 USD Gebühr für Monat 1 (1.Juni – 30.Juni)

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |

### <a name="scenario-suspend-and-reactivate-a-subscription-in-less-than-30-days-after-purchase"></a>Szenario: Stornieren und Reaktivieren eines Abonnements in weniger als 30Tagen nach dem Kauf

Das Abrechnungsdatum des Partners ist der 15. Am 1. Juni kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Am 5.Juni storniert der Partner das Abonnement. Am 10.Juni reaktiviert der Partner das Abonnement. Die Abstimmungsdatei vom 15. Juni wird Folgendes enthalten:

- 30 USD Gebühr für Monat 1 (1.Juni – 30.Juni) 
- -30 USD Erstattung für Stornierung Beachten Sie, dass die Gebühr ab dem 5. Juni berechnet wird, dem Datum, an dem der Partner das Abonnement storniert hat. Die Erstattung ist nicht anteilig. Der Partner erhält eine Erstattung von 100%, da er das Abonnement innerhalb der ersten 30Tage storniert hat.
- 30 USD Reaktivierungsgebühr Beachten Sie, dass die Gebühr ab dem 10. Juni berechnet wird, dem Datum, an dem der Partner das Abonnement reaktiviert hat. Der Betrag ist nicht anteilig. Alle Stornierungen und Reaktivierungen innerhalb von 30Tagen nach dem Kaufdatum werden nicht anteilig berechnet.


|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |
|5.6.2018   |30.6.2018   |-30 USD   |1   |30 USD   |
|10.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |


### <a name="scenario-suspend-a-subscription-in-less-than-30-days-after-purchase-and-reactivate-after-30-days"></a>Szenario: Stornieren eines Abonnements in weniger als 30Tagen nach dem Kauf und Reaktivieren nach 30 Tagen

Das Abrechnungsdatum des Partners ist der 15. Am 1. Juni kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Am 5.Juni storniert der Partner das Abonnement. Die Abstimmungsdatei vom 15. Juni wird Folgendes enthalten:

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |
|5.6.2018   |30.6.2018   |-30 USD   |1   |30 USD   |

Am 10.Juli reaktiviert der Partner das Abonnement. Die Abstimmungsdatei vom 15. Juli wird folgende Gebühren enthalten:

- 21,29 USD Reaktivierungsgebühr Die Gebühr wird ab dem 10.Juli berechnet, dem Datum, an dem der Partner das Abonnement reaktiviert hat, und der anteilige Betrag ist 21,29 USD. Alle Stornierungen und Reaktivierungen nach 30Tagen ab dem Kaufdatum werden anteilig berechnet. 

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|10.7.2018   |31.7.2018   |21,29 USD   |1   |21,29 USD   |

Das Verlängerungsdatum des Abonnements bleibt der 1. Juni des Folgejahrs, weil es 12 Monate nach dem ursprünglichen Kaufdatum liegt.

### <a name="scenario-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Szenario: Stornieren und Reaktivieren eines Abonnements nach mehr als 30Tagen nach dem Kauf 
Das Abrechnungsdatum des Partners der 15. jeden Monats. Am 1. Juni kauft der Partner ein neues Abonnement mit einer Lizenz zum Preis von 30 USD pro Monat. Die Abstimmungsdatei vom 15. Juni wird nur Folgendes enthalten: 30 USD Gebühr für Monat 1 (1. Juni – 30. Juni).

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |

Der Partner storniert das Abonnement am 5.Juli und reaktiviert es am 15.Juli. Die Abstimmungsdatei vom 15. Juli wird Folgendes enthalten:

- 30 USD Gebühr für Monat 2 (1. Juli – 31. Juli)

- -26,19 USD Erstattung für Stornierung Die Gebühr wird ab dem 5.Juli berechnet, dem Datum, an dem der Partner das Abonnement storniert hat. Die Erstattung ist anteilig. Alle Stornierungen und Reaktivierungen nach 30Tagen ab dem Kaufdatum werden anteilig berechnet.

- 21,37 USD Reaktivierungsgebühr Die Gebühr wird ab dem 10.Juli berechnet, dem Datum, an dem der Partner das Abonnement reaktiviert hat. Die Erstattung ist anteilig.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.7.2018   |31.7.2018   |30 USD  |1   |30 USD   |
|5.7.2018   |31.7.2018   |   -26,19 USD   |1   |-26,19 USD|
|10.7.2018   |31.7.2018   |-21,34 USD   |1   |21,34 USD|

### <a name="scenario-change-license-quantity"></a>Szenario: Anzahl der Lizenzen ändern 

Das Abrechnungsdatum des Partners ist der 15. Am 1. Juni kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Am 10.Juni erhöht der Partner die Anzahl der Lizenzen von 1 auf 2. Die Abstimmungsdatei vom 15. Juni wird Folgendes enthalten:

- 30 USD Gebühr für Monat 1 (1.Juni – 30.Juni) Obwohl der Partner die Anzahl der Lizenzen vor seinem Abrechnungsdatum (15.Juni) erhöht hat, wird die Änderung im Microsoft-Abrechnungssystem nicht vor dem Startdatum des Abonnements (1.Juli) registriert.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |

Am 1. Juli, dem Startdatum des Abonnements, registriert das Microsoft-Abrechnungssystem, dass die Anzahl der Lizenzen am 10. Juli von 1 auf 2 erhöht wurde. Das Abrechnungssystem generiert eine Erstattung und anteilige Gebühren für den Monat 1 und eine Gebühr für Monat 2. Die Abstimmungsdatei vom 15. Juli wird Folgendes enthalten:

- -30 USD Erstattung für Monat 1
- 9 USD anteilige Gebühr für Monat 1 (1.Juni – 9. Juni) für 1 Lizenz
- 42 USD anteilige Gebühr für Monat 1 (10.Juni – 30. Juni) für 2 Lizenzen
- 60 USD Gebühr für Monat 2 (1.Juli – 31.Juli) für 2 Lizenzen

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |-30 USD   |1   |-30 USD|
|1.6.2018   |9.6.2018   |9 USD   |1   |9 USD|
|10.6.2018   |30.6.2018   |21 USD   |2   |42 USD|
|1.7.2018   |31.7.2018   |30 USD   |2   |60 USD   |

### <a name="scenario-add-on-subscriptions"></a>Szenario: Add-On-Abonnements

Das Abrechnungsdatum des Partners ist der 15. Am 1. Juni kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Am 10. Juni kauft der Partner ein neues Add-On-Abonnement zum Preis von 5 USD pro Monat. Das Verlängerungsdatum für das Add-On-Abonnement wird das Verlängerungsdatum des Basisabonnement (1.Juni). 

Die Abstimmungsdatei vom 15. Juni wird Folgendes enthalten:

- 30 USD Gebühr für Monat 1 (1.Juni – 30.Juni) Dies gilt für das Basisabonnement.
- 3,50 USD anteilige Gebühr für Monat 1 (10.Juni – 30.Juni) für das Add-On-Abonnement. Die Gebühr wird ab dem 10.Juni berechnet, dem Datum, an dem der Partner das Add-On-Abonnement gekauft hat. Der Betrag ist anteilig.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   |30.6.2018   |30 USD   |1   |30 USD   |
|10.6.2018   |30.6.2018   |5 USD   |1   |5 USD   |

Die Abstimmungsdatei vom 15. Juli wird Folgendes enthalten:

- 30 USD Gebühr für Monat 2 (1. Juli – 31. Juli) Dies gilt für das Basisabonnement.
- 5 USD Gebühr für Monat 2 (1. Juli – 31. Juli) Dies gilt für das Add-On-Abonnement.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.7.2018   |31.7.2018   |30 USD   |1   |30 USD   |
|1.7.2018   |31.7.2018   |5 USD   |1   |5 USD   |

### <a name="scenario-new-purchase-on-the-29th-30th-or-31st"></a>Szenario: Neue Bestellung am 29., 30. oder 31. 

Das Abrechnungsdatum des Partners ist der 15. Am 31. Mai kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Am 29., 30. oder 31. erworbene Abonnements erhalten einen freien Zeitraum bis zum Beginn des Folgemonats. In diesem Beispiel erhält der Kunde einen kostenlosen Zeitraum von einem Tag, da der 12-monatige kostenpflichtige Zeitraum am 1.Juni beginnt. 

Die Abstimmungsdatei vom 15. Juni wird Folgendes enthalten:

- 30 USD Gebühr für Monat 1 (1.Juni – 30.Juni)

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |
|-----------------|:-------------|:----------------|:------------|:------|
|1.6.2018   | 30.6.2018   |30 USD   |1   |30 USD  |
