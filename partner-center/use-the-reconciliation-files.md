---
title: Verwenden der Abstimmungs Dateien
ms.topic: article
ms.date: 06/08/2020
description: Erfahren Sie mehr über das Abgleichen von Dateien in Partner Center und über die Interpretation der detaillierten Zeilen Element Sichten für einen bestimmten Abrechnungszeitraum.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d09c1e57d16937c5656579f3932e9c8feb3ecf24
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94488079"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Erfahren Sie, wie Sie die Zeilen Elemente in Ihren Partner Center-Abstimmungs Dateien lesen.

Gilt für:

- Partner Center
- Partner Center für Microsoft Cloud for US Government

Sie können Ihre Abstimmungs Dateien aus Partner Center herunterladen, um eine ausführliche Ansicht der einzelnen Kosten in einem Abrechnungszeitraum anzuzeigen. Zu den Zeilen Element Details zählen Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. b. das Hinzufügen von Lizenzen zu einem Abonnement).

Geeignete Rollen:

- Abrechnungsadministrator
- Globaler Administrator

Informationen zum Lesen der **Rechnung** finden Sie unter [Lesen der](read-your-bill.md)Rechnung.

## <a name="understand-reconciliation-file-fields"></a>Grundlegendes zu Abstimmungs Datei Feldern

- [Lizenz basierte Abstimmungs Datei Felder](license-based-recon-files.md)
- [Verwendungs basierte Abstimmungs Datei Felder](usage-based-recon-files.md)
- [Nutzungs Abgleich-Datei Felder für die tägliche Bewertung](daily-rated-usage-recon-files.md)
- [Felder für das einmalige kaufen von CSP-Abstimmungs Dateien](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Grundlegendes zu Lade Typen in Abgleich Dateien

Informationen zu den Gebühren Typen in Abgleich Dateien (Spalte **chargetype** ) finden Sie unter Abgleichen von [Datei Gebühren Typen](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Beheben von Formatierungsproblemen

Gelegentlich kann eine Abstimmungs Datei Formatierungs Probleme enthalten. Dieses Problem kann z. b. auftreten, wenn das Gebiets Schema "en-US" nicht verwendet wird.

Führen Sie die folgenden Schritte aus, um alle Formatierungs Probleme in den Abstimmungs Dateien zu beheben:

1. Öffnen Sie die Abstimmungs Datei (im CSV-Format) in Microsoft Excel.
2. Wählen Sie die erste Spalte in der Datei aus.
3. Öffnen **Sie den Assistenten zum Konvertieren von Text in Spalten**. Wählen Sie im Menüband **Daten** aus, und wählen Sie dann **Text in Spalten** aus.
4. Wählen Sie im Assistenten einen **Begrenzungs Dateityp** aus. Klicken Sie anschließend auf **Weiter**.
5. Wählen Sie im Feld **Trenn** Zeichen die Option **Komma** aus. (Wenn die **Tab** -Taste bereits ausgewählt ist, können Sie diese Option aktivieren.) Klicken Sie dann auf **weiter**.
6. Wählen Sie im Feld **Spaltendaten Format** die Option **Date: mdy** aus. Klicken Sie anschließend auf **Weiter**.
7. Wählen Sie im Feld **Spaltendaten Format** die Option **Text** für alle Spalten vom Typ Summe aus. Wählen Sie **Fertig stellen** aus.

## <a name="download-reconciliation-files-programmatically"></a>Programm gesteuertes herunterladen von Abstimmungs Dateien

Abstimmungs Dateien können sehr groß sein und werden manchmal nur schwer heruntergeladen. Informationen zum programmgesteuerten herunterladen von Abstimmungs Dateien finden Sie unter [Get Rechnungs Items](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Map-Steuern oder Mehrwertsteuer

So ordnen Sie der Rechnung Steuern oder Mehrwertsteuer (Tax) hinzu:

- Addieren Sie die Spalte " **Tax** " aus der lizenzbasierten Datei.
- Addieren Sie die Spalte " **taxAmount** " aus der Verwendungs basierten Datei.

## <a name="itemize-reconciliation-files-by-partner"></a>Abstimmungs Dateien nach Partner itemisieren

Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch auf Verwendungs basierten Abstimmungs Dateien verwenden, um die Dateien vom Wiederverkäufer zu itemisieren.

| MPN-ID | BESCHREIBUNG |
| ------ | ----------- |
| MPN-ID | Der Microsoft Partner Network (MPN)-Bezeichner des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt). |
| [MPN-ID der Handelspartner](#reseller-mpn-id) | Der [MPN-Bezeichner des Reseller of-Datensatzes für das Abonnement](#reseller-mpn-id). Dieses Feld entspricht der Wiederverkäufer-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist. Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt. |

### <a name="reseller-mpn-id"></a>MPN-ID der Handelspartner

Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird die **MPN-ID** zweimal aufgelistet, sowohl als **MPN-ID** als auch als **Reseller MPN-ID**.

Wenn ein CSP-Partner über einen Reseller ohne **MPN-ID** verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.

Wenn der CSP-Partner eine **Reseller MPN-ID** entfernt, wird dieser Wert auf *-1* festgelegt.

So können Sie die **Reseller MPN-ID** anzeigen oder aktualisieren:

1. Melden Sie sich bei Partner Center an.
2. Wählen Sie im Menü „Partner Center” **Kunden**.
3. Wählen Sie den Kunden in der Liste aus.
4. Wählen Sie im Menü Kunde die Option **Abonnements** aus.
5. Wählen Sie das Abonnement aus der Liste aus.
6. Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.