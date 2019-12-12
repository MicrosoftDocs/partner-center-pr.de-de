---
title: Preise und Angebote | Partner Center
ms.topic: article
ms.date: 09/26/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Die Angebotsliste enthält die verschiedenen Produktfamilien, die über Partner Center erworben werden können, sowie die entsprechenden Preise.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 0e81ead73308902e75b842c00bbd32ed228ca3a5
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004949"
---
# <a name="pricing-and-offers"></a>Preise und Angebote

**Zielgruppe**

-  Partner Center

**Geeignete Rollen**
-   Globaler Administrator
-   Benutzeradministrator
-   Administratoragent
-   MPN-Partneradministrator
-   Vertriebsbeauftragter
-   Abrechnungsadministrator

Die neuesten Preislisten und Angebote des Cloud Solution Provider-Programms finden Sie unter **Verkaufen > Preise und Angebote**. Dort finden Sie separate Preislisten für lizenzbasierte Dienste wie Office 365, Microsoft Dynamics CRM und Enterprise Mobility Suite sowie für nutzungsbasierte Dienste (einschließlich Azure). 

Die Angebotsliste enthält die verschiedenen Produktfamilien, die über Partner Center erworben werden können. Hierzu zählen aktuell Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM und Microsoft Azure. Diese Liste wird mit der Zeit erweitert.

Innerhalb dieser Produktfamilien gibt es verschiedene SKUs und Produktpakete, die Sie abhängig von Ihrem Geschäft verkaufen können. Über die Angebotsmatrix für Cloud-Handelspartner auf der Seite „Preise und Angebote“ stehen Ihnen stets die neuesten Informationen zur Verfügung.

## <a name="pricelist-preview-and-change-frequency"></a>Preislistenvorschau und Änderungshäufigkeit 

Lizenzbasierte Dienste umfassen eine Preislistenvorschau, die 30 Tage vor jeglichen Änderungen bereitgestellt wird. Die Preislistenvorschau finden Sie unter **Verkaufen > Preise und Angebote**. Für nutzungsbasierte Dienste steht keine Preisvorschau zur Verfügung, da diese Dienste dynamisch sind. Die folgende Tabelle zeigt, wie Sie die Preislistentabelle lesen.

|**Artikel**        |**Definition**      |
|:-----------   |:-----------   |
|HINZUFÜGEN   |Neuer Preislistenartikel|
|CHG   |Änderungen am Listenpreis von Monat zu Monat. Andere Änderungen, die nicht mit dem Listenpreis zusammenhängen, können eintreten, wenn Partner andere Eigenschaften von Monat zu Monat vergleichen, um andere Änderungen zu bestimmen.|
|ENTFERNEN   |Aus der Preisliste entfernter Artikel|
|UNC   |Listenpreis unverändert aus der pricelist des vorherigen Monats  |
|Gültig ab (Datum)   |Das erste Datum, an dem ein Angebot bestellt werden kann    |
|Gültig bis (Datum)   |Das letzte Datum, an dem ein Angebot bestellt werden kann   |
|Angebotsanzeigename   |Der für den Kunden sichtbare Name des Angebots   |
|Angebots-ID   |Der interne Bezeichner für das Angebot   |
|Lizenzvertragstyp   |„Unternehmen“, „Behörde“ oder „Wissenschaftlich“. Bestimmt, an welchen Kundentyp das Angebot verkauft werden kann.|
|Bestelleinheit   |Die Dauer des erworbenen Angebots. In der Regel ein Monat.   |
|Sekundärer Lizenztyp   |Entweder nicht spezifisch, Add-On oder Testversion. Die Add-On-Option gibt an, dass der Kunde über bestimmte Produkte verfügen muss, um das Add-On erwerben zu können.|
|Art des Endkunden   |Geht zurück auf die Art des Softwarelizenzvertrags: Unternehmenslizenz (Cloud-Handelspartner für Unternehmen), Behördenlizenz (Cloud-Handelspartner für Behörden) oder wissenschaftliche Lizenz (Cloud-Handelspartner für Lehrkräfte oder Cloud-Handelspartner für Schüler/Studenten)   |
|Listenpreis   |Der Preis, den der Partner zahlt   |
|ERP-Preis   |Der geschätzte oder empfohlene Einzelhandelspreis für den Kunden   |

## <a name="price-changes"></a>Preisänderungen

Preisänderungen werden häufig vorkommen. Partner können Preisänderungen für Lizenz basierte Angebote einschätzen, indem Sie sich die Preislisten Vorschau auf der Seite Preise und Angebote auf dem Partner Center-Dashboard ansehen. Azure Usage-basierte Preise haben keine Vorschau. Partner können mit der Gebühren Karten-API von Azure den Preis für die Preisgestaltung von Azure erhöhen, die die Verbrauchs Preise für diesen Tag zurückgibt.

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

CSP bietet einige Dienste für spezielle Marktsegmente, z. b. Education, Non-Profit und Government Community Cloud. Nicht alle Dienste sind in allen Kanälen verfügbar. Standardmäßig wird kein Segment verwendet, das als "kommerzielles"-Segment bezeichnet wird. Alle lizenzbasierten Preise sind in der lizenzbasierten Preisliste auf der Seite Preise und Angebote verfügbar. Azure gov-Preise sind in der nutzungsbasierten Preisliste verfügbar, wenn Sie beim Azure gov-aktivierten CSP-Mandanten angemeldet sind.

|**Segment**   |**Wer muss qualifiziert werden**   |**Partner qualifiziert Kunden**|**Aktivierte Produkttypen**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Education|Partner und Kunde|„Ja“|Nur Lizenz basiert|
|Gemeinnützig|Kunde|Nein, Kunden, die sich außerhalb von Partner Center qualifizieren|Nur Lizenz basiert|
|Government Community Cloud (GCC)|Partner und Kunde|Nachdem gcc aktiviert wurde, kann der Partner gcc-Kunden erstellen.| Nur Lizenz basiert|
|Azure gov|Partner|Nach der Qualifikation arbeitet der Partner in einem CSP-Mandanten, der für Azure gov spezifisch ist.|Azure-Ressourcen|

Partner Ränder: der Unterschied zwischen dem Listenpreis und den geschätzten Einzelhandelspreisen kann von Segment zu Segment abweichen. In der Regel haben Education und Non-Profit für CSP-Partner tendenziell niedrigere oder keine Ränder. Genaue Werte finden Sie in der lizenzbasierten Preisliste.  
## <a name="pricing-between-azure-and-non-azure"></a>Preise zwischen Azure und nicht-Azure

Die Preise unterscheiden sich in verschiedenen Angebots Typen. Lizenz basierte Preise sind in der Regel der Betrag pro Arbeitsplatz (Lizenz) für einen bestimmten Monat. Nutzungsbasierte Preise werden durch die Verwendung einer bestimmten Ressource und eine zugeordnete Abrechnungs-ID bestimmt. Für Partner fallen keine Gebühren für den Erwerb des Azure-Abonnements an, werden aber für Ressourcen in Rechnung gestellt, die von verschiedenen bereit Stellungen im Abonnement genutzt werden. Die Preise in der nutzungsbasierten Preisliste werden um verschiedene Ressourcen Zähler-IDs in Azure organisiert.

Azure-Reservierungen sind Begriffs basierte Käufe für den jeweiligen Ressourcentyp Virtual Machines. Der Erwerb einer Azure-Reservierung ermöglicht einem Partner das vorab bezahlen (ein oder drei Jahre) und die Reservierung eines bestimmten virtuellen Computers. Dadurch wird der Partner Geld gespart, und es wird sichergestellt, dass der virtuelle Computer für die Dauer der Laufzeit immer verfügbar ist. Ein Partner kann die gewünschte Reservierung an die nutzungsbasierten Ressourcen Zähler-IDs ausrichten. Die Abrechnungs Einheiten sind für die gesamte Ressource konsistent, unabhängig davon, ob der Partner einen virtuellen Computer kauft oder den virtuellen Computer einfach als Verwendungs basierte Ressource bereitstellt. 


## <a name="offers-matrix"></a>Angebotsmatrix

In der Angebotsmatrix für Cloud-Handelspartner auf der Seite „Preise und Angebote“ erfahren Sie, welche SKUs und Produktpakete Sie verkaufen können. Die Angebotsmatrix gibt auch Aufschluss darüber, welche Angebote pro Gebiet verfügbar sind. Wenn ein Artikel zwar in der Preisliste, aber noch nicht in der Angebotsmatrix enthalten ist, bedeutet das, dass die Produkte noch nicht bestellt werden können. Die Angebotsmatrix wird aktualisiert, sobald sie bestellt werden können.

Für CSP-Partner, die die Partner Center-SDKs (Software Development Kits) verwenden, veröffentlicht Microsoft auf der Seite „Preise und Angebote“ auch eine Liste mit den Azure-Diensten in CSP.

### <a name="offers-matrix-and-pricelist-questions"></a>Fragen zu Angebotsmatrix und Preisliste

Sollten Sie Fragen zur Angebotsmatrix oder zur Preisliste haben, senden Sie eine Serviceanfrage über Partner Center.
