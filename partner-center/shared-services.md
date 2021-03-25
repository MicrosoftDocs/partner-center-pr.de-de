---
title: Hinzufügen von Azure Partner Shared Services
description: Verwenden Sie gemeinsame Azure-Partner Dienste, um Azure-Abonnements für Ihren eigenen Gebrauch zu erwerben und eine einheitliche Methode für den Erwerb, die Nachverfolgung und die Verwaltung von Azure zu haben.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 756fbfda3438933b50fc51936b396291986472a7
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028280"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Hinzufügen gemeinsamer Azure-Partner Dienste, damit Partner Azure-Abonnements zur eigenen Nutzung erwerben können

**Geeignete Rollen**

- Globaler Administrator
- Administrator-Agent
- Vertriebsbeauftragter

Azure Partner Shared Services ist eine neue Art von Angebot für Partner im CSP-Programm. Partner können Azure-Abonnements nun zur eigenen Verwendung erwerben.Damit können Partner eine einheitliche Methode für den Kauf, die Nachverfolgung und Verwaltung von Azure verwenden und haben zudem die Möglichkeit, ihre Lizenz- und Weiterverkaufsvereinbarungen für Azure mit Microsoft zu konsolidieren. Mit den gemeinsamen Diensten von Azure-Partnern haben Partner jetzt die gleiche Flexibilität, Azure-Abonnements in CSP zu verwenden, wie Sie in den Microsoft-Enterprise Agreement-und Web Direct-Programmen durchführen können, wie z. b. das Erstellen von Entwicklungs-und Testumgebungen, das Bereitstellen interner Workloads und das Hosten gemeinsamer Dienste oder mehr Instanzen fähiger Anwendungen  

## <a name="create-the-shared-services-tenant"></a>Erstellen des Mandanten für gemeinsame Dienste

1. Wechseln Sie zu **Einstellungen**  >  **Kontoeinstellungen**  >  **gemeinsame Dienste**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Kontoeinstellungen > gemeinsame Dienste":::

2. Wenn Sie bereits einen Mandanten für gemeinsame Dienste haben, klicken Sie auf **Gemeinsame Dienste erstellen**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Gemeinsame Dienste erstellen":::

3. Dient zum Erstellen eines Mandanten für gemeinsame Dienste und Kaufen eines Azure CSP Shared Services-Abonnement, das für gemeinsame genutzte Ressourcen und interne Workloads verwendet werden kann.

   :::image type="content" source="images/sharedservices5.png" alt-text="Mandanten erstellen und Abonnement kaufen":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informationen zum Angebot „Azure – Internal/Shared Services”

- Das Azure – Internal/Shared Services-Abonnement ist ein neuer Azure-Angebotstyp in CSP, auf den über Partner Center zugegriffen wird, den Partner für die Verwendung von Azure nutzen.

- Azure Partner Shared Services-Abonnements sind berechtigt und können zum Erwerb von RIS verwendet werden.

- Das Angebot „Azure – Internal/Shared Services” gilt nur für den Mandanten für gemeinsame Dienste.

- Der primäre Verwendungszweck für das Azure – Internal/Shared Services-Abonnement ist, dass Sie Azure für Ihre eigenen Entwicklungszwecke verwenden können. Der freigegebene Mandant, den Sie zum Bereitstellen dieses Angebots verwenden, kann nicht für andere Dienste wie Office 365 oder Dynamics-Lizenzen verwendet werden.

- Sie können das Abonnement wie alle anderen Abonnements kündigen. Wechseln Sie zu **Einstellungen**  >  **Ansicht alle Einstellungen**  >  **gemeinsame Dienste**. Wählen Sie das Abonnement „Azure – Internal/Shared Services” aus, und kündigen Sie es.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Überprüfen der Azure Partner Shared Services-Verbrauchsdetails

Sie finden den Azure-Verbrauch in Ihrer CSP-Rechnung und in der Kontoabstimmungsdatei. Der Verbrauch wird als Teil des Postens „Microsoft Azure“ in der Rechnung aufgeführt. Auf die genauen Verbrauchsinformationen kann über die Kontenabstimmungsdatei für den Mandanten zugegriffen werden, der für dieses Angebot erstellt wurde.

## <a name="azure-partner-shared-services-pricing"></a>Preise für Azure Partner Shared Services

Um die neue Preis Datei für gemeinsame Azure-Partner Dienste anzuzeigen, besuchen  >  Sie **Preise und Angebote** verkaufen, und wählen Sie die Preisliste des aktuellen Monats aus. In den kommenden Wochen wird auch eine spezielle Gebührenkarten-API veröffentlicht.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-Angebote und Azure Partner Shared Services

Ab dem 1. März 2019 unterstützt Azure Partner Shared Services (APSS) keine Marketplace-Angebote mehr.

|**Marketplace-Unterstützung**   |**APSS-Unterstützung vor dem 1. März 2019**|**Nach dem 1. März 2019**|
|---------------------------|:----------------------------|:-------------------|
|BYOL (Bring Your Own License) und kostenlose Dienste   | Ja   | Nein|
|Andere Marketplace-Angebote von Drittanbietern   | Nein   |Nein|

Partner mit byol oder kostenlosen Diensten, die mit APSS bereitgestellt werden, sind nicht betroffen. nach dem 1. März 2019 können Sie jedoch keine neuen byol-oder kostenlosen Dienste kaufen.

Um den vollständigen Katalog mit den verfügbaren Marketplace-angeboten (nicht nur byol und kostenlose Dienste) nutzen zu können, empfiehlt es sich, dass CSP-Partner gemeinsame Dienste mithilfe von Azure-Web-Direct-  CSP-Partner, die byol-Ressourcen und kostenlose Dienst Ressourcen von Drittanbietern bereits aus dem Marketplace bereitgestellt haben und die Sie weiterhin verwenden möchten, und Bereitstellen von Drittanbieter-angeboten werden empfohlen, das APSS-Abonnement zu Web Direct [Migration vorhandener Azure-Abonnements](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)zu migrieren.

Partner, die nach dem 1. März 2019 mit dem APSS-Abonnement fortfahren und neue [byol-Dienste](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) von Drittanbietern oder kostenlose Dienste bereitstellen möchten, können die Anweisungen von ISVs befolgen, um diese in ihren APSS-Abonnements bereitzustellen.

## <a name="next-steps"></a>Nächste Schritte

- [Verkaufen von Softwareabonnements über CSP](csp-software-subscriptions.md)