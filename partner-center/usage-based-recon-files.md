---
title: Nutzungsbasierte Abstimmungsdateien
ms.topic: article
ms.date: 06/08/2020
description: Erfahren Sie mehr über alle Elemente in Ihrer nutzungsbasierten Abstimmungsdatei in Partner Center. Enthält einige Beispiele.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431702"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Informationen zu verwendungsbasierten Abstimmungsdateien und deren spezifischen Feldern in Partner Center

**Geeignete Rollen:** Kontoadministrator-| Abrechnungsadministrator

Um Ihre Gebühren mit der Nutzung eines Kunden in Einklang zu bringen, vergleichen Sie **ResellerID,** **ResellerName** und **ResellerBillableAccount** aus der Abstimmungsdatei mit dem Kundennamen und der Abonnement-ID Partner Center.  

## <a name="fields-in-usage-based-reconciliation-files"></a>Felder in verwendungsbasierten Abstimmungsdateien

Die folgenden Felder enthalten Informationen zu den verwendeten Diensten und den Raten.

| Spalte | Beschreibung | Beispielwerte |
| ------ | ----------- | ------------ |
| PartnerId | Partnerbezeichner im GUID-Format. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Name des Partners | *Contoso, Ltd.* |
| PartnerBillableAccountId | Partnerkontobezeichner. | *1010578050* |
| CustomerCompanyName | Der in Partner Center angegebene Organisationsname des Kunden. *Dieser ist für die Abstimmung der Rechnung mit Ihren Systeminformationen sehr wichtig.* | *Testkunde* |
| MPNID | Microsoft Partner Network (MPN) des Cloud Solution Provider -Partners (CSP). | *4390934* |
| ResellerMpnId | MPN-Bezeichner des Vertriebspartners des Datensatzes für das Abonnement.  |
| InvoiceNumber | Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. | *D020001IVK* |
| ChargeStartDate | Startdatum des Abrechnungszyklus, ausgenommen bei der Darstellung von Daten zu den zuvor nicht fakturierten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer der Tagesanfang (0:00 Uhr). | *2/1/2019 0:00* |
| ChargeEndDate | Enddatum des Abrechnungszyklus, ausgenommen bei der Darstellung von Daten zu den zuvor nicht fakturierten latenten Nutzungsdaten (aus dem vorherigen Abrechnungszyklus). Die Uhrzeit ist immer auf das Tagesende um 23:59 Uhr festgelegt. | *2/28/2019 23:59* |
| SubscriptionId | Eindeutiger Bezeichner für ein Abonnement auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um das Abonnement zu identifizieren, wenn Sie sich an den Support wenden. Wird nicht für die Abstimmung verwendet. *Dies ist nicht mit der **Abonnement-ID** in der Partner Admin Console identisch.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Spitzname für das Dienstangebot. | *Microsoft Azure* |
| SubscriptionDescription | Geschäftssparte des Dienstangebots. | *Microsoft Azure* |
| OrderID | Eindeutiger Bezeichner für einen Auftrag auf der Microsoft-Abrechnungsplattform. Kann nützlich sein, um das Abonnement zu identifizieren, wenn Sie sich an den Support wenden. Wird nicht für die Abstimmung verwendet. | *566890604832738111* |
| Dienstname | Der Name des fraglichen Azure-Dienstes | *VIRTUELLE COMPUTER* |
| ServiceType | Der spezifische Typ des Azure-Diensts. | *Service Bus – Einzeln oder Pack*, SQL *Azure-Datenbank – Business oder Web Edition* |
| ResourceGuid | Der jeweilige eindeutige Bezeichner für alle Dienstdaten und Preisstrukturen. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| Ressourcenname | Der Name der Azure-Ressource. | *Datenübertragung in (GB),* *Datenübertragung aus (GB)* |
| Region | Die Region, für die die Nutzung gilt. Wird hauptsächlich zum Zuweisen von Raten zu Datenübertragungen verwendet, da die Raten je nach Region variieren. | *Asien-Pazifik*, *Europa*, *Lateinamerika*, *Nordamerika* |
| Sku | Eindeutiger Microsoft-Bezeichner für ein Angebot. | *7UD-00001* |
| DetailLineItemId | Ein Bezeichner und eine Menge zum Auffüllen verschiedener Tarife für einen Dienst oder eine Ressource in einem bestimmten Abrechnungszeitraum. Für mehrstufige Azure-Preise kann es einen Tarif für bis zu eine bestimmte Menge authentifizierungsfähiger Einheiten und dann einen anderen Tarif nach dieser Menge geben. | *1* |
| ConsumedQuantity | Die Menge der während des Berichtszeitraums verbrauchten Dienste (z. B. Stunden oder GB). Dieser bezieht auch die nicht fakturierte Nutzung aus vorherigen Berichtszeiträumen ein. | *11* |
| IncludedQuantity | Die im Rahmen des Angebots enthaltenen Einheiten. In der Regel nicht in CSP vorhanden. | *0* |
| OverageQuantity | Einheiten, die nicht im Angebot enthalten sind. Diese müssen vom Partner bezahlt werden. Entspricht **ConsumedQuantity minus** **IncludedQuantity**. | *11* |
| ListPrice | Angebotspreis, der zum Startdatum des Abonnements wirksam ist. | *0,0808 $* |
| PretaxCharges | Entspricht **ListPrist multipliziert** mit **OverageQuantity**, gerundet auf den nächsten Cent. | *0,085 $* |
| TaxAmount | In Rechnung gestellter Steuerbetrag. Basierend auf den Steuerregeln Ihres Markts und bestimmten Umständen. | *0,08 USD* |
| PostTaxTotal | Der Gesamtbetrag nach Steuern, sofern Steuern anfallen. | *0,93 USD* |
| Währung | Währungstyp. Jede Abrechnungsentität weist nur eine Währung auf. Überprüfen Sie, ob sie Ihrer ersten Rechnung entspricht, und überprüfen Sie dann, ob die Abrechnungsplattform aktualisiert wurde. | *Eur* |
| PretaxEffectiveRate | Preis pro Einheit vor Steuern. Entspricht **PretaxCharges** dividiert durch **OverageQuantity**, gerundet auf den nächsten Cent. | *0,08 USD* |
| PostTaxEffectiveRate | Preis pro Einheit nach Steuern. Entspricht **PostTaxTotal dividiert** durch **OverageQuantity**, gerundet auf den nächsten Cent. Oder entspricht **PretaxEffectiveRate** zuzüglich des Steuersatzes pro Einheit, gerundet auf den nächsten Cent. | *0,08 USD* |
| ChargeType | Der [Typ der Gebühr oder](recon-file-charge-types.md) Anpassung. | Weitere Informationen [finden Sie unter Gebührentypen.](recon-file-charge-types.md) |
| CustomerId | Eindeutiger Microsoft-Bezeichner für den Kunden im GUID-Format. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Domänenname des Kunden. Dieses Feld wird ggf. bis zum zweiten Abrechnungszyklus leer angezeigt. | *example.onmicrosoft.com* |
| AbrechnungszyklusTyp | Häufigkeit der Zeitabrechnung.| **Monatlich**  |
| Einheit | Die Einheit des **Ressourcennamens.** | *GB* oder *STUNDEN* |
| CustomerBillableAccount | Eindeutiger Kontobezeichner auf der Microsoft-Abrechnungsplattform. | *1280018095* |
| UsageDate | Datum der Dienstbereitstellung. | *2/1/2019 0:00* |
| MeteredRegion | Identifiziert den Standort eines Rechenzentrums in der Region (für Dienste, bei denen dieser Wert anwendbar und aufgefüllt ist). | *Asien, Osten*, *Asien, Osten, Europa,* *Norden,* *Europa,* *Westen,* USA, Norden-Mitte, USA, *Süden-Mitte* |
| MeteredService | Identifiziert die Nutzung einzelner Azure-Dienste, wenn sie nicht ausdrücklich in der **Spalte ServiceName angegeben** ist. Datenübertragungen werden z. B. als *Microsoft Azure Alle Dienste* in der Spalte **ServiceName** gemeldet. | *AccessControl,* *CDN,* *Compute,* *Datenbank,* *ServiceBus,* *Speicher* |
| MeteredServiceType | Unterüberheadung für **das Feld "MeteredService",** das zusätzliche Erläuterungen zur Nutzung von Azure-Diensten bietet. | *EXTERNAL* |
| Project | Benutzerdefinierter Name für die jeweilige Dienstinstanz. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Die Anzahl Azure Service Bus Verbindungen, die an einem bestimmten Tag bereitgestellt und genutzt wurden. | *1.000.0000 Verbindungen/30* Tage (bei einer individuell bereitgestellten Verbindung während eines 30-tägigen Monats), *25 Verbindungen/30 Tage – Verwendet: 1.000.0000* (wenn ein 25-Paket mit Service Bus-Verbindungen bereitgestellt wurde und Sie während dieses Tages 1 verwendet haben) |

## <a name="next-steps"></a>Nächste Schritte

- [Verstehen der Felder in Partner Center lizenzbasierten Abstimmungsdateien](license-based-recon-files.md)