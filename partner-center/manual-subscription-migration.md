---
title: "Migrieren von Dynamics AX-Abonnements zu Dynamics 365 | Partner Center"
description: "Microsoft führt Dynamics 365 ein, die nächste Generation intelligenter Unternehmensanwendungen, mit denen Ihre Organisation wachsen, sich entwickeln und transformiert werden kann, um die Anforderungen Ihrer Kunden zu erfüllen und neue Geschäftschancen zu nutzen."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: cb3523dffbd017aa5c40e6899e1cb37be1f2a726
ms.openlocfilehash: f19e46da31a7e479ebd3b1cd368ca7646c3c55b7

---

# Migrieren von Dynamics AX-Abonnements zu Dynamics 365

**Betrifft**

-  Partner Center

Microsoft führt Dynamics 365 ein, die nächste Generation intelligenter Unternehmensanwendungen, mit denen Ihre Organisation wachsen, sich entwickeln und transformiert werden kann, um die Anforderungen Ihrer Kunden zu erfüllen und neue Geschäftschancen zu nutzen. Im Rahmen des neuen Produkts führt Microsoft am 1. November 2016 neue Microsoft Dynamics-Abonnementpläne für Kunden ein, die den aktuellen Plänen zwar ähnlich, jedoch nicht mit diesen identisch sind.

Die Anweisungen in diesem Dokument beschrieben, wie indirekte Anbieter vorhandene Microsoft Dynamics AX-Abonnements von Kunden zum neuen Microsoft Dynamics 365 migrieren können. Die Anweisungen gelten auch für andere Microsoft-Produkte, die auf neue Versionen aktualisiert werden, sodass Anbieter Kundenabonnements zu einer neuen SKU migrieren müssen.

**Änderungen für die Microsoft Dynamics AX-Lizenzierung**

Die Microsoft Dynamics AX-Produktlinie wird mit Wirkung vom 1. November 2016 eingestellt. Weitere Informationen zu den neuen Lizenzierungsoptionen für Dynamics 365 finden Sie im Lizenzierungshandbuch, das in Kürze veröffentlicht wird. Die folgende Tabelle enthält Details zur Lizenzzuordnung:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Eingestellte Dynamics AX-Lizenz</strong></p></td>
<td><p><strong>Dynamics 365-Lizenz</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Dynamics 365 Enterprise Edition Plan 2</p>
<p>ODER Dynamics 365 for Operations</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Task</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Functional</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Device</p></td>
<td><p>Dynamics 365 for Operations Device</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

Der aktuelle Microsoft Dynamics CRM Online-Plan wird mit Wirkung vom 1. November 2016 eingestellt. Weitere Informationen zu neuen Lizenzierungsoptionen finden Sie unter [Wichtige Informationen für CRM Online-Kunden](https://go.microsoft.com/fwlink/?linkid=831667).

## Migrieren von Kunden zu neuen Produktplänen


Microsoft bietet Wiederverkäufern und Anbietern kontinuierlich neue Produkte und Dienste an. In diesen Fällen müssen Wiederverkäufer Kunden möglicherweise auf neue Dienste aktualisieren oder Kundenabonnements von alten SKUs, die letzten Endes vom Markt genommen werden, zu neueren SKUs migrieren. Die Migration von Kunden von alten SKUs auf neuere SKUs muss in dieser Reihenfolge erfolgen:

-   [Kauf des neuen Abonnements](#manual-subscription-migration-purchasenewsubsc);
-   [Neuzuweisen der aktuellen Benutzerlizenzen](#manual-subscription-migration-reassignlicenses);
-   [Stornieren des alten Abonnements](#manual-subscription-migration-cancelsubscriptions).

Mit den folgenden Verfahren migrieren Sie einen Kunden von Dynamics AX7 Enterprise zu Dynamics 365 for Operations.

<a href="" id="purchasenewsubsc"></a>
Der Wiederverkäufer muss einen Kunden mit einem vorhandenen Dynamics AX Enterprise-Abonnement zu Dynamics 365 for Operations migrieren. Der erste Schritt besteht im Kauf von Dynamics 365 for Operations.

**Kauf des neuen Abonnements**

1.  Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend **Abonnements hinzufügen** aus.
2.  Wählen Sie aus dem Katalog das Abonnement aus, das Sie kaufen möchten (in diesem Fall Dynamics 365 for Operations Enterprise Edition), kaufen Sie die nötigen Anzahl von Lizenzen, und wählen Sie **Übermitteln** aus.

    Ihr Kunde sollte nun alte und neue Abonnements besitzen. In diesem Beispiel sind dies das alte Dynamics AX Enterprise-Abonnement und das neue Abonnement von Dynamics 365 for Operations Enterprise Edition.

<a href="" id="reassignlicenses"></a>
Im nächsten Schritt werden alle vorhandenen Benutzerlizenzen dem neuen Abonnement neu zugewiesen.

**Neuzuweisen von Benutzerlizenzen**

1.  Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend **Benutzer und Lizenzen** aus. Die Seite mit Benutzern und Lizenzen des Kunden wird geöffnet.
2.  Um Benutzerlizenzen neu zuzuweisen, wählen Sie den Benutzer aus, der neu zugewiesen werden soll, und anschließend **Verwalten von Lizenzen**.
3.  Deaktivieren Sie auf der Seite **Verwalten von Lizenzen** das Kontrollkästchen für die Lizenz **Dynamics AX Enterprise**, und wählen Sie die Lizenz **Dynamics 365 for Operations** aus.
4.  Wählen Sie **Übermitteln** aus. Anschließend werden auf einer Bestätigungsseite die neuen Lizenzzuweisungen aufgeführt.
5.  Führen Sie diese Schritte für alle Benutzer des Kunden aus, deren Lizenz neu zugewiesen werden muss.

<a href="" id="cancelsubscriptions"></a>
Nachdem Sie die Benutzerlizenzen zum neuen Dienst migriert haben, können Sie das alte Abonnement auf der obersten Kundenebene ohne Bedenken stornieren.

**Stornieren des alten Abonnements.**

1.  Wählen Sie im Menü **Dashboard**&nbsp;**Kunden** aus, und wählen Sie den Kunden aus, den Sie migrieren möchten. Wählen Sie anschließend das Abonnement aus, das Sie stornieren möchten.
2.  Legen Sie auf der Seite für Abonnementdetails **Status** auf **Ausgesetzt** fest.
3.  Wählen Sie **Übermitteln** aus.

Das alte Abonnement ist nun ausgesetzt, und das neue Abonnement ist aktiv. Die Bereitstellung des ausgesetzten Abonnements wird nach 120 Tagen automatisch aufgehoben. Für den Kunden fallen für das alte Abonnement keine zusätzlichen Kosten an.

## Weitere Aspekte


Wenn Kunden vom Open-Programm zum Programm für Cloud-Lösungsanbieter wechseln, um weitere Abonnements bereitzustellen, müssen Sie die vorhandenen Abonnements ebenfalls migrieren:

-   Wenn Kunden das alte Abonnement über das Open-Programm erhalten haben, ist die Migration zum CSP-Programm für die neue SKU einfach.
-   Wenn Kunden noch nicht als Ihre Kunden eingerichtet sind, können Sie diese einladen. Weitere Informationen finden Sie im Hilfethema [Anfordern einer Beziehung zu einem Kunden](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Nachdem der Kunde Sie als indirekten Anbieter akzeptiert hat, sind die Bereitstellungsschritte größtenteils mit den oben beschriebenen Schritten identisch: Sie kaufen das neue Abonnement und weisen die Benutzerlizenzen zu. Der einzige Unterschied besteht in der Stornierung des/der alten Abonnements. Ein neuer Anbieter kann keine Abonnements aussetzen/stornieren, die über andere Kanäle gekauft wurden. Wenn ein Kunde zuvor Abonnements über einen anderen Vertriebskanal gekauft hat, beispielsweise Open, muss der Kunde die Abonnements selbst über diesen Kanal stornieren.

 

 






<!--HONumber=Jan17_HO2-->


