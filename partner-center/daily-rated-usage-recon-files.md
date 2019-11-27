---
title: Nutzungs Abgleich-Dateien mit täglicher Bewertung | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Grundlegendes zu Nutzungs Abgleich-Dateien für die tägliche Bewertung in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389698"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Nutzungs Abgleich-Dateien mit täglicher Bewertung

Gilt für:

- Partner Center
- Partner Center für Microsoft Cloud for US Government

In diesem Thema wird erläutert, wie Sie Nutzungs Abgleich-Dateien mit täglicher Bewertung lesen.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Felder in den Nutzungs Abgleich-Dateien mit täglicher Bewertung

| Spalte | Description |
| ------ | ----------- |
| PartnerID | Die Partner-ID im GUID-Format. |
| PartnerName | Name des Partners. |
| Kunden-ID | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. |
| CustomerCompanyName | Firmenname des Kunden wie im Partner Center angegeben. *Diese Spalte ist sehr wichtig, um die Rechnung mit ihren Systeminformationen abzustimmen.* |
| CustomerDomainName | Der Domänen Name des Kunden. Für die aktuelle Aktivität nicht verfügbar. |
| Land des Kunden | Das Land, in dem sich der Kunde befindet. |
| MPNID | MPN-Bezeichner des CSP-Partners. |
| MPN-ID des Handelspartners | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement. Für die aktuelle Aktivität nicht verfügbar. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. Für die aktuelle Aktivität nicht verfügbar. |
| ProductID | Der Bezeichner für das Produkt. |
| SkuId | Der Bezeichner für eine bestimmte SKU. |
| AvailabilityId | Der Bezeichner für die Verfügbarkeit einer bestimmten SKU. Dies zeigt, ob die SKU für den Erwerb in den jeweiligen Ländern, Währungen, Industriesegmenten usw. verfügbar ist. |
| SKU-Name | Der Titel einer bestimmten SKU. |
| PublisherName | Der Name des Herausgebers. |
| PublisherID | Der Bezeichner des Verlegers im GUID-Format. Für die aktuelle Aktivität nicht verfügbar. |
| Abonnementbeschreibung | Der Name des Service-Angebots, das der Kunde gekauft hat, wie in der Preisliste definiert. (Dies ist ein identisches Feld für **Offername**). |
| Abonnement-ID | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Wird nicht für die Abstimmung verwendet. *Dieser Bezeichner ist nicht mit der **Abonnement-ID** in der Partner Administrator Konsole identisch.* |
| ChargeStartDate | Das Start Datum des Abrechnungszeitraums (außer bei der Darstellung von Datumsangaben für zuvor nicht berechnete latente Verwendungs Daten aus dem vorherigen Abrechnungszeitraum). Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. |
| ChargeEndDate | Das Enddatum des Abrechnungszeitraums (außer bei der Darstellung von Datumsangaben für zuvor nicht berechnete latente Verwendungs Daten aus dem vorherigen abbildral). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. |
| Nutzungsdatum | Datum der Nutzung des Diensts. |
| Typ der Verbrauchseinheit | Der Typ der Verbrauchseinheit. |
| Kategorie der Verbrauchseinheit | Der Dienst der obersten Ebene für die Nutzung. |
| ID der Verbrauchseinheit | Der Bezeichner für die Verbrauchseinheit, die verwendet wird. |
| Unterkategorie der Verbrauchseinheit | Der Typ des Azure-Dienstanbieter, der die Rate beeinflussen kann. |
| Name der Verbrauchseinheit | Die Maßeinheit für die genutzte Verbrauchseinheit. |
| Region der Verbrauchseinheit | Diese Spalte gibt den Standort eines Rechenzentrums in der Region für die Dienste an, auf die dies zutrifft. |
| Einheit | Die Einheit des Ressourcen **namens**. |
| Verbrauchte Menge | Der Umfang des genutzten dienplatzes (z. b. *Stunden* oder *GB*) während des Berichtszeitraums. Beinhaltet jegliche nicht berechnete Nutzung aus vorherigen Berichterstattungs Zeiträumen. |
| Ressourcenspeicherort | > dem Rechenzentrum, in dem die Verbrauchseinheit ausgeführt wird. |
| Genutzter Dienst | Der Azure-Plattformdienst, den Sie verwendet haben. |
| Ressourcen-URI | Der URI der verwendeten Ressource. |
| Gebührenart | Art der Gebühren oder der Anpassungen. Für die aktuelle Aktivität nicht verfügbar. |
| Preis pro Einheit | Preis pro Lizenz, wie in der Preisliste zum Zeitpunkt des Kaufs veröffentlicht. Stellen Sie sicher, dass dieser Preis den im Abrechnungssystem während der Abstimmung gespeicherten Informationen entspricht. |
| Anzahl | Anzahl der Lizenzen. Stellen Sie sicher, dass dieser Preis den im Abrechnungssystem während der Abstimmung gespeicherten Informationen entspricht. |
| Typ der Einheit | Der Typ der Einheit, mit der die Verbrauchseinheit in Rechnung gestellt wird. Für die aktuelle Aktivität nicht verfügbar. |
| Abrechnung vor Steuern | Gesamtbetrag der Abrechnung vor Steuern. |
| Abrechnungswährung | Die Währung in der geografischen Region des Kunden. |
| Preise vor Steuern gesamt | Die Preise vor Hinzufügen von Steuern. |
| Währung der Preise | Die Währung in der Preisliste. |
| Dienstinformationen 1 | Die Anzahl der Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und verwendet wurden. |
| Dienstinformationen 2 | Ein Legacyfeld, in dem optionale dienstspezifische Metadaten erfasst werden. |
| Zusätzliche Infos | Zusätzliche Informationen, die von anderen Spalten nicht abgedeckt werden. |
