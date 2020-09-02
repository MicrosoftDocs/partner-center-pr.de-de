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
ms.openlocfilehash: 7f6ca7aa7dddbd9e32690928ee8d48afa5071b14
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2020
ms.locfileid: "89367034"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="7fc08-104">Verkaufen Sie Microsoft Azure Reservierungen an Kunden, die Partner Center, die Azure-Portal oder APIs verwenden.</span><span class="sxs-lookup"><span data-stu-id="7fc08-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="7fc08-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="7fc08-105">**Applies to**</span></span>

- <span data-ttu-id="7fc08-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="7fc08-106">Partner Center</span></span>
- <span data-ttu-id="7fc08-107">Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="7fc08-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="7fc08-108">Partner im CSP-Programm</span><span class="sxs-lookup"><span data-stu-id="7fc08-108">Partners in the CSP program</span></span>

<span data-ttu-id="7fc08-109">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="7fc08-109">**Appropriate roles**</span></span>

- <span data-ttu-id="7fc08-110">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="7fc08-110">Admin agent</span></span>
- <span data-ttu-id="7fc08-111">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="7fc08-111">Global admin</span></span>
- <span data-ttu-id="7fc08-112">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="7fc08-112">Helpdesk agent</span></span>
- <span data-ttu-id="7fc08-113">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="7fc08-113">Sales agent</span></span>
- <span data-ttu-id="7fc08-114">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="7fc08-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="7fc08-115">Dieser Artikel gilt nur für Partner im CSP-Programm (Cloud Solution Provider).</span><span class="sxs-lookup"><span data-stu-id="7fc08-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="7fc08-116">Kunden, die andere Abonnementtypen (z. b. Pay-as-you-go, individuelle, Microsoft-Kunden Vereinbarung oder Konzernvertrag Abonnements) verwenden, sollten stattdessen [diese Azure-Reservierungs Dokumentation](https://docs.microsoft.com/azure/cost-management-billing/reservations)lesen.</span><span class="sxs-lookup"><span data-stu-id="7fc08-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="7fc08-117">Partner im CSP-Programm können Ihren Kunden Microsoft Azure Reservierungen anbieten.</span><span class="sxs-lookup"><span data-stu-id="7fc08-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="7fc08-118">Kunden profitieren von deutlichen Einsparungen, wenn sie im Voraus reservieren.</span><span class="sxs-lookup"><span data-stu-id="7fc08-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="7fc08-119">Azure-Reservierungen bieten Kunden Einfachheit und Flexibilität auf folgende Weise:</span><span class="sxs-lookup"><span data-stu-id="7fc08-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="7fc08-120">Ein- oder dreijährige Reservierungslaufzeiten</span><span class="sxs-lookup"><span data-stu-id="7fc08-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="7fc08-121">Einfache Inbetriebnahme, sehr schnelles Setup</span><span class="sxs-lookup"><span data-stu-id="7fc08-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="7fc08-122">Jederzeitiges Stornieren oder Umtauschen reservierter Instanzen gegen angepasste Rückerstattung</span><span class="sxs-lookup"><span data-stu-id="7fc08-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="7fc08-123">Verwalten reservierter Instanzen auf Organisations- oder Abteilungsebene</span><span class="sxs-lookup"><span data-stu-id="7fc08-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="7fc08-124">Azure-Reservierungen können Kunden wie folgt ansprechen:</span><span class="sxs-lookup"><span data-stu-id="7fc08-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="7fc08-125">Reservierungen können für nutzungsbasierte Zahlungsmodelle erhebliche Einsparungen bieten.</span><span class="sxs-lookup"><span data-stu-id="7fc08-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="7fc08-126">Bessere Budgetierung und Prognosen mit Vorauszahlung für Laufzeiten von einem Jahr oder drei Jahren.</span><span class="sxs-lookup"><span data-stu-id="7fc08-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="7fc08-127">Priorisierte Rechenkapazität in der Azure-Region, die den Niederlassungen am nächsten ist</span><span class="sxs-lookup"><span data-stu-id="7fc08-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="7fc08-128">Azure-Reservierungen bilden bei Kombination mit Software wie Microsoft Windows Server und Azure SQL-Datenbank die Grundlage für komplette Infrastrukturlösungen.</span><span class="sxs-lookup"><span data-stu-id="7fc08-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="7fc08-129">Sie können Azure-Reservierungen sowohl im Partner Center- als auch im Azure-Portal sowie mithilfe der Partner Center-API kaufen, verkaufen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="7fc08-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="7fc08-130">Sie können auch Ihren Kunden die Berechtigung erteilen, ihre eigenen Azure-Reservierungen von einem Azure-Abonnement zu erwerben, das Sie für Sie erworben haben.</span><span class="sxs-lookup"><span data-stu-id="7fc08-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="7fc08-131">Weitere Informationen finden Sie unter folgenden Links.</span><span class="sxs-lookup"><span data-stu-id="7fc08-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="7fc08-132">Ressourcen zu Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="7fc08-132">Azure reservations resources</span></span>

|<span data-ttu-id="7fc08-133">**Informationen über**</span><span class="sxs-lookup"><span data-stu-id="7fc08-133">**For information about**</span></span>   |<span data-ttu-id="7fc08-134">**Artikel**</span><span class="sxs-lookup"><span data-stu-id="7fc08-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="7fc08-135">Dokumentation zu Azure-Reservierungen für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="7fc08-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="7fc08-136">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="7fc08-136">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="7fc08-137">Erwerb von Azure-Reservierungen für Ihre Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="7fc08-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="7fc08-138">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="7fc08-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="7fc08-139">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="7fc08-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="7fc08-140">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="7fc08-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="7fc08-141">Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden</span><span class="sxs-lookup"><span data-stu-id="7fc08-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="7fc08-142">Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="7fc08-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="7fc08-143">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="7fc08-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="7fc08-144">[Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="7fc08-144">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="7fc08-145">Gewähren von Kunden die Berechtigung, ihre eigenen Azure-Reservierungen von Ihrem CSP-Abonnement zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="7fc08-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="7fc08-146">Erteilen Sie Kunden die Berechtigung, ihre eigenen Azure-Reservierungen zu erwerben.</span><span class="sxs-lookup"><span data-stu-id="7fc08-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
