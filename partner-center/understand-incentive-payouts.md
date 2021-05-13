---
title: Anzeigen Ihrer Incentive- und Programmdetails
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Verwenden Sie diese Seiten, um Incentives-Programm Status anzuzeigen und zu verwalten.
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 798fde02b87e8f8105dad6d00c32b050fb90097e
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818744"
---
# <a name="view-your-incentives-program-details"></a>Anzeigen der Details ihres Incentives-Programms

**Geeignete Rollen:** Incentivesadministrator | Incentivesbenutzer | Globale | MPN-Partneradministrator

In diesem Artikel wird die **Übersichtsseite Meine Incentives** erläutert, auf der der Gesamtstatus Ihrer Incentiveprogramme sowie der Status der einzelnen Programme an jedem Standort angezeigt werden. Außerdem werden die verschiedenen Registrierungsstatus angezeigt.

>[!NOTE]
>Weitere Informationen zu Incentives und Incentivefeatures in Partner Center finden Sie unter [Partnerinvestitionen und Incentives](https://partner.microsoft.com/membership/partner-incentives) (Anmeldung erforderlich).

## <a name="access-the-incentives-overview-page"></a>Zugreifen auf die Übersichtsseite für Incentives

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.
1. Wählen Sie **Incentives** und dann im Menü **Übersicht** aus.
1. Zeigen Sie im oberen Bereich der Seite die Zusammenfassung der Einnahmen und Zahlungen an. Weitere Details finden Sie in der Tabelle unten. Sie können auch die zugehörige Tabelle sortieren, gruppieren und erweitern:

   - Um nach Spalte zu sortieren, wählen Sie den Spaltennamen aus.
   - Um nach Programm zu gruppieren, wählen Sie die Registerkarte **Nach Programm** oberhalb der Tabelle aus.
   - Um nach Standort zu gruppieren, wählen Sie die Registerkarte **Nach Standort** oberhalb der Tabelle aus.
   - Um weitere Details zu Registrierungen innerhalb einer bestimmten Gruppe anzuzeigen, wählen Sie das Chevronsymbol am Ende einer bestimmten Zeile aus. Dieses Chevron erweitert Ihre Ansicht.
1. Wenn weitere Aktionen erforderlich sind, um sich für ein Programm zu registrieren, werden diese Informationen in der Spalte **Status** angezeigt. Wählen Sie in diesem Fall das Chevron-Symbol aus, um mehr über die nächsten Schritte zu erfahren, die Sie durchführen müssen.

## <a name="enrollment-status"></a>Anmeldungsstatus

In der folgenden Tabelle werden die verschiedenen Registrierungszustände erläutert, die in der Spalte **Status** angezeigt werden.

| **Status**         | **Bedingung für Anzeige** |
|:------------------------------------|:------------------|
| Erforderliche Aktion  | Der Partner hat eine Einladung zur Registrierung für ein Incentive-Programm angenommen, muss aber möglicherweise Bank- oder Steuerinformationen aktualisieren. Weitere Schritte oder Links zum Aktualisieren Ihrer Bank- oder Steuerinformationen in Partner Center finden Sie in der Spalte **Erforderliche** Aktionen. |
| Nicht mehr unterstützt  | Das spezifische Incentive-Programm wird im Incentives-System nicht mehr angeboten. |
| Enrolled (Registriert)  | Alle Steuer- und Bankinformationen wurden überprüft. Vom Partner ist keine weitere Registrierungsaktion erforderlich. |
| Wird registriert  | Der Benutzer ist kein Incentiveadministrator, und die Registrierung befindet sich in den Registrierungszuständen Aktion **erforderlich** **oder Überprüfen.**|
| Inaktiv/Nicht akzeptabel | Das Incentiveprogramm ist derzeit möglicherweise nicht für die Registrierung geöffnet, oder der Partner erfüllt die aktuelle Berechtigung für die Registrierung oder erneute Registrierung nicht. <br><br> Wenn der Status **Nicht wählbar** ist, erfüllt der Partner die aktuellen Berechtigungsanforderungen für das Programm nicht. Wenn Sie **unter** dem Registrierungsstatus den Link Berechtigungsanforderungen anzeigen auswählen, werden die Anforderungen für die Berechtigung und die erfüllten Anforderungen angezeigt. <br><br> Möglicherweise wird auch der **Status Inaktiv** für Registrierungen virtueller Organisationen (VORG) oder globaler Partnerkonto (Partner Global Account, PGA) angezeigt, die nicht mehr im Incentiveprogramm aktiv sind.  |
| Eingeladen  | Eine neue Einladung zur Registrierung des Incentiveprogramms wurde an den Partner gesendet, aber der Partner hat den Registrierungsprozess noch nicht gestartet. In der angrenzenden **Spalte Actions required** (Aktionen erforderlich) werden die nächsten Schritte und alle zugehörigen Links angezeigt.  |
| Überprüfen der Registrierung  | Der Partner hat bereits Bank- und Steuerinformationen für eine neue oder vorhandene Registrierung abgeschlossen oder aktualisiert und wartet darauf, dass Microsoft diese Informationen überprüft. Während des Überprüfungsprozesses kann **die Überprüfung der Registrierung** bis zu 48 Stunden lang angezeigt werden.  |

## <a name="see-your-payment-information"></a>Anzeigen Ihrer Zahlungsinformationen

Wählen Sie das Auszahlungssymbol in der oberen rechten Ecke des Bildschirms aus, um auf diese verschiedenen Zusammenfassungen zu zugreifen:

- Transaktionsverlauf
- Zahlungen
- Exportieren von Daten

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Veranschaulicht das Auszahlungssymbol in der oberen rechten Ecke des Partner Center Portal":::

Diese Informationen umfassen den Gesamtgewinn und die Gesamtzahlungen, seit Sie sich bei Incentive-Programmen angemeldet haben. Diese Seite enthält auch Einnahmen und Zahlungen nach Standort oder Programm sowie alle weiteren Aktionen, die Sie möglicherweise durchführen müssen, um sich an einem bestimmten Ort bei einem Programm anzumelden. 

Sie können auch die [Partnerauszahlungs-API verwenden,](https://apidocs.microsoft.com/services/partnerpayouts) um direkt eine Verbindung herzustellen und Auszahlungstransaktions- und Zahlungsdaten zu erhalten. Weitere [Informationen finden Sie unter Auszahlungsauszahlungen.](payout-statement.md)

## <a name="next-steps"></a>Nächste Schritte

- [Auszahlungsauszüge](payout-statement.md)
