---
title: Lesen der Rechnungs- &-Recon-Datei
ms.topic: article
ms.date: 06/05/2020
description: Erfahren Sie mehr über Ihre Rechnungs- & Abstimmungsdateien. Auf Ihrer Rechnung Partner Center die Gebühren für das Programm, die Produkte und die Kunden für diesen monatlichen Zeitraum.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f16b619aba838da1d1da0c5eb13648ebb107c802
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855912"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Informationen zu Ihrer Rechnungs- und Abstimmungsdatei: Erfahren Sie, wie Sie sie in der Partner Center


**Geeignete Rollen:** Globale Administratorrechte | Abrechnungsadministrator| Administrator-Agent


Ihre **Rechnung** ist eine **Zusammenfassung ihrer Partner Center** Gebühren (programmübergreifend, alle Produkte und alle Kunden). 

## <a name="find-your-bill-and-reconciliation-file"></a>Suchen ihrer Rechnungs- und Abstimmungsdatei 

Sie finden Ihre Rechnung auf der Seite Abrechnung des Dashboards in Partner Center. Auf dieser Seite finden Sie auch Ihren Abrechnungsverlauf, Ihre Ausgabentrends und Abstimmungsdateien. 

1. Melde dich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home) an. 

2. Wählen Sie im Menü auf der linken Seite Abrechnung **aus.** 

3. Wählen Sie auf der Seite „Abrechnungsstatus“ eine Rechnung oder Kontenabstimmungsdatei aus, um ausführlichere Informationen anzuzeigen. 

Einen Link zu Ihrer neuesten Rechnung finden Sie oben auf der Seite unter Kontostand ab dem letzten Rechnungsdatum. 

Vorherige Rechnungen finden Sie im Abschnitt Abrechnungsverlauf. Wählen Sie das entsprechende Jahr und dann den Dropdownpfeil neben dem entsprechenden Abrechnungszeitraum aus. Wählen Sie den Link neben Rechnungen (PDF) aus, um die Rechnung für diesen Zeitraum herunterzuladen. 

## <a name="invoice-types"></a>Rechnungstypen

Microsoft stellt eine Rechnung für lizenzbasierte Gebühren (z. B. Office 365) und nutzungsbasierte Gebühren (z. B. Azure) und eine separate Rechnung für einmalige Gebühren (z. B. Azure RI, Marketplace oder Azure-Plan) aus.

Beispiel:  

**Szenario 1 [Einzelne Währung]**: Partner hat Käufe für 145P-Angebote und O365-Lizenzen,  

- Partner erhalten eine PDF-Rechnung und zwei Abstimmungsdateien, die die Gebühren für O365 und Azure (145p) abdecken.  

**Szenario 2 [Einzelne Währung]**: Partner haben Käufe für Azure RI, Marketplace und/oder Azure-Plan zusammen mit 145p-Käufen.

- Partner erhalten eine PDF-Rechnung und eine Abstimmungsdatei, die die Gebühren für Azure (145p) abdecken. 

- Partner erhalten eine weitere RECHNUNGS-PDF-Datei und eine Abstimmungsdatei, die ihre Gebühren für Azure RI, Marketplace und Azure-Plan abdeckt. 

**Szenario 3 [Multiwährung]**: Partner hat Käufe für Azure RI in DKK und Azure-Plan in EURO zusammen mit 145p-Käufen in €.

- Der Partner erhält eine RECHNUNGS-PDF-Datei und eine Abstimmungsdatei, die die Gebühren für Azure RI in DKK abdeckt. 

- Der Partner erhält eine RECHNUNGS-PDF-Datei und eine Abstimmungsdatei, die die Gebühren für den Azure-Plan in EURO abdeckt. 

- Der Partner erhält eine weitere RECHNUNGS-PDF-Datei und eine Abstimmungsdatei, die die Gebühren für ein 145p-Angebot in EURO (oder der Abrechnungswährung des Partners) abdeckt. 


## <a name="understanding-invoice-pdf"></a>Grundlegendes zur RECHNUNGS-PDF-Datei 

**Rechnungen für Nutzungs- und lizenzbasierte Gebühren:** Rechnungen für Gebühren für Dienste wie Office 365 und Azure sind innerhalb von zwei (2) Tagen nach dem ausgewählten Abrechnungsdatum [UTC] verfügbar.  

**Rechnungen für einmalige und wiederkehrende Gebühren:** Rechnungen für Gebühren für Dienste wie Azure RI, Azure-Plan und Marketplace sind bis zum 8. jedes Monats verfügbar.  

Im Folgenden finden Sie einige der Schlüsselfelder im PDF-Dokument für Rechnungen:

**Rechnungsnummer:** Eindeutiger Bezeichner für das für den jeweiligen Abrechnungszeitraum generierte Rechnungsdokument. 

**Abrechnungszeitraum:** Dies ist der Zeitraum, in dem Sie über Nutzungen und lizenzbasierte Dienste verfügen. 

**Rechnungsdatum:** Das Abrechnungsdatum oder das Jahrestag, an dem Ihre Rechnung jeden Monat generiert wird. 

**Fälligkeitsdatum** der Zahlung: Das Datum, an dem Ihre Zahlung empfangen werden muss. 

**Gebühren:** Der in Ihrer Abrechnungswährung für den jeweiligen Abrechnungszeitraum fällige Betrag. 

**Guthaben:** Guthaben (z. B. SLA) oder Anpassungen für Änderungen an Abonnements (z. B. Erhöhung oder Verringerung der Lizenz). 

**Zahlungsanweisungen:** Beschreibung der Zahlung Ihrer Rechnung basierend auf Ihrer Region. Achten Sie bei einer Zahlung immer darauf, Dass Sie Ihre Rechnungsnummer angeben. 

Eine ausführliche Beschreibung aller Felder in Ihrer Rechnungsdatei (einschließlich der Felder für einmalige Gebühren) finden Sie unter Felder für [Die Rechnungsdatei.](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Verstehen von Abstimmungsdateien

 Abstimmungsdateien, die einen Drilldown bzw. detaillierte Details zu Ihren Gebühren enthalten, können zusammen mit der PDF-Rechnung heruntergeladen werden. Die Abstimmungsdateien enthalten Kunden-IDs und Abonnement-IDs, die Sie zum Erstellen von Kundenrechnungen verwenden können. Weitere Informationen zu den  [Abstimmungsdateien](use-the-reconciliation-files.md) finden Sie unter Verwenden der Abstimmungsdateien. 

## <a name="next-steps"></a>Nächste Schritte

- [Verwenden der Abstimmungsdateien](use-the-reconciliation-files.md)