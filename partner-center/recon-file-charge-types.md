---
title: Gebührenarten für Abstimmungsdateien
ms.topic: article
ms.date: 06/05/2020
description: Entdecken Sie die Arten von Gebühren (z. B. lizenzbasierte, nutzungsbasierte und einmalige Gebühren), Guthaben und Rabatte in Partner Center Abstimmungsdateien.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855878"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Verstehen der verschiedenen Gebührentypen in Partner Center Abstimmungsdateien

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Administrator-Agent| Abrechnungsadministrator| Globaler Administrator

In diesem Artikel werden die Zuordnungen zwischen einem Rechnungsabschnitt und den zugehörigen Gebührentypen beschrieben, die sich möglicherweise in Ihrer Abstimmungsdatei finden. Ihre Rechnung enthält eine Zusammenfassung der Gebühren. Ihre Abstimmungsdatei enthält eine detaillierte Aufschlüsselung der Zeilenelementtransaktionen, einschließlich der Gebührentypen. Weitere Informationen zu Abstimmungsdateien finden Sie unter [Verwenden von Abstimmungsdateien.](use-the-reconciliation-files.md)

Sowohl [nutzungsbasierte Abstimmungsdateien](usage-based-recon-files.md) als auch [lizenzbasierte](license-based-recon-files.md) Abstimmungsdateien zeigen nur nutzungsbezogene Transaktionen und Gebühren (verbrauchte Einheiten und zugehörige Gebühren) an.

> [!NOTE]
> Einmalige Gutschriften, Rabatte oder Rückerstattungen, die  auf der Rechnung als Anpassungen angezeigt werden, werden in der Abstimmungsdatei nicht angezeigt.

## <a name="map-charge-types-to-invoice-charges"></a>Zuordnen von Gebührentypen zu Rechnungsgebühren

Verwenden Sie die Filteroptionen in Microsoft Excel, um auf die Gebührenbeträge zwischen Ihrer Rechnung und der Abstimmungsdatei zu verweisen. Filtern Sie nach Gebührentypen in Ihrer Abstimmungsdatei, um die Rechnungsgebühren einer Reihe von Gebührenaufschlüsselungen in der Abstimmungsdatei zu zuordnen.

## <a name="license-based-charges"></a>Lizenzbasierte Gebühren

Um diese lizenzbasierten Gebühren Ihrer Rechnung zu zuordnen, summiert sich die **Spalte Betrag** aus der lizenzbasierten Datei.

| Charge description (ChargeType column in reconciliation file) (Gebührenbeschreibung (Spalte ChargeType in der Abstimmungsdatei)) | Erläuterung der Gebühr |
| ------------------------------------------------------------- | ------------------ |
| Aktivierungsgebühr | Der Betrag, der dem Kunden in Rechnung gestellt wird, wenn er das Abonnement nach dem Kauf verwendet. |
| Stornierungsgebühr | Anteilierte Gebühren, die an den Kunden zurückerstattet werden, wenn zugehörige Lizenzen geändert werden. |
| Abbrechen der Instanzprorate | Anteilierte Gebühren werden storniert, wenn das Abonnement des Kunden mit einem monatlichen Abonnement ausgesetzt wurde und die zugehörigen Lizenzen innerhalb desselben Monats geändert wurden. |
| Gebühr für Zyklus | Regelmäßige Gebühren für ein Abonnement. |
| Anteiliger Zyklus für Instanz | Anteiligen Gebühren, die vom Kunden berechnet werden, wenn zugeordnete Lizenzen geändert werden. |
| Gebühren bei Stornierung anteilig zuordnen | Anteilige Rückerstattung für nicht verwendeten Teil des Diensts bei Stornierung. |
| Anteilen von Gebühren bei der Umstellung vom aktuellen Angebot | Anteilig berechnete Gebühren nach der Umstellung vom aktuellen monatlichen Abonnement in ein Jahresabonnement. |
| Anteilen von Gebühren bei der Umstellung auf ein neues Angebot | Anteilig berechnete Gebühren nach der Konvertierung eines monatlichen Abonnements in ein neues Jahresabonnement. |
| Anteilige Gebühren beim Kauf | Der Gebührentyp für ein Abonnement, wenn sowohl die monatliche als auch die jährliche Abrechnung verwendet wird. |
| Anteilige Gebühr bei Verlängerung | Anteiligen Gebühren nach Verlängerung des Abonnements. |
| Verlängerungsgebühr | Gebühr für Verlängerung eines Abonnements |
| Anteilige Gebühren beim Aktivieren | Anteiligen Gebühren von der Aktivierung bis zum Ende des Abrechnungszeitraums. |

## <a name="one-time-charges"></a>Einmalige Gebühren

Um diese einmaligen Gebühren Ihrer Rechnung zuzuordnen, summieren Sie die Spalte **Amount** aus der lizenzbasierten Datei.

| Gebührenbeschreibung (Spalte ChargeType in der Abstimmungsdatei) | Erklärung der Gebühren |
| ------------------------------------------------------------- | ------------------ |
| Neu | Wird verwendet, wenn ein neuer Kauf erstellt wird. |
| addQuantity | Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Erhöhung verwendet. |
| removeQuantity | Wird sowohl bei der Rückerstattung des ursprünglichen Kaufs als auch bei der neuen Menge nach einer Abnahme verwendet. |
| Abbrechen | Wird verwendet, wenn ein Abonnement gekündigt wird. |
| Convert | Wird verwendet, wenn eine Lizenz aktualisiert wird, die Anzahl der Lizenzen jedoch unverändert bleibt. |

## <a name="usage-charges"></a>Usage Charges

Um diese Nutzungsgebühren Ihrer Rechnung zuzuordnen, summieren Sie die Spalte **PretaxCharges** aus der nutzungsbasierten Datei.

| Charge description (ChargeType column in reconciliation file) (Gebührenbeschreibung (Spalte ChargeType in der Abstimmungsdatei)) | Erläuterung der Gebühr |
| ------------------------------------------------------------- | ------------------ |
| Nutzungsgebühr beim Stornieren bewerten | Zugriffsnutzungsgebühr bei Abbruch für eine nicht bezahlte Nutzung im aktuellen Abrechnungszeitraum. |
| Nutzungsgebühr für den aktuellen Zyklus bewerten | Zugriffsnutzungsgebühr für den aktuellen Abrechnungszeitraum. |

### <a name="credits"></a>Mitwirkende

So ordnen Sie Diese Gutschriften Ihrer Rechnung zu:

- Summiert **den TotalForCustomer** aus der lizenzbasierten Datei.
- Summiert **die Spalte PostTaxTotal** aus der nutzungsbasierten Datei.

| Charge description (ChargeType column in reconciliation file) (Gebührenbeschreibung (Spalte ChargeType in der Abstimmungsdatei)) | Erläuterung der Gebühr |
| ------------------------------------------------------------- | ------------------ |
| Ausgleichen einer Position | Teilweise oder vollständige Rückerstattung einer Position, einschließlich Steuern. |

### <a name="usage-based-discounts"></a>Nutzungsbasierte Rabatte

Um diese nutzungsbasierten Rabatte Ihrer Rechnung zu zuordnen, summiert die **Spalte PretaxCharges** aus der nutzungsbasierten Datei.

| Charge description (ChargeType column in reconciliation file) (Gebührenbeschreibung (Spalte ChargeType in der Abstimmungsdatei)) | Erläuterung der Gebühr |
| ------------------------------------------------------------- | ------------------ |
| Aktivierungsrabatt | Rabatt, der angewendet wird, wenn das Abonnement aktiviert wird. |
| Zyklusrabatt | Der bei wiederkehrenden Gebühren gewährte Rabatt. |
| Verlängerungsrabatt | Der Rabatt wird angewendet, wenn das Abonnement verlängert wird. |
| Stornorabatt | Die bei Stornierung von Rabatten anfallenden Gebühren. |

### <a name="license-based-discounts"></a>Lizenzbasierte Rabatte

Um Ihrer Rechnung lizenzbasierte Rabatte zu zuordnen, summiert sich die **Spalte TotalOtherDiscount** aus der lizenzbasierten Datei.

*Lizenzbasierte Rabatte können auf mehrere Gebührentypen angewendet werden.*
