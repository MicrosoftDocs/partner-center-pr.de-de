---
title: Beantragen einer SLA-Gutschrift bei Microsoft
ms.topic: article
ms.date: 04/28/2020
description: Informieren Sie sich über die Vorteile, Einschränkungen und Verfahren zum Anfordern einer Vereinbarung zum Service Level (Service Level Agreement, SLA) von Microsoft, wenn für Ihre Kunden ein Dienstausfall auftritt.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 27a444bc5f923b1d2ad18bfe47cf70b365751e42
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992009"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Wie und wann sollte eine Vereinbarung zum Service Level (Service Level Agreement, SLA) von Microsoft angefordert werden?

Sie sind in der Lage, **Vereinbarung zum Service Level (Service Level Agreement, SLA)** von Microsoft anzufordern, wenn ein Dienst, den Sie für Ihre Kunden bereitstellen, einen Ausfall aufweist.

## <a name="sla-credit-calculation"></a>SLA-Bonitäts Berechnung

SLA-Gutschriften von Microsoft werden basierend auf dem betroffenen Dienst bestimmt. Wenn Ihr Kunde beispielsweise eine Office 365 Suite hat, aber nur einen SharePoint-Ausfall erlebt hat, wird die SLA-Gutschrift nur für SharePoint und nicht für den gesamten Plan des Kunden genehmigt.

*Gutschriften werden basierend auf dem betroffenen Dienst und der Dauer des Ausfalls anteilig bewertet.* Informationen zu den Arten von Szenarien, die sich auf SLA-Gutschriften qualifizieren, finden Sie im Dokument zu den [konsolidierten SLA für Online Services](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Diese Informationen gelten auch für Dienste, die über das Cloud Solution Provider-Programm verkauft wurden.

## <a name="request-an-sla-credit"></a>Anfordern einer SLA-Gutschrift

*Der CSP-Partner (Cloud Solution Provider) muss den Anspruch und alle erforderlichen Informationen am Ende des Kalendermonats nach dem Monat, in dem der Vorfall aufgetreten ist, übermitteln.* Wenn der Incident z. b. am 15. Februar aufgetreten ist, muss Microsoft den Anspruch und alle erforderlichen Informationen bis zum 31. März erhalten. Endkunden und indirekte Vertriebspartner können keine SLA-Kredit Ansprüche einreichen. der indirekte Anbieter oder der direkte Rechnungs Partner muss Ansprüche in seinem Auftrag übermitteln.

### <a name="required-information"></a>Erforderliche Informationen

Bevor Sie [eine SLA-Kreditanfrage](#submit-sla-credit-request) an Microsoft senden, müssen Sie die folgenden Informationen sammeln, die in Ihr Support Ticket aufgenommen werden sollen:

- Die GUID des Kunden Mandanten
- Der [Bezeichner des Ausfall Vorfalls](#outage-incident-identifier)?
- Waren die betroffenen Abonnements über CSP erworben? (*Ja* oder *Nein*)

#### <a name="outage-incident-identifier"></a>ID des Ausfall Vorfalls

Sie finden den Bezeichner für den Ausfall des Ausfalls auf der Seite **Service Health** im Microsoft 365 Admin Center. Die **Incident-ID des Ausfalls** ist eine Zahl, der eine zwei buchstabige Abkürzung vorangestellt ist, die den betroffenen Dienst (z. b. *EX25194* für einen Exchange Online-Ausfall) angibt. In der folgenden Tabelle werden häufige Dienst Abkürzungen beschrieben:

| Abkürzung mit zwei Buchstaben | Microsoft-Dienst |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online-Schutz |
| SB | Skype for Business Online (früher lync Online) |
| OS | Office-Abonnement |
| PB | Power BI für Office 365 |
| SP | SharePoint Online |
| D | Yammer Enterprise |
| MO | Portal Fehler |

### <a name="submit-sla-credit-request"></a>SLA-Kreditanfrage senden

So übermitteln Sie Ihre SLA-Kreditanfrage an Microsoft über das Partner Center-Dashboard:

1. Melden Sie sich beim Partner Center-Dashboard an.
2. Wählen Sie im Menü auf der linken Seite **Service Requests**aus, und wählen Sie dann **Partner Supportanfragen**aus.
3. Wählen Sie auf der Seite **Partner Anforderung** die Option **neue Anforderung**aus.
4. Suchen Sie auf der Seite **Anforderung starten** den Abschnitt **CSP-Kunden, Bestellungen und Abonnements**. Wählen Sie in diesem Abschnitt **Problemtyp auswählen**aus, und wählen Sie dann **Kundendienst-Kreditanfragen**aus.
5. Wählen Sie auf der Seite **Empfohlene Lösungen** unter **benötigen Sie weitere Hilfe?** die Option **Ja**aus.
6. Füllen Sie auf der Seite **Details** den Abschnitt **Problem Details** aus. Geben Sie im Textfeld **Details** die [erforderlichen Informationen](#required-information) ein, die Sie zuvor gesammelt haben.
7. Wählen **Sie senden aus** , um Ihre SLA-Kreditanfrage zu senden.
