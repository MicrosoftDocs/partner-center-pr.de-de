---
title: Mandantenkonsolidierung für regionale CSP-Autorisierung
ms.topic: article
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen. Dies schließt Schritte zum Migrieren von Kundenkonten und Kunden Abonnements ein.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 956ed0dec2588e1cc2f697e61671308c2d86f8d0
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114404"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Anweisungen zur Mandantenkonsolidierung für regionale CSP-Autorisierung

**Zielgruppe**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent

\[Einige Informationen beziehen sich auf Vorabversionen, die vor der kommerziellen Freigabe grundlegend geändert werden können. Microsoft übernimmt keine Garantie, weder ausdrücklich noch stillschweigend, für die hier bereitgestellten Informationen.\]

Mandanten können für Ihr Unternehmen konsolidiert werden. Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.

>[!NOTE]  
>Sie müssen alle bereitgestellten Abonnements und Arbeitsplatz Anzahlen für die einzelnen Kunden in dem Konto beachten, von dem aus Sie wechseln. Sie werden im Rahmen des Migrationsprozesses dieselben exakten Abonnements mit der gleichen Anzahl von Arbeitsplätzen unter dem neuen zentralen CSP-Konto bereitstellen. Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen.  Wenn die Konsolidierung fertiggestellt ist, können Sie nicht mehr auf den vorherigen Mandanten Status zurückgreifen. Möglicherweise ist auch eine Kunden Aktion erforderlich.

## <a name="prepare-for-migration"></a>Vorbereiten der Migration

- Melden Sie sich mit dem **transitionskonto** , das Sie zum neuen Konto wechseln, bei **Partner Center** an, und überprüfen Sie alle Kunden und alle Dienste, die für diese Kunden bereitgestellt werden.

- Melden Sie sich von diesem Konto ab.

## <a name="migrate-customer-accounts"></a>Migrieren von Kundenkonten

1. Melden Sie sich bei **Partner Center** mit dem **transitionskonto** (neu) an (das Konto, in das Sie die Kunden wechseln).

2. Wählen Sie **Kunden** aus.

3. Klicken Sie auf **Vertriebspartnerschaft beantragen**. Ihnen wird eine Standard-e-Mail-Nachricht angezeigt, die an Ihre Kunden gesendet wird. Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues Partner Center-Konto.

4. **Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen. Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office 365-Portal aufgefordert. Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office 365 zugreift.

5. Nach der Anmeldung wird der globale Administrator für das **Kundenkonto** aufgefordert, eine Vereinbarung zu übermitteln, die dem neuen CSP-Konto Delegierte Administratorrechte erteilt. Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.

Die Kunden werden in der Kundenliste des Partners angezeigt, nachdem Sie die Vereinbarung nacheinander übermittelt haben.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrieren von nutzungsbasierten Office 365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)

1. Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.

2. Wählen Sie im **Partner Center** **Kunden**aus.

3. Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.

4. Wählen Sie **Abonnement hinzufügen** aus.

5. Fügen Sie die richtigen Abonnements und die korrekte Arbeitsplatzanzahl aus dem Katalog hinzu. Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Kundenliste":::

6. Klicken Sie auf **senden.**

   Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.

7. Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.

Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.

> [!NOTE]
> Partner müssen Abonnements bei der **Umstellung vom** Partner Mandanten Konto in Partner Center an denselben Tag aussetzen, an dem diese Abonnements übertragen werden, und im Partner Center im Rahmen des **Übergangs zum** Partner Mandanten Konto eingerichtet werden, um sicherzustellen, dass keine doppelte Abrechnung erfolgt. Support Anfragen werden aufgrund von Überlappungen bei der Abrechnung verweigert, wenn der **Übergang von** Abonnements nicht ordnungsgemäß deaktiviert wird.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Deaktivieren der Office 365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“

Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr. Azure-Abonnements müssen nicht manuell deaktiviert werden, da Azure-Abonnements während des Migrations Vorgangs automatisch deaktiviert werden.

1. Melden Sie sich im **Partner Center** mit dem CSP-Konto **Wechsel von** an, und navigieren Sie zur Kundenliste.

2. Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.

3. Legen Sie für das Abonnement **suspended** fest, und klicken Sie anschließend auf **Übermitteln**.

   >[!Note]
   >Durch das Anhalten des Abonnements wird sichergestellt, dass keine doppelte Abrechnung erfolgt.

   Das Abonnement **wird** in der Liste Abonnements angezeigt.

4. Wiederholen Sie diese Schritte für alle Abonnements des Kunden. Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.

5. Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrieren von nutzungsbasierten Azure-Abonnements

Im Gegensatz zu den Office 365 CSP-Abonnements müssen Azure und Verwendungs basierte CSP-Abonnements nicht manuell migriert werden. Microsoft Azure Support migriert die Azure-Abonnements sowie alle bereitgestellten Dienste oder Ressourcen von der **Umstellung von** CSP-Reseller-Konten zum Wechsel **zum** CSP-Reseller-Konto. Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.

1. Stellen Sie sicher, dass das Kundenkonto, für das Azure-Abonnements migriert werden sollen, die Vereinbarung zum neuen **Übergang zum** CSP-Konto zugeordnet haben.

2. Sie benachrichtigen Microsoft, welche Kundenkonten für die Migration bereit sind, und geben die Firmennamen dieser Kunden an.

3. Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt Sie, wenn die Migration beendet ist.

4. Sie müssen sicherstellen, dass das Azure-Abonnement im Rahmen des **Übergangs von** CSP-Reseller-Konto jetzt im Partner Center im Abschnitt Kunden Abonnements als angeh **alten gekennzeichnet ist** .

5. Vergewissern Sie sich, dass das Azure-Abonnement unter der **Umstellung auf** das CSP-Reseller-Konto jetzt den Status **aktiv** im Partner Center im Abschnitt Kunden Abonnements anzeigt.

   >[!Note]
   > Durch das Deaktivieren der Abonnements unter dem Kunden wird die Darstellung des Kunden in der Kundenliste nicht geändert. Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen. Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.

6. Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden. Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums. Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.

### <a name="additional-information"></a>Zusätzliche Informationen

- Das Deaktivieren des Abonnements von der **Umstellung vom** CSP-Konto wirkt sich nicht auf den Dienst des Endkunden aus, solange der Dienst vor dem Deaktivieren des Abonnements vom **Übergang zum** CSP-Konto bereitgestellt wurde.

- Abonnements können nicht vom Kunden verwendet werden, und es werden keine Gebühren generiert, wenn Sie angehalten oder abgebrochen werden.

- Es gibt derzeit keine Möglichkeit, einen Kunden vollständig aus der **Kunden** Liste zu entfernen.
- 
    >[!Note]
    > Partner müssen Abonnements bei der **Umstellung vom** Partner Mandanten Konto in Partner Center an denselben Tag, an dem diese Abonnements umgestellt werden, und bei der Umstellung **auf** das Konto sperren, um sicherzustellen, dass keine doppelte Abrechnung erfolgt. Microsoft unterstützt keine Kreditanforderungen aufgrund einer Überlappung bei der Abrechnung, wenn die **Umstellung von** Abonnements auf angehalten nicht ordnungsgemäß festgelegt wird.

### <a name="simplify-migration-using-export"></a>Vereinfachen der Migration mithilfe der Exportfunktion

Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:

1. Klicken Sie auf **Kunden** im Partner Center, um die Kundenliste anzuzeigen. 

2. Öffnen Sie den Namen des gewünschten Kunden.

3. Klicken Sie auf der Seite **Abonnements** auf **Export Subscriptions**, um Details zu Abonnements in eine Excel-Datei zu exportieren.

4. Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.

### <a name="api-registration"></a>API-Registrierung

Weitere Informationen zur API-Registrierung finden [Sie unter Einrichten des API-Zugriffs in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).

## <a name="next-steps"></a>Nächste Schritte

- [Einrichten und Verwalten von Kundenkonten für Reseller-Partner in Partner Center](customer-accounts.md)
