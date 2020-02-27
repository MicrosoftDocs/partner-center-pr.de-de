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
# <a name="transition-your-customers-to-azure-plan"></a><span data-ttu-id="f1ab7-103">Umstellung Ihrer Kunden auf einen Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="f1ab7-103">Transition your customers to Azure plan</span></span>

<span data-ttu-id="f1ab7-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f1ab7-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="f1ab7-105">Admin agent</span></span>
- <span data-ttu-id="f1ab7-106">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="f1ab7-106">Billing admin</span></span>
- <span data-ttu-id="f1ab7-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="f1ab7-107">Global admin</span></span>
- <span data-ttu-id="f1ab7-108">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="f1ab7-108">Helpdesk agent</span></span>
- <span data-ttu-id="f1ab7-109">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="f1ab7-109">Sales agent</span></span>
- <span data-ttu-id="f1ab7-110">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="f1ab7-110">User management admin</span></span>

<span data-ttu-id="f1ab7-111">Indirekte Anbieter und direkte Abrechnungspartner können zur neuen Commerce-Benutzeroberfläche wechseln, die im Microsoft Cloud Service Provider (CSP)-Programm für Azure verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-111">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="f1ab7-112">(Indirekte Wiederverkäufer müssen ihre indirekten Anbieter durchgehen.) Kunden bietet sich ein optimiertes Verfahren zum Kauf von Clouddiensten, gleich ob sie bei Partnern, bei Microsoft-Verkäufern oder direkt im Web kaufen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-112">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="f1ab7-113">Die Funktion zur Umstellung ist nur für Kunden verfügbar, die zur neuen E-Commerce-Benutzeroberfläche für Azure wechseln und einen Microsoft-Kundenvertrag unterzeichnet haben, nicht aber für andere Angebote in CSP, wie etwa Office 365 oder Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-113">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement and not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="available-azure-services-in-azure-csp"></a><span data-ttu-id="f1ab7-114">Verfügbare Azure-Dienste im Azure CSP</span><span class="sxs-lookup"><span data-stu-id="f1ab7-114">Available Azure services in Azure CSP</span></span>

<span data-ttu-id="f1ab7-115">In diesem Abschnitt werden die Azure-Dienste erläutert, die im Azure Cloud Solution Provider (CSP)-Programm verfügbar sind und nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-115">This section discusses the Azure services that are and are not available in the Azure Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="f1ab7-116">Außerdem wird die Dienstverfügbarkeit in den nationalen Clouds [Microsoft Azure Deutschland](https://azure.microsoft.com/overview/clouds/germany/) und [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) erläutert.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-116">It also discusses service availability in the national clouds [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) and [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).</span></span>

>[!Note]
><span data-ttu-id="f1ab7-117">[Azure China]( https://www.azure.cn/) ist im Azure CSP-Programm nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-117">[Azure China]( https://www.azure.cn/) is not available in the Azure CSP program.</span></span>

### <a name="global-cloud"></a><span data-ttu-id="f1ab7-118">Globale Cloud</span><span class="sxs-lookup"><span data-stu-id="f1ab7-118">Global Cloud</span></span> 

<span data-ttu-id="f1ab7-119">Alle Dienste, die auf dem Azure Resource Manager-Modell basieren, sind im CSP-Programm verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-119">All services based on Azure Resource Manager model are available in CSP Program.</span></span>  <span data-ttu-id="f1ab7-120">Dienste, die nicht auf Azure Resource Manager basieren, sind im CSP-Programm nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-120">Non-Azure Resource Manager services are not available in CSP program.</span></span>  

### <a name="csp-specific-service-configurations"></a><span data-ttu-id="f1ab7-121">CSP-spezifische Dienstkonfigurationen</span><span class="sxs-lookup"><span data-stu-id="f1ab7-121">CSP-Specific Service Configurations</span></span>

<span data-ttu-id="f1ab7-122">Die folgenden Dienste erfordern spezielle Konfigurationen im CSP:</span><span class="sxs-lookup"><span data-stu-id="f1ab7-122">The following services require special configurations in CSP:</span></span>

- [<span data-ttu-id="f1ab7-123">StorSimple</span><span class="sxs-lookup"><span data-stu-id="f1ab7-123">StorSimple</span></span>](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [<span data-ttu-id="f1ab7-124">Azure Active Directory Domain Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-124">Azure Active Directory Domain Services</span></span>](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [<span data-ttu-id="f1ab7-125">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="f1ab7-125">Key Vault</span></span>](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- <span data-ttu-id="f1ab7-126">[Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) – Nur Benutzer des Kundenmandanten können auf Daten in ihrer Time Series Insights-Umgebung zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-126">[Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Only users from the customer tenant can access data in their Time Series Insights environment.</span></span> <span data-ttu-id="f1ab7-127">Partner können die Time Series Insights-Umgebung ihres Kunden standardmäßig verwalten. Wenn sie jedoch Zugriff auf die darin enthaltenen Daten benötigen, müssen sie dem Kundenmandanten hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-127">Partners can manage their customer’s Time Series Insights environment by default, but if they need access to the data in it, they must be added to the customer tenant.</span></span> 

### <a name="visual-studio-marketplace"></a><span data-ttu-id="f1ab7-128">Visual Studio Marketplace</span><span class="sxs-lookup"><span data-stu-id="f1ab7-128">Visual Studio Marketplace</span></span>

<span data-ttu-id="f1ab7-129">Sie können jetzt die unten aufgeführten Artikel im Visual Studio Marketplace erwerben. Erweiterungen von Drittanbietern sind davon ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-129">You can now purchase the items listed below from Visual Studio Marketplace, with the exception of third-party extensions.</span></span>

- [<span data-ttu-id="f1ab7-130">Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="f1ab7-130">Azure DevOps</span></span>](https://www.visualstudio.com/team-services/) 

- [<span data-ttu-id="f1ab7-131">Visual Studio-Abonnements</span><span class="sxs-lookup"><span data-stu-id="f1ab7-131">Visual Studio subscriptions</span></span>](https://www.visualstudio.com/subscriptions/)

- [<span data-ttu-id="f1ab7-132">Xamarin University-Schulung</span><span class="sxs-lookup"><span data-stu-id="f1ab7-132">Xamarin University training</span></span>](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

<span data-ttu-id="f1ab7-133">Um Ihnen den Einstieg zu erleichtern, haben wir Videos und Dokumentationen zum [Einrichten, Erwerben und Verwalten von Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) im CSP erstellt.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-133">To help get you started, we have created videos and documentation about [how to set up, purchase, and manage Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) in CSP.</span></span>

### <a name="azure-marketplace-items-in-azure-csp"></a><span data-ttu-id="f1ab7-134">Azure Marketplace-Artikel im Azure CSP</span><span class="sxs-lookup"><span data-stu-id="f1ab7-134">Azure Marketplace items in Azure CSP</span></span>

<span data-ttu-id="f1ab7-135">Derzeit sind nicht alle Azure Marketplace-Artikel in Azure CSP-Abonnements verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-135">Not all Azure Marketplace items are currently available in Azure CSP subscriptions.</span></span>

- <span data-ttu-id="f1ab7-136">Microsoft-basierte Azure-Dienste: Diese Dienste sind verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-136">Microsoft-based Azure services: These services are available.</span></span> <span data-ttu-id="f1ab7-137">Informieren Sie sich anhand der vorherigen Tabelle und Kommentare.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-137">Review the previous table and comments.</span></span>

- <span data-ttu-id="f1ab7-138">BYOL (Bring Your Own License)-Artikel: Diese Artikel sind verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-138">Bring your own license (BYOL) items: These items are available.</span></span> <span data-ttu-id="f1ab7-139">Eine vollständige Liste BYOL-fähiger Azure Marketplace-Artikel finden Sie auf der [BYOL-Seite von Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).</span><span class="sxs-lookup"><span data-stu-id="f1ab7-139">A full list of BYOL-enabled Azure Marketplace items is available on the [Azure Marketplace BYOL page](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).</span></span>

- <span data-ttu-id="f1ab7-140">Azure Marketplace-Artikel von Drittanbietern mit nutzungsbasierter Zahlung: Diese Artikel sind verfügbar, wenn der Anbieter im CSP-Kanal veröffentlicht hat.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-140">Pay-As-You-Go third-party Azure Marketplace items: These items are available if the provider has published to the CSP channel.</span></span> <span data-ttu-id="f1ab7-141">Weitere Informationen finden Sie unter [Verkaufen von Abonnements für Azure Marketplace-Produkte](https://aka.ms/marketplaceincsp).</span><span class="sxs-lookup"><span data-stu-id="f1ab7-141">For more information, see [Sell subscriptions to Azure Marketplace products](https://aka.ms/marketplaceincsp).</span></span>   

- <span data-ttu-id="f1ab7-142">Citrix XenApp Essentials: Partner können XenApp Essentials für Kunden im CSP erwerben.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-142">Citrix XenApp Essentials: Partners can purchase XenApp Essentials for customers in CSP.</span></span> <span data-ttu-id="f1ab7-143">Weitere Informationen finden Sie im folgenden Citrix-Blog: [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) (Distribution von XenApp Essentials jetzt über Microsoft Cloud Solution Provider-Kanal verfügbar).</span><span class="sxs-lookup"><span data-stu-id="f1ab7-143">For more information, see the following Citrix blog- [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).</span></span>

### <a name="national-clouds"></a><span data-ttu-id="f1ab7-144">Nationale Clouds</span><span class="sxs-lookup"><span data-stu-id="f1ab7-144">National clouds</span></span> 
<span data-ttu-id="f1ab7-145">Die folgende Tabelle enthält eine regelmäßig aktualisierte Liste der verfügbaren Azure-Produkte, -Dienste und -Funktionen vom Originalhersteller für CSP in nationalen Clouds.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-145">The following table displays a regularly updated list of the available first-party Azure products, services, and features for CSP in national clouds.</span></span> 

| <span data-ttu-id="f1ab7-146">Azure-Produkt, -Dienst oder -Funktion</span><span class="sxs-lookup"><span data-stu-id="f1ab7-146">Azure product, service, or feature</span></span> | <span data-ttu-id="f1ab7-147">US Government</span><span class="sxs-lookup"><span data-stu-id="f1ab7-147">US Government</span></span> | <span data-ttu-id="f1ab7-148">Deutschland</span><span class="sxs-lookup"><span data-stu-id="f1ab7-148">Germany</span></span> |
| ------ | :-----------: | :-----------: |
|  <span data-ttu-id="f1ab7-149">**Compute**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-149">**Compute**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-150">Virtuelle Computer</span><span class="sxs-lookup"><span data-stu-id="f1ab7-150">Virtual Machines</span></span>  |  <span data-ttu-id="f1ab7-151">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-151">X</span></span>  |  <span data-ttu-id="f1ab7-152">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-152">X</span></span>  |
|  <span data-ttu-id="f1ab7-153">Cloud Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-153">Cloud Services</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-154">Virtual Machine Scale Sets</span><span class="sxs-lookup"><span data-stu-id="f1ab7-154">Virtual machine scale sets</span></span>  |  <span data-ttu-id="f1ab7-155">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-155">X</span></span>  |  <span data-ttu-id="f1ab7-156">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-156">X</span></span>  |
|  <span data-ttu-id="f1ab7-157">Funktionen</span><span class="sxs-lookup"><span data-stu-id="f1ab7-157">Functions</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-158">Azure Container Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-158">Azure Container Service</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-159">**Netzwerk**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-159">**Networking**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-160">Azure DNS</span><span class="sxs-lookup"><span data-stu-id="f1ab7-160">Azure DNS</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-161">Content Delivery Network</span><span class="sxs-lookup"><span data-stu-id="f1ab7-161">Content Delivery Network</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-162">Traffic Manager</span><span class="sxs-lookup"><span data-stu-id="f1ab7-162">Traffic Manager</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-163">ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="f1ab7-163">ExpressRoute</span></span>  |  <span data-ttu-id="f1ab7-164">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-164">X</span></span>  |  <span data-ttu-id="f1ab7-165">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-165">X</span></span>  |
|  <span data-ttu-id="f1ab7-166">Virtual Network</span><span class="sxs-lookup"><span data-stu-id="f1ab7-166">Virtual Network</span></span>  |  <span data-ttu-id="f1ab7-167">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-167">X</span></span>  |  <span data-ttu-id="f1ab7-168">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-168">X</span></span>  |
|  <span data-ttu-id="f1ab7-169">Lastenausgleich</span><span class="sxs-lookup"><span data-stu-id="f1ab7-169">Load Balancer</span></span>  |  <span data-ttu-id="f1ab7-170">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-170">X</span></span>  |  <span data-ttu-id="f1ab7-171">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-171">X</span></span>  |
|  <span data-ttu-id="f1ab7-172">VPN Gateway</span><span class="sxs-lookup"><span data-stu-id="f1ab7-172">VPN Gateway</span></span>  |  <span data-ttu-id="f1ab7-173">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-173">X</span></span>  |  <span data-ttu-id="f1ab7-174">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-174">X</span></span>  |
|  <span data-ttu-id="f1ab7-175">Application Gateway</span><span class="sxs-lookup"><span data-stu-id="f1ab7-175">Application Gateway</span></span>  |  <span data-ttu-id="f1ab7-176">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-176">X</span></span>  |  <span data-ttu-id="f1ab7-177">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-177">X</span></span>  |
|  <span data-ttu-id="f1ab7-178">Network Watcher</span><span class="sxs-lookup"><span data-stu-id="f1ab7-178">Network Watcher</span></span>  |  <span data-ttu-id="f1ab7-179">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-179">X</span></span>  |  <span data-ttu-id="f1ab7-180">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-180">X</span></span>  |
|  <span data-ttu-id="f1ab7-181">**Speicher**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-181">**Storage**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-182">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1ab7-182">Storage</span></span>  |  <span data-ttu-id="f1ab7-183">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-183">X</span></span>  |  <span data-ttu-id="f1ab7-184">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-184">X</span></span>  |
|  <span data-ttu-id="f1ab7-185">Sicherung</span><span class="sxs-lookup"><span data-stu-id="f1ab7-185">Backup</span></span>  |  <span data-ttu-id="f1ab7-186">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-186">X</span></span>  |  <span data-ttu-id="f1ab7-187">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-187">X</span></span>  |
|  <span data-ttu-id="f1ab7-188">StorSimple</span><span class="sxs-lookup"><span data-stu-id="f1ab7-188">StorSimple</span></span>  |    |  <span data-ttu-id="f1ab7-189">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-189">X</span></span>  |
|  <span data-ttu-id="f1ab7-190">Site Recovery</span><span class="sxs-lookup"><span data-stu-id="f1ab7-190">Site Recovery</span></span>  |  <span data-ttu-id="f1ab7-191">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-191">X</span></span>  |  <span data-ttu-id="f1ab7-192">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-192">X</span></span>  |
|  <span data-ttu-id="f1ab7-193">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f1ab7-193">Data Lake Store</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-194">Managed Disks</span><span class="sxs-lookup"><span data-stu-id="f1ab7-194">Managed Disks</span></span>  |  <span data-ttu-id="f1ab7-195">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-195">X</span></span>  |  <span data-ttu-id="f1ab7-196">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-196">X</span></span>  |
|  <span data-ttu-id="f1ab7-197">**Web + Mobil**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-197">**Web + Mobile**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-198">App Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-198">App Service</span></span>  |  <span data-ttu-id="f1ab7-199">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-199">X</span></span>  |  <span data-ttu-id="f1ab7-200">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-200">X</span></span>  |
|  <span data-ttu-id="f1ab7-201">App Service für Linux</span><span class="sxs-lookup"><span data-stu-id="f1ab7-201">App Service on Linux</span></span>  |    |  <span data-ttu-id="f1ab7-202">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-202">X</span></span>  |
|  <span data-ttu-id="f1ab7-203">API Management</span><span class="sxs-lookup"><span data-stu-id="f1ab7-203">API Management</span></span>  |  <span data-ttu-id="f1ab7-204">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-204">X</span></span>  |    |
|  <span data-ttu-id="f1ab7-205">Content Delivery Network</span><span class="sxs-lookup"><span data-stu-id="f1ab7-205">Content Delivery Network</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-206">Media Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-206">Media Services</span></span>  |  <span data-ttu-id="f1ab7-207">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-207">X</span></span>  |  <span data-ttu-id="f1ab7-208">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-208">X</span></span>  |
|  <span data-ttu-id="f1ab7-209">Notification Hubs</span><span class="sxs-lookup"><span data-stu-id="f1ab7-209">Notification Hubs</span></span>  |  <span data-ttu-id="f1ab7-210">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-210">X</span></span>  |  <span data-ttu-id="f1ab7-211">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-211">X</span></span>  |
|  <span data-ttu-id="f1ab7-212">Azure Search</span><span class="sxs-lookup"><span data-stu-id="f1ab7-212">Azure Search</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-213">Logik-Apps-Funktion des Azure App Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-213">Logic Apps feature of Azure App Service</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-214">**Container**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-214">**Containers**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-215">App Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-215">App Service</span></span>  |  <span data-ttu-id="f1ab7-216">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-216">X</span></span>  |  <span data-ttu-id="f1ab7-217">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-217">X</span></span>  |
|  <span data-ttu-id="f1ab7-218">App Service für Linux</span><span class="sxs-lookup"><span data-stu-id="f1ab7-218">App Service on Linux</span></span>  |    |  <span data-ttu-id="f1ab7-219">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-219">X</span></span>  |
|  <span data-ttu-id="f1ab7-220">Batch (Stapel)</span><span class="sxs-lookup"><span data-stu-id="f1ab7-220">Batch</span></span>  |  <span data-ttu-id="f1ab7-221">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-221">X</span></span>  |  <span data-ttu-id="f1ab7-222">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-222">X</span></span>  |
|  <span data-ttu-id="f1ab7-223">Container Registry</span><span class="sxs-lookup"><span data-stu-id="f1ab7-223">Container Registry</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-224">Container Instances</span><span class="sxs-lookup"><span data-stu-id="f1ab7-224">Container Instances</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f1ab7-225">Service Fabric</span></span>  |  <span data-ttu-id="f1ab7-226">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-226">X</span></span>  |  <span data-ttu-id="f1ab7-227">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-227">X</span></span>  |
|  <span data-ttu-id="f1ab7-228">Container Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-228">Container Service</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-229">**Datenbanken**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-229">**Databases**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-230">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="f1ab7-230">SQL Database</span></span>  |  <span data-ttu-id="f1ab7-231">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-231">X</span></span>  |  <span data-ttu-id="f1ab7-232">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-232">X</span></span>  |
|  <span data-ttu-id="f1ab7-233">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f1ab7-233">Azure Cosmos DB</span></span>  |  <span data-ttu-id="f1ab7-234">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-234">X</span></span>  |  <span data-ttu-id="f1ab7-235">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-235">X</span></span>  |
|  <span data-ttu-id="f1ab7-236">SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="f1ab7-236">SQL Data Warehouse</span></span>  |  <span data-ttu-id="f1ab7-237">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-237">X</span></span>  |  <span data-ttu-id="f1ab7-238">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-238">X</span></span>  |
|  <span data-ttu-id="f1ab7-239">Redis Cache</span><span class="sxs-lookup"><span data-stu-id="f1ab7-239">Redis Cache</span></span>  |  <span data-ttu-id="f1ab7-240">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-240">X</span></span>  |  <span data-ttu-id="f1ab7-241">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-241">X</span></span>  |
|  <span data-ttu-id="f1ab7-242">SQL Server Stretch Database</span><span class="sxs-lookup"><span data-stu-id="f1ab7-242">SQL Server Stretch Database</span></span>  |  <span data-ttu-id="f1ab7-243">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-243">X</span></span>  |  <span data-ttu-id="f1ab7-244">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-244">X</span></span>  |
|  <span data-ttu-id="f1ab7-245">Azure Database for MySQL</span><span class="sxs-lookup"><span data-stu-id="f1ab7-245">Azure Database for MySQL</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-246">Azure Database for PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="f1ab7-246">Azure Database for PostgreSQL</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-247">**Daten + Analysen**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-247">**Data + Analytics**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-248">Databricks</span><span class="sxs-lookup"><span data-stu-id="f1ab7-248">Databricks</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-249">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f1ab7-249">HDInsight</span></span>  |  <span data-ttu-id="f1ab7-250">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-250">X</span></span>  |  <span data-ttu-id="f1ab7-251">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-251">X</span></span>  |
|  <span data-ttu-id="f1ab7-252">Stream Analytics</span><span class="sxs-lookup"><span data-stu-id="f1ab7-252">Stream Analytics</span></span>  |    |  <span data-ttu-id="f1ab7-253">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-253">X</span></span>  |
|  <span data-ttu-id="f1ab7-254">Data Factory</span><span class="sxs-lookup"><span data-stu-id="f1ab7-254">Data Factory</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-255">Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f1ab7-255">Log Analytics</span></span>  |  <span data-ttu-id="f1ab7-256">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-256">X</span></span>  |    |
|  <span data-ttu-id="f1ab7-257">Data Catalog</span><span class="sxs-lookup"><span data-stu-id="f1ab7-257">Data Catalog</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-258">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f1ab7-258">Data Lake Store</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-259">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f1ab7-259">Data Lake Analytics</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-260">Azure Analysis Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-260">Azure Analysis Services</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-261">Power BI Embedded</span><span class="sxs-lookup"><span data-stu-id="f1ab7-261">Power BI Embedded</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-262">**KI + Cognitive Services**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-262">**AI + Cognitive Services**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-263">Maschinelles Lernen</span><span class="sxs-lookup"><span data-stu-id="f1ab7-263">Machine Learning</span></span>  |    |  <span data-ttu-id="f1ab7-264">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-264">X</span></span>  |
|  <span data-ttu-id="f1ab7-265">Azure Bot Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-265">Azure Bot Service</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-266">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-266">Cognitive Services</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-267">Azure Batch KI</span><span class="sxs-lookup"><span data-stu-id="f1ab7-267">Azure Batch AI</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-268">**Internet der Dinge**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-268">**Internet of Things**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-269">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="f1ab7-269">IoT Hub</span></span>  |  <span data-ttu-id="f1ab7-270">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-270">X</span></span>  |  <span data-ttu-id="f1ab7-271">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-271">X</span></span>  |
|  <span data-ttu-id="f1ab7-272">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f1ab7-272">IoT Central</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-273">Maschinelles Lernen</span><span class="sxs-lookup"><span data-stu-id="f1ab7-273">Machine Learning</span></span>  |    |  <span data-ttu-id="f1ab7-274">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-274">X</span></span>  |
|  <span data-ttu-id="f1ab7-275">Stream Analytics</span><span class="sxs-lookup"><span data-stu-id="f1ab7-275">Stream Analytics</span></span>  |    |  <span data-ttu-id="f1ab7-276">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-276">X</span></span>  |
|  <span data-ttu-id="f1ab7-277">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f1ab7-277">Event Hubs</span></span>  |  <span data-ttu-id="f1ab7-278">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-278">X</span></span>  |  <span data-ttu-id="f1ab7-279">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-279">X</span></span>  |
|  <span data-ttu-id="f1ab7-280">Location Based Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-280">Location-Based Services</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-281">Notification Hubs</span><span class="sxs-lookup"><span data-stu-id="f1ab7-281">Notification Hubs</span></span>  |  <span data-ttu-id="f1ab7-282">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-282">X</span></span>  |  <span data-ttu-id="f1ab7-283">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-283">X</span></span>  |
|  <span data-ttu-id="f1ab7-284">Time Series Insights</span><span class="sxs-lookup"><span data-stu-id="f1ab7-284">Time Series Insights</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-285">**Enterprise Integration**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-285">**Enterprise Integration**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-286">StorSimple</span><span class="sxs-lookup"><span data-stu-id="f1ab7-286">StorSimple</span></span>  |  <span data-ttu-id="f1ab7-287">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-287">X</span></span>  |    |
|  <span data-ttu-id="f1ab7-288">API Management</span><span class="sxs-lookup"><span data-stu-id="f1ab7-288">API Management</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-289">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f1ab7-289">Event Grid</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-290">Data Factory</span><span class="sxs-lookup"><span data-stu-id="f1ab7-290">Data Factory</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-291">Servicebus</span><span class="sxs-lookup"><span data-stu-id="f1ab7-291">Service Bus</span></span>  |  <span data-ttu-id="f1ab7-292">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-292">X</span></span>  |  <span data-ttu-id="f1ab7-293">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-293">X</span></span>  |
|  <span data-ttu-id="f1ab7-294">Data Catalog</span><span class="sxs-lookup"><span data-stu-id="f1ab7-294">Data Catalog</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-295">SQL Server Stretch Database</span><span class="sxs-lookup"><span data-stu-id="f1ab7-295">SQL Server Stretch Database</span></span>  |    |  <span data-ttu-id="f1ab7-296">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-296">X</span></span>  |
|  <span data-ttu-id="f1ab7-297">Logik-Apps-Funktion des Azure App Service</span><span class="sxs-lookup"><span data-stu-id="f1ab7-297">Logic Apps feature of Azure App Service</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-298">**Sicherheit + Identität**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-298">**Security + Identity**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-299">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f1ab7-299">Azure Active Directory</span></span>  |  <span data-ttu-id="f1ab7-300">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-300">X</span></span>  |  <span data-ttu-id="f1ab7-301">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-301">X</span></span>  |
|  <span data-ttu-id="f1ab7-302">Azure Active Directory B2C</span><span class="sxs-lookup"><span data-stu-id="f1ab7-302">Azure Active Directory B2C</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-303">Mehrstufige Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="f1ab7-303">Multi-Factor Authentication</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-304">Azure Active Directory Domain Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-304">Azure Active Directory Domain Services</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-305">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f1ab7-305">Key Vault</span></span>  |  <span data-ttu-id="f1ab7-306">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-306">X</span></span>  |  <span data-ttu-id="f1ab7-307">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-307">X</span></span>  |
|  <span data-ttu-id="f1ab7-308">Security Center</span><span class="sxs-lookup"><span data-stu-id="f1ab7-308">Security Center</span></span>  |  <span data-ttu-id="f1ab7-309">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-309">X</span></span>  |  <span data-ttu-id="f1ab7-310">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-310">X</span></span>  |
|  <span data-ttu-id="f1ab7-311">**Entwicklungstools**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-311">**Developer Tools**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-312">Visual Studio Team Services</span><span class="sxs-lookup"><span data-stu-id="f1ab7-312">Visual Studio Team Services</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-313">Application Insights</span><span class="sxs-lookup"><span data-stu-id="f1ab7-313">Application Insights</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-314">DevTest Labs</span><span class="sxs-lookup"><span data-stu-id="f1ab7-314">DevTest Labs</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-315">Visual Studio App Center</span><span class="sxs-lookup"><span data-stu-id="f1ab7-315">Visual Studio App Center</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-316">Xamarin University</span><span class="sxs-lookup"><span data-stu-id="f1ab7-316">Xamarin University</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-317">**Überwachung + Verwaltung**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-317">**Monitoring + Management**</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-318">Advisor</span><span class="sxs-lookup"><span data-stu-id="f1ab7-318">Advisor</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-319">Sicherung</span><span class="sxs-lookup"><span data-stu-id="f1ab7-319">Backup</span></span>  |  <span data-ttu-id="f1ab7-320">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-320">X</span></span>  |  <span data-ttu-id="f1ab7-321">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-321">X</span></span>  |
|  <span data-ttu-id="f1ab7-322">Site Recovery</span><span class="sxs-lookup"><span data-stu-id="f1ab7-322">Site Recovery</span></span>  |  <span data-ttu-id="f1ab7-323">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-323">X</span></span>  |  <span data-ttu-id="f1ab7-324">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-324">X</span></span>  |
|  <span data-ttu-id="f1ab7-325">Planer</span><span class="sxs-lookup"><span data-stu-id="f1ab7-325">Scheduler</span></span>  |  <span data-ttu-id="f1ab7-326">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-326">X</span></span>  |  <span data-ttu-id="f1ab7-327">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-327">X</span></span>  |
|  <span data-ttu-id="f1ab7-328">Automatisierung</span><span class="sxs-lookup"><span data-stu-id="f1ab7-328">Automation</span></span>  |  <span data-ttu-id="f1ab7-329">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-329">X</span></span>  |  <span data-ttu-id="f1ab7-330">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-330">X</span></span>  |
|  <span data-ttu-id="f1ab7-331">Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f1ab7-331">Log Analytics</span></span>  |  <span data-ttu-id="f1ab7-332">X</span><span class="sxs-lookup"><span data-stu-id="f1ab7-332">X</span></span>  |    |
|  <span data-ttu-id="f1ab7-333">Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="f1ab7-333">Azure Monitor</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-334">Azure Managed Applications</span><span class="sxs-lookup"><span data-stu-id="f1ab7-334">Azure-Managed Applications</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-335">Azure Migrate</span><span class="sxs-lookup"><span data-stu-id="f1ab7-335">Azure Migrate</span></span>  |    |    |
|  <span data-ttu-id="f1ab7-336">Verwaltungsgruppen</span><span class="sxs-lookup"><span data-stu-id="f1ab7-336">Management Groups</span></span>  |    |  

### <a name="next-steps"></a><span data-ttu-id="f1ab7-337">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f1ab7-337">Next steps</span></span>

- <span data-ttu-id="f1ab7-338">[Erfahren Sie mehr](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) über die verfügbaren Funktionen für Azure im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-338">[Learn](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) about the available capabilities for Azure in Partner Center.</span></span>

- <span data-ttu-id="f1ab7-339">[Erstellen Sie](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) Ihren ersten Kunden im Azure CSP, und stellen Sie Azure-Dienste bereit.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-339">[Create](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) your first customer in Azure CSP, and deploy Azure services.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="f1ab7-340">Umstellung vorhandener CSP-Angebote auf einen Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="f1ab7-340">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="f1ab7-341">Sie können einen Kunden auf der neuen E-Commerce-Benutzeroberfläche im Partner Center von seinen vorhandenen CSP Azure-Angeboten auf Azure-Dienste im Rahmen des Azure-Plan umstellen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-341">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="f1ab7-342">Dazu müssen der Partner und der Kunde im Partner Center eine Wiederverkäuferbeziehung eingerichtet haben, und der Kunde muss die Microsoft-Kundenvereinbarung unterzeichnet haben.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-342">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="f1ab7-343">Auswählen der Umstellung auf den Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="f1ab7-343">Select transition to Azure plan</span></span>

1. <span data-ttu-id="f1ab7-344">Wählen Sie den Azure-Plan für Ihren Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-344">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="f1ab7-345">Wählen Sie **Abrechnung auf Azure-Plan umstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-345">Select **Transition billing to Azure plan**.</span></span>

![Umstellung](images/azure/transition1.png)

3. <span data-ttu-id="f1ab7-347">Wählen Sie **Weiter** aus.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-347">Select **Continue**</span></span>

![Umstellung](images/azure/transition2.png)

<span data-ttu-id="f1ab7-349">Ihr Kunde wird auf den Azure-Plan umgestellt.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-349">Your customer will be transitioned to the Azure plan.</span></span>

<span data-ttu-id="f1ab7-350">**Im Umstellungsworkflow sind die erforderlichen Schritte automatisiert**:</span><span class="sxs-lookup"><span data-stu-id="f1ab7-350">**The transition workflow automates the pre-requisite steps**:</span></span>

- <span data-ttu-id="f1ab7-351">Kauf von Azure-Plänen</span><span class="sxs-lookup"><span data-stu-id="f1ab7-351">Purchase of Azure plan(s)</span></span>
- <span data-ttu-id="f1ab7-352">Ein Plan pro Kunde in Direkt-CSP-Szenarien</span><span class="sxs-lookup"><span data-stu-id="f1ab7-352">One plan per customer in Direct CSP scenarios</span></span>  
- <span data-ttu-id="f1ab7-353">Ein Plan pro Wiederverkäufer</span><span class="sxs-lookup"><span data-stu-id="f1ab7-353">One plan per reseller</span></span>  

<span data-ttu-id="f1ab7-354">Nehmen wir an, ein Partner hat zwei Microsoft Azure-Angebote erworben und hat zwei verschiedene POR in den Kauf mit eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-354">For an example, a partner has purchased two Microsoft Azure offers and has included two distinct POR in the purchase.</span></span> <span data-ttu-id="f1ab7-355">In diesem Fall kauft der Übergangsworkflow zwei Azure-Pläne (einen pro Wiederverkäufer) und ordnet automatisch die entsprechenden Azure-Abonnements den Azure-Plänen zu.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-355">In this case, the transition workflow will purchase two Azure plans (one per reseller) and map the respective Azure subscriptions under the Azure plans automatically.</span></span>  

<span data-ttu-id="f1ab7-356">**Zuordnen eines Azure-Abonnements zu einem Azure-Plan**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-356">**Mapping Azure subscription to Azure plan**</span></span>

<span data-ttu-id="f1ab7-357">Nach Ihrem Kauf von Azure-Plänen ordnet Ihr System die vorhandenen Azure-Abonnements den Azure-Plänen zu.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-357">After your purchase of Azure plan(s), our system will map the existing Azure subscriptions to the Azure plans.</span></span> <span data-ttu-id="f1ab7-358">Der Fortschritt kann im Azure-Portal sowie im Partner Center angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-358">The progress can be viewed in Azure portal as well as in Partner center.</span></span> 

4. <span data-ttu-id="f1ab7-359">Kehren Sie zu den Partner Center-**Abonnements** Ihres Kunden zurück, um seinen Budgetgrenzwert in der lokalen Währung des Kunden zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-359">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span> 

![Umstellung](images/azure/transition3.png)

>[!NOTE]
><span data-ttu-id="f1ab7-361">Das Budget, das Sie im Partner Center festgelegt haben, wird nicht in das Azure-Portal übertragen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-361">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="f1ab7-362">Sie sollten das Budget und die Benachrichtigung auch im Azure-Portal festlegen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-362">You should also set the budget and alert in Azure portal.</span></span>

<span data-ttu-id="f1ab7-363">Wenn Sie auf den Azure-Plan umstellen, können Sie für diesen Kunden keine Azure-Abonnements mehr kaufen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-363">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="f1ab7-364">Sie erstellen die Abonnements unter dem Azure-Plan im Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-364">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

>[!NOTE]
> <span data-ttu-id="f1ab7-365">Alle Azure-Abonnements, die über die RBAC unter dem Azure-Plan erworben wurden, werden in der lokalen Währung abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-365">All Azure subscriptions purchased through RBAC under the Azure plan will be priced and billed in local currency.</span></span> <span data-ttu-id="f1ab7-366">Die Wechselkurse werden nicht verwendet.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-366">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="f1ab7-367">Nachverfolgen der Umstellungsdetails</span><span class="sxs-lookup"><span data-stu-id="f1ab7-367">Track your transition details</span></span>

<span data-ttu-id="f1ab7-368">Folgen Sie dem Fortschritt der Umstellung im Azure-Portal sowie im Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-368">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

![Details anzeigen](images/azure/details1.png)

<span data-ttu-id="f1ab7-370">**Auswirkungen der Abrechnung auf Partner**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-370">**Billing impact to partners**</span></span>

<span data-ttu-id="f1ab7-371">Wenn Sie einen Kunden von einem vorhandenen CSP Azure-Angebot umstellen, treten die folgenden Auswirkungen der Abrechnung auf:</span><span class="sxs-lookup"><span data-stu-id="f1ab7-371">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="f1ab7-372">Bis zu dem Punkt, an dem das ursprüngliche CSP-Azure-Abonnement abgeschlossen ist, erfolgt die Abrechnung Ihrer gesamten Nutzung in Ihrer vorhandenen CSP-Rechnung.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-372">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="f1ab7-373">Wenn Sie über Administratorzugriffsrechte für das vorhandene CSP-Abonnement verfügten, haben Sie auch nach der Migration des Abonnements Zugriff.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-373">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="f1ab7-374">Informationen zur Umstellung von direkten Enterprise-Verträgen auf CSP und Server- und Cloud-Registrierungen bei Azure-Diensten finden Sie unter [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](https://docs.microsoft.com/azure/billing/mpa-request-ownership) (Erwerb des Abrechnungsbesitzes von Azure-Abonnements für den Microsoft-Partnervertrag).</span><span class="sxs-lookup"><span data-stu-id="f1ab7-374">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](https://docs.microsoft.com/azure/billing/mpa-request-ownership)</span></span>

<span data-ttu-id="f1ab7-375">**Überwachungsprotokoll**:</span><span class="sxs-lookup"><span data-stu-id="f1ab7-375">**Audit log**:</span></span>

<span data-ttu-id="f1ab7-376">Um die Abrechnung abzugleichen, musst du nur den Verlauf der „Microsoft Azure“-Abonnements (0145P) auf der Seite **Abonnements** anzeigen.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-376">To reconcile billing, view your history of “Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span> 

<span data-ttu-id="f1ab7-377">Das Abonnement „Microsoft Azure“ (0145P) setzt sich aus zwei Teilen zusammen:</span><span class="sxs-lookup"><span data-stu-id="f1ab7-377">“Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>
1. <span data-ttu-id="f1ab7-378">Commerce-Abonnement</span><span class="sxs-lookup"><span data-stu-id="f1ab7-378">Commerce subscription</span></span> 
2. <span data-ttu-id="f1ab7-379">Azure-Abonnement (Berechtigung)</span><span class="sxs-lookup"><span data-stu-id="f1ab7-379">Azure subscription (entitlement)</span></span>

<span data-ttu-id="f1ab7-380">Nach Abschluss der Umstellung wird das Azure-Abonnement unter den neuen Azure-Plan verschoben, und das Commerce-Abonnement wird angehalten, sodass keine weitere Nutzung gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-380">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

><span data-ttu-id="f1ab7-381">[Hinweis]\: Wenn das Microsoft Azure-Abonnement (0145P) in CSP erworben wird, weisen das Commerce-Abonnement und das Azure-Abonnement (Berechtigung) den gleichen Wert auf.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-381">[Note]: When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="f1ab7-382">Nur im Fall von Änderungen oder einer Übertragung des Abrechnungsbesitzes unterscheiden sich die Werte.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-382">It is only in the case of billing ownership changes or transfers do the values differ.</span></span> 

<span data-ttu-id="f1ab7-383">**Probleme bei der Umstellung**</span><span class="sxs-lookup"><span data-stu-id="f1ab7-383">**Transition issues**</span></span>

<span data-ttu-id="f1ab7-384">Bei Umstellungen sind keine Probleme zu erwarten.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-384">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="f1ab7-385">Wenn ein solcher auftritt, benachrichtigen wir Sie im Übergangsworkflow selbst.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-385">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="f1ab7-386">Es treten keine Störungen der Azure-Nutzung auf.</span><span class="sxs-lookup"><span data-stu-id="f1ab7-386">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="f1ab7-387">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f1ab7-387">Next steps</span></span>

- [<span data-ttu-id="f1ab7-388">Verwalten von Abonnements und Ressourcen in einem Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="f1ab7-388">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="f1ab7-389">Vom Partner erworbenes Guthaben – Übersicht</span><span class="sxs-lookup"><span data-stu-id="f1ab7-389">Partner earned credit - overview</span></span>](partner-earned-credit.md)



