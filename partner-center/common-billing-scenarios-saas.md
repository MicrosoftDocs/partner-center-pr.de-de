---
title: 'Abrechnung: lizenzbasierte SaaS-Transaktionen'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie mehr über gängige Abrechnungsszenarien in Partner Center für lizenzbasierte SaaS-Transaktionen (Software-as-a-Service).
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148634"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Gängige Abrechnungsszenarien für lizenzbasierte SaaS-Transaktionen in Partner Center

**Geeignete Rollen:** Administrator-Agent-| Abrechnungsadministrator-| | des Helpdesk-Agents Vertriebsmitarbeiter


Diese [gängigen Beispielabrechnungsszenarien](common-billing-scenarios.md) gelten für lizenzbasierte SaaS-Abonnements (Software-as-a-Service) in Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Konvertieren eines kostenlosen SaaS-Testabonnements in ein kostenpflichtiges Abonnement

In diesem Szenario wird die Abrechnung für die Verlängerung eines lizenzbasierten kostenlosen SaaS-Testabonnements beschrieben. Die Verlängerung konvertiert die kostenlose Testversion in ein kostenpflichtiges Abonnement am Ende des kostenlosen Testzeitraums.

In diesem Beispiel haben Sie am 10. Juni eine kostenlose Testversion eines lizenzbasierten SaaS-Abonnements (Software-as-a-Service) erworben. Diese kostenlose Testversion wird automatisch als kostenpflichtiges Abonnement verlängert, wenn der kostenlose Testzeitraum endet.

Die Recon-Dateien enthalten die folgenden Gebühren:

| Kaufdatum | Startdatum der Gebühr | Enddatum der Gebühr | Unit price | Einheitenmenge | Gesamtbetrag | Gebührenart | Abonnementbeschreibung |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | 10.06.2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Neu | Kostenlose Testversion |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Erneuern | Kostenpflichtiges Abonnement |

## <a name="cancel-a-free-trial-saas-subscription"></a>Kündigen eines kostenlosen SaaS-Testabonnements

> [!TIP]
> Sie können ein lizenzbasiertes Kostenloses SaaS-Testabonnement jederzeit kündigen, auch während des kostenlosen Testzeitraums.

In diesem Szenario haben Sie am 1. Juli ein lizenzbasiertes kostenloses SaaS-Testabonnement erworben und es dann sofort im Partner Center.

Die Abstimmungsdatei enthält die folgenden Gebühren:

| Kaufdatum | Startdatum der Gebühr | Enddatum der Gebühr | Unit price | Einheitenmenge | Gesamtbetrag | Gebührenart | Abonnementbeschreibung |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | 10.06.2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Neu | Kostenlose Testversion |
| 10.06.2019 | 10.06.2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Abbrechen | Kostenlose Testversion |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Konvertieren eines benutzerdefinierten SaaS-Verbrauchszählerabonnements in eine andere SKU

In diesem Szenario wird beschrieben, wie Sie ein benutzerdefiniertes SaaS-Verbrauchseinheitabonnement an demselben Datum von einer Stock Keeping Unit (SKU) in eine andere SKU für dasselbe Produkt konvertieren.

In diesem Szenario haben Sie eine SKU (Silber) unter einem Produkt erworben und am gleichen Datum in eine andere verfügbare SKU (Bronze) unter diesem Produkt konvertiert.

Die Abstimmungsdatei enthält die folgenden Gebühren:

| Kaufdatum | SKU | Startdatum der Gebühr | Enddatum der Gebühr | Unit price | Einheitenmenge | Gesamtbetrag | Gebührenart | Abonnementbeschreibung |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | Silber | 10.06.2019 | 10.06.2019 | 20 USD | 1 | 20 USD | Neu | Benutzerdefiniertes SaaS-Verbrauchszählerabonnement |
| 10.06.2019 | Silber | 10.06.2019 | 10.06.2019 | 20 USD | 1 | -$20 | Convert | Anteilsierte Neuver rechnung für ein benutzerdefiniertes SaaS-Verbrauchszählerabonnement |
| 10.06.2019 | Bronze | 10.06.2019 | 10.06.2019 | 10 USD | 1 | 10 USD | Convert | Benutzerdefiniertes SaaS-Verbrauchszählerabonnement |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Erwerben und Kündigen eines SaaS-Abonnements für kundenspezifische Verbrauchszähler am selben Datum

In diesem Szenario wird die Abrechnung für ein SaaS-Abonnement der Kundenmessung beschrieben, das Sie am selben Azure-Portal erworben und storniert haben.

In diesem Szenario haben Sie ein benutzerdefiniertes SaaS-Verbrauchszählerabonnement für die Azure-Portal. Anschließend haben Sie das Abonnement am selben Datum storniert.

| Kaufdatum | SKU | Startdatum der Gebühr | Enddatum der Gebühr | Unit price | Einheitenmenge | Gesamtbetrag | Gebührenart | Abonnementbeschreibung |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10.06.2019 | Bronze | 10.06.2019 | 10.06.2019 | 10 USD | 1 | 10 USD | Neu | Benutzerdefiniertes SaaS-Verbrauchszählerabonnement |
| 10.06.2019 | Bronze | 10.06.2019 | 10.06.2019 | 10 USD | 1 | -$10 | CancelImmediate | Benutzerdefiniertes SaaS-Verbrauchszählerabonnement |
