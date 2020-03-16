---
title: Umstellung von Kunden auf einen Azure-Plan | Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Ihre Kunden problemlos auf den Azure-Plan umstellen können.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 7bcb27e521e4f3982fd3e0a94f1ed3a96320cfa3
ms.sourcegitcommit: 45e80e92292d6618b7e73f56d70c85382e7bcc06
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2020
ms.locfileid: "79023486"
---
# <a name="transition-your-customers-to-azure-plan"></a>Umstellung Ihrer Kunden auf einen Azure-Plan

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

Indirekte Anbieter und direkte Abrechnungspartner können zur neuen Commerce-Benutzeroberfläche wechseln, die im Microsoft Cloud Service Provider (CSP)-Programm für Azure verfügbar ist. (Indirekte Wiederverkäufer müssen ihre indirekten Anbieter durchgehen.) Kunden bietet sich ein optimiertes Verfahren zum Kauf von Clouddiensten, gleich ob sie bei Partnern, bei Microsoft-Verkäufern oder direkt im Web kaufen.

Die Funktion zur Umstellung ist nur für Kunden verfügbar, die zur neuen E-Commerce-Benutzeroberfläche für Azure wechseln und einen Microsoft-Kundenvertrag unterzeichnet haben, nicht aber für andere Angebote in CSP, wie etwa Office 365 oder Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Umstellung vorhandener CSP-Angebote auf einen Azure-Plan

Sie können einen Kunden auf der neuen E-Commerce-Benutzeroberfläche im Partner Center von seinen vorhandenen CSP Azure-Angeboten auf Azure-Dienste im Rahmen des Azure-Plan umstellen. Dazu müssen der Partner und der Kunde im Partner Center eine Wiederverkäuferbeziehung eingerichtet haben, und der Kunde muss die Microsoft-Kundenvereinbarung unterzeichnet haben.

### <a name="select-transition-to-azure-plan"></a>Auswählen der Umstellung auf den Azure-Plan

1. Wählen Sie den Azure-Plan für Ihren Kunden aus.

2. Wählen Sie **Abrechnung auf Azure-Plan umstellen** aus.

![Umstellung](images/azure/transition1.png)

3. Wählen Sie **Weiter** aus.

![Umstellung](images/azure/transition2.png)

Ihr Kunde wird auf den Azure-Plan umgestellt.

**Im Umstellungsworkflow sind die erforderlichen Schritte automatisiert**:

- Kauf von Azure-Plänen
- Ein Plan pro Kunde in Direkt-CSP-Szenarien  
- Ein Plan pro Wiederverkäufer  

Nehmen wir an, ein Partner hat zwei Microsoft Azure-Angebote erworben und hat zwei verschiedene POR in den Kauf mit eingeschlossen. In diesem Fall kauft der Übergangsworkflow zwei Azure-Pläne (einen pro Wiederverkäufer) und ordnet automatisch die entsprechenden Azure-Abonnements den Azure-Plänen zu.  

**Zuordnen eines Azure-Abonnements zu einem Azure-Plan**

Nach Ihrem Kauf von Azure-Plänen ordnet Ihr System die vorhandenen Azure-Abonnements den Azure-Plänen zu. Der Fortschritt kann im Azure-Portal sowie im Partner Center angezeigt werden. 

4. Kehren Sie zu den Partner Center-**Abonnements** Ihres Kunden zurück, um seinen Budgetgrenzwert in der lokalen Währung des Kunden zu aktualisieren. 

![Umstellung](images/azure/transition3.png)

>[!NOTE]
>Das Budget, das Sie im Partner Center festgelegt haben, wird nicht in das Azure-Portal übertragen. Sie sollten das Budget und die Benachrichtigung auch im Azure-Portal festlegen.

Wenn Sie auf den Azure-Plan umstellen, können Sie für diesen Kunden keine Azure-Abonnements mehr kaufen. Sie erstellen die Abonnements unter dem Azure-Plan im Azure-Portal.

>[!NOTE]
> Alle Azure-Abonnements, die über die RBAC unter dem Azure-Plan erworben wurden, werden in der lokalen Währung abgerechnet. Die Wechselkurse werden nicht verwendet.

### <a name="track-your-transition-details"></a>Nachverfolgen der Umstellungsdetails

Folgen Sie dem Fortschritt der Umstellung im Azure-Portal sowie im Partner Center.

![Details anzeigen](images/azure/details1.png)

**Auswirkungen der Abrechnung auf Partner**

Wenn Sie einen Kunden von einem vorhandenen CSP Azure-Angebot umstellen, treten die folgenden Auswirkungen der Abrechnung auf:

- Bis zu dem Punkt, an dem das ursprüngliche CSP-Azure-Abonnement abgeschlossen ist, erfolgt die Abrechnung Ihrer gesamten Nutzung in Ihrer vorhandenen CSP-Rechnung.

- Wenn Sie über Administratorzugriffsrechte für das vorhandene CSP-Abonnement verfügten, haben Sie auch nach der Migration des Abonnements Zugriff.

Informationen zur Umstellung von direkten Enterprise-Verträgen auf CSP und Server- und Cloud-Registrierungen bei Azure-Diensten finden Sie unter [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](https://docs.microsoft.com/azure/billing/mpa-request-ownership) (Erwerb des Abrechnungsbesitzes von Azure-Abonnements für den Microsoft-Partnervertrag).

**Überwachungsprotokoll**:

Um die Abrechnung abzugleichen, müssen Sie nur den Verlauf der „Microsoft Azure“-Abonnements (0145P) auf der Seite **Abonnements** anzeigen. 

Das Abonnement „Microsoft Azure“ (0145P) setzt sich aus zwei Teilen zusammen:
1. Commerce-Abonnement 
2. Azure-Abonnement (Berechtigung)

Nach Abschluss der Umstellung wird das Azure-Abonnement unter den neuen Azure-Plan verschoben, und das Commerce-Abonnement wird angehalten, sodass keine weitere Nutzung gemeldet wird.  

>[Hinweis]\: Wenn das Microsoft Azure-Abonnement (0145P) in CSP erworben wird, weisen das Commerce-Abonnement und das Azure-Abonnement (Berechtigung) den gleichen Wert auf. Nur im Fall von Änderungen oder einer Übertragung des Abrechnungsbesitzes unterscheiden sich die Werte. 

**Probleme bei der Umstellung**

Bei Umstellungen sind keine Probleme zu erwarten. Wenn ein solcher auftritt, benachrichtigen wir Sie im Übergangsworkflow selbst. Es treten keine Störungen der Azure-Nutzung auf.  

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)

- [Vom Partner erworbenes Guthaben – Übersicht](partner-earned-credit.md)



