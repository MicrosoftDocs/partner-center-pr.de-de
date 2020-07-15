---
title: Lizenzbasierte Abstimmungsdateien
ms.topic: article
ms.date: 05/18/2020
description: Erfahren Sie, wie Sie Lizenz basierte ababstimmungs Dateien im Partner Center lesen. In diesem Artikel wird die Bedeutung der einzelnen Felder in ihrer lizenzbasierten Reconnaissance-Datei erläutert.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cd275c074bb3710a2a438d65989b16a1be398830
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377694"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Grundlegendes zu den Feldern in den lizenzbasierten Abstimmungs Dateien von Partner Center

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**
- Globaler Administrator
- Benutzeradministrator
- Abrechnungsadministrator
- Administrator-Agent

Vergleichen Sie die **Syndication_Partner_Subscription_Number** aus der Abstimmungs Datei mit der **Abonnement-ID** aus Partner Center, um Ihre Änderungen mit den Aufträgen eines Kunden abzustimmen.

## <a name="fields-in-license-based-reconciliation-files"></a>Felder in lizenzbasierten Abstimmungs Dateien

| Spalte | BESCHREIBUNG | Beispielwert |
| ------ | ----------- | ------------ |
| PartnerId | Eindeutiger Bezeichner im GUID-Format für eine bestimmte Abrechnungs Entität. Für die Abstimmung nicht erforderlich. In allen Zeilen gleich. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. *Sehr wichtiges Feld für die Abstimmung der Rechnung mit ihren Systeminformationen.* | *Testkunde A* |
| MPNID | MPN-Bezeichner des CSP-Partners. Weitere Informationen finden [Sie unter Vorgehensweise beim itemisieren nach Partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| Resellermpnid | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement.  |
| OrderId | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um die Reihenfolge zu identifizieren, in der der Support kontaktiert Wird nicht für die Abstimmung verwendet. | *566890604832738111* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann beim Kontaktieren des Supports hilfreich sein, um das Abonnement zu identifizieren. Wird nicht für die Abstimmung verwendet. *Dieser Wert ist nicht mit der Abonnement- **ID** in der Partner Administrator Konsole identisch. Weitere Informationen finden Sie unter **syndicationpartnerabonnementionnumber** .* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Eindeutiger Bezeichner des Abonnements. Ein Kunde kann über mehrere Abonnements für denselben Plan verfügen. Diese Spalte ist wichtig für die Analyse der Abgleich Datei. Dieses Feld wird der **Abonnement-ID** in der Partner Administrator Konsole zugeordnet. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Eindeutige Angebots Kennung. Standard Angebots Bezeichner, wie in der Preisliste definiert. *Dieser Wert stimmt nicht mit der **Angebots-ID** aus der Preisliste. Siehe **durableofferid** .* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Eindeutiger Bezeichner für permanente Angebote, wie in der Preisliste definiert. *Dieser Wert entspricht der **Angebots-ID** aus der Preisliste.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | Das Startdatum des Abonnements. Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). Dieses Feld ist auf den Tag festgelegt, an dem die Bestellung übermittelt wurde. Wird in Verbindung mit dem Abonnement **Enddatum** verwendet, um zu bestimmen, ob sich der Kunde noch innerhalb des ersten Jahres des Abonnements befindet oder ob das Abonnement für das folgende Jahr erneuert wurde. | *2/1/2019 0:00* |
| SubscriptionEndDate | Das Enddatum des Abonnements. Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). Entweder *12 Monate Plus **x** Tage nach dem Startdatum* , um das Abrechnungsdatum des Partners oder *12 Monate ab dem Erneuerungsdatum*auszurichten. Bei Verlängerung werden die Preise gemäß der aktuellen Preisliste aktualisiert. Vor einer automatischen Verlängerung ist möglicherweise die Kommunikation mit dem Kunden erforderlich. | *2/1/2019 0:00* |
| ChargeStartDate | Der erste Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). Wird verwendet, um tägliche Gebühren zu berechnen (*pro-anteiliger* Gebühren), wenn ein Kunde die Arbeitsplatz Nummern | *2/1/2019 0:00* |
| ChargeEndDate | Letzter Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. Wird verwendet, um tägliche Gebühren zu berechnen (*pro-anteiliger* Gebühren), wenn ein Kunde die Arbeitsplatz Nummern | *2/28/2019 23:59* |
| ChargeType | Der [Typ der Belastung](recon-file-charge-types.md) oder der Anpassung. | Siehe " [Abrechnung](recon-file-charge-types.md)". |
| UnitPrice (Stückpreis) | Preis pro Arbeitsplatz entsprechend der Preisliste zum Kaufzeitpunkt. Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert | *6,82* |
| Menge | Anzahl der Arbeitsplätze Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert | *2* |
| Betrag | Gesamtpreis für die Menge Wird verwendet, um zu überprüfen, ob die Betrag Berechnung mit der Berechnung dieses Werts für Ihre Kunden übereinstimmt. | *13,32* |
| TotalOtherDiscount | Rabattbetrag auf diese Gebühren. Produktlizenzen, die in einer Kompetenz oder in Karten enthalten sind, oder neue Abonnements, die für einen Anreiz geeignet sind, enthalten in dieser Spalte ebenfalls einen Rabatt Betrag. | *2,32* |
| Subtotal (Zwischensumme) | Gesamtbetrag vor Steuern Überprüft, ob Ihr Teilergebnis mit dem erwarteten Gesamtbetrag übereinstimmt, falls ein Rabatt vorliegt. | *11* |
| Tax (Steuern) | Steuern der Steuerbeträge. Basierend auf den Steuerregeln Ihres Marktes und bestimmten Bedingungen. | *0* |
| TotalForCustomer | Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden. | *11* |
| Währung | Währungstyp. Jede Abrechnungsentität weist nur eine Währung auf. Überprüfen Sie, ob Sie Ihrer ersten Rechnung entspricht. Überprüfen Sie nach allen wichtigen Updates der Abrechnungs Plattform erneut. | *EUR* |
| DomainName | Der Domänen Name des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. *Verwenden Sie dieses Feld nicht als eindeutigen Bezeichner für den Kunden. Der Kunde/Partner kann die Vanity oder die Standard Domäne über das Office 365-Portal aktualisieren.* | *example.onmicrosoft.com* |
| SubscriptionName | Spitzname des Abonnements. Wenn kein Spitzname angegeben ist, verwendet Partner Center den **Offername**. | *Project Online* |
| SubscriptionDescription | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Dies ist ein identisches Feld für " **Offername**".) | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
| AbrechnungszyklusTyp | Einmalige Abrechnungs Häufigkeit.| *Monatlich* |