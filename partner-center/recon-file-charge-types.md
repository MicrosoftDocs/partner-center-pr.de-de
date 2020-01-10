---
title: Abgleich-Datei Lade Typen | Partner Center
ms.topic: article
ms.date: 01/06/2020
description: Arten von Gebühren (Lizenz basiert, Nutzungs basiert und einmalig), Gutschriften und Rabatte für Partner Center-Abstimmungs Dateien.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b18a2a7d53e2f9d35baac2412c1710c21d6d98eb
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716871"
---
# <a name="understand-charge-types"></a>Grundlegendes zu Lade Typen

**Gilt für**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Administratoragent
- Abrechnungsadministrator
- Globaler Administrator

In diesem Thema werden die Zuordnungen zwischen einem Rechnungs Abschnitt und den zugehörigen Abrechnungs Typen beschrieben, die möglicherweise in der Abstimmungs Datei liegen. Ihre Rechnung enthält eine Zusammenfassung der Gebühren. Die Abstimmungs Datei bietet eine detaillierte Aufschlüsselung der Zeilen Element Transaktionen, einschließlich der Lade Typen. Weitere Informationen zum Abgleich von Dateien finden [Sie unter Verwenden](use-the-reconciliation-files.md)von Abstimmungs Dateien.

Sowohl [nutzungsbasierte ababstimmungs Dateien](usage-based-recon-files.md) als auch [Lizenz basierte ababstimmungs Dateien](license-based-recon-files.md) zeigen nur nutzungsbezogene Transaktionen und Gebühren an (genutzte Einheiten und zugehörige Gebühren).

> [!NOTE]
> Einmalige Gutschriften, Rabatte oder Rückerstattungen, die auf der Rechnung angezeigt werden **, werden nicht** in der Abstimmungs Datei angezeigt.

## <a name="map-charge-types-to-invoice-charges"></a>Zuordnen von Gebühren Typen zu Rechnungs Gebühren

Verwenden Sie die Filteroptionen in Microsoft Excel, um die Berechnung der Kosten für einen Querverweis zwischen der Rechnung und der Abstimmungs Datei zu überschreiten. Filtern Sie nach den Gebühren Typen in der Abstimmungs Datei, um die Rechnungs Gebühren einem Satz von Gebühren für die Abstimmungs Datei zuzuordnen.

## <a name="license-based-charges"></a>Lizenzbasierte Gebühren

Um diese lizenzbasierten Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.

| Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei) | Erklärung der Abrechnung |
| ------------------------------------------------------------- | ------------------ |
| Aktivierungsgebühr | Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf verwendet. |
| Stornierungsgebühr | Anteilsmäßig an den Kunden abgezahlte Gebühren, wenn die zugeordneten Arbeitsplätze geändert werden. |
| Instanz anteilig stornieren | Anteilsmäßig abgeänderte Gebühren, die abgebrochen wurden, wenn der Kunde mit monatlichem Abonnement das Abonnement angehalten hat und die zugeordneten Arbeitsplätze |
| Gebühr für Zyklus | Regelmäßige Gebühren für ein Abonnement. |
| Anteiliger Zyklus für Instanz | Anteilsmäßig abgeänderte Gebühren vom Kunden, wenn die zugeordneten Arbeitsplätze geändert werden. |
| Gebühren bei Stornierung anteilig zuordnen | Anteilsmäßig abgenommene Rückerstattung für den nicht genutzten Dienst Anteil nach Abbruch. |
| Anteilsmäßig Gebühren beim Konvertieren aus dem aktuellen Angebot | Anteilsmäßig anfallenden Gebühren nach der Umstellung des aktuellen monatlichen Abonnements in ein Jahresabonnement. |
| Angleichen von Gebühren beim Konvertieren in ein neues Angebot | Anteilsmäßig anfallenden Gebühren nach der Umstellung eines monatlichen Abonnements in ein neues Jahresabonnement. |
| Anteilige Gebühren beim Kauf | Der Typ der Gebühr für ein Abonnement bei Verwendung der jährlichen Abrechnung. |
| Kaufgebühr | Der Gebühr für ein Abonnement, wenn die monatliche Abrechnung verwendet wird. |
| Anteilige Gebühr bei Verlängerung | Anteilsmäßig Kosten bei der Erneuerung des Abonnements. |
| Verlängerungsgebühr | Gebühr für Verlängerung eines Abonnements |
| Anteilige Gebühren beim Aktivieren | > anteilsmäßig an der Aktivierung bis zum Ende des Abrechnungszeitraums. |

## <a name="one-time-charges"></a>Einmalige Gebühren

Um diese einmaligen Gebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.

| Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei) | Erklärung der Abrechnung |
| ------------------------------------------------------------- | ------------------ |
| „Neu“, | Wird verwendet, wenn ein neuer Kauf erstellt wird. |
| addQuantity | Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Erhöhung verwendet. |
| removeQuantity | Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Abnahme verwendet. |
| Abbrechen | Wird verwendet, wenn ein Abonnement abgebrochen wird. |
| Konvertieren | Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Arbeitsplätze jedoch unverändert bleibt. |

## <a name="usage-charges"></a>Nutzungsgebühren

Um diese Nutzungsgebühren Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.

| Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei) | Erklärung der Abrechnung |
| ------------------------------------------------------------- | ------------------ |
| Nutzungsgebühr beim Stornieren bewerten | Zugriffsnutzungsgebühr bei Abbruch für eine nicht bezahlte Nutzung im aktuellen Abrechnungszeitraum. |
| Nutzungsgebühr für den aktuellen Zyklus bewerten | Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum. |

### <a name="credits"></a>Gutschriften

So ordnen Sie diese Gutschriften Ihrer Rechnung zu:

- **Addieren Sie totalforcustomer** aus der lizenzbasierten Datei.
- Summieren Sie die **posttaxtotal** -Spalte aus der Verwendungs basierten Datei.

| Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei) | Erklärung der Abrechnung |
| ------------------------------------------------------------- | ------------------ |
| Ausgleichen einer Position | Teilweise oder vollständige Rückerstattung einer Position, einschließlich Steuern. |

### <a name="usage-based-discounts"></a>Nutzungsbasierte Rabatte

Um diese nutzungsbasierten Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **pretaxcharges** aus der Verwendungs basierten Datei.

| Lade Beschreibung (Spalte chargetype in der Abstimmungs Datei) | Erklärung der Abrechnung |
| ------------------------------------------------------------- | ------------------ |
| Aktivierungsrabatt | Der Rabatt wurde beim Aktivieren des Abonnements angewendet. |
| Zyklusrabatt | Der bei wiederkehrenden Gebühren gewährte Rabatt. |
| Verlängerungsrabatt | Der Rabatt wurde bei erneutem Abonnement zugewiesen. |
| Stornorabatt | Gebühren, die beim Abbruch von Rabatten angewendet wurden. |

### <a name="license-based-discounts"></a>Lizenzbasierte Rabatte

Um Lizenz basierte Rabatte Ihrer Rechnung zuzuordnen, addieren Sie die Spalte **totalotherdiscount** aus der lizenzbasierten Datei.

*Lizenz basierte Rabatte können auf mehrere Lade Typen angewendet werden.*
