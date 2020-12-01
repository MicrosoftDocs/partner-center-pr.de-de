---
title: Festlegen eines Azure-Ausgabenbudgets für Kunden
ms.topic: how-to
ms.date: 06/03/2020
description: Erfahren Sie, wie Sie ein monatliches Azure-Ausgabenbudget für Ihre Kunden einrichten oder entfernen und wie Sie Azure-Ausgaben Daten anzeigen und Budget bezogene Benachrichtigungen festlegen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438983"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="1297e-103">Festlegen, überprüfen oder Entfernen eines monatlichen Azure-Ausgabenbudgets für Kunden im Partner Center</span><span class="sxs-lookup"><span data-stu-id="1297e-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="1297e-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="1297e-104">Applies to:</span></span>

- <span data-ttu-id="1297e-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="1297e-105">Partner Center</span></span>
- <span data-ttu-id="1297e-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="1297e-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="1297e-107">Sie können [ein monatliches Azure-Ausgabenbudget für Ihre Kunden](#set-azure-spending-budget) im Partner Center festlegen.</span><span class="sxs-lookup"><span data-stu-id="1297e-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="1297e-108">Dadurch können Ihre Kunden ihre Azure-Ausgaben verwalten.</span><span class="sxs-lookup"><span data-stu-id="1297e-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="1297e-109">Mit dieser Option können Sie die Azure-Ausgaben ihrer Kunden mit dem Budget innerhalb des Monats vergleichen.</span><span class="sxs-lookup"><span data-stu-id="1297e-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="1297e-110">Außerdem hilft es Ihren Kunden, ihre Azure-Ausgaben zu berechnen, sodass Ihre monatliche Rechnung nicht höher als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="1297e-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="1297e-111">Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1297e-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="1297e-112">Nachdem Sie [ein Azure-Ausgabenbudget für Ihre Kunden festgelegt](#set-azure-spending-budget)haben, können Sie die Kundennutzung auf folgende Weise überprüfen.</span><span class="sxs-lookup"><span data-stu-id="1297e-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="1297e-113">Mithilfe dieser Optionen können Sie falsch konfigurierte Dienste oder ungewöhnliche Trends erkennen, die möglicherweise einen Betrugsversuch vorschlagen.</span><span class="sxs-lookup"><span data-stu-id="1297e-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="1297e-114">Sie können dann mit ihren Kunden zusammenarbeiten, um die Ursache zu ermitteln und die Kosten zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="1297e-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="1297e-115">Falls erforderlich, können Sie auch [das Budget des Kunden](#set-azure-spending-budget) in einen höheren Betrag ändern.</span><span class="sxs-lookup"><span data-stu-id="1297e-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="1297e-116">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="1297e-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="1297e-117">E-Mail-Benachrichtigungen aktivieren, wenn die Ausgaben eines Kunden dem Budget Limit nähern</span><span class="sxs-lookup"><span data-stu-id="1297e-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="1297e-118">Anzeigen der aufgelisteten Kosten nach Dienst für nutzungsbasierte Abonnements</span><span class="sxs-lookup"><span data-stu-id="1297e-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="1297e-119">Sie können auch [ein Azure-Ausgabenbudget](#remove-azure-spending-budget) für Kunden jederzeit entfernen.</span><span class="sxs-lookup"><span data-stu-id="1297e-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="1297e-120">Azure-Ausgaben Daten</span><span class="sxs-lookup"><span data-stu-id="1297e-120">Azure spending data</span></span>

<span data-ttu-id="1297e-121">Die Azure-Ausgaben Daten sind *geschätzt* , und die *tatsächlichen Abrechnungs Beträge können variieren*.</span><span class="sxs-lookup"><span data-stu-id="1297e-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="1297e-122">Der Wert der Daten *spiegelt nicht* die Steuern, Gutschriften, Anpassungen oder andere Gebühren wider, die anfallen können.</span><span class="sxs-lookup"><span data-stu-id="1297e-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="1297e-123">Die Ausgaben Daten werden *einmal täglich aktualisiert*.</span><span class="sxs-lookup"><span data-stu-id="1297e-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="1297e-124">Ihre Kunden können weiterhin Azure-Dienste und-Ressourcen nutzen (und dafür in Rechnung gestellt werden), es sei denn, Sie ändern die Kontoeinstellungen in der Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="1297e-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="1297e-125">Festlegen des Azure-Ausgabenbudgets</span><span class="sxs-lookup"><span data-stu-id="1297e-125">Set Azure spending budget</span></span>

<span data-ttu-id="1297e-126">Sie können *ein monatliches Azure-Ausgabenbudget* für mehrere Kunden im Partner Center festlegen:</span><span class="sxs-lookup"><span data-stu-id="1297e-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="1297e-127">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an.</span><span class="sxs-lookup"><span data-stu-id="1297e-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1297e-128">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1297e-129">Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements** die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="1297e-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="1297e-130">Geben Sie einen Wert für **monatliches Budget** ein.</span><span class="sxs-lookup"><span data-stu-id="1297e-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="1297e-131">Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.</span><span class="sxs-lookup"><span data-stu-id="1297e-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="1297e-132">Sie können auch *ein Budget für einen einzelnen Kunden* in seinen Abonnement Einstellungen festlegen:</span><span class="sxs-lookup"><span data-stu-id="1297e-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="1297e-133">Melden Sie sich beim Partner Center-Dashboard an.</span><span class="sxs-lookup"><span data-stu-id="1297e-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="1297e-134">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="1297e-135">Wählen Sie auf der Seite **Kunden** den **Firmennamen** des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="1297e-136">Wählen Sie auf der Seite **Abonnements** des Kunden unter **Nutzungs basiertes Abonnement** die Option **Budget ändern** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="1297e-137">Geben Sie einen Wert für das Budget ein.</span><span class="sxs-lookup"><span data-stu-id="1297e-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="1297e-138">Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.</span><span class="sxs-lookup"><span data-stu-id="1297e-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="1297e-139">Azure-Ausgabenbudget entfernen</span><span class="sxs-lookup"><span data-stu-id="1297e-139">Remove Azure spending budget</span></span>

<span data-ttu-id="1297e-140">Sie können *ein monatliches Azure-Ausgabenbudget* für Ihre Kunden im Partner Center entfernen:</span><span class="sxs-lookup"><span data-stu-id="1297e-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="1297e-141">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an.</span><span class="sxs-lookup"><span data-stu-id="1297e-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1297e-142">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1297e-143">Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements** die Kunden aus, deren Budget Sie entfernen möchten.</span><span class="sxs-lookup"><span data-stu-id="1297e-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="1297e-144">Wählen Sie **Budget entfernen** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="1297e-145">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="1297e-145">Check current Azure spending</span></span>

<span data-ttu-id="1297e-146">Sie können *die aktuellen Azure-Ausgaben und monatlichen Budgets von Kunden* jederzeit nachverfolgen:</span><span class="sxs-lookup"><span data-stu-id="1297e-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="1297e-147">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an.</span><span class="sxs-lookup"><span data-stu-id="1297e-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1297e-148">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1297e-149">Auf der **Azure-Ausgaben** Seite unter **Kunden mit Microsoft Azure-Abonnements** können Sie eine Übersicht über die monatlichen Budgets von Kunden, die aktuellen Ausgabenschätzungen und den Prozentsatz des verwendeten Budgets anzeigen.</span><span class="sxs-lookup"><span data-stu-id="1297e-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="1297e-150">Benachrichtigungen für Budget Limits</span><span class="sxs-lookup"><span data-stu-id="1297e-150">Notifications for budget limits</span></span>

<span data-ttu-id="1297e-151">Sie können *e-Mail-Benachrichtigungen* aktivieren, wenn die monatlichen Ausgaben Ihres Kunden dem Budget Limit nähern.</span><span class="sxs-lookup"><span data-stu-id="1297e-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="1297e-152">Wenn Sie diese Option aktivieren, werden Sie benachrichtigt, wenn Kunden mindestens 80% Ihres monatlichen Budgets verwenden.</span><span class="sxs-lookup"><span data-stu-id="1297e-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="1297e-153">Mit dieser Option können Sie Ihre Azure-Rechnung überwachen.</span><span class="sxs-lookup"><span data-stu-id="1297e-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="1297e-154">So konfigurieren Sie e-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="1297e-154">To configure email notifications:</span></span>

1. <span data-ttu-id="1297e-155">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="1297e-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1297e-156">Wechseln Sie zu **Einstellungen**.</span><span class="sxs-lookup"><span data-stu-id="1297e-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="1297e-157">Wählen Sie **meine Einstellungen** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="1297e-158">Konfigurieren Sie ggf. eine bevorzugte e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="1297e-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="1297e-159">Konfigurieren Sie die bevorzugte Sprache für die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="1297e-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="1297e-160">Wählen Sie im Abschnitt **Benachrichtigungseinstellungen** die Registerkarte **CSP** .</span><span class="sxs-lookup"><span data-stu-id="1297e-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="1297e-161">Aktivieren Sie die e-Mail-Option **Azure-Ausgaben** Benachrichtigung, und **Speichern** Sie Sie.</span><span class="sxs-lookup"><span data-stu-id="1297e-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="1297e-162">Itemisierte Kosten nach Dienst</span><span class="sxs-lookup"><span data-stu-id="1297e-162">Itemized costs by service</span></span>

<span data-ttu-id="1297e-163">Sie können die *aufgelisteten Kosten (und die geschätzte Nutzung) nach Dienst für nutzungsbasierte Abonnements anzeigen*:</span><span class="sxs-lookup"><span data-stu-id="1297e-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="1297e-164">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="1297e-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1297e-165">Wählen Sie im Menü auf der linken Seite unter **CSP** die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="1297e-166">Wählen Sie auf der Seite **Kunden** den **Firmennamen** des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="1297e-167">Wählen Sie auf der Seite **Abonnements** des Kunden unter **nutzungsbasierte Abonnements** den Namen des **Abonnements** aus.</span><span class="sxs-lookup"><span data-stu-id="1297e-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="1297e-168">Auf der Seite des Abonnements können Sie die **aufgelisteten Kosten** nach Dienst und die **geschätzte Nutzung** des aktuellen Monats überprüfen.</span><span class="sxs-lookup"><span data-stu-id="1297e-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
