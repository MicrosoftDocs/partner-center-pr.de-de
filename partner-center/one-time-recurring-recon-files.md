---
title: Einmalige und wiederkehrende Abstimmungs Dateien | Partner Center
ms.topic: article
ms.date: 01/03/2020
description: Grundlegendes zu einmaligen und wiederkehrenden Abstimmungs Dateien im Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6f381189fc1d8fad692ef248dcdcbf5ab8b0af43
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757233"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Einmalige und wiederkehrende Abstimmungs Dateien

**Gilt für**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Abrechnungsadministrator
-   Administratoragent
-   Vertriebsbeauftragter

In diesem Thema wird erläutert, wie Sie einmalige und wiederkehrende Abstimmungs Dateien im Partner Center lesen.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Felder in einmaligen und wiederkehrenden Abgleich Dateien

| Spalte | Beschreibung |
| ------ | ----------- |
| PartnerID | Eindeutige Azure Active Directory (Azure AD)-Mandanten Bezeichner für eine bestimmte Abrechnungs Entität im GUID-Format. Für die Abstimmung nicht erforderlich. In allen Zeilen gleich. |
| Kunden-ID | Eindeutige Azure AD Mandanten-ID im GUID-Format. Identifiziert den Kunden. |
| CustomerName | Der in Partner Center angegebene Organisationsname des Kunden. |
| CustomerDomainName | Der Domänen Name des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. *Verwenden Sie dieses Feld nicht als eindeutigen Bezeichner für den Kunden. Der Kunde/Partner kann die Vanity oder die Standard Domäne über das Office 365-Portal aktualisieren.* |
| CustomerCountry | Das Land/eine Region, in dem sich der Kunde befindet. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
| MPNID | MPN-Bezeichner des CSP-Partners. |
| OrderID | Eindeutiger Bezeichner für eine Bestellung auf der Microsoft Commerce Platform. Wird nicht für die Abstimmung verwendet. |
| Bestellungsdatum | Das Datum, an dem die Bestellung aufgegeben wurde. |
| ProductID | Der Bezeichner für das Produkt. |
| SkuID | Der Bezeichner für eine bestimmte SKU (Stock-Keeping Unit). |
| AvailabilityId | Der Bezeichner für die Verfügbarkeit einer bestimmten SKU. Dies zeigt, ob die SKU für den Erwerb in den jeweiligen Ländern, Währungen, Industriesegmenten usw. verfügbar ist. |
| SkuName | Der Titel einer bestimmten SKU. |
| ProductName | Name des Produkts. |
| ChargeType | Art der Gebühren oder der Anpassung. |
| UnitPrice | Der in der Preisliste zum Zeitpunkt des Kaufs veröffentlichte Einheitspreis. *Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert* |
| Anzahl | Anzahl der Einheiten. *Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert* |
| SubTotal | Gesamtbetrag vor Steuern Überprüft, ob Ihr Teilergebnis mit dem erwarteten Gesamtbetrag übereinstimmt, falls ein Rabatt vorliegt. |
| TaxTotal | Steuern der Steuerbeträge. Basierend auf den Steuerregeln Ihres Marktes und bestimmten Bedingungen. |
| Gesamt | Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden. |
| Währung | Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Stellen Sie sicher, dass dies mit ihrer ersten Rechnung übereinstimmt, und prüfen Sie nach allen wichtigen Updates der Abrechnungs Plattform. |
| Preis Beschreibung | Eine Erklärung der geltenden Rabatte. |
| PublisherName | Der Name des Herausgebers des Produkts.
| PublisherId | Eindeutiger Bezeichner für einen bestimmten Verleger. |
| SubscriptionDescription | Anzeigename eines Abonnements. |
| Abonnement-ID | Eindeutiger Bezeichner eines Abonnements auf der Microsoft Commerce Platform. Wird nicht für die Abstimmung verwendet. *Dieser Bezeichner ist nicht mit der **Abonnement-ID** in der Partner Administrator Konsole identisch.* |
| ChargeStartDate | Der erste Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. |
| ChargeEndDate | Letzter Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| Termandbillingcycle | Die Begriffs Länge und der Abrechnungszeitraum für den Erwerb (z. b. *1 Jahr, monatlich*). |
| Effectiveunitprice | Der Preis pro Einheit, nachdem Anpassungen vorgenommen wurden. |
| UnitType | Der Typ der Einheit, die gekauft wird. |
| AlternateId | Ein alternativer **Bezeichner**für eine Auftrags-ID. |
| Billablemenge | Stellt die Gesamtanzahl erworbener oder genutzter Einheiten dar. |
| Billingfrequency | Beschreibt, ob das Zeilen Element monatlich oder einmalig abgerechnet wird. *Dies wird derzeit nur für Azure RI unterstützt, wobei die unterstützten Werte monatlich unterstützt werden. Wenn das RI-Programm mit einer einmaligen Abrechnungs Frequenz erworben wird, wird dieses Feld in der Datei "Recon" leer angezeigt.* |
| PricingCurrency | Der Listenpreis der Ressource oder des Angebots. |
| Pctobcexchangerate | Wechselkurs für Preiswährung auf Abrechnungswährung. |
| Pctobcexchangeratedate | Das Datum, an dem die Preiswährung der Abrechnungswährung festgelegt wird. |
| Meterbeschreibung | Die Verbrauchseinheit für das Verbrauchs Zeilen Element. |


