---
title: 'Incentives: Probleme bei der Kundenzuordnung'
description: Erfahren Sie, wie Sie Probleme beheben, die bei der Arbeit mit CPOR-Kundenzuordnungen (Claimed Partner of Record) auftkommen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152170"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Probleme mit CPOR-Kundenzuordnungen (Claimed Partner of Record)

**Geeignete Rollen:** Abrechnungsadministrator| Globale Administratorrechte | Incentives-Administrator

Der folgende Inhalt hilft Ihnen bei der Lösung von Problemen, die bei der Arbeit mit Kundenzuordnungen auftkommen können.

## <a name="domain-tenant-mismatch"></a>Konflikt zwischen Domäne und Mandant

Im Anspruchsfluss anspruchsanspruch "Claimed Partner of Record( CPOR)" werden Sie aufgefordert, die Mandanten-ID und unterdomäne des Kunden eins zu geben. Wenn Sie eine Fehlermeldung erhalten, die besagt, dass sie nicht übereinstimmen, wenden Sie sich an Ihren Kunden, um sicherzustellen, dass Sie über die richtigen Details verfügen.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Abonnementfehler im CPOR-Zuordnungsanspruchsfluss

Im CPOR-Zuordnungsanspruchsablauf werden Sie möglicherweise aufgefordert, ein Abonnement für ein Produkt zu erstellen, das Sie über Business Applications (Dynamics 365) beanspruchen möchten. Wir fragen nach dem Abonnement, da wir dynamisch überprüfen, ob das Produkt und das Abonnement zu dem Mandanten gehören, für den der Anspruch beansprucht wird. Wir überprüfen auch, ob das Abonnement aktiv bzw. im Toleranzstatus ist.

Wenn Sie den Fehler erhalten, kann dies mehrere Gründe haben:

- Das ausgewählte Produkt ist im Mandanten des Kunden nicht vorhanden.
- Das bereitgestellte Abonnement gilt nicht für Dynamics.
- Das angegebene Abonnement gilt für CSP.
- Der Kunde hat die Produkte für dieses Abonnement noch nicht aktiviert/bereitgestellt.
- Das Abonnement wurde bereits beansprucht.
- Der bereitgestellte Bezeichner ist keine Abonnement-ID.

Wenn Sie eine Frage zur Genauigkeit Ihres Abonnements haben, arbeiten Sie mit Ihrem Kunden zusammen, um sicherzustellen, dass das Abonnement korrekt ist und Sie die richtige Mandanten-ID verwenden.

Wenn das Problem mit dieser Route nicht behoben wurde, wenden Sie sich an [den Support.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="when-subscriptions-will-be-available-to-claim"></a>Wann Abonnements für den Anspruch verfügbar sind

Wenn Sie ein Abonnement beanspruchen, erhalten Sie eine Fehlermeldung, wenn das Abonnement noch nicht bereitgestellt wurde. Es gibt mehrere Schritte, die der Kunde ausführen muss, damit das Abonnement für die CPOR-Plattform verfügbar wird, um es zu übernehmen und für den Anspruch verfügbar zu machen. Wenn Sie beim Versuch, ein Abonnement in Anspruch zu nehmen, einen Fehler erhalten, wenden Sie sich an Ihren Kunden, um sicherzustellen, dass es bereitgestellt wurde und das abonnement, das Sie beanspruchen, richtig ist. Wenn Sie diese Route bereits genommen haben, wenden Sie sich an den [Support.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>Welche Aktivität wähle ich aus?

Die CPOR-Anspruchsplattform ermöglicht CPOR-Zuordnungsansprüche im Zusammenhang mit Business Applications und Microsoft 365 Lösungsbereichen. Unten sind die Aktivitäten aufgeführt, die für die einzelnen Lösungsbereiche gelten. Wählen Sie die richtige Aktivität basierend auf den Beschreibungen aus, um zu vermeiden, dass sie in Zukunft zurückgefordert werden muss. Ein Anspruch mit einer falschen Aktivität kann zu einer verfehlten Berechtigung und zu incentive-Einnahmen führen.


| Lösungsbereich | Aktivität | Gilt für |
| ------ | ----------- | ----------- |
| Geschäftsanwendungen      | Presales   | Wählen Sie aus, ob Sie den Kauf eines berechtigten Produkts beeinflusst haben, und möchten Sich für Pre-Sale-Incentives bewerben. Diese Option gilt nur, wenn der Kunde diese Produkte über einen Volumenlizenzvertrag oder Web-Direct erworben hat. |
|    |  Verwendung  | Wählen Sie aus, ob Sie deren Einführung und Nutzung einer berechtigten Workload steuern und Nutzungs-Incentives beantragen möchten. Diese Option gilt nur, wenn der Kunde diese Produkte über einen Volumenlizenzvertrag oder Web-Direct erworben hat. |
|    | Umsatzzuordnung   | Wählen Sie aus, ob Sie die Auswahl eines geeigneten Produkts als Geschäftlichen Einfluss beeinflusst haben. Diese Option gilt nur für die Umsatzzuordnung, nicht für Incentivezahlungen. Diese Option gilt nur, wenn der Kunde diese Produkte über einen Volumenlizenzvertrag oder Web-Direct erworben hat.   |
| Microsoft 365   | Verwendung   | Wählen Sie aus, ob Sie deren Einführung und Nutzung einer berechtigten Workload steuern und Nutzungs-Incentives beantragen möchten. |

## <a name="which-mpn-do-i-choose"></a>Welches MPN wähle ich aus?

Im Anspruchsflow für die CPOR-Zuordnung werden Sie aufgefordert, ein Unternehmens-MPN auszuwählen, das der Arbeit zugeordnet werden soll, für die Sie beim Endkunden anspruchsbeansprucht werden. Ihr Unternehmen kann über viele MPNs verfügen, von denen einige in Incentiveprogrammen registriert sind, und andere, die einem Partnertyp wie FRP FastTrack zugeordnet sind. Der CPOR-Zuordnungsanspruchsfluss identifiziert, welche MPNs in einem Incentive-Programm registriert sind, er gibt jedoch nicht an, ob es sich um einen bestimmten Partnertyp MPN handelt. Es ist wichtig, das richtige MPN auszuwählen, um zu vermeiden, dass es in Zukunft wieder zurückgefordert werden muss. Das Beanspruchen mit einem falschen MPN kann zu verpassten Berechtigungs- und Incentive-Einnahmen führen.

Wenn Sie nicht wissen, welches MPN verwendet werden soll, wenden Sie sich an Ihren globalen Administrator.

Wenn das MPN, das Sie verwenden möchten, nicht registriert ist, können Sie dies auf der Registerkarte [Übersicht](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) über Incentives verwalten (Anmeldung erforderlich).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Auswählen eines Produkts im Vergleich zum Eingeben eines Abonnements

Wenn ein Dynamics-Produkt beansprucht und genehmigt wird, kann der Partner die Abonnement-ID im CPOR-Zuordnungsanspruch selbst anzeigen. Wenn dieses Abonnement beansprucht wird, befindet es sich im aktiven status oder im Toleranzstatus, aber es kann eine Zeit geben, zu der das Abonnement endet, und die neuen Abonnements müssen in einem separaten CPOR-Zuordnungsanspruch beansprucht werden.

## <a name="competing-claims"></a>Konkurrierende Ansprüche

Wenn Sie einen CPOR-Zuordnungsanspruch für einen Kunden und seine Produkte erstellen, die bereits mit einem anderen Partner verknüpft sind, wird Ihr Anspruch durch eine Vermittlungsverfahren:

1. Nachdem Sie eine neue Kundenzuordnung erstellt haben, überprüft Microsoft die Details der Zuordnung und den bereitgestellten Ausführungsnachweis, um deren Richtigkeit sicherzustellen.

2. Wenn Sie und ein anderer Partner denselben Kunden und dasselbe Produkt/dieselbe Workload beanspruchen, überprüft Microsoft die Dokumentation zum Ausführungsnachweis jedes Partners, um zu bestimmen, welcher Partner genehmigt werden soll.

3. Möglicherweise werden von beiden Partnern zusätzliche Informationen angefordert, was zu Verzögerungen bei der Verarbeitung Ihrer Zuordnungsanforderung führen kann.

4. Ihr CPOR-Zuordnungsanspruch wird weiterhin innerhalb von fünf Werktagen überprüft, obwohl sein Status möglicherweise für einen längeren Zeitraum als Unter Überprüfung bleibt.  Dieses Szenario kann vorkommen, wenn Microsoft mit dem Partner zusammenarbeiten kann, der derzeit das Produkt bzw. die Workload besitzt. Wenn dies der Fall ist, werden Sie im Kommentarabschnitt Ihres Anspruchs benachrichtigt. 

>[!IMPORTANT]
>Wenn wir zusätzliche Informationen benötigen, um Ihren CPOR-Zuordnungsnachweis (Proof of Execution, PoE) zu überprüfen, wenden wir uns über den Abschnitt CPOR association claim comments (Kommentare zu CPOR-Zuordnungsansprüchen) an Sie.

## <a name="next-steps"></a>Nächste Schritte

- [Erste Schritte mit Incentives](incentives-get-started-intro.md)
