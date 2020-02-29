---
title: Preise und Angebote | Partner Center
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Die Angebotsliste enthält die verschiedenen Produktfamilien, die über Partner Center erworben werden können, sowie die entsprechenden Preise.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e33b89e76a57e1e6f5457e208a61bc04ad841271
ms.sourcegitcommit: 2634057663a0ea27393212f898018538dada796e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/28/2020
ms.locfileid: "78161514"
---
# <a name="pricing-and-offers"></a>Preise und Angebote

**Gilt für:**

-  Partner Center

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Administratoragent
-   MPN-Partneradministrator
-   Vertriebsbeauftragter
-   Abrechnungsadministrator

Die neuesten Angebote und Angebote für das Cloud Solution Provider-Programm finden Sie unter **verkaufen > Preise und Angebote**. Sie finden separate Preislisten für Lizenz basierte Dienste wie Office 365, Microsoft Dynamics CRM und Enterprise Mobility Suite und Verwendungs basierte Dienste, die Azure enthalten. 

Die Angebotsliste enthält die verschiedenen Produktfamilien, die über Partner Center erworben werden können. Diese umfassen derzeit Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM und Microsoft Azure. Diese Liste wird weiterhin erweitert, wenn neue Produkte verfügbar werden.

In jeder dieser Produktfamilien gibt es verschiedene SKUs und Produktbündel, die Sie je nach Ihrem Unternehmen verkaufen können. Sie können jederzeit auf die neuesten Informationen zu diesen Produkten mithilfe der Cloud Reseller offer-Matrix zugreifen, die auf der Seite Preise und Angebote verfügbar ist.

## <a name="price-list-preview-and-change-frequency"></a>Preislisten Vorschau und Änderungs Häufigkeit 

Lizenz basierte Dienste enthalten eine Vorschau der Preisliste, die 30 Tage vor allen Änderungen bereitgestellt wird. Um die Vorschau der Preisliste anzuzeigen, besuchen Sie **> Preise und Angebote zu verkaufen**. Für nutzungsbasierte Dienste steht keine Preisvorschau zur Verfügung, da diese Dienste dynamisch sind. In der folgenden Tabelle wird erläutert, wie die Preislisten Tabelle gelesen wird.

|**Artikel**        |**Definition**      |
|:-----------   |:-----------   |
|HINZUFÜGEN   |Ein neues Element in der Preisliste.|
|CHG   |Änderungen am Listenpreis von Monat zu Monat. Andere Änderungen, die nicht mit dem Listenpreis zusammenhängen, können eintreten, wenn Partner Preislisten zwischen Monaten vergleichen, um Änderungen an anderen Eigenschaften zu ermitteln.|
|DEL   |Ein Element, das aus der Preisliste entfernt wurde.|
|UNC   |Listenpreis unverändert aus der Preisliste des vorherigen Monats  |
|Gültig ab (Datum)   |Das erste Datum, an dem ein Angebot bestellt werden kann    |
|Gültig bis (Datum)   |Das letzte Datum, an dem ein Angebot bestellt werden kann   |
|Angebotsanzeigename   |Der für den Kunden sichtbare Name des Angebots   |
|Angebots-ID   |Der interne Bezeichner für das Angebot   |
|Lizenzvertragstyp   |Lizenzvertrags Typen können entweder Unternehmen, Government oder Academic sein und bestimmen, an welche Kundentypen das Angebot verkauft werden kann.|
|Bestelleinheit   |Die Dauer des erworbenen Angebots. Kauf Einheiten sind in der Regel ein Monat.   |
|Sekundärer Lizenztyp   |Sekundäre Lizenztypen sind entweder nicht spezifisch, Add-on oder Testversion. Die Add-On-Option gibt an, dass der Kunde über bestimmte Produkte verfügen muss, um das Add-On erwerben zu können.|
|Art des Endkunden   |Bezieht sich auf den Lizenz Vertragstyp: Corporate License-Cloud Reseller Corporate, Government License-Cloud Reseller Government oder Academic License-Cloud Reseller Dozenten oder Cloud Reseller Student   |
|Listenpreis   |Der Preis, den der Partner zahlt   |
|ERP-Preis   |Der geschätzte oder empfohlene Einzelhandelspreis für den Kunden   |

## <a name="price-changes"></a>Preisänderungen

Preisänderungen werden häufig vorkommen. Partner können Preisänderungen für Lizenz basierte Angebote einschätzen, indem Sie sich die Preislisten Vorschau auf der Seite Preise und Angebote auf dem Partner Center-Dashboard ansehen. Azure Usage-basierte Preise haben keine Vorschau. Partner können mithilfe der Ratecard-API, die die Abrechnungspreise für diesen Tag zurückgibt, die Preisänderungen für Azure-Verbrauchseinheiten aufrechterhalten.

|**Produkttyp**   |**Produktbeispiele**  |**Vorschau verfügbar** |**Details ändern**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Lizenz basiert|Office, Dynamics, InTune, Windows Enterprise|30 Tage|Auflisten von Preisänderungen, die in Vorschau Preislisten als "Chng|
|Verwendungs basiert|Azure-Ressourcen|Nicht verfügbar|Änderungsprotokoll in der Registerkarte " **Änderungs Verlauf** " des vorherigen Monats|
|Software||Nicht verfügbar|Manuelles Vergleichen von Preislisten von Monat zu Monat|
|Reservierungen|Virtuelle Computer, vorab bezahlt|Nicht verfügbar|Manuelles Vergleichen von Preislisten von Monat zu Monat|

Nutzungsbasierte Preise können sich im Laufe eines Monats ändern. Um die täglichen Preise für diese Azure-Ressourcen zu erhalten, müssen Partner die Ratecard-API anrufen. 

>[!Note] 
>Abonnementpreis Änderungen gelten nur während einer Verlängerung. Die monatliche Gebühr für einen Partner wird durch den Kauf Preis oder den Preis zum Zeitpunkt der Erstellung eines Abonnements festgelegt. Wenn ein Preis erhöht oder verringert wird, nachdem die Jahresfrist bezogen wurde, wird dem Partner der geänderte Preis bis zur Verlängerung nicht berechnet (in der Regel in der 12-monatigen Laufzeit).

## <a name="pricing-and-special-segments"></a>Preise und spezielle Segmente

CSP bietet einige Dienste für spezielle Marktsegmente, z. b. Education, Non-Profit und Government Community Cloud. Nicht alle Dienste sind in allen Kanälen verfügbar. Standardmäßig wird kein Segment verwendet, das als "kommerzielles"-Segment bezeichnet wird. Alle lizenzbasierten Preise sind in der lizenzbasierten Preisliste auf der Seite Preise und Angebote verfügbar. Azure Government Preise sind in der nutzungsbasierten Preisliste verfügbar, wenn Sie beim Azure Government aktivierten CSP-Mandanten angemeldet sind.

|**Segment**   |**Wer muss qualifiziert werden**   |**Partner qualifiziert Kunden**|**Aktivierte Produkttypen**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Bildung|Kunde|Nein, Kunden Qualifizierung wird von Microsoft durchgeführt. |Nur Lizenz basiert|
|Non-Profit|Kunde|Nein, Kunden, die sich außerhalb von Partner Center qualifizieren|Nur Lizenz basiert|
|Government Community Cloud (gcc)|Partner und Kunde|Nachdem gcc aktiviert wurde, kann der Partner gcc-Kunden erstellen.| Nur Lizenz basiert|
|Azure gov|Partner-|Nach der Qualifikation arbeitet der Partner in einem CSP-Mandanten, der für Azure gov spezifisch ist.|Azure-Ressourcen|

Partner Ränder: der Unterschied zwischen dem Listenpreis und den geschätzten Einzelhandelspreisen kann von Segment zu Segment abweichen. In der Regel haben Education und Non-Profit für CSP-Partner tendenziell niedrigere oder keine Ränder. Genaue Werte finden Sie in der lizenzbasierten Preisliste.  
## <a name="pricing-between-azure-and-non-azure"></a>Preise zwischen Azure und nicht-Azure

Die Preise unterscheiden sich in verschiedenen Angebots Typen. Lizenz basierte Preise sind in der Regel der Betrag pro Arbeitsplatz (Lizenz) für einen bestimmten Monat. Nutzungsbasierte Preise werden durch die Verwendung einer bestimmten Ressource und eine zugeordnete Abrechnungs-ID bestimmt. Für Partner fallen keine Gebühren für den Erwerb des Azure-Abonnements an, werden aber für Ressourcen in Rechnung gestellt, die von verschiedenen bereit Stellungen im Abonnement genutzt werden. Die Preise in der nutzungsbasierten Preisliste werden um verschiedene Ressourcen Zähler-IDs in Azure organisiert.

Azure-Reservierungen sind Begriffs basierte Käufe für den jeweiligen Ressourcentyp Virtual Machines. Der Erwerb einer Azure-Reservierung ermöglicht einem Partner die vorab Zahlung (ein oder drei Jahre) und die Reservierung eines bestimmten virtuellen Computers, das Speichern der Partner Kosten und die Sicherstellung, dass der virtuelle Computer für die Dauer der Laufzeit immer verfügbar ist. Ein Partner kann die gewünschte Reservierung an die nutzungsbasierten Ressourcen Zähler-IDs ausrichten. Die Abrechnungs Einheiten sind für die gesamte Ressource konsistent, unabhängig davon, ob der Partner einen virtuellen Computer kauft oder den virtuellen Computer einfach als Verwendungs basierte Ressource bereitstellt. 


## <a name="offers-matrix"></a>Angebotsmatrix

In der Angebotsmatrix für Cloud-Handelspartner auf der Seite „Preise und Angebote“ erfahren Sie, welche SKUs und Produktpakete Sie verkaufen können. Die Angebotsmatrix gibt auch Aufschluss darüber, welche Angebote pro Gebiet verfügbar sind. Wenn ein Element in der Preisliste enthalten ist, aber noch nicht in der Angebots Matrix aufgeführt ist, bedeutet dies, dass die Produkte noch nicht sortiert werden können. Die Angebotsmatrix wird aktualisiert, sobald sie bestellt werden können.

Für CSP-Partner, die den Partner Center Software Development Kits (SDKs) verwenden. veröffentlicht Microsoft auf der Seite „Preise und Angebote“ auch eine Liste mit den Azure-Diensten in CSP.

### <a name="offers-matrix-and-price-list-questions"></a>Angebote zu Matrizen und Preislisten

Wenn Sie Fragen zur Preisliste oder Angebots Matrix haben, senden Sie eine Service Request über das Partner Center.

### <a name="taxes-and-pricing"></a>Steuern und Preise

Alle Preise in den Preislisten der Partner Center-CSP sind Tax inklusiv. Weitere Informationen finden Sie im Partner Center in den Dokumenten [Steuern und Steuern](https://docs.microsoft.com/partner-center/tax-and-tax-exemptions).
