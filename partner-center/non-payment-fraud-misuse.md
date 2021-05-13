---
title: Verwalten von Nichtbezahlung, Betrug oder Missbrauch
description: Erfahren Sie mehr über die verschiedenen Risiken, die mit Onlinetransaktionen verbunden sind, und die bewährten Methoden zum Verwalten und Mindern dieser Risiken in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 1d8e59ea2d2e8d40163ea06b305845c37a356f16
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818659"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Verwalten von Nichtzahlung, Betrug oder Missbrauch im Partner Center

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** globale | | des Benutzerverwaltungsadministrators | des Administrator-Agents Abrechnungsadministrator

Sie sind finanziell verantwortlich für betrügerische Einkäufe Ihrer Kunden und/oder für die Nichtzahlung von gekauften Dienstleistungen durch Ihre Kunden. Aus diesem Grund wird dringend empfohlen, Kontrollen *zur Betrugs- und Erkennungsrisikominderung zu erstellen.*

Um betrügerische Aktivitäten oder Missbrauch zu vermeiden und/oder zu bekämpfen, ist es wichtig, potenzielle Risiken zu verstehen und Richtlinien und Praktiken zu entwickeln, die Ihre Gefährdung verringern können.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Erzwingung der Microsoft-Richtlinie zur zulässigen Verwendung

Wenn Microsoft Partner- oder Kundenaktivitäten erkennt, die wir bestätigen oder vermuten, dass sie gegen die Richtlinie zur zulässigen Nutzung verstoßen, führen wir Erzwingungsschritte aus. Der Kunde kann sofort angehalten werden. Sie werden über Erzwingungsaktionen benachrichtigt oder auf Ihre Anforderungen von Microsoft aktualisiert.

## <a name="abuse-of-service-risks"></a>Missbrauch von Dienstrisiken

**Missbrauch von Dienstrisiken** bedeutet, dass Kunden, die Clouddienste verwenden, gegen die Nutzungsrichtlinie von Microsoft verstoßen.

### <a name="examples-of-abuse-of-service"></a>Beispiele für den Missbrauch des Diensts

Beispiele für diese Verstöße gegen die zulässige Verwendungsrichtlinie von Microsoft sind:

- Spamming
- Hacken
- Verteilte Denial-of-Service-Angriffe (DDoS)
- Bitcoin-Mining
- Verteilung von Schadsoftware
- Weiterverkauf unrechtmäßig erworbener Abonnements

## <a name="theft-of-service-risks"></a>Diebstahl von Dienstrisiken

**Der Diebstahl von Dienstrisiken** bedeutet, dass Kunden, die nicht beabsichtigen, für genutzte Dienste zu bezahlen. Dieser Diebstahl kann die Verwendung gestohlener Zahlungsmethoden, das Bereitstellen falscher Abrechnungsinformationen und/oder die Standardeinstellung für ausstehende Guthaben umfassen.

### <a name="examples-of-service-theft"></a>Beispiele für Dienstdiebstahl

Beispiele für diese Onlinetransaktionsrisiken sind:

- Transaktionen, die nicht persönlich auftreten ("Kreditkartentransaktionen nicht vorhanden")
- Falsch angegebene Identitäten
- Dienste, die bereitgestellt und verwendet werden, bevor die erste Zahlung empfangen wird
- Neue Märkte und/oder Regionen mit hohem Risiko für Online-Betrug
- Automatisieren der Kontoerstellung und des Kaufs durch Bad Actors

## <a name="managing-online-risk"></a>Verwalten von Onlinerisiken

Sie können die folgenden Empfehlungen verwenden, um Richtlinien und Vorgehensweisen zu entwickeln, mit denen Sie das Risiko von Onlinetransaktionsrisiken im Lebenszyklus Ihrer Kundenbeziehungen reduzieren können.

### <a name="onboarding-new-customers"></a>Onboarding neuer Kunden

Vorschläge zur Reduzierung von Onlinerisiken beim Onboarding neuer Kunden:

- Richten Sie nach Möglichkeit persönliche Beziehungen mit Kunden ein (z. B. telefonische Kontaktaufnahme mit Kunden).
- Überprüfen Sie die Anmeldeinformationen und den Hintergrund von Kunden mithilfe besserer Methoden (z. B. mithilfe von Kreditbüros oder Geschäftsberichtsstellen).
- Verwenden Sie die mehrstufige Authentifizierung (z. B. SMS-Überprüfung) während der Anmeldung, um die Gefährdung durch die Erstellung und den Erwerb von Roboterkontos zu minimieren.
- Verwalten und Nachverfolgen von Identitäten mithilfe von Diensten (z. B. digitale Identitätsdienste).
- Bewerten Sie die Finanzstärke der Kunden durch strenge Betrugserkennungssysteme für Kreditkarten.
- Richten Sie eine klare Sammlungsrichtlinie ein. Beschreiben Sie den Inkassoprozess, und geben Sie an, wann der Zugriff auf Abonnements durch Nichtzahlungsvorgänge wirkt. (Sie können den Zugriff deaktivieren [oder abonnements eines](create-a-new-subscription.md#suspend-a-subscription) Kunden bei Nichtzahlung aussetzen.)

### <a name="managing-customer-accounts"></a>Kundenkonten

Vorschläge für die Verwaltung von Kundenkonten nach dem Kauf sind:

- Implementieren Sie einen Prozess, um Microsoft-Benachrichtigungen schnell zu empfangen, zu überprüfen, zu verarbeiten und darauf zu reagieren.
- Arbeiten Sie mit Kunden zusammen, um ihre Geschäftlichen Anforderungen an die Cloudnutzung zu verstehen, während Sie geeignete Überwachungsschwellenwerte festlegen. (Sie können z. B. [ein monatliches Azure-Ausgabenbudget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center. Dieses Verständnis ermöglicht es Ihnen, die Kundennutzung während des Monats zu überwachen und benachrichtigt zu werden, wenn kunden sich in der Nähe ihres Budgets befinden.)
- Überwachen [Sie regelmäßig Kundenaktivitätsprotokolle,](activity-logs.md) um Betrug frühzeitig zu erkennen.
- Ergreifen Sie schnelle Maßnahmen, wenn verdächtige Aktivitäten erkannt werden.
- Vermeiden Sie es, Kunden vollständigen Administratorzugriff auf Abonnements zu erteilen, ohne zuerst Kontrollen zur Risikominderung zu implementieren.

### <a name="managing-customer-billing"></a>Verwalten der Kundenabrechnung

Vorschläge für die Verwaltung der Kundenabrechnung nach dem Kauf:

- Fordern Sie Vorauszahlungen vor den ersten Transaktionen und der Abrechnung an.
- Akzeptieren Sie keine Zahlungsinstrument mit hohem Risiko (z. B. vorab bezahlte Karten oder karten mit gespeicherten Werten).
- Überwachen Von Kundenzahlungen und Konten mit Alterung Aggressives Erzwingen standardisierter Dunningprozesse bei zahlungsverzugeter oder nicht erfolgter Zahlung.

Detailliertere Strategien zur Minderung des Onlinerisikos finden Sie in der [Anleitung zur Verwaltung von Onlinetransaktionsrisiken](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt).
