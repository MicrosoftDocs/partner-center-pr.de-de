---
title: Lizenzbasierte Abstimmungsdateien
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie lizenzbasierte Abstimmungsdateien in Partner Center. In diesem Artikel wird die Bedeutung jedes Felds in Ihrer lizenzbasierten Recon-Datei erläutert.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 041f0fadfea107027ae1d9796d235700e66e6834
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146577"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Verstehen der Felder in Partner Center lizenzbasierten Abstimmungsdateien

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Abrechnungsadministrator| Administrator-Agent

Um Ihre Änderungen mit den Bestellungen  eines Kunden abgleichen zu können, vergleichen Sie die Syndication_Partner_Subscription_Number aus der Abstimmungsdatei mit der **Abonnement-ID** Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Felder in lizenzbasierten Abstimmungsdateien

| Column | BESCHREIBUNG | Beispielwert |
| ------ | ----------- | ------------ |
| PartnerId | Eindeutiger Bezeichner im GUID-Format für eine bestimmte Abrechnungsentität. Für die Abstimmung nicht erforderlich. In allen Zeilen gleich. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. *Sehr wichtiges Feld für die Abstimmung der Rechnung mit Ihren Systeminformationen.* | *Testkunde A* |
| MPNID | MPN-Bezeichner des CSP-Partners. Erfahren [Sie, wie Sie nach Partner auf elementisieren.](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *4390934* |
| ResellerMpnId | MPN-Bezeichner des Vertriebspartners des Datensatzes für das Abonnement.  |
| OrderId | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um die Bestellung zu identifizieren, wenn Sie sich an den Support wenden. Wird nicht für die Abstimmung verwendet. | *566890604832738111* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um das Abonnement zu identifizieren, wenn Sie sich an den Support wenden. Wird nicht für die Abstimmung verwendet. *Dieser Wert ist nicht mit der **Abonnement-ID** in der Partner Admin Console identisch. Weitere Informationen finden **Sie stattdessen unter SyndicationPartnerSubscriptionNumber.*** | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Eindeutiger Bezeichner des Abonnements. Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen. Diese Spalte ist wichtig für die Analyse der Abstimmungsdatei. Dieses Feld wird der **Abonnement-ID** in der Partner Admin Console zugeordnet. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Eindeutiger Angebotsbezeichner. Standard-Angebotsbezeichner, wie in der Preisliste definiert. *Dieser Wert stimmt nicht mit der **Angebots-ID** aus der Preisliste überein. Siehe stattdessen **DurableOfferID.*** | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Eindeutiger permanenter Angebotsbezeichner, wie in der Preisliste definiert. *Dieser Wert entspricht der **Angebots-ID** aus der Preisliste.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | Das Startdatum des Abonnements in UTC. Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). Dieses Feld wird auf den Tag festgelegt, an dem der Auftrag übermittelt wurde. Wird mit **SubscriptionEndDate** verwendet, um zu bestimmen, ob sich der Kunde noch innerhalb des ersten Jahres des Abonnements befindet oder ob das Abonnement für das folgende Jahr erneuert wurde. | *2/1/2019 0:00* |
| SubscriptionEndDate | Das Enddatum des Abonnements in UTC. Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). Entweder *12 Monate plus **x** Tage nach dem Startdatum,* um mit dem Abrechnungsdatum des Partners in Einklang zu bringen, oder *12 Monate nach dem Verlängerungsdatum.* Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert. Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich. | *2/1/2019 0:00* |
| ChargeStartDate | Der erste Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). Wird verwendet, um tägliche Gebühren *(anteilige* Gebühren) zu berechnen, wenn ein Kunde Lizenznummern ändert. | *2/1/2019 0:00* |
| ChargeEndDate | Letzter Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. Wird verwendet, um tägliche Gebühren *(anteilige* Gebühren) zu berechnen, wenn ein Kunde Lizenznummern ändert. | *2/28/2019 23:59* |
| ChargeType | Die [Art der Gebühr](recon-file-charge-types.md) oder Anpassung. | Weitere Informationen [finden Sie unter Gebührentypen.](recon-file-charge-types.md) |
| UnitPrice | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dies den Informationen entspricht, die während der Abstimmung in Ihrem Abrechnungssystem gespeichert sind. | *6.82* |
| Menge | Anzahl der Lizenzen. Stellen Sie sicher, dass dies den Informationen entspricht, die während der Abstimmung in Ihrem Abrechnungssystem gespeichert sind. | *2* |
| Amount (Betrag) | Gesamtpreis für die Menge Wird verwendet, um zu überprüfen, ob die Berechnung des Betrags der Berechnung dieses Werts für Ihre Kunden entspricht. | *13.32* |
| TotalOtherDiscount | Rabattbetrag auf diese Gebühren. Produktlizenzen, die in einer Kompetenz oder maps enthalten sind, oder neue Abonnements, die für einen Incentive berechtigt sind, enthalten ebenfalls einen Rabattbetrag in dieser Spalte. | *2.32* |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern Überprüft, ob Ihre Teilsumme mit der erwarteten Summe im Falle eines Rabatts entspricht. | *11* |
| Tax (Steuern) | Steuerbetragsgebühr. Basierend auf den Steuerregeln Ihres Markts und bestimmten Umständen. | *0* |
| TotalForCustomer | Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden. | *11* |
| Währung | Währungstyp. Jede Abrechnungsentität weist nur eine Währung auf. Überprüfen Sie, ob sie ihrer ersten Rechnung entspricht. Überprüfen Sie es nach allen wichtigen Updates der Abrechnungsplattform erneut. | *EUR* |
| DomainName | Domänenname des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. *Verwenden Sie dieses Feld nicht als eindeutigen Bezeichner für den Kunden. Der Kunde/Partner kann die Vanity- oder Standarddomäne über das Office 365-Portal aktualisieren.* | *example.onmicrosoft.com* |
| SubscriptionName | Spitzname des Abonnements. Wenn kein Spitzname angegeben ist, verwendet Partner Center **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Dies ist ein identisches Feld mit **OfferName**.) | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
| AbrechnungszyklusTyp | Häufigkeit der einmaligen Abrechnung.| *Monatlich* |
