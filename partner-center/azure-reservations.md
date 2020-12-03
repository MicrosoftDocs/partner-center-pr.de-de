---
title: Verkaufen von Kunden Microsoft Azure Reservierungen
description: Als cloudlösungsanbieter können Sie Azure-Reservierungen für Kunden erwerben, verkaufen oder verwalten. Verwenden Sie Partner Center, die Azure-Portal oder die Partner Center-API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534895"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="0ada6-104">Verkaufen Sie Microsoft Azure Reservierungen an Kunden, die Partner Center, die Azure-Portal oder APIs verwenden.</span><span class="sxs-lookup"><span data-stu-id="0ada6-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="0ada6-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="0ada6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="0ada6-106">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="0ada6-106">Admin agent</span></span>
- <span data-ttu-id="0ada6-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="0ada6-107">Global admin</span></span>
- <span data-ttu-id="0ada6-108">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="0ada6-108">Helpdesk agent</span></span>
- <span data-ttu-id="0ada6-109">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="0ada6-109">Sales agent</span></span>
- <span data-ttu-id="0ada6-110">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="0ada6-110">User management admin</span></span>

<span data-ttu-id="0ada6-111">Als Partner im Cloud Solution Provider-Programm (CSP) können Sie Azure-Reservierungen für Kunden erwerben, verkaufen oder verwalten.</span><span class="sxs-lookup"><span data-stu-id="0ada6-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="0ada6-112">Verwenden Sie Partner Center, die Azure-Portal oder die Partner Center-API.</span><span class="sxs-lookup"><span data-stu-id="0ada6-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="0ada6-113">Dieser Artikel gilt nur für Partner in CSP.</span><span class="sxs-lookup"><span data-stu-id="0ada6-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="0ada6-114">Kunden, die andere Abonnementtypen (z. b. Pay-as-you-go, individuelle, Microsoft-Kunden Vereinbarung oder Konzernvertrag Abonnements) verwenden, sollten stattdessen [diese Azure-Reservierungs Dokumentation](/azure/cost-management-billing/reservations)lesen.</span><span class="sxs-lookup"><span data-stu-id="0ada6-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="0ada6-115">Partner im CSP-Programm können Ihren Kunden Microsoft Azure Reservierungen anbieten.</span><span class="sxs-lookup"><span data-stu-id="0ada6-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="0ada6-116">Kunden profitieren von deutlichen Einsparungen, wenn sie im Voraus reservieren.</span><span class="sxs-lookup"><span data-stu-id="0ada6-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="0ada6-117">Azure-Reservierungen bieten Kunden Einfachheit und Flexibilität auf folgende Weise:</span><span class="sxs-lookup"><span data-stu-id="0ada6-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="0ada6-118">Ein- oder dreijährige Reservierungslaufzeiten</span><span class="sxs-lookup"><span data-stu-id="0ada6-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="0ada6-119">Einfache Inbetriebnahme, sehr schnelles Setup</span><span class="sxs-lookup"><span data-stu-id="0ada6-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="0ada6-120">Jederzeitiges Stornieren oder Umtauschen reservierter Instanzen gegen angepasste Rückerstattung</span><span class="sxs-lookup"><span data-stu-id="0ada6-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="0ada6-121">Verwalten reservierter Instanzen auf Organisations- oder Abteilungsebene</span><span class="sxs-lookup"><span data-stu-id="0ada6-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="0ada6-122">Azure-Reservierungen können Kunden wie folgt ansprechen:</span><span class="sxs-lookup"><span data-stu-id="0ada6-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="0ada6-123">Reservierungen können für nutzungsbasierte Zahlungsmodelle erhebliche Einsparungen bieten.</span><span class="sxs-lookup"><span data-stu-id="0ada6-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="0ada6-124">Bessere Budgetierung und Prognosen mit Vorauszahlung für Laufzeiten von einem Jahr oder drei Jahren.</span><span class="sxs-lookup"><span data-stu-id="0ada6-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="0ada6-125">Priorisierte Rechenkapazität in der Azure-Region, die den Niederlassungen am nächsten ist</span><span class="sxs-lookup"><span data-stu-id="0ada6-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="0ada6-126">Azure-Reservierungen bilden bei Kombination mit Software wie Microsoft Windows Server und Azure SQL-Datenbank die Grundlage für komplette Infrastrukturlösungen.</span><span class="sxs-lookup"><span data-stu-id="0ada6-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="0ada6-127">Sie können Azure-Reservierungen sowohl im Partner Center- als auch im Azure-Portal sowie mithilfe der Partner Center-API kaufen, verkaufen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="0ada6-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="0ada6-128">Sie können auch Ihren Kunden die Berechtigung erteilen, ihre eigenen Azure-Reservierungen von einem Azure-Abonnement zu erwerben, das Sie für Sie erworben haben.</span><span class="sxs-lookup"><span data-stu-id="0ada6-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="0ada6-129">Weitere Informationen finden Sie unter folgenden Links.</span><span class="sxs-lookup"><span data-stu-id="0ada6-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="0ada6-130">Ressourcen zu Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="0ada6-130">Azure reservations resources</span></span>

|<span data-ttu-id="0ada6-131">**Informationen über**</span><span class="sxs-lookup"><span data-stu-id="0ada6-131">**For information about**</span></span>   |<span data-ttu-id="0ada6-132">**Artikel**</span><span class="sxs-lookup"><span data-stu-id="0ada6-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="0ada6-133">Dokumentation zu Azure-Reservierungen für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="0ada6-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="0ada6-134">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="0ada6-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="0ada6-135">Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="0ada6-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="0ada6-136">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="0ada6-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="0ada6-137">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="0ada6-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="0ada6-138">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="0ada6-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="0ada6-139">Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden</span><span class="sxs-lookup"><span data-stu-id="0ada6-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="0ada6-140">Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="0ada6-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="0ada6-141">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="0ada6-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="0ada6-142">[Kaufen von Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="0ada6-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="0ada6-143">Gewähren von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von Ihrem CSP-Abonnement zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="0ada6-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="0ada6-144">Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="0ada6-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |