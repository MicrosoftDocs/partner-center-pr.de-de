---
title: Vom Partner erworbenes Guthaben für verwaltete Dienste (Vorschau) | Partner Center
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hier erfährst du, wie die durch Microsoft-Partner erworbenen Guthaben für verwaltete Dienste berechnet und ausgezahlt werden und wie du deine Berechtigung für das Programm prüfen kannst.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 776fea7eea91e15f872021356562af05e89f1fcf
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2020
ms.locfileid: "75004999"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="2683d-103">Wie von Partnern erworbene Guthaben berechnet und bezahlt werden</span><span class="sxs-lookup"><span data-stu-id="2683d-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="2683d-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="2683d-104">**Appropriate roles**</span></span>
-   <span data-ttu-id="2683d-105">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="2683d-105">Global admin</span></span>
-   <span data-ttu-id="2683d-106">Benutzeradministrator</span><span class="sxs-lookup"><span data-stu-id="2683d-106">User admin</span></span>
-   <span data-ttu-id="2683d-107">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="2683d-107">Admin agent</span></span>
-   <span data-ttu-id="2683d-108">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="2683d-108">Billing admin</span></span>
-   <span data-ttu-id="2683d-109">Vertriebsbeauftragter</span><span class="sxs-lookup"><span data-stu-id="2683d-109">Sales agent</span></span>

<span data-ttu-id="2683d-110">Von Partnern erworbene Guthaben für verwaltete Dienste (Partner-Earned Credit, PEC) bedeuten Anerkennung und Belohnung für Partner, die die Kontrolle und Verwaltung der IT Operations der Azure-Umgebungen ihrer Kunden rund um die Uhr ganz oder teilweise innehaben.</span><span class="sxs-lookup"><span data-stu-id="2683d-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="2683d-111">Standardmäßig werden Partnern in CSP die erforderlichen Zugriffsrechte auf das Kundenabonnement erteilt, die es ihnen ermöglichen, die operative Verwaltung und Steuerung der Abonnementressourcen rund um die Uhr (24/7) durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="2683d-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="2683d-112">Weitere Möglichkeiten, wie der Kunde den Zugriff für den handelnden Partner bereitstellen kann, sind im folgenden Abschnitt beschrieben.</span><span class="sxs-lookup"><span data-stu-id="2683d-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="2683d-113">Der monatliche Rechnungsbetrag ist bezogen auf die vom Partner erworbene Gutschrift netto.</span><span class="sxs-lookup"><span data-stu-id="2683d-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="2683d-114">Die Partner können die PEC-Details in ihrer monatlichen Abstimmungsdatei sehen.</span><span class="sxs-lookup"><span data-stu-id="2683d-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="2683d-115">Informationen zu weiteren Verfahren, mit denen ein Kunde den Zugriff für den handelnden Partner bereitstellen kann, finden Sie unter [Verwalten von Abonnements und Ressourcen in einem Azure-Plan](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="2683d-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="2683d-116">Lesen Sie auch [Reaktivieren von Administratorrechten für Azure CSP-Abonnements](revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="2683d-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="2683d-117">Wichtige Informationen zu Berechtigung und Berechnung</span><span class="sxs-lookup"><span data-stu-id="2683d-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="2683d-118">Der Partner sollte einen aktiven MPN-Vertrag und eine gültige RBAC-Rolle besitzen, um erworbene Gutschriften für die von ihm verwalteten Azure-Ressourcen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="2683d-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="2683d-119">Im Fall indirekter Anbieter und ihrer indirekten Wiederverkäufer ist der indirekte Anbieter für PEC qualifiziert, wenn entweder er, der indirekte Wiederverkäufer oder beide die operative Steuerung und Verwaltung der Azure-Ressourcen des Kunden in CSP rund um die Uhr (24/7) sicherstellen.</span><span class="sxs-lookup"><span data-stu-id="2683d-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="2683d-120">PEC ist der abgerechneten (kostenpflichtigen) Nutzung der Azure-Umgebung des Kunden in CSP zugeordnet, die vom Partner verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="2683d-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="2683d-121">PEC ist nur für Partner in CSP verfügbar, die mit Microsoft abrechnen (indirekter Anbieter und Direktrechnungspartner).</span><span class="sxs-lookup"><span data-stu-id="2683d-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="2683d-122">Berechtigte Dienste: Von Partnern erworbenes Guthaben kann auf Dienste angerechnet werden, die in den **Preisen für Azure-Plannutzung** aufgelistet sind, die Partner von der Seite [Azure-Plan-Preise](https://partner.microsoft.com/commerce/sales) exportieren können.</span><span class="sxs-lookup"><span data-stu-id="2683d-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="2683d-123">Beachten Sie, dass es Ausnahmen gibt, beispielsweise Produkte von Drittanbietern, die in der **Tags**-Spalte der Preisliste für die Azure-Plannutzung und Azure-Plan Reservierungen als **Drittanbieter** gekennzeichnet sind, sowie Produkte in der Marketplace-Preisliste.</span><span class="sxs-lookup"><span data-stu-id="2683d-123">Note, there are exceptions including, but not limited to, third-party products identified as **Third Party** in  the **Tags** column of the Azure plan consumption price list and Azure Plan reservations, and products in the Marketplace price list.</span></span>

- <span data-ttu-id="2683d-124">PEC wird täglich berechnet und kann in der täglichen Nutzungsdatei und der Abstimmungsdatei zur monatlichen Rechnung angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2683d-124">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="2683d-125">Ein Partner (indirekter Anbieter oder indirekter Wiederverkäufer) muss den gesamten Tag hindurch (rund um die Uhr) Zugriff haben, um sicherzustellen, dass er PEC erwirbt.</span><span class="sxs-lookup"><span data-stu-id="2683d-125">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>  

- <span data-ttu-id="2683d-126">PEC wird bis hinab zur Azure-Ressourcenebene erworben.</span><span class="sxs-lookup"><span data-stu-id="2683d-126">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="2683d-127">Wenn der Partner über gültigen Zugriff verfügt, verdient jede Ressource auf Abonnement- oder Ressourcengruppenebene, die an die nächst höhere Entität berichtet, PEC.</span><span class="sxs-lookup"><span data-stu-id="2683d-127">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="2683d-128">Die Details von PEC sind auch unter [Azure-Kostenmanagement](https://go.microsoft.com/fwlink/?linkid=2106482) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2683d-128">PEC details will also be available on [Azure Cost management](https://go.microsoft.com/fwlink/?linkid=2106482)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="2683d-129">Azure-Kostenmanagement</span><span class="sxs-lookup"><span data-stu-id="2683d-129">Azure Cost Management</span></span>

 <span data-ttu-id="2683d-130">Azure Cost Management (ACM) mit Kostenanalyse ermöglicht es Ihnen als Partner, die Kosten anzuzeigen, auf die der PEC-Vorteil angerechnet wurde.</span><span class="sxs-lookup"><span data-stu-id="2683d-130">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="2683d-131">Melden Sie sich im Azure-Portal bei Ihrem Partnermandanten an, und wählen Sie **Kostenmanagement + Abrechnung** aus.</span><span class="sxs-lookup"><span data-stu-id="2683d-131">In the Azure Portal, sign into your partner tenant and select **Cost Management + Billing**.</span></span>
2.  <span data-ttu-id="2683d-132">Wählen Sie **Kostenmanagement** aus.</span><span class="sxs-lookup"><span data-stu-id="2683d-132">Select **Cost management**</span></span>
3.  <span data-ttu-id="2683d-133">Wählen Sie **Kostenanalyse** aus.</span><span class="sxs-lookup"><span data-stu-id="2683d-133">Select **Cost Analysis**</span></span>

<span data-ttu-id="2683d-134">In der Ansicht „Kostenanalyse“ werden die Kosten für Ihr Abrechnungskonto für alle erworbenen und genutzten Dienste mit den Preisen angezeigt, die Sie an Microsoft bezahlen.</span><span class="sxs-lookup"><span data-stu-id="2683d-134">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4.  <span data-ttu-id="2683d-135">Wählen Sie **PartnerEarnedCreditApplied** in der Dropdownliste einer PivotChart aus, um die Kosten anzuzeigen, auf die PEC angerechnet wurden.</span><span class="sxs-lookup"><span data-stu-id="2683d-135">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="2683d-136">Wenn die **PartnerEarnedCreditApplied**-Eigenschaft den Wert „True“ aufweist, wurde auf die zugehörigen Kosten das vom Partner erworbene Guthaben angerechnet.</span><span class="sxs-lookup"><span data-stu-id="2683d-136">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="2683d-137">Wenn die Eigenschaft „PartnerEarnedCreditApplied“ den Wert „False“ aufweist, haben die zugehörigen Kosten nicht die erforderliche Berechtigung für die Gutschrift erfüllt, oder der erworbene Dienst ist nicht für PEC qualifiziert.</span><span class="sxs-lookup"><span data-stu-id="2683d-137">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

<span data-ttu-id="2683d-138">Hinweis: In der Regel dauert es 8-24 Stunden, bis die Verwendung von Diensten unter **Kostenmanagement** angezeigt wird, und die PEC-Gutschriften werden innerhalb von 48 Stunden ab dem Zeitpunkt des Zugriffs in Azure Cost Management angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2683d-138">Note:Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="2683d-139">Sie können auch nach der **PartnerEarnedCreditApplied** Eigenschaft gruppieren und filtern, indem Sie die Filterfeatures **Gruppieren nach** verwenden, um einen Drilldown der Kosten auszuführen, für die PEC angerechnet ober nicht angerechnet wurden.</span><span class="sxs-lookup"><span data-stu-id="2683d-139">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

 <span data-ttu-id="2683d-140">**Weitere Informationen**</span><span class="sxs-lookup"><span data-stu-id="2683d-140">**For more information**</span></span>

- [<span data-ttu-id="2683d-141">Vom Partner erworbenes Guthaben – Übersicht</span><span class="sxs-lookup"><span data-stu-id="2683d-141">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="2683d-142">Detaillierte Berechnungsbeispiele für von Partnern erworbenes Guthaben finden Sie in der Preisliste, auf die Sie über das Partner Center-Dashboard zugreifen können (Anmeldung erforderlich).</span><span class="sxs-lookup"><span data-stu-id="2683d-142">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="2683d-143">Umstellung auf Azure-Plan: Einstieg</span><span class="sxs-lookup"><span data-stu-id="2683d-143">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="2683d-144">Verwalten von Abonnements und Ressourcen in einem Azure-Plan</span><span class="sxs-lookup"><span data-stu-id="2683d-144">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="2683d-145">Wiederrufen oder Reaktivieren von Administratorrechten für Azure CSP-Abonnements</span><span class="sxs-lookup"><span data-stu-id="2683d-145">Revoke or re-instate admin privileges for Azure CSP subscriptions  </span></span>](revoke-reinstate-csp.md)

