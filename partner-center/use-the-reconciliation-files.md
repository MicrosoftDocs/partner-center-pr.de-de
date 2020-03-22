---
title: Verwenden der Abstimmungs Dateien | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Verwenden Sie Ihre Abstimmungs Dateien, um ausführliche Informationen zu den einzelnen Aufgaben des Partner Centers zu verstehen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 36b8242cc8c47ed36d16f86338a075080c2441e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/21/2020
ms.locfileid: "80114962"
---
# <a name="use-your-reconciliation-files"></a>Verwenden der Abstimmungs Dateien

Betrifft:

- Partner Center
- Partner Center für Microsoft Cloud for US Government

Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen. Zu den Zeilen Element Details zählen die Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Arbeitsplätzen zu einem Abonnement).

Geeignete Rollen:

- Abrechnungsadministrator
- Globaler Administrator

Informationen zum Lesen der **Rechnung**finden Sie unter [Lesen der](read-your-bill.md)Rechnung.

## <a name="understand-reconciliation-file-fields"></a>Grundlegendes zu Abstimmungs Datei Feldern

- [Lizenz basierte Abstimmungs Datei Felder](license-based-recon-files.md)
- [Verwendungs basierte Abstimmungs Datei Felder](usage-based-recon-files.md)
- [Einmalige und wiederkehrende Abstimmungs Datei Felder](one-time-recurring-recon-files.md)
- [Nutzungs Abgleich-Datei Felder für die tägliche Bewertung](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Grundlegendes zu Lade Typen in Abgleich Dateien

Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Beheben von Formatierungsproblemen

Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten. Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.

Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:

1. Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.
2. Wählen Sie die erste Spalte in der Datei aus.
3. Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**. Wählen Sie im Menüband **Daten**aus, und wählen Sie dann **Text in Spalten**aus.
4. Wählen Sie im Assistenten einen **Begrenzungs Dateityp**aus. Klicken Sie dann auf **weiter**.
5. Wählen Sie im Feld **Trenn** Zeichen die Option **Komma**aus. (Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.
6. Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy**aus. Klicken Sie dann auf **weiter**.
7. Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus. Wählen Sie dann **Fertig**stellen aus.

## <a name="download-reconciliation-files-programmatically"></a>Programm gesteuertes herunterladen von Abstimmungs Dateien

Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen. Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Map-Steuern oder Mehrwertsteuer

So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:

- Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.
- Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.

## <a name="itemize-reconciliation-files-by-partner"></a>Abstimmungs Dateien nach Partner itemisieren

Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.

| MPN-ID | Beschreibung |
| ------ | ----------- |
| MPN-ID | Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt). |
| [MPN-ID des Wiederverkäufers](#reseller-mpn-id) | Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id). Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist. Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt. |

### <a name="reseller-mpn-id"></a>MPN-ID der Handelspartner

Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.

Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID**verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.

Wenn der CSP-Partner eine **Reseller MPN-ID**entfernt, wird dieser Wert auf *-1*festgelegt.

So können Sie die **Reseller MPN-ID**anzeigen oder aktualisieren:

1. Melden Sie sich bei Partner Center an.
2. Wählen Sie im Menü „Partner Center” **Kunden**.
3. Wählen Sie den Kunden aus der Liste aus.
4. Wählen Sie im Menü Kunde die Option **Abonnements**aus.
5. Wählen Sie das Abonnement aus der Liste aus.
6. Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.
