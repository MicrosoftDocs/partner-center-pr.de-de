---
title: Verwenden Ihrer Abstimmungsdateien
ms.topic: article
ms.date: 03/26/2021
description: Erfahren Sie mehr über Abstimmungsdateien in Partner Center und wie Sie die detaillierten Zeilenansichten der Gebühren für einen bestimmten Abrechnungszyklus interpretieren.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431570"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Erfahren Sie, wie Sie die Zeilenelemente in Ihren Partner Center Abstimmungsdateien lesen.

**Geeignete Rollen:** Abrechnungsadministrator | Globaler Administrator

Sie können Ihre Abstimmungsdateien aus Partner Center herunterladen, um eine detaillierte Zeilenansicht der einzelnen Gebühren in einem Abrechnungszyklus zu erhalten. Die Details der Einzelnen enthalten Gebühren für die Abonnements der einzelnen Kunden und detaillierte Ereignisse (z. B. das kurzfristige Hinzufügen von Lizenzen zu einem Abonnement).

Informationen zum Lesen Ihrer **Rechnung** finden Sie unter [Lesen Ihrer Rechnung.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Grundlegendes zu Abstimmungsdateifeldern

- [Grundlegendes zu den Feldern in lizenzbasierten Abstimmungsdateien von Partner Center](license-based-recon-files.md)
- [Grundlegendes zu nutzungsbasierten Abstimmungsdateien und ihren spezifischen Feldern im Partner Center](usage-based-recon-files.md)
- [Abstimmungsdateien zur täglich bewerteten Nutzung: Felder](daily-rated-usage-recon-files.md)
- [Felder für die CSP-Abstimmungsdatei für einmaligen Kauf](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Grundlegendes zu Gebührentypen in Abstimmungsdateien

Informationen zu den Gebührentypen in Abstimmungsdateien (Spalte **ChargeType)** finden Sie unter Gebührentypen für [Abstimmungsdateien.](recon-file-charge-types.md)

## <a name="fix-formatting-issues"></a>Beheben von Formatierungsproblemen

Gelegentlich kann eine Abstimmungsdatei Formatierungsprobleme enthalten. Dieses Problem kann beispielsweise auftreten, wenn das Gebietsschema "en-US" nicht verwendet wird.

Führen Sie die folgenden Schritte aus, um Formatierungsprobleme in Ihren Abstimmungsdateien zu beheben:

1. Öffnen Sie die Abstimmungsdatei (im .csv Format) in Microsoft Excel.
2. Wählen Sie die erste Spalte in der Datei aus.
3. Öffnen Sie den **Assistenten zum Konvertieren von Text in Spalten.** Wählen Sie auf dem Menüband **Daten** und dann **Text in Spalten aus.**
4. Wählen Sie im Assistenten **Dateityp mit Trennzeichen aus.** Klicken Sie anschließend auf **Weiter**.
5. Wählen Sie im Feld **Trennzeichen** die Option **Komma** aus. (Wenn **die Registerkarte** bereits ausgewählt ist, können Sie diese Option aktiviert lassen.) Wählen Sie dann **Weiter** aus.
6. Wählen Sie im Feld **Spaltendatenformat** die Option **Date:MDY** aus. Klicken Sie anschließend auf **Weiter**.
7. Wählen Sie im Feld **Spaltendatenformat** die Option **Text** für alle Spalten vom Datentyp "Amount" aus. Wählen Sie **Fertig stellen** aus.

## <a name="download-reconciliation-files-programmatically"></a>Programmgesteuertes Herunterladen von Abstimmungsdateien

Abstimmungsdateien können sehr groß sein und sind manchmal schwierig herunterzuladen. Informationen zum programmgesteuerten Herunterladen von Abstimmungsdateien finden Sie unter [Abrufen von Rechnungspositionen.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Wenn Ihre Datei das Zeilenlimit in Excel überschreitet

Wenn Sie eine Abstimmungsdatei herunterladen, aber nicht in Microsoft Excel öffnen können, bedeutet dies wahrscheinlich, dass die Datei mehr Zeilen enthält, als Excel zulässt. In diesem Fall können Sie eine der folgenden Verfahren verwenden, um die Datei zu öffnen.

### <a name="open-a-recon-file-in-power-bi"></a>Öffnen einer Recon-Datei in Power BI

1. Laden Sie die Abstimmungsdatei wie gewohnt herunter.
2. Laden Sie eine Instanz von Microsoft Power BI herunter, installieren und öffnen Sie sie.
3. Wählen Sie auf der **Registerkarte** Start Power BI Daten **abrufen** aus.
4. Wählen Sie in der Liste **allgemeine Datenquellen** die Option **Text/CSV** aus.
5. Öffnen Sie ihre Recon-Datei, wenn Sie dazu aufgefordert werden.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Öffnen einer Recon-Datei in einer Excel-Pivot-Tabelle

1. Laden Sie die Abstimmungsdatei wie gewohnt herunter.
2. Öffnen Sie eine neue Datei in Microsoft Excel.
3. Wählen Sie auf der Registerkarte **Daten** die Option **Daten abrufen** **aus,** wählen Sie Aus Datei und dann **Text/CSV** aus.
4. Öffnen Sie ihre Recon-Datei, wenn Sie dazu aufgefordert werden. Ihre Daten werden angezeigt.
5. Wählen **Sie** im Dropdownmenü Laden die Option **Laden in** und dann **OK** aus.
6. Wählen **Sie** im Dialogfeld Daten importieren die Option **PivotTable-Bericht** aus, um die Datei zu öffnen.

## <a name="negative-amount-displayed"></a>Negativer Betrag angezeigt

Möglicherweise wird in Ihrer Abstimmungsdatei ein negativer Betrag angezeigt. Dieses Problem hat häufig eine der folgenden Ursachen:

- Sie haben ihre Anzahl von Lizenzen vor Kurzem gekündigt oder reduziert.
- Sie haben entweder eine Gutschrift für einen Dienstlizenzvertrag (Service License Agreement, SLA) oder für die Azure-Nutzung erhalten.

Um weitere Informationen über diese Transaktion zu erhalten, überprüfen Sie das Attribut „Gebührentyp“ in Ihrer Abstimmungsdatei.

## <a name="map-taxes-or-vat"></a>Zuordnen von Steuern oder Steuern

So ordnen Sie Steuern oder Mehrwertsteuer (USt) Ihrer Rechnung zu:

- Addiert die Spalte **Steuern** aus der lizenzbasierten Datei.
- Addiert die **Spalte TaxAmount** aus der nutzungsbasierten Datei.

## <a name="itemize-reconciliation-files-by-partner"></a>Auf itemisieren von Abstimmungsdateien nach Partner

Partner im **indirekten Modell** können diese zusätzlichen Felder sowohl in lizenzbasierten als auch in nutzungsbasierten Abstimmungsdateien verwenden, um die Dateien nach Handelspartner aufzuschlüsseln.

| MPN-ID | Beschreibung |
| ------ | ----------- |
| MPN-ID | Der MPN-Bezeichner (Microsoft Partner Network) des CSP-Partners (Cloud Solution Provider) (direkt oder indirekt). |
| [MPN-ID der Handelspartner](#reseller-mpn-id) | Der [MPN-Bezeichner des Datensatzhändlers für das Abonnement](#reseller-mpn-id). Dieses Feld entspricht der Reseller-ID, die für das jeweilige Abonnement in Partner Center aufgeführt ist. Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt. |

### <a name="reseller-mpn-id"></a>MPN-ID der Handelspartner

Wenn ein CSP-Partner das Abonnement direkt an den Kunden verkauft hat, wird seine **MPN-ID** zweimal aufgeführt, sowohl als **MPN-ID** als auch als **Reseller MPN ID**.

Wenn ein CSP-Partner über einen Handelspartner ohne **MPN-ID** verfügt, wird dieser Wert stattdessen auf die **MPN-ID** des Partners festgelegt.

Wenn der CSP-Partner eine **Reseller-MPN-ID** entfernt, wird dieser Wert auf *-1* festgelegt.

So zeigen Sie die **MPN-ID** des Handelspartners an oder aktualisieren sie:

1. Melden Sie sich bei Partner Center an.
2. Wählen Sie im Menü „Partner Center” **Kunden**.
3. Wählen Sie den Kunden in der Liste aus.
4. Wählen Sie im Menü "Kunde" die Option **Abonnements aus.**
5. Wählen Sie das Abonnement aus der Liste aus.
6. Wählen Sie **Aktualisieren** aus, um **Vertriebspartner (MPN-ID)** zu ändern.

## <a name="next-steps"></a>Nächste Schritte

- [Lesen Ihrer Rechnung & Abstimmungsdatei](read-your-bill.md) 