---
title: Nutzungsbasierte Abstimmungs Dateien | Partner Center
ms.topic: article
ms.date: 01/08/2020
description: Alle Elemente in ihrer Verwendungs basierten Abstimmungs Datei wurden mit Beispielen erläutert.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d0b50240ec62f10a202c3ad0de3d6425aec878ef
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757223"
---
# <a name="usage-based-file-fields"></a>Nutzungsbasierte Dateifelder

Betrifft

- Partner Center
- Partner Center für Microsoft Cloud for US Government

Wenn Sie Ihre Kosten mit der Nutzung eines Kunden abstimmen möchten, vergleichen Sie **resellerid**, **resellername**und **resellerbillableaccount** aus der Abstimmungs Datei mit dem **Kundennamen** und der **Abonnement-ID** aus Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Felder in Verwendungs basierten Abstimmungs Dateien

Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.

| Spalte | Beschreibung | Beispiel Wert (e) |
| ------ | ----------- | ------------ |
| PartnerID | Die Partner-ID im GUID-Format. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Name des Partners | *"Configuration Manager", Ltd.* |
| Partnerbillableaccountid | ID des Partner Kontos. | *1010578050* |
| CustomerCompanyName | Der in Partner Center angegebene Organisationsname des Kunden. *Sehr wichtig für die ababstimmung der Rechnung mit ihren Systeminformationen.* | *Test Kunde* |
| MPNID | MPN-Bezeichner des CSP-Partners. | *4390934* |
| Resellermpnid | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement. Für die aktuelle Aktivität nicht verfügbar. |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. | *D020001IVK* |
| ChargeStartDate | Startdatum des Abrechnungszyklus, ausgenommen bei der Darstellung von Daten zu den zuvor nicht fakturierten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer auf den Tagesbeginn um 0:00 Uhr festgelegt. | *2/1/2019 0:00* |
| ChargeEndDate | Enddatum des Abrechnungszyklus, ausgenommen bei der Darstellung von Daten zu den zuvor nicht fakturierten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. | *2/28/2019 23:59* |
| Abonnement-ID | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann beim Kontaktieren des Supports hilfreich sein, um das Abonnement zu identifizieren. Wird nicht für die Abstimmung verwendet. *Dies ist nicht mit der Abonnement- **ID** in der Partner Administrator Konsole identisch.* | *"US cbmgaaaaaaaaia"* |
| SubscriptionName | Spitzname für das Dienst Angebot. | *Microsoft Azure* |
| SubscriptionDescription | Geschäftssparte des Dienstangebots. | *Microsoft Azure* |
| OrderID | Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform. Kann beim Kontaktieren des Supports hilfreich sein, um das Abonnement zu identifizieren. Wird nicht für die Abstimmung verwendet. | *566890604832738111* |
| ServiceName | Der Name des fraglichen Azure-Dienstes | *virtuelle Computer* |
| ServiceType | Der spezifische Typ des Azure-Dienstanbieter. | *Service Bus – Einzel-oder Paket* *SQL Azure Datenbank – Business oder Web Edition* |
| ResourceGuid | Bestimmter eindeutiger Bezeichner für alle Dienstdaten und die Preisstruktur. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| Ressourcenname | Der Name der Azure-Ressource. | *Datenübertragung in (GB)* , *Datenübertragung ausgehend (GB)* |
| Region | Der Bereich, für den die Verwendung gilt. Wird hauptsächlich zum Zuweisen von Raten zu Datenübertragungen verwendet, da die Preise je nach Region variieren. | *Asien-Pazifik*, *Europa*, *Lateinamerika*, *Nordamerika* |
| Sku | Eindeutiger Microsoft-Bezeichner für ein Angebot. | *7ud-00001* |
| DetailLineItemId | Ein Bezeichner und eine Menge zum itemisieren verschiedener Raten für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum. Für mehrstufige Azure-Preise kann eine Rate für bis zu einer bestimmten Menge abrechenbare Einheiten und dann eine andere Rate nach dieser Menge festgelegt werden. | *1* |
| ConsumedQuantity | Der Umfang des genutzten dienplatzes (z. b. Stunden oder GB) während des Berichtszeitraums. Enthält außerdem jede nicht berechnete Nutzung aus dem vorherigen Berichtszeitraum. | *11* |
| IncludedQuantity | Enthaltene Einheiten als Teil des Angebots. In der Regel nicht im CSP vorhanden. | *0* |
| OverageQuantity | Einheiten, die nicht im Rahmen des Angebots enthalten sind. Diese müssen vom Partner bezahlt werden. Entspricht **consumedmenge** minus **includecodmenge**. | *11* |
| ListPrice | Der Preis für das Abonnement ist für das Startdatum des Abonnements wirksam. | *$0,0808* |
| PretaxCharges | Entspricht **listprist** multipliziert mit **overagemenge**, gerundet auf den nächstgelegenen Prozentwert. | *$0,085* |
| TaxAmount | Gebührenpflichtig. Basierend auf den Steuerregeln Ihres Marktes und bestimmten Bedingungen. | *$0,08* |
| PostTaxTotal | Gesamtbetrag nach Steuern, wo Steuern berechnet werden. | *$0,93* |
| Währung | Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Überprüfen Sie, ob es mit ihrer ersten Rechnung und nach allen wichtigen Updates der Abrechnungs Plattform übereinstimmt. | *Betragen* |
| PretaxEffectiveRate | Nettopreis pro Einheit. Entspricht **pretaxcharges** dividiert durch **overagemenge**, gerundet auf den nächstgelegenen Prozentwert. | *$0,08* |
| PostTaxEffectiveRate | Bruttopreis pro Einheit. Entspricht **posttaxtotal** dividiert durch **overagemenge**, gerundet auf den nächstgelegenen Prozentwert. Oder entspricht **pretaxeffectiverate** zuzüglich der Steuerquote pro Einheiten-Amoun, gerundet auf den nächstgelegenen Prozentsatz. | *$0,08* |
| ChargeType | Der [Typ der Belastung](recon-file-charge-types.md) oder der Anpassung. | Siehe " [Abrechnung](recon-file-charge-types.md)". |
| Kunden-ID | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Der Domänen Name des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. | *example.onmicrosoft.com* |
| AbrechnungszyklusTyp | Zeit Abrechnungs Häufigkeit.| **Monatlich**  |
| Einheit | Die Einheit des Ressourcen **namens**. | *GB* oder *Stunden* |
| CustomerBillableAccount | Eindeutige Konto Kennung in der Microsoft-Abrechnungs Plattform. | *1280018095* |
| UsageDate | Datum der Service-Bereitstellung. | *2/1/2019 0:00* |
| MeteredRegion | Gibt den Speicherort eines Rechenzentrums innerhalb der Region an (für Dienste, bei denen dieser Wert anwendbar und aufgefüllt ist). | *Asien, Osten*, *Süd Asien, Osten*, *Europa, Norden*, *Europa, Westen*, USA, Norden- *Mitte*, USA, *Süden-Mitte* |
| MeteredService | Gibt die Verwendung einzelner Azure-Dienste an, wenn diese nicht explizit in der **Service Name** -Spalte identifiziert werden. Beispielsweise werden Datenübertragungen in der Spalte **Service Name** als *Microsoft Azure-all-Dienste* gemeldet. | *AccessControl*, *CDN*, *Compute*, *Datenbank*, *ServiceBus*, *Speicher* |
| MeteredServiceType | Unterüberschrift für das Feld " **meteredservice** ", das weitere Erläuterungen zur Nutzung von Azure-Diensten bietet. | *EXTERNAL* |
| Projizieren | Benutzerdefinierter Name für die jeweilige Dienstinstanz. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Die Anzahl der Azure Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und verwendet wurden. | *1,000000 Verbindungen/30 Tage* (wenn Sie über eine einzeln bereitgestellte Verbindung während eines 30-tägigen Monats verfügen), *25 Verbindungen/30 Tage – wird verwendet: 1,000000* (wenn Sie über ein 25 Pack Service Bus Verbindungen verfügen und 1 an diesem Tag verwendet haben) |
