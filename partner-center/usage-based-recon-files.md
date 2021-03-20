---
title: Nutzungsbasierte Abstimmungsdateien
ms.topic: article
ms.date: 06/08/2020
description: Erfahren Sie mehr über alle Elemente in ihrer nutzungsbasierten Abstimmungs Datei im Partner Center. Enthält einige Beispiele.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 403b2704c600f21fc06576e679ff538a74ae5046
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712969"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Grundlegendes zu nutzungsbasierten Abstimmungs Dateien und ihren spezifischen Feldern im Partner Center

**Geeignete Rollen**

- Kontoadministrator
- Abrechnungsadministrator

Wenn Sie Ihre Kosten mit der Nutzung eines Kunden abstimmen möchten, vergleichen Sie **resellerid**, **resellername** und **resellerbillableaccount** aus der Abstimmungs Datei mit dem **Kundennamen** und der **Abonnement-ID** aus Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Felder in Verwendungs basierten Abstimmungs Dateien

Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.

| Column | BESCHREIBUNG | Beispiel Wert (e) |
| ------ | ----------- | ------------ |
| PartnerId | Die Partner-ID im GUID-Format. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Name des Partners | *"Configuration Manager", Ltd.* |
| Partnerbillableaccountid | ID des Partner Kontos. | *1010578050* |
| CustomerCompanyName | Der in Partner Center angegebene Organisationsname des Kunden. *Sehr wichtig für die ababstimmung der Rechnung mit ihren Systeminformationen.* | *Test Kunde* |
| MPNID | MPN-Bezeichner des CSP-Partners. | *4390934* |
| Resellermpnid | MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement.  |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. | *D020001IVK* |
| ChargeStartDate | Startdatum des Abrechnungszyklus, ausgenommen bei der Darstellung von Daten zu den zuvor nicht fakturierten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). | *2/1/2019 0:00* |
| ChargeEndDate | Enddatum des Abrechnungszyklus, ausgenommen bei der Darstellung von Daten zu den zuvor nicht fakturierten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. | *2/28/2019 23:59* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann beim Kontaktieren des Supports hilfreich sein, um das Abonnement zu identifizieren. Wird nicht für die Abstimmung verwendet. *Dies ist nicht mit der Abonnement- **ID** in der Partner Administrator Konsole identisch.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Spitzname für das Dienst Angebot. | *Microsoft Azure* |
| SubscriptionDescription | Geschäftssparte des Dienstangebots. | *Microsoft Azure* |
| OrderID | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann beim Kontaktieren des Supports hilfreich sein, um das Abonnement zu identifizieren. Wird nicht für die Abstimmung verwendet. | *566890604832738111* |
| Dienstname | Der Name des fraglichen Azure-Dienstes | *virtuelle Computer* |
| ServiceType | Der spezifische Typ des Azure-Dienstanbieter. | *Service Bus – Einzel-oder Paket* *SQL Azure Datenbank – Business oder Web Edition* |
| ResourceGuid | Der jeweilige eindeutige Bezeichner für alle Dienstdaten und Preisstrukturen. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| Ressourcenname | Der Name der Azure-Ressource. | *Datenübertragung in (GB)*, *Datenübertragung ausgehend (GB)* |
| Region | Der Bereich, für den die Verwendung gilt. Wird hauptsächlich zum Zuweisen von Raten zu Datenübertragungen verwendet, da die Preise je nach Region variieren. | *Asien-Pazifik*, *Europa*, *Lateinamerika*, *Nordamerika* |
| Sku | Eindeutiger Microsoft-Bezeichner für ein Angebot. | *7UD-00001* |
| DetailLineItemId | Ein Bezeichner und eine Menge zum itemisieren verschiedener Raten für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum. Für mehrstufige Azure-Preise kann eine Rate für bis zu einer bestimmten Menge abrechenbare Einheiten und dann eine andere Rate nach dieser Menge festgelegt werden. | *1* |
| ConsumedQuantity | Der Umfang des genutzten dienplatzes (z. b. Stunden oder GB) während des Berichtszeitraums. Dieser bezieht auch die nicht fakturierte Nutzung aus vorherigen Berichtszeiträumen ein. | *11* |
| IncludedQuantity | Die im Rahmen des Angebots enthaltenen Einheiten. In der Regel nicht im CSP vorhanden. | *0* |
| OverageQuantity | Einheiten, die nicht im Rahmen des Angebots enthalten sind. Diese müssen vom Partner bezahlt werden. Entspricht **consumedmenge** minus **includecodmenge**. | *11* |
| ListPrice | Der Preis für das Abonnement ist für das Startdatum des Abonnements wirksam. | *0,0808 $* |
| PretaxCharges | Entspricht **listprist** multipliziert mit **overagemenge**, gerundet auf den nächstgelegenen Prozentwert. | *0,085 $* |
| TaxAmount | Gebührenpflichtig. Basierend auf den Steuerregeln Ihres Marktes und bestimmten Bedingungen. | *$0,08* |
| PostTaxTotal | Der Gesamtbetrag nach Steuern, sofern Steuern anfallen. | *$0,93* |
| Währung | Währungstyp. Jede Abrechnungsentität weist nur eine Währung auf. Überprüfen Sie, ob es mit ihrer ersten Rechnung und nach allen wichtigen Updates der Abrechnungs Plattform übereinstimmt. | *EUR* |
| PretaxEffectiveRate | Preis pro Einheit vor Steuern. Entspricht **pretaxcharges** dividiert durch **overagemenge**, gerundet auf den nächstgelegenen Prozentwert. | *$0,08* |
| PostTaxEffectiveRate | Preis pro Einheit nach Steuern. Entspricht **posttaxtotal** dividiert durch **overagemenge**, gerundet auf den nächstgelegenen Prozentwert. Oder, gleich **pretaxeffectiverate** zuzüglich des Steuersatzes pro Einheiten Betrag, auf den nächstgelegenen Cent gerundet. | *$0,08* |
| ChargeType | Der [Typ der Belastung](recon-file-charge-types.md) oder der Anpassung. | Siehe " [Abrechnung](recon-file-charge-types.md)". |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Der Domänen Name des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. | *example.onmicrosoft.com* |
| AbrechnungszyklusTyp | Zeit Abrechnungs Häufigkeit.| **Monatlich**  |
| Einheit | Die Einheit des Ressourcen **namens**. | *GB* oder *Stunden* |
| CustomerBillableAccount | Eindeutige Konto Kennung in der Microsoft-Abrechnungs Plattform. | *1280018095* |
| UsageDate | Datum der Dienstbereitstellung. | *2/1/2019 0:00* |
| MeteredRegion | Gibt den Speicherort eines Rechenzentrums innerhalb der Region an (für Dienste, bei denen dieser Wert anwendbar und aufgefüllt ist). | *Asien, Osten*, *Süd Asien, Osten*, *Europa, Norden*, *Europa, Westen*, USA, Norden- *Mitte*, USA, *Süden-Mitte* |
| MeteredService | Gibt die Verwendung einzelner Azure-Dienste an, wenn diese nicht explizit in der **Service Name** -Spalte identifiziert werden. Beispielsweise werden Datenübertragungen in der Spalte **Service Name** als *Microsoft Azure-all-Dienste* gemeldet. | *AccessControl*, *CDN*, *Compute*, *Datenbank*, *ServiceBus*, *Speicher* |
| MeteredServiceType | Unterüberschrift für das Feld " **meteredservice** ", das weitere Erläuterungen zur Nutzung von Azure-Diensten bietet. | *EXTERNAL* |
| Project | Benutzerdefinierter Name für die jeweilige Dienstinstanz. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Die Anzahl der Azure Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und verwendet wurden. | *1,000000 Verbindungen/30 Tage* (wenn Sie über eine einzeln bereitgestellte Verbindung während eines 30-tägigen Monats verfügen), *25 Verbindungen/30 Tage – wird verwendet: 1,000000* (wenn Sie über ein 25 Pack Service Bus Verbindungen verfügen und 1 an diesem Tag verwendet haben) |

## <a name="next-steps"></a>Nächste Schritte

- [Grundlegendes zu den Feldern in den lizenzbasierten Abstimmungs Dateien von Partner Center](license-based-recon-files.md)