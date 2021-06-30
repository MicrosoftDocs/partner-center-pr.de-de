---
title: Beantragen einer SLA-Gutschrift bei Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Erfahren Sie mehr über die Vorteile, Einschränkungen und Verfahren zum Anfordern eines Sla-Guthabens (Service Level Agreement, SLA) von Microsoft, wenn Für Ihre Kunden ein Dienstausfälle vor sich geht.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: f521e55869d60987fb46cd5d570bf206939e0782
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080638"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Anfordern eines SLA-Guthabens (Service Level Agreement, Vereinbarung zum Servicelevel) von Microsoft

**Geeignete Rollen:** Administrator-Agent| Globaler Administrator

Sie können **Sla-Gutschriften (Sla)** von Microsoft anfordern, wenn ein Dienst, den Sie für Ihre Kunden bereitstellen, aus dem Dienst aus ist.

## <a name="sla-credit-calculation"></a>SLA-Gutschriftberechnung

SLA-Gutschriften von Microsoft werden basierend auf den Diensten bestimmt, die davon in Mit wirkungen sind. Wenn Ihr Kunde beispielsweise über eine Office 365-Suite verfügt, aber nur ein SharePoint-Ausfall auftrat, wird das SLA-Guthaben nur für SharePoint und nicht für den gesamten Plan des Kunden genehmigt.

*Guthaben werden basierend auf dem betroffenen Dienst und der Dauer des Ausfalls anteilsgewertet.* Die Typen von Szenarien, die für SLA-Gutschriften qualifiziert sind, finden Sie im Dokument [Zur konsolidierten SLA für Onlinedienste.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Diese Informationen gelten auch für Dienste, die über Cloud Solution Provider CSP-Programm (CSP) verkauft werden.


## <a name="request-an-sla-credit"></a>Anfordern einer SLA-Gutschrift

*Der CSP-Partner muss den Anspruch und alle erforderlichen Informationen bis zum Ende des Kalendermonats übermitteln, der auf den Monat folgt, in dem der Vorfall aufgetreten ist.* Wenn der Vorfall beispielsweise am 15. Februar aufgetreten ist, muss Microsoft den Anspruch und alle erforderlichen Informationen bis zum 31. März erhalten. Endkunden und indirekte Vertriebspartner können keine SLA-Gutschriftansprüche übermitteln. Entweder der indirekte Anbieter oder der Direktabrechnungspartner muss Ansprüche in ihrem Namen übermitteln.

> [!NOTE]
> Beratungsvorfälle sind nicht für SLA-Gutschriften berechtigt. Ein Incident, der auf dem Service Health-Dashboard  veröffentlicht wird, gibt an, dass ein Mandant möglicherweise davon in Mitfällen besehen ist, und stellt die besten Informationen dar, die Microsoft zum Zeitpunkt der Veröffentlichung hat. Integritätsseitendaten stellen die allgemeine Verfügbarkeit eines Diensts dar. Die Auswirkungen, Entschärfung und Lösung einzelner Dienste können variieren. Weitere Informationen finden Sie in der abschließenden Incident Post- und Post Incident Review. Weitere [Informationen finden Sie Microsoft 365 Überprüfen der Integrität des](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) Diensts.

### <a name="required-information"></a>Erforderliche Informationen

Kundenname, Mandantenbezeichner, Partnerticket# und ticket created date/time stamp sind für die Verarbeitung eines Anspruchs nicht ausreichend.

Bevor Sie [eine SLA-Gutschriftanforderung](#submit-sla-credit-request) an  Microsoft übermitteln, müssen Sie alle folgenden Informationen erfassen, die in Ihr Supportticket enthalten sind:

- GuiD des Kunden mandanten
- Der [Incidentbezeichner für den Ausfall?](#outage-incident-identifier)
- Der Nachweis, dass der Kunde von dem Ausfall in Mitbewirkung genommen wurde und ein SLA-Guthaben angefordert hat.
- Wurden die über CSP erworbenen Abonnements von den Auswirkungen? (*ja* oder *nein*)

#### <a name="evidence-that-proves-customer-impact"></a>Beweise, die auswirkungen auf Kunden belegen

- Informationen zu Zeit und Dauer der Ausfallzeit
- Anzahl und Speicherort der betroffenen Benutzer (falls zutreffend)
- Beschreibungen Ihrer Versuche, den Incident zum Zeitpunkt des Auftretens zu beheben
- Eine E-Mail des kundenspezifischen Kunden, der Support anklangt, und anschließend eine Gutschrift
- Die Nummer des Supporttickets und details des Kundenkontakts im Hinblick auf die Lösung der Auswirkungen auf den Dienst


#### <a name="outage-incident-identifier"></a>Id des Incidents "Ausfall"

Sie finden den Bezeichner für den Ausfallvorfall auf **Service Health** Seite im Microsoft 365 Admin Center. Die **Incident-ID** für Den Ausfall ist eine Zahl, der eine zweibuchstabende Abkürzung voran steht, die den betroffenen Dienst angibt (z. B. *EX25194* für einen Exchange Online-Ausfall). In der folgenden Tabelle werden allgemeine Dienstabkürzungen beschrieben:

| Zwei buchstabenbasierte Abkürzung | Microsoft-Dienst |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online-Schutz |
| SB | Skype for Business Online (ehemals Lync Online) |
| Betriebssystem | Office-Abonnement |
| PB | Power BI für Office 365 |
| SP | SharePoint Online |
| Ya | Yammer Enterprise |
| MO | Portalfehler |

### <a name="submit-sla-credit-request"></a>Übermitteln einer SLA-Gutschriftanforderung

So übermitteln Sie Ihre SLA-Gutschriftanforderung über das dashboard Partner Center An Microsoft:

1. Melden Sie sich beim Partner Center-Dashboard an.
2. Wählen Sie im Menü auf der linken Seite **service requests (Serviceanfragen)** und dann **Partner support requests (Partnersupportanfragen) aus.**
3. Wählen Sie **auf der Seite Partneranforderung** die Option **Neue Anforderung aus.**
4. Suchen Sie **auf der Seite Anforderung** starten den Abschnitt **CSP – Kunden, Bestellungen und Abonnements**. Wählen Sie in diesem Abschnitt **Problemtyp auswählen** und dann **Customer Services Credit Requests aus.**
5. Wählen Sie **auf der Seite** Empfohlene Lösungen unter Benötigen Sie weitere **Hilfe?** die Option **Ja aus.**
6. Füllen Sie **auf der** Seite Details den Abschnitt **Problemdetails** aus. Geben Sie **im** Textfeld Details die erforderlichen Informationen ein, [die](#required-information) Sie zuvor gesammelt haben.
7. Wählen Sie **Senden aus,** um Ihre SLA-Gutschriftanforderung zu senden.

## <a name="next-steps"></a>Nächste Schritte

- [Melden von Problemen im Auftrag Ihres Kunden](report-problems-on-behalf-of-a-customer.md)
