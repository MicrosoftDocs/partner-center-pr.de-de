---
title: Anbieten von Testversionen von Microsoft-Produkten für Kunden | Partner Center
ms.topic: article
ms.date: 03/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ihre Kunden können Microsoft-Abonnements für 30 Tage testen. Registrieren Sie sich wie viele andere Onlinedienste für diese Tests im Katalog.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 6775656c53eed787d94e1b87924426f998b1adbe
ms.sourcegitcommit: 36b8242cc8c47ed36d16f86338a075080c2441e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/21/2020
ms.locfileid: "80112459"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Anbieten von Testversionen von Microsoft-Produkten für Kunden

**Gilt für:**

- Partner Center

**Geeignete Rollen**
-   Globaler Administrator 
-   Benutzeradministrator
-   Vertriebsbeauftragter

Eine gute Möglichkeit, Kunden neue Microsoft-Produkte vorzustellen, ist eine kostenlose Testversion für 30 Tage. Sie können sich für die Testversionen im Katalog ebenso wie für viele andere Onlinedienste registrieren. Alle Partner können daran teilnehmen.

## <a name="available-trial-offers"></a>Verfügbare Testangebote

Sie finden alle ausstehenden Testangebote auf der **Kunden** Seite. Auf dieser Seite werden alle Abonnements einschließlich kostenloser und kostenpflichtiger Abonnements aufgelistet. (Dieses Feature ist in China zurzeit nicht verfügbar.)

Jeder Kunde hat Anspruch auf eine kostenlose Testversion für jedes verfügbare Angebot. Sie können z. B. eine kostenlose Testversion für Office 365 Business Premium und eine kostenlose Testversion für Office 365 E3 erhalten. Wenn der Kunde das Angebot jedoch bereits besitzt, kann er für dieses Angebot keine kostenlose Testversion verwenden.

### <a name="available-products"></a>Verfügbare Produkte

Kostenlose Testversionen sind für folgende Produkte verfügbar:

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 mit PSTN
- Office 365 E5 ohne PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Plan 1
- Dynamics 365 Business Central
- Microsoft 365 Business

Wir bieten kostenlose Testversionen für diese Produkte an, da sie die umfassendsten und beliebtesten geschäftlichen Angebote sind. Wir werden in Zukunft möglicherweise weitere kostenlose Testangebote hinzufügen.

Zurzeit sind **keine kostenlosen** Testversionen für behördliche Angebote, Schulungsangebote oder Add-on-Angebote verfügbar.

## <a name="licenses-for-free-trial-offers"></a>Lizenzen für kostenlose Testangebote

Alle kostenlosen Testversionen bieten 25 Lizenzen. Diese Anzahl kann während des Testzeitraums nicht geändert werden. Sie können keine Arbeitsplätze in der kostenlosen Testversion hinzufügen oder entfernen. Nachdem die Testversion in ein kostenpflichtiges Abonnement konvertiert wurde, können Sie dem Abonnement weitere Lizenzen hinzufügen.

Sie sollten Testlizenzen und Arbeitsplätze genauso wie bei einem kostenpflichtigen Dienst im Partner Center zuweisen.

## <a name="sign-customers-up-for-trials"></a>Registrieren von Kunden für Testversionen

So signieren Sie Ihren Kunden für eine Testversion über Partner Center:

1. Navigieren Sie im Partner Center unter **Verkaufen** zu **Katalog**. 
2. Klicken Sie im Katalog unter **Abrechnungshäufigkeit** auf **Testangebot**. Dadurch werden nur kostenlose Testversionen angezeigt und Angebote ausgeblendet, die nicht kostenlos sind. Testversionen werden im Katalog auf der Registerkarte **Testversionen** angezeigt.
3. Wählen Sie die kostenlose Testversion aus, die Sie anbieten möchten, und wählen Sie dann **Übermitteln**. Alle Testversionen gelten für 30 Tage, in denen keine Kosten in Rechnung gestellt werden. Sie können sie zu einem beliebigen Zeitpunkt während der Testphase auch in ein kostenpflichtiges Abonnement umwandeln.

## <a name="converting-trials-to-paid-subscriptions"></a>Umstellen von Testversionen in kostenpflichtige Abonnements

Eine kostenlose Testversion wird nicht automatisch in ein kostenpflichtiges Abonnement konvertiert. Nach 30 Tagen muss eine kostenlose Testversion in ein kostenpflichtiges Abonnement konvertiert werden, oder Sie [läuft](#expiring-offers)ab. Kostenlose Testversionen können nicht erweitert werden.

Sie müssen die Testversion selbst in ein kostenpflichtiges Abonnement konvertieren. Hierfür können Sie [das Partner Center](#convert-trials-using-partner-center) oder [die Partner Center-APIs](#convert-trials-using-apis)verwenden.

> [!NOTE]
> Kostenlose Testversionen für das Cloud Solution Provider-Programm (CSP) können nicht in einen anderen Programm Mandanten (z. b. EA, Open oder musp) konvertiert werden.

### <a name="convert-trials-using-partner-center"></a>Konvertieren von Tests mithilfe von Partner Center

Sie können mithilfe des Partner Center-Dashboards wie folgt Tests in kostenpflichtige Abonnements konvertieren:

1. Wählen Sie von der Abonnementseite des Kunden die kostenlose Testversion aus.
2. Wählen Sie **Umwandeln eines Probeabonnements in ein kostenpflichtiges Abonnement**
3. Geben Sie die gewünschte Anzahl Lizenzen und die Abrechnungsfrequenz ein, und wählen Sie **Übernehmen** aus.
4. Die Abrechnung für das kostenpflichtige Abonnement beginnt mit dem Datum der Konvertierung, und das Abonnement wird automatisch 12 Monate nach der Konvertierung erneuert. 

### <a name="convert-trials-using-apis"></a>Konvertieren von Testversionen mithilfe von APIs

Möglicherweise müssen Sie Ihre APIs ändern, um die Konvertierung einer kostenlosen Testversion in ein kostenpflichtiges Abonnement zu ermöglichen. Weitere Informationen finden Sie in der folgenden Entwicklerdokumentation:

- [Umwandeln eines Probeabonnements in ein kostenpflichtiges Abonnement](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Abrufen einer Liste der Wechselangebote für Probeabonnements](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Tests ohne Konvertierungen

Nicht alle Tests können in kostenpflichtige Abonnements konvertiert werden. Partner können eine Testversion verwenden, die über keine Konvertierungen bis zum Ablaufdatum verfügt. Partner können kompatible Angebote erwerben, die dieselben Dienste wie das Testangebot unterstützen.  Dies sollte vor Ablauf der Testversion erfolgen, um sicherzustellen, dass die Dienste der neu erworbenen Angebote mit den Diensten der Testversion übereinstimmen. 

|**Versuchten**   |**Kompatible Small Business-Angebote**   |**Kompatible Enterprise-Angebote**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Testversion der kommerziellen Cloud von Microsoft Teams (vom Benutzer initiiert)   |Business Essentials, Business Premium, M365 Business   | F3 (ehemals F1), Office 365 for Enterprise (E1, E3 und E5), M365 F1/F3, M365 Enterprise (E3)   |

>[!Note] 
>Die oben aufgeführten Angebote verfügen über ähnliche Servicepläne mit ähnlichen Funktionen, es gibt jedoch möglicherweise einige Unterschiede zwischen den angeboten. 

### <a name="expiring-offers"></a>Ablaufende Angebote

Sie werden nicht über ablaufende Angebote benachrichtigt. Sie können anstehende Ablaufdatums Angaben mithilfe der Kundenansicht im Partner Center oder durch Abfragen der API verfolgen. Sie sollten diese Daten häufig überwachen, damit die entsprechende Transaktion zusammen mit dem Kunden durchgeführt werden kann.

Nachdem eine Testversion abgelaufen ist, wird für einen Kunden, der versucht, sich bei dieser Testversion anzumelden, eine Ablauf Meldung angezeigt. Die Daten werden jedoch in Übereinstimmung mit den Daten Aufbewahrungs Standards gespeichert. Nachdem Sie ein neues Abonnement mit denselben Serviceplänen erworben haben, können Sie über das neu aktivierte Abonnement erneut auf die Informationen Ihres Kunden zugreifen.

## <a name="billing"></a>Abrechnung

Die jährlichen Abrechnungs-und kostenlosen Testversionen sind in unabhängigen Clouds und in den Public Cloud identisch. Der einzige Unterschied besteht darin, dass die Test-SKUs zum Zeitpunkt des Starts verfügbar sind.

## <a name="billing-for-free-trials"></a>Abrechnung für kostenlose Testversionen

Kostenlose Testversionen können sowohl für monatliche als auch für jährlich in Rechnung gestellte Abonnements verwendet werden. Sie können die Abrechnungs Häufigkeit auswählen, wenn Sie die Testversion in ein kostenpflichtiges Abonnement konvertieren.

Das Startdatum des Abonnements basiert auf dem Konvertierungs Datum. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit jährlicher Abrechnung umgewandelt wird, ist zwölf Monate nach dem Datum der Umwandlung das Verlängerungsdatum erreicht. Wenn die kostenlose Testversion in ein kostenpflichtiges Angebot mit monatlicher Abrechnung umgewandelt, liegt das Verlängerungsdatum des Abonnements zwölf Monate nach dem Verlängerungsdatum der Konvertierung.

### <a name="invoices"></a>Rechnungen

In Ihrer Rechnung oder lizenzbasierten Abstimmungs Datei werden keine kostenlosen Testversionen aufgeführt. Kostenlose Testversionen werden nur auf der Rechnung und der lizenzbasierten Abstimmungs Datei angezeigt, nachdem Sie eine kostenlose Testversion in ein kostenpflichtiges Abonnement konvertiert haben. Das konvertierte Abonnement wird auf die gleiche Weise wie jedes neue Abonnement angezeigt.

### <a name="incentives"></a>Vorteile

Kostenlose Testversionen haben keine Auswirkung auf die Anreize.

## <a name="support"></a>Unterstützungswert

Um Unterstützung für kostenlose Testversionen zu erhalten, senden Sie eine Service Request über Partner Center.
