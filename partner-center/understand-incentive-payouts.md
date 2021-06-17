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
ms.openlocfilehash: 33ec3befdc4b2bab2f31d25d210679594debbbf1
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277248"
---
# <a name="view-your-incentives-program-details"></a>Anzeigen der Details ihres Incentives-Programms

**Geeignete Rollen:** Incentivesadministrator | Incentivesbenutzer | Globale | MPN-Partneradministrator

In diesem Artikel wird die **Übersichtsseite Meine Incentives** erläutert, auf der der Gesamtstatus Ihrer Incentiveprogramme sowie der Status der einzelnen Programme an jedem Standort angezeigt werden. Außerdem werden die verschiedenen Registrierungsstatus angezeigt.

>[!NOTE]
>Weitere Informationen zu Incentives und Incentivefunktionen in Partner Center finden Sie unter [Partnerinvestitionen und Incentives](https://partner.microsoft.com/membership/partner-incentives) (Anmeldung erforderlich).

## <a name="access-the-incentives-overview-page"></a>Zugreifen auf die Übersichtsseite für Incentives

1. Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard) an.
1. Wählen Sie **Incentives** und dann im Menü **Übersicht** aus.
1. Zeigen Sie im oberen Bereich der Seite die Zusammenfassung der Einnahmen und Zahlungen an. Weitere Details finden Sie in der Tabelle unten. Sie können auch die zugehörige Tabelle sortieren, gruppieren und erweitern:

   - Um nach Spalte zu sortieren, wählen Sie den Spaltennamen aus.
   - Um nach Programm zu gruppieren, wählen Sie die Registerkarte **Nach Programm** oberhalb der Tabelle aus.
   - Um nach Standort zu gruppieren, wählen Sie die Registerkarte **Nach Standort** oberhalb der Tabelle aus.
   - Um weitere Details zu Registrierungen innerhalb einer bestimmten Gruppe anzuzeigen, wählen Sie das Chevronsymbol am Ende einer bestimmten Zeile aus. Mit diesem Chevron wird Ihre Ansicht erweitert.
1. Wenn weitere Aktionen erforderlich sind, um sich für ein Programm zu registrieren, werden diese Informationen in der Spalte **Status** angezeigt. Wählen Sie in diesem Fall das Chevron-Symbol aus, um mehr über die nächsten Schritte zu erfahren, die Sie durchführen müssen.

## <a name="enrollment-status"></a>Anmeldungsstatus

In der folgenden Tabelle werden die verschiedenen Registrierungszustände erläutert, die in der Spalte **Status** angezeigt werden.

| **Status**         | **Bedingung für Anzeige** |
|:------------------------------------|:------------------|
| Erforderliche Aktion  | Der Partner hat eine Einladung zur Registrierung für ein Incentive-Programm angenommen, muss aber möglicherweise Bank- oder Steuerinformationen aktualisieren. Weitere Schritte oder Links zum Aktualisieren Ihrer Bank- oder Steuerinformationen in Partner Center finden Sie in der Spalte **Erforderliche** Aktionen. |
| Nicht mehr unterstützt  | Das spezifische Incentive-Programm wird im Incentives-System nicht mehr angeboten. |
| Registriert  | Alle Steuer- und Bankinformationen wurden überprüft. Für den Partner ist keine weitere Registrierungsaktion erforderlich. |
| Wird registriert  | Der Benutzer ist kein Incentiveadministrator, und die Registrierung befindet sich im Status **Aktion erforderlich** oder Überprüfung **der Registrierung.**|
| Inactive/Ineligible | Das Incentive-Programm ist derzeit möglicherweise nicht für die Registrierung geöffnet, oder der Partner erfüllt die aktuelle Berechtigung für die Registrierung oder erneute Registrierung nicht. <br><br> Wenn der Status **Ineligible** lautet, erfüllt der Partner nicht die aktuellen Berechtigungsanforderungen für das Programm. Wenn Sie unter dem Registrierungsstatus den Link **Berechtigungsanforderungen anzeigen** auswählen, werden die Anforderungen für die Berechtigung angezeigt, und welche dieser Anforderungen erfüllt wurden. <br><br> Möglicherweise wird auch ein **Inaktivitätsstatus** für Registrierungen virtueller Organisationen (VORG) oder globaler Partnerkonten (Partner Global Account, PGA) angezeigt, die nicht mehr im Incentive-Programm aktiv sind.  |
| Eingeladen  | Eine neue Einladung zur Incentiveprogrammregistrierung wurde an den Partner gesendet, aber der Partner hat den Registrierungsprozess noch nicht gestartet. In der nebenstehenden Spalte **Aktionen erforderlich** werden die nächsten Schritte und alle zugehörigen Links angezeigt.  |
| Überprüfen der Registrierung  | Der Partner hat bereits Bank- und Steuerinformationen für eine neue oder vorhandene Registrierung abgeschlossen oder aktualisiert und wartet darauf, dass Microsoft diese Informationen überprüft. Während des Überprüfungsprozesses kann die **Überprüfung der Registrierung** bis zu 48 Stunden lang angezeigt werden.  |

## <a name="see-your-payment-information"></a>Anzeigen Ihrer Zahlungsinformationen

Wählen Sie das Auszahlungssymbol in der oberen rechten Ecke des Bildschirms aus, um auf diese verschiedenen Zusammenfassungen zuzugreifen:

- Transaktionsverlauf
- Zahlungen
- Exportieren von Daten

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Auszahlungssymbol rechts oben im Partner Center-Portal":::

Diese Informationen umfassen den Gesamtgewinn und die Gesamtzahlungen, seit Sie sich bei Incentive-Programmen angemeldet haben. Diese Seite enthält auch Einnahmen und Zahlungen nach Standort oder Programm sowie alle weiteren Aktionen, die Sie möglicherweise durchführen müssen, um sich an einem bestimmten Ort bei einem Programm anzumelden. 

Sie können auch die [Partnerauszahlungs-API](https://apidocs.microsoft.com/services/partnerpayouts) verwenden, um direkt eine Verbindung mit Auszahlungstransaktionen und Zahlungsdaten herzustellen und diese abzurufen. Weitere Informationen finden Sie unter [Auszahlungsanweisungen.](payout-statement.md)

## <a name="next-steps"></a>Nächste Schritte

- [Auszahlungsauszüge](payout-statement.md)
