---
title: 'Azure-Plan: Abrechnung – Rechnungs- und Kontenabstimmungsdateien'
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie auf die Struktur der Rechnungs-/Abstimmungsdatei im Zusammenhang mit der Abrechnung für den Azure-Plan zugreifen und sie verstehen können.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f0246338ef8c0da06dce557573cd2811d07a0e9e
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908360"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung 

**Geeignete Rollen:**

- Administrator-Agent
- Abrechnungsadministrator
- Globaler Administrator

Abrechnungen im Rahmen eines Azure-Plans bieten ein vereinfachtes Abrechnungsverfahren, das ein einheitliches Abrechnungsdatum und einen Abrechnungszeitraum auf der Grundlage von Kalendermonaten verwendet.

## <a name="summary-of-billing-essentials"></a>Zusammenfassung der Abrechnungsgrundlagen

- **Rechnungsdatum**: Die Rechnungs- und Abstimmungsdatei steht auf dem Partner Center-Dashboard bzw. über die -API am 8. des Monats zur Verfügung (Mitternacht UTC).

- **Abrechnungszeitraum der Rechnung**: Der Abrechnungszeitraum der Rechnung ist am Kalendermonat ausgerichtet, z.B. 01.10.–31.10., 01.11.–30.11.

- **Belastung von Dienstzeiträumen**: Die Gebühren richten sich nach dem Kalendermonat. Wenn ein Abrechnungspartner beispielsweise Azure-Dienste über einen Azure-Plan am 15.10. hinzufügt und der Kunde mit der Nutzung der Azure-Dienste am 15.10 beginnt, erhält der Abrechnungspartner am 08.11. die Rechnung/Abstimmung über den Kundenverbrauch für den Dienstzeitraum von 15.10–31.10. Die Rechnung des nächsten Monats, die am 08.12. generiert wird, enthält alle Gebühren für den Dienstzeitraum vom 01.11.–31.11.

- **Fälligkeit der Rechnung**: 60 Tage netto.

- **Rechnungswährung** : Partner werden weiterhin in der offiziellen Landeswährung des Kunden abgerechnet. Wenn der Abrechnungspartner sich beispielsweise in Irland befindet und Kunden im Vereinigten Königreich, Norwegen und Deutschland bedient, erhält der Abrechnungspartner eine Rechnung/Abstimmung in GBP, NOK und EUR.

- **Partnerincentives**: 45 Tage nach dem Ende des Rechnungsmonats bezahlt.

## <a name="access-your-invoices-and-reconciliation-files"></a>Zugriff auf Ihre Rechnungen und Abstimmungsdateien

Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist. 

**Zugriff auf die Rechnungs- und Abstimmungsdatei**

1. Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/en-us/dashboard/) an.

2. Wählen Sie im Menü des Partner Center **Abrechnung** aus.

3. Wählen Sie die Registerkarte für **laufende** und **einmalige** Gebühren sowie die für Sie relevante Währung aus.

![Abrechnung](images/azure/billing3.png)

4. Wählen Sie **Rechnung** oder **Abstimmungsdatei** aus.  

Zum Anzeigen früherer Rechnungen und Abstimmungsdateien erweitern Sie die Zeile „Abrechnungsverlauf“ unten.


## <a name="understanding-usage-data"></a>Grundlegendes zu Verwendungsdaten 

1. Der Azure-Plan ist der Stammcontainer oder der Container der obersten Ebene für die Verwendung. Alle Verwendungsdaten sind an einen einzelnen Azure-Plan gebunden.

2. Ein Plan kann ein oder mehrere Azure-Abonnements enthalten. Dies sind Container, die für die Ressourcenverwaltung und -bereitstellung verwendet werden. 

3. Innerhalb eines Abonnements werden Ressourcengruppen zu Gruppenressourcen hinzugefügt. Jede Ressource wird in einer Ressourcengruppe bereitgestellt. 

4. Beispiele für Ressourcen sind virtuelle Computer und Speicherkonten. 

5. Ressourcen geben Verbrauchszähler aus: Verbrauchszähler sind Verbrauchsmessungen einer Ressource, und eine Ressource kann Verwendungsdaten für verschiedene Verbrauchszähler ausgeben. Verbrauchszähler werden durch „ProductId“-, „SKUId“- und „AvailabilityId“-Werte identifiziert. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchie von Abonnementressourcengruppen und -messungen

**Azure-Konto (Mandant)**

- Abonnement A
    - ResourceGroup 1
        - Virtueller Computer (Ressource)
            - Computeverbrauchseinheit
        - Virtuelles Netzwerk (Ressource)
            - Keine Abrechnungsverbrauchseinheit

    - ResourceGroup 2
        - Virtueller Computer (Ressource)
            - Computerverbrauchseinheit
        - Verwalteter SSD Premium-Datenträger (Ressource)
            - Verbrauchseinheit für Speicherkapazität
            - Verbrauchseinheit für Speichervorgänge

- Abonnement B   -ResourceGroup 1       - Azure SQL (Ressource)           - DTU-Verbrauchseinheit       - VPN Gateway (Ressource)           - Verbrauchseinheit für VPN-Gateway

    - ResourceGroup 2
        - Virtuelle Netzwerkschnittstelle (Ressource)
            - Keine Abrechnungsverbrauchseinheit

## <a name="read-the-invoice"></a>Lesen der Rechnung

1. Die Rechnung steht spätestens am 8. jedes Monats zur Verfügung.

2. Partner haben 60 Tage Zeit, die Zahlung zu überweisen.

3. Der Abrechnungszeitraum deckt einen bestimmten Kalendermonat ab, beispielsweise 01.10–31.10.

4. Gebühren werden ohne Wertberichtigungen angezeigt (Betrag ohne Anrechnung von „vom Partner erworbene Gutschrift für verwaltete Dienste“).

5. Weitere Abrechnungsdetails können Sie der Abstimmungsdatei zur Rechnung und der täglich ausgewerteten Nutzungsdatei entnehmen.

![Rechnung](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a>Lesen der Rechnungs-/Abstimmungsdatei

1. Jede Kombination von Azure-Plan und Verbrauchseinheit kann bis zu zwei Abrechnungszeilen in der Abstimmungsdatei aufweisen.

2. Wenn die Verbrauchseinheit während des gesamten Kalendermonats zu Rabatten oder Gutschriften berechtigt – etwa die Rabatte in Schicht 1 oder das vom Partner erworbene Guthaben (PEC) für verwaltete Dienste – enthält die Abstimmungsdatei nur eine Abrechnungszeile. Die Spalte **PriceAdjusmentDescription** verweist auf den Rabatt oder das erworbene Guthaben.

3. Wenn für eine bestimmte Verbrauchseinheit, die zu einem Rabatt oder PEC berechtigt, keine Ressourcen vorliegen, enthält die Abstimmungsdatei nur eine Abrechnungszeile, und der effektive Einzelpreis stimmt mit dem Endkundenpreis (bei dem es sich um den Einzelpreis handelt) überein.

4. Wenn die Verbrauchseinheit oder eine beliebige Ressource, die diese Verbrauchseinheit ausgibt, während eines Teils des Monats für **Vom Partner erworbenes Guthaben für verwaltete Dienste** berechtigt war, enthält die Abstimmungsdatei zwei Abrechnungszeilen. Eine Zeile stellt die Tage dar, an denen eine Berechtigung der Verbrauchseinheit bestand, die andere die Tage, an denen diese Berechtigung nicht bestand. 

## <a name="read-the-daily-usage-file"></a>Lesen der täglichen Nutzungsdatei

- Verbrauchseinheiten von Abonnements im Rahmen eines Azure-Plans werden täglich bewertet und kumuliert. 

- **Partner earned credit for services managed** wird auf täglicher Grundlage bestimmt und angewendet.

- Jede Verbrauchseinheit für Abonnements weist eine Zeile für jeden Tag des Monats auf, an dem ein Verbrauch angefallen ist.

- Bezogen auf das Beispiel unten:

  - Die Verbrauchseinheit ist vom 01.07–3.07. für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift).

   - Die Verbrauchseinheit ist vom 04.07–07.07. nicht für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis stimmt nicht mit dem Endkundenpreis überein).

    - Die Verbrauchseinheit ist vom 08.07–31.07. für **vom Partner erworbene Gutschrift für verwaltete Dienste** qualifiziert (der effektive Einzelpreis ergibt sich aus dem Endkundenpreis abzüglich der vom Partner erworbenen Gutschrift).

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a>Rechnung in Währung des Kunden 

Im Rahmen eines Azure-Plans erbrachte Azure-Dienste haben Preise in USD und werden in der Landeswährung des Kunden abgerechnet. Wenn die Abrechnungswährung nicht USD ist, wird der zugrunde gelegte Wechselkurs auf der letzten Seite der Rechnung angezeigt. Wechselkurse werden monatlich bestimmt und auf die folgende Rechnung angewendet. Eine vollständige Liste der Landeswährungen finden Sie in der [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354) (Matrix für die Länderverfügbarkeit neuer E-Commerce-Angebote und Kundenwährungen). 

Microsoft nutzt [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) zum Ermitteln des Wechselkurses, der für die Konvertierung aus der Preiswährung in die Abrechnungswährung verwendet wird. Die Wechselkurse werden aktualisiert und stehen am Tag vor dem Ersten des Monats zur Verfügung, für den sie gelten.

**Beispiel**:  Nutzungsgebühren für den Dienstzeitraum vom 1. August–31. August unter Verwendung des am 31. Juli veröffentlichten Wechselkurses. Diese Gebühren werden auf der September-Rechnung aufgeführt, und der Wechselkurs ist auf der letzten Seite der Rechnung vermerkt. 

 
## <a name="azure-reservations"></a>Azure Reservations 

Wenn Sie [Azure-Reservierungen](https://docs.microsoft.com/partner-center/azure-reservations) im Rahmen eines Azure-Plans erwerben, ist im Partner Center anfänglich nur die Auswahl der einmaligen Abrechnung möglich. Die monatliche Abrechnung steht im Azure-Portal zur Verfügung. Die monatliche Abrechnung ist im Partner Center zu einem späteren Termin verfügbar. 

## <a name="azure-spending"></a>Azure-Ausgaben 

Die bestehende Azure-Kaufumgebung wird aktualisiert, um die neue Azure-Planabrechnung im Partner Center zu unterstützen. Dadurch wird Partnern Folgendes ermöglicht:

- Anzeigen, Verwalten und Empfangen von Benachrichtigungen für Budgets, die auf Kundenebene festgelegt wurden 

- Anzeigen der geschätzten Gesamtausgaben für einen Azure-Plan (aufgeschlüsselt nach Ressourcen und Verbrauchseinheitswert)

Da die Abrechnungsmodell für Azure-Dienste unter einem Azure-Plan nachträglich nach Verbrauch berechnet wird, können Partner ein monatliches Budget festlegen und den Prozentsatz der Nutzung nachverfolgen, um zu vermeide, dass die Rechnung höher als erwartet ausfällt. Ein Budget kann auf einen Kunden oder auf mehrere Kunden zugleich angewendet werden. 

![Azure-Ausgaben](images/azure/azurespend.png)

**Weitere Informationen**

-  Wie das vom Partner erworbene Guthaben (PEC) berechnet wird, finden Sie in der Preisliste, die auf dem Partner Center-[Dashboard](https://partner.microsoft.com/en-us/dashboard/) verfügbar ist (Anmeldung erforderlich). 
   
-  [Erwerb des Azure-Plans](purchase-azure-plan.md)

-  [Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP ](azure-plan-price-list.md)
