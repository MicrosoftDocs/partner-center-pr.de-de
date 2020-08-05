---
title: Probleme bei der Kundenzuordnung
description: Erfahren Sie, wie Sie Probleme beheben, die bei der Arbeit mit den in Anspruch genommenen Kunden Zuordnungen von Partner of Record (cpor) auftreten.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: 69c0eb822ed8bf2ff09d7fc4a37e920dc123133a
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/04/2020
ms.locfileid: "87546011"
---
# <a name="customer-association-issues"></a>Probleme bei der Kundenzuordnung

Gilt für:

- Partner Center

Der folgende Inhalt hilft Ihnen beim Beheben von Problemen, die bei der Arbeit mit Kunden Zuordnungen auftreten können.

Geeignete Rollen:

- Abrechnungsadministrator
- Globaler Administrator
- Incentiveadministrator

## <a name="domain-tenant-mismatch"></a>Domänen-Mandanten stimmen nicht überein.

Im beanspruchten cpor-Zuordnungs Anspruchs Fluss (Partner of Record) werden Sie aufgefordert, die Kunden Mandanten-ID und die Unterdomäne anzugeben. Wenn Sie eine Fehlermeldung erhalten, die besagt, dass Sie nicht identisch sind, wenden Sie sich an Ihren Kunden.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Abonnement Fehler im cpor Association-Anspruchs Fluss

Im cpor-Zuordnungs Anspruchs-Flow werden Sie möglicherweise aufgefordert, ein Abonnement für ein Produkt anzugeben, das Sie über Business Applications (Dynamics 365) zu beanspruchen versuchen. Wir bitten um das Abonnement, da wir dynamisch überprüfen, ob das Produkt und das Abonnement zu dem Mandanten gehören, für den die Ansprüche beansprucht werden. Wir überprüfen auch, ob sich das Abonnement im Status aktiv/im Aktivierungs Status befindet.

Wenn Sie den Fehler erhalten, kann dies aus verschiedenen Gründen der Fall sein:

- Das ausgewählte Produkt ist im Mandanten des Kunden nicht vorhanden.
- Das angegebene Abonnement ist nicht für Dynamics
- Das angegebene Abonnement gilt für CSP.
- Der Kunde hat die Produkte für dieses Abonnement noch nicht aktiviert und bereitgestellt.
- Das Abonnement wurde bereits beansprucht.
- Der angegebene Bezeichner ist keine Abonnement-ID.

Wenn Sie Fragen zur Genauigkeit Ihres Abonnements haben, wenden Sie sich an Ihren Kunden, um sicherzustellen, dass das Abonnement korrekt ist und Sie die korrekte Mandanten-ID verwenden.

Wenden Sie sich an den [Support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives), wenn diese Route Ihr Problem nicht behoben hat.

## <a name="when-subscriptions-will-be-available-to-claim"></a>Wenn Abonnements für den Anspruch verfügbar sind

Wenn Sie ein Abonnement anfordern, erhalten Sie eine Fehlermeldung, wenn das Abonnement noch nicht bereitgestellt wurde. Es gibt mehrere Schritte, die der Kunde ausführen muss, damit das Abonnement für die cpor-Plattform verfügbar ist, um es für die Inanspruchnahme verfügbar zu machen. Wenn Sie beim Versuch, ein Abonnement anzufordern, eine Fehlermeldung erhalten, wenden Sie sich an Ihren Kunden, um sicherzustellen, dass er bereitgestellt wurde und das Abonnement, das Sie beanspruchen, korrekt ist. Wenn Sie diese Route bereits übernommen haben, wenden Sie sich an den [Support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Welche Aktivität wähle ich aus?

Die cpor-Plattform, die die Plattform beansprucht, ermöglicht cpor-Zuordnungs Ansprüche im Zusammenhang mit Business Applications und Microsoft 365 Lösungsbereichen Die Aktivitäten, die für die einzelnen Lösungs Bereiche anwendbar sind, sind unten aufgeführt. Wählen Sie die richtige Aktivität basierend auf den Beschreibungen aus, um eine spätere Freigabe zu vermeiden. Die Inanspruchnahme von mit einer falschen Aktivität kann zu fehlenden Berechtigungen und berechtigten Ergebnissen führen.


| Lösungsbereich | Aktivität | Anwendbar für |
| ------ | ----------- | ----------- |
| Geschäftsanwendungen      | Presales   | Wählen Sie diese Option aus, wenn Sie den Erwerb eines berechtigten Produkts beeinflusst haben und sich für die vorab Verkaufsanreize bewerben möchten. Diese Option ist nur anwendbar, wenn der Kunde diese Produkte über einen Volumenlizenzvertrag oder über Web-Direct erworben hat. |
|    |  Verwendung  | Wählen Sie diese Option aus, wenn Sie die Übernahme und Nutzung einer berechtigten Arbeitsauslastung fördern und für Nutzungs Anreize verwenden möchten. Diese Option ist nur anwendbar, wenn der Kunde diese Produkte über einen Volumenlizenzvertrag oder über Web-Direct erworben hat. |
|    | Umsatz Zuordnung   | Wählen Sie diese Option aus, wenn Sie die Auswahl eines berechtigten Produkts als geschäftliche Einflussfaktoren beeinflusst haben. Diese Option gilt nur für die Umsatz Zuweisung, nicht für Incentive-Zahlungen. Diese Option ist nur anwendbar, wenn der Kunde diese Produkte über einen Volumenlizenzvertrag oder über Web-Direct erworben hat.   |
| Microsoft 365   | Verwendung   | Wählen Sie diese Option aus, wenn Sie die Übernahme und Nutzung einer berechtigten Arbeitsauslastung fördern und für Nutzungs Anreize verwenden möchten. |

## <a name="which-mpn-do-i-choose"></a>Welches MPN wähle ich aus?

Im cpor-Zuordnungs Anspruchs-Flow werden Sie aufgefordert, einen Unternehmens-MPN auszuwählen, der den für den Endkunden beanspruchten arbeiten zugeordnet werden soll. Ihr Unternehmen kann über viele mpns verfügen, von denen einige möglicherweise in Incentive-Programmen registriert sind, und andere, die mit einem Partnertyp wie FRP FastTrack verknüpft sind. Der cpor Association-Anspruchs Fluss identifiziert, welche mpns in einem Incentive-Programm registriert sind. Sie werden jedoch nicht informiert, wenn es sich um einen bestimmten Partnertyp MPN handelt. Es ist wichtig, den richtigen MPN auszuwählen, um zu vermeiden, dass er in Zukunft wieder zugänglich ist. Die Inanspruchnahme mit einem falschen MPN kann zu fehlenden Berechtigungen und berechtigten Ergebnissen führen.

Wenn Sie nicht wissen, welcher MPN verwendet werden soll, wenden Sie sich an ihren globalen Administrator.

Wenn der MPN, den Sie verwenden möchten, nicht registriert ist, können Sie diesen auf der [Registerkarte "Incentives Overview](https://partner.microsoft.com/dashboard/incentives/enrollment/summary)" verwalten.

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Auswählen eines Produkts und Eingeben eines Abonnements

Wenn ein Dynamics-Produkt beansprucht und genehmigt wird, kann der Partner die Abonnement-ID im cpor Association-Anspruch Selbstanzeigen. Wenn dieses Abonnement beansprucht wird, befindet es sich im Status "aktiv" oder "aktiviert", aber es kann ein Zeitpunkt sein, zu dem das Abonnement endet, und die neuen Abonnements müssen in einem separaten cpor-Zuordnungs Anspruch beansprucht werden.

## <a name="competing-claims"></a>Konkurrierende Ansprüche

Wenn Sie einen cpor-Zuordnungs Anspruch für einen Kunden und ihre Produkte erstellen, der bereits einem anderen Partner zugeordnet ist, wird Ihr Anspruch durch die Vermittlung geleitet:

1. Nachdem Sie eine neue Kundenzuordnung erstellt haben, überprüft Microsoft die Details der Zuordnung und den bereitgestellten Ausführungsnachweis, um deren Richtigkeit sicherzustellen.

2. Wenn Sie und ein anderer Partner den gleichen Kunden und das gleiche Produkt/die gleiche Arbeitsauslastung beanspruchen, prüft Microsoft die Ausführungs Dokumentation der einzelnen Partner, um zu bestimmen, welcher Partner genehmigt werden muss.

3. Möglicherweise werden von beiden Partnern Weitere Informationen angefordert, was Verzögerungen bei der Verarbeitung der Zuordnungs Anforderung verursachen kann.

4. Ihr cpor-Zuordnungs Anspruch wird immer noch innerhalb von fünf Werktagen überprüft, obwohl der Status für einen längeren Zeitraum _als überprüft bleiben_ kann. Dieses Szenario kann eintreten, wenn Microsoft mit dem Partner zusammenarbeitet, der derzeit das Produkt/die Arbeitsauslastung besitzt. Wenn dies der Fall ist, werden Sie im Kommentar Abschnitt Ihres Anspruchs benachrichtigt. 

>[!IMPORTANT]
>Wenn Sie zusätzliche Informationen benötigen, um Ihre cpor-Zuordnung zu überprüfen, kontaktieren wir Sie über den cpor Association Claim comments-Abschnitt.
