---
title: Übertragen eines Azure-Abonnements unter einem Azure-Plan an einen anderen CSP-Partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie Sie den Cloud Solution Provider Programmpartner ändern, der den Azure-Abonnements eines Kunden unter einem Azure-Plan zugeordnet ist.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856048"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Übertragen von Azure-Planabonnements eines Kunden an einen anderen Partner

**Geeignete Rollen:** Kontoadministrator-| Sales agent | Abrechnungs-Agent

In diesem Artikel wird beschrieben, wie ein Kunde seine Azure-Abonnements unter einem Azure-Plan von einem Cloud Solution Provider (CSP) in einen anderen umschalten kann.

Führen Sie die folgenden Schritte aus, um die Azure-Abonnements eines Kunden von einem anderen Partner zu wechseln. Sowohl der Partner als auch der Kunde müssen schritte ausführen.

>[!Note]  
>Nur Partner mit direkter Abrechnungsbeziehung mit Microsoft können auf die Umstellungstools zugreifen. Indirekte Wiederverkäufer müssen mit ihren indirekten Anbietern zusammenarbeiten, um dieses Übergangstool zu nutzen.

Der Kunde muss mit beiden Partnern (aktuell und zukünftig) im Gespräch sein, bevor dieses Tool genutzt wird. Eine Offline-Konversation muss ausgeführt werden, um Verwirrung und Abwanderung zu vermeiden. Darüber hinaus sollten Partner und Kunden diese Überlegungen und Voraussetzungen kennen, bevor sie einen Übergang initiieren:

**Wichtige Überlegungen:**

- Azure-Reservierungen werden nicht mit dem Abonnement zum zukünftigen Partner umziehen.
- CSP-Preise für Azure-Dienste unter dem aktuellen Partner werden nicht umstiegen  
- Supportaufgaben für Den Kunden werden zu zukünftigen Partnern wechseln
- Abrechnung und Rechnungsstellung werden zum Zeitpunkt der Übertragung an den zukünftigen Partner übertragen.
- Azure Role-Based Access Control (RBAC) ist von der Übertragung nicht betroffen.
- Der Administrator im Auftrag von (AOBO) wird dem zukünftigen Partner nicht standardmäßig gewährt.
- Marketplace-Produkte von Drittanbietern werden übertragen, solange die Produkte die Marketplace-Berechtigungsprüfung bestehen.
    - Es gibt keine besonderen Rabatte oder regionalen Einschränkungen.
    - Die Produkte sind nicht abonnementbasiert.
    - Der zukünftige Partner sollte mit dem Herausgeber zusammenarbeiten, um sicherzustellen, dass er sich in der Liste mit den Zulässigen für die Bereitstellung des Produkts befindet.
    - Wenn nicht alle diese Bedingungen erfüllt sind, um die Marketplace-Produkte zu übertragen, sollten sie storniert, die Azure-Abonnements übertragen und dann marketplace-Produkte mit dem neuen Partner erneut erworben werden.

**Voraussetzungen:**

- Der Kunde betreibt den aktuellen CSP-Partner bei seiner Absicht, zu übergehen.
- Zukünftiger CSP-Partner arbeitet mit Kunden zusammen, um sicherzustellen, dass die Kundenanforderungen erfüllt werden können.
- Zukünftiger CSP-Partner richtet eine Beziehung mit dem Kunden ein und erwirbt einen Azure-Plan, bevor der Übergang beginnt.  
- Kunde muss Microsoft-Kundenvereinbarung mit zukünftigem CSP-Partner signieren
- Der zukünftige CSP-Partner muss die Microsoft Partner-Vereinbarung signiert haben, um dieses Tool verwenden zu können.

## <a name="customer-tasks-to-be-completed"></a>Auszuführende Kundenaufgaben

Um ein Azure-Abonnement unter einem Azure-Plan zu übertragen, muss der Kunde den Prozess starten, indem er sich an den aktuellen Partner wendet. Sie sollten den Firmennamen und die Domäne ihres aktuellen Partners erfassen, damit der zukünftige Partner das Formular für die Übertragungsanforderung in ihrem Namen ausfüllen kann.

Der Kunde muss auch die Abonnements identifizieren, die er vom aktuellen Partner übertragen möchte. Partner für Office 365-, Enterprise Mobility Suite- oder Microsoft Dynamics CRM-Abonnements können nicht geändert werden.

>[!Note]  
>Es liegt in der Verantwortung des zukünftigen Partners, das Formular für die Übertragungsanforderung auszufüllen, das den Übertragungsvorgang initiiert. Microsoft kann nicht im Auftrag des Kunden oder des aktuellen Partners eingreifen. Der Kunde sollte planen, eng mit dem zukünftigen und aktuellen Partner zusammenzuarbeiten, damit der Übergang reibungslos verläuft.

## <a name="future-partner-tasks-to-be-completed"></a>Zukünftige Partneraufgaben, die abgeschlossen werden sollen

Der zukünftige Partner des Abonnements muss ein Übertragungsanforderungsformular von Partner Center ausfüllen, um eine Abonnementübertragung anzufordern:

1.  Wählen Sie im menü Partner Center die Option **Kunden** und dann den Kunden aus, für den Sie ein Formular für eine Übertragungsanforderung ausfüllen möchten.
2.  Wählen Sie im Menü Kunde die Option **Abonnements** aus.
3.  Wählen Sie den **Abschnitt Übertragungsanforderung** aus.
4.  Wählen Sie **im Abschnitt Übertragungsanforderung** die Option **Neue Anforderung hinzufügen aus.**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Abschnitt &quot;Übertragungen&quot;":::

5.  Füllen Sie das **Formular Neue Übertragungsanforderung** aus.

6.  Wählen Sie **Übertragungsanforderung**  >  **senden Senden aus.**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formular &quot;Übertragungsanforderung abschließen&quot;":::

7.  Überprüfen der Bestätigung der Übertragungsanforderung

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Überprüfen der ausstehenden Übertragung":::

    >[!Note]
    >Der zukünftige Partner kann die Übertragungsanforderung nur dann abbrechen, wenn der Status der Übertragungsanforderung "Ausstehend" ist.  Sobald der Status der Übertragungsanforderung "In Bearbeitung" oder "Abgeschlossen" ist, sind Abbruche nicht mehr möglich.

## <a name="current-partner-tasks-to-be-completed"></a>Aktuelle Partneraufgaben, die abgeschlossen werden sollen

Der Administrator-Agent des aktuellen Partners des Kunden erhält eine E-Mail, dass der Kunde eine Übertragung seiner Abonnements an fordert:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Überprüfung":::

Überprüfen und akzeptieren Sie das Formular für die Übertragungsanforderung Partner Center, um die Abonnementübertragung abschließen zu können.

>[!Note]  
>Wenn der aktuelle Partner innerhalb von 30 Tagen keine Aktion ergriffen hat, läuft die Anforderung ab, und der zukünftige Partner hat eine , um eine neue Übertragungsanforderung zu erstellen.

1.  Wählen Sie **in der E-Mail die Option** Übertragungsanforderung überprüfen oder aus.
1.  Wählen Sie Partner Center Menü Kunden aus, und wählen Sie dann den Kunden aus, für den eine Übertragungsanforderung übermittelt wurde.
2.  Wählen Sie im Menü Kunde die Option **Abonnements aus.**
3.  Wählen Sie den **Abschnitt Übertragungsanforderung** aus.
4.  Erweitern Sie Übertragungsinformationen, indem Sie unter Empfangene Anforderungen die ausgewählte **Übertragungsanforderungs-ID** **auswählen.**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Übertragungsanforderung für Quellüberprüfungen":::

5.  Überprüfen Sie die Übertragungsanforderung. Wählen Sie die angeforderten Azure-Abonnements aus, die übertragen werden sollen.

>[!Note]  
> Bevor Sie fortfahren, beachten Sie Folgendes: Sie haben keinen Zugriff mehr auf die ausgewählten Abonnements.
> Die weitere Nutzung wird Ihnen nicht in Rechnung stellen.
> Azure-Reservierungen werden nicht mit den Abonnements übertragen.

6.  Wählen Sie dann **Akzeptieren und übertragen** aus, um den Übertragungsvorgang abzuschließen.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Auswählen von Abonnements, die unter Ihren Azure-Plänen übertragen werden sollen":::

7.  Anzeigen der Bestätigung der Übertragungsakzeptanz.

   An diesem Punkt werden der zukünftige Partner, der Kunde und der aktuelle Partner per E-Mail über die akzeptierte Übertragungsanforderung benachrichtigt.

   Nachdem der Übergang akzeptiert wurde, kann der Übertragungsstatus bis zu 15 Minuten lang ausstehend bleiben, während das System aktualisiert wird. Wenn es länger dauert, versucht das System drei Tage lang weiter. Wenn der Übertragungsstatus weiterhin Ausstehend bleibt, sollte der Partner eine Serviceanfrage senden.

   Sobald die Übertragung abgeschlossen ist, werden die in der Anforderung enthaltenen Abonnements im Azure-Plan des zukünftigen Partners angezeigt und nicht mehr bei Ihnen aufgeführt.

>[!Note]  
>Für indirekte Anbieter: Informieren Sie Ihren indirekten Handelspartner, dass die Übertragungsanforderung akzeptiert wurde.

### <a name="managing-your-transferred-customer-subscriptions"></a>Verwalten Ihrer übertragenen Kundenabonnements

- Der Zugriff auf vorhandene Benutzer, Gruppen oder Dienstprinzipale, die per rollenbasierter Azure-Zugriffssteuerung (Azure Role-Based Access Control, Azure RBAC) zugewiesen wurden, ist von der Übertragung nicht betroffen. Die rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, [Azure RBAC)](/azure/role-based-access-control/overview) unterstützt Ihren Kunden bei der Verwaltung, wer Zugriff auf Azure-Ressourcen hat, was er mit diesen Ressourcen tun kann und auf welche Bereiche er Zugriff hat. Als neuer Partner erhalten Sie nach der Abonnementübertragung keinen RBAC-Zugriff auf die Ressourcen Ihres Kunden. Der vorherige Partner Ihres Kunden behält seinen RBAC-Zugriff bei. Arbeiten Sie mit Ihrem Kunden zusammen, um zu verstehen, wer Einblicke in seine Abonnements hat und wie sie gewünschte Änderungen vornehmen können.

- Daher ist es wichtig, dass Ihr Kunde den Azure RBAC-Zugriff für seinen vorherigen Partner entfernt und den Zugriff für den neuen Partner hinzufüge. Weitere Informationen dazu, wie Ihr Kunde neuen Zugriff bietet, finden Sie unter Was [ist die rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, Azure RBAC)?](/azure/role-based-access-control/overview) Weitere Informationen dazu, wie Ihr Kunde den RBAC-Zugriff Ihres vorherigen Partners entfernt, finden Sie unter [Entfernen einer Rollenzuweisung.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

- Darüber hinaus erhalten Sie nicht automatisch [AOBO-Zugriff (Admin on Behalf Of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) auf Ihre Abonnements. AOBO ist erforderlich, damit Partner die Azure-Abonnements ihrer Kunden in ihrem Namen verwalten können. Weitere Informationen zu Azure-Berechtigungen finden Sie unter Abrufen von Berechtigungen zum Verwalten des Diensts [oder Abonnements eines Kunden.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Nächste Schritte:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Erhalten Sie Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden.](./customers-revoke-admin-privileges.md)
