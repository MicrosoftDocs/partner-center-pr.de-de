---
title: "Mandantenkonsolidierung für regionale CSP-Autorisierung | Partner Center"
description: "Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen."
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
keywords: Migrieren von Kunden, Bereitstellung, Mandantenkonto, Mandanten konsolidieren
ms.openlocfilehash: e895fd049211a3dfcb4db930b75d94906563b700
ms.sourcegitcommit: 09f6988db95a3d7c62f2cf16f02cabc2c4418646
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/17/2018
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>Mandantenkonsolidierung für regionale CSP-Autorisierung

**Betrifft:**

-  Partner Center
-  Partner Center für Microsoft Cloud für US-Behörden
-  Partner Center für Microsoft Cloud Deutschland

\[Einige Informationen beziehen sich auf die Vorabversion, die vor der kommerziellen Freigabe möglicherweise wesentlichen Änderungen unterliegt. Microsoft übernimmt für die hier bereitgestellten Informationen keine Garantie, weder ausdrücklicher noch impliziter Art.\]

Konsolidieren Sie anhand dieser Anweisungen Mandanten für verschiedene Länder/Regionen.

**Hinweis:** Sie müssen alle Abonnements und die Anzahl von Arbeitsplätzen für Ihre Kunden kennen, die über die Übergangskonten bereitgestellt wurden. Sie werden im Rahmen des Migrationsprozesses unter dem neuen zentralen CSP-Konto genau dieselben Abonnements mit derselben Anzahl von Arbeitsplätzen erneut bereitstellen. Verwenden Sie das Feature zum Exportieren der Liste, um eine Liste mit Kunden zu erstellen, die zum zentralisierten Mandanten migriert werden sollen. Partner entscheiden sich für die Konsolidierung ihrer Mandanten. Nach Abschluss der Konsolidierung können Partner nicht den vorherigen Zustand wiederherstellen. Beachten Sie, dass auch Schritte vonseiten des Kunden erforderlich sind.

 

## <a name="prepare-for-migration"></a>Vorbereitung auf die Migration


-   Melden Sie sich mit dem zu migrierenden (vorhandenen) Konto unter <https://partnercenter.microsoft.com> an, und notieren Sie alle Kunden und alle für diese Kunden bereitgestellten Dienste.

![Liste regionaler Kunden](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Migrieren von Kundenkonten


1.  Melden Sie sich mit dem zu migrierenden (vorhandenen) Konto unter <https://partnercenter.microsoft.com> an, und navigieren Sie auf dem Partner Center-Dashboard zur Kundenliste.

2.  Wählen Sie die gewünschten Kunden.

3.  Klicken Sie auf **Vertriebspartnerschaft beantragen**. Ihnen wird eine Standard-E-Mail-Nachricht für die Weiterleitung an Ihre Kunden angezeigt. Diese Nachricht enthält eine URL mit der Organisations-ID für Ihr neues PartnerCenter-Konto.

4.  **Kundenaktion:** Stellen Sie sicher, dass alle aktiven Kunden, die Sie migrieren möchten, diese URL aufrufen. Beim Öffnen der URL wird der Kunde zur Anmeldung beim Office365-Portal aufgefordert. Der Kunde meldet sich mit der gleichen Organisations-ID an, mit der er auch auf die Verwaltungsportale von Azure und Office365 zugreift.

5.  Nach der Anmeldung wird der globale Administrator für das Kundenkonto aufgefordert, eine Vereinbarung zu übermitteln, um dem neuen CSP-Konto delegierte Administratorrechte zu gewähren. Ist er einverstanden, aktiviert der Kunde das Kontrollkästchen und stimmt damit der Autorisierung der Beziehung zu.

Die Kunden werden nach Übermittlung der Vereinbarung nacheinander in der Kundenliste des Partners angezeigt.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrieren von nutzungsbasierten Office365-Abonnements und anderen nutzungsbasierten Abonnements (nicht Azure)


1.  Nachdem der Kunde die Vereinbarung unterzeichnet hat, können Sie die Abonnements unter dem zentralisierten Partnermandanten erneut erstellen.

2.  Klicken Sie auf dem PartnerCenter-Dashboard im linken Navigationsmenü auf **Kunden**.

3.  Öffnen Sie den Unternehmensnamen für den Kunden, den Sie migrieren möchten.

4.  Klicken Sie auf **Abonnement hinzufügen**.

5.  Fügen Sie die richtigen Abonnements und die korrekte Arbeitsplatzanzahl aus dem Katalog hinzu. Gleichen Sie die Angaben mit den Informationen der Partnerkonten vom Typ **Transitioning From** ab.

    ![Screenshot der Kundenliste](images/regionalcustomer2.png)

6.  Klicken Sie auf **Übermitteln**.

Die Dienste werden jetzt für den Kunden aus dem Partnerkonto vom Typ **Transitioning To** bereitgestellt.

Wiederholen Sie diese Schritte, um Abonnements für alle weiteren Kunden zu migrieren.

Bevor Sie mit dem nächsten Abschnitt fortfahren, stellen Sie sicher, dass alle Kundenabonnements unter den Partnerkonten vom Typ **Transitioning From** unter dem Partnerkonto vom Typ **Transitioning To** erneut bereitgestellt wurden.

**Hinweis:** Partner müssen Abonnements im Partnermandantenkonto vom Typ **Transitioning From** in Partner Center am selben Tag aussetzen, an dem diese Abonnements migriert und unter dem Partnermandantenkonto vom Typ **Transitioning To** in Partner Center eingerichtet werden, um eine doppelte Abrechnung von Kosten zu vermeiden. Supportanfragen in Bezug auf Kosten, die infolge sich überschneidender Abrechnungen auftreten, weil die Abonnements vom Typ **Transitioning From** nicht ordnungsgemäß deaktiviert wurden, werden abgelehnt.

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Deaktivieren der Office365-Abonnements unter dem Partnerkonto vom Typ „Transitioning From“


Durch die Deaktivierung des CSP-Abonnements unter den Partnerkonten vom Typ **Transitioning From** erfolgen keine zukünftigen Abrechnungen mehr. Azure-Abonnements müssen nicht manuell deaktiviert werden, da diese Abonnements während des Migrationsprozesses automatisch deaktiviert werden.

1.  Melden Sie sich mit dem CSP-Konto vom Typ **Transitioning From** unter <https://partnercenter.microsoft.com> an, und navigieren Sie zur Kundenliste.

2.  Öffnen Sie den Kunden, für den Sie Abonnements deaktivieren möchten, und wählen Sie das erste zu deaktivierende Angebot aus.
3.  Legen Sie für das Abonnement **suspended** fest, und klicken Sie anschließend auf **Übermitteln**.

    **Hinweis:** Durch Aussetzen des Abonnements wird sichergestellt, dass die Abrechnung nicht doppelt erfolgt.

     

    Für das Abonnement wird in der Abonnementliste **suspended** angezeigt.

4.  Wiederholen Sie diese Schritte für alle Abonnements des Kunden. Vergewissern Sie sich, dass für alle Abonnements **suspended** angezeigt wird.

5.  Wählen Sie den nächsten Kunden in der Liste aus, und wiederholen Sie die Schritte zum Deaktivieren aller Abonnements.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrieren von nutzungsbasierten Azure-Abonnements


Beachten Sie, dass nutzungsbasierte Azure-CSP-Abonnements nicht wie Office365-CSP-Abonnements manuell migriert werden müssen. Der Microsoft Azure-Support kann die Azure-Abonnements sowie alle bereitgestellten Dienste oder Ressourcen von den CSP-Vertriebspartnerkonten vom Typ **Transitioning From** zum CSP-Vertriebspartnerkonto vom Typ **Transitioning To** migrieren. Während dieses Übergangs treten beim Kunden keine Dienstunterbrechungen auf.

1.  Stellen Sie sicher, dass für die Kundenkonten, deren Azure-Abonnements migriert werden müssen, die Vereinbarung für das neue CSP-Konto vom Typ **Transitioning To** akzeptiert wurde.
2.  Partner informieren Microsoft darüber, welche Kundenkonten mit Azure-Abonnements migriert werden können, und stellen die Firmennamen dieser Kunden bereit.
3.  Microsoft migriert die nutzungsbasierten Azure-Abonnements und benachrichtigt den Partner, wenn die Migration abgeschlossen ist.
4.  Der Partner überprüft, ob für das Azure-Abonnement unter den CSP-Vertriebspartnerkonten vom Typ **Transitioning From** in Partner Center im Abschnitt mit den Kundenabonnements jetzt „suspended“ angezeigt wird.
5.  Der Partner überprüft, ob für das Azure-Abonnement unter dem CSP-Vertriebspartnerkonto vom Typ **Transitioning To** nun in Partner Center im Abschnitt mit den Kundenabonnements der Status **active** angezeigt wird.

    **Hinweis:** Durch die Deaktivierung der Abonnements im Kundeneintrag wird nicht die Darstellung des Kunden in der Kundenliste geändert. Zurzeit besteht keine Möglichkeit, Kunden aus der Liste zu entfernen. Partner sollten in Zukunft das erneute Hinzufügen von Abonnements zu diesen Kunden aus dem Konto vom Typ **Transitioning From** vermeiden.

     

6.  Wiederholen Sie diese Schritte für alle Abonnements in allen Kundendatensätzen, um künftige Kosten für die Konten vom Typ **Transitioning From** zu vermeiden. Der Partner erhält eine endgültige Rechnung mit einer Gutschrift für die Anzahl der nicht genutzten Tage zwischen dem Stornierungsdatum und dem letzten Tag des Abrechnungszeitraums. Nach diesem letzten Abrechnungszeitraum werden keine zukünftigen Rechnungen generiert.

### <a name="notes"></a>Hinweise

-   Die Deaktivierung des Abonnements im CSP-Konto vom Typ **Transitioning From** wirkt sich nicht auf den Dienst des Endkunden aus, sofern der Dienst vor der Deaktivierung über das CSP-Konto vom Typ **Transitioning To** bereitgestellt wurde.

-   Abonnements können vom Kunden nicht verwendet werden und generieren keine Gebühren, wenn sie ausgesetzt oder gekündigt wurden.

-   Zurzeit besteht keine Möglichkeit, einen Kunden vollständig aus der Kundenliste zu entfernen.

-   **Hinweis:** Partner müssen Abonnements im Partnermandantenkonto vom Typ **Transitioning From** in Partner Center am selben Tag aussetzen, an dem diese Abonnements migriert und unter dem Partnermandantenkonto vom Typ **Transitioning To** in Partner Center eingerichtet werden, um eine doppelte Abrechnung von Kosten zu vermeiden. Microsoft lehnt Supportanfragen in Bezug auf Kosten ab, die infolge sich überschneidender Abrechnungen auftreten, weil Abonnements vom Typ **Transitioning From** nicht ordnungsgemäß auf „suspended“ gesetzt wurden.

     

### <a name="simplify-migration-using-export"></a>Vereinfachen der Migration mithilfe der Exportfunktion

Mit der **Exportfunktion** können Sie die Abonnements erfassen, die Sie in der neuen konsolidierten Struktur benötigen:

1.  Klicken Sie auf dem Dashboard auf **Kunden**, um die Liste der Kunden in der vorhandenen Struktur anzuzeigen.

2.  Öffnen Sie den Namen des gewünschten Kunden.

3.  Klicken Sie auf der Seite **Abonnements** auf **Export Subscriptions**, um Details zu Abonnements in eine Excel-Datei zu exportieren.

4.  Verwenden Sie diese Liste, um die Abonnements im neuen konsolidierten Mandanten neu zu erstellen.

### <a name="api-registration"></a>API-Registrierung

Weitere Informationen zur API-Registrierung finden Sie in [auf dieser Seite](https://go.microsoft.com/fwlink/?linkid=847990).

## <a name="partner-center-activity-log"></a>Partner Center-Aktivitätsprotokoll


Mithilfe des Aktivitätsprotokolls können Partner Informationen zu allen den Kunden betreffenden Änderungen anzeigen, die auf dem Mandanten vorgenommen wurden. Dies ermöglicht Partnern die Nachverfolgung von Änderungen an einem Kundenmandanten.

**Anzeigen des Aktivitätsprotokolls**

1.  Klicken Sie auf dem Partner Center-Dashboard auf den Link **Aktivitätsprotokoll**.
2.  Sehen Sie sich auf der Seite **Aktivitätsprotokoll** die Änderungen an, die an Kundenkonten vorgenommen wurden. Wählen Sie zum Filtern des Aktivitätsprotokolls nach **Datum Start-** und **Enddatum** aus, um die ausgewählten Einträge im Protokoll einzuschränken. Verwenden Sie das Suchfeld, um im **Aktivitätsprotokoll** nach Kunde zu filtern.

**Exportieren des Aktivitätsprotokolls**

-   Klicken Sie auf **Export log**, um die Daten Ihres Aktivitätsprotokolls in eine CSV-Datei zu exportieren.

    Sie können auch die Kunden- und die Abonnementliste eines einzelnen Kunden exportieren (auf der Abonnementseite des Kunden).

 

 



