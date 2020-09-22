---
title: Abrechnung für kommerzielle Marketplace-Produkte
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie die Abrechnung für ISV SaaS-Produkte oder-Abonnements funktioniert, die für Kunden vom kommerziellen Marketplace innerhalb von Partner Center erworben wurden.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c03ab358b8fb6ab0f23ea5f42b9d35c6f6c2b80c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000424"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Abrechnung für kommerzielle Marketplace-Produkte und-Abonnements im Partner Center

**Zielgruppe**

- Partner Center
- Partner im CSP-Programm

**Geeignete Rollen**

- Globaler Administrator
- Abrechnungsadministrator

Als Partner im CSP-Programm können Sie mit Partner Center Lizenz basierte SaaS-Produkte von ISV-Verlegern im kommerziellen Marketplace erwerben. Anschließend können Sie auf eine Rechnung für diese Art von Käufen zugreifen. Der Abrechnungszeitraum beginnt am ersten Tag des Kalendermonats und endet am letzten Tag des Kalendermonats. Rechnungen werden am 8. Tag des folgenden Monats verfügbar gemacht.

Sie können auf Rechnungen entweder über das Partner Center- [Dashboard](https://partner.microsoft.com/dashboard/) oder mithilfe von [Partner Center-APIs](/partner-center/develop/)zugreifen.

Partner im CSP-Programm werden für einen Kunden erworbene ISV-Marketplace-Lösungen in Rechnung gestellt, wenn Sie diese Produkte entweder über Partner Center oder über den Azure-Portal erwerben (über den früheren, von CSP erworbenen Azure-Mandanten des Kunden).

>[!NOTE]
>Wenn Kunden ihren eigenen Azure AD Mandanten verwenden (nicht einer von einem Partner im CSP-Programm erworbenen), können Kunden auch eine eigene ISV-SaaS-Lösung direkt von ([Microsoft AppSource](https://appsource.microsoft.com/) oder [Azure Marketplace](https://azuremarketplace.microsoft.com/)) erwerben. Wenn dies der Fall ist, erhalten Sie eine eigene Rechnung direkt von Microsoft. Wenn ein Partner im CSP-Programm ein Azure-Abonnement oder den neuen Azure-Plan an den Kunden verkauft und dem Kunden (oder dem indirekten Reseller) [rollenbasierten Zugriff](/azure/role-based-access-control/built-in-roles) auf diesen Mandanten gewährt (dem Kunden neben **Reader**eine Rolle zuweisen), kann dieser Kunde (oder indirekte Reseller) auch kommerzielle Marketplace-Angebote erwerben, ohne vorherige Genehmigung oder Benachrichtigung an den CSP-Partner zu erhalten. In diesen Fällen werden Partner im CSP-Programm von Microsoft nicht direkt über die von ihren Kunden getätigten Einkäufe benachrichtigt. Microsoft bietet jedoch einen optionalen [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) Mechanismus an, den Sie verwenden können, um Warnungen oder Benachrichtigungen zu Aktivitäten in einem Azure-Abonnement festzulegen.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Zugriff auf Abrechnungsinformationen für kommerzielle Marketplace-Produkte

Der globale Administrator oder der Abrechnungsadministrator Ihres Unternehmens erhält eine E-Mail, wenn eine Rechnung zum Anzeigen bereit ist. So greifen Sie auf die aktuelle Rechnungs-und Abstimmungs Datei für kommerzielle Marketplace-Produkt Einkäufe zu:

1. Melden Sie sich beim Partner Center-[Dashboard](https://partner.microsoft.com/dashboard/) an.

2. Wählen Sie im Menü des Partner Center **Abrechnung** aus. 

    Am oberen Rand der Abrechnungs Seite werden zwei Registerkarten angezeigt: **wiederkehrende** und **wiederkehrende und einmalige Käufe**. Auf jeder Registerkarte können Sie auf Rechnungen und Abgleich Dateien (Recon) für verschiedene Marketplace-Produkte zugreifen:

    - Registerkarte "wieder **holt** ": zeigt Rechnungs-und Abstimmungs Dateien für Abonnements im Zusammenhang mit Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI pro und Microsoft Azure an.

    - Registerkarte " **wiederkehrende und einmalige Käufe** ": zeigt Rechnungs-und Abgleich Dateien für Azure-Plan, Azure-Reservierungen, Software und kommerzielle Marketplace-Produkte.
  
3. Wählen Sie die Registerkarte **wiederkehrende und einmalige Käufe** aus. Wenn Sie Abonnements für einen Kunden in einer anderen Währung erworben haben, wird für jede Währung eine Registerkarte angezeigt. Sie können Folgendes tun: "OM This page:

    - Um die neueste Rechnung und die Abstimmungs Datei anzuzeigen, wählen Sie die **Rechnungs** -oder Abstimmungs **Datei**aus. (Wenn Sie möchten, können Sie auch auf die neueste Rechnung zugreifen und Datei Daten mithilfe der [Partner Center-APIs](/partner-center/develop/)wiederholen.

    - Wenn Sie frühere Rechnungen anzeigen und Dateien wiederholen möchten, erweitern Sie unten die Zeile **Abrechnungs Verlauf** .

    - Wählen Sie unter der Überschrift **Schätzungen** einen Link aus, um den geschätzten Konto Saldo oder die Rechnung zu einem beliebigen Zeitpunkt basierend auf der aktuellen Kontoaktivität zu überprüfen.  

    >[!NOTE]
    > Wenn wir Ihre Rechnung am 8. Tag des Monats veröffentlichen, umfasst Sie steuern und alle anderen anwendbaren Gebühren und Gutschriften. Dies bedeutet, dass der endgültige Betrag möglicherweise von dem, was Sie während des Abrechnungszeitraums sehen, abweicht.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Weitere Informationen zu Rechnungen und zum Wiederholen von Dateien für kommerzielle Marketplace-Produkte

Dieser Abschnitt enthält weitere Informationen zu Rechnungs-und Abstimmungs Dateien für kommerzielle Marketplace-Saas-Abonnements, die für Kunden von Drittanbietern erworben wurden.

Wenn Sie im Partner Center im Menü "Partner Center" **wiederkehrende und einmalige Käufe** von der **Abrechnungs** Option auswählen, erhalten Sie Zugriff auf Rechnungen und Abstimmungs Dateien, die sich auf die Gebühren für Microsoft-Käufe (First-Party) und ISV-Käufe (Drittanbieter) beziehen. Diese Käufe können zugeordnet werden:

- Saas-Abonnements (von Microsoft-oder ISV-Verlegern)

- Azure-Plan

- Azure-Reservierungen

- Andere Abonnement basierte Software (von Microsoft-oder ISV-Verlegern)

Beispiele für diese Käufe können SUSE Linux-Software (ein Software Abonnement) oder ein Azure ISV Saas-Produkt Abonnement enthalten.

>[!NOTE]
> Weitere Informationen zum Lesen von Rechnungen und zum Wiederholen von Dateien finden Sie unter [Übersicht über die Abrechnung](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Tipps zum Lesen Ihrer Rechnung

Wenn Sie ein Lizenz basiertes Saas-Produkt von einem Drittanbieter-ISV-Verleger erwerben, werden Ihnen nur Gebühren für die Lizenzgebühr in Ihrer Rechnung angezeigt. Dies gilt auch, wenn das SaaS-Produkt von ISV zugrunde liegende Azure-Infrastruktur Ressourcen verwendet (oder nutzt). Dies liegt daran, dass die Nutzungsgebühren für die Azure-Infrastruktur Ihres Kunden für das SaaS-Produkt eines ISV direkt an den ISV abgerechnet werden. (Für ISVs werden zugeordnete Azure-verbrauchsgebühren in ihrer eigenen Azure-nutzungsbasierten Rechnung für die Rechnungs Abstimmung angezeigt.)

Ihre Rechnung enthält mehrere Seiten:

- **Seite 1 der Rechnung:** Enthält eine Übersicht über die Abrechnungsdetails des CSP-programmpartners. Dies umfasst eine Zusammenfassung der Gebühren für den Abrechnungszeitraum, eine Rechnungsnummer, Zahlungsbedingungen (Netto 60 Tage) und Zahlungsmethoden für Rechnungen, die per Wire oder Check abgerechnet werden.

- **Seite 2 (und alle nachfolgenden Seiten) der Rechnung:** Details fallen für die ersten Käufe von Microsoft und Drittanbieter-ISV-Käufe (Lizenz basiert) aus dem kommerziellen Marketplace an. Sie können ISV-Lizenz basierte Käufe von der **Herausgeber** Leitung unter jedem Produktnamen ermitteln. Die zugehörige Abstimmungs Datei bietet weitere Abrechnungsdetails zu bestimmten Rechnungs Gebühren.

- **Abschließende Seite der Rechnung:** Wenn Sie von einem ISV Lizenz basierte Marketplace-Produkte in Rechnung gestellt haben, werden auf dieser letzten Seite Weitere Details zum Namen und zur Adresse des ISV-Verlegers angezeigt.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tipps zum Lesen der Abstimmungs Datei

Die Abstimmungs Datei für **wiederkehrende und einmalige Käufe** enthält mehrere Spalten mit zusätzlichen Details, die den Gebühren in Ihrer Rechnung entsprechen. In der Spalte **PublisherName** wird angezeigt, ob der Kauf von Microsoft oder einem Drittanbieter-ISV-Verleger erfolgt.

Einige Gebühren in der Abstimmungs Datei werden möglicherweise mit den Kosten $0 angezeigt. Dies liegt möglicherweise an einem kostenlosen ISV-Testangebot (in der Regel 30 oder 60 Tage) oder einem Bring-your-own-License-Angebot.

Bei einer kostenlosen Testversion bietet ISV Folgendes:

- Der Zeitraum für die kostenlose Testversion deckt während dieser Zeit die Kosten des lizenzbasierten Saas-Produkts von ISV ab. Ihnen wird auch die Nutzung dieses Saas-Produkts in der Azure-Infrastruktur nicht in Rechnung gestellt.  Wenn Sie jedoch ein Nutzungs basiertes ISV-Angebot verwenden, umfasst die kostenlose Testversion nicht die Kosten der zugrunde liegenden Nutzung der Azure-Infrastruktur. In diesem Fall werden die Nutzungsgebühren für die Azure-Infrastruktur in einer separaten Azure-Abstimmungs Datei angezeigt.

- Wenn Sie für Ihren Kunden ein kostenloses, von ISV kostenloses Testprodukt erwerben und bereitstellen, wird der Kunde automatisch von dem ISV-Verleger in der kostenlosen Testversion angemeldet. Der Zeitraum für die kostenlose Testversion endet automatisch nach dem vom ISV-Verleger definierten Zeitraum. Nach Ablauf des Zeitraums wird der Kunde in Rechnung gestellt. Dies bedeutet, dass die Abstimmungs Datei möglicherweise zwei Zeilen für ein in der Testversion geeignetes Produkt anzeigt: einen, der den Testzeitraum nachverfolgt, und einen, der das kostenpflichtige Angebot nachverfolgt (in dem die Kosten $0 bis zum Ende des Testzeitraums angezeigt werden). Nach Ablauf der Testversion werden in der Zeile, in der das kostenpflichtige Angebot angezeigt wird, Gebühren berechnet. 

Weitere Informationen dazu, was die einzelnen Spalten darstellen, finden [Sie unter Verwenden](use-the-reconciliation-files.md)von Abstimmungs Dateien. Siehe auch [Abrechnungs Typen in Partner Center](billing-different-types.md)

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten kommerzieller Marketplace-Produkte für Kunden](csp-commercial-marketplace-manage.md)
- [Weitere Informationen zur Unterstützung für kommerzielle Marketplace-Produkte](csp-commercial-marketplace-support.md)