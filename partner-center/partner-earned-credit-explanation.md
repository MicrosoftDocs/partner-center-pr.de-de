---
title: Vom Partner erworbenes Guthaben für verwaltete Dienste
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie vom Microsoft-Partner erworbenes Guthaben (Partner Earned Credit, PEC) für verwaltete Dienste berechnet und ausgezahlt wird und wie Sie sicherstellen können, dass Sie berechtigt sind.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 022e7aabd0d850660f8236dce9a4fab9069af01b
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087126"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Wie von Partnern erworbene Guthaben berechnet und bezahlt werden

**Geeignete Rollen**

- Globaler Administrator
- Benutzerverwaltungsadministrator
- Administrator-Agent
- Abrechnungsadministrator
- Vertriebsbeauftragter

Von Partnern erworbene Guthaben für verwaltete Dienste (Partner-Earned Credit, PEC) bedeuten Anerkennung und Belohnung für Partner, die die Kontrolle und Verwaltung der IT Operations der Azure-Umgebungen ihrer Kunden rund um die Uhr ganz oder teilweise innehaben. Standardmäßig werden Partnern in CSP die erforderlichen Zugriffsrechte auf das Kundenabonnement erteilt, die es ihnen ermöglichen, die operative Verwaltung und Steuerung der Abonnementressourcen rund um die Uhr (24/7) durchzuführen. Weitere Möglichkeiten, wie Kunden den Zugriff für handelnde Partner bereitstellen können, sind im folgenden Abschnitt beschrieben. Der monatliche Rechnungsbetrag ist bezogen auf das vom Partner erworbene Guthaben netto. Die Partner können die PEC-Details in ihrer monatlichen Abstimmungsdatei sehen. Informationen zu weiteren Verfahren, mit denen ein Kunde den Zugriff für den handelnden Partner bereitstellen kann, finden Sie unter [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md).

Lesen Sie auch [Reaktivieren von Administratorrechten für Azure CSP-Abonnements](revoke-reinstate-csp.md).

## <a name="eligibility"></a>Berechtigung

Um von Partnern erworbene Guthaben (PEC) zu erhalten, gelten die folgenden Anforderungen: 

- Sie müssen eine aktive MPN-Vereinbarung und eine gültige RBAC-Rolle (rollenbasierte Zugriffssteuerung) besitzen, um erworbene Guthaben für die von Ihnen verwalteten Azure-Ressourcen zu erhalten.

- Sie müssen über die operative Kontrolle und Verwaltung der Azure-Ressourcen des Kunden in CSP rund um die Uhr (24/7) verfügen. Das bedeutet, dass Sie Administratorrechte für das Azure-Abonnement, die Azure-Ressourcengruppe und die Azure-Ressource des Kunden besitzen müssen. Im Fall indirekter Anbieter und ihrer indirekten Wiederverkäufer ist der indirekte Anbieter für PEC qualifiziert, wenn entweder er, der indirekte Wiederverkäufer oder beide über diese operative Kontrolle verfügen. Weitere Informationen darüber finden Sie unter [Reaktivieren von Administratorrechten für Azure CSP-Abonnements](./revoke-reinstate-csp.md).

- Zusätzlich zu den oben genannten Anforderungen können von Partnern erworbene Guthaben nur auf Dienste angerechnet werden, die in den Preisen für die Azure-Plannutzung aufgelistet sind, die Sie von der Seite [Preise für Azure-Pläne](https://partner.microsoft.com/commerce/sales) exportieren können.

- PEC kann auf folgende Dienste **nicht** angerechnet werden:
    - Azure-Planreservierungen
    - Produkte von Drittanbietern, die in der Spalte „Tags“ der Preisliste für die Azure-Plannutzung als „Drittanbieter“ gekennzeichnet sind
    - Produkte in der Marketplace-Preisliste
    - [Azure Spot-VMs](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC wird bis hinab zur Azure-Ressourcenebene erworben. Wenn Sie über gültigen Zugriff entweder auf Abonnement- oder Ressourcengruppenebene verfügen, wird PEC für jede Ressource erworben, für die ein Rollup zur höheren Entität durchgeführt wird.

- Ausführliche Informationen zu PEC sind auch auf der Seite [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) enthalten.

### <a name="calculation"></a>Berechnung

PEC wird täglich berechnet und kann in der täglichen Nutzungsdatei und der Abstimmungsdatei zur monatlichen Rechnung angezeigt werden. Ein Partner (indirekter Anbieter oder indirekter Wiederverkäufer) muss den gesamten Tag hindurch (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er PEC erwirbt. PEC wird täglich für die verwalteten Azure-Ressourcen berechnet. Partner, die den permanenten privilegierten Zugriff während des gesamten Monats (Zugriffsdauer) und für alle in Frage kommenden Ressourcen (Zugriffsumfang) aufrechterhalten, erhalten die volle PEC-Rate. Eine Reduzierung von Umfang und Dauer führt zu einer niedrigeren PEC-Rate für den Monat. In der Datei zur täglich bewerteten Nutzung ist für eine Azure-Ressource für jeden Tage angegeben, ob PEC angewendet wird oder nicht. Partner können sich auch für Warnungen registrieren, um Änderungen beim permanenten privilegierten Zugriff zu überwachen.

## <a name="azure-cost-management"></a>Azure-Kostenmanagement

Azure Cost Management (ACM) mit Kostenanalyse ermöglicht es Ihnen als Partner, die Kosten anzuzeigen, auf die der PEC-Vorteil angerechnet wurde.  

1. Melden Sie sich im [Azure-Portal](https://portal.azure.com) bei Ihrem Partnermandanten an, und wählen Sie **Kostenmanagement + Abrechnung** aus.

2. Wählen Sie **Kostenmanagement** aus.

3. Wählen Sie **Kostenanalyse** aus.

   In der Ansicht „Kostenanalyse“ werden die Kosten für Ihr Abrechnungskonto für alle erworbenen und genutzten Dienste mit den Preisen angezeigt, die Sie an Microsoft bezahlen.

4. Wählen Sie **PartnerEarnedCreditApplied** in der Dropdownliste einer PivotChart aus, um die Kosten anzuzeigen, auf die PEC angerechnet wurden. Wenn die **PartnerEarnedCreditApplied**-Eigenschaft den Wert „True“ aufweist, wurde auf die zugehörigen Kosten das vom Partner erworbene Guthaben angerechnet. 

   Wenn die Eigenschaft „PartnerEarnedCreditApplied“ den Wert „False“ aufweist, haben die zugehörigen Kosten nicht die erforderliche Berechtigung für die Gutschrift erfüllt, oder der erworbene Dienst ist nicht für PEC qualifiziert.

   >[!NOTE] 
   >In der Regel dauert es 8–24 Stunden, bis die Verwendung von Diensten unter **Kostenmanagement** angezeigt wird, und die PEC-Gutschriften werden innerhalb von 48 Stunden ab dem Zeitpunkt des Zugriffs in Azure Cost Management angezeigt.

5. Sie können auch nach der **PartnerEarnedCreditApplied** Eigenschaft gruppieren und filtern, indem Sie die Filterfeatures **Gruppieren nach** verwenden, um einen Drilldown der Kosten auszuführen, für die PEC angerechnet ober nicht angerechnet wurden.

## <a name="next-steps"></a>Nächste Schritte

- [Vom Partner erworbenes Guthaben – Übersicht](partner-earned-credit.md)

- Detaillierte Berechnungsbeispiele für von Partnern erworbenes Guthaben finden Sie in der Preisliste, auf die Sie über das Partner Center-Dashboard zugreifen können (Anmeldung erforderlich).

- [Umstellung auf Azure-Plan: Einstieg](azure-plan-get-started.md)

- [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)

- [Widerrufen oder Reaktivieren von Administratorrechten für Azure CSP-Abonnements](revoke-reinstate-csp.md)
