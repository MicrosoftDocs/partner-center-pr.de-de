---
title: Beantragen einer SLA-Gutschrift bei Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Erfahren Sie mehr über die Vorteile, Einschränkungen und Verfahren zum Anfordern eines SLA-Guthabens (Service Level Agreement) von Microsoft, wenn bei Ihren Kunden ein Dienstausfall vorliegt.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 100a3d2988c19d57f7426c7212b7464d8e96dc94
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152952"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Anfordern eines SLA-Guthabens (Service Level Agreement) von Microsoft

**Geeignete Rollen:** Administrator-Agent-| Globaler Administrator

Sie können **SLA-Gutschriften (Service Level Agreement)** von Microsoft anfordern, wenn ein Dienst, den Sie für Ihre Kunden bereitstellen, einen Ausfall hat.

## <a name="sla-credit-calculation"></a>SLA-Kreditberechnung

SLA-Gutschriften von Microsoft werden basierend darauf bestimmt, welche Dienste betroffen waren. Wenn Ihr Kunde beispielsweise über eine Office 365-Suite verfügt, aber nur einen SharePoint-Ausfall aufgetreten ist, wird das SLA-Guthaben nur für SharePoint und nicht für den gesamten Plan des Kunden genehmigt.

*Guthaben werden basierend auf dem betroffenen Dienst und der Dauer des Ausfalls anteilsbasiert bewertet.* Informationen zu den Typen von Szenarien, die für SLA-Gutschriften qualifiziert sind, finden Sie im Dokument Konsolidierte SLA für [Onlinedienste.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Diese Informationen gelten auch für Dienste, die über das Cloud Solution Provider-Programm verkauft werden.


## <a name="request-an-sla-credit"></a>Anfordern eines SLA-Guthabens

*Der CSP-Partner (Cloud Solution Provider) muss den Anspruch und alle erforderlichen Informationen bis zum Ende des Kalendermonats übermitteln, der auf den Monat folgt, in dem der Vorfall aufgetreten ist.* Wenn der Vorfall beispielsweise am 15. Februar aufgetreten ist, muss Microsoft den Anspruch und alle erforderlichen Informationen bis zum 31. März erhalten. Endkunden und indirekte Vertriebspartner können keine SLA-Gutschriftansprüche übermitteln. entweder der indirekte Anbieter oder der Direktabrechnungspartner muss Ansprüche in ihrem Namen übermitteln.

>[!NOTE]
>Beratungsvorfälle[(Überprüfen Microsoft 365 Service Health)](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)sind nicht für SLA-Gutschriften berechtigt.

### <a name="required-information"></a>Erforderliche Informationen

Kundenname, Mandanten-ID, Partnerticket# und datums-/zeitstempelerstellende Tickets reichen nicht aus, damit ein Anspruch verarbeitet werden kann.

Bevor Sie [eine SLA-Gutschriftanforderung](#submit-sla-credit-request) an Microsoft übermitteln, müssen Sie **alle** folgenden Informationen sammeln, die In Ihr Supportticket aufgenommen werden sollen:

- GUID des Kundenmandanten
- Der [Incidentbezeichner](#outage-incident-identifier)für den Ausfall ?
- Der Nachweis, dass der Kunde von dem Ausfall abgefragt wurde und eine SLA-Gutschrift angefordert hat.
- Wurden die über CSP erworbenen Abonnements von den Auswirkungen? (*Ja* oder *Nein*)

#### <a name="evidence-that-proves-customer-impact"></a>Beweise, die auswirkungen auf Kunden belegen

- Informationen zu Zeit und Dauer der Ausfallzeit
- Anzahl und Speicherort der betroffenen Benutzer (falls zutreffend)
- Beschreibungen Ihrer Versuche, den Incident zum Zeitpunkt des Auftretens zu beheben
- Eine E-Mail des kundenspezifischen Kunden, der Support anklangt, und anschließend eine Gutschrift
- Die Nummer des Supporttickets und details des Kundenkontakts in Bezug auf die Lösung der Auswirkungen auf den Dienst


#### <a name="outage-incident-identifier"></a>Id des Incidents "Ausfall"

Sie finden den Bezeichner für den Ausfallfall auf **Service Health** Seite im Microsoft 365 Admin Center. Die **Incident-ID** für Den Ausfall ist eine Zahl, der eine zweibuchstabende Abkürzung voran steht, die den betroffenen Dienst angibt (z. B. *EX25194* für einen Exchange Online-Ausfall). In der folgenden Tabelle werden allgemeine Dienstabkürzungen beschrieben:

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

### <a name="submit-sla-credit-request"></a>Senden einer SLA-Gutschriftanforderung

So übermitteln Sie Ihre SLA-Gutschriftanforderung über das Partner Center-Dashboard an Microsoft:

1. Melden Sie sich beim Partner Center-Dashboard an.
2. Wählen Sie im Menü auf der linken Seite **service requests (Dienstanforderungen)** und dann **Partner support requests (Partnersupportanfragen) aus.**
3. Wählen Sie auf der Seite **Partneranforderung** die Option **Neue Anforderung** aus.
4. Suchen **Sie** auf der Seite Anforderung starten den Abschnitt **CSP – Kunden, Bestellungen und Abonnements.** Wählen Sie in diesem Abschnitt **Problemtyp auswählen** und dann **Kundendienstguthabenanforderungen** aus.
5. Wählen Sie auf der Seite **Empfohlene Lösungen** unter Benötigen Sie **weitere Hilfe?** die Option **Ja** aus.
6. Füllen Sie auf der Seite **Details** den Abschnitt **Problemdetails** aus. Geben Sie im Textfeld **Details** die [erforderlichen Informationen](#required-information) ein, die Sie zuvor gesammelt haben.
7. Wählen Sie **Senden** aus, um Ihre SLA-Gutschriftanforderung zu senden.

## <a name="next-steps"></a>Nächste Schritte

- [Melden von Problemen im Auftrag Ihres Kunden](report-problems-on-behalf-of-a-customer.md)
