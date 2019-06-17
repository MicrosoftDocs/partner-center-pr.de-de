---
title: Verkaufen von Abonnements für Azure Marketplace-Produkte | Partner Center
ms.topic: article
ms.date: 06/10/2019
description: Sie können das Partner Center verwenden, um Ihren Kunden Abonnements für SaaS-Produkte (Software as a Service) zu verkaufen, die in Azure Marketplace von unabhängigen Softwareherstellern (ISVs) veröffentlicht wurden.
author: JnHs
ms.author: jenhayes
keywords: Abonnements, Marketplace, Drittanbieter, ISV
ms.localizationpriority: medium
ms.openlocfilehash: d870bfef7d967e8f5b890fadfe86f527e558cda5
ms.sourcegitcommit: a9916e90efbb21bff250effd36a213420889633c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/13/2019
ms.locfileid: "67045072"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Verkaufen von Abonnements für Azure Marketplace-Produkte

**Gilt für**

- Partner Center

Sie können das Partner Center verwenden, um Ihren Kunden Abonnements für SaaS-Produkte (Software as a Service) zu verkaufen, die in [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) von unabhängigen Softwareherstellern (ISVs) veröffentlicht wurden. Dies kann Ihnen dabei helfen, Ihr Unternehmen von der Konkurrenz abzuheben und Ihren Kunden Softwarepakete anzubieten, die ihre speziellen geschäftlichen Anforderungen erfüllen. Sie verwalten Lizenzen und Abonnements für diese Azure Marketplace SaaS-Produkte wie für Microsoft-Produkte.

Für weitere Informationen zu Azure Marketplace finden Sie unter [Häufig gestellte Fragen zu Azure Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Anzeigen von Marketplace-Angeboten und -Preisen

Wählen Sie **Marketplace** aus dem linken Navigationsmenü aus, um alle verfügbaren Angebote anzuzeigen. Standardmäßig werden Ihnen Produkte aller Arten und Kategorien angezeigt. Sie können nach Typ und/oder Kategorie filtern oder das Suchfeld verwenden, um nach bestimmten Schlüsselwörtern zu suchen. Wählen Sie ein Produkt aus, um Informationen zu Herausgeber und verfügbaren SKUs anzuzeigen.

> [!NOTE]
> Einige Produkte, die in Azure Marketplace erhältlich sind, werden hier möglicherweise nicht angezeigt. Unabhängige Softwarehersteller (ISVs) haben die Wahl, ob sie ihre Produkte den Partnern des Cloud Solution Providers (CSP) im Partner Center anbieten. Wenn Sie ein Produkt in Azure Marketplace sehen, das Sie Ihren Kunden über das Partner Center anbieten möchten, suchen Sie die Kontaktdaten des Herausgebers in Azure Marketplace und lassen Sie ihn wissen, dass Sie interessiert sind.

Die Preise für Azure Marketplace-Produkte können sich ständig ändern. Um aktuelle Preisinformationen für alle Marketplace-Produkte zu erhalten, wählen Sie **Preisliste exportieren** in der oberen rechten Ecke der Seite **Marketplace** aus. Dadurch wird eine Kalkulationstabelle mit allen Preisdaten erstellt. Die Preisinformationen werden täglich aktualisiert, sodass Sie sie jederzeit einsehen können, wenn Sie aktuelle Preise benötigen.

## <a name="purchase-marketplace-products-for-your-customers"></a>Kaufen von Marketplace-Produkten für Ihre Kunden

Der Kauf von Abonnements für Azure Marketplace SaaS-Produkte folgt dem gleichen Prozess wie bei Microsoft-Produkten. Wenn Sie ein Abonnement für einen Kunden hinzufügen, können Sie wählen, ob Sie nur Marketplace-Angebote von unabhängigen Softwareherstellern anzeigen möchten, indem Sie **Partner** im Filter für **Herausgeber** auswählen. Weitere Informationen finden Sie unter [Erstellen eines neuen Abonnements](create-a-new-subscription.md).

> [!IMPORTANT]
> Sie können SaaS-Produktabonnements (Software as a Service) nur im Partner Center erwerben. Andere Angebotsarten (z. B. Azure-Anwendungen, Container oder VMs) werden über das Azure-Portal verwaltet und nutzungsbasiert abgerechnet. Es ist ein vorhandenes Azure-Abonnement erforderlich, um nutzungsbasierte Lösungen über das Azure-Portal zu ermöglichen.

Beachten Sie, dass einige Angebote, die auf der Seite **Marketplace** angezeigt werden, für einen bestimmten Kunden möglicherweise nicht verfügbar sind. Die Verfügbarkeit kann von einer Reihe von Faktoren beeinflusst werden, einschließlich der Frage, ob der unabhängige Softwarehersteller das Abrechnungsland bzw. die Abrechnungsregion des Kunden unterstützt.

> [!TIP]
> Sie können auch [Partner Center-APIs](https://docs.microsoft.com/partner-center/develop/) verwenden, um Abonnements für Ihre Kunden in Azure Marketplace zu erstellen. Weitere Informationen finden Sie unter [Erstellen von Abonnements für Azure Marketplace-Produkte](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Bei Abonnements für Azure Marketplace-Produkte haben Sie die Möglichkeit, [das Abonnement innerhalb der Kündigungsfrist (24 Stunden für Monatsabonnements oder 14 Tage für Jahresabonnements) zu kündigen](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription). Sie können auch [auswählen, ob Sie das Abonnement automatisch verlängern möchten](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

> [!NOTE]
> Für [Azure Marketplace-Produkte](sell-marketplace-products.md), Zuweisen von Lizenzen und Aktivierung durch den Hersteller ISVS (Independent Software), die das Produkt veröffentlicht verwaltet wird.

## <a name="access-billing-info-for-marketplace-products"></a>Zugreifen auf Abrechnungsinformationen für Marketplace-Produkte

Bei Marketplace-Produkten beginnt der Abrechnungszeitraum am 1. Tag des Kalendermonats, und er endet am letzten Tag des Kalendermonats. Wir werden Ihre Rechnung am 8. Tag des Folgemonats zur Verfügung stellen. Sie können auf diese Rechnungen entweder im Partner Center oder über die APIs des Partner Centers zugreifen.

Weitere Informationen finden Sie unter [Grundlegendes zu Abrechnungsarten in Partner Center](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Bereitstellen von Support für Kunden, die Marketplace-Produkte verwenden

Wie bei Microsoft-Produkten sollten Sie der erste Ansprechpartner für Ihren Kunden bei Fragen zur Abrechnung und Abonnementverwaltung sein. Wenden Sie sich für den technischen Support an den Herausgeber. Microsoft bietet keinen Support für Marketplace-Produkte, sondern stellt Ihnen die Kontaktinformationen des Herausgebers zur Verfügung.

Weitere Informationen finden Sie unter [Support für Azure Marketplace-Produkte](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) und [Bereitstellen von Support für Ihre Kunden](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Verwalten von Abonnements mithilfe von Partner Center-APIs

Sie können ein Abonnement für Azure Marketplace-Produkte über die Partner Center-APIs erstellen, indem Sie eine Liste der Angebote für einen Markt abrufen, eine Bestellung für ein Azure Marketplace-Abonnement erstellen und übermitteln und dann einen Aktivierungslink abrufen. Sie können auch Partner Center-APIs verwenden, um die Lebenszyklusverwaltung durchzuführen und Rechnungen für diese Abonnements zu verwalten.

Weitere Informationen finden Sie unter [Erstellen von Abonnements für Azure Marketplace-Produkte](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).