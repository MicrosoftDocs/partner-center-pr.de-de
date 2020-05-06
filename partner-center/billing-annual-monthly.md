---
title: Monatliche und jährliche Abrechnungs Unterschiede | Partner Center
ms.topic: article
ms.date: 11/25/2019
Description: Erfahren Sie mehr über die Unterschiede zwischen monatlichen und jährlichen Abrechnungszyklen im Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09e651638e50afeef3d43dd9c35c11998ba904ca
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798598"
---
# <a name="monthly-and-annual-billing-differences"></a>Unterschiede zwischen monatlicher und jährlicher Abrechnung

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Globaler Administrator
- Incentiveadministrator
- Incentivebenutzer
- Helpdesk-Agent
- Vertriebsbeauftragter

In diesem Thema werden die Unterschiede zwischen **monatlicher Abrechnung** und **jährlicher Abrechnung** in Partner Center erläutert, einschließlich Vorteilen und Anwendungsfällen. Sie haben die Möglichkeit, monatlich oder jährlich für bestimmte CSP-Abonnements (Cloud Solution Provider) zu bezahlen.

## <a name="applicability"></a>Anwendbarkeit

Die meisten lizenzierten Abonnements haben die Möglichkeit, eine monatliche oder jährliche Abrechnungs Option zu erhalten. Für nutzungsbasierte Abonnements ist nur die monatliche Abrechnung verfügbar.

Sowohl die jährliche als auch die monatliche Abrechnung erfolgt **pro Abonnement**, ** *nicht* pro Lizenz**.

### <a name="find-subscription-applicability"></a>Suchen von Abonnement Anwendbarkeit

Sie können die verfügbaren Abrechnungs Frequenzen für jedes Angebot mithilfe der Spalte J in der Angebots Matrix identifizieren. Die Angebots Matrix finden Sie im Abschnitt " **Angebote und Preise** " im Partner Center.

### <a name="applicable-partners"></a>Anwendbare Partner

Alle Partner und Partner Typen können monatlich oder jährlich abgerechnet werden.

### <a name="applicable-markets"></a>Anwendbare Märkte

Monatliche und jährliche Abrechnung (für anwendbare Angebote) ist in allen Märkten verfügbar, in denen das CSP-Programm zurzeit verfügbar ist.

## <a name="change-billing-frequency"></a>Ändern der Abrechnungshäufigkeit

Sie können jederzeit zwischen monatlicher und jährlicher Abrechnung wechseln. Möglicherweise möchten Sie die Abrechnungs Häufigkeit ändern, wenn sich Ihre geschäftlichen Anforderungen ändern.

Wenn Sie die Abrechnungs Häufigkeit in jährlich ändern, wird die Jahres Laufzeit aktualisiert, um das Datum widerzuspiegeln, an dem Sie die Abrechnungs Häufigkeit geändert haben. Außerdem wird ein neues Erneuerungsdatum eingerichtet.

### <a name="monthly-to-annual-billing"></a>Monatliche Abrechnung

Der Wechsel von der monatlichen Abrechnung zur jährlichen Abrechnung kann nützlich sein, wenn Sie über zahlreiche Abonnements verfügen, die monatlich abgerechnet werden. Wenn Sie zur jährlichen Abrechnung wechseln, können Sie die Abonnements auf ein gängiges Abrechnungsdatum ausrichten.

### <a name="annual-to-monthly-billing"></a>Abrechnung jährlich in monatlicher Abrechnung

Die Umstellung von der jährlichen Abrechnung auf die monatliche Abrechnung kann nützlich sein, wenn Sie Ihre Abrechnungsdaten an die einzelnen Kunden anpassen möchten.

## <a name="annual-billing"></a>Jährliche Abrechnung

Die jährliche Abrechnung bietet folgende Vorteile:

- Mehr Flexibilität im Hinblick auf die Zahlungsoptionen
- Bessere Abstimmung mit der Fakturierung Ihrer Kunden
- Geringere Auswirkungen von Wechselkursschwankungen
- Reduzierte Betriebskosten für die Abrechnung

### <a name="configure-annual-billing"></a>Konfigurieren der jährlichen Abrechnung

Wenn Sie beabsichtigen, zur jährlichen Abrechnung in Partner Center zu wechseln, achten Sie darauf, dass Sie die Auswirkungen auf Ihre Verkaufs Bewegung in Erwägung gezogen haben. Informieren Sie Ihr Team, und aktualisieren Sie die internen Prozesse nach Bedarf. Sie sollten auch Änderungen an Ihrer Rechnung und der lizenzbasierten Abstimmungs Datei überprüfen. 

Außerdem müssen Sie [Ihre APIs für die jährliche Abrechnung aktualisieren](#required-api-changes).

#### <a name="required-api-changes"></a>Erforderliche API-Änderungen

Um die jährliche Abrechnung nutzen zu können, müssen Sie einige Änderungen an Ihren APIs vornehmen.

- [Order. billingcycle (Eigenschaft)](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Erstellen eines Auftrags](https://docs.microsoft.com/partner-center/develop/create-an-order)

Weitere Informationen zu Partner Center-APIs finden Sie unter alle [Partner Center-Entwickler Ressourcen und-Dokumentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Platzieren von Aufträgen

Der Abrechnungs Frequenztyp, einschließlich der jährlichen Abrechnung, wird dem **Angebot** als Attribut zugewiesen. Es gibt kein eindeutiges Angebot für Aufträge mit jährlicher Abrechnung. Sie können jedoch ein Angebot mithilfe eines kundenfreundlicheren namens umbenennen, um es leicht zu unterscheiden.

### <a name="select-annual-billing"></a>Jährliche Abrechnung auswählen

Wenn Sie ein neues Abonnement hinzufügen, werden Sie aufgefordert, die Abrechnungs Häufigkeit auszuwählen. An dieser Stelle können Sie die Option für jährliche Abrechnung auswählen. Wenn Sie die jährliche Abrechnung auswählen, werden alle verfügbaren Angebote angezeigt.

### <a name="billing-time"></a>Abrechnungszeit

Ihnen wird das nächste Abrechnungsdatum in Rechnung gestellt. Wenn Ihr Abrechnungsdatum z. b. der 1. Tag des Monats ist und Sie ein Abonnement, das jährlich in Rechnung gestellt wird, ab dem 29. Oktober 2019, wird Ihnen der 1. November 2019 in Rechnung gestellt. Vorausgesetzt, dass Sie keine Lizenzänderungen vornehmen, werden Sie am 1. November 2020 erneut in Rechnung gestellt. Wenn Sie eine Lizenzänderung vornehmen, erhalten Sie ein Guthaben und können sich beim nächsten Abrechnungsdatum anmelden.

### <a name="annual-renewals"></a>Jährliche Erneuerungen

Das Erneuerungsdatum Ihres Abonnements liegt bei 12 Monaten nach dem Startdatum des dienstanzvorgangs. Der Leistungszeitraum beginnt an dem Datum, an dem das Abonnement erstellt wird.  Beispielsweise wird ein Abonnement, das am 10. Januar 2019 erstellt wurde, am 10. Januar 2020 erneuert.

Die Rechnungslegung erfolgt am nächsten Abrechnungsdatum nach dem Verlängerungsdatum des Abonnements. Wenn Sie beispielsweise am 15. Januar 2018 ein Abonnement mit jährlicher Abrechnung erwerben und Ihr Abrechnungsdatum der 20. Januar ist, wird Ihr Abonnement am 15. Januar 2019 verlängert. Die Verlängerung wird Ihnen am 20. Januar 2019 in Rechnung gestellt.

### <a name="split-subscription-billing-frequency"></a>Abrechnungs Häufigkeit für das Aufteilen von Abonnements

Es ist nicht möglich, ein **einzelnes Abonnement** aufzuteilen, damit ein Teil monatlich abgerechnet wird und der andere Teil jährlich abgerechnet wird. Das gesamte Abonnement muss über dieselbe Abrechnungs Häufigkeit verfügen (entweder monatliche oder jährliche Abrechnung).

Für Kunden, die über **mehrere Abonnements** desselben Angebots verfügen, ist es möglicherweise möglich, unterschiedliche Abrechnungs Frequenzen pro Abonnement zu haben. Bestimmte Angebote sind auf ein Abonnement pro Kunde beschränkt. Wenn für das Angebot keine Einschränkung gelten, kann ein Kunde mehrere Abonnements für das gleiche Angebot mit unterschiedlichen Abrechnungshäufigkeiten besitzen. Details zu allen Angebotseinschränkungen sind in der Spalte „I“ der Angebotsmatrix angegeben. Die Angebots Matrix finden Sie im Abschnitt " **Angebote und Preise** " im Partner Center.

### <a name="free-subscription-period"></a>Kostenloser Abonnementzeitraum

Abonnements mit jährlicher Abrechnungs Häufigkeit erhalten keinen kostenlosen Zeitraum. Der kostenpflichtige 12-Monats-Zeitraum beginnt mit dem Kauf Datum. Dies unterscheidet sich von Abonnements mit monatlicher Abrechnung, für die nach dem Kauf ein kostenloser Zeitraum bis zum nächsten Abrechnungsdatum gilt.

### <a name="adding-and-removing-licenses"></a>Hinzufügen und Entfernen von Lizenzen

Sie können die Anzahl von Lizenzen für Ihre Abonnements jederzeit ändern. Das Hinzufügen zusätzlicher Lizenzen hat keinen Einfluss auf die Abrechnungshäufigkeit.

Sie können jederzeit Lizenzen hinzufügen oder entfernen.  Nachdem Sie die Anzahl der Lizenzen geändert haben, erhalten Sie eine Gutschrift und eine anteilsmäßig Abrechnungen für das nächste Abrechnungsdatum.

Wenn für Ihr vorhandenes Abonnement eine jährliche Abrechnung erfolgt, ist es nicht möglich, Lizenzen mit monatlicher Abrechnung für dieses Abonnement hinzuzufügen. Nach dem Kauf eines Abonnements mit jährlicher Abrechnung gilt diese Abrechnungshäufigkeit für alle zusätzlichen Lizenzen. Wenn Sie Lizenzen mit monatlicher Abrechnung benötigen, müssen Sie ein neues Abonnement kaufen.

### <a name="add-on-offers"></a>Add-on-Angebote

Dem Add-On-Abonnement wird automatisch die gleiche Abrechnungshäufigkeit zugewiesen wie dem übergeordneten Abonnement. Die jährliche Abrechnung ist für Add-on-Angebote verfügbar. 

### <a name="cancelling-subscriptions"></a>Abonnements werden abgebrochen

Für alle Abrechnungshäufigkeiten gelten die gleichen Kündigungsbedingungen.

Wenn das Abonnement in den ersten 30 Tagen der kostenpflichtigen zwölfmonatigen Abrechnung abgebrochen wird, erhalten Sie bei der jährlichen Abrechnung eine Gutschrift von 100% beim nächsten Abrechnungsdatum. Wenn das Abonnement nach 30 Tagen des kostenpflichtigen zwölfmonatigen Zeitraums abgebrochen wird, erhalten Sie beim nächsten Abrechnungsdatum eine Anteils mäßige Gutschrift.

### <a name="moving-subscriptions-between-partners"></a>Verschieben von Abonnements zwischen Partnern

Kunden können Abonnements nicht zwischen Partnern verschieben. Dies gilt für Abonnements mit monatlicher und jährlicher Abrechnung.

Der neue Partner muss im Auftrag des Kunden ein neues Abonnement erwerben. Es ist nicht möglich, Abonnements zwischen Partnern zu verschieben.

### <a name="reactivating-subscriptions"></a>Erneutes Aktivieren von Abonnements

Sie können ein Abonnement für bis zu 90 Tage nach dem Ablaufdatum erneut aktivieren. Die anteilig e Gebühr wird zum folgenden Abrechnungsdatum in Rechnung gestellt. Das Verlängerungsdatum des Abonnements bleibt unverändert.

## <a name="pricing"></a>Preise

### <a name="offer-pricing"></a>Angebotspreise

Der Angebotspreis zum Zeitpunkt des Kaufs ist für die Abonnement Laufzeit garantiert (ein Monat für die monatliche Abrechnung, 12 Monate für die jährliche Abrechnung). Wenn ein Abonnement verlängert wird, gilt der Preis in der aktuellen Preisliste zum Zeitpunkt der Verlängerung. Der neue Preis ist für die nächste Abonnement Laufzeit garantiert.

Wenn sich der Preis eines Angebots während des Abrechnungszeitraums verringert, ändert sich der Betrag, den Sie in Rechnung stellen, nicht. Der Preis wird für den vollständigen Abrechnungszeitraum zum Zeitpunkt des Kaufs festgelegt. Dies gilt sowohl für die monatliche als auch für die jährliche Abrechnung.

### <a name="cancellation-credits"></a>Abbruch Guthaben

Die Gutschrift für eine abgebrochene Lizenz oder ein Abonnement wird wie folgt berechnet:

**Abbruch Guthaben** = ((* * monatliche Preis * * * 12)/365) \* **Tage verbleiben in der zwölfmonatigen** \* Anzahl von Lizenzen, die abgebrochen wurden.

## <a name="reconciliation-file"></a>Abstimmungsdatei

### <a name="find-subscriptions-billing-frequency"></a>Suchen der Abrechnungs Häufigkeit des Abonnements

In der Spalte **AA** der Abstimmungs Datei erfahren Sie, ob Ihr Abonnement monatlich oder jährlich abgerechnet wird.

Informationen dazu, ob Sie ein monatliches Abonnement für die jährliche Abrechnung ändern können, finden Sie unter [Suchen von Abonnements](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Abstimmungs Dateiänderungen für die jährliche Abrechnung

Wenn Sie ein Abonnement mit jährlicher Abrechnung erwerben oder erneuern, ändert sich Ihre Lizenz basierte Abstimmungs Datei wie folgt:

- Es gibt eine neue Zeile in der lizenzbasierten Abstimmungs Datei, die beim ersten Abrechnungsdatum nach dem Kauf oder einem neuen Abonnement erstellt wird.

- Wenn keine Änderungen am Abonnement vorgenommen werden, gibt es für die Abstimmungs Dateien keine Zeilen für die Monate 2 bis 12 der Abonnement Laufzeit. Wenn während der zwölfmonatigen Laufzeit eine Änderung an dem Abonnement vorgenommen wird, werden ein Guthaben und eine anteilsmäßig aufgenommene Rechnung in der nächsten Abstimmungs Datei angezeigt, nachdem die Änderung vorgenommen wurde.

- Die nächste Änderung an der Abstimmungs Datei wird angezeigt, wenn das Abonnement erneuert wird. Diese Änderung erscheint am ersten Abrechnungsdatum nach der Verlängerung.

### <a name="usage-file-changes-for-annual-billing"></a>Änderungen an der Nutzungs Datei für die jährliche Abrechnung

Die folgenden Abonnement Änderungen, die im Jahr abgerechnet werden, werden in der Spalte P ihrer Nutzungs Datei angezeigt:

- Anteilsmäßig **Kosten bei Kauf**: der anfängliche Erwerb eines Jahresabonnements.
- **Zyklisch instanzanstanzwert**: Lizenzänderungen, die zu Guthaben und einer erneuten Abrechnung führen.
- **Abbruchgebühr**: der [Abbruch eines jährlichen Abonnements](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Abbruch des Jahresabonnements

Wenn ein Abonnement, das jährlich abgerechnet wird, abgebrochen wird, enthält die Abstimmungs Datei ein Zeilen Element für eine Abbruch Gutschrift.

Wenn der Abbruch in den ersten 30 Tagen der 12-monatigen Laufzeit erfolgt, wird das Abonnement bei 100 Prozent gutgeschrieben. Wird das Abonnement nach den ersten 30 Tagen storniert, wird der anteilige Betrag dem Abonnement gutgeschrieben

### <a name="adding-licenses-to-annual-subscription"></a>Hinzufügen von Lizenzen zum Jahresabonnement

Wenn Sie einem Abonnement Lizenzen hinzufügen, enthält die Abstimmungs Datei ein Guthaben und eine anteilsmäßig aufgehende Rechnung. Dies gilt für monatliche und jährlich in Rechnung gestellte Abonnements.

### <a name="price-lists-for-annual-billing"></a>Preislisten für die jährliche Abrechnung

In den Preislisten für Partner Center werden die monatlichen Preise angezeigt. Es ist kein Jahrespreis aufgeführt. Sie können den jährlichen Preis berechnen, indem Sie den monatlichen Preis um 12 multiplizieren.

### <a name="offer-matrix"></a>Angebots Matrix

Angebots-IDs in der Angebots Matrix sind für alle Abrechnungs Häufigkeiten identisch. Es gibt keine eindeutigen IDs für Angebote, die jährlich abgerechnet werden können.

## <a name="incentives"></a>Incentives

### <a name="incentives-calculation"></a>Berechnung der Anreize

Die Anreize werden basierend auf dem **Umsatz in Rechnung**gestellt, ** *nicht* **mit dem Umsatz. Erzielte Anreizzahlungen werden im Einklang mit unserer Richtlinien gezahlt, wie in den CSP-Anreizhandbüchern aufgeführt.

Wenn ein Abonnement, das jährlich in Rechnung gestellt wird, verkauft wird, wird der Umsatz dieses Abonnements für die Berechnung von Anreizen basierend auf dem berechneten Umsatz erkannt.

### <a name="payout"></a>Auszahlung

Zurzeit werden alle Incentive-Zahlungen zweimal pro Jahr durchgeführt. Diese Zahlungen erfolgen 45 Tage nach Halbjahresende.

### <a name="rates"></a>Rates

Partner erhalten für alle berechtigten Transaktionen, unabhängig davon, wie ein Abonnement in Rechnung gestellt wird, Anreize. Der Incentive-Gewinn wird basierend auf der globalen Incentive-Rate (die für den Zeitraum abgerechnet wird), der lokalen Zugriffstaste (für alle Regionen, in denen es lokale Beschleuniger gibt) und allen globalen Kampagnen (falls zutreffend) berechnet.

### <a name="contacts"></a>Kontakte

Wenden Sie sich an das entsprechende Support Team von Regional Incentives

| Region | E-Mail-Adresse |
| ------ | ------------- |
| Nordamerika | <ocina@microsoft.com> |
|Lateinamerika & Brasilien | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| Apoac (mit Ausnahme von Japan) | <ociapgc@microsoft.com> |
| Japan | <ocijp@microsoft.com> |


### <a name="suspension"></a>Ten

Wenn Sie ein Abonnement (in Partner Center oder über die APIs) innerhalb von 30 Tagen erwerben, erhalten Sie eine Gutschrift von 100%, unabhängig von der Abrechnungs Häufigkeit.

Bei jährlicher Abrechnung:

1. Der Partner kauft das Abonnement am 1. Januar. Für den Dienst Zeitraum vom 1. Januar bis zum 31. Dezember wird eine Abrechnungsgebühr abgerechnet.
2. Der Partner hält das Abonnement am 25. Januar an. Für den Dienst Zeitraum vom 1. Januar bis zum 31. Dezember wird eine Kredit Abrechnungs Linie erstellt.
3. Der Partner aktiviert das Abonnement am 29. Januar erneut. Für den Dienst Zeitraum aus dem 29. Januar bis zum 31. Dezember wird eine Abrechnungsgebühr abgerechnet.

Für monatliche Abrechnung:

1. Der Partner kauft das Abonnement am 1. Januar. Für den Dienst Zeitraum vom 1. Januar bis zum 31. Januar wird eine Abrechnungsgebühr abgerechnet.
2. Der Partner hält das Abonnement am 25. Januar an. Für den Dienst Zeitraum vom 1. Januar bis zum 31. Januar wird eine Kredit Abrechnungs Linie erstellt.
3. Der Partner aktiviert das Abonnement am 29. Januar erneut. Für den Dienst Zeitraum aus dem 29. Januar bis zum 31. Januar wird eine Abrechnungsgebühr abgerechnet.
