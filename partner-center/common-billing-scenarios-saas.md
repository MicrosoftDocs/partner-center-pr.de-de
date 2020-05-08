---
title: Abrechnungs Lizenz basierte Saas-Transaktionen
ms.topic: article
ms.date: 05/05/2020
description: Erfahren Sie mehr über häufige Abrechnungs Szenarien im Partner Center für Lizenz basierte Saas-Transaktionen.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: Abrechnung, Zahlungen, einmaliger Kauf, wiederkehrende Käufe, Abonnements, Arbeitsplätze
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 02a50f5be3c19f179014fd7db4e1418ba025e874
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908195"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Häufige Abrechnungs Szenarien für Lizenz basierte Saas-Transaktionen im Partner Center

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Helpdesk-Agent
- Vertriebsbeauftragter


Diese Beispiel [Szenarien für allgemeine Abrechnung](common-billing-scenarios.md) gelten für Lizenz basierte Saas-Abonnements (Software-as-a-Service) im Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konvertieren eines kostenlosen Saas-Test Abonnements in ein kostenpflichtiges Abonnement

In diesem Szenario wird die Abrechnung für die Erneuerung eines lizenzbasierten kostenlosen Testversion von Saas-Abonnements beschrieben. Bei der Verlängerung wird die kostenlose Testversion am Ende des kostenlosen Testzeitraums in ein kostenpflichtiges Abonnement konvertiert.

In diesem Beispiel haben Sie am 10. Juni eine kostenlose Testversion eines lizenzbasierten Saas-Abonnements (Software-as-a-Service) erworben. Diese kostenlose Testversion wird beim Ende der kostenlosen Testversion automatisch als kostenpflichtiges Abonnement erneuert.

Die Datei für die Wiederaufnahme umfasst die folgenden Gebühren:

| Kaufdatum | Startdatum der Abrechnung | Enddatum der Abrechnung | Unit price | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | 10.06.2019 | 07/09/2019 | 0 USD | 1 | 0 USD | „Neu“, | Kostenlose Testversion |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Erneuern | Kostenpflichtiges Abonnement |

## <a name="cancel-a-free-trial-saas-subscription"></a>Kündigen Sie ein kostenloses Saas-Testabonnement an

> [!TIP]
> Sie können auch während des kostenlosen Testzeitraums jederzeit ein Lizenz basiertes Abonnement für die kostenlose Testversion von Saas kündigen.

In diesem Szenario haben Sie am 1. Juli ein Lizenz basiertes Abonnement für eine kostenlose Testversion von Saas erworben und dann sofort im Partner Center abgebrochen.

Die Datei "Reconnaissance" enthält die folgenden Gebühren:

| Kaufdatum | Startdatum der Abrechnung | Enddatum der Abrechnung | Unit price | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | 10.06.2019 | 07/09/2019 | 0 USD | 11 | 0 USD | „Neu“, | Kostenlose Testversion |
| 10.06.2019 | 10.06.2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Abbrechen | Kostenlose Testversion |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konvertieren eines benutzerdefinierten Abrechnungs-Saas-Abonnements in eine andere SKU

In diesem Szenario wird beschrieben, wie Sie ein benutzerdefiniertes Abrechnungs-Saas-Abonnement von einem Stock Keeping Unit (SKU) in eine andere SKU für das gleiche Produkt am gleichen Datum konvertieren.

In diesem Szenario haben Sie eine SKU (Silver) unter einem Produkt erworben und in eine andere verfügbare SKU (Bronze) unter diesem Produkt zum gleichen Datum konvertiert.

Die Datei "Reconnaissance" enthält die folgenden Gebühren:

| Kaufdatum | SKU | Startdatum der Abrechnung | Enddatum der Abrechnung | Unit price | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | Silber | 10.06.2019 | 10.06.2019 | 20 USD | 1 | 20 USD | „Neu“, | Benutzerdefiniertes Abrechnungs Abonnement für Saas |
| 10.06.2019 | Silber | 10.06.2019 | 10.06.2019 | 20 USD | 1 | -$20 | Convert | Anteilsmäßig angeforderte Rechnung für benutzerdefiniertes Abrechnungs-Saas-Abonnement |
| 10.06.2019 | Bronze | 10.06.2019 | 10.06.2019 | 10 USD | 1 | 10 USD | Convert | Benutzerdefiniertes Abrechnungs Abonnement für Saas |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Erwerben und kündigen eines Kunden Abrechnungs-Saas-Abonnements am gleichen Datum

In diesem Szenario wird die Abrechnung für ein SaaS-Abonnement für Kunden Zähler beschrieben, das Sie über die Azure-Portal zum gleichen Zeitpunkt erworben und abgebrochen haben.

In diesem Szenario haben Sie ein benutzerdefiniertes Abrechnungs Abonnement für SaaS-Abonnements auf der Azure-Portal erworben. Anschließend haben Sie das Abonnement am gleichen Datum abgebrochen.

| Kaufdatum | SKU | Startdatum der Abrechnung | Enddatum der Abrechnung | Unit price | Einheiten Menge | Gesamtbetrag | Gebührenart | Abonnement Beschreibung |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | Bronze | 10.06.2019 | 10.06.2019 | 10 USD | 1 | 10 USD | „Neu“, | Benutzerdefiniertes Abrechnungs Abonnement für Saas |
| 10.06.2019 | Bronze | 10.06.2019 | 10.06.2019 | 10 USD | 1 | -$10 | CancelImmediate | Benutzerdefiniertes Abrechnungs Abonnement für Saas |
