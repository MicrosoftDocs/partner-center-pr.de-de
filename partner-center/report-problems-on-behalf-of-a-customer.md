---
title: Melden von Problemen im Auftrag eines Kunden
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wann Sie ein Kundendienstproblem an Microsoft eskalieren und wie Sie ein Supportticket für verschiedene Arten von Microsoft-Dienste erstellen.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ba25d0bfc4796ca43d36bb34bf6d9e82889881c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855708"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Melden eines Dienstproblems im Auftrag eines Kunden – einschließlich wann und wie dies zu tun ist

**Gilt für**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Geeignete Rollen:** Globaler Administrator

Wenn bei Ihrem Kunden ein Dienstproblem auftritt, das Sie nicht lösen können und das die unter [Eskalieren](escalate-problems-to-microsoft.md)von Problemen an Microsoft beschriebenen Kriterien erfüllt, kann Ihr indirekter Anbieter ein Supportticket für den Kunden erstellen. Dieser Vorgang eignet sich auch zum Eskalieren von Abrechnungsproblemen oder -streitigkeiten und Betrugsverdachtsfällen.

## <a name="submit-a-service-request-for-a-customer"></a>Übermitteln einer Serviceanfrage für einen Kunden

1. Wählen Sie im Partner Center-Menü unter „CSP“ die Option **Customers** (Kunden) aus.

2. Wählen Sie auf der Seite Kunden den gewünschten Kunden aus, oder suchen Sie nach diesem.
    
3. Wählen Sie im Kundenmenü **Service Requests** (Serviceanfragen) aus.

4. Wählen Sie aus dem Dropdownmenü **Neue Anforderung** entweder **Azure** oder **Office 365, Dynamics 365, Enterprise Mobility Suite** aus. Sie werden entweder zum Microsoft Azure-Portal oder zum Office 365 Admin Center umgeleitet.

>[!NOTE]
>Supportbetriebspartner, die Dynamics 365 in CSP durchführen, müssen eine Supportvereinbarung des ASfP-Plans (Advanced Support for Partner) oder höher einhalten. Diese Supportvereinbarung ist erforderlich, um Dynamics 365-Vorfälle im Auftrag eines CSP-Kunden zu übermitteln. [Erfahren Sie mehr](https://partner.microsoft.com/support/partnersupport) über die Supportvereinbarungsoptionen.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Wenn Sie eine Serviceanfrage für Ihren Kunden in Azure erstellen möchten, beachten Sie Folgendes:
>
>- Damit Sie als indirekter Vertriebspartner Serviceanfragen für Ihren Kunden in Azure erstellen können, muss Ihr indirekter Anbieter Ihnen Zugriff auf das Azure-Konto des Kunden gewähren. Dies unterscheidet sich von der Verwaltung im Auftrag von Kunden für Office 365.
>
>- Der Helpdesk-Administrator in Partner Center kann zwar keine Serviceanfragen im Azure-Serviceportal erstellen, er kann jedoch eine Supportgruppe im Azure-Serviceportal erstellen und dieser Gruppe Berechtigungen zum Protokollieren von Supportanfragen zuweisen.

1. Wählen Sie **Neue Supportanfrage** aus.

2. Füllen Sie die Supportanfrage mit den entsprechenden Informationen aus, und wählen Sie dann **Erstellen**:

   - Wählen Sie im Abschnitt **Grundlagen** im Feld **Supportplan** die Option **Cloud-Lösungsanbieter**.

   - Geben Sie im Abschnitt **Kontakt** der Supportanfrage Ihre Informationen und nicht die Ihres Kunden ein.

3. Überprüfen Sie später die Serviceanfragen Ihrer Kunden über das Microsoft Azure-Portal, indem Sie **Supportanfragen verwalten** wählen.

Möglicherweise müssen Sie eine Supportanfrage für einen Kunden erstellen, wenn Sie nicht über Administratorberechtigungen für diesen Kunden verfügen. Dies kann in einem der folgenden Szenarios auftreten:

- Sie haben keine Administratorrechte angefordert, als Sie die Beziehung zum ersten Mal eingerichtet haben.
- Sie verwalten nur die Azure-Abonnements eines Kunden, sodass Sie nicht über Administratorberechtigungen verfügen.
 
In beiden Fällen können Sie das folgende Verfahren zum Erstellen einer Supportanfrage anwenden. 

1. Kopieren Sie den Domänennamen des Kunden von der Kontoseite in Partner Center.

2. Wechseln Sie zu https://portal.azure.com/[customerdomainname]. 

3. Wählen Sie das Azure-Abonnement aus, für das Support benötigt wird.

4. Wählen Sie **Neue Supportanfrage** aus, und befolgen Sie anschließend die Anweisungen zum Erstellen einer Anfrage. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Wählen Sie im Abschnitt **ServiceAnfrage erstellen** die entsprechende Supportkategorie aus. Möglicherweise müssen Sie **Mehr...** auswählen, um weitere Artikel anzuzeigen.

2. Füllen Sie das Formular für Die Dienstanforderung aus, und wählen Sie **Senden** aus.

   > [!TIP]
   > Denken Sie daran, Ihre Kontaktinformationen und nicht die Ihres Kunden anzugeben.

3. Überprüfen Sie später die Serviceanfragen Ihres Kunden, indem Sie zum Office 365 Admin Center gehen und **alle Supporttickets anzeigen** auswählen.

### <a name="support-for-commercial-marketplace-products"></a>Support für Produkte des kommerziellen Marketplace

Microsoft bietet keine Produktunterstützung für Produkte im kommerziellen Marketplace. Wenden Sie sich an den unabhängigen Softwarehersteller (Independent Software Vendor, ISV), der das Produkt veröffentlicht hat, um Support zu erhalten.

So finden Sie Kontaktdaten des ISV:

1.  Wählen Sie auf der Seite **Marketplace** das Produkt aus, zu dem Sie Hilfe benötigen.

2.  Auf der Produktseite finden Sie Kontaktinformationen zum Support. Dies kann eine oder mehrere der folgenden Optionen sein:

    - Einen Supportlink auf der Website des ISV
    - Eine Support-E-Mail-Adresse
    - Eine Supportrufnummer

## <a name="faq"></a>Häufig gestellte Fragen

Sehen Sie sich die folgenden häufig gestellten Fragen zu Serviceanfragen an, die Sie im Auftrag eines Kunden übermitteln können. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Was ist Bestandteil des Supportanspruchs?

Dienstanforderungen sollten über die Partner Center. Sie sind für Azure, Microsoft Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite verfügbar. Partner, die am Cloud Solution Provider-Programm teilnimmt, werden bei schwerwiegenden Problemen bevorzugt behandelt.

Der Support für Ihren eigenen Partner-Mandanten ist nicht im Rahmen des CSP-Supportvorteils enthalten. Für Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite wird jedoch keine separate Supportabonnementgebühr für Partner oder Kunden berechnet. Azure berechnet eine Gebühr, aber wenn Sie berechtigt sind, Signature Cloud Support oder andere Microsoft Partner Network-Vorteile (MPN) zu nutzen, können Sie diese Vorteile nutzen, um diese Gebühr zu bezahlen.

Dieser Vorteil wird Partnern, die am kostenpflichtigen Cloud Solution Provider-Programm teilnehmen, ebenso gewährt wie Partnern, die den Testzeitraum nutzen. Support für die Abrechnung und Abonnementverwaltung ist auch als kostenlose Komponente in diesem Paket enthalten.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Wie schnell erhalte ich eine erste Antwort?

Unsere Reaktionszeiten hängen vom Schweregrad des übermittelten Ereignisses ab. Der Schweregrad eines Problems wird durch die bei der Übermittlung der Serviceanfrage angegebenen geschäftlichen Auswirkungen festgelegt.

Erste Reaktionszeiten für **technische Fehlerbehebungsvorfälle:**

- Kritische Auswirkung (Schweregrad A): Zwei Stunden (Signifikanter Verlust oder Verschlechterung von Diensten. Ausfall der Produktionssdienste.)
- Mittlere Auswirkung (Schweregrad B): Vier Stunden (mittlerer Verlust oder Beeinträchtigung von Diensten. Produktionsdienste teilweise betroffen.)
- Minimale Auswirkung (Schweregrad C): Acht Stunden (minimaler Verlust oder Beeinträchtigung von Diensten. Dienste, die weiterhin verfügbar sind oder nicht für die Produktion verfügbar sind.)

Die anfänglichen Reaktionszeiten gelten nur für englischsprachigen Support. Support in der Landessprache steht nur während der Geschäftszeiten zur Verfügung.
Für Incidents, die innerhalb der Grenzen der Supportberechtigung liegen, aber nicht als Break-Fix-Incidents betrachtet werden, kann die anfängliche Antwortzeit bis zu einem Geschäftstag liegen.

### <a name="can-i-submit-a-service-request-by-phone"></a>Kann ich eine Serviceanfrage per Telefon übermitteln?

Nein, für dieses Programm wird kein Telefonsupport angeboten.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Was geschieht, wenn ich mich beim Azure-Portal anmelde und das Partner Center umgehe?

Wenn Sie sich direkt beim Microsoft Azure-Portal anmelden, sehen Sie das Center in Ihrem eigenen Kontext, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Microsoft Azure-Portal beim Erstellen einer Serviceanfrage für Ihre eigenen Abonnements anmelden.

Ihre CSP-Programm-Supportberechtigung bietet keinen Support für Ihr eigenes Partnerabonnement. Aus diesem Grund müssen Sie Ihre gültige Supportplanberechtigung bereitstellen, wenn Sie eine Serviceanfrage erstellen, die Ihr eigenes Partnerabonnement betrifft. Beispiele hierfür sind die MPN-Vertrags-ID, Premier oder ein Azure-Supportplan. Weitere Informationen finden Sie in den [häufig gestellten Fragen zu Azure-Support](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Was geschieht, wenn ich mich beim Office 365 Admin Center-Portal anmelde und Partner Center umgehe?

Wenn Sie sich direkt beim Office 365 Admin Center anmelden, sehen Sie das Center in Ihrem eigenen Kontext und nicht im Kontext eines Kunden. Daher sollten Sie sich beim Erstellen einer Serviceanfrage für Ihre eigenen Abonnements nur direkt beim Office 365 Admin Center anmelden.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Wie kann ich zusätzlichen Dynamics 365-Support anfordern?

Wenn Probleme im Zusammenhang mit folgenden Themen auftreten: Dynamics 365-Planabonnements, Lizenzierung, Abrechnung, Finance & Operations, Dynamics 365-Produktlizenzen oder sie benötigen weiteren technischen Support:
 
Wenden Sie sich an [Dynamics-Support](/dynamics365/customer-engagement/admin/contact-technical-support).

## <a name="next-steps"></a>Nächste Schritte

- [Bereitstellen von Support für Kunden](customer-support.md)
- [Überprüfen der Dienstintegrität](check-service-health.md)
