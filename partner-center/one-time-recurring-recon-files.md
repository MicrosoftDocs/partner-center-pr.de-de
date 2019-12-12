---
title: Einmalige und wiederkehrende Abstimmungs Dateien | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Grundlegendes zu einmaligen und wiederkehrenden Abstimmungs Dateien im Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 51c37c9ea2110b7666c4d1a9bc92a2b01f92209c
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004899"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Einmalige und wiederkehrende Abstimmungs Dateien

**Zielgruppe**

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

| Column | Beschreibung |
| ------ | ----------- |
| PartnerID | Eindeutige Azure Active Directory (Azure AD)-Mandanten Bezeichner für eine bestimmte Abrechnungs Entität im GUID-Format. Für die Abstimmung nicht erforderlich. In allen Zeilen gleich. |
| Kunden-ID | Eindeutige Azure AD Mandanten-ID im GUID-Format. Identifiziert den Kunden. |
| Kundenname | Der in Partner Center angegebene Organisationsname des Kunden. |
| CustomerDomainName | Der Domänen Name des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. *Verwenden Sie dieses Feld nicht als eindeutigen Bezeichner für den Kunden. Der Kunde/Partner kann die Vanity oder die Standard Domäne über das Office 365-Portal aktualisieren.* |
| Land des Kunden | Das Land, in dem sich der Kunde befindet. |
| Rechnungsnummer | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
| MPNID | MPN-Bezeichner des CSP-Partners. |
| MPN-ID des Handelspartners | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement. |
| Bestellnummer | Eindeutiger Bezeichner für eine Bestellung auf der Microsoft Commerce Platform. Wird nicht für die Abstimmung verwendet. |
| Bestellungsdatum | Das Datum, an dem die Bestellung aufgegeben wurde. |
| ProductID | Der Bezeichner für das Produkt. |
| SkuId | Der Bezeichner für eine bestimmte SKU (Stock-Keeping Unit). |
| AvailabilityId | Der Bezeichner für die Verfügbarkeit einer bestimmten SKU. Dies zeigt, ob die SKU für den Erwerb in den jeweiligen Ländern, Währungen, Industriesegmenten usw. verfügbar ist. |
| SKU-Name | Der Titel einer bestimmten SKU. |
| Produktname | Name des Produkts. |
| PublisherName | Der Name des Herausgebers des Produkts.
| PublisherID | Eindeutiger Bezeichner für einen bestimmten Verleger. |
| Abonnementbeschreibung | Anzeigename eines Abonnements. |
| Abonnement-ID | Eindeutiger Bezeichner eines Abonnements auf der Microsoft Commerce Platform. Wird nicht für die Abstimmung verwendet. *Dieser Bezeichner ist nicht mit der **Abonnement-ID** in der Partner Administrator Konsole identisch.* |
| ChargeStartDate | Der erste Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. |
| ChargeEndDate | Letzter Tag, an dem Gebühren anfallen. Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| Laufzeit und Abrechnungszyklus | Die Begriffs Länge und der Abrechnungszeitraum für den Erwerb (z. b. *1 Jahr, monatlich*). |
| Gebührenart | Art der Gebühren oder der Anpassung. |
| Preis pro Einheit | Der in der Preisliste zum Zeitpunkt des Kaufs veröffentlichte Einheitspreis. *Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert* |
| Effektiver Preis pro Einheit | Der Preis pro Einheit, nachdem Anpassungen vorgenommen wurden. |
| Anzahl | Anzahl der Einheiten. *Stellen Sie sicher, dass dies mit den Informationen übereinstimmt, die im Abrechnungssystem während der Abstimmung gespeichert* |
| Typ der Einheit | Der Typ der Einheit, die gekauft wird. |
| DiscountDetails | Eine Erklärung der geltenden Rabatte. |
| Zwischensumme | Gesamtbetrag vor Steuern Überprüft, ob Ihr Teilergebnis mit dem erwarteten Gesamtbetrag übereinstimmt, falls ein Rabatt vorliegt. |
| Steuern gesamt | Steuern der Steuerbeträge. Basierend auf den Steuerregeln Ihres Marktes und bestimmten Bedingungen. |
| Gesamt | Gesamtsumme nach Steuern. Überprüft, ob in der Rechnung Steuern berechnet werden. |
| Währung | Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Stellen Sie sicher, dass dies mit ihrer ersten Rechnung übereinstimmt, und prüfen Sie nach allen wichtigen Updates der Abrechnungs Plattform. |
| AlternateID | Ein alternativer **Bezeichner**für eine Auftrags-ID. |
