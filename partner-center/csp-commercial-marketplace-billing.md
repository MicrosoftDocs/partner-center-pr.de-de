---
title: Abrechnung für Produkte im kommerziellen Marketplace
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie die Abrechnung für ISV-SaaS-Produkte oder -Abonnements funktioniert, die für Kunden über den kommerziellen Marketplace innerhalb des Partner Center.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148022"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Abrechnung für Produkte und Abonnements im kommerziellen Marketplace in Partner Center


**Geeignete Rollen:** Globale Administratorrechte | Abrechnungsadministrator

Als Partner im CSP-Programm können Sie Partner Center verwenden, um lizenzbasierte SaaS-Produkte von ISV-Herausgebern im kommerziellen Marketplace zu erwerben. Danach können Sie auf eine Rechnung für diese Arten von Käufen zugreifen. Der Abrechnungszeitraum beginnt am ersten Tag des Kalendermonats und endet am letzten Tag des Kalendermonats. Rechnungen werden am 8. Tag des folgemonats zur Verfügung gestellt.

Sie können auf Rechnungen entweder über das dashboard Partner Center [oder](https://partner.microsoft.com/dashboard/) mithilfe Partner Center [APIs zugreifen.](/partner-center/develop/)

Partnern im CSP-Programm werden ISV-Lösungen für den kommerziellen Marketplace in Rechnung stellen, die für einen Kunden erworben wurden, wenn sie diese Produkte entweder über Partner Center oder über Azure-Portal erwerben (unter Verwendung des vorherigen, von CSP erworbenen Azure-Mandanten des Kunden).

>[!NOTE]
>Wenn Kunden ihren eigenen Azure AD-Mandanten verwenden (nicht einer, der von einem Partner im CSP-Programm erworben wurde), können Kunden auch ihre eigene ISV-SaaS-Lösung direkt bei ([Microsoft AppSource](https://appsource.microsoft.com/) oder [Azure Marketplace ) erwerben.](https://azuremarketplace.microsoft.com/) Wenn sie dies tun, erhalten sie ihre eigene Rechnung direkt von Microsoft. Wenn ein Partner im CSP-Programm ein Azure-Abonnement oder den neuen [Azure-Plan](/azure/role-based-access-control/built-in-roles) an den Kunden verkauft und dem Kunden (oder indirekten Wiederverkäufer) rollenbasierten Zugriff auf diesen Mandanten gewährt (dem Kunden neben **Leser** eine beliebige Rolle zu zuweisen), kann dieser Kunde (oder indirekter Wiederverkäufer) auch Angebote für den kommerziellen Marketplace ohne vorherige Genehmigung oder Benachrichtigung an den CSP-Partner erwerben. In diesen Fällen benachrichtigt Microsoft Partner im CSP-Programm nicht direkt über Käufe ihrer Kunden. Microsoft bietet jedoch einen optionalen [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) Mechanismus, mit dem Sie Warnungen oder Benachrichtigungen zu Aktivitäten in einem Azure-Abonnement festlegen können.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Zugreifen auf Abrechnungsinformationen für Kommerzielle Marketplace-Produkte

Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist. So greifen Sie auf die neueste Rechnung und Abstimmungsdatei für Produktkäufe im kommerziellen Marketplace zu:

1. Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im Menü des Partner Center **Abrechnung** aus. 

    Oben auf der Seite Abrechnung werden zwei Registerkarten angezeigt: **Wiederkehrende** und **wiederkehrende und einmalige Käufe.** Auf jeder Registerkarte können Sie auf Rechnungs- und Abstimmungsdateien für verschiedene Marketplace-Produkte zugreifen:

    - **Wiederkehrende** Registerkarte: Zeigt Rechnungs- und Abstimmungsdateien für Abonnements im Zusammenhang mit Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro und Microsoft Azure an.

    - **Registerkarte für wiederkehrende und einmalige Käufe:** Zeigt Rechnungs- und Abstimmungsdateien für Azure-Pläne, Azure-Reservierungen, Software und kommerzielle Marketplace-Produkte an.
  
3. Wählen Sie die Registerkarte **Wiederkehrende und einmalige Käufe** aus. Wenn Sie Abonnements für einen Kunden in einer anderen Währung erworben haben, wird eine Registerkarte für jede Währung angezeigt. Auf dieser Seite können Sie einige Dinge erledigen:

    - Um die aktuelle Rechnungs- und Abstimmungsdatei anzuzeigen, wählen Sie **Rechnung** oder **Abstimmungsdatei** aus. (Wenn Sie möchten, können Sie auch mit [Partner Center-APIs](/partner-center/develop/)auf die aktuelle Rechnung zugreifen und Dateidaten neu konfigurieren.

    - Um frühere Rechnungen und Abstimmungsdateien anzuzeigen, erweitern Sie unten die Zeile **Abrechnungsverlauf.**

    - Wählen Sie unter der Überschrift **Schätzungen** einen Link aus, um Ihren geschätzten Kontostand oder Ihre Rechnung jederzeit basierend auf der aktuellen Kontoaktivität zu überprüfen.  

    >[!NOTE]
    > Wenn wir Ihre Rechnung am 8. Tag des Monats veröffentlichen, enthält sie Steuern und alle anderen anfallenden Gebühren und Gutschriften. Dies bedeutet, dass sich der endfällige Betrag von dem unterscheiden kann, was während des Abrechnungszeitraums angezeigt wird.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Weitere Informationen zu Rechnungen und Abstimmungsdateien für Kommerzielle Marketplace-Produkte

Dieser Abschnitt enthält weitere Informationen zu Rechnungs- und Abstimmungsdateien für SaaS-Abonnements im kommerziellen Marketplace, die für Kunden von ISV-Herausgebern von Drittanbietern erworben wurden.

Wenn Sie  im Menü Partner Center über  die Option Abrechnung die Option Wiederkehrende und einmalige Käufe auswählen, erhalten Sie Zugriff auf Rechnungen und Abstimmungsdateien für Gebühren im Zusammenhang mit Microsoft-Käufen (Erstabkäufen) und ISV-Käufen (Drittanbieter). Diese Käufe können Folgendem zugeordnet sein:

- SaaS-Abonnements (von Microsoft- oder ISV-Herausgebern)

- Azure-Plan

- Azure-Reservierungen

- Andere abonnementbasierte Software (von Microsoft- oder ISV-Herausgebern)

Beispiele für diese Käufe sind SUSE Linux-Software (ein Softwareabonnement) oder ein Azure ISV SaaS-Produktabonnement.

>[!NOTE]
> Weitere Informationen zum Lesen von Rechnungs- und Abstimmungsdateien finden Sie unter [Abrechnungsübersicht.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Tipps zum Lesen Ihrer Rechnung

Wenn Sie ein lizenzbasiertes SaaS-Produkt von einem ISV-Herausgeber eines Drittanbieters erwerben, werden ihnen nur Gebühren für die Lizenzgebühr auf Ihrer Rechnung ausgewiesen. Dies gilt auch, wenn das SaaS-Produkt des ISV zugrunde liegende Azure-Infrastrukturressourcen verwendet (oder nutzt). Dies liegt daran, dass die Nutzungsgebühren für die Azure-Infrastruktur ihres Kunden für das SaaS-Produkt eines ISV direkt an den ISV abgerechnet werden. (ISVs sehen zugeordnete Azure-Verbrauchsgebühren in ihrer eigenen Täglich bewerteten Azure-Abrechnungsabstimmungsdatei.)

Ihre Rechnung enthält mehrere Seiten:

- **Seite 1 der Rechnung:** Enthält eine zusammenfassende Übersicht über die Abrechnungsdetails des CSP-Programmpartners. Dies umfasst eine Zusammenfassung der Gebühren für den Abrechnungszeitraum, eine Rechnungsnummer, Zahlungsbedingungen (netto 60 Tage) und Zahlungsmethoden zur Zahlung per Überweisung oder Überprüfung.

- **Seite 2 (und alle nachfolgenden Seiten) der Rechnung:** Details zu den Gebühren für Käufe von Microsoft-Erst- und Drittanbieter-ISV(lizenzbasierten) Käufen über den kommerziellen Marketplace. Sie können lizenzbasierte ISV-Käufe anhand der Zeile **Herausgeber** unter jedem Produktnamen identifizieren. Die zugeordnete Abstimmungsdatei bietet weitere Abrechnungsdetails für bestimmte Rechnungsgebühren.

- **Letzte Seite der Rechnung:** Wenn Ihnen lizenzbasierte Marketplace-Produkte von einem ISV in Rechnung gestellt wurden, werden auf dieser letzten Seite weitere Details zum Namen und zur Adresse des ISV-Herausgebers angezeigt.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tipps zum Lesen Ihrer Abstimmungsdatei

Die **Abstimmungsdatei für wiederkehrende und einmalige Käufe** enthält mehrere Spalten mit zusätzlichen Details, die den Gebühren in Ihrer Rechnung zugeordnet sind. In der Spalte **PublisherName** wird angezeigt, ob der Kauf von Microsoft oder einem ISV-Herausgeber eines Drittanbieters erfolgt.

Einige Gebühren in Ihrer Abstimmungsdatei können mit Kosten von 0 US-Dollar angezeigt werden. Dies kann auf ein ISV-Angebot "kostenlose Testversion" (in der Regel 30 oder 60 Tage) oder ein Bring Your Own License-Angebot zurückzuführen sein.

Bei ISV-Angeboten mit kostenloser Testversion:

- Der kostenlose Testzeitraum deckt die Kosten für das lizenzbasierte SaaS-Produkt des ISV während dieser Zeit ab. Außerdem werden Ihnen keine Kosten für die damit verbundene Nutzung der Azure-Infrastruktur dieses SaaS-Produkts in Rechnung gestellt.  Wenn Sie jedoch ein nutzungsbasiertes ISV-Angebot verwenden, enthält die kostenlose Testversion nicht die Kosten für die zugrunde liegende Nutzung der Azure-Infrastruktur. In diesem Fall werden die Nutzungsgebühren für die Azure-Infrastruktur in einer separaten Azure-Abstimmungsdatei angezeigt.

- Wenn Sie das kostenlose Testprodukt eines ISV für Ihren Kunden erwerben und bereitstellen, wird der Kunde automatisch vom ISV-Herausgeber für die kostenlose Testversion registriert. Der kostenlose Testzeitraum endet automatisch nach dem vom ISV-Herausgeber definierten Zeitraum. Nach Ablauf des Zeitraums werden dem Kunden Gebühren in Rechnung gestellt. Dies bedeutet, dass die Abstimmungsdatei zwei Zeilen für ein testfähiges Produkt anzeigen kann: eine, die den Testzeitraum nachzeichnet, und eine, die das kostenpflichtige Angebot nachzeichnet (die Kosten von 0 US-Dollar bis zum Ende des Testzeitraums anzeigen). Sobald die Testversion endet, werden in der Zeile mit dem kostenpflichtigen Angebot Gebühren angezeigt. 

Weitere Informationen dazu, was die einzelnen Spalten darstellen, finden Sie unter [Verwenden Ihrer Abstimmungsdateien.](use-the-reconciliation-files.md) Siehe auch [Abrechnungstypen in Partner Center](./billing-basics.md)

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Produkten im kommerziellen Marketplace für Kunden](csp-commercial-marketplace-manage.md)
- [Erfahren Sie mehr über die Unterstützung für Produkte im kommerziellen Marketplace.](csp-commercial-marketplace-support.md)