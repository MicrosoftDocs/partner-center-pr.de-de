---
title: Verkaufen von Kunden Microsoft Azure Reservierungen
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Als cloudlösungsanbieter können Sie Azure-Reservierungen für Kunden erwerben, verkaufen oder verwalten. Verwenden Sie Partner Center, die Azure-Portal oder die Partner Center-API.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, verwalten, Abrechnung, kaufen, Azure-RI, Azure Reserved Instances
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5393e757b209de5a7df22b35a0cee0703419bef4
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198638"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="6ed9b-105">Verkaufen Sie Microsoft Azure Reservierungen an Kunden, die Partner Center, die Azure-Portal oder APIs verwenden.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="6ed9b-106">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="6ed9b-106">**Applies to**</span></span>

- <span data-ttu-id="6ed9b-107">Partner Center</span><span class="sxs-lookup"><span data-stu-id="6ed9b-107">Partner Center</span></span>
- <span data-ttu-id="6ed9b-108">Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="6ed9b-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="6ed9b-109">Partner im CSP</span><span class="sxs-lookup"><span data-stu-id="6ed9b-109">Partners in CSP</span></span>

<span data-ttu-id="6ed9b-110">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="6ed9b-110">**Appropriate roles**</span></span>

- <span data-ttu-id="6ed9b-111">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="6ed9b-111">Admin agent</span></span>
- <span data-ttu-id="6ed9b-112">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="6ed9b-112">Global admin</span></span>
- <span data-ttu-id="6ed9b-113">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="6ed9b-113">Helpdesk agent</span></span>
- <span data-ttu-id="6ed9b-114">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="6ed9b-114">Sales agent</span></span>
- <span data-ttu-id="6ed9b-115">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="6ed9b-115">User management admin</span></span>

<span data-ttu-id="6ed9b-116">Partner im Cloud Solution Provider-Programm (CSP) können ihren Kunden Microsoft Azure-Reservierungen anbieten.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="6ed9b-117">Kunden profitieren von deutlichen Einsparungen, wenn sie im Voraus reservieren.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="6ed9b-118">Azure-Reservierungen bieten Kunden Einfachheit und Flexibilität auf folgende Weise:</span><span class="sxs-lookup"><span data-stu-id="6ed9b-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="6ed9b-119">Ein- oder dreijährige Reservierungslaufzeiten</span><span class="sxs-lookup"><span data-stu-id="6ed9b-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="6ed9b-120">Einfache Inbetriebnahme, sehr schnelles Setup</span><span class="sxs-lookup"><span data-stu-id="6ed9b-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="6ed9b-121">Jederzeitiges Stornieren oder Umtauschen reservierter Instanzen gegen angepasste Rückerstattung</span><span class="sxs-lookup"><span data-stu-id="6ed9b-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="6ed9b-122">Verwalten reservierter Instanzen auf Organisations- oder Abteilungsebene</span><span class="sxs-lookup"><span data-stu-id="6ed9b-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="6ed9b-123">Azure-Reservierungen können Kunden wie folgt ansprechen:</span><span class="sxs-lookup"><span data-stu-id="6ed9b-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="6ed9b-124">Reservierungen können für nutzungsbasierte Zahlungsmodelle erhebliche Einsparungen bieten.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="6ed9b-125">Bessere Budgetierung und Prognosen mit Vorauszahlung für Laufzeiten von einem Jahr oder drei Jahren.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="6ed9b-126">Priorisierte Rechenkapazität in der Azure-Region, die den Niederlassungen am nächsten ist</span><span class="sxs-lookup"><span data-stu-id="6ed9b-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="6ed9b-127">Azure-Reservierungen bilden bei Kombination mit Software wie Microsoft Windows Server und Azure SQL-Datenbank die Grundlage für komplette Infrastrukturlösungen.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="6ed9b-128">Sie können Azure-Reservierungen sowohl im Partner Center- als auch im Azure-Portal sowie mithilfe der Partner Center-API kaufen, verkaufen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="6ed9b-129">Sie können auch Ihren Kunden die Berechtigung erteilen, ihre eigenen Azure-Reservierungen von einem Azure-Abonnement zu erwerben, das Sie für Sie erworben haben.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="6ed9b-130">Weitere Informationen finden Sie unter folgenden Links.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="6ed9b-131">Ressourcen zu Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="6ed9b-131">Azure reservations resources</span></span>

|<span data-ttu-id="6ed9b-132">**Informationen über**</span><span class="sxs-lookup"><span data-stu-id="6ed9b-132">**For information about**</span></span>   |<span data-ttu-id="6ed9b-133">**Artikel**</span><span class="sxs-lookup"><span data-stu-id="6ed9b-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="6ed9b-134">Dokumentation zu Azure-Reservierungen für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="6ed9b-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="6ed9b-135">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="6ed9b-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="6ed9b-136">Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="6ed9b-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="6ed9b-137">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="6ed9b-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="6ed9b-138">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="6ed9b-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="6ed9b-139">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="6ed9b-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="6ed9b-140">Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden</span><span class="sxs-lookup"><span data-stu-id="6ed9b-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="6ed9b-141">Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="6ed9b-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="6ed9b-142">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="6ed9b-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="6ed9b-143">[Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="6ed9b-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="6ed9b-144">Gewähren von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von Ihrem CSP-Abonnement zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="6ed9b-145">Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="6ed9b-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
