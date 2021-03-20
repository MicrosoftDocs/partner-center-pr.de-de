---
title: Anzeigen von Informationen zu Incentives und Programmen
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Verwenden Sie diese Seiten zum Anzeigen und Verwalten des Status der Incentive-Programme.
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: a66e32a3c9320ac32b0749c67197c6a27574ce75
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712612"
---
# <a name="view-your-incentives-program-details"></a>Details zu den Programm Details anzeigen

**Geeignete Rollen**

- Incentiveadministrator
- Incentivebenutzer
- Globaler Administrator
- MPN-Partneradministrator

In diesem Artikel wird die Übersichtsseite " **meine Incentives** " erläutert, die den Gesamtstatus Ihrer Incentive-Programme sowie den Status der einzelnen Programme an jedem Standort anzeigt. Außerdem gibt es die verschiedenen Registrierungsstatus.

>[!NOTE]
>Weitere Informationen zu Incentives und Incentive-Features in Partner Center finden Sie unter [Partner Investitionen und-Anreize](https://partner.microsoft.com/membership/partner-incentives) (Anmeldung erforderlich).

## <a name="access-the-incentives-overview-page"></a>Seite "Übersicht über die Incentives"

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.
1. Wählen Sie im Menü den Befehl **Incentives** und dann **Overview** aus.
1. Zeigen Sie im oberen Bereich der Seite die Zusammenfassung der Einnahmen und Zahlungen an. Weitere Details finden Sie in der Tabelle unten. Sie können die zugehörige Tabelle auch sortieren, gruppieren und erweitern:

   - Wenn Sie nach Spalte sortieren möchten, wählen Sie den Spaltennamen aus.
   - Um nach einem Programm zu gruppieren, wählen Sie die Registerkarte **nach Programm** über der Tabelle aus.
   - Um nach Standort zu gruppieren, wählen Sie die Registerkarte **nach Speicherort** über der Tabelle aus.
   - Wenn Sie weitere Details zu Registrierungen innerhalb einer bestimmten Gruppe anzeigen möchten, wählen Sie das Chevron-Symbol am Ende einer bestimmten Zeile aus. Dieses Chevron erweitert Ihre Ansicht.
1. Wenn weitere Aktionen erforderlich sind, um sich für ein Programm zu registrieren, werden diese Informationen in der Spalte **Status** angezeigt. Wählen Sie in diesem Fall das Chevron-Symbol aus, um mehr über die nächsten Schritte zu erfahren, die Sie durchführen müssen.

## <a name="enrollment-status"></a>Anmeldungsstatus

In der folgenden Tabelle werden die verschiedenen Registrierungs Zustände erläutert, die in der Spalte **Status** angezeigt werden.

| **Status**         | **Bedingung für Anzeige** |
|:------------------------------------|:------------------|
| Erforderliche Aktion  | Der Partner hat eine Einladung zum Anmelden bei einem Incentive-Programm akzeptiert, muss jedoch die Bank-oder Steuerinformationen aktualisieren. In der Spalte **erforderliche Aktionen** finden Sie alle nächsten Schritte oder Links zum Aktualisieren Ihrer Bank-oder Steuerinformationen in Partner Center. |
| Nicht mehr unterstützt  | Das spezielle Incentive-Programm wird nicht mehr im System "Incentives" angeboten. |
| Registriert  | Alle Steuer-und Bankinformationen wurden überprüft. Es ist keine weitere Registrierungsaktion für den Partner erforderlich. |
| Wird registriert  | Der Benutzer ist kein Incentive-Administrator, und die Registrierung erfolgt in der **erforderlichen Aktion** oder **bei** der Überprüfung der Registrierungs Zustände.|
| Inaktiv/nicht berechtigt | Das Incentive-Programm ist zu diesem Zeitpunkt möglicherweise nicht für die Registrierung geöffnet, oder der Partner erfüllt nicht die aktuelle Berechtigung zur Registrierung oder erneuten Registrierung. <br><br> Wenn der Status nicht **qualifiziert** ist, erfüllt der Partner nicht die aktuellen Berechtigungsanforderungen für das Programm. Wenn Sie unter dem Registrierungsstatus den Link Informationen zu den **Berechtigungsanforderungen** anzeigen auswählen, werden die Voraussetzungen für die Berechtigung angezeigt, und welche dieser Anforderungen erfüllt sind. <br><br> Möglicherweise wird auch ein **inaktiver** Status für Registrierungen virtueller Organisationen (Vorg) oder Partner globaler Konten (Partner Global Account, PGA) angezeigt, die im Incentive-Programm nicht mehr aktiv sind.  |
| Eingeladen  | Es wurde eine neue Einladungsprogramm-Registrierungs Einladung an den Partner gesendet, aber der Partner hat den Registrierungsprozess noch nicht gestartet. In der angrenzenden Spalte **Aktionen erforderlich** werden die nächsten Schritte und alle zugehörigen Links angezeigt.  |
| Die Registrierung wird überprüft.  | Der Partner hat die Bank-und Steuerinformationen für eine neue oder vorhandene Registrierung bereits abgeschlossen oder aktualisiert und wartet darauf, dass Microsoft diese Informationen überprüft. Während der über **Prüfung wird die** Überprüfung der Registrierung möglicherweise für bis zu 48 Stunden angezeigt.  |

## <a name="see-your-payment-information"></a>Anzeigen der Zahlungsinformationen

Wählen Sie das Auszahlungs Symbol in der oberen rechten Ecke des Bildschirms aus, um auf diese unterschiedlichen Zusammenfassungen zuzugreifen:

- Transaktionsverlauf
- Zahlungen
- Exportieren von Daten

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Veranschaulicht das Auszahlungs Symbol in der oberen rechten Ecke des Partner Center-Portals.":::

Diese Informationen umfassen den Gesamtgewinn und die Gesamtzahlungen, seit Sie sich bei Incentive-Programmen angemeldet haben. Diese Seite enthält auch Einnahmen und Zahlungen nach Standort oder Programm sowie alle weiteren Aktionen, die Sie möglicherweise durchführen müssen, um sich an einem bestimmten Ort bei einem Programm anzumelden. 

Sie können auch die [Partner-Auszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts) verwenden, um eine Verbindung zu Auszahlungs Transaktionen und Zahlungsdaten direkt herzustellen und diese zu erhalten. Weitere Informationen finden Sie unter [Auszahlungs Anweisungen](payout-statement.md) .

## <a name="next-steps"></a>Nächste Schritte

- [Auszahlungsauszüge](payout-statement.md)
