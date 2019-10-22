---
title: 'Azure-Plan: Abrechnung | Partner Center'
ms.topic: article
ms.date: 10/04/2019
description: Beschreibt die Dateistruktur für Rechnungen und Abstimmungen
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171302"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung 

Abrechnungen im Rahmen eines Azure-Plans bieten ein vereinfachtes Abrechnungsverfahren, das ein einheitliches Abrechnungsdatum und einen Abrechnungszeitraum auf der Grundlage von Kalendermonaten verwendet. Informationen zur Abrechnungsplattform finden Sie unter [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (Partner Center Modern Commerce – Betriebshandbuch).

## <a name="summary-of-billing-essentials"></a>Zusammenfassung der Abrechnungsgrundlagen

- **Rechnungsdatum**: Die Rechnungs- und Abstimmungsdatei steht auf dem Partner Center-Dashboard bzw. über die -API am 8. des Monats zur Verfügung (Mitternacht UTC).

- **Abrechnungszeitraum der Rechnung**: Der Abrechnungszeitraum der Rechnung ist am Kalendermonat ausgerichtet, z.B. 01.10.–31.10., 01.11.–30.11.

- **Belastung von Dienstzeiträumen**: Die Gebühren richten sich nach dem Kalendermonat. Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10. Die Rechnung des nächsten Monats, die am 08.12. generiert wird, enthält alle Gebühren für den Dienstzeitraum vom 01.11.–30.11.

- **Fälligkeit der Rechnung**: 60 Tage netto.

- **Rechnungswährung** : Partner werden weiterhin in der offiziellen Landeswährung des Kunden abgerechnet. Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.

- **Partnerincentives**: 45 Tage nach dem Ende des Rechnungsmonats bezahlt.

##  <a name="access-your-invoices-and-recon-files"></a>Zugriff auf Ihre Rechnungen und Abstimmungsdateien

Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist. 

**Zugriff auf die Rechnung und Abstimmungsdatei**

1. Melden Sie sich bei Partner Center an.

2. Wählen Sie im Menü des Partner Center **Abrechnung** aus.

3. Wählen Sie die Registerkarte für die **kalenderbasierte** Abrechnung und die Sie interessierende Währung aus.

![Abrechnung](images/azure/billing1.png)

4. Wählen Sie **Rechnung und Abstimmungsdatei** aus.  

Zum Anzeigen früherer Rechnungen und Abstimmungsdateien erweitern Sie die Zeile „Abrechnungsverlauf“ unten.

## <a name="read-the-invoice"></a>Lesen der Rechnung

1. Die Rechnung steht spätestens am 8. jedes Monats zur Verfügung.

2. Partner haben 60 Tage Zeit, die Zahlung zu überweisen.

3. Der Abrechnungszeitraum deckt einen bestimmten Kalendermonat ab, beispielsweise 01.10–31.10.

4. Gebühren werden ohne Wertberichtigungen angezeigt (Betrag ohne Anrechnung von „Partner earned credit for services managed“).

5. Weitere Abrechnungsdetails können Sie der Abstimmungsdatei zur Rechnung und der täglich ausgewerteten Nutzungsdatei entnehmen.

![Rechnung](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a>Lesen der Abstimmungsdatei

1. Jede Verbrauchseinheit von Azure-Abonnements kann bis zu zwei Abrechnungszeilen in der Abstimmungsdatei aufweisen.

2. Wenn die Verbrauchseinheit während des gesamten Kalendermonats zu Rabatten oder Gutschriften berechtigt (etwa die Rabatte in Schicht 1 oder die „Partner earned credit for managed services“), enthält die Abstimmungsdatei nur eine Abrechnungszeile. Die Spalte **PriceAdjusmentDescription** weist den Rabatt oder die erworbene Gutschrift aus; der effektive Preis pro Einheit ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift oder anderer Rabatte.

3. Wenn die Verbrauchseinheit während des gesamten Kalendermonats nicht zu Gutschriften für die „Partner earned credit for managed services“ berechtigt war, enthält die Abstimmungsdatei nur eine Abrechnungszeile, und der effektive Einzelpreis stimmt mit dem Endkundenpreis (bei dem es sich um den Einzelpreis handelt) überein.

4. Wenn die Verbrauchseinheit während eines Teils des Monats für **Partner earned credit for services managed** berechtigt war, enthält die Abstimmungsdatei zwei Abrechnungszeilen. Eine Zeile stellt die Tage dar, an denen eine Berechtigung der Verbrauchseinheit bestand, die andere die Tage, an denen diese Berechtigung nicht bestand. 

## <a name="read-the-daily-usage-file"></a>Lesen der täglichen Nutzungsdatei

- Verbrauchseinheiten von Abonnements im Rahmen eines Azure-Plans werden täglich bewertet und kumuliert. 

- **Partner earned credit for services managed** wird auf täglicher Grundlage bestimmt und angewendet.

- Jede Verbrauchseinheit für Abonnements weist eine Zeile für jeden Tag des Monats auf, an dem ein Verbrauch angefallen ist.

- Bezogen auf das Beispiel unten:

  - Die Verbrauchseinheit ist vom 01.07–03.07. für **Partner earned credit for services managed** qualifiziert (beachten Sie, dass der effektive Einzelpreis sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift ergibt).

   - Die Verbrauchseinheit ist vom 04.07–07.07. nicht für **Partner earned credit for services managed** qualifiziert (beachten Sie, dass der effektive Einzelpreis mit dem Endkundenpreis übereinstimmt).

    - Die Verbrauchseinheit ist vom 08.07–31.07. für **Partner earned credit for services managed** qualifiziert (beachten Sie, dass der effektive Einzelpreis sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift ergibt).

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a>Rechnung in Währung des Kunden 

Im Rahmen eines Azure-Plans erbrachte Azure-Dienste haben Preise in USD und werden in der Landeswährung des Kunden abgerechnet. Wenn die Abrechnungswährung nicht USD ist, wird der zugrunde gelegte Wechselkurs auf der letzten Seite der Rechnung angezeigt. Wechselkurse werden monatlich bestimmt und auf die folgende Rechnung angewendet. Eine vollständige Liste der Landeswährungen finden Sie in der [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V) (Matrix für die Länderverfügbarkeit neuer E-Commerce-Angebote und Kundenwährungen). 

Microsoft nutzt [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) zum Ermitteln des Wechselkurses, der für die Konvertierung aus der Preiswährung in die Rechnungswährung verwendet wird. Der Wechselkurs wird aktualisiert und steht am Tag vor dem Ersten des Monats zur Verfügung, für den er gilt.

**Beispiel**:  Nutzungsgebühren für den Dienstzeitraum vom 1. August–31. August unter Verwendung des am 1. August veröffentlichten Wechselkurses. Diese Gebühren werden auf der September-Rechnung aufgeführt, und der Wechselkurs ist auf der letzten Seite der Rechnung vermerkt. 

Benutzer von Partnermandanten sehen auch weiterhin rollenspezifische Informationen zu allen Kunden und Bestellungen, unabhängig von der Rechnungswährung. Darüber hinaus kann der Benutzer alle Rechnungen in allen Währungen anzeigen.  
 
## <a name="azure-reservations"></a>Azure Reservations 

Wenn Sie [Azure-Reservierungen](https://docs.microsoft.com/partner-center/azure-reservations) im Rahmen eines Azure-Plans erwerben, ist im Partner Center anfänglich nur die Auswahl der einmaligen Abrechnung möglich. Die monatliche Abrechnung steht im Azure-Portal zur Verfügung. Die monatliche Abrechnung ist im Partner Center zu einem späteren Termin verfügbar. 

## <a name="azure-cost-management"></a>Azure-Kostenmanagement 

Mithilfe der Azure-Tools für Kostenmanagement können Organisationen Kosten überall in Microsoft Azure visualisieren, verwalten und optimieren. Diese Funktion soll im Azure-Portal verfügbar sein. Partner verfügen über eine Always-On-Lösung mit geringer Latenz, die folgende Features unterstützt: 

- Umfangreichere Analyse- und Budgetwarnungen 
- APIs und Power BI-Connectors 
- Ansicht für mehrere Kunden 
- Kostenlose Verwaltung von Azure-Kosten 
- Erweiterung von Rollen/Benutzern 

Weitere Informationen zu diesem Feature, das für Enterprise-Verträge seit Februar 2019 verfügbar ist, finden Sie unter [Azure-Kostenmanagement](https://azure.microsoft.com/services/cost-management). Es steht nur für Azure-Dienste zur Verfügung, die im Rahmen dieser neuen Azure-E-Commerce-Benutzeroberfläche in CSP erworben wurden. 
 
## <a name="azure-spending"></a>Azure-Ausgaben 

Ein Azure-Ausgabentool soll im Partner Center für die neue E-Commerce-Benutzeroberfläche in CSP zur Verfügung stehen. Wenn es angewendet wird, können Partner mit dieser Funktion Folgendes anzeigen:  

- Das Gesamtbudget für einen Kunden 
- Geschätzte Gesamtausgaben für einen vorhandenen Azure-Plan 
- Prozentsatz der Nutzung durch den Kunden in jedem Abrechnungszeitraum 

Da das Abrechnungsmodell für Azure-Dienste im Rahmen eines Azure-Plans die Nutzung nach Vorkasse vorsieht, können Partner zum Vermeiden einer höher als erwarteten Rechnung ein monatliches Budget zuweisen und den Prozentsatz seiner Nutzung nachverfolgen. Ein Budget kann auf einen Kunden oder auf mehrere Kunden zugleich angewendet werden. 

![Azure-Ausgaben](images/azure/azurespend.png)

**Weitere Informationen**

-  How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard (Art der Berechnung der vom Partner erworbenen Gutschriften (PEC) und ihre Position in der Preisliste, die auf dem Partner Center-Dashboard verfügbar ist). 
   
-  [Erwerb des Azure-Plans](purchase-azure-plan.md)

-  [Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP ](azure-plan-price-list.md)
