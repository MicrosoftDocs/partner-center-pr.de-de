---
title: Grundlegendes zu den Typen der Abrechnung im Partner Center | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Informationen zu anderen Typen Abrechnung Abrechnungszeiträume und Abrechnung Datumsangaben
author: MaggiePucciEvans
ms.author: evansma
keywords: Rechnungen, Zahlungen, Bestellungen, abstimmungsdateien und Abstimm.
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

Je nach Art der Produkte, die Sie für Ihre Kunden erwerben, müssen Sie möglicherweise die verschiedenen Abrechnungszeiträume und an verschiedenen Tagen des gleichen Monats in Rechnung gestellt werden. Dieser Artikel beschreibt die Änderungen an der ab dem 1. März 2019 und wie sich Änderungen auswirken werden.

## <a name="billing-for-recurring-charges"></a>Die Abrechnung für laufende Gebühren

Das Abrechnungssystem für laufende Gebühren Lizenz- und nutzungsbasierte Abonnements nicht geändert. Wir werden weiterhin Sie am Tag des Monats in Rechnung, die Sie als Ihre Rechnungsdatum ausgewählt, und des Abrechnungszeitraums des Monats vor diesem Datum werden weiterhin. Wenn Sie den 15. Tag des Monats für Ihre Abrechnung Datum ausgewählt haben, werden Sie für alle Aktivitäten in einem Kalendermonat 15. diesen auf dem 14. des nächsten Kalendermonats berechnet. Rechnungen und kontenabstimmungsdateien sind allgemein verfügbar 2 – 4 Tage nach Ablauf des mit dem.

Wie zuvor, Sie für diese Produkte in der Währung für das Land bzw. die Region, die, denen Sie abgerechnet werden in wohnen, verkauft Sie unabhängig davon, wo der Kunde das Produkt.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Die Abrechnung für einmalige, und wählen eine laufende Gebühren

Ab dem 1. März 2019 vorgestellt ein neues Abrechnungssystem für wiederkehrende und einmaligen Gebühren für Microsoft und ISV-Produkte von Drittanbietern.

Für diese Produkte des Rechnungszeitraums aufaddiert am ersten Tag des Monats beginnt und endet am letzten Tag des Kalendermonats. Wir werden Ihre Rechnung am 8. Tag des Folgemonats zur Verfügung stellen. 

Das heißt, erscheint alle Transaktionen, die Sie zwischen dem 1. Mai und 31 Mai 2019 treffen in Ihrer Rechnung Juni 8. Alle Transaktionen, die Sie, zwischen dem 1. Juni und 30 Juni 2019 vornehmen werden auf Ihrer Rechnung 8. Juli angezeigt. Sie können wiederkehrende oder einmalig Käufe in der Rechnung in Rechnung gestellt. 

Sie können auch Ihre Konto-Balance/Rechnung überprüfen, wann immer Sie (z. B. zwischen 1. Mai und Juni 7 möchten), und sehen die neueste Kontoaktivität ohne zu warten, bis die Rechnung. Beachten Sie, dass wenn wir Ihre Rechnung für den 8. veröffentlichen, es wird steuern und alle anderen entsprechenden Kosten und -Guthaben, damit die endgültige Menge für die Anzeige während des Abrechnungszeitraums unterscheiden kann. 

Sie werden Ihre Rechnungen genauso zugreifen, die Sie nun entweder im Partner Center oder API verwenden. Sie werden vor Mitternacht UTC am 8. Tag des Monats angezeigt. 

|**Abrechnungsumgebung**|**Produkt-Typen**|**Abrechnungsdatum**|**Abrechnungszeitraum**|**Rechnungswährung**|**Aktuelle Aktivität zur Verfügung?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Laufende Gebühren für Lizenz- und nutzungsbasierte Abonnements |Alle Produkte aus der [online Services-Katalog](https://partner.microsoft.com/commerce/preferredoffers/list). Beispiele hierfür sind Office 365, Microsoft 365, Azure Active Directory, Azure (nutzungsbasierte Bezahlung), Dynamics 365, Power BI Pro |Das Datum an, das Sie ausgewählt, bei der Erstellung von Ihrem Partner Center-Konto |Der Monat vor Ablauf des mit dem. |Die Währung des Landes bzw. der Region, die, dem Sie in wohnen. Wenn Ihr Unternehmen im Vereinigten Königreich befindet, werden wir Sie z. B. in britischen Pfund (GBP) rechnen. Wenn Ihr Unternehmen in Indien befindet, müssen Sie in Indien Rupie (INR) abgerechnet.  |Nein |
|Wiederkehrende und einmaligen Gebühren für Microsoft und Drittanbieter-ISV-Produkte |Alle SaaS-Abonnements, Azure-Reservierungen und (fortwährende und abonnementbasierte) Softwareprodukte von Microsoft und Drittanbietern bereitgestellt. Finden Sie unter verfügbaren Produkte für die [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Beispiele für SUSE Linux-Software (Softwareabonnement), Windows Server 2019 Essentials (fortwährende Software), Azure ISV-SaaS-Produkt-Abonnement. |Die 8. Tag jedes Monats |Vom ersten Tag bis zum letzten Tag eines jeden Kalendermonats |Die Währung des Landes bzw. der Region, in dem sich der Kunde befindet. Dies bedeutet, dass Sie separate Rechnungen und kontenabstimmungsdateien in die Währung des Landes bzw. der Region jeder Kunde erhalten werden, die Sie auf den Abrechnungszeitraum verkauft. |Ja |
