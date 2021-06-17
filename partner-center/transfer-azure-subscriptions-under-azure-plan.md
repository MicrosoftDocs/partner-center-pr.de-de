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
ms.openlocfilehash: 092c76fb874eb7308bdb69503223f722657db957
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277316"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Übertragen von Azure-Planabonnements eines Kunden an einen anderen Partner

**Geeignete Rollen:** Kontoadministrator-| | des Vertriebsmitarbeiters Abrechnungs-Agent

In diesem Artikel wird beschrieben, wie ein Kunde seine Azure-Abonnements unter einem Azure-Plan von einem Cloud Solution Provider (CSP) auf einen anderen umstellen kann.

Führen Sie die folgenden Schritte aus, um die Azure-Abonnements eines Kunden von einem anderen Partner zu wechseln. Sowohl der Partner als auch der Kunde müssen schritte ausführen.

>[!Note]  
>Nur Partner mit einer direkten Abrechnungsbeziehung mit Microsoft können auf die Übergangstools zugreifen. Indirekte Vertriebspartner müssen mit ihren indirekten Anbietern zusammenarbeiten, um dieses Übergangstool nutzen zu können.

Der Kunde muss sich mit beiden Partnern (aktuell und zukünftig) in Verbindung setzen, bevor dieses Tool genutzt wird. Eine Offlinekonversation muss erforderlich sein, um Verwirrung und Abwanderung zu vermeiden. Darüber hinaus sollten Partner und Kunden diese Überlegungen und Voraussetzungen verstehen, bevor sie einen Übergang initiieren:

**Wichtige Überlegungen:**

- Azure-Reservierungen werden nicht mit dem Abonnement zu einem zukünftigen Partner verschoben
- CSP-Preise für Azure-Dienste unter dem aktuellen Partner werden nicht umgestellt  
- Supportaufgaben für Kunden werden an zukünftige Partner übertragen
- Abrechnung und Rechnungsstellung werden zum Zeitpunkt der Übertragung an den zukünftigen Partner verschoben.
- Azure Role-Based Access Control (RBAC) ist von der Übertragung nicht betroffen
- Administrator im Auftrag von (Admin on Behalf Of, AOBO) wird dem zukünftigen Partner nicht standardmäßig gewährt.
- Marketplace-Produkte von Drittanbietern werden übertragen, solange die Produkte die Überprüfung der Marketplace-Berechtigung bestehen.
    - Es gibt keine speziellen Rabatte oder regionalen Einschränkungen.
    - Die Produkte sind nicht abonnementbasiert.
    - Der zukünftige Partner sollte mit dem Herausgeber zusammenarbeiten, um sicherzustellen, dass er sich in der Liste mit den Zulässigen für die Bereitstellung des Produkts befindet.
    - Wenn nicht alle diese Bedingungen erfüllt sind, um die Marketplace-Produkte zu übertragen, sollten sie storniert, die Azure-Abonnements übertragen und dann marketplace-Produkte mit dem neuen Partner erneut erworben werden.

**Voraussetzungen:**

- Der Kunde betreibt den aktuellen CSP-Partner bei der Absicht des Übergangs.
- Zukünftiger CSP-Partner arbeitet mit kundenspezifischen Kunden zusammen, um sicherzustellen, dass die Kundenanforderungen erfüllt werden können.
- Zukünftiger CSP-Partner stellt eine Beziehung mit dem Kunden her und erwirbt einen Azure-Plan, bevor der Übergang beginnt.  
- Kunde muss Microsoft-Kundenvereinbarung mit zukünftigem CSP-Partner signieren
- Zukünftiger CSP-Partner muss die Microsoft Partner-Vereinbarung signiert haben, um dieses Tool verwenden zu können.

## <a name="customer-tasks-to-be-completed"></a>Auszuführende Kundenaufgaben

Um ein Azure-Abonnement unter einem Azure-Plan zu übertragen, muss der Kunde den Prozess starten, indem er sich an den aktuellen Partner wendet. Sie sollten den Firmennamen und die Domäne ihres aktuellen Partners erfassen, damit der zukünftige Partner das Formular für die Übertragungsanforderung in ihrem Namen ausfüllen kann.

Der Kunde muss auch die Abonnements identifizieren, die er vom aktuellen Partner übertragen möchte. Partner für Office 365-, Enterprise Mobility Suite- oder Microsoft Dynamics CRM-Abonnements können nicht geändert werden.

>[!Note]  
>Es liegt in der Verantwortung des zukünftigen Partners, das Formular für die Übertragungsanforderung auszufüllen, das den Übertragungsvorgang initiiert. Microsoft kann nicht im Auftrag des Kunden oder des aktuellen Partners eingreifen. Der Kunde sollte planen, eng mit dem zukünftigen und aktuellen Partner zusammenzuarbeiten, damit der Übergang reibungslos verläuft.

## <a name="future-partner-tasks-to-be-completed"></a>Zukünftige Partneraufgaben, die abgeschlossen werden sollen

Der zukünftige Partner des Abonnements muss ein Übertragungsanforderungsformular von Partner Center ausfüllen, um eine Abonnementübertragung anzufordern:

1.  **Wählen** Sie im Menü Partner Center kunden und dann den Kunden aus, für den Sie ein Formular für eine Übertragungsanforderung ausfüllen möchten.
2.  Wählen Sie im Menü Kunde die Option **Abonnements** aus.
3.  Wählen Sie den Abschnitt **Übertragungsanforderung** aus.
4.  Wählen Sie im **Abschnitt Übertragungsanforderung** die Option **Neue Anforderung hinzufügen** aus.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Abschnitt &quot;Übertragungen&quot;.":::

5.  Füllen Sie das Formular **Neue Übertragungsanforderung** aus.

6.  Wählen Sie Send transfer request Send **(Übertragungsanforderung**  >  **senden) aus.**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Füllen Sie das Formular für übertragungsanforderung aus.":::

7.  Überprüfen der Bestätigung der Übertragungsanforderung

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Überprüfen Sie die ausstehende Übertragung.":::

    >[!Note]
    >Der zukünftige Partner kann die Übertragungsanforderung abbrechen, indem er die **Anforderung abbrechen** in der oberen rechten Ecke nur dann auswählt, wenn der Status der Übertragungsanforderung "Ausstehend" lautet. Sobald der Status der Übertragungsanforderung "In Bearbeitung" oder "Abgeschlossen" lautet, sind Keine Abbruchs möglich.

## <a name="current-partner-tasks-to-be-completed"></a>Aktuelle Partneraufgaben, die abgeschlossen werden sollen

Der Administrator-Agent des aktuellen Partners des Kunden erhält eine E-Mail, dass der Kunde eine Übertragung seiner Abonnements anfordert:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Bewertung.":::

Überprüfen und akzeptieren Sie das Formular für die Übertragungsanforderung von Partner Center, um die Abonnementübertragung abzuschließen.

>[!Note]  
>Wenn vom aktuellen Partner innerhalb von 30 Tagen keine Aktion ausgeführt wird, läuft die Anforderung ab, und der zukünftige Partner muss eine neue Übertragungsanforderung erstellen.

1.  Wählen Sie **Übertragungsanforderung** überprüfen aus der E-Mail oder aus.
1.  **Wählen** Sie im Menü Partner Center kunden und dann den Kunden aus, für den eine Übertragungsanforderung übermittelt wurde.
2.  Wählen Sie im Menü Kunde die Option **Abonnements** aus.
3.  Wählen Sie den Abschnitt **Übertragungsanforderung** aus.
4.  Erweitern Sie Übertragungsinformationen, indem Sie unter **Empfangene Anforderungen** die ausgewählte **Übertragungsanforderungs-ID** auswählen.

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Übertragungsanforderung für Quellüberprüfungen.":::

5.  Überprüfen Sie die Übertragungsanforderung. Wählen Sie die angeforderten Azure-Abonnements aus, die übertragen werden sollen.

>[!Note]  
> Bevor Sie fortfahren, beachten Sie Folgendes: Sie haben keinen Zugriff mehr auf die ausgewählten Abonnements.
> Die weitere Nutzung wird Ihnen nicht in Rechnung stellen.
> Azure-Reservierungen werden nicht mit den Abonnements übertragen.

6.  Wählen Sie dann **Akzeptieren und übertragen** aus, um den Übertragungsvorgang abzuschließen.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Wählen Sie abonnements aus, die unter Ihren Azure-Plänen übertragen werden sollen.":::

7.  Anzeigen der Bestätigung der Übertragungsakzeptanz.

   An diesem Punkt werden der zukünftige Partner, der Kunde und der aktuelle Partner per E-Mail über die akzeptierte Übertragungsanforderung benachrichtigt.

   Nachdem der Übergang akzeptiert wurde, kann der Übertragungsstatus bis zu 15 Minuten lang ausstehend bleiben, während das System aktualisiert wird. Wenn dies länger dauert, versucht das System drei Tage lang weiter. Wenn der Übertragungsstatus weiterhin Ausstehend bleibt, sollte der Partner eine Serviceanfrage senden.

   Sobald die Übertragung abgeschlossen ist, werden die in der Anforderung enthaltenen Abonnements im Azure-Plan des zukünftigen Partners angezeigt und nicht mehr bei Ihnen aufgeführt.

>[!Note]  
>Für indirekte Anbieter: Informieren Sie Ihren indirekten Handelspartner, dass die Übertragungsanforderung akzeptiert wurde.

### <a name="managing-your-transferred-customer-subscriptions"></a>Verwalten Ihrer übertragenen Kundenabonnements

- Der Zugriff auf vorhandene Benutzer, Gruppen oder Dienstprinzipale, die per rollenbasierter Azure-Zugriffssteuerung (Azure Role-Based Access Control, Azure RBAC) zugewiesen wurden, ist von der Übertragung nicht betroffen. Die rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, [Azure RBAC)](/azure/role-based-access-control/overview) unterstützt Ihren Kunden bei der Verwaltung, wer Zugriff auf Azure-Ressourcen hat, was er mit diesen Ressourcen tun kann und auf welche Bereiche er Zugriff hat. Als neuer Partner erhalten Sie nach der Abonnementübertragung keinen RBAC-Zugriff auf die Ressourcen Ihres Kunden. Der vorherige Partner Ihres Kunden behält seinen RBAC-Zugriff bei. Arbeiten Sie mit Ihrem Kunden zusammen, um zu verstehen, wer Einblicke in seine Abonnements hat und wie sie gewünschte Änderungen vornehmen können.

- Daher ist es wichtig, dass Ihr Kunde den Azure RBAC-Zugriff für seinen vorherigen Partner entfernt und den Zugriff für den neuen Partner hinzufüge. Weitere Informationen dazu, wie Ihr Kunde neuen Zugriff erteilt, finden Sie unter Was ist die [rollenbasierte Zugriffssteuerung in Azure (Azure Role-Based Access Control, Azure RBAC)?](/azure/role-based-access-control/overview) Weitere Informationen dazu, wie Ihr Kunde den RBAC-Zugriff Ihres vorherigen Partners entfernt, finden Sie unter [Entfernen einer Rollenzuweisung.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

- Darüber hinaus erhalten Sie nicht automatisch [Zugriff vom Administrator im Auftrag von (Admin on Behalf Of, AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) auf Ihre Abonnements. AOBO ist erforderlich, damit Partner die Azure-Abonnements ihrer Kunden in ihrem Namen verwalten können. Weitere Informationen zu Azure-Berechtigungen finden Sie unter [Abrufen von Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Nächste Schritte:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Abrufen von Berechtigungen zum Verwalten des Diensts oder Abonnements eines Kunden.](./customers-revoke-admin-privileges.md)
