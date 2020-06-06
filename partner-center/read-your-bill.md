---
title: Lesen Ihrer Rechnung & Datei "Reconnaissance"
ms.topic: article
ms.date: 06/05/2020
description: Erfahren Sie mehr über Ihre Rechnung & Abstimmungs Dateien. Ihre Rechnung zeigt Partner Center-Gebühren für das Programm, die Produkte und Kunden für diesen monatlichen Zeitraum an.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: LauraBrenner
ms.author: labrenne
keywords: Abonnementabrechnungen, Abrechnung, Abrechnung im Partner Center, Partner Center-Abrechnung, meine Rechnung lesen, Rechnung, Rechnung für Partner Center, CSP-Abrechnung, wo ist meine Rechnung?
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab5e9667b766566e3af4ddd524805ff31dfc2a59
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467460"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Informationen zu Ihrer Rechnung und Abstimmungs Datei: erfahren Sie, wie Sie diese im Partner Center finden.

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Globaler Administrator
- Abrechnungsadministrator
- Administrator-Agent


Ihre **Rechnung** ist eine **Zusammenfassung aller Kosten Ihres Partner Centers** (Programm übergreifend, alle Produkte und alle Kunden). 

## <a name="invoice-types"></a>Rechnungs Typen

Microsoft gibt eine Rechnung für Lizenz basierte Gebühren (z. b. Office 365) und nutzungsbasierte Gebühren (z. b. Azure) und eine separate Rechnung für einmalige Gebühren (z. b. Azure RI, Marketplace oder Azure-Plan) aus.

Beispiel:  

**Szenario 1 [Einzel Währung]**: Partner verfügt über Einkäufe für das Angebot "145P" und "O365 Licenses",  

- Der Partner erhält eine Rechnung PDF und 2 Abstimmungs Dateien, die die Gebühren für O365 und Azure (145P) abdecken.  

**Szenario 2 [Einzel Währung]**: der Partner hat Käufe für den Azure-RI-, Marketplace-und/oder Azure-Plan zusammen mit 145P-Käufen.

- Der Partner erhält eine Rechnung PDF und eine Abstimmungs Datei mit den Gebühren für Azure (145P). 

- Der Partner erhält eine weitere Rechnung PDF und eine Abstimmungs Datei mit den Gebühren für den Azure RI-, Marketplace-und Azure-Plan. 

**Szenario 3 [Multi-currency]**: der Partner hat Käufe für Azure RI in DKK und Azure-Plan in EUR zusammen mit 145P-Käufen in EUR.

- Der Partner erhält eine Rechnung PDF und eine Abstimmungs Datei, die die Gebühren für Azure RI in DKK abdeckt. 

- Der Partner erhält eine Rechnung PDF und eine Abstimmungs Datei, in der die Gebühren für den Azure-Plan in Euro abgerechnet werden. 

- Der Partner erhält eine weitere Rechnung PDF und eine Abstimmungs Datei, in der die Gebühren für das Angebot "145P" in EUR (oder die Partner Abrechnungswährung) abgedeckt werden. 

## <a name="find-your-bill"></a>Auffinden Ihrer Rechnung 

Sie finden Ihre Rechnung auf der Seite Abrechnung des Dashboards im Partner Center. Sie können auf dieser Seite auch ihren Abrechnungs Verlauf, Ausgaben Trends und Abstimmungs Dateien finden. 

1. Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/home) an. 

2. Wählen Sie im Menü auf der linken Seite die Option **Abrechnung**aus. 

3. Wählen Sie auf der Seite Abrechnung die Rechnung aus, die Sie herunterladen möchten. 

Einen Link zu ihrer neuesten Rechnung finden Sie oben auf der Seite unter Account Saldo as of Last Rechnungs Date. 

Vorherige Rechnungen finden Sie im Abschnitt Abrechnungs Verlauf. Wählen Sie das entsprechende Jahr aus, und wählen Sie dann den Dropdown Pfeil neben dem entsprechenden Abrechnungszeitraum aus. Wählen Sie den Link neben Rechnungen (PDF) aus, um die Rechnung dieses Zeitraums herunterzuladen. 

## <a name="understanding-invoice-pdf"></a>Grundlegendes zur Rechnung PDF 

**Rechnungen für Nutzungs-und Lizenz basierte Gebühren**: Rechnungen für Gebühren für Dienste wie Office 365 und Azure sind innerhalb von zwei (2) Tagen nach dem ausgewählten Abrechnungsdatum [UTC] verfügbar.  

**Rechnungen für einmalige und wiederkehrende Gebühren**: Rechnungen für Gebühren für Dienste wie Azure RI, Azure-Plan, Marketplace sind nicht später als 8. jeden Monats verfügbar.  

Im folgenden finden Sie einige der Schlüsselfelder im PDF-Dokument der Rechnung –

**Rechnungsnummer**: eindeutiger Bezeichner für das Rechnungsdokument, das für den jeweiligen Abrechnungszeitraum generiert wurde. 

**Abrechnungszeitraum**: Dies ist der Zeitraum, in dem Sie Verwendungs-und Lizenz basierte Dienste haben. 

**Rechnungsdatum**: Das Abrechnungsdatum oder das Enddatum, an dem Ihre Rechnung monatlich generiert wird. 

**Fälligkeitsdatum der Zahlung**: das Datum, an dem Ihre Zahlung empfangen werden muss. 

**Gebühren**: der Betrag, der in ihrer Abrechnungswährung für den jeweiligen Abrechnungszeitraum fällig ist. 

**Gutschriften**: Guthaben (z. b. SLA) oder Anpassungen bei Änderungen an Abonnements (z. b. erhöhen oder verringern des Arbeitsplatzes). 

**Zahlungsanweisungen**: Beschreibung der Bezahlung Ihrer Rechnung basierend auf Ihrer Region. Stellen Sie bei einer Zahlung immer sicher, dass Sie Ihre Rechnungsnummer einschließen. 

Eine ausführliche Beschreibung aller Felder in der Rechnungs Datei (einschließlich der Felder für einmalige Gebühren) finden Sie unter [Rechnungs Datei Felder](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Grundlegendes zu Abstimmungs Dateien

 Abstimmungs Dateien, die einen Drilldown/Details zu ihren Gebühren enthalten, können zusammen mit der Rechnung PDF heruntergeladen werden. Zu den Abstimmungs Dateien gehören Kunden Bezeichner und Abonnement Bezeichner, mit denen Sie Kunden Rechnungen erstellen können. Weitere Informationen zu den Reconnaissance-Dateien finden Sie unter  [Verwenden der](use-the-reconciliation-files.md) ababstimmungs Dateien. 
