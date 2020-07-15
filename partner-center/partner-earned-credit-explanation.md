---
title: Vom Partner erworbenes Guthaben für verwaltete Dienste
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie vom Microsoft-Partner erworbenes Guthaben (Partner Earned Credit, PEC) für verwaltete Dienste berechnet und ausgezahlt wird und wie Sie sicherstellen können, dass Sie berechtigt sind.
author: adamyeh
ms.author: adamyeh
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d240b3d8e411ce55b086a63d1c14903d6f666d7
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390617"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Wie von Partnern erworbene Guthaben berechnet und bezahlt werden

**Geeignete Rollen**

- Globaler Administrator
- Benutzeradministrator
- Administrator-Agent
- Abrechnungsadministrator
- Vertriebsbeauftragter

Von Partnern erworbene Guthaben für verwaltete Dienste (Partner-Earned Credit, PEC) bedeuten Anerkennung und Belohnung für Partner, die die Kontrolle und Verwaltung der IT Operations der Azure-Umgebungen ihrer Kunden rund um die Uhr ganz oder teilweise innehaben. Standardmäßig werden Partnern in CSP die erforderlichen Zugriffsrechte auf das Kundenabonnement erteilt, die es ihnen ermöglichen, die operative Verwaltung und Steuerung der Abonnementressourcen rund um die Uhr (24/7) durchzuführen. Weitere Möglichkeiten, wie der Kunde den Zugriff für den handelnden Partner bereitstellen kann, sind im folgenden Abschnitt beschrieben. Der monatliche Rechnungsbetrag ist bezogen auf die vom Partner erworbene Gutschrift netto. Die Partner können die PEC-Details in ihrer monatlichen Abstimmungsdatei sehen. Informationen zu weiteren Verfahren, mit denen ein Kunde den Zugriff für den handelnden Partner bereitstellen kann, finden Sie unter [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md).

Lesen Sie auch [Reaktivieren von Administratorrechten für Azure CSP-Abonnements](revoke-reinstate-csp.md).

## <a name="important-eligibility-and-calculation-information"></a>Wichtige Informationen zu Berechtigung und Berechnung

- Der Partner sollte einen aktiven MPN-Vertrag und eine gültige RBAC-Rolle besitzen, um erworbene Gutschriften für die von ihm verwalteten Azure-Ressourcen zu erhalten. 

- Im Fall indirekter Anbieter und ihrer indirekten Wiederverkäufer ist der indirekte Anbieter für PEC qualifiziert, wenn entweder er, der indirekte Wiederverkäufer oder beide die operative Steuerung und Verwaltung der Azure-Ressourcen des Kunden in CSP rund um die Uhr (24/7) sicherstellen.

- PEC ist der abgerechneten (kostenpflichtigen) Nutzung der Azure-Umgebung des Kunden in CSP zugeordnet, die vom Partner verwaltet wird. PEC ist nur für Partner in CSP verfügbar, die mit Microsoft abrechnen (indirekter Anbieter und Direktrechnungspartner). 

- Berechtigte Dienste: Von Partnern erworbenes Guthaben kann auf Dienste angerechnet werden, die in den **Preisen für Azure-Plannutzung** aufgelistet sind, die Partner von der Seite [Azure-Plan-Preise](https://partner.microsoft.com/commerce/sales) exportieren können. Beachten Sie, dass es Ausnahmen gibt, beispielsweise Produkte von Drittanbietern, die in der **Tags**-Spalte der Preisliste für die Azure-Plannutzung und Azure-Plan Reservierungen als **Drittanbieter** gekennzeichnet sind, sowie Produkte in der Marketplace-Preisliste.

- PEC wird täglich berechnet und kann in der täglichen Nutzungsdatei und der Abstimmungsdatei zur monatlichen Rechnung angezeigt werden. Ein Partner (indirekter Anbieter oder indirekter Wiederverkäufer) muss den gesamten Tag hindurch (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er PEC erwirbt.  

- PEC wird bis hinab zur Azure-Ressourcenebene erworben. Wenn der Partner über gültigen Zugriff verfügt, verdient jede Ressource auf Abonnement- oder Ressourcengruppenebene, die an die nächst höhere Entität berichtet, PEC.  

- Die Details von PEC sind auch unter [Azure-Kostenmanagement](https://go.microsoft.com/fwlink/?linkid=2106482) verfügbar.

## <a name="azure-cost-management"></a>Azure-Kostenmanagement

 Azure Cost Management (ACM) mit Kostenanalyse ermöglicht es Ihnen als Partner, die Kosten anzuzeigen, auf die der PEC-Vorteil angerechnet wurde.  

1. Melden Sie sich im Azure-Portal bei Ihrem Partnermandanten an, und wählen Sie **Kostenmanagement + Abrechnung** aus.
2.  Wählen Sie **Kostenmanagement** aus.
3.  Wählen Sie **Kostenanalyse** aus.

In der Ansicht „Kostenanalyse“ werden die Kosten für Ihr Abrechnungskonto für alle erworbenen und genutzten Dienste mit den Preisen angezeigt, die Sie an Microsoft bezahlen.

4.  Wählen Sie **PartnerEarnedCreditApplied** in der Dropdownliste einer PivotChart aus, um die Kosten anzuzeigen, auf die PEC angerechnet wurden. Wenn die **PartnerEarnedCreditApplied**-Eigenschaft den Wert „True“ aufweist, wurde auf die zugehörigen Kosten das vom Partner erworbene Guthaben angerechnet. 

Wenn die Eigenschaft „PartnerEarnedCreditApplied“ den Wert „False“ aufweist, haben die zugehörigen Kosten nicht die erforderliche Berechtigung für die Gutschrift erfüllt, oder der erworbene Dienst ist nicht für PEC qualifiziert.

>[!NOTE] 
>In der Regel dauert es 8–24 Stunden, bis die Verwendung von Diensten unter **Kostenmanagement** angezeigt wird, und die PEC-Gutschriften werden innerhalb von 48 Stunden ab dem Zeitpunkt des Zugriffs in Azure Cost Management angezeigt.

5. Sie können auch nach der **PartnerEarnedCreditApplied** Eigenschaft gruppieren und filtern, indem Sie die Filterfeatures **Gruppieren nach** verwenden, um einen Drilldown der Kosten auszuführen, für die PEC angerechnet ober nicht angerechnet wurden.

## <a name="next-steps"></a>Nächste Schritte

- [Vom Partner erworbenes Guthaben – Übersicht](partner-earned-credit.md)

- Detaillierte Berechnungsbeispiele für von Partnern erworbenes Guthaben finden Sie in der Preisliste, auf die Sie über das Partner Center-Dashboard zugreifen können (Anmeldung erforderlich).

- [Umstellung auf Azure-Plan: Einstieg](azure-plan-get-started.md)

- [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)

- [Wiederrufen oder Reaktivieren von Administratorrechten für Azure CSP-Abonnements](revoke-reinstate-csp.md)

