---
title: Berechnung der Gutschrift durch den Partner Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie der Azure-Plan für Partner verdiente Gutschriften ("Partner verdiente Guthaben") berechnet wird. Dies schließt die Berechtigungsanforderungen für Partner und indirekte Anbieter ein.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 59cbc822e886b031a49c281334e8287580311408
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253416"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="8f798-104">Berechnen der Gutschrift für den Partner (PEC)</span><span class="sxs-lookup"><span data-stu-id="8f798-104">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="8f798-105">Partner, die die rund um die Uhr über die IT-Betriebsverwaltung von Teilen oder die gesamte Azure-Umgebung ihrer Kunden im CSP besitzen, werden mit PEC belohnt.</span><span class="sxs-lookup"><span data-stu-id="8f798-105">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="8f798-106">Das PEC wird als Teil der Rechnung an den Partner über eine direkte abrechnungsbeziehung mit Microsoft bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="8f798-106">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="8f798-107">Die Gutschrift wird täglich berechnet und in der monatlichen Rechnung widergespiegelt.</span><span class="sxs-lookup"><span data-stu-id="8f798-107">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="8f798-108">Standardmäßig erhalten Partner in CSP die erforderlichen Zugriffsrechte für das Abonnement des Kunden, das es Ihnen ermöglicht, rund um die Uhr Betriebsverwaltung zu verfügen und die Ressourcen des Abonnements zu steuern.</span><span class="sxs-lookup"><span data-stu-id="8f798-108">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="8f798-109">Weitere Möglichkeiten zum Bereitstellen von Zugriff für einen Transaktionspartner finden Sie im folgenden Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="8f798-109">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="8f798-110">Wichtige Anforderungen für die Eignung und Berechnung:</span><span class="sxs-lookup"><span data-stu-id="8f798-110">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="8f798-111">Ein Partner sollte über eine aktive MPN-Vereinbarung und eine gültige RBAC-Rolle (Role Based Account C) verfügen, um eine Gutschrift für die von Ihnen verwalteten Azure-Ressourcen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="8f798-111">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="8f798-112">Weitere Informationen zu [gültige RBAC-Rollen]</span><span class="sxs-lookup"><span data-stu-id="8f798-112">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="8f798-113">Der indirekte Anbieter kann sich für die Verwaltung von Management Pack qualifizieren, wenn Sie oder der indirekte Händler über eine operative Kontrolle und Verwaltung der Azure-Ressourcen des Kunden in CSP verfügen.</span><span class="sxs-lookup"><span data-stu-id="8f798-113">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="8f798-114">PEC ist der abgerechneten (kostenpflichtigen) Nutzung der Azure-Umgebung des Kunden in CSP zugeordnet, die vom Partner verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="8f798-114">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="8f798-115">PEC ist nur für Partner in CSP verfügbar, die von Microsoft (indirekter Anbieter und direkter Rechnungs Partner) abgerechnet werden.</span><span class="sxs-lookup"><span data-stu-id="8f798-115">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="8f798-116">Berechtigte Dienste: die Gutschrift eines Partners ist für alle Azure-1-PP-Azure-Verbrauchs in der Preisliste anwendbar.</span><span class="sxs-lookup"><span data-stu-id="8f798-116">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="8f798-117">Es gibt Ausnahmen, einschließlich, aber nicht beschränkt auf 3PP und Azure reservations.</span><span class="sxs-lookup"><span data-stu-id="8f798-117">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="8f798-118">PEC wird täglich berechnet und kann in der täglichen Reconnaissance-Datei angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="8f798-118">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="8f798-119">Ein Partner (Anbieter oder Reseller (über seinen Anbieter) muss für den ganzen Tag (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er die Leistung von PEC erhält.</span><span class="sxs-lookup"><span data-stu-id="8f798-119">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="8f798-120">PEC wird bis hinab zur Azure-Ressourcenebene erworben.</span><span class="sxs-lookup"><span data-stu-id="8f798-120">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="8f798-121">Wenn der Partner über einen gültigen Zugriff auf Abonnement-oder Ressourcengruppen Ebene verfügt, wird jede Ressource, die für die höhere Entität verwendet wird, mit dem Wert "PEC" erhalten.</span><span class="sxs-lookup"><span data-stu-id="8f798-121">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="8f798-122">PEC wird in die monatliche Rechnung des Partners eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="8f798-122">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="8f798-123">Die Rechnung ist gebührenpflichtig.</span><span class="sxs-lookup"><span data-stu-id="8f798-123">The invoice is net of charges.</span></span> <span data-ttu-id="8f798-124">Die Details werden in der Datei "Rechnungs Reconnaissance" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8f798-124">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="8f798-125">Weitere Informationen zum Zugriff auf die Verwaltung von Azure-Abonnements und zum Verknüpfen ihrer MPN-ID mit RBAC-Rollen finden Sie [unter Verwalten von Abonnements und Ressourcen im Azure-Plan](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="8f798-125">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="8f798-126">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="8f798-126">For more information</span></span>

- [<span data-ttu-id="8f798-127">Azure-Plan: Abrechnung</span><span class="sxs-lookup"><span data-stu-id="8f798-127">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="8f798-128">Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP </span><span class="sxs-lookup"><span data-stu-id="8f798-128">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)