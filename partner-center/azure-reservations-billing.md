---
title: Abrechnung für Azure Reservations | Partner Center
Description: Information about billing for Azure reservations.
author: v-petand
keywords: Azure RI, Azure Reserved Instances, Reservierungen, virtuelle Computer, verwalten, Abrechnung, kaufen
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: 846f2863e9c4dc9967b8c337bcab40f153b99eb6
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489436"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Microsoft Azure Reserved VM Instances – Abrechnung

**Betriff:**

-  Partner Center
-  Microsoft Azure-Portal
-  CSP-Partner

Partner im Cloud Solution Provider-Programm (CSP) können Angebote ihren Kunden reservierte Instanzen auf Microsoft Azure-VMs anbieten. Kunden können virtuelle Maschinen im Voraus reservieren – für ein Jahr oder drei Jahre – und erhebliche Einsparungen bei der Azure-Nutzung erhalten.   

Die Kunden bezahlen im Voraus für Azure Reserved VM Instances. Wenn Sie Azure Reserved VM Instances im Auftrag eines Kunden kaufen, erhalten Sie Rechnungen und Abgleichungsdateien für die einmaligen Gebühren. 

>[!IMPORTANT]
>Wenn Sie Azure Reserved VM Instances für einen Kunden in einem Markt mit einer anderen Währung, als der standardmäßigen Währung erwerben, basiert die Abrechnung auf dem Markt des Kunden, nicht Ihrem Standort. Wenn Sie Kunden in mehreren Märkten haben, erhalten Sie verschiedene Rechnungen und Abgleichungsdateien für jede Währung der Kunden, die in Rechnung gestellt werden, damit Ihre Kunden in der entsprechenden Währung in Rechnung gestellt werden. 

Um auf einmalige Rechnungen und abgleichungsdateien zuzugreifen, wählen Sie aus dem Partner Center **Abrechnung** , und wählen Sie dann **ein Mal**. 

Weitere allgemeine Informationen zur Abrechnung im Cloud Solution Provider-Programm finden Sie unter [Grundlagen zur Abrechnung](billing-basics.md).

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Azure Reserved VM Instance – Definitionen zur Rechnungsdatei

**Allgemeine Rechnungsinformationen**

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|US FEIN |Ihre Steuernummer. |
|Rechnungsempfänger |Verwendete rechtliche Geschäftsadresse für Steuern. Um diese Adresse zu ändern, wechseln Sie zu Einstellungen > Partnerabrechnungsprofil. |
|Gebühren |Gesamtsumme der aktuellen Gebühren. |
|Guthaben |Guthaben für Rückerstattungsaktivität seit dem ersten Kauf. |
|Rabatte |Rabatte, die für Azure Reservations oder andere Elemente in der jeweiligen Kundenbestellung gelten. |
|Steuern |Die gesamten Steuern für die aktuellen Gebühren, wie im Abschnitt „Details“ auf Seite 2 der Rechnung summiert. |
|Aktuelle Gebühren insgesamt |Der in Ihrer Abrechnungswährung für den Abrechnungszeitraum zum angegebenen Termin fällige Betrag. |
|Zahlungsanweisungen |Beschreibt, wo und wie Ihre Rechnung auf der Grundlage Ihrer Region bezahlt wird. Geben Sie bei einer Zahlung stets die Rechnungsnummer an. |
|Rechnungsnr. |Die Nummer Ihrer Rechnung. |
|Rechnungsdatum |Das Ausstellungsdatum Ihrer Rechnung. |
|Zahlungsbedingungen |Für einmalige Einkäufe wird dies immer 60Tage sein. |
|Fälligkeitsdatum der Zahlung |Ihre Zahlung muss bis zu diesem Datum eingegangen sein. |


**Detaillierte Liste einmaliger Gebühren**

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|Datum |Kaufdatum. |
|Beschreibung |Produktname. |
|Anzahl |Die Anzahl von erworbenen Produkten (Reservierungen etc). |
|Preis pro Einheit |Preis pro Produkt (Reservierungen etc). |
|Rabatte |Alle anwendbaren Rabatte. |
|Vorsteuerbetrag |Zwischensumme vor Steuern. |
|Mehrwertsteuer |Steuerbetrag. |
|Gesamt |Zahlungen gesamt. |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Azure Reserved VM Instance – Gebührenbeschreibung der Abstimmungsdatei

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|PartnerID |Partner-ID im GUID-Format. |
|Kunden-ID |Eindeutige Microsoft-ID im GUID-Format: wird zur Identifizierung des Kunden verwendet. |
|CustomerName |Firmenname des Kunden wie im Partner Center angegeben. Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen. |
|CustomerDomainName |Domänenname des Kunden. |
|CustomerCountry |Land, in dem sich der Kunde befindet. |
|InvoiceNumber |Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
|MPNID |Die MPN-ID des CSP Partners (direkt oder indirekt). |
|MPN-ID der Handelspartner |Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt. Die MPN-ID des registrierten Handelspartners für die Reservierung. Dies entspricht der Handelspartner-ID, die für die spezifische Reservierung im Partner Center aufgeführt ist. Wenn ein CSP-Partner die Reservierung direkt an den Kunden veräußert hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners. Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt. Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt. |
|OrderID |Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform. Kann beim Kontakt zum Support zum Identifizieren von Azur Reservations hilfreich sein, jedoch nicht zur Abstimmung. |
|Bestellungsdatum |Der Zeitpunkt der Auftragserstellung. |
|ProductId |Die ID für das Produkt. |
|SkuID  |Die ID für eine bestimmte SKU. |
|AvailabilityId |Die ID für eine bestimmte Verfügbarkeit. "Verfügbarkeit" bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, Währung, Branche usw. erhältlich ist. |
|SkuName  |Titel für eine bestimmte SKU. |
|ProductName |Name des Produkts. |
|ChargeType |Art der Gebühren oder der Anpassung. |
|UnitPrice |Preis pro bestelltem Produkt. |
|Anzahl |Anzahl der bestellten Produkte. |
|Zwischensumme |Gesamtbetrag vor Steuern Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt. |
|TaxTotal |Die Summe aller anwendbaren Steuern. |
|Gesamt |Dies ist die Gesamtanzahl der Käufe. |
|Währung |Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform. |
|DiscountDetails |Detaillierte Liste der relevanten Rabatte. |


## <a name="manage-your-billing"></a>Verwalten Ihrer Abrechnung

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>Anzeigen des aktuellen Abrechnungsstatus, Rechnungen und Abstimmungsdateien

1.  Wählen Sie im Partner Center **Abrechnung** und anschließend **einmal** um Ihren Rechnungsstatus anzuzeigen. 
2.  Wählen Sie eine Rechnung oder Abstimmungsdatei, um ausführlichere Informationen anzuzeigen. 

### <a name="view-a-customers-order-history"></a>Bestellverlauf eines Kunden anzeigen

1.  Wählen Sie **Kunden** aus dem Menü "Partner Center".
2.  Auf der Seite **Kunden**, suchen Sie den Kunden, deren Bestellverlauf Sie anzeigen möchten, und wählen Sie dann den Pfeil nach unten, um den Datensatz des Kunden zu erweitern. 
3.  Wählen Sie **Aufträge anzeigen**, um den Bestellverlauf anzuzeigen.

### <a name="create-a-credit-or-void-note"></a>Erstellen Sie eine Gutschrift oder eine leere Rechnung

Zu einem bestimmten Zeitpunkt müssen Sie möglicherweise eine Rechnung stornieren und eine neue ausstellen. Beispielsweise kann ein Kunde den Namen der Geschäftsabläufe ändern, und dann eine Rechnung mit dem alten Namen erhalten. 

Um eine Rechnung zu stornieren und eine neue auszustellen, laden Sie das Formular aus der Abrechnungsseite unter „Anpassen” herunter.

## <a name="azure-reservations-resources"></a>Azure Reservations-Ressourcen
|**Weitere Informationen**   |**Bitte lesen**    |
|:-----------------------------|:-----------------|
|Azure Reservations in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure Reservations für Ihre Kunden im Partner Center   |[Azure Reservations kaufen](azure-reservations-buying.md)
| Verwalten von Azure Reservations im Partner Center | [Verwalten von Azure Reservations im Partner Center](azure-reservations-manage.md)
|Erwerb von Azure Reservations im Azure-Portal | [Für virtuelle Maschinen mit Azure Reserved VM Instances im Voraus bezahlen](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure Reservations im Azure-Portal   |[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure Reservations über die Partner Center-API | [Erwerben Sie Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in die Partner Center-Entwicklerdokumentation

 
