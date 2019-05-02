---
title: Grundlegendes zu den Abrechnungsarten im Partner Center | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Information zu unterschiedlichen Abrechnungsarten, Abrechnungszeiträumen und Abrechnungsdaten
author: MaggiePucciEvans
ms.author: evansma
keywords: Abrechnung, Zahlungen, Bestellungen, Kontenabstimmungsdateien, Kontenabstimmungsdatei
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 4b2b42c0d9bbb2654bbd486f987e3d5da9c562a2
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135380"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Grundlegendes zu Abrechnungsarten in Partner Center

**Gilt für**

-  Partner Center
-  Partner im CSP-Programm

Je nach den Typen der Produkte, die Sie für Ihre Kunden erwerben, gibt es möglicherweise unterschiedliche Abrechnungszeiträume, die an verschiedenen Tagen desselben Monats in Rechnung gestellt werden. In diesem Artikel wird erläutert, was sich ab dem 1. März 2019 geändert hat und wie sich die Änderungen auf Sie auswirken werden.

## <a name="billing-for-recurring-charges"></a>Abrechnung für wiederkehrende Gebühren

Das Abrechnungssystem für wiederkehrende Gebühren von lizenzbasierten und nutzungsbasierten Abonnements ändert sich nicht. Wir werden Ihnen weiterhin eine Rechnung an dem Tag des Monats stellen, den Sie als Ihr Abrechnungsdatum ausgewählt haben, und Ihr Abrechnungszeitraum bleibt weiterhin der Monat vor diesem Datum. Wenn Sie den 15. Tag des Monats als Ihr Abrechnungsdatum ausgewählt haben, werden wir Ihnen sämtliche Aktivitäten ab dem 15. eines Kalendermonats bis zum 14. des nächsten Kalendermonats in Rechnung stellen. Rechnungen und Kontenabstimmungsdateien stehen in der Regel 2–4 Tage nach Ihrem Abrechnungsdatum zur Verfügung.

Wie zuvor werden wir Ihnen diese Produkte in der Währung für das Land/die Region, in dem/der Sie sich befinden, in Rechnung stellen – unabhängig vom Standort des Kunden, an den Sie das Produkt verkauft haben.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Abrechnung für einmalige und ausgewählte wiederkehrende Gebühren

Ab dem 1. März 2019 haben wir ein neues Abrechnungssystem für wiederkehrende und einmalige Gebühren bei Produkten von Microsoft und Drittanbieter-ISVs eingeführt.

Bei diesen Produkten beginnt der Abrechnungszeitraum am 1. Tag des Kalendermonats, und er endet am letzten Tag des Kalendermonats. Wir werden Ihre Rechnung am 8. Tag des Folgemonats zur Verfügung stellen. 

Anders ausgedrückt: Alle Transaktionen, die Sie zwischen dem 1. Mai und dem 31. Mai 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juni angezeigt. Alle Transaktionen, die Sie zwischen dem 1. Juni und dem 30. Juni 2019 tätigen, werden auf Ihrer Rechnung vom 8. Juli angezeigt. Möglicherweise werden wiederkehrende und einmalige Käufe in derselben Monatsrechnung abgerechnet. 

Sie können auch jederzeit Ihren Kontostand/Ihre Rechnung überprüfen (z.B. zwischen dem 1. Mai und dem 7. Juni) und die neueste Kontoaktivität sehen, ohne auf die Monatsrechnung warten zu müssen. Beachten Sie bitte Folgendes: Wenn wir Ihre Rechnung am 8. bereitstellen, enthält sie Steuern sowie alle anderen anwendbaren Gebühren und Guthaben. Deshalb kann der endgültige Betrag von demjenigen abweichen, der Ihnen während des Abrechnungszeitraums angezeigt wird. 

Sie werden auf Ihre Rechnungen genauso wie jetzt zugreifen – entweder im Partner Center oder über API. Die Rechnungen werden am 8. Tag des Monats vor Mitternacht UTC angezeigt. 

|**Abrechnungssystem**|**Produkttyp(en)**|**Abrechnungsdatum**|**Abrechnungszeitraum**|**Abrechnungswährung**|**Aktuelle Aktivität anzeigen?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Wiederkehrende Gebühren für lizenzbasierte und nutzungsbasierte Abonnements |Alle Produkte aus dem [Katalog der Onlinedienste](https://partner.microsoft.com/commerce/preferredoffers/list). Beispiele hierfür sind Office 365, Microsoft 365, Azure Active Directory, Azure (nutzungsbasierte Bezahlung), Dynamics 365, Power BI Pro |Das Datum, das Sie bei der Erstellung Ihres Partner Center-Kontos ausgewählt haben |Der Monat vor Ihrem Abrechnungsdatum. |Die Währung des Landes/der Region, in dem/der Sie sich befinden. Wenn sich Ihr Unternehmen beispielsweise in Großbritannien befindet, werden wir die Rechnung in Britische Pfund (GBP) stellen. Befindet sich Ihr Unternehmen in Indien, erhalten Sie eine Rechnung in Indische Rupien (INR).  |Nein |
|Wiederkehrende und einmalige Gebühren für Produkte von Microsoft und Drittanbieter-ISVs |Alle SaaS-Abonnements, Azure-Reservierungen und Softwareprodukte (unbefristet und abonnementbasiert), die von Microsoft und Drittanbieter-ISVs angeboten werden. Sehen Sie dazu verfügbare Produkte im [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Beispiele hierfür sind SUSE Linux-Software (Softwareabonnement), Windows Server 2019 Essentials (unbefristete Software), Azure ISV-SaaS-Produktabonnement. |Der 8. Tag jedes Monats |Vom ersten Tag bis zum letzten Tag jedes Kalendermonats |Die Währung des Landes/der Region, in dem/der sich Ihr Kunde befindet. Dies bedeutet: Sie erhalten getrennte Rechnungen und Kontenabstimmungsdateien in der Währung für das Land/die Region jedes Kunden, an den Sie im Abrechnungszeitraum verkauft haben. |Ja |
