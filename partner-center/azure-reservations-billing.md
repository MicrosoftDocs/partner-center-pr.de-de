---
title: Abrechnung für Azure-Reservierungen | Partner Center
ms.topic: article
ms.date: 03/15/2019
Description: Informationen zur Abrechnung von Azure-Reservierungen.
author: LauraBrenner
ms.author: v-petand
keywords: Azure RI, reservierte Azure-Instanzen, Reservierungen, VM, virtuelle Computer, verwalten, Abrechnung, kaufen
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: b99cb2a72d69cd33f9267a956f921aa65dedd482
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135420"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Microsoft Azure Reserved VM Instances – Abrechnung

**Gilt für**

-  Partner Center
-  Microsoft Azure-Portal
-  CSP-Partner

Partner im Cloud Solution Provider-Programm (CSP) können ihren Kunden reservierte Instanzen auf Microsoft Azure-VMs anbieten. Kunden können virtuelle Computer im Voraus reservieren – für ein Jahr oder drei Jahre – und erhebliche Einsparungen bei der Azure-Nutzung erhalten.   

Die Kunden bezahlen im Voraus für Azure Reserved VM Instances. Wenn Sie Azure Reserved VM Instances im Auftrag eines Kunden kaufen, erhalten Sie Rechnungen und Kontenabstimmungsdateien für diese einmaligen Gebühren. 

>[!IMPORTANT]
>Wenn Sie Azure Reserved VM Instances für einen Kunden in einem Markt mit einer anderen Währung als Ihrer Währung erwerben, basiert die Standardabrechnungswährung auf dem Markt des Kunden, nicht Ihrem Standort. Wenn Sie Kunden in mehreren Märkten haben, erhalten Sie getrennte Rechnungen und Kontenabstimmungsdateien für jede Währung der Kunden, die in Rechnung gestellt werden müssen, damit Sie Ihren Kunden Rechnungen in der entsprechenden Währung ausstellen können. 

Um auf einmalige Rechnungen und Kontenabstimmungsdateien zuzugreifen, wählen Sie im Partner Center **Abrechnung** und dann **Einmal** aus. 

Weitere allgemeine Informationen zur Abrechnung im Cloud Solution Provider-Programm finden Sie unter [Grundlagen zur Abrechnung](billing-basics.md).

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Azure Reserved VM Instance – Definitionen zur Rechnungsdatei

**Allgemeine Abrechnungsinformationen**

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|US FEIN |Ihre Steuernummer. |
|Rechnungsempfänger |Die verwendete rechtliche Geschäftsadresse für steuerliche Zwecke. Um diese Adresse zu ändern, wechseln Sie zu „Kontoeinstellungen“ > „Partnerabrechnungsprofil“. |
|Gebühren |Gesamtsumme der aktuellen Gebühren. |
|Gutschriften |Gutschriften für Rückerstattungsaktivitäten seit dem ersten Kauf. |
|Rabatte |Rabatte, die für Azure-Reservierungen oder andere Elemente in der jeweiligen Kundenbestellung gelten. |
|Steuern |Die gesamten Steuern für die aktuellen Gebühren, wie im Abschnitt „Details“ auf Seite 2 der Rechnung summiert. |
|Gesamtsumme der aktuellen Gebühren |Der in Ihrer Abrechnungswährung für den Abrechnungszeitraum zum angegebenen Termin fällige Betrag. |
|Zahlungsanweisungen |Beschreibt, wann und wie Ihre Rechnung auf der Grundlage Ihrer Region bezahlt wird. Geben Sie bei einer Zahlung stets die Rechnungsnummer an. |
|Rechnungsnr. |Die Nummer Ihrer Rechnung. |
|Rechnungsdatum |Das Ausstellungsdatum Ihrer Rechnung. |
|Zahlungsbedingungen |Für einmalige Einkäufe wird dies immer 60 Tage sein. |
|Fälligkeitsdatum der Zahlung |Ihre Zahlung muss bis zu diesem Datum eingegangen sein. |


**Detaillierte Liste einmaliger Gebühren**

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|Datum |Kaufdatum. |
|Beschreibung |Produktname. |
|Anzahl |Die Anzahl von erworbenen Produkten (z.B. Reservierungen). |
|Preis pro Einheit |Preis pro Produkt (z.B. Reservierung). |
|Rabatte |Alle anwendbaren Rabatte. |
|Vorsteuerbetrag |Zwischensumme der Einkäufe vor Steuern. |
|Mehrwertsteuer |Steuerbetrag. |
|Gesamt |Zahlungen gesamt. |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Azure Reserved VM Instance – Beschreibungen der Kontenabstimmungsdatei

|**Feld** |**Definition**|
|:----------------|:-----------------------------|
|PartnerID |Partner-ID im GUID-Format. |
|Kunden-ID |Eindeutige Microsoft-ID im GUID-Format, die zur Identifizierung des Kunden verwendet wird. |
|CustomerName |Firmenname des Kunden wie im Partner Center angegeben. Dies ist sehr wichtig für die Abstimmung der Rechnung mit Ihren Systeminformationen. |
|CustomerDomainName |Der Name der Kundendomäne. |
|CustomerCountry |Das Land, in dem sich der Kunde befindet. |
|InvoiceNumber |Rechnungsnummer, in der die angegebene Transaktion angezeigt wird. |
|MPNID |Die MPN-ID des CSP-Partners (direkt oder indirekt). |
|MPN-ID der Handelspartner |Wird nur in den Abstimmungsdateien für Partner im indirekten Modell angezeigt. Die MPN-ID des registrierten Handelspartners für die Reservierung. Dies entspricht der Handelspartner-ID, die für die spezifische Reservierung im Partner Center aufgeführt ist. Wenn ein CSP-Partner die Reservierung direkt an den Kunden verkauft hat, wird seine MPN-ID zweimal aufgeführt: als MPN-ID und als MPN-ID des Handelspartners. Wenn ein CSP-Partner über einen Handelspartner ohne MPN-ID verfügt, wird dieser Wert stattdessen auf die MPN-ID des Partners festgelegt. Wenn der CSP-Partner eine Handelspartner-ID entfernt, wird dieser Wert auf-1 festgelegt. |
|OrderID |Eindeutiger Bezeichner für eine Bestellung auf der Microsoft-Abrechnungsplattform. Kann beim Kontaktieren des Supports zur Identifizierung der Azure-Reservierung hilfreich sein, jedoch nicht zur Kontenabstimmung. |
|OrderDate |Das Datum, an dem die Bestellung aufgegeben wurde. |
|ProductID |Die ID des Produkts. |
|SkuId  |Die ID einer bestimmten SKU. |
|AvailabilityId |Die ID einer bestimmten Verfügbarkeit. „Verfügbarkeit“ bezieht sich darauf, ob eine bestimmte SKU für ein bestimmtes Land, eine Währung, ein Branchensegment usw. erhältlich ist. |
|SkuName  |Der Titel einer bestimmten SKU. |
|ProductName |Der Name des Produkts. |
|ChargeType |Art der Gebühren oder der Anpassungen. |
|UnitPrice |Preis pro bestelltem Produkt. |
|Anzahl |Anzahl der bestellten Produkte. |
|Zwischensumme |Gesamtbetrag vor Steuern Überprüft, ob bei Rabatten Ihre Zwischensumme mit dem erwarteten Gesamtbetrag übereinstimmt. |
|TaxTotal |Die Summe aller anwendbaren Steuern. |
|Gesamt |Der Gesamtbetrag für diesen Erwerb. |
|Währung |Währungstyp Jede Abrechnungsentität verfügt nur über eine Währung. Überprüft auf Übereinstimmung in Ihrer ersten Rechnung und nach jedem großen Update der Abrechnungsplattform. |
|DiscountDetails |Detaillierte Liste der relevanten Rabatte. |


## <a name="manage-your-billing"></a>Verwalten Ihrer Abrechnung

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>Anzeigen Ihres aktuellen Abrechnungsstatus, Ihrer Rechnungen und Kontenabstimmungsdateien

1.  Wählen Sie im Partner Center **Abrechnung** und dann **Einmal** aus, um Ihren Abrechnungsstatus anzuzeigen. 
2.  Wählen Sie eine Rechnung oder Kontenabstimmungsdatei aus, um ausführlichere Informationen anzuzeigen. 

### <a name="view-a-customers-order-history"></a>Anzeigen des Bestellverlaufs eines Kunden

1.  Wählen Sie im Menü „Partner Center” **Kunden** aus.
2.  Suchen Sie auf der Seite **Kunden** den Kunden, dessen Bestellverlauf Sie anzeigen möchten, und wählen Sie den Abwärtspfeil aus, um den Datensatz des Kunden zu erweitern. 
3.  Wählen Sie **Bestellungen anzeigen** aus, um den Bestellverlauf anzuzeigen.

### <a name="create-a-credit-or-void-note"></a>Erstellen einer Gutschrift oder eines Stornierungshinweises

Zu einem bestimmten Zeitpunkt müssen Sie eine Rechnung möglicherweise stornieren und eine neue ausstellen. Beispielsweise kann ein Kunde den Namen seines Unternehmens ändern und dann eine Rechnung mit dem alten Namen erhalten. 

Um eine Rechnung zu stornieren und eine neue auszustellen, laden Sie das Formular aus der Abrechnungsseite unter „Anpassungen” herunter.

## <a name="azure-reservations-resources"></a>Ressourcen zu Azure-Reservierungen
|**Weitere Informationen**   |**Bitte lesen**    |
|:-----------------------------|:-----------------|
|Azure-Reservierungen in CSP (Übersicht)  | [Verkaufen von Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Erwerb von Azure-Reservierungen für Ihre Kunden im Partner Center   |[Kaufen von Azure-Reservierungen](azure-reservations-buying.md)
| Verwalten von Azure-Reservierungen im Partner Center | [Verwalten von Azure-Reservierungen im Partner Center](azure-reservations-manage.md)
|Erwerb von Azure-Reservierungen im Azure-Portal | [Vorauszahlen für virtuelle Computer mit Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in der Azure-Hilfe |
|Verwalten von Azure-Reservierungen im Azure-Portal   |[Verwalten von reservierten VM-Instanzen](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in der Azure-Hilfe  |
|Erwerb von Azure-Reservierungen über die Partner Center-API | [Erwerb von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation

 
