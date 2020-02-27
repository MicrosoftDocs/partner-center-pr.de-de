---
title: Umstellung von Kunden auf einen Azure-Plan | Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfahren Sie, wie Sie Ihre Kunden problemlos auf den Azure-Plan umstellen können.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567236"
---
# <a name="transition-your-customers-to-azure-plan"></a>Umstellung Ihrer Kunden auf einen Azure-Plan

**Geeignete Rollen**

- Administrator-Agent
- Abrechnungsadministrator
- Globaler Administrator
- Helpdesk-Agent
- Vertriebsbeauftragter
- Benutzerverwaltungsadministrator

Indirekte Anbieter und direkte Abrechnungspartner können zur neuen Commerce-Benutzeroberfläche wechseln, die im Microsoft Cloud Service Provider (CSP)-Programm für Azure verfügbar ist. (Indirekte Wiederverkäufer müssen ihre indirekten Anbieter durchgehen.) Kunden bietet sich ein optimiertes Verfahren zum Kauf von Clouddiensten, gleich ob sie bei Partnern, bei Microsoft-Verkäufern oder direkt im Web kaufen.

Die Funktion zur Umstellung ist nur für Kunden verfügbar, die zur neuen E-Commerce-Benutzeroberfläche für Azure wechseln und einen Microsoft-Kundenvertrag unterzeichnet haben, nicht aber für andere Angebote in CSP, wie etwa Office 365 oder Dynamics 365.

## <a name="available-azure-services-in-azure-csp"></a>Verfügbare Azure-Dienste im Azure CSP

In diesem Abschnitt werden die Azure-Dienste erläutert, die im Azure Cloud Solution Provider (CSP)-Programm verfügbar sind und nicht verfügbar sind. Außerdem wird die Dienstverfügbarkeit in den nationalen Clouds [Microsoft Azure Deutschland](https://azure.microsoft.com/overview/clouds/germany/) und [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) erläutert.

>[!Note]
>[Azure China]( https://www.azure.cn/) ist im Azure CSP-Programm nicht verfügbar.

### <a name="global-cloud"></a>Globale Cloud 

Alle Dienste, die auf dem Azure Resource Manager-Modell basieren, sind im CSP-Programm verfügbar.  Dienste, die nicht auf Azure Resource Manager basieren, sind im CSP-Programm nicht verfügbar.  

### <a name="csp-specific-service-configurations"></a>CSP-spezifische Dienstkonfigurationen

Die folgenden Dienste erfordern spezielle Konfigurationen im CSP:

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Schlüsseltresor](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) – Nur Benutzer des Kundenmandanten können auf Daten in ihrer Time Series Insights-Umgebung zugreifen. Partner können die Time Series Insights-Umgebung ihres Kunden standardmäßig verwalten. Wenn sie jedoch Zugriff auf die darin enthaltenen Daten benötigen, müssen sie dem Kundenmandanten hinzugefügt werden. 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Sie können jetzt die unten aufgeführten Artikel im Visual Studio Marketplace erwerben. Erweiterungen von Drittanbietern sind davon ausgenommen.

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Visual Studio-Abonnements](https://www.visualstudio.com/subscriptions/)

- [Xamarin University-Schulung](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Um Ihnen den Einstieg zu erleichtern, haben wir Videos und Dokumentationen zum [Einrichten, Erwerben und Verwalten von Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) im CSP erstellt.

### <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-Artikel im Azure CSP

Derzeit sind nicht alle Azure Marketplace-Artikel in Azure CSP-Abonnements verfügbar.

- Microsoft-basierte Azure-Dienste: Diese Dienste sind verfügbar. Informieren Sie sich anhand der vorherigen Tabelle und Kommentare.

- BYOL (Bring Your Own License)-Artikel: Diese Artikel sind verfügbar. Eine vollständige Liste BYOL-fähiger Azure Marketplace-Artikel finden Sie auf der [BYOL-Seite von Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Azure Marketplace-Artikel von Drittanbietern mit nutzungsbasierter Zahlung: Diese Artikel sind verfügbar, wenn der Anbieter im CSP-Kanal veröffentlicht hat. Weitere Informationen finden Sie unter [Verkaufen von Abonnements für Azure Marketplace-Produkte](https://aka.ms/marketplaceincsp).   

- Citrix XenApp Essentials: Partner können XenApp Essentials für Kunden im CSP erwerben. Weitere Informationen finden Sie im folgenden Citrix-Blog: [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) (Distribution von XenApp Essentials jetzt über Microsoft Cloud Solution Provider-Kanal verfügbar).

### <a name="national-clouds"></a>Nationale Clouds 
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

### <a name="next-steps"></a>Nächste Schritte

- [Erfahren Sie mehr](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) über die verfügbaren Funktionen für Azure im Partner Center.

- [Erstellen Sie](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) Ihren ersten Kunden im Azure CSP, und stellen Sie Azure-Dienste bereit.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Umstellung vorhandener CSP-Angebote auf einen Azure-Plan

Sie können einen Kunden auf der neuen E-Commerce-Benutzeroberfläche im Partner Center von seinen vorhandenen CSP Azure-Angeboten auf Azure-Dienste im Rahmen des Azure-Plan umstellen. Dazu müssen der Partner und der Kunde im Partner Center eine Wiederverkäuferbeziehung eingerichtet haben, und der Kunde muss die Microsoft-Kundenvereinbarung unterzeichnet haben.

### <a name="select-transition-to-azure-plan"></a>Auswählen der Umstellung auf den Azure-Plan

1. Wählen Sie den Azure-Plan für Ihren Kunden aus.

2. Wählen Sie **Abrechnung auf Azure-Plan umstellen** aus.

![Umstellung](images/azure/transition1.png)

3. Wählen Sie **Weiter** aus.

![Umstellung](images/azure/transition2.png)

Ihr Kunde wird auf den Azure-Plan umgestellt.

**Im Umstellungsworkflow sind die erforderlichen Schritte automatisiert**:

- Kauf von Azure-Plänen
- Ein Plan pro Kunde in Direkt-CSP-Szenarien  
- Ein Plan pro Wiederverkäufer  

Nehmen wir an, ein Partner hat zwei Microsoft Azure-Angebote erworben und hat zwei verschiedene POR in den Kauf mit eingeschlossen. In diesem Fall kauft der Übergangsworkflow zwei Azure-Pläne (einen pro Wiederverkäufer) und ordnet automatisch die entsprechenden Azure-Abonnements den Azure-Plänen zu.  

**Zuordnen eines Azure-Abonnements zu einem Azure-Plan**

Nach Ihrem Kauf von Azure-Plänen ordnet Ihr System die vorhandenen Azure-Abonnements den Azure-Plänen zu. Der Fortschritt kann im Azure-Portal sowie im Partner Center angezeigt werden. 

4. Kehren Sie zu den Partner Center-**Abonnements** Ihres Kunden zurück, um seinen Budgetgrenzwert in der lokalen Währung des Kunden zu aktualisieren. 

![Umstellung](images/azure/transition3.png)

>[!NOTE]
>Das Budget, das Sie im Partner Center festgelegt haben, wird nicht in das Azure-Portal übertragen. Sie sollten das Budget und die Benachrichtigung auch im Azure-Portal festlegen.

Wenn Sie auf den Azure-Plan umstellen, können Sie für diesen Kunden keine Azure-Abonnements mehr kaufen. Sie erstellen die Abonnements unter dem Azure-Plan im Azure-Portal.

>[!NOTE]
> Alle Azure-Abonnements, die über die RBAC unter dem Azure-Plan erworben wurden, werden in der lokalen Währung abgerechnet. Die Wechselkurse werden nicht verwendet.

### <a name="track-your-transition-details"></a>Nachverfolgen der Umstellungsdetails

Folgen Sie dem Fortschritt der Umstellung im Azure-Portal sowie im Partner Center.

![Details anzeigen](images/azure/details1.png)

**Auswirkungen der Abrechnung auf Partner**

Wenn Sie einen Kunden von einem vorhandenen CSP Azure-Angebot umstellen, treten die folgenden Auswirkungen der Abrechnung auf:

- Bis zu dem Punkt, an dem das ursprüngliche CSP-Azure-Abonnement abgeschlossen ist, erfolgt die Abrechnung Ihrer gesamten Nutzung in Ihrer vorhandenen CSP-Rechnung.

- Wenn Sie über Administratorzugriffsrechte für das vorhandene CSP-Abonnement verfügten, haben Sie auch nach der Migration des Abonnements Zugriff.

Informationen zur Umstellung von direkten Enterprise-Verträgen auf CSP und Server- und Cloud-Registrierungen bei Azure-Diensten finden Sie unter [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](https://docs.microsoft.com/azure/billing/mpa-request-ownership) (Erwerb des Abrechnungsbesitzes von Azure-Abonnements für den Microsoft-Partnervertrag).

**Überwachungsprotokoll**:

Um die Abrechnung abzugleichen, musst du nur den Verlauf der „Microsoft Azure“-Abonnements (0145P) auf der Seite **Abonnements** anzeigen. 

Das Abonnement „Microsoft Azure“ (0145P) setzt sich aus zwei Teilen zusammen:
1. Commerce-Abonnement 
2. Azure-Abonnement (Berechtigung)

Nach Abschluss der Umstellung wird das Azure-Abonnement unter den neuen Azure-Plan verschoben, und das Commerce-Abonnement wird angehalten, sodass keine weitere Nutzung gemeldet wird.  

>[Hinweis]\: Wenn das Microsoft Azure-Abonnement (0145P) in CSP erworben wird, weisen das Commerce-Abonnement und das Azure-Abonnement (Berechtigung) den gleichen Wert auf. Nur im Fall von Änderungen oder einer Übertragung des Abrechnungsbesitzes unterscheiden sich die Werte. 

**Probleme bei der Umstellung**

Bei Umstellungen sind keine Probleme zu erwarten. Wenn ein solcher auftritt, benachrichtigen wir Sie im Übergangsworkflow selbst. Es treten keine Störungen der Azure-Nutzung auf.  

## <a name="next-steps"></a>Nächste Schritte

- [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md)

- [Vom Partner erworbenes Guthaben – Übersicht](partner-earned-credit.md)



