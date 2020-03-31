---
title: Häufige Abrechnungs Szenarien für Lizenz basierte Saas-Transaktionen | Partner Center
ms.topic: article
ms.date: 03/26/2020
description: Erfahren Sie mehr über häufige Abrechnungs Szenarien im Partner Center für Lizenz basierte Saas-Transaktionen.
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
Keywords: Abrechnung, Zahlungen, einmaliger Kauf, wiederkehrende Käufe, Abonnements, Arbeitsplätze
ms.localizationpriority: medium
ms.openlocfilehash: b509278166d858c64cfab6c98a27c266f9bc2c55
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390099"
---
# <a name="billing-scenarios-for-license-based-saas-transactions"></a>Abrechnungs Szenarien für Lizenz basierte Saas-Transaktionen

**Geeignete Rollen**

- Administratoragent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter


Diese Beispiel [Szenarien für allgemeine Abrechnung](common-billing-scenarios.md) gelten für Lizenz basierte Saas-Abonnements (Software-as-a-Service) im Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konvertieren eines kostenlosen Saas-Test Abonnements in ein kostenpflichtiges Abonnement

In diesem Szenario wird die Abrechnung für die Erneuerung eines lizenzbasierten kostenlosen Testversion von Saas-Abonnements beschrieben. Bei der Verlängerung wird die kostenlose Testversion am Ende des kostenlosen Testzeitraums in ein kostenpflichtiges Abonnement konvertiert.

In diesem Beispiel haben Sie am 10. Juni eine kostenlose Testversion eines lizenzbasierten Saas-Abonnements (Software-as-a-Service) erworben. Diese kostenlose Testversion wird beim Ende der kostenlosen Testversion automatisch als kostenpflichtiges Abonnement erneuert.

Die Datei für die Wiederaufnahme umfasst die folgenden Gebühren:

| Kaufdatum | Startdatum der Abrechnung | Enddatum der Abrechnung | Preis pro Einheit | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 1 | $0 | Neu | Kostenlose Testversion |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Verlängern | Kostenpflichtiges Abonnement |

## <a name="cancel-a-free-trial-saas-subscription"></a>Kündigen Sie ein kostenloses Saas-Testabonnement an

> [!TIP]
> Sie können auch während des kostenlosen Testzeitraums jederzeit ein Lizenz basiertes Abonnement für die kostenlose Testversion von Saas kündigen.

In diesem Szenario haben Sie am 1. Juli ein Lizenz basiertes Abonnement für eine kostenlose Testversion von Saas erworben und dann sofort im Partner Center abgebrochen.

Die Datei "Reconnaissance" enthält die folgenden Gebühren:

| Kaufdatum | Startdatum der Abrechnung | Enddatum der Abrechnung | Preis pro Einheit | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 11 | $0 | Neu | Kostenlose Testversion |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 11 | $0 | Abbrechen | Kostenlose Testversion |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konvertieren eines benutzerdefinierten Abrechnungs-Saas-Abonnements in eine andere SKU

In diesem Szenario wird beschrieben, wie Sie ein benutzerdefiniertes Abrechnungs-Saas-Abonnement von einem Stock Keeping Unit (SKU) in eine andere SKU für das gleiche Produkt am gleichen Datum konvertieren.

In diesem Szenario haben Sie eine SKU (Silver) unter einem Produkt erworben und in eine andere verfügbare SKU (Bronze) unter diesem Produkt zum gleichen Datum konvertiert.

Die Datei "Reconnaissance" enthält die folgenden Gebühren:

| Kaufdatum | SKU | Startdatum der Abrechnung | Enddatum der Abrechnung | Preis pro Einheit | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silber | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Neu | Benutzerdefiniertes Abrechnungs Abonnement für Saas |
| 06/10/2019 | Silber | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -$20 | Konvertieren | Anteilsmäßig angeforderte Rechnung für benutzerdefiniertes Abrechnungs-Saas-Abonnement |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 € | 1 | 10 € | Konvertieren | Benutzerdefiniertes Abrechnungs Abonnement für Saas |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Erwerben und kündigen eines Kunden Abrechnungs-Saas-Abonnements am gleichen Datum

In diesem Szenario wird die Abrechnung für ein SaaS-Abonnement für Kunden Zähler beschrieben, das Sie über die Azure-Portal zum gleichen Zeitpunkt erworben und abgebrochen haben.

In diesem Szenario haben Sie ein benutzerdefiniertes Abrechnungs Abonnement für SaaS-Abonnements auf der Azure-Portal erworben. Anschließend haben Sie das Abonnement am gleichen Datum abgebrochen.

| Kaufdatum | SKU | Startdatum der Abrechnung | Enddatum der Abrechnung | Preis pro Einheit | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 € | 1 | 10 € | Neu | Benutzerdefiniertes Abrechnungs Abonnement für Saas |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 € | 1 | -$10 | CancelImmediate | Benutzerdefiniertes Abrechnungs Abonnement für Saas |
