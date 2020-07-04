---
title: Berechnen der Gutschrift für den Partner
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie der Azure-Plan für Partner verdiente Gutschriften ("Partner verdiente Guthaben") berechnet wird. Dies schließt die Berechtigungsanforderungen für Partner und indirekte Anbieter ein.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 065cf0c8f95667b470081edcb1b66398235604b3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948137"
---
# <a name="how-partner-earned-credit-pec-is-calculated-for-partners-in-the-cloud-solution-provider-program"></a>Wie Partner Guthaben (PEC) für Partner im Cloud Solution Provider-Programm berechnet werden

**Geeignete Rollen**

- Globaler Administrator
- Abrechnungsadministrator

Partner, die die rund um die Uhr über die IT-Betriebsverwaltung von Teilen oder die gesamte Azure-Umgebung ihrer Kunden im CSP besitzen, werden mit PEC belohnt. Das PEC wird als Teil der Rechnung an den Partner über eine direkte abrechnungsbeziehung mit Microsoft bereitgestellt. Die Gutschrift wird täglich berechnet und in der monatlichen Rechnung widergespiegelt. Standardmäßig erhalten Partner in CSP die erforderlichen Zugriffsrechte für das Abonnement des Kunden, das es Ihnen ermöglicht, rund um die Uhr Betriebsverwaltung zu verfügen und die Ressourcen des Abonnements zu steuern. Weitere Möglichkeiten zum Bereitstellen von Zugriff für einen Transaktionspartner finden Sie im folgenden Abschnitt.


## <a name="important-eligibility-and-calculation-requirements"></a>Wichtige Anforderungen für die Eignung und Berechnung:

- Ein Partner sollte über eine aktive MPN-Vereinbarung und eine gültige regelbasierte Rolle für die Konto Steuerung (RBAC) verfügen, um eine Gutschrift für die von Ihnen verwalteten Azure-Ressourcen zu erhalten. Weitere Informationen zu [gültige RBAC-Rollen]

- Der indirekte Anbieter kann sich für die Verwaltung von Management Pack qualifizieren, wenn Sie oder der indirekte Händler über eine operative Kontrolle und Verwaltung der Azure-Ressourcen des Kunden in CSP verfügen.

- PEC ist der abgerechneten (kostenpflichtigen) Nutzung der Azure-Umgebung des Kunden in CSP zugeordnet, die vom Partner verwaltet wird. 

- PEC ist nur für Partner in CSP verfügbar, die von Microsoft (indirekter Anbieter und direkter Rechnungs Partner) abgerechnet werden.

- Berechtigte Dienste: die Gutschrift eines Partners ist für alle Azure-1-PP-Azure-Verbrauchs in der Preisliste anwendbar. Es gibt Ausnahmen, einschließlich, aber nicht beschränkt auf 3PP und Azure reservations.

- PEC wird täglich berechnet und kann in der täglichen Reconnaissance-Datei angezeigt werden. Ein Partner (Anbieter oder Reseller (über seinen Anbieter) muss für den ganzen Tag (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er die Leistung von PEC erhält.

- PEC wird bis hinab zur Azure-Ressourcenebene erworben. Wenn der Partner über einen gültigen Zugriff auf Abonnement-oder Ressourcengruppen Ebene verfügt, wird jede Ressource, die für die höhere Entität verwendet wird, mit dem Wert "PEC" erhalten. 

- PEC wird in die monatliche Rechnung des Partners eingeschlossen. Die Rechnung ist gebührenpflichtig. Die Details werden in der Datei "Rechnungs Reconnaissance" angezeigt.

Weitere Informationen zum Zugriff auf die Verwaltung von Azure-Abonnements und zum Verknüpfen ihrer MPN-ID mit RBAC-Rollen finden Sie [unter Verwalten von Abonnements und Ressourcen im Azure-Plan](azure-plan-manage.md).

Weitere Informationen finden Sie unter

- [Azure-Plan: Abrechnung](azure-plan-billing.md)

- [Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP ](azure-plan-price-list.md)