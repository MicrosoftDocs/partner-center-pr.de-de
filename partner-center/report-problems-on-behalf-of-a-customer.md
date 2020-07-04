---
title: Melden von Problemen im Auftrag eines Kunden
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wann es sinnvoll ist, ein Kundendienst Problem an Microsoft zu eskalieren und ein Support Ticket dafür zu erhalten.
author: BrentSerbus
ms.author: brserbus
Keywords: Serviceanfrage, Serviceticket, Support, Supportanspruch, AOBO, Azure-AOBO
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 512b8b51dd036bb6428a3f5f730c36168c5fa455
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949277"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Melden eines Dienst Problems im Namen eines Kunden, einschließlich des Zeit-und Vorgehensweise

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

Wenn Ihr Kunde ein Dienst Problem hat, das Sie nicht beheben können, und das die unter [eskalieren von Problemen an Microsoft](escalate-problems-to-microsoft.md)beschriebenen Kriterien erfüllt, müssen Sie ein Support Ticket für Sie einreichen. Dieser Vorgang eignet sich auch zum Eskalieren von Abrechnungsproblemen oder -streitigkeiten und Betrugsverdachtsfällen.

## <a name="submit-a-service-request-for-a-customer"></a>Übermitteln einer Serviceanfrage für einen Kunden

1. Wählen Sie vom **Partner Center**-Menü **Serviceanfragen** und dann **Kundenanfragen** aus. 

2. Suchen Sie auf der Seite der Kundenanforderungen die gewünschten Kunden aus.

3. Wählen Sie aus dem Dropdownmenü **Neue Anforderung** entweder **Azure** oder **Office 365, Dynamics 365, Enterprise Mobility Suite** aus. Sie werden entweder an die Microsoft Azure-Portal oder an das Office 365 Admin Center umgeleitet.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Wenn Sie eine Serviceanfrage für Ihren Kunden in Azure erstellen möchten, beachten Sie Folgendes:
>
>- Damit Sie in Azure Serviceanfragen für Ihren Kunden erstellen können, muss Ihnen Ihr indirekter Anbieter Zugriff auf das Azure-Konto des Kunden gewähren. Dies unterscheidet sich von der Verwaltung im Auftrag von Kunden für Office 365.
>
>- Der Helpdesk-Administrator in Partner Center kann zwar keine Serviceanfragen im Azure-Serviceportal erstellen, er kann jedoch eine Supportgruppe im Azure-Serviceportal erstellen und dieser Gruppe Berechtigungen zum Protokollieren von Supportanfragen zuweisen.

1. Wählen Sie **Neue Supportanfrage** aus.

2. Füllen Sie die Supportanfrage mit den entsprechenden Informationen aus, und wählen Sie dann **Erstellen**:

   - Wählen Sie im Abschnitt **Grundlagen** im Feld **Supportplan** die Option **Cloud-Lösungsanbieter**.

   - Geben Sie im Abschnitt **Kontakt** der Supportanfrage Ihre Informationen und nicht die Ihres Kunden ein.

3. Überprüfen Sie später die Serviceanfragen Ihrer Kunden über das Microsoft Azure-Portal, indem Sie **Supportanfragen verwalten** wählen.

Unter Umständen müssen Sie eine Supportanfrage für einen Kunden erstellen, wenn Sie für diesen Kunden nicht über Administratorberechtigungen verfügen. Dies kann in einem der folgenden Szenarios auftreten:

- Bei der erstmaligen Einrichtung der Beziehung haben Sie keine Administratorrechte angefordert.
- Sie verwalten die Azure-Abonnements eines Kunden und keine anderen, für die keine Administrator Berechtigungen erforderlich sind.
 
In beiden Fällen können Sie das folgende Verfahren zum Erstellen einer Supportanfrage anwenden. 

1. Kopieren Sie den Domänen Namen des Kunden von der Kontoseite im Partner Center.

2. Wechseln Sie zu https://portal.azure.com/[customerdomainname]. 

3. Wählen Sie das Azure-Abonnement aus, für das Support benötigt wird.

4. Wählen Sie **Neue Supportanfrage** aus, und befolgen Sie anschließend die Anweisungen zum Erstellen einer Anfrage. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Wählen Sie im Abschnitt **Serviceanfrage erstellen** die geeignete Supportkategorie aus. Möglicherweise müssen Sie **mehr auswählen...** , um weitere Themen anzuzeigen.    

2. Vervollständigen Sie das Service Request Formular, und wählen Sie **senden**aus.

   > [!TIP]
   > Denken Sie daran, Ihre Kontaktinformationen und nicht die Ihres Kunden anzugeben.

3. Überprüfen Sie später die Service Requests Ihres Kunden, indem Sie zum Office 365 Admin Center wechseln und **alle Support Tickets**anzeigen auswählen.

### <a name="support-for-commercial-marketplace-products"></a>Support für Produkte des kommerziellen Marketplace

Microsoft bietet keinen Produktsupport für Produkte des kommerziellen Marketplace an. Sie müssen sich an den unabhängigen Software Hersteller (Independent Software Vendor, ISV) wenden, der das Produkt veröffentlicht hat, um Support zu erhalten.

So finden Sie Kontaktdaten des ISV:

1.  Wählen Sie auf der Seite **Marketplace** das Produkt aus, zu dem Sie Hilfe benötigen.

2.  Auf der Seite des Produkts finden Sie Support-Kontaktinformationen. Dies kann Folgendes umfassen:

    - Einen Supportlink auf der Website des ISV
    - Eine Support-E-Mail-Adresse
    - Eine Supportrufnummer

## <a name="faq"></a>FAQ

**Was ist Bestandteil des Supportanspruchs?**

Serviceanfragen sollten über das Partner Center eingereicht werden. Sie sind für Azure, Microsoft Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite verfügbar. Partner, die am Cloud Solution Provider-Programm teilnimmt, werden bei schwerwiegenden Problemen bevorzugt behandelt.

Die Unterstützung für Ihren eigenen Partnermandanten ist nicht Bestandteil des CSP-Supportvorteils. Für Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite werden jedoch keine separaten Abonnementgebühren für den Support für Partner oder Kunden berechnet. Azure erhebt eine Gebühr, aber wenn Sie Anspruch auf Signature Cloud Support oder andere Microsoft Partner Network (MPN)-Vorteile haben, können Sie damit die Gebühr bezahlen.

Dieser Vorteil wird Partnern, die am kostenpflichtigen Cloud Solution Provider-Programm teilnehmen, ebenso gewährt wie Partnern, die den Testzeitraum nutzen. Support für die Abrechnung und Abonnementverwaltung ist auch als kostenlose Komponente in diesem Paket enthalten.

**Wie schnell erhalte ich eine erste Antwort?**

Unsere Reaktionszeiten hängen vom Schweregrad des übermittelten Ereignisses ab. Der Schweregrad eines Problems wird durch die bei der Übermittlung der Serviceanfrage angegebenen geschäftlichen Auswirkungen festgelegt.

Die anfänglichen Reaktionszeiten für **technische Problemlösungsfälle** sind wie folgt:

- Kritische Auswirkungen (Schweregrad A): 2 Stunden (Erhebliche Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Ausfall der Produktionssdienste.)
- Mittlere Auswirkungen (Schweregrad B): 4 Stunden (Mäßige Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Produktionsdienste teilweise betroffen.)
- Minimale Auswirkungen (Schweregrad C): 8 Stunden (Minimale Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Dienste sind weiterhin verfügbar oder es sind Dienste ohne Auswirkungen auf die Produktion betroffen.)

Die anfänglichen Reaktionszeiten gelten nur für englischsprachigen Support. Support in der Landessprache steht nur während der Geschäftszeiten zur Verfügung.
Für Fälle, die innerhalb der Grenzen des Supportanspruchs liegen, jedoch keine Break-Fix-Ereignisse sind, kann die anfängliche Reaktionszeit bis zu einem Werktag betragen.

**Kann ich eine Serviceanfrage per Telefon übermitteln?**

Nein, für dieses Programm wird kein telefonischer Support angeboten.

**Was geschieht, wenn ich mich beim Azure-Portal anmelde und Partner Center umgehe?**

Wenn Sie sich direkt beim Microsoft Azure-Portal anmelden, wird das Center in Ihrem eigenen Kontext angezeigt, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Microsoft Azure-Portal anmelden, wenn Sie eine Serviceanfrage für Ihre eigenen Abonnements erstellen.

Ihr Anspruch auf Support für das CSP-Programm umfasst keinen Support für Ihr eigenes Partnerabonnement. Wenn Sie also eine Serviceanfrage erstellen, die sich auf Ihr eigenes Partnerabonnement bezieht, müssen Sie einen gültigen Supportplan nachweisen. Beispiele für Nachweise sind die MPN-Vertrags-ID, ein Premier- oder ein Azure-Supportplan. Informationen dazu finden Sie auf der Seite [Häufig gestellte Fragen zum Azure-Support](https://go.microsoft.com/fwlink/?LinkId=717532).

**Was geschieht, wenn ich mich beim Office 365 Admin Center-Portal anmeldet und Partner Center umgehe?**

Wenn Sie sich direkt beim Office 365 Admin Center anmelden, sehen Sie das Center in Ihrem eigenen Kontext und nicht im Kontext eines Kunden. Daher sollten Sie sich beim Erstellen eines Service Request für Ihre eigenen Abonnements nur direkt beim Office 365 Admin Center anmelden.

**Wie kann ich zusätzlichen Dynamics 365-Support anfordern?**

Bei Problemen im Zusammenhang mit: Dynamics 365 planen Sie Abonnements, Lizenzierung, Abrechnung, Finanzen & Vorgängen, Dynamics 365-Produktlizenzen oder benötigen Sie technischen Support:
 
Wenden Sie sich an [Dynamics-Support](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support).

Lesen Sie [Support für Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur).
