---
title: Berechnung der Gutschrift durch den Partner Partner Center
ms.topic: article
ms.date: 09/17/2019
description: Berechnung der Gutschrift des Partners für die Gutschrift des Azure-Plans
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318768"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="96e2f-103">Berechnen der Gutschrift für den Partner (PEC)</span><span class="sxs-lookup"><span data-stu-id="96e2f-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="96e2f-104">Partner, die die rund um die Uhr über die IT-Betriebsverwaltung von Teilen oder die gesamte Azure-Umgebung ihrer Kunden im CSP besitzen, werden mit PEC belohnt.</span><span class="sxs-lookup"><span data-stu-id="96e2f-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="96e2f-105">Das PEC wird als Teil der Rechnung an den Partner über eine direkte abrechnungsbeziehung mit Microsoft bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="96e2f-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="96e2f-106">Die Gutschrift wird täglich berechnet und in der monatlichen Rechnung widergespiegelt.</span><span class="sxs-lookup"><span data-stu-id="96e2f-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="96e2f-107">Standardmäßig erhalten Partner in CSP die erforderlichen Zugriffsrechte für das Abonnement des Kunden, das es Ihnen ermöglicht, rund um die Uhr Betriebsverwaltung zu verfügen und die Ressourcen des Abonnements zu steuern.</span><span class="sxs-lookup"><span data-stu-id="96e2f-107">By default, in CSP, partners are granted the necessary access rights to the customer’s subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="96e2f-108">Weitere Möglichkeiten zum Bereitstellen von Zugriff für einen Transaktionspartner finden Sie im folgenden Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="96e2f-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="96e2f-109">Wichtige Anforderungen für die Eignung und Berechnung:</span><span class="sxs-lookup"><span data-stu-id="96e2f-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="96e2f-110">Ein Partner sollte über eine aktive MPN-Vereinbarung und eine gültige RBAC-Rolle (Role Based Account C) verfügen, um eine Gutschrift für die von Ihnen verwalteten Azure-Ressourcen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="96e2f-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="96e2f-111">Weitere Informationen zu [gültige RBAC-Rollen]</span><span class="sxs-lookup"><span data-stu-id="96e2f-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="96e2f-112">Der indirekte Anbieter kann sich für die Verwaltung von Management Pack qualifizieren, wenn Sie oder der indirekte Händler über eine operative Kontrolle und Verwaltung der Azure-Ressourcen des Kunden in CSP verfügen.</span><span class="sxs-lookup"><span data-stu-id="96e2f-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer’s Azure resources in CSP.</span></span>

- <span data-ttu-id="96e2f-113">PEC ist dem in Rechnung gestellten (kostenpflichtigen) Verbrauch des Azure-Immobilienkunden in CSP zugeordnet, der vom Partner verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="96e2f-113">PEC is associated to billed (chargeable) consumption of customer’s Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="96e2f-114">PEC ist nur für Partner in CSP verfügbar, die von Microsoft (indirekter Anbieter und direkter Rechnungs Partner) abgerechnet werden.</span><span class="sxs-lookup"><span data-stu-id="96e2f-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="96e2f-115">Berechtigte Dienste: die Gutschrift eines Partners ist für alle Azure-1-PP-Azure-Verbrauchs in der Preisliste anwendbar.</span><span class="sxs-lookup"><span data-stu-id="96e2f-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="96e2f-116">Es gibt Ausnahmen, einschließlich, aber nicht beschränkt auf 3PP und Azure reservations.</span><span class="sxs-lookup"><span data-stu-id="96e2f-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="96e2f-117">PEC wird täglich berechnet und kann in der täglichen Reconnaissance-Datei angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="96e2f-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="96e2f-118">Ein Partner (Anbieter oder Reseller (über seinen Anbieter) muss für den ganzen Tag (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er die Leistung von PEC erhält.</span><span class="sxs-lookup"><span data-stu-id="96e2f-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="96e2f-119">Die Azure-Ressourcenebene reicht von der Azure-Ressourcenebene.</span><span class="sxs-lookup"><span data-stu-id="96e2f-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="96e2f-120">Wenn der Partner über einen gültigen Zugriff auf Abonnement-oder Ressourcengruppen Ebene verfügt, wird jede Ressource, die für die höhere Entität verwendet wird, mit dem Wert "PEC" erhalten.</span><span class="sxs-lookup"><span data-stu-id="96e2f-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="96e2f-121">PEC wird in die monatliche Rechnung des Partners eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="96e2f-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="96e2f-122">Die Rechnung ist gebührenpflichtig.</span><span class="sxs-lookup"><span data-stu-id="96e2f-122">The invoice is net of charges.</span></span> <span data-ttu-id="96e2f-123">Die Details werden in der Datei "Rechnungs Reconnaissance" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="96e2f-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="96e2f-124">Weitere Informationen zum Zugriff auf die Verwaltung von Azure-Abonnements und zum Verknüpfen ihrer MPN-ID mit RBAC-Rollen finden Sie [unter Verwalten von Abonnements und Ressourcen im Azure-Plan](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="96e2f-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="96e2f-125">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="96e2f-125">For more information</span></span>

- [<span data-ttu-id="96e2f-126">Azure-Plan: Abrechnung</span><span class="sxs-lookup"><span data-stu-id="96e2f-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="96e2f-127">Preisliste für die neue Commerce-Funktion in CSP</span><span class="sxs-lookup"><span data-stu-id="96e2f-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)