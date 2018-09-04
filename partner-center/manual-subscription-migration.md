---
title: Migrieren von Dynamics AX-Abonnements zu Dynamics365 | Partner Center
description: Microsoft führt Dynamics365 ein, die nächste Generation intelligenter Unternehmensanwendungen, mit denen Ihre Organisation wachsen, sich entwickeln und transformiert werden kann, um die Anforderungen Ihrer Kunden zu erfüllen und neue Geschäftschancen zu nutzen.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 8a8aaf2591b6a67114da7d2226dde7bf94dd06b0
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876300"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrieren von Dynamics AX-Abonnements zu Dynamics 365

**Betrifft**

-  Partner Center

Microsoft führt Dynamics365 ein, die nächste Generation intelligenter Unternehmensanwendungen, mit denen Ihre Organisation wachsen, sich entwickeln und transformiert werden kann, um die Anforderungen Ihrer Kunden zu erfüllen und neue Geschäftschancen zu nutzen. Im Rahmen des neuen Produkts führt Microsoft am 1.November2016 neue Microsoft Dynamics-Abonnementpläne für Kunden ein, die den aktuellen Plänen zwar ähnlich, jedoch nicht mit diesen identisch sind.

Die Anweisungen in diesem Dokument beschrieben, wie indirekte Anbieter vorhandene Microsoft Dynamics AX- und Microsoft Dymanics CRM Online-Abonnements von Kunden zum neuen Microsoft Dynamics365 migrieren können. Die Anweisungen gelten auch für andere Microsoft-Produkte, die auf neue Versionen aktualisiert werden, sodass Anbieter Kundenabonnements zu einer neuen SKU migrieren müssen.

Die Microsoft Dynamics CRM Online und AX-Pläne werden deaktiviert.  Ab dem 1.Juli2017 können die älteren Pläne nicht mehr verlängert werden. Auch bestehende E4-Abonnements werden nicht automatisch verlängert.

Wenn CRM Online und AX-Abonnements enden, werden sie storniert. Um Kontinuität für Kunden zu gewährleisten, sollten Sie Kunden mit ablaufenden Abonnements auf eine unterstützte SKU-Option (nachfolgend aufgeführt) übertragen. Um Serviceausfälle für Kunden zu vermeiden, empfehlen wir, die Kunden zu veranlassen, vor dem jährlichen Abonnementende neue Abonnements abzuschließen. 

Auf der Detailseite des Abonnements wurde der Abonnementstatus von „Datum der automatischen Verlängerung: [Datum]“ in „Gültig bis [Datum]“ geändert. 

Wenn Sie die API (CREST oder Partner Center) verwenden, können Sie ablaufende Abonnements durch Auswerten des Enddatums des Abonnements sowie der Eigenschaft „False“ für die automatische Verlängerung ermitteln. Die Abonnements wurden für den 1. Juli 2017 auf „renew=False“ gesetzt. Sie können Kunden zu einem beliebigen Zeitpunkt in einen neuen Plan verschieben. 

**Änderungen für die Microsoft Dynamics AX-Lizenzierung**

Die Microsoft Dynamics AX-Produktlinie wird mit Wirkung vom 1.November2016 eingestellt. Weitere Informationen zu den neuen Lizenzierungsoptionen für Dynamics365 finden Sie im [Lizenzierungshandbuch](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf), das in Kürze veröffentlicht wird.

 Die folgende Tabelle enthält Details zur Lizenzzuordnung:

|**Veraltete SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Microsoft Dynamics 365 for Unified Operations oder Microsoft Dynamics 365 Plan |
|Aufgabe|Microsoft Dynamics 365 for Sales
|Aufgabe/Self-Service|Microsoft Dynamics 365 for Team Members|
|Gerät|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Microsoft Dynamics CRM Online-Lizenzierungsänderungen 

**Microsoft Dynamics CRM Online**

Der aktuelle Microsoft Dynamics CRM Online-Plan wird mit Wirkung vom 1.November2016 eingestellt. Weitere Informationen zu den neuen Lizenzierungsoptionen für Microsoft Dynamics365 finden Sie im [Lizenzierungshandbuch](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Weitere Informationen zu neuen Lizenzierungsoptionen finden Sie unter [Wichtige Informationen für CRM Online-Kunden](https://go.microsoft.com/fwlink/?linkid=831667).

Die folgende Tabelle enthält Details zur Lizenzzuordnung:

|**Veraltete SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Dynamics 365 Enterprise Customer Engagement Plan |
|Professional|Dynamics 365 Enterprise Customer Engagement Plan, Dynamics 365 for Sales oder Dynamics 365 for Customer Service|
|Basic|Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service oder Dynamics 365 Enterprise Customer Engagement Plan|
|Unentbehrlich|Dynamics 365 for Team Member|
|Field Service-Add-On|Dynamics 365 Enterprise Customer Engagement Plan oder Dynamics 365 for Field Service|
|Projekt Service Authomation-Add-On|Dynamics 365 Customer Engagement Plan oder Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Migrieren von Kunden zu neuen Produktplänen


Microsoft bietet Wiederverkäufern und Anbietern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Wiederverkäufer Kunden möglicherweise auf neue Dienste aktualisieren oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden von alten SKUs auf neuere SKUs muss in dieser Reihenfolge erfolgen:

-   [Kauf des neuen Abonnements](#manual-subscription-migration-purchasenewsubsc);
-   [Neuzuweisen der aktuellen Benutzerlizenzen](#manual-subscription-migration-reassignlicenses);
-   [Stornieren des alten Abonnements](#manual-subscription-migration-cancelsubscriptions).

Mit den folgenden Verfahren migrieren Sie einen Kunden von Microsoft Dynamics AX oder CRM Online zu Dynamics365.

Der Wiederverkäufer muss einen Kunden mit einem vorhandenen Dynamics AX Enterprise-Abonnement zu Dynamics365 for Operations migrieren. Der erste Schritt besteht im Kauf von Dynamics365 for Operations.  Wiederholen Sie diese Schrittefür einen CRM Online-Kunden zum Wechsel zu Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Kauf des neuen Abonnements**

1.  Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend **Abonnements hinzufügen** aus.
2.  Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall Dynamics365 for Operations Enterprise Edition), kaufen Sie die nötigen Anzahl von Lizenzen, und wählen Sie **Übermitteln** aus.

    Ihr Kunde sollte nun alte und neue Abonnements besitzen. In diesem Beispiel sind dies das alte Dynamics AX Enterprise-Abonnement und das neue Abonnement von Dynamics365 for Operations Enterprise Edition.

<a href="" id="reassignlicenses"></a> Im nächsten Schritt werden alle vorhandenen Benutzerlizenzen dem neuen Abonnement neu zugewiesen.

**Neuzuweisen von Benutzerlizenzen**

1.  Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend **Benutzer und Lizenzen** aus. Die Seite mit Benutzern und Lizenzen des Kunden wird geöffnet.
2.  Um Benutzerlizenzen neu zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen**.
3.  Deaktivieren Sie auf der Seite **Verwalten von Lizenzen** das Kontrollkästchen für die Lizenz **Dynamics AX Enterprise**, und wählen Sie die Lizenz **Dynamics365 for Operations** aus.
4.  Wählen Sie **Übermitteln** aus. Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.
5.  Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.

<a href="" id="cancelsubscriptions"></a> Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das alte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

**Stornieren des alten Abonnements.**

1.  Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend das Abonnement aus, das Sie stornieren möchten.
2.  Legen Sie auf der Seite für Abonnementdetails **Status** auf **Ausgesetzt** fest.
3.  Wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.

## <a name="additional-considerations"></a>Weitere Aspekte


Wenn Kunden vom Open-Programm zum Programm für Cloud-Lösungsanbieter wechseln, um weitere Abonnements bereitzustellen, müssen Sie die vorhandenen Abonnements ebenfalls migrieren:

-   Wenn Kunden das alte Abonnement über das Open-Programm erhalten haben, ist die Migration zum CSP-Programm für die neue SKU einfach.
-   Wenn Kunden noch nicht als Ihre Kunden eingerichtet sind, können Sie diese einladen. Weitere Informationen finden Sie im Hilfethema [Anfordern einer Beziehung zu einem Kunden](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Nachdem der Kunde Sie als indirekten Anbieter akzeptiert hat, sind die Bereitstellungsschritte größtenteils mit den oben beschriebenen Schritten identisch: Sie kaufen das neue Abonnement und weisen die Benutzerlizenzen zu. Der einzige Unterschied besteht in der Stornierung des/der alten Abonnements. Ein neuer Anbieter kann keine Abonnements aussetzen/stornieren, die über andere Kanäle gekauft wurden. Wenn ein Kunde zuvor Abonnements über einen anderen Vertriebskanal gekauft hat, beispielsweise Open, muss der Kunde die Abonnements selbst über diesen Kanal stornieren.

 

 



