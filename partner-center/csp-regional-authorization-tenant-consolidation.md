---
title: Mandantenkonsolidierung für regionale CSP-Autorisierung
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen. Dies umfasst schritte zum Migrieren von Kundenkonten und Kundenabonnements.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147580"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Anweisungen zur Mandantenkonsolidierung für regionale CSP-Autorisierung

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent

\[Einige Informationen beziehen sich auf Vorabversionen, die vor der kommerziellen Freigabe grundlegend geändert werden können. Microsoft übernimmt keine Garantie, weder ausdrücklich noch stillschweigend, für die hier bereitgestellten Informationen.\]

Sie können Mandanten für Ihr Unternehmen konsolidieren. Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.

>[!NOTE]  
>Sie müssen alle bereitgestellten Abonnements und Lizenzanzahlen für jeden Ihrer Kunden in dem Konto kennen, von dem Sie den Übergang unternehmen. Sie werden genau diese Abonnements mit der gleichen Lizenzanzahl im Rahmen des Migrationsprozesses unter dem neuen zentralen CSP-Konto erneut bereitstellen. Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen.  Nach Abschluss der Konsolidierung können Sie nicht mehr auf den vorherigen Mandantenstatus zurückverwenden. Möglicherweise ist auch eine Kundenaktion erforderlich.

## <a name="prepare-for-migration"></a>Vorbereiten der Migration

- Melden Sie sich **bei** Partner Center  mithilfe des Übergangskontos (das Konto, das Sie auf das neue Konto umstiegen) an, und überprüfen Sie alle Kunden und alle Dienste, die für diese Kunden bereitgestellt werden.

- Melden Sie sich von diesem Konto ab.

## <a name="migrate-customer-accounts"></a>Migrieren von Kundenkonten

1. Melden Sie sich **mit Partner Center** **(neues)** Konto (dem Konto, in das Sie Kunden umstiegen) bei ihrem Konto an.

2. Wählen Sie **Kunden** aus.

3. Wählen Sie **Handelspartnerbeziehung anfordern aus.** Ihnen wird eine Standard-E-Mail-Nachricht angezeigt, die an Ihre Kunden gesendet werden soll. Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues Partner Center-Konto.

4. **Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen. Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office 365-Portal aufgefordert. Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office 365 zugreift.

5. Nach der Anmeldung wird der  globale Administrator für das Kundenkonto aufgefordert, eine Vereinbarung zu übermitteln, die dem neuen CSP-Konto delegierte Administratorrechte erteilt. Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.

Die Kunden werden in der Kundenliste des Partners angezeigt, nachdem sie die Vereinbarung 1:1 übermittelt haben.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrieren von nutzungsbasierten Office 365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)

1. Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.

2. Wählen **Partner Center** die Option **Kunden aus.**

3. Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.

4. Wählen Sie **Abonnement hinzufügen** aus.

5. Fügen Sie die richtigen Abonnements und Lizenzanzahlen aus dem Katalog hinzu. Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Kundenliste":::

6. Wählen Sie **Senden aus.**

   Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.

7. Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.

Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.

> [!NOTE]
> Partner müssen Abonnements für das Konto "Übergang vom Partner-Mandanten" in Partner Center an dem Tag  aussetzen, an dem diese Abonnements über das Konto "Übergang zum Partner-Mandanten" in der Partner Center eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt.  Supportanfragen für Guthaben werden aufgrund von Überschneidungen bei der Abrechnung verweigert, die auftreten, wenn die **Umstellung von** Abonnements nicht ordnungsgemäß deaktiviert wird.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Deaktivieren der Office 365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“

Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr. Sie müssen Azure-Abonnements nicht manuell deaktivieren, da Azure-Abonnements während des Migrationsprozesses automatisch deaktiviert werden.

1. Melden Sie sich im **Partner Center** mit dem CSP-Konto **Wechsel von** an, und navigieren Sie zur Kundenliste.

2. Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.

3. Legen Sie das Abonnement auf **angehalten fest,** und wählen Sie dann **übermitteln** aus.

   >[!Note]
   >Durch das Anhalten des Abonnements wird sichergestellt, dass keine doppelte Abrechnung erfolgt.

   Das Abonnement wird in der Abonnementliste **als angehalten** angezeigt.

4. Wiederholen Sie diese Schritte für alle Abonnements des Kunden. Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.

5. Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrieren von nutzungsbasierten Azure-Abonnements

Im Gegensatz zu Office 365-CSP-Abonnements, Azure, müssen nutzungsbasierte CSP-Abonnements nicht manuell migriert werden. Microsoft Azure Support migriert die Azure-Abonnements und alle bereitgestellten Dienste oder Ressourcen von den Konten für den **Übergang von** CSP-Handelspartnern zum Konto für den **Übergang zum** CSP-Handelspartner. Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.

1. Stellen Sie sicher, dass die Kundenkonten, für die Azure-Abonnements migriert werden, der Vereinbarung zugestimmt haben, dem neuen CSP-Konto zugeordnet **zu** werden.

2. Sie benachrichtigen Microsoft darüber, welche Kundenkonten für die Migration bereit sind, und geben die Firmennamen dieses Kunden an.

3. Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt Sie, wenn die Migration abgeschlossen ist.

4. Sie müssen sich vergewissern, dass das Azure-Abonnement unter dem Konto für den **Übergang vom** CSP-Handelspartner jetzt in Partner Center im Abschnitt "Kundenabonnements" als **angehalten** markiert ist.

5. Vergewissern Sie sich, dass für das Azure-Abonnement unter dem Konto **"Übergang zum** CSP-Handelspartner" jetzt der Status **aktiv** in Partner Center im Abschnitt "Kundenabonnements" angezeigt wird.

   >[!Note]
   > Das Deaktivieren der Abonnements unter dem Kunden ändert nicht die Darstellung des Kunden in der Kundenliste. Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen. Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.

6. Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden. Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums. Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.

### <a name="additional-information"></a>Zusätzliche Informationen

- Das Deaktivieren des Abonnements aus dem **Konto "Übergang vom** CSP" wirkt sich nicht auf den Dienst des Endkunden aus, solange der Dienst vor dem Deaktivieren des Abonnements über das Konto **"Übergang** zum CSP" bereitgestellt wurde.

- Abonnements können nicht vom Kunden verwendet werden und generieren keine Gebühren, wenn sie angehalten oder storniert werden.

- Es gibt derzeit keine Möglichkeit, einen Kunden vollständig aus der **Kundenliste zu** entfernen.
- 
    >[!Note]
    > Partner müssen Abonnements  für das Konto für den Übergang vom Partner-Mandanten in Partner Center dem Tag  aussetzen, an dem diese Abonnements in das Konto übergangen und unter dem Kontoübergang eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt. Microsoft unterstützt keine Guthabenanforderungen aufgrund von Überschneidungen bei der Abrechnung,  die auftreten, wenn der Übergang von Abonnements auf "Angehalten" nicht ordnungsgemäß eingestellt wird.

### <a name="simplify-migration-using-export"></a>Vereinfachen der Migration mithilfe der Exportfunktion

Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:

1. Wählen **Sie kunden** auf Partner Center, um die Liste der Kunden zu sehen. 

2. Öffnen Sie den Namen des gewünschten Kunden.

3. Wählen Sie **auf der** Seite Abonnements die Option **Abonnements exportieren** aus, um Details zu Abonnements in eine Excel-Datei zu exportieren.

4. Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.

### <a name="api-registration"></a>API-Registrierung

Weitere Informationen zur API-Registrierung finden Sie unter [Einrichten des API-Zugriffs in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Nächste Schritte

- [Cloud Solution Provider Programm für regionale Märkte und Währungen, in denen Sie CSP-Angebote verkaufen können](regional-authorization-overview.md)
