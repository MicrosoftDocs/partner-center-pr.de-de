---
title: 'Partner Center – Microsoft Azure: Übersicht über Reservierungen | Partner Center'
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Erfahren Sie, wie cloudlösungsanbieter Azure-Reservierungen für Kunden mithilfe von Partner Center, der Azure-Portal oder der Partner Center-API erwerben, verkaufen oder verwalten können.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, Reservierungen, verwalten, Abrechnung, kaufen, Azure-RI, Azure Reserved Instances
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: f6d6e073d33baafe8ca65c8b06b2e2097c350cbd
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722266"
---
# <a name="partner-center---sell-microsoft-azure-reservations"></a><span data-ttu-id="3f9ad-104">Partner Center – Verkaufen von Microsoft Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="3f9ad-104">Partner Center - Sell Microsoft Azure reservations</span></span>

<!--Maggie, 12/7/18 - Added "Partner Center" to metadata title and H1 title as per Catherine Watson in bug #19868631-->

<span data-ttu-id="3f9ad-105">**Zielgruppe**</span><span class="sxs-lookup"><span data-stu-id="3f9ad-105">**Applies to**</span></span>

- <span data-ttu-id="3f9ad-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="3f9ad-106">Partner Center</span></span>
- <span data-ttu-id="3f9ad-107">Microsoft Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="3f9ad-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="3f9ad-108">Partner im CSP</span><span class="sxs-lookup"><span data-stu-id="3f9ad-108">Partners in CSP</span></span>

<span data-ttu-id="3f9ad-109">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="3f9ad-109">**Appropriate roles**</span></span>

- <span data-ttu-id="3f9ad-110">Administratoragent</span><span class="sxs-lookup"><span data-stu-id="3f9ad-110">Admin agent</span></span>
- <span data-ttu-id="3f9ad-111">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="3f9ad-111">Global admin</span></span>
- <span data-ttu-id="3f9ad-112">Helpdesk-Agent</span><span class="sxs-lookup"><span data-stu-id="3f9ad-112">Helpdesk agent</span></span>
- <span data-ttu-id="3f9ad-113">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="3f9ad-113">Sales agent</span></span>
- <span data-ttu-id="3f9ad-114">Benutzerverwaltungsadministrator</span><span class="sxs-lookup"><span data-stu-id="3f9ad-114">User management admin</span></span>

<span data-ttu-id="3f9ad-115">Partner im Cloud Solution Provider-Programm (CSP) können ihren Kunden Microsoft Azure-Reservierungen anbieten.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-115">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="3f9ad-116">Kunden profitieren von deutlichen Einsparungen, wenn sie im Voraus reservieren.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="3f9ad-117">Azure-Reservierungen bieten Kunden Einfachheit und Flexibilität auf folgende Weise:</span><span class="sxs-lookup"><span data-stu-id="3f9ad-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="3f9ad-118">Ein- oder dreijährige Reservierungslaufzeiten</span><span class="sxs-lookup"><span data-stu-id="3f9ad-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="3f9ad-119">Einfache Inbetriebnahme, sehr schnelles Setup</span><span class="sxs-lookup"><span data-stu-id="3f9ad-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="3f9ad-120">Jederzeitiges Stornieren oder Umtauschen reservierter Instanzen gegen angepasste Rückerstattung</span><span class="sxs-lookup"><span data-stu-id="3f9ad-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="3f9ad-121">Verwalten reservierter Instanzen auf Organisations- oder Abteilungsebene</span><span class="sxs-lookup"><span data-stu-id="3f9ad-121">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="3f9ad-122">Azure-Reservierungen können Kunden wie folgt ansprechen:</span><span class="sxs-lookup"><span data-stu-id="3f9ad-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="3f9ad-123">Reservierungen können für nutzungsbasierte Zahlungsmodelle erhebliche Einsparungen bieten.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="3f9ad-124">Bessere Budgetierung und Prognosen mit Vorauszahlung für Laufzeiten von einem Jahr oder drei Jahren.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="3f9ad-125">Priorisierte Rechenkapazität in der Azure-Region, die den Niederlassungen am nächsten ist</span><span class="sxs-lookup"><span data-stu-id="3f9ad-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="3f9ad-126">Azure-Reservierungen bilden bei Kombination mit Software wie Microsoft Windows Server und Azure SQL-Datenbank die Grundlage für komplette Infrastrukturlösungen.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="3f9ad-127">Sie können Azure-Reservierungen sowohl im Partner Center- als auch im Azure-Portal sowie mithilfe der Partner Center-API kaufen, verkaufen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="3f9ad-128">Weitere Informationen finden Sie unter folgenden Links.</span><span class="sxs-lookup"><span data-stu-id="3f9ad-128">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="3f9ad-129">Ressourcen zu Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="3f9ad-129">Azure reservations resources</span></span>

|<span data-ttu-id="3f9ad-130">**Weitere Informationen zu**</span><span class="sxs-lookup"><span data-stu-id="3f9ad-130">**For information about**</span></span>   |<span data-ttu-id="3f9ad-131">**Bitte lesen**</span><span class="sxs-lookup"><span data-stu-id="3f9ad-131">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="3f9ad-132">Dokumentation zu Azure-Reservierungen für Ihre Kunden</span><span class="sxs-lookup"><span data-stu-id="3f9ad-132">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="3f9ad-133">Was sind Azure-Reservierungen?</span><span class="sxs-lookup"><span data-stu-id="3f9ad-133">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="3f9ad-134">Erwerb von Azure-Reservierungen für Ihre Kunden im Partner Center</span><span class="sxs-lookup"><span data-stu-id="3f9ad-134">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="3f9ad-135">Kaufen von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="3f9ad-135">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="3f9ad-136">Verwalten von Azure-Reservierungen in Partner Center</span><span class="sxs-lookup"><span data-stu-id="3f9ad-136">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="3f9ad-137">Verwalten von Azure-Reservierungen im Partner Center</span><span class="sxs-lookup"><span data-stu-id="3f9ad-137">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="3f9ad-138">Bestimmen der richtigen VM-Größe und Überprüfen der VM-Nutzung durch den Kunden</span><span class="sxs-lookup"><span data-stu-id="3f9ad-138">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="3f9ad-139">Bestimmen der VM-Größe für die maximale Nutzung von Azure-Reservierungen</span><span class="sxs-lookup"><span data-stu-id="3f9ad-139">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="3f9ad-140">Erwerb von Azure-Reservierungen über die Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="3f9ad-140">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="3f9ad-141">[Kaufen von Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in der Partner Center-Entwicklerdokumentation</span><span class="sxs-lookup"><span data-stu-id="3f9ad-141">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
