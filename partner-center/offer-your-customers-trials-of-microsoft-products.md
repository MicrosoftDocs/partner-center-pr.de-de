---
title: Anbieten von Testversionen von Microsoft-Produkten für Kunden
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Kunden können Microsoft-Abonnementprodukte 30 Tage lang testen. Registrieren Sie sich für diese kostenlosen Testversionen im Katalog wie viele andere Onlinedienste.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151133"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Geben Sie Kunden 30 Tage kostenlose Testversionen von Microsoft-Produkten.

**Geeignete Rollen:** Globale Administratorrechte | Administratorrechte für | Vertriebs-Agent

Eine gute Möglichkeit, Kunden neue Microsoft-Produkte einzuführen, ist das Anbieten von kostenlosen 30-Tage-Testversionen. Sie können sich für die Testversionen im Katalog ebenso wie für viele andere Onlinedienste registrieren. Alle Partner können daran teilnehmen.

## <a name="available-trial-offers"></a>Verfügbare Testangebote

Alle Ausstehenden Testangebote finden Sie auf der **Seite "Kunde".** Auf dieser Seite werden alle Abonnements aufgeführt, einschließlich kostenloser Testversionen und kostenpflichtiger Abonnements. (Dieses Feature ist derzeit in China nicht verfügbar.)

Jeder Kunde hat Anspruch auf eine kostenlose Testversion für jedes verfügbare Angebot. Beispielsweise können sie eine kostenlose Testversion für Microsoft 365 Business Standard und eine kostenlose Testversion für Office 365 E3 erhalten. Wenn der Kunde das Angebot jedoch bereits besitzt, kann er keine kostenlose Testversion für dieses Angebot verwenden.

### <a name="available-products"></a>Verfügbare Produkte

Kostenlose Testversionen sind für die umfassendsten und beliebtesten Angebote verfügbar. Neue Testangebote können monatlich eingeführt werden.

Partner finden Testversionen in der monatlichen Preisliste auf der Seite **Preise und** Angebote Partner Center. Bei Testangeboten wird "TESTVERSION" in der Spalte Sekundärer **Lizenztyp** der Preisliste aufgeführt.

Derzeit gibt es **keine kostenlosen Testversionen für** Behördenangebote, Bildungsangebote oder Add-On-Angebote.

## <a name="licenses-for-free-trial-offers"></a>Lizenzen für kostenlose Testangebote

Alle kostenlosen Testversionen bieten 25 Lizenzen. Sie können diese Zahl während der Testversion nicht ändern. Sie können keine Lizenzen in der kostenlosen Testversion hinzufügen oder entfernen. Nachdem die Testversion in ein kostenpflichtiges Abonnement konvertiert wurde, können Sie dem Abonnement weitere Lizenzen hinzufügen.

Testlizenzen sollten Benutzern auf die gleiche Weise zugewiesen werden, wie kostenpflichtige Dienstlizenzen zugewiesen werden.

## <a name="sign-customers-up-for-trials"></a>Registrieren von Kunden für Testversionen

Erhalten Sie eine Testversion für Ihren Kunden in Partner Center:

1. Navigieren Sie im Partner Center unter **Verkaufen** zu **Katalog**. 
2. Wählen Sie im Katalog unter **Abrechnungshäufigkeit** die Option **Testangebot** aus. Dadurch werden nur kostenlose Testversionen angezeigt und kostenpflichtige Angebote ausgeblendet. Testversionen werden im Katalog auf der Registerkarte **Testversionen** angezeigt.
3. Wählen Sie die kostenlose Testversion aus, die Sie anbieten möchten, und wählen Sie dann **Übermitteln** aus. Alle Testversionen gelten für 30 Tage, in denen keine Kosten in Rechnung gestellt werden. Sie können sie auch zu einem beliebigen Zeitpunkt während des Testzeitraums in ein kostenpflichtiges Abonnement umwandeln.

## <a name="converting-trials-to-paid-subscriptions"></a>Konvertieren von Testversionen in kostenpflichtige Abonnements

Eine kostenlose Testversion wird nicht automatisch in ein kostenpflichtiges Abonnement konvertiert. Nach 30 Tagen muss eine kostenlose Testversion in ein kostenpflichtiges Abonnement konvertiert werden, andernfalls läuft sie [ab.](#expiring-offers) Kostenlose Testversionen können nicht erweitert werden.

Sie müssen die Testversion selbst in ein kostenpflichtiges Abonnement konvertieren. Hierzu können Sie [die Partner Center](#convert-trials-using-partner-center) oder [die Partner Center-APIs](#convert-trials-using-apis)verwenden.

> [!NOTE]
> Kostenlose Testversionen von Kunden für das CSP-Programm (Cloud Solution Provider) können nicht in einen anderen Programmmandanten (z. B. EA, Open oder MOSP) konvertiert werden.

### <a name="convert-trials-using-partner-center"></a>Konvertieren von Testversionen mit Partner Center

Sie können Testversionen mithilfe von Partner Center in kostenpflichtige Abonnements konvertieren:

1. Wählen Sie auf der Abonnementseite des Kunden die kostenlose Testversion aus.
2. Wählen Sie **Testabonnement auf kostenpflichtiges Abonnement umstellen** aus.
3. Geben Sie die gewünschte Anzahl von Lizenzen und die Abrechnungshäufigkeit ein, und wählen Sie **Übernehmen** aus.
4. Die Abrechnung für das kostenpflichtige Abonnement beginnt am Konvertierungsdatum, und das Abonnement wird 12 Monate nach dem Konvertierungsdatum automatisch verlängert. 

### <a name="convert-trials-using-apis"></a>Konvertieren von Testversionen mithilfe von APIs

Möglicherweise müssen Sie Ihre APIs ändern, um die Konvertierung einer kostenlosen Testversion in ein kostenpflichtiges Abonnement zu ermöglichen. Weitere Informationen finden Sie in der folgenden Entwicklerdokumentation:

- [Umwandeln eines Testabonnements in ein kostenpflichtiges Abonnement](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Abrufen einer Liste von Testwechselangeboten](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Testversionen ohne Konvertierungen

Nicht alle Testversionen können in kostenpflichtige Abonnements konvertiert werden. Partner können eine Testversion verwenden, für die bis zum Ablaufdatum keine Konvertierungen mehr zur Verfügung steht. Partner können kompatible Angebote erwerben, die die gleichen Dienste wie das Testangebot unterstützen.  Dies sollte vor Ablauf der Testversion erfolgen, um sicherzustellen, dass die Dienste der neu erworbenen Angebote mit den Diensten der Testversion in Einklang sind. 

|**Testversion**   |**Kompatible Angebote für kleine Unternehmen**   |**Kompatible Enterprise-Angebote**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Testversion von Microsoft Teams Commercial Cloud (vom Benutzer initiiert)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (früher F1), Office 365 for Enterprise (E1, E3 und E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Die oben genannten Angebote verfügen über ähnliche Servicepläne mit ähnlicher Funktionalität, es kann jedoch einige Unterschiede zwischen den Angeboten geben.

### <a name="expiring-offers"></a>Läuft angebote ab

Sie werden nicht über das Ende von Angeboten benachrichtigt. Sie können anstehende Ablaufdaten mithilfe der Kundenansicht auf Partner Center oder durch Abfragen der API nachverfolgen. Sie sollten diese Datumsangaben regemäßig überprüfen, damit Sie zusammen mit dem Kunden die entsprechenden Folgeaktionen durchführen können, wenn eine Entscheidung getroffen werden muss.

Nach Ablauf einer Testversion wird einem Kunden, der versucht, sich bei dieser Testversion zu anmelden, eine Ablaufmeldung angezeigt. Die Daten werden jedoch in Übereinstimmung mit den Datenaufbewahrungsstandards gespeichert. Nachdem Sie ein neues Abonnement mit denselben Serviceplänen erworben haben, kann über das neu aktivierte Abonnement erneut auf die Informationen Ihres Kunden zugegriffen werden.

## <a name="billing"></a>Abrechnung

Die jährliche Abrechnung und kostenlose Testversionen sind in Sovereign Clouds und der öffentlichen Cloud identisch. Der einzige Unterschied sind die Test-SKUs, die zum Zeitpunkt des Starts verfügbar sind.

## <a name="billing-for-free-trials"></a>Abrechnung für kostenlose Testversionen

Kostenlose Testversionen können sowohl für monatliche als auch für jährlich abgerechnete Abonnements verwendet werden. Sie können die Abrechnungshäufigkeit auswählen, wenn Sie die Testversion in ein kostenpflichtiges Abonnement konvertieren.

Das Startdatum des Abonnements basiert auf dem Konvertierungsdatum. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit jährlicher Abrechnung konvertiert wird, beträgt das Verlängerungsdatum des Abonnements 12 Monate nach dem Konvertierungsdatum. Wird die kostenlose Testversion in ein kostenpflichtiges Angebot mit monatlicher Abrechnung umgewandelt, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem auf das Datum der Umwandlung folgenden Abrechnungsdatum.

### <a name="invoices"></a>Invoices

In Ihrer Rechnung oder lizenzbasierten Abstimmungsdatei werden keine kostenlosen Testversionen aufgeführt. Kostenlose Testversionen werden erst in Ihrer Rechnung und lizenzbasierten Abstimmungsdatei angezeigt, nachdem Sie eine kostenlose Testversion in ein kostenpflichtiges Abonnement konvertiert haben. Das konvertierte Abonnement wird auf die gleiche Weise wie jedes neue Abonnement angezeigt.

### <a name="incentives"></a>Incentives

Kostenlose Testversionen haben keine Auswirkungen auf Incentives.

## <a name="support"></a>Support

Um Unterstützung für kostenlose Testversionen zu erhalten, übermitteln Sie eine Serviceanfrage über Partner Center.