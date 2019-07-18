---
title: Melden von Problemen im Auftrag eines Kunden | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Wenn ein Kunde ein Problem mit einem Dienst meldet, das Sie nicht beheben können und das die unter „Eskalieren von Problemen an Microsoft“ beschriebenen Kriterien erfüllt, beantragen Sie ein Supportticket für den Kunden.
ms.assetid: 417E8EE3-EBD2-41DA-BF6E-DD935BE78EF5
author: MaggiePucciEvans
ms.author: evansma
Keywords: Serviceanfrage, Serviceticket, Support, Supportanspruch, AOBO, Azure-AOBO
ms.localizationpriority: medium
ms.openlocfilehash: b43652e4d0e73b73bd4e0caf7f9eb4fc7f4a5bcd
ms.sourcegitcommit: 9156f3a7711fae5e0f9a2c5f29e74e8791836c8e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2019
ms.locfileid: "67818754"
---
# <a name="report-problems-on-behalf-of-a-customer"></a>Melden von Problemen im Auftrag eines Kunden

**Gilt für**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government


Wenn ein Kunde ein Problem mit einem Dienst meldet, das Sie nicht beheben können und das die unter [Eskalieren von Problemen an Microsoft](escalate-problems-to-microsoft.md) beschriebenen Kriterien erfüllt, beantragen Sie ein Supportticket für den Kunden. Dieser Vorgang eignet sich auch zum Eskalieren von Abrechnungsproblemen oder -streitigkeiten und Betrugsverdachtsfällen.

## <a name="submit-a-service-request-for-a-customer"></a>Übermitteln einer Serviceanfrage für einen Kunden

1.  Wählen Sie vom **Partner Center**-Menü **Serviceanfragen** und dann **Kundenanfragen** aus. 

2.  Suchen Sie auf der Seite der Kundenanforderungen die gewünschten Kunden aus.

3.  Wählen Sie aus dem Dropdownmenü **Neue Anforderung** entweder **Azure** oder **Office 365, Dynamics 365, Enterprise Mobility Suite** aus. Sie werden zum Microsoft Azure-Portal oder Office 365 Admin Center umgeleitet.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Wenn Sie eine Serviceanfrage für Ihren Kunden in Azure erstellen möchten, beachten Sie Folgendes:
>
>- Damit Sie in Azure Serviceanfragen für Ihren Kunden erstellen können, muss Ihnen Ihr indirekter Anbieter Zugriff auf das Azure-Konto des Kunden gewähren. Dies unterscheidet sich von der Verwaltung im Auftrag von Kunden für Office 365. 
>
>- Der Helpdesk-Administrator in Partner Center kann zwar keine Serviceanfragen im Azure-Serviceportal erstellen, er kann jedoch eine Supportgruppe im Azure-Serviceportal erstellen und dieser Gruppe Berechtigungen zum Protokollieren von Supportanfragen zuweisen.

1. Wählen Sie **Neue Supportanfrage** aus.
2. Füllen Sie die Supportanfrage mit den entsprechenden Informationen aus, und wählen Sie dann **Erstellen**:
-   Wählen Sie im Abschnitt **Grundlagen** im Feld **Supportplan** die Option **Cloud-Lösungsanbieter**.
-   Geben Sie im Abschnitt **Kontakt** der Supportanfrage Ihre Informationen und nicht die Ihres Kunden ein.

3. Überprüfen Sie später die Serviceanfragen Ihres Kunden im Microsoft Azure-Portal, indem Sie **Supportanfragen verwalten** auswählen.

Unter Umständen müssen Sie eine Supportanfrage für einen Kunden erstellen, wenn Sie für diesen Kunden nicht über Administratorberechtigungen verfügen. Dies kann in einem der folgenden Szenarios auftreten: 
 
-   Bei der erstmaligen Einrichtung der Beziehung haben Sie keine Administratorrechte angefordert.
-   Sie verwalten das Azure-Abonnement eines Kunden und keine anderen, weshalb Sie keine Administratorberechtigungen benötigen.
 
In beiden Fällen können Sie das folgende Verfahren zum Erstellen einer Supportanfrage anwenden. 

1. Kopieren Sie den Domänennamen des Kunden von dessen Kontoseite in Partner Center.

2. Wechseln Sie zu https://portal.azure.com/ [customerdomainname]. 

3. Wählen Sie das Azure-Abonnement aus, für das Support benötigt wird.

4. Wählen Sie **Neue Supportanfrage** aus, und befolgen Sie anschließend die Anweisungen zum Erstellen einer Anfrage. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Wählen Sie im Abschnitt **Serviceanfrage erstellen** die geeignete Supportkategorie aus. Möglicherweise müssen Sie **Mehr...** auswählen, um weitere Themen anzuzeigen.    
2. Füllen Sie das Formular für die Serviceanfrage aus, und wählen Sie **Übermitteln** aus.

   > [!TIP]
   > Denken Sie daran, Ihre Kontaktinformationen und nicht die Ihres Kunden anzugeben.

3. Überprüfen Sie später die Serviceanfragen Ihres Kunden, indem Sie zum Office 365 Admin Center wechseln und **Alle Supporttickets anzeigen** auswählen.

### <a name="support-for-azure-marketplace-products"></a>Support für Azure Marketplace-Produkte

Microsoft bietet keinen Produktsupport für Azure Marketplace-Produkte an. Wenden Sie sich an den unabhängigen Softwarehersteller (ISV), der das Produkt veröffentlicht hat, wenn Sie Support benötigen.

So finden Sie Kontaktdaten des ISV:

1.  Wählen Sie auf der Marketplace-Seite das Produkt aus, zu dem Sie Hilfe benötigen.
2.  Auf der Produktseite finden Sie Kontaktinformationen für Support. Dies kann Folgendes umfassen:
    - Einen Supportlink auf der Website des ISV
    - Eine Support-E-Mail-Adresse 
    - Eine Supportrufnummer

## <a name="faq"></a>FAQ

**Was ist Bestandteil des Supportanspruchs?**

Serviceanfragen sollten über das Partner Center eingereicht werden. Sie sind für Azure, Microsoft Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite verfügbar. Als Partner, der am Cloud Solution Provider-Programm teilnimmt, können Sie die Prioritäts Antwortzeit für Ihre wichtigsten Probleme erwarten.

Die Unterstützung für Ihren eigenen Partnermandanten ist nicht Bestandteil des CSP-Supportvorteils. Für Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite werden jedoch keine separaten Abonnementgebühren für den Support für Partner oder Kunden berechnet. Azure erhebt eine Gebühr, aber wenn Sie Anspruch auf Signature Cloud Support oder andere Microsoft Partner Network (MPN)-Vorteile haben, können Sie damit die Gebühr bezahlen.

Dieser Vorteil gilt für alle Partner, die am Cloud Solution Provider-Programm teilnehmen, unabhängig davon, ob diese kostenpflichtig sind. Support für die Abrechnung und Abonnementverwaltung ist auch als kostenlose Komponente in diesem Paket enthalten.

**Wie schnell erhalte ich eine erste Antwort?**

Unsere Reaktionszeiten hängen vom Schweregrad des übermittelten Ereignisses ab. Der Schweregrad eines Problems wird durch die bei der Übermittlung der Serviceanfrage angegebenen geschäftlichen Auswirkungen festgelegt.

Die anfänglichen Reaktionszeiten für **technische Problemlösungsfälle** sind wie folgt:

-   Kritische Auswirkungen (Schweregrad A): 2 Stunden (erhebliche Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Ausfall der Produktionssdienste.)
-   Mittlere Auswirkung (Schweregrad B): 4 Stunden (mittelschwere Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Produktionsdienste teilweise betroffen.)
-   Minimale Auswirkungen (Schweregrad C): 8 Stunden (minimale Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Dienste sind weiterhin verfügbar oder es sind Dienste ohne Auswirkungen auf die Produktion betroffen.)

Die anfänglichen Reaktionszeiten gelten nur für englischsprachigen Support. Support in der Landessprache steht nur während der Geschäftszeiten zur Verfügung.
Für Fälle, die innerhalb der Grenzen des Supportanspruchs liegen, jedoch keine Break-Fix-Ereignisse sind, kann die anfängliche Reaktionszeit bis zu einem Werktag betragen.

**Kann ich eine Serviceanfrage per Telefon übermitteln?**

Nein, für dieses Programm wird kein telefonischer Support angeboten.

**Was geschieht, wenn ich mich beim Azure-Portal anmelde und Partner Center umgehe?**

Wenn Sie sich direkt beim Microsoft Azure-Portal anmelden, wird das Center in Ihrem eigenen Kontext angezeigt, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Microsoft Azure-Portal anmelden, wenn Sie eine Serviceanfrage für Ihre eigenen Abonnements erstellen.

Ihre CSP-Programm Unterstützungs Berechtigung bietet keine Unterstützung für Ihr eigenes Partner Abonnement. Wenn Sie also eine Service Request erstellen, die ihr eigenes Partner Abonnement betrifft, müssen Sie Ihre gültige Support Plan Berechtigung angeben. Beispiele für Nachweise sind die MPN-Vertrags-ID, ein Premier- oder ein Azure-Supportplan. Informationen dazu finden Sie auf der Seite [Häufig gestellte Fragen zum Azure-Support](https://go.microsoft.com/fwlink/?LinkId=717532).

**Was geschieht, wenn ich mich beim Office 365 Admin Center-Portal anmelde und Partner Center umgehe?**

Wenn Sie sich direkt beim Office 365 Admin Center anmelden, wird das Center in Ihrem eigenen Kontext angezeigt, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Office 365 Admin Center anmelden, wenn Sie eine Serviceanfrage für Ihre eigenen Abonnements erstellen.

**Wie kann ich zusätzlichen Dynamics 365-Support anfordern?**

Wenn Probleme im Zusammenhang mit Dynamics 365 Planen von Abonnements, Lizenzierung, Abrechnung, Finanz & Vorgängen, Dynamics 365-Produktlizenzen oder benötigen technischen Support:
 
Wenden Sie sich an [Dynamics-Support](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support).

Lesen Sie [Support für Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur).



