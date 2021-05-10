---
title: Verwalten von Nichtbezahlung, Betrug oder Missbrauch
description: Erfahren Sie mehr über die verschiedenen Risiken im Zusammenhang mit Onlinetransaktionen und die bewährten Methoden zum Verwalten und Minimieren dieser Risiken in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686295"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Verwalten von Nichtzahlung, Betrug oder Missbrauch im Partner Center

**Zielgruppe**

- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Administrator-Agent
- Abrechnungsadministrator

Sie sind finanziell verantwortlich für betrügerische Einkäufe Ihrer Kunden und/oder für die Nichtzahlung von gekauften Dienstleistungen durch Ihre Kunden. Aus diesem *Grund wird dringend empfohlen, Kontrollen* zur Betrugs- und Erkennungsrisikominderung zu verwenden.

Um betrügerische Aktivitäten oder Missbrauch zu vermeiden und/oder zu bekämpfen, ist es wichtig, potenzielle Risiken zu verstehen und Richtlinien und Praktiken zu entwickeln, die Ihre Gefährdung verringern können.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Erzwingung der Microsoft-Richtlinie zur zulässigen Verwendung

Wenn Microsoft Partner- oder Kundenaktivitäten erkennt, die wir bestätigen oder vermuten, dass sie gegen die Richtlinie zur zulässigen Verwendung verstoßen, werden wir Schritte zur Erzwingung ergreifen. Der Kunde kann sofort angehalten werden. Sie werden über Erzwingungsaktionen benachrichtigt oder auf Ihre Anforderungen von Microsoft aktualisiert.

## <a name="abuse-of-service-risks"></a>Missbrauch von Dienstrisiken

**Missbrauch von Dienstrisiken** bedeutet, dass Kunden, die Clouddienste verwenden, gegen die Richtlinie zur zulässigen Nutzung von Microsoft verstoßen.

### <a name="examples-of-abuse-of-service"></a>Beispiele für missbrauchten Dienst

Beispiele für diese Verstöße gegen die Richtlinie zur zulässigen Verwendung von Microsoft sind:

- Spamming
- Hacken
- Verteilte Denial-of-Service-Angriffe (DDoS)
- Bitcoin-Mining
- Verteilung von Schadsoftware
- Weiterverkauf unrechtmäßig erworbener Abonnements

## <a name="theft-of-service-risks"></a>Diebstahl von Dienstrisiken

**Der Diebstahl von Dienstrisiken** bedeutet, dass Kunden nicht die Absicht haben, für verbrauchte Dienste zu zahlen. Bei diesem Diebstahl kann es sich um die Verwendung gestohlener Zahlungsmittel, die Bereitstellung falscher Abrechnungsinformationen und/oder den Ausfall ausstehender Salden handelt.

### <a name="examples-of-service-theft"></a>Beispiele für Dienstdiebstahl

Beispiele für diese Onlinetransaktionsrisiken sind:

- Transaktionen, die nicht persönlich auftreten ("Kreditkartentransaktionen nicht vorhanden")
- Falsch angegebene Identitäten
- Dienste, die bereitgestellt und verwendet werden, bevor die erste Zahlung empfangen wird
- Neue Märkte und/oder Regionen mit hohem Risiko für Online-Betrug
- Automatisieren der Kontoerstellung und des Kaufs durch Bad Actors

## <a name="managing-online-risk"></a>Verwalten von Onlinerisiken

Sie können die folgenden Empfehlungen verwenden, um Richtlinien und Methoden zu entwickeln, um die Gefährdung durch Onlinetransaktionsrisiken im Lebenszyklus Ihrer Kundenbeziehungen zu reduzieren.

### <a name="onboarding-new-customers"></a>Onboarding neuer Kunden

Vorschläge zur Verringerung von Onlinerisiken beim Onboarding neuer Kunden:

- Stellen Sie nach Möglichkeit persönliche Beziehungen mit Kunden her (z. B. telefonische Kontaktaufnahme mit Kunden).
- Überprüfen Sie die Anmeldeinformationen und den Hintergrund der Kunden mithilfe besserer Methoden (z. B. mitHilfe von Kreditausstellen oder Geschäftlichen Berichtsbehörden).
- Verwenden Sie die mehrstufige Authentifizierung (z. B. SMS-Überprüfung) während der Registrierung, um die Gefährdung durch die Erstellung und den Kauf von Roboterkonten zu minimieren.
- Verwalten und Nachverfolgen von Identitäten mithilfe von Diensten (z. B. digitale Identitätsdienste).
- Bewerten Sie die Finanzielle Stärke der Kunden mithilfe strenger Systeme zur Erkennung von Kreditkarten betrugsversuchen.
- Richten Sie eine Richtlinie für eindeutige Sammlungen ein. Beschreiben Sie Ihren Sammlungsprozess und wann der Zugriff auf Abonnements durch die Nichtzahlung beeinträchtigt wird. (Sie können den Zugriff deaktivieren oder [abonnements eines Kunden aussetzen,](create-a-new-subscription.md#suspend-a-subscription) wenn keine Zahlung erfolgt.)

### <a name="managing-customer-accounts"></a>Kundenkonten

Vorschläge für die Verwaltung von Kundenkonten nach dem Kauf:

- Implementieren Sie einen Prozess zum schnellen Empfangen, Überprüfen, Reagieren auf und Reagieren auf Microsoft-Benachrichtigungen.
- Arbeiten Sie mit Kunden zusammen, um ihre Geschäftlichen Anforderungen an die Cloudnutzung zu verstehen, während Sie geeignete Überwachungsschwellenwerte festlegen. (Beispielsweise können Sie [ein monatliches Azure-Ausgabenbudget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center festlegen. Dieses Verständnis ermöglicht es Ihnen, die Kundennutzung während des Monats zu überwachen und benachrichtigt zu werden, wenn Kunden ihrem Budget nahe kommen.)
- Überwachen Sie regelmäßig [Kundenaktivitätsprotokolle,](activity-logs.md) um Betrug frühzeitig zu erkennen.
- Ergreifen Sie schnelle Maßnahmen, wenn verdächtige Aktivitäten erkannt werden.
- Vermeiden Sie es, Kunden vollständigen Administratorzugriff auf Abonnements zu erteilen, ohne zuerst Kontrollen zur Risikominderung zu implementieren.

### <a name="managing-customer-billing"></a>Verwalten der Kundenabrechnung

Vorschläge für die Verwaltung der Kundenabrechnung nach dem Kauf sind:

- Fordern Sie Vorauszahlungen vor den ersten Transaktionen und der Abrechnung an.
- Akzeptieren Sie keine Risikozahlungsarten (z. B. vorausbezahlungte Karten oder Karten mit gespeicherten Wert).
- Überwachen Sie Kundenzahlungen und veraltete Konten. Erzwingen Sie aggressiv standardisierte Dunningprozesse bei Zahlungsverzug oder Nichtzahlung.

Detailliertere Strategien zur Minderung des Onlinerisikos finden Sie in der [Anleitung zur Verwaltung von Onlinetransaktionsrisiken](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt).
