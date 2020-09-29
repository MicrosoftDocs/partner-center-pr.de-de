---
title: Übertragen eines Azure-Abonnements im Azure-Plan auf einen anderen CSP-Partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie den Programmpartner von Cloud Solution Provider ändern, der mit den Azure-Abonnements eines Kunden in einem Azure-Plan verknüpft ist.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e1b70f26dc146507ac3764ae223ca27915162f0c
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422568"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Übertragen der Azure-Plan Abonnements eines Kunden an einen anderen Partner

## <a name="applies-to"></a>Gilt für:

- Partner im CSP-Programm (Cloud Solution Provider)

In diesem Artikel wird beschrieben, wie ein Kunde seine Azure-Abonnements in einem Azure-Plan von einem Cloud Solution Provider (CSP) zu einem anderen wechseln kann.

Um die Azure-Abonnements eines Kunden von einem anderen Partner zu wechseln, führen Sie die folgenden Schritte aus. Sowohl der Partner als auch der Kunde müssen die erforderlichen Schritte ausführen.

>[!Note]  
>Nur Partner mit einer direkten abrechnungsbeziehung mit Microsoft können auf die Übergangs Tools zugreifen. Indirekte Reseller müssen mit ihren indirekten Anbietern zusammenarbeiten, um dieses Übergangs Tool nutzen zu können.

Der Kunde muss sich in der Konversation mit beiden Partnern (Current und Future) befinden, bevor dieses Tool genutzt wird. Eine Offline Konversation muss durchgeführt werden, um Verwirrung und Abwanderung zu vermeiden. Außerdem sollten Partner und Kunden diese Überlegungen und Voraussetzungen vor dem Initiieren eines Übergangs verstehen:

**Wichtige Überlegungen:**

- Azure reservations wird nicht mit dem Abonnement an den zukünftigen Partner verschoben
- CSP-Preise für Azure-Dienste unter dem aktuellen Partner werden nicht übertragen  
- Support Aufgaben für Kunden werden auf den zukünftigen Partner verschoben
- Abrechnung und Rechnungsstellung werden zum Zeitpunkt der Übertragung auf den zukünftigen Partner verschoben
- Die rollenbasierte Access Control in Azure (RBAC) ist von der Übertragung nicht betroffen.
- Administrator im Auftrag von (Aobo) wird dem zukünftigen Partner standardmäßig nicht gewährt.
- Marketplace-Produkte von Drittanbietern werden übertragen, solange die Produkte die Marketplace-Berechtigungsüberprüfung bestehen.
    - Es gibt keine besonderen Rabatte oder regionalen Einschränkungen.
    - Die Produkte sind nicht Abonnement basiert.
    - Der zukünftige Partner sollte mit dem Verleger zusammenarbeiten, um sicherzustellen, dass er für die Bereitstellung des Produkts in der Zulassungsliste enthalten ist.
    - Wenn nicht alle diese Bedingungen erfüllt sind, um die Marketplace-Produkte zu übertragen, sollten Sie abgebrochen werden, die Azure-Abonnements übertragen und dann mit dem neuen Partner Marketplace-Produkte erneut erwerben.

**Voraussetzungen:**

- Der Kunde nimmt den aktuellen CSP-Partner an seine Absicht für den Übergang
- Zukünftiger CSP-Partner arbeitet mit Kunden zusammen, um sicherzustellen, dass Kundenanforderungen erfüllt werden können
- Zukünftiger CSP-Partner stellt vor Beginn des Übergangs eine Beziehung mit dem Kunden her  
- Kunde muss den Microsoft-Kundenvertrag mit dem zukünftigen CSP-Partner Signieren
- Der spätere CSP-Partner muss den Microsoft-Partnervertrag zur Verwendung dieses Tools signiert haben.

## <a name="customer-tasks-to-be-completed"></a>Kunden Aufgaben, die abgeschlossen werden müssen

Um ein Azure-Abonnement unter einem Azure-Plan zu übertragen, muss der Kunde den Prozess starten, indem er sich an den aktuellen Partner wenden. Sie sollten den Firmennamen und die Domäne Ihres aktuellen Partners erfassen, damit Ihr zukünftiger Partner das Übertragungs Anforderungs Formular in seinem Namen ausfüllen kann.

Der Kunde muss auch die Abonnements ermitteln, die er vom aktuellen Partner übertragen möchten. Partner für Office 365-, Enterprise Mobility Suite-oder Microsoft Dynamics CRM-Abonnements können nicht geändert werden.

>[!Note]  
>Es ist Aufgabe des zukünftigen Partners, das Übertragungs Anforderungs Formular abzuschließen, das den Übertragungsvorgang initiiert. Microsoft kann nicht im Auftrag des Kunden oder des aktuellen Partners eingreifen. Der Kunde sollte planen, eng mit Ihrem zukünftigen und aktuellen Partner zusammenzuarbeiten, damit der Übergang reibungslos verläuft.

## <a name="future-partner-tasks-to-be-completed"></a>Zukünftige Partner Aufgaben, die abgeschlossen werden müssen

Der zukünftige Partner des Abonnements muss ein Übertragungs Anforderungs Formular von Partner Center abschließen, um eine Abonnement Übertragung anzufordern:

1.  Wählen Sie im Partner Center-Menü **Kunden**aus, und wählen Sie dann den Kunden aus, für den Sie ein Übertragungs Anforderungs Formular im Auftrag von ausführen möchten.
2.  Wählen Sie im Menü Kunde die Option **Abonnements**aus.
3.  Wählen Sie den Abschnitt **Übertragungs Anforderung** aus.
4.  Wählen Sie im **Abschnitt Übertragungs Anforderung**die Option **neue Anforderung hinzufügen**aus.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Abschnitt Übertragungen":::

5.  Vervollständigen Sie das Formular für **neue Übertragungsanforderungen** .

6.  Wählen Sie Sende **Übertragungs Anforderung**  >  **senden**aus.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formular zum Vervollständigen der Übertragungs Anforderung":::

7.  Bestätigung der Übertragungs Anforderung überprüfen

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Ausstehende Übertragung überprüfen":::

    >[!Note]
    >Der zukünftige Partner kann die Übertragungs Anforderung abbrechen, indem er in der oberen rechten Ecke nur **Anforderung abbrechen** auswählt, wenn der Übertragungs Anforderungs Status "Ausstehend" lautet. Wenn der Übertragungs Anforderungs Status "in Bearbeitung" oder "abgeschlossen" lautet, sind keine Abbrüche möglich.

## <a name="current-partner-tasks-to-be-completed"></a>Aktuelle Partner Aufgaben, die abgeschlossen werden müssen

Der Administrator-Agent des aktuellen Partners des Kunden erhält eine e-Mail, dass der Kunde eine Übertragung der Abonnements anfordert:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Überprüfung":::

Überprüfen und akzeptieren Sie das Übertragungs Anforderungs Formular von Partner Center, um die Abonnement Übertragung abzuschließen.

>[!Note]  
>Wenn der aktuelle Partner innerhalb von 30 Tagen keine Aktion durchführt, läuft die Anforderung ab, und der zukünftige Partner erhält eine, um eine neue Übertragungs Anforderung zu erstellen.

1.  Wählen Sie über **Prüfen der Übertragungs Anforderung** per e-Mail oder
1.  Wählen Sie im Partner Center-Menü **Kunden**aus, und wählen Sie dann den Kunden aus, für den eine Übertragungs Anforderung übermittelt wurde.
2.  Wählen Sie im Menü Kunde die Option **Abonnements**aus.
3.  Wählen Sie den Abschnitt **Übertragungs Anforderung** aus.
4.  Erweitern Sie Übertragungs Informationen, indem Sie die ausgewählte **Übertragungs Anforderungs-ID** unter **empfangene Anforderungen** auswählen.

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Übertragungs Anforderung für Quell Reviews":::

5.  Überprüfen Sie die Übertragungs Anforderung. Wählen Sie die angeforderten zu übertragenden Azure-Abonnements aus.

>[!Note]  
> Beachten Sie, dass Sie nicht mehr auf die ausgewählten Abonnements zugreifen können, bevor Sie fortfahren.
> Sie werden nicht für die weitere Verwendung in Rechnung gestellt.
> Azure-Reservierungen werden nicht mit den Abonnements übertragen.

6.  Wählen Sie dann **akzeptieren und übertragen** aus, um den Übertragungsvorgang abzuschließen.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Auswählen von Abonnements, die in ihren Azure-Plänen übertragen werden sollen":::

7.  Bestätigung der Übertragungs Annahme anzeigen.

   An diesem Punkt werden der zukünftige Partner, der Kunde und der aktuelle Partner über die akzeptierte Übertragungs Anforderung per e-Mail benachrichtigt.

   Nachdem der Übergang akzeptiert wurde, bleibt der Übertragungs Status möglicherweise bis zu 15 Minuten ausstehend, während das System aktualisiert wird. Wenn es länger dauert, versucht das System, drei Tage lang einen Versuch zu durchführen. Wenn der Übertragungs Status weiterhin aussteht, sollte der Partner eine Service Request übermitteln.

   Nach Abschluss der Übertragung werden die in der Anforderung enthaltenen Abonnements im Azure-Plan des zukünftigen Partners angezeigt, und Sie werden nicht mehr mit Ihnen aufgelistet.

>[!Note]  
>Für indirekte Anbieter: informieren Sie den indirekten Händler, dass die Übertragungs Anforderung akzeptiert wurde.

### <a name="managing-your-transferred-customer-subscriptions"></a>Verwalten Ihrer übertragenen Kunden Abonnements
- Der Zugriff auf vorhandene Benutzer, Gruppen oder Dienstprinzipale, die per rollenbasierter Azure-Zugriffssteuerung (Azure Role-Based Access Control, Azure RBAC) zugewiesen wurden, ist von der Übertragung nicht betroffen. Mit der rollenbasierten Zugriffs Steuerung von Azure [(Azure RBAC)](/azure/role-based-access-control/overview) kann Ihr Kunde steuern, wer Zugriff auf Azure-Ressourcen hat, welche Möglichkeiten Sie mit diesen Ressourcen haben und auf welche Bereiche Sie zugreifen können. Als neuer Partner erhalten Sie nach der Abonnement Übertragung keinen RBAC-Zugriff auf die Ressourcen Ihres Kunden. Der vorherige Partner Ihres Kunden behält seinen RBAC-Zugriff bei. Wenden Sie sich an Ihren Kunden, um zu verstehen, wer Einblicke in seine Abonnements hat und wie Sie alle gewünschten Änderungen vornehmen können.

- Folglich ist es wichtig, dass Ihr Kunde den Azure RBAC-Zugriff für den vorherigen Partner entfernt und den neuen Partner für den neuen Partner zugreift. Weitere Informationen zu Ihrem Kunden, der neuen Zugriff gewährt, finden Sie unter [Was ist die rollenbasierte Zugriffs Steuerung in Azure (Azure RBAC)?](/azure/role-based-access-control/overview) Weitere Informationen über den Kunden, der den RBAC-Zugriff ihres früheren Partners entfernt, finden Sie unter [Entfernen einer Rollenzuweisung](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Außerdem erhalten Sie keinen automatischen [Administrator im Auftrag von (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) -Zugriff auf Ihre Abonnements. Aobo ist erforderlich, damit Partner die Azure-Abonnements Ihres Kunden in Ihrem Namen verwalten können. Weitere Informationen zu Azure-Berechtigungen finden [Sie unter Abrufen von Berechtigungen zum Verwalten eines Kunden Dienstanbieter oder Abonnements.](/partner-center/customers-revoke-admin-privileges)

## <a name="next-steps"></a>Nächste Schritte:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Abrufen der Berechtigungen zum Verwalten des Dienstanbieter oder Abonnements eines Kunden.](/partner-center/customers-revoke-admin-privileges)