---
title: Verständnis der Abrechnung im Partner Center | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Informationen zu anderen Typen Abrechnung, Abrechnung Punkte und Abrechnung Datumsangaben
author: labrenne
ms.author: labrenne
keywords: Abrechnung, Zahlungen, Aufträge, abstimmungsdateien, abstimmungsdatei
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 777a98f8780eb036b4bac99eca9a5621d61da66b
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122304"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Verständnis der Abrechnung im Partner Center

**Betrifft:**

-  Partner Center
-  Partner im CSP-Programm

Je nach den Arten von Produkten, die Sie für Ihre Kunden erworben werden soll, müssen Sie möglicherweise verschiedene Abrechnung arbeiten und an unterschiedlichen Tagen des gleichen Monats in Rechnung gestellt. In diesem Artikel wird erläutert, was ab dem 1. März 2019 geändert wird und wie die Änderungen Sie auswirkt.

## <a name="billing-for-recurring-charges"></a>Abrechnung für laufende Gebühren

Die Abrechnung Erfahrung für laufende Gebühren lizenzbasierten und nutzungsbasierten Abonnements wird nicht geändert. Wir weiterhin Sie am Tag des Monats in Rechnung, die Sie als Ihr Abrechnungsdatum ausgewählt haben, und Ihre Abrechnungsperiode weiterhin den Monat vor diesem Datum. Wenn Sie bis zum 15. Tag des Monats für Ihr Abrechnungsdatum ausgewählt haben, werden Sie für alle Aktivität aus der 15. einer Monatsansicht des Kalenders die 14. des nächsten Monats in Rechnung gestellt. Rechnungen und abgleichungsdateien sind 2 bis 4 Tage nach Ihrem Abrechnungsdatum in der Regel verfügbar.

Wie vor, wir Sie für diese Produkte in der Währung für das Land/die Region in Rechnung, die, denen Sie gestellt werden in ausfindig gemacht haben, verkauft Sie unabhängig von den Speicherort des Kunden das Produkt.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Abrechnung für einmalige und wählen Sie eine laufende Gebühren

Ab dem 1. März 2019 vorgestellt eine neue Abrechnung Funktion für wiederkehrende und einmaligen Gebühren für Microsoft und Drittanbieter-ISV-Produkte.

Für diese Produkte der Abrechnungszeitraum am ersten Tag des Monats beginnt und endet am letzten Tag des Monats. Wir werden Ihre Rechnung am 8. Tag des Folgemonats zur Verfügung stellen. 

Anders ausgedrückt, werden alle Transaktionen, die Sie zwischen dem 1. Mai und 31 Mai 2019 vornehmen zu Ihrer Rechnung 8. Juni angezeigt. Alle Transaktionen, die Sie zwischen dem 1. Juni und 30 Juni 2019 vornehmen auf Ihrer Rechnung 8. Juli angezeigt. Sie können für wiederkehrende und einmalige Einkäufe in der Rechnung in Rechnung gestellt abrufen. 

Sie können auch Ihre Konto Saldo/Rechnung überprüfen, wenn Sie (z. B. zwischen Mai 1 bis 7. Juni möchten) und finden Sie unter den neuesten Kontoaktivitäten ohne zu warten, bis der Rechnung. Beachten Sie, dass wenn wir Ihre Rechnung auf der 8. bereitzustellen, es wird steuern und andere anwendbar Gebühren und Guthaben, der endgültige Betrag unterscheiden sich möglicherweise während des Abrechnungszeitraums angezeigt. 

Sie müssen Ihre Rechnungen die gleiche Weise zugreifen, die Sie jetzt im Partner Center oder durch API ausführen. Er vor Mitternacht UTC am 8. Tag des Monats angezeigt. 

|**Abrechnung Erfahrung**|**Produkt-Typen**|**Abrechnungsdatum**|**Abrechnungszeitraum**|**Währung der Abrechnung**|**Aktuelle Aktivität verfügbar?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Laufende Gebühren für lizenzbasierte und nutzungsbasierte Abonnements |Alle Produkte aus dem [Katalog online-Dienste](https://partner.microsoft.com/commerce/preferredoffers/list). Beispiele für Office 365, Microsoft 365, Azure Active Directory, Azure (nutzungsbasierte), Dynamics 365, PowerBI Pro |Das Datum, die, das Sie ausgewählt, wenn Sie Ihr Partner Center-Konto erstellt |Der Monat vor Ihrem Abrechnungsdatum. |Die Währung des Landes/der Region, die Sie in gefunden werden. Beispielsweise, wenn Ihr Unternehmen in Großbritannien befindet, werden wir Sie Britisches Pfund (GBP) in Rechnung. Wenn Ihr Unternehmen in Indien befindet, werden wir Sie in Indien Rupie (INR) in Rechnung stellen.  |Nein |
|Wiederkehrende und einmaligen Gebühren für Microsoft und Drittanbieter-ISVs Produkte |Alle SaaS-Abonnements, Azure Reservations und Software (unbefristeten und abonnementbasierten) Produkte von Microsoft und Drittanbietern ISVs angeboten. Finden Sie unter Verfügbare Produkte im [Markt](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Beispiele umfassen SUSE Linux-Software (Softwareabonnement), Windows Server 2019 Essentials (unbefristeten Software), Azure ISV SaaS-Produkt-Abonnement. |Am 8. Tag des Monats |Vom ersten Tag in den letzten Tag des Monats Kalender |Die Währung des Landes/der Region befindet sich in der Kunden. Dies bedeutet, dass Sie verschiedene Rechnungen und abgleichungsdateien in der Währung des Landes/der Region einzelnen Kunden erhalten, die Sie in den Abrechnungszeitraum zum verkauft. |Ja |
