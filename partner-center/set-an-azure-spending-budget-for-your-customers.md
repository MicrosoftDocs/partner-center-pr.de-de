---
title: Festlegen eines Azure-Ausgabenbudgets für Kunden
ms.topic: article
ms.date: 06/03/2020
description: Erfahren Sie, wie Sie ein monatliches Azure-Ausgabenbudget für Ihre Kunden einrichten oder entfernen und wie Sie Azure-Ausgaben Daten anzeigen und Budget bezogene Benachrichtigungen festlegen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17b6186d7e6cddaf598dc663c70841275c0db853
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425989"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="f20d7-103">Festlegen, überprüfen oder Entfernen eines monatlichen Azure-Ausgabenbudgets für Kunden im Partner Center</span><span class="sxs-lookup"><span data-stu-id="f20d7-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="f20d7-104">Gilt für:</span><span class="sxs-lookup"><span data-stu-id="f20d7-104">Applies to:</span></span>

- <span data-ttu-id="f20d7-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="f20d7-105">Partner Center</span></span>
- <span data-ttu-id="f20d7-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f20d7-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f20d7-107">Sie können [ein monatliches Azure-Ausgabenbudget für Ihre Kunden](#set-azure-spending-budget) im Partner Center festlegen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="f20d7-108">Dadurch können Ihre Kunden ihre Azure-Ausgaben verwalten.</span><span class="sxs-lookup"><span data-stu-id="f20d7-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="f20d7-109">Mit dieser Option können Sie die Azure-Ausgaben ihrer Kunden mit dem Budget innerhalb des Monats vergleichen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="f20d7-110">Außerdem hilft es Ihren Kunden, ihre Azure-Ausgaben zu berechnen, sodass Ihre monatliche Rechnung nicht höher als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="f20d7-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="f20d7-111">Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f20d7-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="f20d7-112">Nachdem Sie [ein Azure-Ausgabenbudget für Ihre Kunden festgelegt](#set-azure-spending-budget)haben, können Sie die Kundennutzung auf folgende Weise überprüfen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="f20d7-113">Mithilfe dieser Optionen können Sie falsch konfigurierte Dienste oder ungewöhnliche Trends erkennen, die möglicherweise einen Betrugsversuch vorschlagen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="f20d7-114">Sie können dann mit ihren Kunden zusammenarbeiten, um die Ursache zu ermitteln und die Kosten zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="f20d7-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="f20d7-115">Falls erforderlich, können Sie auch [das Budget des Kunden](#set-azure-spending-budget) in einen höheren Betrag ändern.</span><span class="sxs-lookup"><span data-stu-id="f20d7-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="f20d7-116">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="f20d7-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="f20d7-117">E-Mail-Benachrichtigungen aktivieren, wenn die Ausgaben eines Kunden dem Budget Limit nähern</span><span class="sxs-lookup"><span data-stu-id="f20d7-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="f20d7-118">Anzeigen der aufgelisteten Kosten nach Dienst für nutzungsbasierte Abonnements</span><span class="sxs-lookup"><span data-stu-id="f20d7-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="f20d7-119">Sie können auch [ein Azure-Ausgabenbudget](#remove-azure-spending-budget) für Kunden jederzeit entfernen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="f20d7-120">Azure-Ausgaben Daten</span><span class="sxs-lookup"><span data-stu-id="f20d7-120">Azure spending data</span></span>

<span data-ttu-id="f20d7-121">Die Azure-Ausgaben Daten sind *geschätzt* , und die *tatsächlichen Abrechnungs Beträge können variieren*.</span><span class="sxs-lookup"><span data-stu-id="f20d7-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="f20d7-122">Der Wert der Daten *spiegelt nicht* die Steuern, Gutschriften, Anpassungen oder andere Gebühren wider, die anfallen können.</span><span class="sxs-lookup"><span data-stu-id="f20d7-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="f20d7-123">Die Ausgaben Daten werden *einmal täglich aktualisiert*.</span><span class="sxs-lookup"><span data-stu-id="f20d7-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="f20d7-124">Ihre Kunden können weiterhin Azure-Dienste und-Ressourcen nutzen (und dafür in Rechnung gestellt werden), es sei denn, Sie ändern die Kontoeinstellungen in der Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="f20d7-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="f20d7-125">Festlegen des Azure-Ausgabenbudgets</span><span class="sxs-lookup"><span data-stu-id="f20d7-125">Set Azure spending budget</span></span>

<span data-ttu-id="f20d7-126">Sie können *ein monatliches Azure-Ausgabenbudget* für mehrere Kunden im Partner Center festlegen:</span><span class="sxs-lookup"><span data-stu-id="f20d7-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="f20d7-127">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an.</span><span class="sxs-lookup"><span data-stu-id="f20d7-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f20d7-128">Wählen Sie im Menü auf der linken Seite unter **CSP**die Option **Azure-Ausgaben**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f20d7-129">Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements**die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="f20d7-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="f20d7-130">Geben Sie einen Wert für **monatliches Budget**ein.</span><span class="sxs-lookup"><span data-stu-id="f20d7-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="f20d7-131">Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.</span><span class="sxs-lookup"><span data-stu-id="f20d7-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="f20d7-132">Sie können auch *ein Budget für einen einzelnen Kunden* in seinen Abonnement Einstellungen festlegen:</span><span class="sxs-lookup"><span data-stu-id="f20d7-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="f20d7-133">Melden Sie sich beim Partner Center-Dashboard an.</span><span class="sxs-lookup"><span data-stu-id="f20d7-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="f20d7-134">Wählen Sie im Menü auf der linken Seite unter **CSP**die Option **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="f20d7-135">Wählen Sie auf der Seite **Kunden** den **Firmennamen**des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="f20d7-136">Wählen Sie auf der Seite **Abonnements** des Kunden unter **Nutzungs basiertes Abonnement**die Option **Budget ändern**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="f20d7-137">Geben Sie einen Wert für das Budget ein.</span><span class="sxs-lookup"><span data-stu-id="f20d7-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="f20d7-138">Wählen Sie übernehmen aus, **um die Änderungen** zu speichern.</span><span class="sxs-lookup"><span data-stu-id="f20d7-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="f20d7-139">Azure-Ausgabenbudget entfernen</span><span class="sxs-lookup"><span data-stu-id="f20d7-139">Remove Azure spending budget</span></span>

<span data-ttu-id="f20d7-140">Sie können *ein monatliches Azure-Ausgabenbudget* für Ihre Kunden im Partner Center entfernen:</span><span class="sxs-lookup"><span data-stu-id="f20d7-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="f20d7-141">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an.</span><span class="sxs-lookup"><span data-stu-id="f20d7-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f20d7-142">Wählen Sie im Menü auf der linken Seite unter **CSP**die Option **Azure-Ausgaben**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f20d7-143">Wählen Sie auf der Seite **Azure-Ausgaben** unter **Kunden mit Microsoft Azure Abonnements**die Kunden aus, deren Budget Sie entfernen möchten.</span><span class="sxs-lookup"><span data-stu-id="f20d7-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="f20d7-144">Wählen Sie **Budget entfernen**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="f20d7-145">Überprüfen der aktuellen Azure-Ausgaben</span><span class="sxs-lookup"><span data-stu-id="f20d7-145">Check current Azure spending</span></span>

<span data-ttu-id="f20d7-146">Sie können *die aktuellen Azure-Ausgaben und monatlichen Budgets von Kunden* jederzeit nachverfolgen:</span><span class="sxs-lookup"><span data-stu-id="f20d7-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="f20d7-147">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/)an.</span><span class="sxs-lookup"><span data-stu-id="f20d7-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f20d7-148">Wählen Sie im Menü auf der linken Seite unter **CSP**die Option **Azure-Ausgaben**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f20d7-149">Auf der **Azure-Ausgaben** Seite unter **Kunden mit Microsoft Azure-Abonnements**können Sie eine Übersicht über die monatlichen Budgets von Kunden, die aktuellen Ausgabenschätzungen und den Prozentsatz des verwendeten Budgets anzeigen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="f20d7-150">Benachrichtigungen für Budget Limits</span><span class="sxs-lookup"><span data-stu-id="f20d7-150">Notifications for budget limits</span></span>

<span data-ttu-id="f20d7-151">Sie können *e-Mail-Benachrichtigungen* aktivieren, wenn die monatlichen Ausgaben Ihres Kunden dem Budget Limit nähern.</span><span class="sxs-lookup"><span data-stu-id="f20d7-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="f20d7-152">Wenn Sie diese Option aktivieren, werden Sie benachrichtigt, wenn Kunden mindestens 80% Ihres monatlichen Budgets verwenden.</span><span class="sxs-lookup"><span data-stu-id="f20d7-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="f20d7-153">Mit dieser Option können Sie Ihre Azure-Rechnung überwachen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="f20d7-154">So konfigurieren Sie e-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="f20d7-154">To configure email notifications:</span></span>

1. <span data-ttu-id="f20d7-155">Melden Sie sich beim Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="f20d7-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="f20d7-156">Wählen Sie im Menü auf der linken Seite unter **CSP**die Option **Azure-Ausgaben**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f20d7-157">Schalten **Sie auf** der Seite Azure- **Ausgaben** unter **e-Mail-Benachrichtigungen die Einstellung e-Mail-** Adressen **aktivieren auf ein.**</span><span class="sxs-lookup"><span data-stu-id="f20d7-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>

4. <span data-ttu-id="f20d7-158">Wählen Sie **e-Mail-Adresse ändern** , um die e-Mail-Adresse für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="f20d7-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="f20d7-159">Wenn die e-Mail-Adresse *nicht korrekt*ist, **Geben Sie die**richtige e-Mail-Adresse ein</span><span class="sxs-lookup"><span data-stu-id="f20d7-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="f20d7-160">Wenn die e-Mail-Adresse *richtig ist*, wählen Sie **Abbrechen**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="f20d7-161">Itemisierte Kosten nach Dienst</span><span class="sxs-lookup"><span data-stu-id="f20d7-161">Itemized costs by service</span></span>

<span data-ttu-id="f20d7-162">Sie können die *aufgelisteten Kosten (und die geschätzte Nutzung) nach Dienst für nutzungsbasierte Abonnements anzeigen*:</span><span class="sxs-lookup"><span data-stu-id="f20d7-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="f20d7-163">Melden Sie sich beim Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="f20d7-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="f20d7-164">Wählen Sie im Menü auf der linken Seite unter **CSP**die Option **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="f20d7-165">Wählen Sie auf der Seite **Kunden** den **Firmennamen**des Kunden aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="f20d7-166">Wählen Sie auf der Seite **Abonnements** des Kunden unter **nutzungsbasierte Abonnements**den Namen des **Abonnements**aus.</span><span class="sxs-lookup"><span data-stu-id="f20d7-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="f20d7-167">Auf der Seite des Abonnements können Sie die **aufgelisteten Kosten** nach Dienst und die **geschätzte Nutzung** des aktuellen Monats überprüfen.</span><span class="sxs-lookup"><span data-stu-id="f20d7-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
