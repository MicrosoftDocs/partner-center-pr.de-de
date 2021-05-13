---
title: Hinzufügen von Azure Partner Shared Services
description: Verwenden Azure Partner Shared Services, um Azure-Abonnements für Ihre eigene Verwendung zu erwerben und eine einheitliche Methode für den Erwerb, die Nachverfolgung und die Verwaltung von Azure zu verwenden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855334"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Hinzufügen Azure Partner Shared Services, damit Partner Azure-Abonnements für ihre eigene Verwendung erwerben können

**Geeignete Rollen:** Globale Administratorrechte | Administrator-Agent| Vertriebs-Agent

Azure Partner Shared Services ist eine neue Art von Angebot für Partner im CSP-Programm. Partner können Azure-Abonnements nun zur eigenen Verwendung erwerben.Damit können Partner eine einheitliche Methode für den Kauf, die Nachverfolgung und Verwaltung von Azure verwenden und haben zudem die Möglichkeit, ihre Lizenz- und Weiterverkaufsvereinbarungen für Azure mit Microsoft zu konsolidieren. Mit Azure Partner Shared Services verfügen Partner jetzt über die gleiche Flexibilität bei der Verwendung von Azure-Abonnements in CSP wie in den Microsoft Enterprise Agreement- und Web Direct-Programmen. Dadurch werden Szenarien wie das Erstellen von Entwicklungs- und Testumgebungen, das Bereitstellen interner Workloads und das Hosten gemeinsam genutzter Dienste oder mehrstufiger Anwendungen ermöglicht.  

## <a name="create-the-shared-services-tenant"></a>Erstellen des Mandanten für gemeinsame Dienste

1. Wechseln Sie zu **Einstellungen**  >  **Kontoeinstellungen**  >  **Freigegebene Dienste.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Kontoeinstellungen > Freigegebene Dienste":::

2. Wenn Sie bereits einen Mandanten für gemeinsame Dienste haben, klicken Sie auf **Gemeinsame Dienste erstellen**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Gemeinsame Dienste erstellen":::

3. Dient zum Erstellen eines Mandanten für gemeinsame Dienste und Kaufen eines Azure CSP Shared Services-Abonnement, das für gemeinsame genutzte Ressourcen und interne Workloads verwendet werden kann.

   :::image type="content" source="images/sharedservices5.png" alt-text="Mandanten erstellen und Abonnement kaufen":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informationen zum Angebot „Azure – Internal/Shared Services”

- Das Azure – Internal/Shared Services-Abonnement ist ein neuer Azure-Angebotstyp in CSP, auf den über eine Partner Center, die Partner für ihre eigene Nutzung von Azure erhalten.

- Azure Partner Shared Services Abonnements sind berechtigt und können verwendet werden, um RIs zu erwerben.

- Das Angebot „Azure – Internal/Shared Services” gilt nur für den Mandanten für gemeinsame Dienste.

- Die primäre Verwendung für das Azure – Internal/Shared Services-Abonnement ist, dass Sie Azure für Ihre eigenen Entwicklungszwecke verwenden können. Der freigegebene Mandant, den Sie zum Bereitstellen dieses Angebots verwenden, kann nicht für andere Dienste wie Office 365- oder Dynamics-Lizenzen verwendet werden.

- Sie können das Abonnement wie alle anderen Abonnements kündigen. Wechseln Sie zu den **Einstellungen Alle anzeigen**  >  **Einstellungen Gemeinsame**  >  **Dienste**. Wählen Sie das Abonnement „Azure – Internal/Shared Services” aus, und kündigen Sie es.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Überprüfen der Azure Partner Shared Services-Verbrauchsdetails

Sie finden den Azure-Verbrauch in Ihrer CSP-Rechnung und in der Kontoabstimmungsdatei. Der Verbrauch wird als Teil des Postens „Microsoft Azure“ in der Rechnung aufgeführt. Auf die genauen Verbrauchsinformationen kann über die Kontenabstimmungsdatei für den Mandanten zugegriffen werden, der für dieses Angebot erstellt wurde.

## <a name="azure-partner-shared-services-pricing"></a>Preise für Azure Partner Shared Services

Um die neue Preisdatei für die Azure Partner Shared Services, wechseln Sie zu **Sell** Pricing and offers (Preise und Angebote verkaufen), und wählen Sie die  >   Preisliste des aktuellen Monats aus. In den kommenden Wochen wird auch eine spezielle Gebührenkarten-API veröffentlicht.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-Angebote und Azure Partner Shared Services

Seit dem 1. März 2019 unterstützt Azure Partner Shared Services (APSS) keine Marketplace-Angebote mehr.

|**Marketplace-Unterstützung**   |**APSS-Unterstützung vor dem 1. März 2019**|**Nach dem 1. März 2019**|
|---------------------------|:----------------------------|:-------------------|
|BYOL (Bring Your Own License) und kostenlose Dienste   | Ja   | Nein|
|Andere Marketplace-Angebote von Drittanbietern   | Nein   |Nein|

Partner, die über BYOL oder kostenlose Dienste verfügen, die mit APSS bereitgestellt wurden, sind nicht von den Auswirkungen in Mithilfe von Nach dem 1. März 2019 können sie jedoch keine neuen BYOL- oder kostenlosen Dienste erwerben.

Um den vollständigen Katalog der verfügbaren Marketplace-Angebote (nicht nur BYOL und kostenlose Dienste) nutzen zu können, empfehlen wir CSP-Partnern die Bereitstellung gemeinsam genutzter Dienste mithilfe von Azure-Web-Direktabonnements.  CSP-Partner, die zuvor BYOL- und kostenlose Dienstressourcen von Drittanbietern aus dem Marketplace bereitgestellt haben und diese weiterhin verwenden und weitere Angebote von Drittanbietern bereitstellen möchten, werden empfohlen, das APSS-Abonnement zu einer webdirekten [Migration vorhandener Azure-Abonnements](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)zu migrieren.

Partner, die planen, das APSS-Abonnement nach dem 1. März 2019 weiterhin zu verwenden und neue [BYOL-Dienste](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) von Drittanbietern oder kostenlose Dienste bereitstellen möchten, können die Anweisungen von ISVs befolgen, um diese in ihren APSS-Abonnements bereitzustellen.

## <a name="next-steps"></a>Nächste Schritte

- [Verkaufen von Softwareabonnements über CSP](csp-software-subscriptions.md)