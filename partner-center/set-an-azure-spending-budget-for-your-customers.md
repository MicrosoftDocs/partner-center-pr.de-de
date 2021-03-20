---
title: Festlegen eines Azure-Ausgabenbudgets für Kunden
ms.topic: how-to
ms.date: 03/17/2021
description: Erfahren Sie, wie Sie ein monatliches Azure-Ausgabenbudget für Ihre Kunden einrichten oder entfernen und wie Sie Azure-Ausgaben Daten anzeigen und Budget bezogene Benachrichtigungen festlegen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712748"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="5d1e5-103">Festlegen, überprüfen oder Entfernen eines monatlichen Azure-Ausgabenbudgets für Kunden im Partner Center</span><span class="sxs-lookup"><span data-stu-id="5d1e5-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="5d1e5-104">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="5d1e5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5d1e5-105">Administrator-Agent</span><span class="sxs-lookup"><span data-stu-id="5d1e5-105">Admin agent</span></span>

<span data-ttu-id="5d1e5-106">Sie können [ein monatliches Azure-Ausgabenbudget für Ihre Kunden](#set-azure-spending-budget) im Partner Center festlegen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="5d1e5-107">Dadurch können Ihre Kunden ihre Azure-Ausgaben verwalten.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="5d1e5-108">Mit dieser Option können Sie die Azure-Ausgaben ihrer Kunden mit dem Budget innerhalb des Monats vergleichen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="5d1e5-109">Außerdem hilft es Ihren Kunden, ihre Azure-Ausgaben zu berechnen, sodass Ihre monatliche Rechnung nicht höher als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="5d1e5-110">Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="5d1e5-111">Nachdem Sie [ein Azure-Ausgabenbudget für Ihre Kunden festgelegt](#set-azure-spending-budget)haben, können Sie die Kundennutzung auf folgende Weise überprüfen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="5d1e5-112">Mithilfe dieser Optionen können Sie falsch konfigurierte Dienste oder ungewöhnliche Trends erkennen, die möglicherweise einen Betrugsversuch vorschlagen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="5d1e5-113">Sie können dann mit ihren Kunden zusammenarbeiten, um die Ursache zu ermitteln und die Kosten zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="5d1e5-114">Falls erforderlich, können Sie auch [das Budget des Kunden](#set-azure-spending-budget) in einen höheren Betrag ändern.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="5d1e5-115">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="5d1e5-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="5d1e5-116">E-Mail-Benachrichtigungen aktivieren, wenn die Ausgaben eines Kunden dem Budget Limit nähern</span><span class="sxs-lookup"><span data-stu-id="5d1e5-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="5d1e5-117">Anzeigen der aufgelisteten Kosten nach Dienst für nutzungsbasierte Abonnements</span><span class="sxs-lookup"><span data-stu-id="5d1e5-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="5d1e5-118">Sie können auch [ein Azure-Ausgabenbudget](#remove-azure-spending-budget) für Kunden jederzeit entfernen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="5d1e5-119">Azure-Ausgaben Daten</span><span class="sxs-lookup"><span data-stu-id="5d1e5-119">Azure spending data</span></span>

<span data-ttu-id="5d1e5-120">Die Azure-Ausgaben Daten sind *geschätzt* , und die *tatsächlichen Abrechnungs Beträge können variieren*.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="5d1e5-121">Der Wert der Daten *spiegelt nicht* die Steuern, Gutschriften, Anpassungen oder andere Gebühren wider, die anfallen können.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="5d1e5-122">Die Ausgaben Daten werden *einmal täglich aktualisiert*.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="5d1e5-123">Ihre Kunden können weiterhin Azure-Dienste und-Ressourcen nutzen (und dafür in Rechnung gestellt werden), es sei denn, Sie ändern die Kontoeinstellungen in der Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="5d1e5-124">Festlegen des Azure-Ausgabenbudgets</span><span class="sxs-lookup"><span data-stu-id="5d1e5-124">Set Azure spending budget</span></span>

<span data-ttu-id="5d1e5-125">Sie können *ein monatliches Azure-Ausgabenbudget* für mehrere Kunden im Partner Center festlegen:</span><span class="sxs-lookup"><span data-stu-id="5d1e5-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="5d1e5-126">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5d1e5-127">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="5d1e5-128">Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements** die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="5d1e5-129">Geben Sie einen Wert für **monatliches Budget** ein.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="5d1e5-130">Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="5d1e5-131">Sie können auch *ein Budget für einen einzelnen Kunden* in seinen Abonnement Einstellungen festlegen:</span><span class="sxs-lookup"><span data-stu-id="5d1e5-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="5d1e5-132">Melden Sie sich beim Partner Center-Dashboard an.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="5d1e5-133">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="5d1e5-134">Wählen Sie auf der Seite **Kunden** den **Firmennamen** des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="5d1e5-135">Wählen Sie auf der Seite **Abonnements** des Kunden unter **Nutzungs basiertes Abonnement** die Option **Budget ändern** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="5d1e5-136">Geben Sie einen Wert für das Budget ein.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="5d1e5-137">Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="5d1e5-138">Azure-Ausgabenbudget entfernen</span><span class="sxs-lookup"><span data-stu-id="5d1e5-138">Remove Azure spending budget</span></span>

<span data-ttu-id="5d1e5-139">Sie können *ein monatliches Azure-Ausgabenbudget* für Ihre Kunden im Partner Center entfernen:</span><span class="sxs-lookup"><span data-stu-id="5d1e5-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="5d1e5-140">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5d1e5-141">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="5d1e5-142">Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements** die Kunden aus, deren Budget Sie entfernen möchten.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="5d1e5-143">Wählen Sie **Budget entfernen** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="5d1e5-144">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="5d1e5-144">Check current Azure spending</span></span>

<span data-ttu-id="5d1e5-145">Sie können *die aktuellen Azure-Ausgaben und monatlichen Budgets von Kunden* jederzeit nachverfolgen:</span><span class="sxs-lookup"><span data-stu-id="5d1e5-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="5d1e5-146">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5d1e5-147">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="5d1e5-148">Auf der **Azure-Ausgaben** Seite unter **Kunden mit Microsoft Azure-Abonnements** können Sie eine Übersicht über die monatlichen Budgets von Kunden, die aktuellen Ausgabenschätzungen und den Prozentsatz des verwendeten Budgets anzeigen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="5d1e5-149">Benachrichtigungen für Budget Limits</span><span class="sxs-lookup"><span data-stu-id="5d1e5-149">Notifications for budget limits</span></span>

<span data-ttu-id="5d1e5-150">Sie können *e-Mail-Benachrichtigungen* aktivieren, wenn die monatlichen Ausgaben Ihres Kunden dem Budget Limit nähern.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="5d1e5-151">Wenn Sie diese Option aktivieren, werden Sie benachrichtigt, wenn Kunden mindestens 80% Ihres monatlichen Budgets verwenden.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="5d1e5-152">Mit dieser Option können Sie Ihre Azure-Rechnung überwachen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="5d1e5-153">So konfigurieren Sie e-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="5d1e5-153">To configure email notifications:</span></span>

1. <span data-ttu-id="5d1e5-154">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="5d1e5-155">Wechseln Sie zu **Einstellungen**.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="5d1e5-156">Wählen Sie **meine Einstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="5d1e5-157">Konfigurieren Sie ggf. eine bevorzugte e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="5d1e5-158">Konfigurieren Sie die bevorzugte Sprache für die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="5d1e5-159">Wählen Sie im Abschnitt **Benachrichtigungseinstellungen** die Registerkarte **CSP** .</span><span class="sxs-lookup"><span data-stu-id="5d1e5-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="5d1e5-160">Aktivieren Sie die e-Mail-Option **Azure-Ausgaben** Benachrichtigung, und **Speichern** Sie Sie.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="5d1e5-161">Itemisierte Kosten nach Dienst</span><span class="sxs-lookup"><span data-stu-id="5d1e5-161">Itemized costs by service</span></span>

<span data-ttu-id="5d1e5-162">Sie können die *aufgelisteten Kosten (und die geschätzte Nutzung) nach Dienst für nutzungsbasierte Abonnements anzeigen*:</span><span class="sxs-lookup"><span data-stu-id="5d1e5-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="5d1e5-163">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="5d1e5-164">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="5d1e5-165">Wählen Sie auf der Seite **Kunden** den **Firmennamen** des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="5d1e5-166">Wählen Sie auf der Seite **Abonnements** des Kunden unter **nutzungsbasierte Abonnements** den Namen des **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="5d1e5-167">Auf der Seite des Abonnements können Sie die **aufgelisteten Kosten** nach Dienst und die **geschätzte Nutzung** des aktuellen Monats überprüfen.</span><span class="sxs-lookup"><span data-stu-id="5d1e5-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="5d1e5-168">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="5d1e5-168">Next steps</span></span>

- [<span data-ttu-id="5d1e5-169">Neues E-Commerce-Verfahren in CSP: Azure-Abrechnung</span><span class="sxs-lookup"><span data-stu-id="5d1e5-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
