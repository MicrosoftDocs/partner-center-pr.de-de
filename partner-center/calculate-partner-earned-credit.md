---
title: Berechnen der Gutschrift für den Partner
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Erfahren Sie, wie der Azure-Plan für Partner verdiente Gutschriften ("Partner verdiente Guthaben") berechnet wird. Dies schließt die Berechtigungsanforderungen für Partner und indirekte Anbieter ein.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 065cf0c8f95667b470081edcb1b66398235604b3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948137"
---
# <a name="how-partner-earned-credit-pec-is-calculated-for-partners-in-the-cloud-solution-provider-program"></a><span data-ttu-id="0464c-104">Wie Partner Guthaben (PEC) für Partner im Cloud Solution Provider-Programm berechnet werden</span><span class="sxs-lookup"><span data-stu-id="0464c-104">How partner earned credit (PEC) is calculated for partners in the Cloud Solution Provider program</span></span>

<span data-ttu-id="0464c-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="0464c-105">**Appropriate roles**</span></span>

- <span data-ttu-id="0464c-106">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="0464c-106">Global admin</span></span>
- <span data-ttu-id="0464c-107">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="0464c-107">Billing admin</span></span>

<span data-ttu-id="0464c-108">Partner, die die rund um die Uhr über die IT-Betriebsverwaltung von Teilen oder die gesamte Azure-Umgebung ihrer Kunden im CSP besitzen, werden mit PEC belohnt.</span><span class="sxs-lookup"><span data-stu-id="0464c-108">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="0464c-109">Das PEC wird als Teil der Rechnung an den Partner über eine direkte abrechnungsbeziehung mit Microsoft bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="0464c-109">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="0464c-110">Die Gutschrift wird täglich berechnet und in der monatlichen Rechnung widergespiegelt.</span><span class="sxs-lookup"><span data-stu-id="0464c-110">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="0464c-111">Standardmäßig erhalten Partner in CSP die erforderlichen Zugriffsrechte für das Abonnement des Kunden, das es Ihnen ermöglicht, rund um die Uhr Betriebsverwaltung zu verfügen und die Ressourcen des Abonnements zu steuern.</span><span class="sxs-lookup"><span data-stu-id="0464c-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="0464c-112">Weitere Möglichkeiten zum Bereitstellen von Zugriff für einen Transaktionspartner finden Sie im folgenden Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="0464c-112">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="0464c-113">Wichtige Anforderungen für die Eignung und Berechnung:</span><span class="sxs-lookup"><span data-stu-id="0464c-113">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="0464c-114">Ein Partner sollte über eine aktive MPN-Vereinbarung und eine gültige regelbasierte Rolle für die Konto Steuerung (RBAC) verfügen, um eine Gutschrift für die von Ihnen verwalteten Azure-Ressourcen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="0464c-114">A partner should have an active MPN agreement and a valid Rules Based Account Control (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="0464c-115">Weitere Informationen zu [gültige RBAC-Rollen]</span><span class="sxs-lookup"><span data-stu-id="0464c-115">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="0464c-116">Der indirekte Anbieter kann sich für die Verwaltung von Management Pack qualifizieren, wenn Sie oder der indirekte Händler über eine operative Kontrolle und Verwaltung der Azure-Ressourcen des Kunden in CSP verfügen.</span><span class="sxs-lookup"><span data-stu-id="0464c-116">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="0464c-117">PEC ist der abgerechneten (kostenpflichtigen) Nutzung der Azure-Umgebung des Kunden in CSP zugeordnet, die vom Partner verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="0464c-117">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="0464c-118">PEC ist nur für Partner in CSP verfügbar, die von Microsoft (indirekter Anbieter und direkter Rechnungs Partner) abgerechnet werden.</span><span class="sxs-lookup"><span data-stu-id="0464c-118">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="0464c-119">Berechtigte Dienste: die Gutschrift eines Partners ist für alle Azure-1-PP-Azure-Verbrauchs in der Preisliste anwendbar.</span><span class="sxs-lookup"><span data-stu-id="0464c-119">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="0464c-120">Es gibt Ausnahmen, einschließlich, aber nicht beschränkt auf 3PP und Azure reservations.</span><span class="sxs-lookup"><span data-stu-id="0464c-120">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="0464c-121">PEC wird täglich berechnet und kann in der täglichen Reconnaissance-Datei angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0464c-121">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="0464c-122">Ein Partner (Anbieter oder Reseller (über seinen Anbieter) muss für den ganzen Tag (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er die Leistung von PEC erhält.</span><span class="sxs-lookup"><span data-stu-id="0464c-122">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="0464c-123">PEC wird bis hinab zur Azure-Ressourcenebene erworben.</span><span class="sxs-lookup"><span data-stu-id="0464c-123">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="0464c-124">Wenn der Partner über einen gültigen Zugriff auf Abonnement-oder Ressourcengruppen Ebene verfügt, wird jede Ressource, die für die höhere Entität verwendet wird, mit dem Wert "PEC" erhalten.</span><span class="sxs-lookup"><span data-stu-id="0464c-124">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="0464c-125">PEC wird in die monatliche Rechnung des Partners eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="0464c-125">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="0464c-126">Die Rechnung ist gebührenpflichtig.</span><span class="sxs-lookup"><span data-stu-id="0464c-126">The invoice is net of charges.</span></span> <span data-ttu-id="0464c-127">Die Details werden in der Datei "Rechnungs Reconnaissance" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0464c-127">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="0464c-128">Weitere Informationen zum Zugriff auf die Verwaltung von Azure-Abonnements und zum Verknüpfen ihrer MPN-ID mit RBAC-Rollen finden Sie [unter Verwalten von Abonnements und Ressourcen im Azure-Plan](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="0464c-128">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="0464c-129">Weitere Informationen finden Sie unter</span><span class="sxs-lookup"><span data-stu-id="0464c-129">For more information</span></span>

- [<span data-ttu-id="0464c-130">Azure-Plan: Abrechnung</span><span class="sxs-lookup"><span data-stu-id="0464c-130">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="0464c-131">Preisliste für die neue E-Commerce-Benutzeroberfläche in CSP </span><span class="sxs-lookup"><span data-stu-id="0464c-131">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)