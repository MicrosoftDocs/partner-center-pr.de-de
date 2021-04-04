---
title: Verwalten von Nichtbezahlung, Betrug oder Missbrauch
description: Erfahren Sie mehr über die verschiedenen Risiken bei Online Transaktionen und die bewährten Methoden zum Verwalten und mindern dieser Risiken in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 75881544097abdfac8d6f96bde37e9700eb28cf7
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132348"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Verwalten von Nichtzahlung, Betrug oder Missbrauch im Partner Center

Gilt für:

- Partner Center für Microsoft Government Cloud

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Administrator-Agent
- Abrechnungsadministrator

Sie sind finanziell verantwortlich für betrügerische Einkäufe Ihrer Kunden und/oder für die Nichtzahlung von gekauften Dienstleistungen durch Ihre Kunden. Daher wird *dringend empfohlen, dass Sie die Verhinderung von Betrugsschutz-und Erkennungs Risiken durchsetzen*.

Um betrügerische Aktivitäten oder Missbrauch zu vermeiden und/oder zu bekämpfen, ist es wichtig, potenzielle Risiken zu verstehen und Richtlinien und Praktiken zu entwickeln, die Ihre Gefährdung verringern können.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Erzwingung der von Microsoft akzeptablen Nutzungsrichtlinie

Wenn Microsoft Partner-oder Kunden Aktivitäten erkennt, die wir bestätigen oder vermuten, dass Sie die akzeptable Nutzungsrichtlinie verletzen, führen wir Erzwingungs Schritte aus. Der Kunde könnte sofort angehalten werden. Sie werden über Erzwingungs Aktionen benachrichtigt oder bei Ihren Anfragen von Microsoft aktualisiert.

## <a name="abuse-of-service-risks"></a>Missbrauch von Dienst Risiken

**Der Missbrauch von Dienst** Risiken bedeutet, dass Kunden, die Clouddienste verwenden, gegen die akzeptable Nutzungsrichtlinie von Microsoft verstoßen.

### <a name="examples-of-abuse-of-service"></a>Beispiele für den Missbrauch von Diensten

Beispiele für diese Verstöße gegen die Acceptable Use Policy von Microsoft können Folgendes umfassen:

- Spamming
- Hacken
- Verteilte Denial-of-Service-Angriffe (DDoS)
- Bitcoin-Mining
- Verteilung von Schadsoftware
- Weiterverkauf unrechtmäßig erworbener Abonnements

## <a name="theft-of-service-risks"></a>Diebstahl von Dienst Risiken

**Der Diebstahl von Dienst** Risiken bedeutet, dass Kunden, die nicht über die Absicht verfügen, für genutzte Dienste zu bezahlen. Dieser Diebstahl kann die Verwendung von gestohlenen Zahlungsinstrumenten, das Bereitstellen falscher Abrechnungsinformationen und/oder das standardmäßige überprüfen von ausstehenden Guthaben beinhalten.

### <a name="examples-of-service-theft"></a>Beispiele für den Diebstahl von Diensten

Beispiele für diese Online Transaktionsrisiken sind:

- Transaktionen, die nicht in der Person vorkommen ("Kreditkarte nicht vorhanden" Transaktionen)
- Falsch angegebene Identitäten
- Dienste, die bereitgestellt und verwendet werden, bevor die erste Zahlung erfolgt
- Aufstrebende Märkte und/oder Hochrisiko Bereiche für Online Betrug
- Automatisieren der Kontoerstellung und des Kaufs durch fehlerhafte Actors

## <a name="managing-online-risk"></a>Verwalten des Online Risikos

Anhand der folgenden Empfehlungen können Sie Richtlinien und Vorgehensweisen entwickeln, um das Risiko von Online Transaktionsrisiken im Lebenszyklus Ihrer Kundenbeziehungen zu verringern.

### <a name="onboarding-new-customers"></a>Onboarding von neuen Kunden

Vorschläge zum Verringern von Online Risiken beim Onboarding von neuen Kunden:

- Richten Sie nach Möglichkeit persönliche Beziehungen mit Kunden ein (z. b. kontaktieren von Kunden per Telefon).
- Überprüfen Sie die Anmelde Informationen und den Hintergrund der Kunden durch bessere Methoden (z. b. durch die Verwendung von Gutschriften oder Geschäfts kommerziellen Berichten).
- Verwenden Sie die Multi-Factor Authentication (z. b. die SMS-Überprüfung) während der Registrierung, um das Risiko für die Erstellung und den Einkauf von Robotor
- Verwalten und Nachverfolgen von Identitäten mithilfe von Diensten (z. b. digitalen Identitäts Diensten).
- Bewerten Sie die Finanzstärke von Kunden durch strenge Kreditkarten-Betrugs Erkennungssysteme.
- Richten Sie eine Richtlinie zum Löschen von Sammlungen ein Beschreiben Sie den Prozess ihrer Sammlungen, und wenn der Zugriff auf Abonnements durch eine Nichtzahlung beeinträchtigt wird. (Sie können den Zugriff auf [die Abonnements eines Kunden für eine](create-a-new-subscription.md#suspend-a-subscription) Nichtzahlung deaktivieren oder diese Sperren.)

### <a name="managing-customer-accounts"></a>Kundenkonten

Vorschläge für die Verwaltung von Kundenkonten nach dem Kauf:

- Implementieren Sie einen Prozess zum schnellen empfangen, überprüfen, reagieren und reagieren auf Microsoft-Benachrichtigungen.
- Arbeiten Sie mit Kunden zusammen, um Ihre geschäftlichen Anforderungen für die cloudnutzung zu verstehen, während Sie Einstellungen für die Überwachung (Sie können z. b. [ein monatliches Azure-Ausgabenbudget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center festlegen. Mit diesem Verständnis können Sie die Kundennutzung während des Monats überwachen und benachrichtigt werden, wenn sich Kunden in der Nähe Ihres Budgets befinden.)
- Überwachen Sie die [Kunden Aktivitäts Protokolle](activity-logs.md) regelmäßig, um den Betrug frühzeitig zu
- Führen Sie schnell Maßnahmen aus, wenn verdächtige Aktivitäten erkannt werden.
- Vermeiden Sie es, den Benutzern vollen Administrator Zugriff auf Abonnements zu gewähren, ohne zuvor die Steuerungsmaßnahmen zur Risikominderung

### <a name="managing-customer-billing"></a>Verwalten der Kundenabrechnung

Vorschläge zur Verwaltung der Kundenabrechnung nach dem Kauf:

- Anfordern von Vorabzahlungen vor anfänglichen Transaktionen und der Abrechnung.
- Akzeptieren Sie keine risikoreichen Zahlungsinstrumente (z. b. vorab bezahlte Karten oder gespeicherte Wertkarten).
- Überwachen von Kunden Zahlungen und Abrechnungen von Konten. Erzwingen Sie eine aggressive Durchsetzung standardisierter Prozesse für späte Zahlungen oder eine Nichtzahlung.

Detailliertere Strategien zur Minderung des Onlinerisikos finden Sie in der [Anleitung zur Verwaltung von Onlinetransaktionsrisiken](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt).
