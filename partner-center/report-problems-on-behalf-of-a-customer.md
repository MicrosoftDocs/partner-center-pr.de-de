---
title: Melden von Problemen im Auftrag eines Kunden
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wann Sie ein Kundendienst Problem an Microsoft eskalieren und wie Sie ein Support Ticket einreichen.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 01a4fb132d2ec396bfe45e22cccdabc7f2d15a2e
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811320"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Melden eines Dienst Problems im Namen eines Kunden, einschließlich des Zeit-und Vorgehensweise

**Zielgruppe**

- Partner Center
- Partner Center für Microsoft Cloud for US Government

Wenn Ihr Kunde ein Dienst Problem hat, das Sie nicht beheben können, und das die unter [eskalieren von Problemen an Microsoft](escalate-problems-to-microsoft.md)beschriebenen Kriterien erfüllt, können Sie ein Support Ticket für Sie einreichen. Dieser Vorgang eignet sich auch zum Eskalieren von Abrechnungsproblemen oder -streitigkeiten und Betrugsverdachtsfällen. 

## <a name="submit-a-service-request-for-a-customer"></a>Übermitteln einer Serviceanfrage für einen Kunden

1. Wählen Sie vom **Partner Center**-Menü **Serviceanfragen** und dann **Kundenanfragen** aus. 

2. Suchen Sie auf der Seite der Kundenanforderungen die gewünschten Kunden aus.

3. Wählen Sie aus dem Dropdownmenü **Neue Anforderung** entweder **Azure** oder **Office 365, Dynamics 365, Enterprise Mobility Suite** aus. Sie werden entweder an die Microsoft Azure-Portal oder an das Office 365 Admin Center umgeleitet.

>[!NOTE]
>Unterstützung von Betriebs Partnern, die Dynamics 365 im CSP-Dienst unterstützen, sind erforderlich, um eine Supportvereinbarung des Advanced Support for Partner (asfp)-Plans oder höher aufrechtzuerhalten. Diese Supportvereinbarung ist erforderlich, um Dynamics 365-Vorfälle im Auftrag eines CSP-Kunden zu übermitteln. [Weitere](https://partner.microsoft.com/support/partnersupport) Informationen zu den Optionen für die Supportvereinbarung.

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

Sie müssen möglicherweise eine Supportanfrage für einen Kunden erstellen, wenn Sie nicht über Administrator Berechtigungen für diesen Kunden verfügen. Dies kann in einem der folgenden Szenarios auftreten:

- Beim ersten feststellen der Beziehung haben Sie keine Administrator Berechtigungen angefordert.
- Sie verwalten nur die Azure-Abonnements eines Kunden, sodass Sie nicht über Administrator Berechtigungen verfügen.
 
In beiden Fällen können Sie das folgende Verfahren zum Erstellen einer Supportanfrage anwenden. 

1. Kopieren Sie den Domänen Namen des Kunden von der Kontoseite im Partner Center.

2. Wechseln Sie zu https://portal.azure.com/[customerdomainname]. 

3. Wählen Sie das Azure-Abonnement aus, für das Support benötigt wird.

4. Wählen Sie **Neue Supportanfrage** aus, und befolgen Sie anschließend die Anweisungen zum Erstellen einer Anfrage. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Wählen Sie im Abschnitt **Service Request erstellen** die entsprechende Support Kategorie aus. Möglicherweise müssen Sie **mehr auswählen...** , um weitere Artikel anzuzeigen.

2. Vervollständigen Sie das Service Request Formular, und wählen Sie **senden**aus.

   > [!TIP]
   > Denken Sie daran, Ihre Kontaktinformationen und nicht die Ihres Kunden anzugeben.

3. Überprüfen Sie später die Service Requests Ihres Kunden, indem Sie zum Office 365 Admin Center wechseln und **alle Support Tickets**anzeigen auswählen.

### <a name="support-for-commercial-marketplace-products"></a>Support für Produkte des kommerziellen Marketplace

Microsoft bietet keine Produktunterstützung für kommerzielle Marketplace-Produkte. Sie müssen sich an den unabhängigen Software Hersteller (Independent Software Vendor, ISV) wenden, der das Produkt veröffentlicht hat, um Support zu erhalten.

So finden Sie Kontaktdaten des ISV:

1.  Wählen Sie auf der Seite **Marketplace** das Produkt aus, zu dem Sie Hilfe benötigen.

2.  Auf der Seite des Produkts finden Sie Support-Kontaktinformationen. Dies kann eine oder mehrere der folgenden Optionen sein:

    - Einen Supportlink auf der Website des ISV
    - Eine Support-E-Mail-Adresse
    - Eine Supportrufnummer

## <a name="faq"></a>Häufig gestellte Fragen

**Was ist Bestandteil des Supportanspruchs?**

Service Requests sollten über Partner Center abgelegt werden. Sie sind für Azure, Microsoft Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite verfügbar. Partner, die am Cloud Solution Provider-Programm teilnimmt, werden bei schwerwiegenden Problemen bevorzugt behandelt.

Die Unterstützung für Ihren eigenen Partner Mandanten ist nicht im Rahmen des CSP-Support-Vorteils enthalten. Allerdings berechnen Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite keine separaten Support Abonnementgebühren für Partner oder Kunden. Azure berechnet eine Gebühr, aber wenn Sie berechtigt sind, Cloud-Support oder andere Microsoft Partner Network (MPN) zu unterstützen, können Sie diese Gebühren nutzen, um diese Gebühren zu bezahlen.

Dieser Vorteil wird Partnern, die am kostenpflichtigen Cloud Solution Provider-Programm teilnehmen, ebenso gewährt wie Partnern, die den Testzeitraum nutzen. Support für die Abrechnung und Abonnementverwaltung ist auch als kostenlose Komponente in diesem Paket enthalten.

**Wie schnell erhalte ich eine erste Antwort?**

Unsere Reaktionszeiten hängen vom Schweregrad des übermittelten Ereignisses ab. Der Schweregrad eines Problems wird durch die bei der Übermittlung der Serviceanfrage angegebenen geschäftlichen Auswirkungen festgelegt.

Anfängliche Reaktionszeiten für **technische Fehlerbehebung**:

- Kritische Auswirkungen (Schweregrad A): 2 Stunden (Erhebliche Ausfälle oder Beeinträchtigungen in Bezug auf Dienste. Ausfall der Produktionssdienste.)
- Moderate Auswirkung (Schweregrad B): vier Stunden (mittlerer Verlust oder Verschlechterung der Dienste. Die Produktions Dienste sind teilweise betroffen.)
- Minimale Auswirkung (Schweregrad C): acht Stunden (minimaler Verlust oder Verschlechterung der Dienste. Dienste sind weiterhin verfügbar oder nicht-Produktions Dienste betroffen.)

Die anfänglichen Reaktionszeiten gelten nur für englischsprachigen Support. Support in der Landessprache steht nur während der Geschäftszeiten zur Verfügung.
Bei Vorfällen, die innerhalb der Grenzen der Support Berechtigung liegen, aber nicht als Fehlerbehebung für Vorfälle angesehen werden, kann die anfängliche Antwortzeit bis zu einem Werktag betragen.

**Kann ich eine Serviceanfrage per Telefon übermitteln?**

Nein, der telefonischen Support wird für dieses Programm nicht angeboten.

**Was geschieht, wenn ich mich beim Azure-Portal anmelde und Partner Center umgehe?**

Wenn Sie sich direkt bei der Microsoft Azure-Portal anmelden, sehen Sie das Center in Ihrem eigenen Kontext und nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich beim Erstellen eines Service Request für Ihre eigenen Abonnements nur direkt beim Microsoft Azure-Portal anmelden.

Ihre CSP-Programm Unterstützungs Berechtigung bietet keine Unterstützung für Ihr eigenes Partner Abonnement. Aus diesem Grund müssen Sie Ihre gültige Support Plan Berechtigung angeben, wenn Sie eine Service Request erstellen, die ihr eigenes Partner Abonnement betrifft. Beispiele hierfür sind MPN Contract ID, Premier oder ein Azure-Support Plan. Weitere Informationen finden Sie unter Häufig gestellte Fragen zum [Azure-Support](https://go.microsoft.com/fwlink/?LinkId=717532).

**Was geschieht, wenn ich mich beim Office 365 Admin Center-Portal anmeldet und Partner Center umgehe?**

Wenn Sie sich direkt beim Office 365 Admin Center anmelden, sehen Sie das Center in Ihrem eigenen Kontext und nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich beim Erstellen eines Service Request für Ihre eigenen Abonnements nur direkt beim Office 365 Admin Center anmelden.

**Wie kann ich zusätzlichen Dynamics 365-Support anfordern?**

Bei Problemen im Zusammenhang mit: Dynamics 365 planen Sie Abonnements, Lizenzierung, Abrechnung, Finanzen & Vorgänge, Dynamics 365-Produktlizenzen oder benötigen Sie technischen Support:
 
Wenden Sie sich an [Dynamics-Support](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support).

Lesen Sie [Support für Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur).

## <a name="next-steps"></a>Nächste Schritte

- [Bereitstellen von Support für Kunden](customer-support.md)
- [Überprüfen der Dienstintegrität](check-service-health.md)
