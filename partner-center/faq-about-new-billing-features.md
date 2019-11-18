---
title: Häufig gestellte Fragen zu neuen Abrechnungsfunktionen | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Im Folgenden finden Sie häufig gestellte Fragen zur jährlichen Abrechnung und zu kostenlosen Testversionen von Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: high
ms.openlocfilehash: db43e1904e5299ca552cb4f294f801e2cb94da24
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653127"
---
# <a name="faq-about-new-billing-features"></a>Häufig gestellte Fragen zu neuen Abrechnungsfunktionen

**Gilt für**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government


Im Folgenden finden Sie häufig gestellte Fragen zur jährlichen Abrechnung und zu kostenlosen Testversionen von Partner Center. 

## <a name="in-this-section"></a>Inhalt dieses Abschnitts

-   [Häufig gestellte Fragen zur jährlichen Abrechnung](#annualbillingfaq)

-   [Häufig gestellte Fragen zu kostenlosen Testversionen](#freetrialsfaq)

-   [Häufig gestellte Fragen zur Rechnungsanpassung](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Häufig gestellte Fragen zur jährlichen Abrechnung

Abschnitte:

[Übersicht und Vorteile der jährlichen Abrechnung](#overviewandbenefits)

[Bestellungs- und Abrechnungsszenarien](#placingyourorder)

[Ändern des Abonnements](#changingyoursubscription)

[Preisberechnung](#pricingcalculation)

[Berichterstellung](#reporting)

[Incentives](#incentives)


<a href="" id="overviewandbenefits"></a>**Übersicht und Vorteile der jährlichen Abrechnung**

**F:** Was hat sich geändert?

-   **A:** Aufgrund Ihrer Anfragen haben wir die Option eingeführt, bestimmte Cloud Solution Provider-Abonnements (CSP) jährlich oder monatlich zu bezahlen. Diese neue Option ist seit dem 17. Oktober 2017 verfügbar.

**F:** Wer kann daran teilnehmen?

-   **A:** Alle Partner und Partnertypen können die jährliche Abrechnung nutzen. Die jährliche Abrechnung ist in allen Märkten verfügbar, in denen CSP derzeit zur Verfügung steht. 

**F:** Was muss ich berücksichtigen, wenn ich die jährliche Abrechnung nutzen möchte?    

-   **A:** Sie sollten die Auswirkungen auf Ihren Verkaufsprozess berücksichtigen. Hier einige Tipps zur effektiven Nutzung der jährlichen Abrechnung. 
    - Aktualisieren Sie ggf. Ihre APIs zur Unterstützung der jährlichen Abrechnungsfunktion. 
    - Überprüfen Sie die Änderungen an der Rechnung und der lizenzbasierten Abstimmungsdatei.
    - Stellen Sie sicher, dass Ihr Team informiert wird.
    - Aktualisieren Sie bei Bedarf Ihre internen Prozesse.

**F:** Welche Vorteile bietet die jährliche Abrechnung? 

-   **A:** Die jährliche Abrechnung bietet folgende Vorteile:

    - Mehr Flexibilität im Hinblick auf die Zahlungsoptionen

    - Bessere Abstimmung mit der Fakturierung von Kunden

    - Geringere Auswirkungen von Wechselkursschwankungen

    - Reduzierte Betriebskosten für die Abrechnung

**F:** Für welche Angebote ist die jährliche Abrechnung verfügbar?

-   **A:** Bei den meisten lizenzbasierten Abonnements können Sie zwischen monatlicher und jährlicher Abrechnung wählen. Für nutzungsbasierte Abonnements ist nur die monatliche Abrechnung verfügbar. Die verfügbaren Abrechnungshäufigkeiten für jedes Angebot sind in der Spalte „J“ der Angebotsmatrix angegeben. Die Angebotsmatrix findest du im Abschnitt „Anzeigen von Angeboten und Preisen” im Partner Center. .

**F:** Erfolgt die jährliche Abrechnung pro Abonnement oder pro Lizenz?       

-   **A:** Sowohl die jährliche als auch die monatliche Abrechnung erfolgen pro Abonnement.

**F:** Sind zur Unterstützung der jährlichen Abrechnung Änderungen an APIs erforderlich?    

-   **A:** Die Nutzung der jährlichen Abrechnung erfordert einige Änderungen an Ihren APIs. Ausführlichere Informationen finden Sie in den folgenden Artikeln:

    - https://partnercenter.microsoft.com/partner/developer

    - https://msdn.microsoft.com/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Beispielcode: https://msdn.microsoft.com/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Bestellungs- und Abrechnungsszenarien**

**F:** Gibt es ein spezielles Angebot für Bestellungen mit jährlicher Abrechnung?   

-   **A:** Nein. Alle Abrechnungshäufigkeiten (einschließlich der jährlichen Abrechnung) sind dem Angebot als Attribut zugewiesen. Sie können ein Angebot jedoch zur Differenzierung umbenennen und einen benutzerfreundlichen Namen verwenden.

**F:** Wie wähle ich die jährliche Abrechnung aus?

-   **A:** Wenn Sie ein neues Abonnement hinzufügen, werden Sie aufgefordert, die Abrechnungshäufigkeit auszuwählen. An dieser Stelle können Sie die Option für jährliche Abrechnung auswählen. Nach dem Auswählen der jährlichen Abrechnung werden alle verfügbaren Angebote angezeigt.

**F:** Wann wird das Abonnement in Rechnung gestellt, wenn ich mich für die jährliche Abrechnung entscheide?    

-   **A:** Das Abonnement wird am nächsten Abrechnungsdatum in Rechnung gestellt. Wenn Ihr Abrechnungsdatum beispielsweise der 1. ist und Sie am 29. Oktober 2017 ein Abonnement mit jährlicher Abrechnung kaufen, wird Ihnen das Abonnement am 1. November 2017 in Rechnung gestellt. Sofern Sie keine Änderungen an den Lizenzen vornehmen, erfolgt die Rechnungslegung dann wieder am 1. November 2018. Wenn Sie eine Lizenzänderung vornehmen, erhalten Sie zum nächsten Abrechnungsdatum eine Gutschrift und eine anteilige Verrechnung. 

**F:** Kann ich ein Abonnement so aufteilen, dass ein Teil monatlich und ein Teil jährlich abgerechnet wird?  

-   **A:** Nein. Für das gesamte Abonnement muss die gleiche Abrechnungshäufigkeit gelten. Das gesamte Abonnement wird entweder monatlich oder jährlich abgerechnet.

**F:** Wann erfolgt die Verlängerung für ein Abonnement mit jährlicher Abrechnung?     

-   **A:** Das Abonnement wird zwölf Monate nach seinem Startdatum verlängert. Der Leistungszeitraum beginnt an dem Datum, an dem das Abonnement erstellt wird.  Ein am 10. Januar 2018 erstelltes Abonnement wird beispielsweise am 10. Januar 2019 verlängert.

**F:** Wann wird mir die Verlängerung eines Abonnements mit jährlicher Abrechnung in Rechnung gestellt? 

-   **A:** Die Rechnungslegung erfolgt am nächsten Abrechnungsdatum nach dem Verlängerungsdatum des Abonnements. Wenn Sie beispielsweise am 15. Januar 2018 ein Abonnement mit jährlicher Abrechnung erwerben und Ihr Abrechnungsdatum der 20. Januar ist, wird Ihr Abonnement am 15. Januar 2019 verlängert. Die Verlängerung wird Ihnen am 20. Januar 2019 in Rechnung gestellt.

**F:** Gilt für Abonnements mit jährlicher Abrechnung ein kostenloser Zeitraum?

-   **A:** Nein. Abonnements mit jährlicher Abrechnung erhalten keinen kostenlosen Zeitraum. Die kostenpflichtige Laufzeit von zwölf Monaten beginnt mit dem Kaufdatum. Dies unterscheidet sich von Abonnements mit monatlicher Abrechnung, für die nach dem Kauf ein kostenloser Zeitraum bis zum nächsten Abrechnungsdatum gilt.

**F:** Kann ein Kunde mehrere Abonnements für das gleiche Angebot mit unterschiedlichen Abrechnungshäufigkeiten haben?    

-   **A:** Das hängt vom Angebot ab. Bestimmte Angebote sind auf ein Abonnement pro Kunde beschränkt. Wenn für das Angebot keine Einschränkung gelten, kann ein Kunde mehrere Abonnements für das gleiche Angebot mit unterschiedlichen Abrechnungshäufigkeiten besitzen. Details zu allen Angebotseinschränkungen sind in der Spalte „I“ der Angebotsmatrix angegeben. Die Angebotsmatrix findest du im Abschnitt „Anzeigen von Angeboten und Preisen” im Partner Center.

<a href="" id="changingyoursubscription"></a>**Ändern des Abonnements**

**F:** Kann ich einem vorhandenen Abonnement mit jährlicher Abrechnung eine neue Lizenz hinzufügen?    

-   **A:** Ja. Sie können die Anzahl von Lizenzen für Ihre Abonnements jederzeit ändern. Das Hinzufügen zusätzlicher Lizenzen hat keinen Einfluss auf die Abrechnungshäufigkeit. 

**F:** Kann ich einem vorhandenen Abonnement mit jährlicher Abrechnung Lizenzen mit monatlicher Abrechnung hinzufügen? 

-   **A:** Nach dem Kauf eines Abonnements mit jährlicher Abrechnung gilt diese Abrechnungshäufigkeit für alle zusätzlichen Lizenzen. Wenn Sie Lizenzen mit monatlicher Abrechnung benötigen, müssen Sie ein neues Abonnement kaufen.

**F:** Kann ich die Abrechnungshäufigkeit für ein Abonnement von monatlicher auf jährliche Abrechnung (und umgekehrt) umstellen? 

-   **A:** Ja. Informationen zum **Ändern der Abrechnungshäufigkeit für einen Onlinedienst** finden Sie unter [Übersicht über die Abrechnung](https://docs.microsoft.com/partner-center/billing-basics).

**F:** Ist die jährliche Abrechnung für Add-On-Angebote verfügbar?   

-   **A:** Ja. Dem Add-On-Abonnement wird automatisch die gleiche Abrechnungshäufigkeit zugewiesen wie dem übergeordneten Abonnement.

**F:** Wie funktioniert die jährliche Abrechnung, wenn ich Lizenzen hinzufüge oder entferne? 

-   **A:** Sie können jederzeit Lizenzen hinzufügen oder entfernen. Nach dem Ändern der Anzahl von Lizenzen erhalten Sie zum nächsten Abrechnungsdatum eine Gutschrift und eine anteilige Verrechnung. 

**F:** Was passiert, wenn ich ein Abonnement mit jährlicher Abrechnung kündige?    

-   **A:** Für alle Abrechnungshäufigkeiten gelten die gleichen Kündigungsbedingungen. Wenn das Abonnement in den ersten 30 Tagen der kostenpflichtigen Laufzeit von zwölf Monaten gekündigt wird, erhalten Sie zum nächsten Abrechnungsdatum eine Gutschrift über den vollen Betrag. Wird das Abonnement nach den ersten 30 Tagen der kostenpflichtigen Laufzeit von zwölf Monaten gekündigt, erhalten Sie zum nächsten Abrechnungsdatum eine anteilige Gutschrift.

**F:** Kann ein Kunde ein Abonnement mit jährlicher Abrechnung von einem Partner auf einen anderen übertragen?  

-   **A:** Nein. Abonnements können nicht zwischen Partnern übertagen werden. Der neue Partner muss im Auftrag des Kunden ein neues Abonnement erwerben. Dies gilt für Abonnements mit monatlicher und jährlicher Abrechnung.

**F:** Kann ich ein Abonnement mit jährlicher Abrechnung reaktivieren?

-   **A:** Ja. Sie haben ab dem Datum der Aussetzung 90 Tage Zeit, das Abonnement zu reaktivieren. Die anteilig e Gebühr wird zum folgenden Abrechnungsdatum in Rechnung gestellt. Das Verlängerungsdatum des Abonnements bleibt unverändert.

<a href="" id="pricingcalculation"></a>**Preisberechnung**

**F:** Was geschieht, wenn sich der Angebotspreis für ein Abonnement mit jährlicher Abrechnung während des Zeitraums von zwölf Monaten ändert?    

-   **A:** Der Angebotspreis zum Zeitpunkt des Kaufs ist für die 12-monatige Laufzeit des Abonnements garantiert. 

**F:** Welcher Preis gilt für ein Abonnement, wenn es nach zwölf Monaten automatisch verlängert wird?    

-   **A:** Wenn ein Abonnement verlängert wird, gilt der Preis in der aktuellen Preisliste zum Zeitpunkt der Verlängerung. Der neue Preis ist für die nächste Abonnementlaufzeit von zwölf Monaten garantiert.

**F:** Wie wird die Gutschrift für eine gekündigte Lizenz oder ein gekündigtes Abonnement berechnet? Wird sie pro Tag oder pro Monat berechnet?   

-   **A:** Eine Stornierungsgutschrift wird wie folgt berechnet:

    - Stornierungsgutschrift = ((Monatspreis*12)/365) * verbleibende Tage in der 12-monatigen Laufzeit * Anzahl gekündigter Lizenzen

**F:** Was geschieht, wenn der Angebotspreis für ein Abonnement mit jährlicher Abrechnung während der Laufzeit von zwölf Monaten gesenkt wird? 

-   **A:** Eine Änderung des Preises findet nicht statt. Der Preis gilt für den gesamten Zeitraum von zwölf Monaten. Dies entspricht der monatlichen Abrechnung.


<a href="" id="reporting"></a>**Berichterstellung**

**F:** Wo kann ich feststellen, ob ein Abonnement jährlich oder monatlich abgerechnet wird?   

-   **A:** Die lizenzbasierte Abstimmungsdatei enthält die Abrechnungshäufigkeit. Sie ist in der Spalte „AA“ angegeben.

**F:** Welche Änderungen enthält die lizenzbasierte Abstimmungsdatei, wenn ein Abonnement mit jährlicher Abrechnung gekauft oder verlängert wird?  

-   **A:** Die erste Änderung ist eine neue Zeile in der lizenzbasierten Abstimmungsdatei am ersten Abrechnungsdatum nach dem Kauf eines neuen Abonnements. Wenn keine Änderungen am Abonnement vorgenommen werden, enthalten die Abstimmungsdateien keine Zeilen für die Monate 2 –12 der Abonnementlaufzeit. Die nächste Änderung in der Abstimmungsdatei erfolgt, wenn das Abonnement verlängert wird. Diese Änderung erscheint am ersten Abrechnungsdatum nach der Verlängerung. Wenn während der 12-monatigen Laufzeit eine Änderung am Abonnement vorgenommen wird, enthält die nächste Abstimmungsdatei nach der Änderung eine Gutschrift und eine anteilige Verrechnung.

**F:** Wie werden der Kauf, die Änderung oder die Kündigung eines Jahresabonnements in der Spalte „P“ der Nutzungsdateien angezeigt?

-   **A:** Die anfängliche Gebühr wird als „Anteilige Gebühren beim Kauf” angezeigt. Lizenzänderungen, die zu einer Gutschrift und Verrechnung führen, werden als „Anteiliger Zyklus für Instanz” angezeigt. Stornierungsgutschriften werden als „Stornierungsgebühr” angezeigt.

**F:** Was wird in der Abstimmungsdatei angezeigt, wenn ein Jahresabonnement gekündigt wird?   

-   **A:** Die Abstimmungsdatei enthält eine Position für eine Stornierungsgutschrift. Erfolgt die Kündigung in den ersten 30 Tagen der 12-monatigen Laufzeit, wird der volle Betrag für das Abonnement gutgeschrieben. Wird das Abonnement nach den ersten 30 Tagen storniert, wird der anteilige Betrag dem Abonnement gutgeschrieben

**F:** Was wird in der Abstimmungsdatei angezeigt, wenn einem Abonnement mit jährlicher Abrechnung Lizenzen hinzugefügt werden?  

-   **A:** Die Abstimmungsdatei enthält eine Gutschrift und eine anteilige Verrechnung. Dies gilt auch für ein Abonnement mit monatlicher Abrechnung.

**F:** Was wird in der Abstimmungsdatei angezeigt, wenn Lizenzen aus einem Abonnement mit jährlicher Abrechnung entfernt werden? 

-   **A:** Die Abstimmungsdatei enthält eine Gutschrift und eine anteilige Verrechnung.  Dies gilt auch für ein Abonnement mit monatlicher Abrechnung.

**F:** Wird der jährliche Preis in der Preisliste angezeigt? 

-   **A:** Nein. Die Preisliste enthält den monatlichen Preis. Sie können die jährlichen Preis berechnen, indem Sie den monatlichen Preis mit zwölf multiplizieren.

**F:** Enthält die Angebotsmatrix unterschiedliche Einträge für Angebote, für die die jährliche Abrechnung verfügbar ist?   

-   **A:**  Nein. Der Angebots-IDs sind für alle Abrechnungshäufigkeiten identisch. Es gibt keine speziellen Angebots-IDs für die jährliche Abrechnung.


<a href="" id="incentives"></a>**Incentives**

**F:** Wie oft werden Incentives für Jahresabonnements berechnet? 

-   **A:** Die Berechnung erfolgt nach dem fakturierten Umsatz. Erzielte Anreizzahlungen werden im Einklang mit unserer Richtlinien gezahlt, wie in den CSP-Anreizhandbüchern aufgeführt. 

**F:** Wie werden Incentives für Abonnements mit jährlicher Abrechnung gezahlt?  

-   **A:** Derzeit erfolgen alle Incentive-Zahlungen zweimal pro Jahr. Diese Zahlungen erfolgen 45 Tage nach Halbjahresende.

**F:** Wie werden die Umsatzerlöse eines Abonnements mit jährlicher Abrechnung mit der Berechnung der Incentives verbucht? Erfolgt die Berechnung auf der Grundlage der fakturierten oder der angepassten Umsatzerlöse? 

-   **A:** Incentive-Berechnungen basieren auf den fakturierten Umsatzerlösen.

**F:** Wie werden die Incentive-Einnahmen für ein berechtigtes Abonnement mit jährlicher Abrechnung bezüglich der verschiedenen CSP-Incentive-Raten (globale Incentive-Raten, lokale Beschleunigungsraten und lokale Kampagnen) berechnet?

-   **A:** Unabhängig von der Abrechnungshäufigkeit eines Abonnements (monatlich oder jährlich) erhalten Partner Incentives für alle berechtigten Transaktionen. Dazu gehören die globale Incentive-Rate, die auf die fakturierten Umsatzerlöse des Zeitraums angewendet wird, der lokale Beschleuniger für alle Regionen, in denen es lokale Beschleuniger gibt, und ggf. globale Kampagnen.

**F:** An wen kann ich mich bei Fragen zu Incentives wenden?

- **A:** Wenden Sie sich an das jeweilige regionale Supportteam für Incentives:

  - Nordamerika: ocina@microsoft.com

  - Lateinamerika und Brasilien: ocilatam@microsoft.com

  - Europa, Naher Osten und Afrika (EMEA): ociemea@microsoft.com

  - Asien-Pazifik (APAC, ausgenommen Japan): ociapgc@microsoft.com

  - Japan: ocijp@microsoft.com


**F:** Was geschieht, wenn ich mein Abonnement aussetze? 

-   **A:** Wenn Sie ein Abonnement innerhalb von 30 Tagen nach dem Kauf in Partner Center oder über die API aussetzen, wird Ihnen unabhängig von der Abrechnungshäufigkeit der volle Betrag erstattet. 

    Bei der jährlichen Abrechnung würde dies wie folgt aussehen:

    - Der Partner kauft das Abonnement am 1. Januar = Rechnungsposition für die Gebühr für den Leistungszeitraum 1. Januar – 31. Dezember
    - Der Partner setzt das Abonnement am 25. Januar aus = Rechnungsposition für die Gutschrift für den Leistungszeitraum 1. Januar – 31. Dezember
    - Der Partner reaktiviert das Abonnement am 29. Januar = Rechnungsposition für die Gebühr für den Leistungszeitraum 29. Januar – 31. Dezember

    Bei der monatlichen Abrechnung würde dies wie folgt aussehen:

    - Der Partner kauft das Abonnement am 1. Januar = Rechnungsposition für die Gebühr für den Leistungszeitraum 1. Januar – 31. Januar
    - Der Partner setzt das Abonnement am 25. Januar aus = Rechnungsposition für die Gutschrift für den Leistungszeitraum 1. Januar – 31. Januar
    - Der Partner reaktiviert das Abonnement am 29. Januar = Rechnungsposition für die Gebühr für den Leistungszeitraum 29. Januar – 31. Januar



## <a href="" id="freetrialsfaq"></a>Häufig gestellte Fragen zu kostenlosen Testversionen

**F1:** Was sind kostenlose Testversionen?

-   **A:** Sie können Ihren Kunden eine 30-tägige kostenlose Testversion von bestimmten Produkten anbieten. Dadurch können Ihre Kunden das Produkt vor dem Kauf bewerten. Kostenlose Testversionen sind für folgende Produkte verfügbar: 

    - Office 365 Business Premium (ab dem 17. Oktober 2017)
    - Office 365 E3 (ab dem 17. Oktober 2017)
    - Office 365 E5 mit PSTN (ab dem 17. Oktober 2017)
    - Office 365 E5 ohne PSTN (ab dem 17. Oktober 2017)
    - Enterprise Mobility + Security E5 (ab dem 17. Oktober 2017)
    - Dynamics 365 Customer Engagement Plan 1 (ab dem 17. Oktober 2017)
    - Dynamics 365 for Financials (ab dem 17. Oktober 2017)
    - Microsoft 365 Business (ab dem 1. März 2018)
    
**F2:** Unterscheiden sich die jährliche Abrechnung und kostenlose Testversionen bei der unabhängigen Cloud und der öffentlichen Cloud?

-   **A:** Nein. Sie sind identisch. Der einzige Unterschied sind die Testversions-SKUs, die zum Einführungszeitpunkt verfügbar sind.

**F3:** Wer kann daran teilnehmen?

-   **A:** Alle Partner können daran teilnehmen. Allerdings sind in China derzeit keine Testversionen verfügbar. 

**F4:** Was muss ich unternehmen, um von diesen kostenlosen Testversionen zu profitieren?

-   **A:** Überlegen Sie, wie die kostenlose Testversion in Ihren Verkaufsprozess integriert werden kann und welche Auswirkung sie auf interne Prozesse hat. Möglicherweise müssen Sie zudem Ihre APIs ändern, um die Umwandlung einer kostenlosen Testversion in ein kostenpflichtiges Abonnement zu unterstützen. Im Ankündigungsbereich von Partner Center werden detaillierte technische Spezifikationen für API-Änderungen zur Verfügung gestellt.

**F5:** Wird die kostenlose Testversion in meiner Rechnung und Abstimmungsdatei aufgeführt?

-   **A:** Nein. Kostenlose Testversionen werden nicht in Ihrer Rechnung oder lizenzbasierten Abstimmungsdatei angezeigt. Eine kostenlose Testversion erscheint erst nach der Umwandlung in ein kostenpflichtiges Abonnement auf Ihrer Rechnung und in der lizenzbasierten Abstimmungsdatei. Das umgewandelte Abonnement wird wie jedes andere neue Abonnement in Ihrer Rechnung und der lizenzbasierten Abstimmungsdatei aufgeführt.

**F6:** Haben kostenlose Testversionen Auswirkungen auf Incentives?

-   **A:** Nein. Die kostenlose Testversion wirkt sich nicht auf Incentives aus.

**F7:** Werden in Zukunft kostenlose Testversionen für weitere Office-Produkte zur Verfügung gestellt?

-   **A:** Wir bieten kostenlose Testversionen für diese Produkte an, da sie die umfassendsten und beliebtesten Angebote für Unternehmen sind. Wir werden in Zukunft möglicherweise weitere kostenlose Testversionen anbieten.

**F8:** Kann ein Kunde mehrere kostenlose Testversionen nutzen?

-   **A:** Jeder Kunde hat Anspruch auf eine kostenlose Testversion pro verfügbarem Angebot.

**F9:** Gibt es Beschränkungen für eine kostenlose Testversion?

-   **A:** Ja. Die Testversion gilt für maximal 25 Lizenzen. Die Anzahl von Lizenzen kann während des Testzeitraums nicht geändert werden. Nachdem die Testversion in ein kostenpflichtiges Abonnement umgewandelt wurde, können Sie dem Abonnement zusätzliche Lizenzen hinzufügen.

**F10:** Wird eine kostenlose Testversion automatisch in ein kostenpflichtiges Abonnement umgewandelt?

-   **A:** Nein. Der Partner muss das Abonnement selbst in Partner Center oder über die API umwandeln.

**F11:** Können kostenlose Testversionen sowohl für Abonnements mit monatlicher als auch jährlicher Abrechnung verwendet werden?

-   **A:** Ja. Sie können die Abrechnungshäufigkeit auswählen, wenn Sie die Testversion in ein kostenpflichtiges Abonnement umwandeln.

**F12:** Wird das Startdatum des Abonnements basierend auf dem Datum der kostenlosen Testversion bestimmt oder basierend auf dem Datum, an dem die Testversion in ein kostenpflichtiges Abonnement umgewandelt wird? 

-   **A:** Das Startdatum basiert auf dem Datum der Umwandlung. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit jährlicher Abrechnung umgewandelt wird, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem Datum der Umwandlung. Wird die kostenlose Testversion in ein kostenpflichtiges Angebot mit monatlicher Abrechnung umgewandelt, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem auf das Datum der Umwandlung folgenden Abrechnungsdatum.

**F13:** Können während der kostenlosen Testphase Arbeitsplätze hinzugefügt oder entfernt werden?

-   **A:** Nein. Kostenlose Testversionen umfassen standardmäßig 25 Lizenzen, und die Anzahl von Arbeitsplätzen kann nicht erhöht werden.

**F14:** Gibt es Testversionen für Add-On-Angebote wie ATP und PSTN?

-   **A:** Zurzeit sind keine kostenlosen Testversionen für Add-On-Angebote verfügbar.

**F15:** Kann ich eine kostenlose Testversion für ein Angebot anbieten, das ein Kunde bereits besitzt?

-   **A:** Nein. Wenn der Kunde das Angebot bereits besitzt, kann dafür keine kostenlose Testversion bereitgestellt werden.

**F16:** Kann ich all meine ausstehenden Testangebote anzeigen?

-   **A:** Ja. Auf der Kundenseite sind alle Abonnements aufgeführt. Es werden sowohl Abonnements für kostenlose Testversionen als auch kostenpflichtige Abonnements angezeigt.

**F17:** Werde ich benachrichtigt, wenn kostenlose Testversionen ablaufen?

-   **A:** Nein. Sie können bevorstehende Ablauftermine in der Kundenansicht in Partner Center verfolgen oder das Datum mit der API abfragen. Du solltest die Datumsangaben regemäßig überprüfen, damit du zusammen mit dem Kunden die entsprechenden Folgeaktionen durchführen kannst, wenn eine Entscheidung getroffen werden muss.

**F18:** Kann ein Kunde, der bereits eine kostenlose Testversion für ein Angebot genutzt hat, weitere Testversionen für andere Angebote erhalten? 

-   **A:** Ja. Kunden können sich für eine Testversion pro Angebot registrieren. Sie können z. B. eine kostenlose Testversion für Office 365 Business Premium und eine kostenlose Testversion für Office 365 E3 erhalten.

**F19:** Was geschieht, wenn die Testversion abläuft? Werde ich benachrichtigt, oder erhält der Kunde eine Benachrichtigung? Welche Benachrichtigungen werden angezeigt, wenn ich versuche, mich bei einer abgelaufenen Testversion anzumelden?

-   **A:** Wenn der Kunde versucht, sich nach dem Ablauf einer Testversion bei dieser anzumelden, wird eine Meldung angezeigt, dass die Testversion abgelaufen ist. Es gibt keine Benachrichtigungen über den bevorstehenden Ablauf einer Testversion. Als Partner können Sie das Ablaufdatum jedoch in der Kundenansicht oder mit API-Abfragen nachverfolgen.

**F20:** Kann eine Testversion verlängert werden?

-   **A:** Nein. Nach 30 Tagen muss die Testversion umgewandelt werden. Andernfalls läuft sie ab.

**F21:** Kann auf die Informationen in einer Testversion zugegriffen werden, nachdem diese abgelaufen ist?

-   **A:** Ja. Die Daten werden entsprechend den Standards für die Datenaufbewahrung gespeichert. Nachdem Sie ein neues Abonnement mit den gleichen Serviceplänen erworben haben, können Sie über das neu aktivierte Abonnement auf die Daten Ihres Kunden zugreifen.

**F22:** Gibt es kostenlose Testversionen für Behörden und Bildungseinrichtungen?

-   **A:** Zurzeit sind keine kostenlosen Testversionen für Angebote für Behörden und Bildungseinrichtungen verfügbar.

**F23:** Können kostenlose Testversionen für das Cloud Solution Provider-Programm (CSP) auf andere Programmmandanten wie EA, Open oder MOSP übertragen werden? 

-   **A:** Nein. Abonnements können nicht vom CSP-Programm auf andere Programme übertragen werden.

**F24:** Wie erhalte ich Support für kostenlose Testversionen? 

-   **A:** Übermitteln Sie eine Serviceanfrage über Partner Center.

## <a href="" id="billingalignmentfaq"></a>Rechnungsanpassung: Aufhebung des kostenlosen Zeitraums

Die „Anpassung des Abrechnungsdatums“ für neue Abonnements mit monatlicher Abrechnung wird ab dem 21. Februar 2018 im Cloud Solution Provider-Programm (CSP) implementiert. Diese „Anpassung des Rechnungsdatums” bietet den Partnern mehr Flexibilität und Vorhersagbarkeit für Vertrieb, Abrechnung, Bereitstellung und Verwaltung von Kundenabonnements. 

**UPDATE – 23. FEBRUAR:**  Wir hatten die Implementierung bereits für den 20. Februar angekündigt, aber sie hat sich leicht verzögert und ist nach Produktkategorien gestaffelt.  In der folgenden Tabelle finden Sie das Implementierungsdatum für die verschiedenen Produktkategorien. 

|**Produktkategorie**   |**Implementierungsdatum**   |
|-----------------|:-------------|
|Office  |21. Februar   |
|Windows, Minecraft   |22. Februar   |
|Office 365 (China)   |23. Februar   |
|Dynamics/Intune   |23. Februar   |

Für Abonnements, die vor dem Implementierungsdatum (siehe obige Tabelle) gekauft wurden, gilt ein kostenloser Zeitraum vom Kaufdatum bis zum Abrechnungsdatum des Partners. Abonnements, die nach dem Implementierungsdatum gekauft wurden, erhalten keinen kostenlosen Zeitraum mehr. Die 12-monatige Zahlungsfrist beginnt mit dem Kaufdatum auf der Partnerabrechnung. Partnern wird keine Rechnungszeile mehr mit einem Nullbetrag angezeigt, die den kostenlosen Zeitraum in der Abstimmungsdatei darstellt. Es gibt keine Änderungen an APIs, Fakturierung oder Incentives.  Partner sollten ihre Verkaufs- und Buchhaltungsteams über diese neue Abrechnungslogik informieren und sicherstellen, dass alle Vorgänge bei Bedarf angepasst werden.  

Vor der Anpassung des Abrechnungsdatums sind wir bei der Rechnungsstellung von dem Datum ausgegangen, an dem der Partner dem CSP-Programm beigetreten ist, und nicht von dem Datum, an dem der Kunde das Abonnement erworben hat. Nach dem Implementierungsdatum erfolgt die Abrechnung für Partner zum Jahrestag des Abonnements, wodurch dieser kostenlose Zeitraum entfällt.  Partner erhalten weiterhin Rechnungen zum Jahrestag der Abrechnung, das effektive Rechnungsdatum ist jedoch der Jahrestag des Kundenabonnements. 

Abonnements, die sich zum Implementierungsdatum im kostenlosen Zeitraum befinden, werden zwischen dem Kaufdatum und dem Abrechnungsdatum des Partners nicht berechnet. Zudem werden sie im ersten Monat der kostenpflichtigen Laufzeit von zwölf Monaten nicht in Rechnung gestellt. Wenn Sie eine Abstimmungsdatei zur Überprüfung verwenden, beachten Sie, dass die Gebühren für diesen ersten Monat nicht mehr angezeigt werden.  

**F1:** Was ändert sich beim Abrechnungsdatum?

-   **A:** Für lizenzbasierte Abonnements gibt es keinen kostenlosen Zeitraum mehr. Derzeit ist der Zeitraum zwischen dem Kaufdatum und dem Abrechnungsdatum des Partners kostenlos.

**F2:** Wann entfällt der kostenlose Zeitraum?

- **A:** Ab dem in der folgenden Tabelle angegebenen Implementierungsdatum gilt für neue Abonnements kein kostenloser Zeitraum mehr.

|**Produktkategorie**   |**Implementierungsdatum**   |
|-----------------|:-------------|
|Office  |21. Februar   |
|Windows, Minecraft   |22. Februar   |
|Office 365 (China)   |23. Februar   |
|Dynamics/Intune   |23. Februar   |

**F3:** Wie wirkt sich dies auf Abonnements aus, die sich am Implementierungsdatum im kostenlosen Zeitraum befinden?

- **A:** Für Abonnements, die sich am Implementierungsdatum im kostenlosen Zeitraum befinden, gilt weiterhin ein kostenloser Zeitraum vom Kaufdatum bis zum Abrechnungsdatum des Partners. Diese Lizenzen erhalten zudem einen „verlängerten kostenlosen Zeitraum” und werden für den ersten Monat der kostenpflichtigen Laufzeit von zwölf Monaten nicht berechnet. Der „verlängerte kostenlose Zeitraum” gilt nicht für Lizenzen, die im ersten Monat hinzugefügt werden. Wenn Sie die Lizenzanzahl im ersten Monat erhöhen, werden Ihnen die zusätzlichen Lizenzen mit der nächsten Rechnung/Abstimmung in Rechnung gestellt. Wenn Sie die Abstimmungsdatei zur Überprüfung verwenden, beachten Sie, dass die Gebühren für diesen ersten Monat möglicherweise nicht mehr in der Datei angezeigt werden. Die nachstehenden Szenarien enthalten eine genauere Beschreibung.

**F4:** Wann beginnt der kostenpflichtige Zeitraum von zwölf Monaten für ein neues Abonnement?

- **A:** Derzeit beginnt der kostenpflichtige Zeitraum an dem auf das Kaufdatum folgenden Abrechnungsdatum des Partners. Ab dem Implementierungsdatum beginnt der kostenpflichtige Zeitraum für neue Abonnements am Kaufdatum.

**F5:** Wann werden Abonnements automatisch verlängert?

- **A:** Abonnements werden zwölf Monate nach dem ersten Abrechnungsdatum automatisch verlängert. Derzeit erfolgt die automatische Verlängerung von Abonnements somit zwölf Monate nach dem auf das Kaufdatum folgenden Abrechnungsdatum des Partners. Ab dem Implementierungsdatum werden neue Abonnements zwölf Monate nach dem Kaufdatum automatisch verlängert.

**F6:** Was geschieht, wenn ich das Abonnement am 29., 30. oder 31. eines Monats erwerbe?

- **A:** Das Abonnement ist ab dem Kaufdatum verfügbar. Die kostenpflichtige Laufzeit von zwölf Monaten beginnt jedoch erst am ersten Tags des Folgemonats.

**F7:** Welche Angebote sind betroffen?

- **A:** Der kostenlose Zeitraum entfällt für alle lizenzbasierten CSP-Abonnements.

**F8:** Wie wirkt sich diese Änderung auf die Rechnung und die Abstimmungsdatei aus? 

- **A:** Die Nullbetragszeile erscheint nicht mehr in der Rechnung und Abstimmungsdatei. Derzeit bezeichnet die Nullbetragszeile einen kostenlosen Zeitraum.

**F9:** Ändert sich mein Abrechnungsdatum?

- **A:** Nein. Sie erhalten die Rechnung und die Abstimmungsdatei weiterhin an Ihrem bisherigen Abrechnungsdatum.

**F10:** Ändern sich das monatliche Anfangs- und Enddatum für bestehende Abonnements?

- **A:** Nein. Das monatliche Anfangs- und Enddatum für bestehende Abonnements entspricht weiterhin Ihrem Abrechnungsdatum. Neue Abonnements werden jedoch nach dem Kaufdatum berechnet. Siehe Beispiel unten.

**F11:** Ändert sich die Berechnung der Incentives?

- **A:** Nein. Es gibt keine Änderung bei den Incentives-Berechnungen.

**F12:** Werden die APIs geändert?

- **A:** Nein. Die APIs werden nicht geändert.

### <a name="common-scenarios"></a>Häufige Szenarien


|**Szenarien**   |**Szenario 1: Der kostenlose Zeitraum des Abonnements endet vor dem Implementierungsdatum.**   |**Szenario 2: Das Abonnement befindet sich am Implementierungsdatum im kostenlosen Zeitraum.**  | **Szenario 3: Das Abonnement wurde am oder nach dem Implementierungsdatum gekauft.**   |
|----------|:------------|:--------------------|:------------|
|Kaufdatum |1\. Februar 2018    | 1\. Februar 2018    | 1\. Juni 2018     |
|Bereitstellungsdatum | 1\. Februar 2018   |1\. Februar 2018   |1\. Juni 2018   |
|Abrechnungsdatum   | 15. jedes Monats   |25. jedes Monats   | 15. jedes Monats|
|Kostenloser Zeitraum   | 1\. Februar 2018 – 14. Februar 2018|1\. Februar 2018 – 24. Februar 2018   |Kein kostenloser Zeitraum|
|Gebühr für den ersten Monat   | 15. Februar 2018 – 14. März 2018 | Für am 24. Februar 2018 bestehende Lizenzen gilt ein verlängerter kostenloser Zeitraum bis zum 24. März 2018. Nach dem 24. Februar 2018 hinzugefügte Lizenzen werden in Rechnung gestellt. |1\. Juni 2018 – 30. Juni 2018   |
|Gebühr für den zweiten Monat   | 15. März 2018 – 14. April 2018|25. März 2018 – 24. April 2018   |1\. Juli 2018 – 31. Juli 2018|
|Beginn des kostenpflichtigen Zeitraums   | 15. Februar 2018 | 25. Februar 2018| 1\. Juni 2018| 
|Ende des kostenpflichtigen Zeitraums | 14. Februar 2019   |24. Februar 2019   | 31. Mai 2019  |
|Verlängerungsdatum | 15. Februar 2019 |25. Februar 2019   |1\. Juni 2019|

### <a name="scenario-4---new-purchase"></a>Szenario 4: Neukauf

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni 2018 kauft der Partner ein neues Abonnement. Das Abonnement kostet 30 USD pro Lizenz und Monat. 

Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall nur die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Szenario 5a: Aussetzen und Reaktivieren vor dem Abrechnungsdatum

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni 2018 kauft der Partner ein neues Abonnement. Das Abonnement kostet 30 USD pro Lizenz und Monat. Am 5. Juni 2018 setzt der Partner das Abonnement aus. Am 10. Juni 2018 reaktiviert der Partner das Abonnement. Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni. 
- -30 USD Stornierungsgutschrift für den Leistungszeitraum 5. Juni – 30. Juni. Die Gutschrift ist nicht anteilig, da das Abonnement in den ersten 30 Tagen ausgesetzt wurde. 
- 30 USD Gebühr für den Leistungszeitraum 10. Juni – 30. Juni. Die Gebühr ist nicht anteilig, da das Abonnement in den ersten 30 Tagen reaktiviert wurde. 

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |
|05.06.2018   |30.06.2018   |-30 USD   |1   |30 USD   |Stornierungsgebühr |
|10.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Aktivierungsgebühr |

Beachten Sie, dass die automatische Verlängerung bei der Aussetzung und Reaktivierung eines Abonnements weiterhin zwölf Monate nach dem ursprünglichen Kaufdatum erfolgt.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Szenario 5b: Aussetzen und Reaktivieren eines Abonnements nach dem Abrechnungsdatum, aber in weniger als 30 Tagen nach dem Kaufdatum

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni 2018 kauft der Partner ein neues Abonnement. Das Abonnement kostet 30 USD pro Lizenz und Monat. Am 20. Juni 2018 setzt der Partner das Abonnement aus. Am 25. Juni 2018 reaktiviert der Partner das Abonnement. Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni. 

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |

Die Abstimmungsdatei vom 15. Juli enthält in diesem Fall die folgenden Rechnungspositionen:
- -30 USD Stornierungsgutschrift für den Leistungszeitraum 20. Juni – 30. Juni Die Gutschrift ist nicht anteilig, da das Abonnement in den ersten 30 Tagen ausgesetzt wurde.
- 30 USD Gebühr für den Leistungszeitraum 25. Juni – 30. Juni Die Gebühr ist nicht anteilig, da das Abonnement in den ersten 30 Tagen reaktiviert wurde.
- 30 USD Gebühr für den Leistungszeitraum 1. Juli – 31. Juli.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20.06.2018   |30.06.2018   |-30 USD   |1   |-30 USD   |Stornierungsgebühr |
|25.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Aktivierungsgebühr |
|01.07.2018   |31.07.2018   |30 USD   |1   |30 USD   |Gebühr für Zyklus |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Szenario 5c: Aussetzen und Reaktivieren einer unterschiedlichen Anzahl von Lizenzen nach dem Abrechnungsdatum, aber in weniger als 30 Tagen nach dem Kaufdatum

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni 2018 kauft der Partner ein neues Abonnement. Das Abonnement kostet 30 USD pro Lizenz und Monat. Am 20. Juni 2018 setzt der Partner das Abonnement aus. Am 25. Juni 2018 reaktiviert der Partner das Abonnement mit zwei Lizenzen. Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni. 

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |

Die Abstimmungsdatei vom 15. Juli enthält in diesem Fall die folgenden Rechnungspositionen:
- -30 USD Stornierungsgutschrift für den Leistungszeitraum 20. Juni – 30. Juni Die Gutschrift ist nicht anteilig, da das Abonnement in den ersten 30 Tagen ausgesetzt wurde.
- 30 USD Gebühr für den Leistungszeitraum 25. Juni – 30. Juni Die Reaktivierungsgebühr ist nicht anteilig, da das Abonnement in den ersten 30 Tagen reaktiviert wurde. Die Gebühr basiert ebenfalls auf der ursprünglichen Anzahl von Lizenzen (eine Lizenz).
- -6 USD Gutschrift für den Leistungszeitraum 25. Juni – 30. Juni Die Reaktivierungsgebühr wurde während des Leistungszeitraums 25. Juni – 30. Juni, in dem du zwei Lizenzen hattest, nur für eine Lizenz in Rechnung gestellt. Die Gutschrift von -6 USD hebt die fälschlicherweise erhobene Gebühr für den Leistungszeitraum 25. Juni – 30. Juni auf.
- 12 USD anteilige Nachberechnung für den Leistungszeitraum 25. Juni –30. Juni Der Partner besaß während dieses Leistungszeitraums zwei Lizenzen. Der Preis pro Einheit wird wie folgt berechnet: (30/30)*6*2 = 12 USD.
- 60 USD Gebühr für den Leistungszeitraum 1. Juli – 31. Juli

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20.06.2018   |30.06.2018   |-30 USD   |1   |-30 USD   |Stornierungsgebühr |
|25.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Aktivierungsgebühr |
|25.06.2018   |30.06.2018   |-6 USD   |1   |-6 USD   |Anteiliger Zyklus für Instanz |
|25.06.2018   |30.06.2018   |6 USD   |2   |12 USD   |Anteiliger Zyklus für Instanz |
|01.07.2018   |31.07.2018   |30 USD   |2   |60 USD   |Gebühr für Zyklus |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Szenario 6: Aussetzen eines Abonnements in weniger als 30 Tagen nach dem Kauf und Reaktivieren nach mehr als 30 Tagen nach dem Kaufdatum 

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni kauft der Partner ein neues Abonnement mit einer Lizenz zum Preis von 30 USD pro Monat. Am 5. Juni 2018 setzt der Partner das Abonnement aus. Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni.
- -30 USD Stornierungsgutschrift für den Leistungszeitraum 5. Juni – 30. Juni. Die Gutschrift ist nicht anteilig, da das Abonnement in den ersten 30 Tagen ausgesetzt wurde.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf
|05.06.2018   |30.06.2018   |-30 USD   |1   |-30 USD   |Stornierungsgebühr

Am 10. Juli reaktiviert der Partner das Abonnement. Die Abstimmungsdatei vom 15. Juli enthält in diesem Fall die folgenden Rechnungspositionen:

- 21,30 USD Reaktivierungsgebühr für den Leistungszeitraum 10. Juli – 31. Juli. Reaktivierungen nach 30 Tagen ab dem Kaufdatum werden anteilig berechnet. 

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10.07.2018   |31.07.2018   |21,30 USD   |1   |21,30 USD   |Aktivierungsgebühr |

Die Abstimmungsdatei vom 15. August enthält in diesem Fall die folgenden Rechnungspositionen:
- 30 USD Gebühr für den Leistungszeitraum 1. August – 31. August

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01.08.2018   |31.08.2018   |30 USD   |1   |30 USD   |Gebühr für Zyklus |

Beachten Sie, dass die automatische Verlängerung bei der Aussetzung und Reaktivierung eines Abonnements weiterhin zwölf Monate nach dem ursprünglichen Kaufdatum erfolgt. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Szenario 7: Aussetzen und Reaktivieren eines Abonnements nach mehr als 30 Tagen nach dem Kauf 
Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni kauft der Partner ein neues Abonnement mit einer Lizenz zum Preis von 30 USD pro Monat. 

Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall nur die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |

Der Partner setzt das Abonnement am 5. Juli aus und reaktiviert es am 15. Juli. Die Abstimmungsdatei vom 15. Juli enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juli – 31. Juli.
- -26,14 USD Stornierungsgutschrift für den Leistungszeitraum 5. Juli – 31. Juli Stornierungen nach 30 Tagen ab Kaufdatum führen zu einer anteiligen Gutschrift. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl x (-1) = (30/31) x 27 x 1 x (-1) = -26,14
- 16,45 USD Reaktivierungsgebühr für den Leistungszeitraum 15. Juli–31. Juli. Reaktivierungen nach 30 Tagen ab dem Kaufdatum werden anteilig berechnet. Berechnung: (30/31) x 17 x 1 = 16,45.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01.07.2018   |31.07.2018   |30 USD  |1   |30 USD   |Gebühr für Zyklus |
|05.07.2018   |31.07.2018   |   -26,14 USD   |1   |-26,14 USD|Stornierungsgebühr |
|15.07.2018   |31.07.2018   |16,45 USD   |1   |16,45 USD|Aktivierungsgebühr |

Die Abstimmungsdatei vom 15. August enthält in diesem Fall Folgendes:
- 30 USD Gebühr für den Leistungszeitraum 1. August – 31. August

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01.08.2018   |31.08.2018   |30 USD  |1   |30 USD   |Gebühr für Zyklus |

### <a name="scenario-8-change-of-license-quantity"></a>Szenario 8: Änderung der Lizenzanzahl 

Das Abrechnungsdatum des Partners ist der 15. Am 1. Juni kauft der Partner ein neues Abonnement zum Preis von 30 USD pro Monat. Am 10. Juni erhöht der Partner die Anzahl von Lizenzen von 1 auf 2. Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni. Obwohl der Partner die Anzahl von Lizenzen vor seinem Abrechnungsdatum (15. Juni) erhöht hat, wird die Änderung im Microsoft-Abrechnungssystem nicht vor dem Startdatum des Abonnements (1. Juli) registriert.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |

Am 1. Juli, dem Startdatum des Abonnements, registriert das Microsoft-Abrechnungssystem, dass die Anzahl von Lizenzen am 10. Juni von 1 auf 2 erhöht wurde. Das Abrechnungssystem generiert eine Gutschrift und anteilige Verrechnung für den Leistungszeitraum 1. Juni – 9. Juni und 10. Juni – 30. Juni. 

Die Abstimmungsdatei vom 15. Juli enthält in diesem Fall Folgendes:

- -30 USD Gutschrift für den Leistungszeitraum 1. Juni – 30. Juni.
- 9 USD anteilige Nachberechnung für den Leistungszeitraum 1. Juni – 9. Juni Dies ist der Zeitraum, in dem der Kunde eine Lizenz besaß. Berechnung: (monatlicher Preis/Tage im gesamten Leistungszeitraum) x Tage im anteiligen Leistungszeitraum x Lizenzanzahl = (30/30) x 9 x 1 = 9
- 42 USD anteilige Nachberechnung für den Leistungszeitraum 10. Juni – 30. Juni Dies ist der Zeitraum, in dem der Kunde zwei Lizenzen besaß. Berechnung: (30/30) x 21 x 2 = 42.
- 60 USD Gebühr für den Leistungszeitraum 1. Juli – 31. Juli

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01.06.2018   |30.06.2018   |-30 USD   |1   |-30 USD|Anteiliger Zyklus für Instanz |
|01.06.2018   |09.06.2018   |9 USD   |1   |9 USD|Anteiliger Zyklus für Instanz |
|10.06.2018   |30.06.2018   |21 USD   |2   |42 USD|Anteiliger Zyklus für Instanz |
|01.07.2018   |31.07.2018   |30 USD   |2   |60 USD   |Gebühr für Zyklus |

### <a name="scenario-9-add-on-subscriptions"></a>Szenario 9: Add-On-Abonnements

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 1. Juni kauft der Partner ein neues Abonnement mit einer Lizenz zum Preis von 30 USD pro Monat. Am 10. Juni kauft der Partner ein neues Add-On-Abonnement zum Preis von 5 USD pro Monat. Das Verlängerungsdatum für das Add-On-Abonnement entspricht dem Verlängerungsdatum des Basisabonnements (1. Juni). 

Am 10. Juni kauft der Partner ein Add-On-Abonnement mit einer Lizenz zum Preis von 5 USD pro Monat. 

Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni. Dies ist die Gebühr für das Basisabonnement.
- 3,50 USD anteilige Gebühr für den Leistungszeitraum 10. Juni – 30. Juni Dies ist die Gebühr für das Add-On-Abonnement. 

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01.06.2018   |30.06.2018   |30 USD   |1   |30 USD   |Anteilige Gebühren beim Kauf |
|10.06.2018   |30.06.2018   |3,50 USD   |1   |3,50 USD   |Anteilige Gebühren beim Kauf |

Die Abstimmungsdatei vom 15. Juli enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juli – 31. Juli. Dies ist die Gebühr für das Basisabonnement.
- 5 USD Gebühr für den Leistungszeitraum 1. Juli – 31. Juli Dies ist die Gebühr für das Add-On-Abonnement.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|01.07.2018   |31.07.2018   |30 USD   |1   |30 USD   |Gebühr für Zyklus |
|01.07.2018   |31.07.2018   |5 USD   |1   |5 USD   |Gebühr für Zyklus |

Beachten Sie, dass für das Add-On-Abonnement das automatische Verlängerungsdatum 1. Juni 2019 des Basisabonnements gilt.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Szenario 10: Neukauf am 29., 30. oder 31. 

Das Abrechnungsdatum des Partners ist der 15. jedes Monats. Am 29. Mai kauft der Partner ein neues Abonnement mit einer Lizenz zum Preis von 30 USD pro Monat. Für am 29., 30. oder 31. eines Monats erworbene Abonnements gilt ein kostenloser Zeitraum vom Kaufdatum bis zum 1. des Folgemonats. Das Abonnementdatum ist standardmäßig der 1. des Monats. In diesem Szenario gilt für das Abonnement ein kostenloser Zeitraum vom 29. bis 31. Mai, und der kostenpflichtige Zeitraum von zwölf Monaten beginnt am 1. Juni. 

Die Abstimmungsdatei vom 15. Juni enthält in diesem Fall die folgenden Rechnungspositionen:

- 30 USD Gebühr für den Leistungszeitraum 1. Juni – 30. Juni.

|**Beginn der Abrechnung**   |**Ende der Abrechnung**   |**Preis pro Einheit**   |**Anzahl**   |**Betrag**   |**Gebührenart** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29.05.2018   | 30.06.2018   |30 USD   |1   |30 USD  |Anteilige Gebühren beim Kauf |

Beachten Sie, dass das Abonnement am 1. Juni 2019 automatisch verlängert wird.
