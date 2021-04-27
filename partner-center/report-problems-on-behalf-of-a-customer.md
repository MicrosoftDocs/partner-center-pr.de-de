---
title: Melden von Problemen im Auftrag eines Kunden
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wann Sie ein Kundendienstproblem an Microsoft eskalieren und wie Sie ein Supportticket für verschiedene Arten von Microsoft-Dienste.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f67a3b6a403f09cb773a5ca663d6cf6db1b03e2e
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018117"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Melden eines Dienstproblems im Namen eines Kunden – einschließlich wann und wie.

**Zielgruppe**

- Partner Center für Microsoft Cloud for US Government

**Geeignete Rollen**

- Globaler Administrator

Wenn ihr Kunde ein Dienstproblem hat, das Sie nicht beheben können und das die unter Eskalieren von Problemen an [Microsoft](escalate-problems-to-microsoft.md)beschriebenen Kriterien erfüllt, kann Ihr indirekter Anbieter ein Supportticket für ihn erstellen. Dieser Vorgang eignet sich auch zum Eskalieren von Abrechnungsproblemen oder -streitigkeiten und Betrugsverdachtsfällen.

## <a name="submit-a-service-request-for-a-customer"></a>Übermitteln einer Serviceanfrage für einen Kunden

1. Wählen Sie im Partner Center unter CSP die Option **Kunden aus.**

2. Wählen Sie auf der Seite Kunden den kundenspezifischen Kunden aus, oder suchen Sie nach diesem.
    
3. Wählen Sie im Menü "Kunde" **die Option Service requests (Dienstanforderungen) aus.**

4. Wählen Sie aus dem Dropdownmenü **Neue Anforderung** entweder **Azure** oder **Office 365, Dynamics 365, Enterprise Mobility Suite** aus. Sie werden entweder an das Microsoft Azure-Portal office 365 Admin Center umgeleitet.

>[!NOTE]
>Support operations partners transacting Dynamics 365 in CSP are required to maintain a support agreement of Advanced Support for Partner (ASfP) plan or higher( Supportvereinbarung des ASfP-Plans (Advanced Support for Partner) oder höher. Diese Supportvereinbarung ist erforderlich, um Dynamics 365-Incidents im Auftrag eines CSP-Kunden zu übermitteln. [Erfahren Sie mehr](https://partner.microsoft.com/support/partnersupport) über die Supportvereinbarungsoptionen.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Wenn Sie eine Serviceanfrage für Ihren Kunden in Azure erstellen möchten, beachten Sie Folgendes:
>
>- Damit Sie als indirekter Wiederverkäufer Serviceanfragen für Ihren Kunden in Azure erstellen können, muss Ihr indirekter Anbieter Ihnen Zugriff auf das Azure-Konto des Kunden gewähren. Dies unterscheidet sich von der Verwaltung im Auftrag von Kunden für Office 365.
>
>- Der Helpdesk-Administrator in Partner Center kann zwar keine Serviceanfragen im Azure-Serviceportal erstellen, er kann jedoch eine Supportgruppe im Azure-Serviceportal erstellen und dieser Gruppe Berechtigungen zum Protokollieren von Supportanfragen zuweisen.

1. Wählen Sie **Neue Supportanfrage** aus.

2. Füllen Sie die Supportanfrage mit den entsprechenden Informationen aus, und wählen Sie dann **Erstellen**:

   - Wählen Sie im Abschnitt **Grundlagen** im Feld **Supportplan** die Option **Cloud-Lösungsanbieter**.

   - Geben Sie im Abschnitt **Kontakt** der Supportanfrage Ihre Informationen und nicht die Ihres Kunden ein.

3. Überprüfen Sie später die Serviceanfragen Ihrer Kunden über das Microsoft Azure-Portal, indem Sie **Supportanfragen verwalten** wählen.

Möglicherweise müssen Sie eine Supportanfrage für einen Kunden erstellen, wenn Sie nicht über Administratorberechtigungen für diesen Kunden verfügen. Dies kann in einem der folgenden Szenarios auftreten:

- Sie haben keine Administratorrechte bei der erstmaligen Beziehungserstellung anfordern.
- Sie verwalten nur die Azure-Abonnements eines Kunden, sodass Sie nicht über Administratorberechtigungen verfügen.
 
In beiden Fällen können Sie das folgende Verfahren zum Erstellen einer Supportanfrage anwenden. 

1. Kopieren Sie den Domänennamen des Kunden von seiner Kontoseite in Partner Center.

2. Wechseln Sie zu https://portal.azure.com/[customerdomainname]. 

3. Wählen Sie das Azure-Abonnement aus, für das Support benötigt wird.

4. Wählen Sie **Neue Supportanfrage** aus, und befolgen Sie anschließend die Anweisungen zum Erstellen einer Anfrage. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Wählen Sie **im Abschnitt Serviceanfrage erstellen** die entsprechende Supportkategorie aus. Möglicherweise müssen Sie **Mehr... auswählen, um** weitere Artikel anzeigen zu können.

2. Füllen Sie das Formular für die Dienstanforderung aus, und wählen Sie **Senden aus.**

   > [!TIP]
   > Denken Sie daran, Ihre Kontaktinformationen und nicht die Ihres Kunden anzugeben.

3. Überprüfen Sie später die Serviceanfragen Ihres Kunden, indem Sie zum Office 365 Admin Center gehen und **Alle Supporttickets sehen auswählen.**

### <a name="support-for-commercial-marketplace-products"></a>Support für Produkte des kommerziellen Marketplace

Microsoft bietet keine Produktunterstützung für Produkte im kommerziellen Marketplace. Sie müssen sich an den unabhängigen Softwarehersteller (Independent Software Vendor, ISV) wenden, der das Produkt veröffentlicht hat, um Support zu erhalten.

So finden Sie Kontaktdaten des ISV:

1.  Wählen Sie auf der Seite **Marketplace** das Produkt aus, zu dem Sie Hilfe benötigen.

2.  Auf der Seite des Produkts finden Sie Kontaktinformationen zum Support. Dies kann eine oder mehrere der folgenden Optionen sein:

    - Einen Supportlink auf der Website des ISV
    - Eine Support-E-Mail-Adresse
    - Eine Supportrufnummer

## <a name="faq"></a>Häufig gestellte Fragen

Sehen Sie sich die folgenden häufig gestellten Fragen zu Serviceanfragen an, die Sie möglicherweise im Auftrag eines Kunden übermitteln. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Was ist Bestandteil des Supportanspruchs?

Dienstanforderungen sollten über Partner Center abgelegt werden. Sie sind für Azure, Microsoft Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite verfügbar. Partner, die am Cloud Solution Provider-Programm teilnimmt, werden bei schwerwiegenden Problemen bevorzugt behandelt.

Der Support für Ihren eigenen Partnermandanten ist nicht im Rahmen des CSP-Supportvorteils enthalten. Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite berechnen jedoch keine separate Supportabonnementgebühr für Partner oder Kunden. Azure berechnet eine Gebühr, aber wenn Sie berechtigt sind, Signature Cloud Support oder andere MPN-Vorteile (Microsoft Partner Network) zu nutzen, können Sie diese Vorteile nutzen, um diese Gebühr zu bezahlen.

Dieser Vorteil wird Partnern, die am kostenpflichtigen Cloud Solution Provider-Programm teilnehmen, ebenso gewährt wie Partnern, die den Testzeitraum nutzen. Support für die Abrechnung und Abonnementverwaltung ist auch als kostenlose Komponente in diesem Paket enthalten.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Wie schnell erhalte ich eine erste Antwort?

Unsere Reaktionszeiten hängen vom Schweregrad des übermittelten Ereignisses ab. Der Schweregrad eines Problems wird durch die bei der Übermittlung der Serviceanfrage angegebenen geschäftlichen Auswirkungen festgelegt.

Anfängliche Antwortzeiten für **Technische Unterbrechungsbehebungsvorfälle:**

- Kritische Auswirkung (Schweregrad A): Zwei Stunden (erheblicher Verlust oder Beeinträchtigung von Diensten. Ausfall der Produktionssdienste.)
- Mittlere Auswirkung (Schweregrad B): Vier Stunden (mittelschwerer Verlust oder Beeinträchtigung von Diensten. Teilweise betroffene Produktionsdienste.)
- Minimale Auswirkung (Schweregrad C): Acht Stunden (Minimaler Verlust oder Beeinträchtigung von Diensten. Dienste, die weiterhin verfügbar sind oder nicht für die Produktion verfügbar sind, sind betroffen.)

Die anfänglichen Reaktionszeiten gelten nur für englischsprachigen Support. Support in der Landessprache steht nur während der Geschäftszeiten zur Verfügung.
Bei Incidents, die innerhalb der Grenzen der Supportberechtigung liegen, aber nicht als Incidents zur Behebung von Unterbrechungen betrachtet werden, kann die anfängliche Antwortzeit bis zu einem Geschäftstag dauern.

### <a name="can-i-submit-a-service-request-by-phone"></a>Kann ich eine Serviceanfrage per Telefon übermitteln?

Nein, für dieses Programm wird kein Telefonsupport angeboten.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Was geschieht, wenn ich mich beim Azure-Portal anmelde und das Partner Center umgehe?

Wenn Sie sich direkt beim Microsoft Azure-Portal anmelden, sehen Sie sich das Center in Ihrem eigenen Kontext an, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Microsoft Azure-Portal anmelden, wenn Sie eine Serviceanfrage für Ihre eigenen Abonnements erstellen.

Ihre CSP-Programmunterstützungsberechtigung bietet keinen Support für Ihr eigenes Partnerabonnement. Aus diesem Grund müssen Sie Ihre gültige Supportplanberechtigung bereitstellen, wenn Sie eine Serviceanfrage erstellen, die Ihr eigenes Partnerabonnement betrifft. Beispiele hierfür sind die MPN-Vertrags-ID, Premier oder ein Azure-Supportplan. Weitere Informationen finden Sie in den häufig [gestellten Azure-Support](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Was geschieht, wenn ich mich beim Office 365 Admin Center-Portal anmelde und Partner Center?

Wenn Sie sich direkt beim Office 365 Admin Center anmelden, sehen Sie das Center in Ihrem eigenen Kontext, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Office 365 Admin Center anmelden, wenn Sie eine Dienstanforderung für Ihre eigenen Abonnements erstellen.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Wie kann ich zusätzlichen Dynamics 365-Support anfordern?

Wenn Probleme im Zusammenhang mit Dynamics 365-Planabonnements, Lizenzierung, Abrechnung, Finance & Operations, Dynamics 365-Produktlizenzen oder weitere technische Unterstützung erforderlich sind:
 
Wenden Sie sich an [Dynamics-Support](/dynamics365/customer-engagement/admin/contact-technical-support).

## <a name="next-steps"></a>Nächste Schritte

- [Bereitstellen von Support für Kunden](customer-support.md)
- [Überprüfen der Dienstintegrität](check-service-health.md)
