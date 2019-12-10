---
title: Anfordern einer SLA-Gutschrift von Microsoft | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Informieren Sie sich über die Vorteile, Einschränkungen und Verfahren zum Anfordern einer SLA-Gutschrift von Microsoft, wenn für Ihre Kunden ein Dienstausfall auftritt.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: bcc094b877d0128c73041044ce6304123d895fdb
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943143"
---
# <a name="request-an-sla-credit-from-microsoft"></a>Anfordern einer SLA-Gutschrift von Microsoft 

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
| Betriebssystem | Office-Abonnement |
| PB | Power BI für Office 365 |
| SP | SharePoint Online |
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
