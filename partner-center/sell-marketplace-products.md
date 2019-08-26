---
title: Verkaufen von Abonnements für Produkte des kommerziellen Marketplace | Partner Center
ms.topic: article
ms.date: 08/16/2019
description: Sie können Partner Center verwenden, um Ihren Kunden Abonnements für SaaS-Produkte (Software as a Service) zu verkaufen, die auf dem kommerziellen Marketplace von unabhängigen Softwareherstellern (ISVs) veröffentlicht wurden.
author: JnHs
ms.author: jenhayes
keywords: Abonnements, Marketplace, Drittanbieter, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 1338ad86572fad40aabce74688f33f6544a3ec1a
ms.sourcegitcommit: e84322e2cb6f3f559de93c98a16ab19531a2f95c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/19/2019
ms.locfileid: "69578792"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>Verkaufen von Abonnements für Produkte des kommerziellen Marketplace

**Zielgruppe**

- Partner Center

Sie können Partner Center verwenden, um Ihren Kunden Abonnements für SaaS-Produkte (Software as a Service) zu verkaufen, die auf dem kommerziellen Marketplace ([Microsoft AppSource](https://appsource.microsoft.com/) und [Azure Marketplace](https://azuremarketplace.microsoft.com/)) von unabhängigen Softwareherstellern (ISVs) veröffentlicht wurden. Dies kann Ihnen dabei helfen, Ihr Unternehmen von der Konkurrenz abzuheben und Ihren Kunden Softwarepakete anzubieten, die ihre speziellen geschäftlichen Anforderungen erfüllen. Sie verwalten Lizenzen und Abonnements für diese Marketplace SaaS-Produkte wie für Microsoft-Produkte.

Weitere Informationen zum kommerziellen Marketplace finden Sie unter [Häufig gestellte Fragen zum Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

> [!IMPORTANT]
> In Partner Center können nur SaaS-Abonnements (Software-as-a-Service) des kommerziellen Marketplace erworben werden. Andere Angebotsarten des kommerziellen Marketplace (z. B. Azure-Anwendungen, Container oder VMs) werden über das Azure-Portal verwaltet und nutzungsbasiert abgerechnet. Es ist ein vorhandenes Azure-Abonnement erforderlich, um nutzungsbasierte Lösungen über das Azure-Portal zu ermöglichen.

## <a name="view-marketplace-offers-and-pricing"></a>Anzeigen von Marketplace-Angeboten und -Preisen

Wählen Sie im linken Navigationsmenü **Marketplace** aus, um alle verfügbaren Angebote des kommerziellen Marketplace anzuzeigen. Standardmäßig werden Ihnen Produkte aller Arten und Kategorien angezeigt. Sie können nach Typ und/oder Kategorie filtern oder das Suchfeld verwenden, um nach bestimmten Schlüsselwörtern zu suchen. Wählen Sie ein Produkt aus, um Informationen zum Herausgeber und zu den verfügbaren SKUs zu erhalten, einschließlich der Frage, ob ein kostenloser Testzeitraum angeboten wird.

> [!NOTE]
> Einige Produkte, die auf dem kommerziellen Marketplace erhältlich sind, werden hier möglicherweise nicht angezeigt. Unabhängige Softwarehersteller (ISVs) haben die Wahl, ob sie ihre Produkte den Partnern des Cloud Solution Providers (CSP) im Partner Center anbieten. Wenn Sie ein Produkt des kommerziellen Marketplace sehen, das Sie Ihren Kunden über Partner Center anbieten möchten, suchen Sie die Kontaktinformationen des Herausgebers im Produkteintrag, und lassen Sie ihn wissen, dass Sie interessiert sind.

Die Preise für Produkte des kommerziellen Marketplace können sich ständig ändern. Um aktuelle Preisinformationen für alle Produkte des kommerziellen Marketplace zu erhalten, wählen Sie in der rechten oberen Ecke der Seite **Marketplace** die Option **Preisliste exportieren** aus. Dadurch wird eine Kalkulationstabelle mit allen Preisdaten erstellt. Diese Preisinformationen werden täglich aktualisiert, sodass Sie sie jederzeit einsehen können, wenn Sie aktuelle Preise benötigen.

> [!TIP]
> Wenn ein Produkt in dieser Liste eine kostenlose Testversion anbietet, enthält die Kalkulationstabelle zwei Zeilen für dieses Produkt. In einer Zeile wird der Preis Null angezeigt, was bedeutet, dass eine kostenlose Testversion verfügbar ist. Die andere Zeile enthält den Preis und die Laufzeit, die nach Ablauf des Testzeitraums gelten.
>
> Wenn ein Produkt in dieser Liste [Gemessene Abrechnung](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing) verwendet, ist das Feld für die Laufzeitfeld leer.

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>Kaufen von Produkten des kommerziellen Marketplace für Ihre Kunden

Der Kauf von Abonnements für SaaS-Produkte des kommerziellen Marketplace folgt dem gleichen Prozess wie bei Microsoft-Produkten. Vor dem Kauf eines Abonnements müssen Sie einen Kunden auswählen oder einen neuen Kunden hinzufügen.

Wenn Sie ein Abonnement für einen Kunden hinzufügen, können Sie wählen, ob Sie nur Marketplace-Angebote von unabhängigen Softwareherstellern anzeigen möchten, indem Sie **Partner** im Filter für **Herausgeber** auswählen. Weitere Informationen finden Sie unter [Erstellen eines neuen Abonnements](create-a-new-subscription.md).

Beachten Sie, dass einige Angebote, die auf der Seite **Marketplace** angezeigt werden, für einen bestimmten Kunden möglicherweise nicht verfügbar sind. Die Verfügbarkeit kann von einer Reihe von Faktoren beeinflusst werden, einschließlich der Frage, ob der unabhängige Softwarehersteller das Abrechnungsland bzw. die Abrechnungsregion des Kunden unterstützt.

> [!TIP]
> Sie können auch [Partner Center-APIs](https://docs.microsoft.com/partner-center/develop/) verwenden, um Abonnements für Ihre Kunden im kommerziellen Marketplace zu erstellen. Weitere Informationen finden Sie unter [Erstellen von Abonnements für Produkte des kommerziellen Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Bei Abonnements für Produkte des kommerziellen Marketplace haben Sie die Möglichkeit, [das Abonnement innerhalb der Kündigungsfrist (24 Stunden für Monatsabonnements oder 14 Tage für Jahresabonnements) zu kündigen](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription). Sie können auch [auswählen, ob Sie das Abonnement automatisch verlängern möchten](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-commercial-marketplace-products"></a>Lizenzaktivierung für Produkte des kommerziellen Marketplace

Für Angebote vom Typ „Software-as-a-Service“ (SaaS) wird die Lizenzzuordnung und -aktivierung durch den unabhängigen Softwarehersteller (ISV) verwaltet, der das Produkt veröffentlicht hat. Um diesen Prozess abzuschließen, müssen Sie die Website des Herausgebers besuchen, indem Sie einen personalisierten Link mit einem Autorisierungscode verwenden, mit dem der Herausgeber Ihren spezifischen Kauf identifizieren kann. Sie finden diesen Link auf der Bestätigungsseite, die nach dem Erwerb eines SaaS-Angebots angezeigt wird, und auf der Seite **Abonnements** (in der Zeile für dieses Angebot). Sie können auch die [Partner Center-APIs verwenden, um diesen Link abzurufen](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Wenn Sie die Website des Herausgebers über diesen Link besuchen, sehen Sie, welche zusätzlichen Informationen oder Maßnahmen erforderlich sind, um Lizenzen bereitzustellen und zuzuweisen oder den Setupprozess abzuschließen. Die erforderlichen Schritte können je nach Herausgeber und Angebot variieren. Sie sind dafür verantwortlich, alle erforderlichen Informationen zu übermitteln (oder die URL an Ihren Kunden zu senden, um diese Informationen direkt bereitzustellen). Nach Bereitstellung der erforderlichen Informationen stellt der Herausgeber die entsprechenden Lizenzen bereit und weist sie zu. Die Abrechnung des Abonnements beginnt erst, wenn die Lizenzen erfolgreich zugewiesen wurden.

## <a name="access-billing-info-for-commercial-marketplace-products"></a>Zugriff auf Abrechnungsinformationen für Produkte des kommerziellen Marketplace

Bei Produkten des kommerziellen Marketplace beginnt der Abrechnungszeitraum am 1. Tag des Kalendermonats und endet am letzten Tag des Kalendermonats. Wir werden Ihre Rechnung am 8. Tag des Folgemonats zur Verfügung stellen. Sie können auf diese Rechnungen entweder im Partner Center oder über die APIs des Partner Centers zugreifen.

Weitere Informationen finden Sie unter [Grundlegendes zu Abrechnungsarten in Partner Center](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>Bereitstellen von Support für Kunden, die Produkte des kommerziellen Marketplace verwenden

Wie bei Microsoft-Produkten sollten Sie der erste Ansprechpartner für Ihren Kunden bei Fragen zur Abrechnung und Abonnementverwaltung sein. Wenden Sie sich für den technischen Support an den Herausgeber. Microsoft bietet keinen Support für Produkte des kommerziellen Marketplace an, sondern stellt Ihnen die Kontaktinformationen des Herausgebers zur Verfügung.

Weitere Informationen finden Sie unter [Support für Produkte des kommerziellen Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products) und [Bereitstellen von Support für Ihre Kunden](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Verwalten von Abonnements mithilfe von Partner Center-APIs

Mithilfe der Partner Center-APIs können Sie ein Abonnement für Produkte des kommerziellen Marketplace erstellen. Hierzu rufen Sie zunächst eine Liste der Angebote für einen Markt ab, erstellen dann eine Bestellung für ein bestimmtes Abonnement des kommerziellen Marketplace und senden diese ab. Zuletzt rufen Sie einen Aktivierungslink für das Abonnement ab.

Sie können auch Partner Center-APIs verwenden, um die Lebenszyklusverwaltung durchzuführen und Rechnungen für diese Abonnements zu verwalten.

Weitere Informationen finden Sie unter [Erstellen von Abonnements für Produkte des kommerziellen Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).