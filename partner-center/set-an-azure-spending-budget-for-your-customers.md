---
title: Festlegen eines Azure-Ausgabenbudgets für Kunden
ms.topic: how-to
ms.date: 03/17/2021
description: Erfahren Sie, wie Sie monatliche Azure-Ausgabenbudgets für Ihre Kunden festlegen oder entfernen sowie Azure-Ausgabendaten anzeigen und budgetbezogene Benachrichtigungen festlegen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855351"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="dac8f-103">Festlegen, Überprüfen oder Entfernen monatlicher Azure-Ausgabenbudgets für Kunden in Partner Center</span><span class="sxs-lookup"><span data-stu-id="dac8f-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="dac8f-104">**Geeignete Rollen:** Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="dac8f-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="dac8f-105">Sie können [ein monatliches Azure-Ausgabenbudget für Ihre Kunden](#set-azure-spending-budget) in Partner Center festlegen.</span><span class="sxs-lookup"><span data-stu-id="dac8f-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="dac8f-106">Dies hilft Ihren Kunden bei der Verwaltung ihrer Azure-Ausgaben.</span><span class="sxs-lookup"><span data-stu-id="dac8f-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="dac8f-107">Mit dieser Option können Sie die Azure-Ausgaben Ihrer Kunden mit dem Budget während des Monats vergleichen.</span><span class="sxs-lookup"><span data-stu-id="dac8f-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="dac8f-108">Außerdem können Ihre Kunden ihre Azure-Ausgaben so planen, dass ihre monatliche Rechnung nicht höher als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="dac8f-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="dac8f-109">Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="dac8f-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="dac8f-110">Nachdem Sie [ein Azure-Ausgabenbudget für Ihre Kunden festgelegt](#set-azure-spending-budget)haben, können Sie die Kundennutzung auch wie folgt überprüfen.</span><span class="sxs-lookup"><span data-stu-id="dac8f-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="dac8f-111">Diese Optionen können Ihnen helfen, falsch konfigurierte Dienste oder ungewöhnliche Trends zu erkennen, die auf Betrug hindeuten können.</span><span class="sxs-lookup"><span data-stu-id="dac8f-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="dac8f-112">Anschließend können Sie mit Ihren Kunden zusammenarbeiten, um die Grundursache zu ermitteln und die Kosten zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="dac8f-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="dac8f-113">Bei Bedarf können Sie auch das Budget des Kunden in einen höheren Betrag [ändern.](#set-azure-spending-budget)</span><span class="sxs-lookup"><span data-stu-id="dac8f-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="dac8f-114">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="dac8f-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="dac8f-115">Aktivieren von E-Mail-Benachrichtigungen für den Zeitpunkt, an dem sich die Ausgaben eines Kunden dem Budgetlimit nähern</span><span class="sxs-lookup"><span data-stu-id="dac8f-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="dac8f-116">Anzeigen der aufgeschlüsselten Kosten nach Dienst für nutzungsbasierte Abonnements</span><span class="sxs-lookup"><span data-stu-id="dac8f-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="dac8f-117">Sie können auch [jederzeit ein Azure-Ausgabenbudget](#remove-azure-spending-budget) für Kunden entfernen.</span><span class="sxs-lookup"><span data-stu-id="dac8f-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="dac8f-118">Azure-Ausgabendaten</span><span class="sxs-lookup"><span data-stu-id="dac8f-118">Azure spending data</span></span>

<span data-ttu-id="dac8f-119">Die Azure-Ausgabendaten sind eine *Schätzung,* und *die tatsächlichen Abrechnungsbeträge können variieren.*</span><span class="sxs-lookup"><span data-stu-id="dac8f-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="dac8f-120">Der Wert der Daten *spiegelt keine* Steuern, Gutschriften, Anpassungen oder andere Gebühren wider, die möglicherweise anfallen.</span><span class="sxs-lookup"><span data-stu-id="dac8f-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="dac8f-121">Die Ausgabendaten *werden einmal pro Tag aktualisiert.*</span><span class="sxs-lookup"><span data-stu-id="dac8f-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="dac8f-122">Ihre Kunden können weiterhin Azure-Dienste und -Ressourcen verwenden (und dafür in Rechnung gestellt werden), es sei denn, Sie ändern ihre Kontoeinstellungen im Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="dac8f-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="dac8f-123">Festlegen des Azure-Ausgabenbudgets</span><span class="sxs-lookup"><span data-stu-id="dac8f-123">Set Azure spending budget</span></span>

<span data-ttu-id="dac8f-124">Sie können *ein monatliches Azure-Ausgabenbudget* für mehrere Kunden in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="dac8f-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="dac8f-125">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="dac8f-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dac8f-126">Wählen Sie im linken Menü unter **CSP** die Option **Azure-Ausgaben aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dac8f-127">Wählen Sie **auf der Seite Azure-Ausgaben** unter Kunden **Microsoft Azure** Abonnements die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="dac8f-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="dac8f-128">Geben Sie einen Wert für **Monatliches Budget ein.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="dac8f-129">Wählen Sie **Übernehmen aus,** um Ihre Änderungen zu speichern.</span><span class="sxs-lookup"><span data-stu-id="dac8f-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="dac8f-130">Sie können auch *ein Budget für einen einzelnen Kunden* in den Abonnementeinstellungen festlegen:</span><span class="sxs-lookup"><span data-stu-id="dac8f-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="dac8f-131">Melden Sie sich beim Partner Center-Dashboard an.</span><span class="sxs-lookup"><span data-stu-id="dac8f-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="dac8f-132">Wählen Sie im linken Menü unter **CSP** die Option **Kunden aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="dac8f-133">Wählen Sie **auf der** Seite Kunden den Firmennamen des **Kunden aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="dac8f-134">Wählen Sie auf der Seite **Abonnements des** Kunden unter **Nutzungsbasiertes Abonnement** die Option Budget ändern **aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="dac8f-135">Geben Sie einen Wert für das Budget ein.</span><span class="sxs-lookup"><span data-stu-id="dac8f-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="dac8f-136">Wählen Sie **Übernehmen aus,** um Ihre Änderungen zu speichern.</span><span class="sxs-lookup"><span data-stu-id="dac8f-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="dac8f-137">Entfernen des Azure-Ausgabenbudgets</span><span class="sxs-lookup"><span data-stu-id="dac8f-137">Remove Azure spending budget</span></span>

<span data-ttu-id="dac8f-138">Sie können *ein monatliches Azure-Ausgabenbudget* für Ihre Kunden in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="dac8f-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="dac8f-139">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="dac8f-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dac8f-140">Wählen Sie im linken Menü unter **CSP** die Option **Azure-Ausgaben aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dac8f-141">Wählen Sie **auf der Seite Azure-Ausgaben** unter **Kunden Microsoft Azure** Abonnements die Kunden aus, deren Budget Sie entfernen möchten.</span><span class="sxs-lookup"><span data-stu-id="dac8f-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="dac8f-142">Wählen Sie **Budget entfernen aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="dac8f-143">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="dac8f-143">Check current Azure spending</span></span>

<span data-ttu-id="dac8f-144">Sie können *die aktuellen Azure-Ausgaben und monatlichen* Budgets Ihrer Kunden jederzeit nachverfolgen:</span><span class="sxs-lookup"><span data-stu-id="dac8f-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="dac8f-145">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="dac8f-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dac8f-146">Wählen Sie im linken Menü unter **CSP** die Option **Azure-Ausgaben aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dac8f-147">Auf der **Seite Azure-Ausgaben** finden Sie unter **Kunden mit Microsoft Azure Abonnements** eine Übersicht über die monatlichen Budgets der Kunden, aktuelle Ausgabenschätzungen und den Prozentsatz des verwendeten Budgets.</span><span class="sxs-lookup"><span data-stu-id="dac8f-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="dac8f-148">Benachrichtigungen zu Budgetlimits</span><span class="sxs-lookup"><span data-stu-id="dac8f-148">Notifications for budget limits</span></span>

<span data-ttu-id="dac8f-149">Sie können *E-Mail-Benachrichtigungen aktivieren,* wenn sich die monatlichen Ausgaben Ihres Kunden dem Budgetlimit nähern.</span><span class="sxs-lookup"><span data-stu-id="dac8f-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="dac8f-150">Wenn Sie diese Option aktivieren, werden Sie benachrichtigt, wenn Kunden 80 % oder mehr ihres monatlichen Budgets verwenden.</span><span class="sxs-lookup"><span data-stu-id="dac8f-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="dac8f-151">Mit dieser Option können Sie Ihre Azure-Rechnung im Auge behalten.</span><span class="sxs-lookup"><span data-stu-id="dac8f-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="dac8f-152">So konfigurieren Sie E-Mail-Benachrichtigungen:</span><span class="sxs-lookup"><span data-stu-id="dac8f-152">To configure email notifications:</span></span>

1. <span data-ttu-id="dac8f-153">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="dac8f-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dac8f-154">Wechseln Sie zu **Einstellungen**.</span><span class="sxs-lookup"><span data-stu-id="dac8f-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="dac8f-155">Wählen Sie **Meine Einstellungen aus.**</span><span class="sxs-lookup"><span data-stu-id="dac8f-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="dac8f-156">Konfigurieren Sie ggf. eine bevorzugte E-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="dac8f-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="dac8f-157">Konfigurieren Sie die bevorzugte Sprache für die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="dac8f-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="dac8f-158">Wählen Sie im Abschnitt **Benachrichtigungseinstellungen** die Registerkarte **CSP** aus.</span><span class="sxs-lookup"><span data-stu-id="dac8f-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="dac8f-159">Aktivieren Sie die Option E-Mail für **Azure-Ausgabenbenachrichtigung,** und **speichern Sie**.</span><span class="sxs-lookup"><span data-stu-id="dac8f-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="dac8f-160">Aufgeschlüsselte Kosten nach Dienst</span><span class="sxs-lookup"><span data-stu-id="dac8f-160">Itemized costs by service</span></span>

<span data-ttu-id="dac8f-161">Sie können *die nach Dienst aufgeschlüsselten Kosten (und die geschätzte Nutzung) für nutzungsbasierte Abonnements anzeigen:*</span><span class="sxs-lookup"><span data-stu-id="dac8f-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="dac8f-162">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="dac8f-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dac8f-163">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="dac8f-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="dac8f-164">Wählen Sie auf der Seite **Kunden** den **Unternehmensnamen** des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="dac8f-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="dac8f-165">Wählen Sie auf der Seite **Abonnements** des Kunden unter **Nutzungsbasierte Abonnements** den Namen des **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="dac8f-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="dac8f-166">Auf der Seite des Abonnements können Sie die **Artikelkosten** nach Dienst und die **geschätzte Nutzung** für den aktuellen Monat überprüfen.</span><span class="sxs-lookup"><span data-stu-id="dac8f-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="dac8f-167">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="dac8f-167">Next steps</span></span>

- [<span data-ttu-id="dac8f-168">Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="dac8f-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
