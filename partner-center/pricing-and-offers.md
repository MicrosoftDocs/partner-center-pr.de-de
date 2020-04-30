---
title: Preise und Angebote
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Die Angebotsliste enthält die verschiedenen Produktfamilien, die über Partner Center erworben werden können, sowie die entsprechenden Preise.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 19e935122d1223c87714ca8c3a3f4fd212f2cf3c
ms.sourcegitcommit: 4731d6647db34cf214f781f9e002074210fcfc29
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/21/2020
ms.locfileid: "81664285"
---
# <a name="pricing-and-offers"></a>Preise und Angebote

**Zielgruppe**

- Partner Center

**Geeignete Rollen**

- Globaler Administrator
- Benutzeradministrator
- Administrator-Agent
- MPN-Partneradministrator
- Vertriebsbeauftragter
- Abrechnungsadministrator

Um die neuesten Programme und Angebote für Cloud Solution Provider anzuzeigen, wechseln Sie im Partner Portal zu **verkaufen > Preise und Angebote**. Sie finden separate Preislisten für Lizenz basierte Dienste, einschließlich Office 365, Microsoft Dynamics CRM und Enterprise Mobility Suite, sowie für nutzungsbasierte Dienste, die Azure enthalten.

Die Angebotsliste enthält die verschiedenen Produktfamilien, die über Partner Center erworben werden können. Diese umfassen derzeit Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM und Microsoft Azure. Diese Liste wird weiterhin erweitert, wenn neue Produkte verfügbar werden.

In jeder dieser Produktfamilien gibt es verschiedene SKUs und Produktbündel, die Sie je nach Ihrem Unternehmen verkaufen können. Sie können jederzeit auf die neuesten Informationen zu diesen Produkten mithilfe der Cloud Reseller offer-Matrix zugreifen, die auf der Seite Preise und Angebote verfügbar ist.

## <a name="price-list-preview-and-change-frequency"></a>Preislisten Vorschau und Änderungs Häufigkeit 

Lizenz basierte Dienste enthalten eine Vorschau der Preisliste, die 30 Tage vor allen Änderungen bereitgestellt wird. Um die Vorschau der Preisliste anzuzeigen, besuchen Sie **> Preise und Angebote zu verkaufen**. Für nutzungsbasierte Dienste gibt es keine Preis Vorschau, da diese Dienste dynamisch sind. In der folgenden Tabelle wird erläutert, wie die Preislisten Tabelle gelesen wird.

|**Element**        |**Definition**      |
|:-----------   |:-----------   |
|ADD   |Ein neues Element in der Preisliste.|
|CHG   |Änderungen am Listenpreis von Monat zu Monat. Andere Änderungen, die nicht mit dem Listenpreis zusammenhängen, können eintreten, wenn Partner Preislisten zwischen Monaten vergleichen, um Änderungen an anderen Eigenschaften zu ermitteln.|
|DEL   |Ein Element, das aus der Preisliste entfernt wurde.|
|UNC   |Listenpreis unverändert aus der Preisliste des vorherigen Monats  |
|Gültig ab (Datum)   |Das erste Datum, an dem ein Angebot bestellt werden kann    |
|Gültig bis (Datum)   |Das letzte Datum, an dem ein Angebot bestellt werden kann   |
|Angebotsanzeigename   |Der für den Kunden sichtbare Name des Angebots   |
|Angebots-ID   |Der interne Bezeichner für das Angebot   |
|Lizenzvertragstyp   |Lizenzvertrags Typen können entweder "Corporate", "Government" oder "Academic" lauten. Der Vertragstyp bestimmt, an welche Kundentypen das Angebot verkauft werden kann.|
|Bestelleinheit   |Die Dauer des erworbenen Angebots. Kauf Einheiten sind in der Regel ein Monat.   |
|Sekundärer Lizenztyp   |Sekundäre Lizenztypen sind entweder nicht spezifisch, Add-on oder Testversion. Add-on gibt an, dass die erforderlichen Produkte vom Kunden vor dem Erwerb des Add-on erworben werden müssen.|
|Art des Endkunden   |Bezieht sich auf den Lizenz Vertragstyp: Corporate License-Cloud Reseller Corporate, Government License-Cloud Reseller Government oder Academic License-Cloud Reseller Dozenten oder Cloud Reseller Student   |
|Listenpreis   |Der Preis, den der Partner zahlt   |
|ERP-Preis   |Der geschätzte oder empfohlene Einzelhandelspreis für den Kunden   |

## <a name="price-changes"></a>Preisänderungen

Preisänderungen werden häufig vorkommen. Partner können Preisänderungen für Lizenz basierte Angebote antizipieren, indem Sie sich die Preislisten Vorschau ansehen. Öffnen Sie auf dem Partner Center-Dashboard die Seite "Preise und Angebote", um die Vorschau der Preisliste anzuzeigen.

Azure Usage-basierte Preise haben jedoch keine Vorschau. Partner können mithilfe der Ratecard-API, die die Abrechnungspreise für diesen Tag zurückgibt, die Preisänderungen für Azure-Verbrauchseinheiten aufrechterhalten.

|**Produkttyp**   |**Produktbeispiele**  |**Vorschau verfügbar** |**Details ändern**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Lizenz basiert|Office, Dynamics, InTune, Windows Enterprise|30 Tage|Auflisten von Preisänderungen, die in Vorschau Preislisten als "Chng|
|Verwendungs basiert|Azure-Ressourcen|Nicht verfügbar|Änderungsprotokoll in der Registerkarte " **Änderungs Verlauf** " des vorherigen Monats|
|Software||Nicht verfügbar|Manuelles Vergleichen von Preislisten von Monat zu Monat|
|Reservations|Virtuelle Computer, vorab bezahlt|Nicht verfügbar|Manuelles Vergleichen von Preislisten von Monat zu Monat|

Nutzungsbasierte Preise können sich im Laufe eines Monats ändern. Um die täglichen Preise für diese Azure-Ressourcen zu erhalten, müssen Partner die Ratecard-API anrufen. 

> [!Note] 
> Abonnementpreis Änderungen gelten nur während einer Verlängerung. Die monatliche Gebühr für einen Partner wird durch den Kauf Preis oder den Preis zum Zeitpunkt der Erstellung eines Abonnements festgelegt. Wenn ein Preis erhöht oder verringert wird, nachdem die Jahresfrist bezogen wurde, wird dem Partner der geänderte Preis bis zur Verlängerung nicht berechnet (in der Regel in der 12-monatigen Laufzeit).

## <a name="pricing-and-special-segments"></a>Preise und spezielle Segmente

CSP bietet einige Dienste für spezielle Marktsegmente, z. b. Education, Non-Profit und Government Community Cloud. Nicht alle Dienste sind in jedem Kanal verfügbar. Standardmäßig wird kein Segment verwendet, das als "kommerzielles"-Segment bezeichnet wird. Alle lizenzbasierten Preise sind in der lizenzbasierten Preisliste auf der Seite Preise und Angebote verfügbar. Azure Government Preise sind in der nutzungsbasierten Preisliste verfügbar, wenn Sie beim Azure Government aktivierten CSP-Mandanten angemeldet sind.

|**Segment**   |**Wer muss qualifiziert werden**   |**Partner qualifiziert Kunden**|**Aktivierte Produkttypen**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Education|Kunde|Nein, Kunden Qualifizierung wird von Microsoft durchgeführt. |Nur Lizenz basiert|
|Non-Profit|Kunde|Nein, Kunden, die sich außerhalb von Partner Center qualifizieren|Nur Lizenz basiert|
|Government Community Cloud (GCC)|Partner und Kunde|Nachdem gcc aktiviert wurde, kann der Partner gcc-Kunden erstellen.| Nur Lizenz basiert|
|Azure Government|Partner|Nach der Qualifikation arbeitet der Partner in einem CSP-Mandanten, der für Azure Government|Azure-Ressourcen|

Partner Ränder: der Unterschied zwischen dem Listenpreis und den geschätzten Einzelhandelspreisen kann von Segment zu Segment abweichen. In der Regel haben Education und Non-Profit für CSP-Partner tendenziell niedrigere oder keine Ränder. Genaue Werte finden Sie in der lizenzbasierten Preisliste.  
## <a name="pricing-between-azure-and-non-azure"></a>Preise zwischen Azure-Angeboten und Azure-fremden Angeboten

Die Preise unterscheiden sich in verschiedenen Angebots Typen. Lizenz basierte Preise sind in der Regel der Betrag pro Arbeitsplatz (Lizenz) für einen bestimmten Monat. Nutzungsbasierte Preise werden durch die Verwendung einer bestimmten Ressource und eine zugeordnete Abrechnungs-ID bestimmt. Für Partner fallen keine Gebühren für den Erwerb des Azure-Abonnements an. Allerdings werden den Partnern Ressourcen in Rechnung gestellt, die von verschiedenen bereit Stellungen im Rahmen des Azure-Abonnements beansprucht werden. Die Preise in der nutzungsbasierten Preisliste werden um verschiedene Ressourcen Zähler-IDs in Azure organisiert.

Azure-Reservierungen sind Begriffs basierte Käufe für den jeweiligen Ressourcentyp Virtual Machines. Der Erwerb einer Azure-Reservierung ermöglicht einem Partner das vorab bezahlen (ein oder drei Jahre) und die Reservierung eines bestimmten virtuellen Computers. Durch Reservierungen werden die Partner Kosten eingespart und sichergestellt, dass Ihr virtueller Computer für die Dauer der Laufzeit immer verfügbar ist. Ein Partner kann die gewünschte Reservierung an die nutzungsbasierten Ressourcen Zähler-IDs ausrichten. Die Abrechnungs Einheiten sind für die gesamte Ressource konsistent, unabhängig davon, ob der Partner einen virtuellen Computer kauft oder den virtuellen Computer einfach als Verwendungs basierte Ressource bereitstellt.

## <a name="offers-matrix"></a>Angebotsmatrix

Zeigen Sie auf der Seite "Preise und Angebote" die Angebots Matrix für den Cloud-Reseller an, um sich über die unterschiedlichen SKUs und Produktpakete zu informieren, die Ihnen zur Verfügung stehen. Die Angebotsmatrix gibt auch Aufschluss darüber, welche Angebote pro Gebiet verfügbar sind. Wenn ein Element in der Preisliste, aber nicht in der Angebots Matrix aufgeführt ist, bedeutet dies, dass die Produkte noch nicht sortiert werden können. Die Angebotsmatrix wird aktualisiert, sobald sie bestellt werden können.

Für CSP-Partner, die die Partner Center Software Development Kits (SDKs) verwenden. veröffentlicht Microsoft auf der Seite „Preise und Angebote“ auch eine Liste mit den Azure-Diensten in CSP.

### <a name="offers-matrix-and-price-list-questions"></a>Angebote zu Matrizen und Preislisten

Wenn Sie Fragen zur Preisliste oder Angebots Matrix haben, senden Sie eine Service Request über das Partner Center.

## <a name="offer-limits"></a>Angebots Limits

Einige Lizenz basierte Angebote haben bestimmte Regeln und Einschränkungen, die mehrere Käufe für denselben Kunden zulassen. Diese Regeln gelten für die meisten Tests und viele der kleinen geschäftlichen Angebote. **Small Business-Angebote** werden durch die Angebote definiert, die eine maximale Anzahl von Lizenzen aufweisen, die kleiner als 300 ist.

Diese Kauf Einschränkungen werden als Teil der Angebots Konfiguration definiert und können durch die Suche in der Angebots Listen Matrix gefunden werden. Zwei Datenspalten werden zusammen verwendet, um die Erzwingung zu definieren: 1. Bereich für Angebots Beschränkung und 2. Angebots Limit. Die Einschränkungen werden während eines Kaufs erzwungen. Der Katalog in Partner Center lässt nicht zu, dass ein Partner mehr Angebote kauft, als die Regeln zulassen. Jeder Versuch, die Einschränkungen zu verletzen, führt zu einem Fehler.

Der Bereich des Angebots Limits wird als Spalte in der Angebots Listen Matrix aufgezeichnet und kann Werte von "None", "Lifetime" oder "Concurrent" aufweisen. 

- Angebote mit " **keine** " können ohne Einschränkungen erworben werden.
- **Lebensdauer** -Angebote können nur einmal erworben werden.
- **Gleichzeitige** Angebote können so oft wie durch den Wert des **Angebots Limits** für dieses Angebot zugelassen erworben werden. Die meisten Testversionen verfügen über einen Gültigkeitsbereich für die Lebensdauer Angebote mit einem Angebots Limit von "1". Die meisten kleinen Geschäftsangebote verfügen über einen Grenzwert für gleichzeitige Angebote mit einem Angebots Limit von "2".

> [!IMPORTANT]
> Parallelitäts Grenzwerte werden auch dann erzwungen, wenn ein Angebot abgebrochen wird. Ein Angebot muss vollständig abgebrochen und dann bereitgestellt werden, um einen zusätzlichen Speicherplatz freizugeben, der einen anderen Kauf ermöglicht.

### <a name="taxes-and-pricing"></a>Steuern und Preise

Alle Preise in den Preislisten der Partner Center-CSP sind Tax inklusiv. Weitere Informationen finden Sie im Partner Center in den Dokumenten [Steuern und Steuern](tax-and-tax-exemptions.md).
