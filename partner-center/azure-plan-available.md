---
title: Verfügbare Azure-Dienste im Azure CSP
description: In diesem Artikel werden die im Azure Cloud Solution Provider-Programm (CSP) verfügbaren und nicht verfügbaren Azure-Dienste behandelt.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 2ca8df054a48217a21dbdd897bd260e7bc181e62
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534963"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Im Azure Cloud Solution Provider (CSP)-Programm verfügbare Azure-Dienste

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

## <a name="available-azure-services-in-azure-csp"></a>Verfügbare Azure-Dienste im Azure CSP

In diesem Artikel sind die Azure-Dienste aufgeführt, die im Azure Cloud Solution Provider (CSP)-Programm verfügbar sind und nicht verfügbar sind. Außerdem wird die Dienstverfügbarkeit in den nationalen Clouds [Microsoft Azure Deutschland](https://azure.microsoft.com/overview/clouds/germany/) und [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) erläutert.

>[!Note]
> [Azure China](https://www.azure.cn/) ist im Azure CSP-Programm nicht verfügbar.

## <a name="global-cloud"></a>Globale Cloud

Alle Dienste, die auf dem Azure Resource Manager-Modell basieren, sind im CSP-Programm verfügbar.  Dienste, die nicht auf Azure Resource Manager basieren, sind im CSP-Programm nicht verfügbar.  

## <a name="csp-specific-service-configurations"></a>CSP-spezifische Dienstkonfigurationen

Die folgenden Dienste erfordern spezielle Konfigurationen im CSP:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Schlüsseltresor](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) – Nur Benutzer des Kundenmandanten können auf Daten in ihrer Time Series Insights-Umgebung zugreifen. Partner können die Time Series Insights-Umgebung ihres Kunden standardmäßig verwalten. Wenn sie jedoch Zugriff auf die darin enthaltenen Daten benötigen, müssen sie dem Kundenmandanten hinzugefügt werden.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Sie können jetzt die unten aufgeführten Artikel im Visual Studio Marketplace erwerben. Erweiterungen von Drittanbietern sind davon ausgenommen.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio-Abonnements](https://www.visualstudio.com/subscriptions/)

- [Xamarin University-Schulung](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Um Ihnen den Einstieg zu erleichtern, haben wir Videos und Dokumentationen zum [Einrichten, Erwerben und Verwalten von Azure DevOps](/vsts/billing/csp/set-up-csp-customer) im CSP erstellt.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-Artikel im Azure CSP

Derzeit sind nicht alle Azure Marketplace-Artikel in Azure CSP-Abonnements verfügbar.

- Microsoft-basierte Azure-Dienste: Diese Dienste sind verfügbar. Informieren Sie sich anhand der vorherigen Tabelle und Kommentare.

- BYOL (Bring Your Own License)-Artikel: Diese Artikel sind verfügbar. Eine vollständige Liste BYOL-fähiger Azure Marketplace-Artikel finden Sie auf der [BYOL-Seite von Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Azure Marketplace-Artikel von Drittanbietern mit nutzungsbasierter Zahlung: Diese Artikel sind verfügbar, wenn der Anbieter im CSP-Kanal veröffentlicht hat. Weitere Informationen finden Sie unter [Verkaufen von Abonnements für Azure Marketplace-Produkte](csp-commercial-marketplace-overview.md).

- Citrix XenApp Essentials: Partner können XenApp Essentials für Kunden im CSP erwerben. Weitere Informationen finden Sie im folgenden Citrix-Blog: [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) (Distribution von XenApp Essentials jetzt über Microsoft Cloud Solution Provider-Kanal verfügbar).

## <a name="national-clouds"></a>Nationale Clouds

Die folgende Tabelle enthält eine regelmäßig aktualisierte Liste der verfügbaren Azure-Produkte, -Dienste und -Funktionen vom Originalhersteller für CSP in nationalen Clouds.

| Azure-Produkt, -Dienst oder -Funktion | US Government | Deutschland |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Virtuelle Computer  |  X  |  X  |
|  Cloud Services  |    |    |
|  Virtual Machine Scale Sets  |  X  |  X  |
|  Funktionen  |    |    |
|  Azure Container Service  |    |    |
|  **Netzwerk**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  Lastenausgleich  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Speicher**  |    |    |
|  Speicher  |  X  |  X  |
|  Sicherung  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web + Mobil**  |    |    |
|  App Service  |  X  |  X  |
|  App Service für Linux  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Logik-Apps-Funktion des Azure App Service  |    |    |
|  **Container**  |    |    |
|  App Service  |  X  |  X  |
|  App Service für Linux  |    |  X  |
|  Batch (Stapel)  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **Datenbanken**  |    |    |
|  SQL-Datenbank  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **Daten + Analysen**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **KI + Cognitive Services**  |    |    |
|  Maschinelles Lernen  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch KI  |    |    |
|  **Internet der Dinge**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Maschinelles Lernen  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location Based Services  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise Integration**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Servicebus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Logik-Apps-Funktion des Azure App Service  |    |    |
|  **Sicherheit + Identität**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Mehrstufige Authentifizierung  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Security Center  |  X  |  X  |
|  **Entwicklungstools**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Überwachung + Verwaltung**  |    |    |
|  Advisor  |    |    |
|  Sicherung  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Planer  |  X  |  X  |
|  Automatisierung  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure Managed Applications  |    |    |
|  Azure Migrate  |    |    |
|  Verwaltungsgruppen  |    |  

## <a name="next-steps"></a>Nächste Schritte

- [Erfahren Sie mehr](/azure/cloud-solution-provider/overview/partner-center-overview) über die verfügbaren Funktionen für Azure im Partner Center.

- [Erstellen Sie](/azure/cloud-solution-provider/customer-management/create-new-customer) Ihren ersten Kunden im Azure CSP, und stellen Sie Azure-Dienste bereit.
