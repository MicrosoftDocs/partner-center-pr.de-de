---
title: Melden von Problemen im Auftrag eines Kunden | Partner Center
ms.topic: article
ms.date: 03/01/2019
Description: Wenn ein Kunde ein Problem mit einem Dienst meldet, das Sie nicht beheben können und das die unter „Eskalieren von Problemen an Microsoft“ beschriebenen Kriterien erfüllt, beantragen Sie ein Supportticket für den Kunden.
ms.assetid: 417E8EE3-EBD2-41DA-BF6E-DD935BE78EF5
author: MaggiePucciEvans
ms.author: evansma
Keywords: Service Request-Diensttickets, unterstützen, unterstützen die Berechtigung, Aobo, Azure aobo
ms.localizationpriority: medium
ms.openlocfilehash: af024782202bc2127b76277b29049e3d34f17215
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134060"
---
# <a name="report-problems-on-behalf-of-a-customer"></a>Melden von Problemen im Auftrag eines Kunden

**Gilt für**

-  Partner Center
-  Partner Center für Microsoft Cloud for US Government


Wenn ein Kunde ein Problem mit einem Dienst meldet, das Sie nicht beheben können und das die unter [Eskalieren von Problemen an Microsoft](escalate-problems-to-microsoft.md) beschriebenen Kriterien erfüllt, beantragen Sie ein Supportticket für den Kunden. Dieser Vorgang eignet sich auch zum Eskalieren von Abrechnungsproblemen oder -streitigkeiten und Betrugsverdachtsfällen.

## <a name="submit-a-service-request-for-a-customer"></a>Übermitteln einer Serviceanfrage für einen Kunden

1.  Von der **Partner Center** , wählen Sie im Menü **Dienstanforderungen** und dann **kundenanforderung**. 

2.  Suchen Sie auf der Seite der Kundenanforderungen die gewünschten Kunden aus.

3.  Wählen Sie aus dem Dropdownmenü **Neue Anforderung** entweder **Azure** oder **Office 365, Dynamics 365, Enterprise Mobility Suite** aus. Sie werden zum Microsoft Azure-Portal oder Office 365 Admin Center umgeleitet.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Wenn Sie eine Serviceanfrage für Ihren Kunden in Azure erstellen möchten, achten Sie darauf, dass Sie die folgenden:
>
>- In der Reihenfolge für dienstanforderungen für Ihren Kunden in Azure zu erstellen muss Ihren indirekte Anbieter gewähren, dass Sie Zugriff auf Azure-Konto des Kunden. Dies unterscheidet sich von der Verwaltung im Auftrag von Kunden für Office 365. 
>
>- Der Helpdesk-Administrator im Partner Center im Azure-Service-Portal Erstellen von Service Requests nicht möglich, zwar was man tun kann eine Supportgruppe im Azure-Service-Portal erstellen, und weisen Sie dieser Gruppenberechtigungen um Supportanfragen zu protokollieren.

1. Wählen Sie **Neue Supportanfrage** aus.
2. Füllen Sie die Supportanfrage mit den entsprechenden Informationen aus, und wählen Sie dann **Erstellen**:
-   Wählen Sie im Abschnitt **Grundlagen** im Feld **Supportplan** die Option **Cloud-Lösungsanbieter**.
-   Geben Sie im Abschnitt **Kontakt** der Supportanfrage Ihre Informationen und nicht die Ihres Kunden ein.

3. Überprüfen Sie später die Serviceanfragen Ihres Kunden im Microsoft Azure-Portal, indem Sie **Supportanfragen verwalten** auswählen.

Sie müssen möglicherweise eine Supportanfrage für einen Kunden erstellen, wenn Sie nicht über Administratorberechtigungen für diesen Kunden verfügen. Dies kann in einem der beiden Szenarien auftreten: 
 
-   Sie hat keine Administratorrechte angefordert, wenn Sie sich zuerst um die Beziehung festgelegt.
-   Sie Verwalten eines Kunden Azure-Abonnements und keine andere, die nicht über Administratorberechtigungen verfügen müssen.
 
In beiden Fällen können Sie das folgende Verfahren zum Erstellen einer Supportanfrage. 

1. Kopieren der Domänenname des Kunden auf ihrer Kontoseite im Partner Center an.

2. Wechseln Sie zu https://portal.azure.com/[Customerdomainname]. 

3. Wählen Sie das Azure-Abonnement, das erfordert.

4. Wählen Sie **neue Supportanfrage**, und befolgen Sie dann die Anweisungen zum Erstellen der Anforderung. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Wählen Sie im Abschnitt **Serviceanfrage erstellen** die geeignete Supportkategorie aus. Möglicherweise müssen Sie **Mehr...** auswählen, um weitere Themen anzuzeigen.    
2. Füllen Sie das Formular für die Serviceanfrage aus, und wählen Sie **Übermitteln** aus.

   > [!TIP]
   > Denken Sie daran, Ihre Kontaktinformationen und nicht die Ihres Kunden anzugeben.

3. Überprüfen Sie später die Serviceanfragen Ihres Kunden, indem Sie zum Office 365 Admin Center wechseln und **Alle Supporttickets anzeigen** auswählen.

### <a name="support-for-azure-marketplace-products"></a>Support für Azure Marketplace-Produkte

Microsoft bietet keine Produkt-Support für Azure Marketplace-Produkte. Sie müssen sich an Hersteller der unabhängige Softwareanbieter (ISV) wenden, die Veröffentlichung des Produkts, um Unterstützung zu erhalten.

So finden Sie Kontaktinformationen des ISV

1.  Wählen Sie auf der Marketplace-Seite das Produkt, dem Sie Hilfe benötigen.
2.  Auf des Produkts finden Sie Kontaktinformationen für Support. Dies kann eine oder mehrere der folgenden sein:
    - Einen Link zu einer Support-Einstiegspunkt des ISV-Website
    - Eine e-Mail-Adresse 
    - Eine Supportrufnummer wenden Sie sich an

## <a name="faq"></a>Häufig gestellte Fragen

**Was ist Bestandteil der Unterstützung-Berechtigung?**

Serviceanfragen sollten über das Partner Center eingereicht werden. Sie sind für Azure, Microsoft Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite verfügbar. Als CSP-Partner haben Sie Priorität bei der Reaktionszeit für Ihre größten Probleme.

Die Unterstützung für Ihren eigenen Partnermandanten ist nicht Bestandteil des CSP-Supportvorteils. Für Office 365, Microsoft Dynamics CRM Online und Enterprise Mobility Suite werden jedoch keine separaten Abonnementgebühren für den Support für Partner oder Kunden berechnet. Azure erhebt eine Gebühr, aber wenn Sie Anspruch auf Signature Cloud Support oder andere Microsoft Partner Network (MPN)-Vorteile haben, können Sie damit die Gebühr bezahlen.

Dieser Vorteil gilt für alle CSP-Partner, die bezahlen oder eine Testversion nutzen. Support für die Abrechnung und Abonnementverwaltung ist auch als kostenlose Komponente in diesem Paket enthalten.

**Wie schnell erhalte ich eine erste Antwort?**

Unsere Reaktionszeiten hängen vom Schweregrad des übermittelten Ereignisses ab. Der Schweregrad eines Problems wird durch die bei der Übermittlung der Serviceanfrage angegebenen geschäftlichen Auswirkungen festgelegt.

Die anfänglichen Reaktionszeiten für **technische Problemlösungsfälle** sind wie folgt:

-   Kritische Auswirkungen (Schweregrad A): 2 Stunden (Drastischer Verlust oder drastische Verschlechterung der Dienste. Ausfall der Produktionssdienste.)
-   Mittlere Auswirkung (Schweregrad B): 4 Stunden (mittelschwerer Verlust oder drastische Verschlechterung der Dienste. Produktionsdienste teilweise betroffen.)
-   Minimale Auswirkungen (Schweregrad C): acht Stunden (minimale Verlust oder drastische Verschlechterung der Dienste. Dienste sind weiterhin verfügbar oder es sind Dienste ohne Auswirkungen auf die Produktion betroffen.)

Die anfänglichen Reaktionszeiten gelten nur für englischsprachigen Support. Support in der Landessprache steht nur während der Geschäftszeiten zur Verfügung.
Für Fälle, die innerhalb der Grenzen des Supportanspruchs liegen, jedoch keine Break-Fix-Ereignisse sind, kann die anfängliche Reaktionszeit bis zu einem Werktag betragen.

**Kann ich per Telefon eine Serviceanfrage senden?**

Nein, für dieses Programm wird kein telefonischer Support angeboten.

**Was geschieht, wenn ich das Azure-Portal anmelden und umgehen das Partner Center?**

Wenn Sie sich direkt beim Microsoft Azure-Portal anmelden, wird das Center in Ihrem eigenen Kontext angezeigt, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Microsoft Azure-Portal anmelden, wenn Sie eine Serviceanfrage für Ihre eigenen Abonnements erstellen.

Ihre Berechtigung zu CSP-Support enthält keinen Support für Ihr eigenes Partnerabonnement. Wenn Sie eine Serviceanfrage erstellen, die sich auf Ihr eigenes Partnerabonnement bezieht, müssen Sie eine gültige Supportplanberechtigung nachweisen. Beispiele für Nachweise sind die MPN-Vertrags-ID, ein Premier- oder ein Azure-Supportplan. Informationen dazu finden Sie auf der Seite [Häufig gestellte Fragen zum Azure-Support](https://go.microsoft.com/fwlink/?LinkId=717532).

**Was geschieht, wenn ich melden Sie sich beim Office 365 Admin Center-Portal, und umgehen das Partner Center?**

Wenn Sie sich direkt beim Office 365 Admin Center anmelden, wird das Center in Ihrem eigenen Kontext angezeigt, nicht im Kontext eines Kunden. Aus diesem Grund sollten Sie sich nur direkt beim Office 365 Admin Center anmelden, wenn Sie eine Serviceanfrage für Ihre eigenen Abonnements erstellen.

**Wie erhalte ich weitere Unterstützung für Dynamics 365?**

Wenn Sie Probleme im Zusammenhang mit auftreten: Dynamics 365-Plan-Abonnements, Lizenzierung, Abrechnung, Finanzen, & Operationen, die IURs angegeben wird, oder Sie benötigen weitere technischen Support:
 
Wenden Sie sich an [Dynamics-Support](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support).

Lesen Sie [Support für Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur).



