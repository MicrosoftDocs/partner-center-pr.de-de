---
title: Einrichten eines Kundenbudgets für Azure-Kosten | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Set a monthly budget per customer in Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 05212746e1ccbcc5081c68ca97ced6a99e20bb8c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384889"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="5402d-103">Einrichten eines Kundenbudgets für Azure-Kosten</span><span class="sxs-lookup"><span data-stu-id="5402d-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="5402d-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="5402d-104">Applies to:</span></span>

- <span data-ttu-id="5402d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="5402d-105">Partner Center</span></span>
- <span data-ttu-id="5402d-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="5402d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="5402d-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5402d-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="5402d-108">This helps your customers manage their Azure spending.</span><span class="sxs-lookup"><span data-stu-id="5402d-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="5402d-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span><span class="sxs-lookup"><span data-stu-id="5402d-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="5402d-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span><span class="sxs-lookup"><span data-stu-id="5402d-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>


> [!NOTE]  
> <span data-ttu-id="5402d-111">Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5402d-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="5402d-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span><span class="sxs-lookup"><span data-stu-id="5402d-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="5402d-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span><span class="sxs-lookup"><span data-stu-id="5402d-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="5402d-114">You can then work with your customer(s) to identify the root cause and manage costs.</span><span class="sxs-lookup"><span data-stu-id="5402d-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="5402d-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span><span class="sxs-lookup"><span data-stu-id="5402d-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="5402d-116">Check current Azure spending</span><span class="sxs-lookup"><span data-stu-id="5402d-116">Check current Azure spending</span></span>](#check-current-azure-spending)
- [<span data-ttu-id="5402d-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span><span class="sxs-lookup"><span data-stu-id="5402d-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)
- [<span data-ttu-id="5402d-118">View itemized costs by service for usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="5402d-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="5402d-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span><span class="sxs-lookup"><span data-stu-id="5402d-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="5402d-120">Azure spending data</span><span class="sxs-lookup"><span data-stu-id="5402d-120">Azure spending data</span></span>

<span data-ttu-id="5402d-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span><span class="sxs-lookup"><span data-stu-id="5402d-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="5402d-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span><span class="sxs-lookup"><span data-stu-id="5402d-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="5402d-123">The spending data is *refreshed once per day*.</span><span class="sxs-lookup"><span data-stu-id="5402d-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="5402d-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="5402d-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="5402d-125">Set Azure spending budget</span><span class="sxs-lookup"><span data-stu-id="5402d-125">Set Azure spending budget</span></span>

<span data-ttu-id="5402d-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="5402d-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="5402d-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5402d-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5402d-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="5402d-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="5402d-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span><span class="sxs-lookup"><span data-stu-id="5402d-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>
4. <span data-ttu-id="5402d-130">Enter a value for **Monthly budget**.</span><span class="sxs-lookup"><span data-stu-id="5402d-130">Enter a value for **Monthly budget**.</span></span>
5. <span data-ttu-id="5402d-131">Choose **Apply** to save your changes.</span><span class="sxs-lookup"><span data-stu-id="5402d-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="5402d-132">You can also *set a budget for an individual customer* in their subscription settings:</span><span class="sxs-lookup"><span data-stu-id="5402d-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="5402d-133">Sign in to the Partner Center dashboard.</span><span class="sxs-lookup"><span data-stu-id="5402d-133">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="5402d-134">In the left-hand menu under **CSP**, choose **Customers**.</span><span class="sxs-lookup"><span data-stu-id="5402d-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="5402d-135">On the **Customers** page, select the customer's **Company name**.</span><span class="sxs-lookup"><span data-stu-id="5402d-135">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="5402d-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span><span class="sxs-lookup"><span data-stu-id="5402d-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>
5. <span data-ttu-id="5402d-137">Enter a value for the budget.</span><span class="sxs-lookup"><span data-stu-id="5402d-137">Enter a value for the budget.</span></span>
6. <span data-ttu-id="5402d-138">Choose **Apply** to save your changes.</span><span class="sxs-lookup"><span data-stu-id="5402d-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="5402d-139">Remove Azure spending budget</span><span class="sxs-lookup"><span data-stu-id="5402d-139">Remove Azure spending budget</span></span>

<span data-ttu-id="5402d-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="5402d-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="5402d-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5402d-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5402d-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="5402d-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="5402d-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span><span class="sxs-lookup"><span data-stu-id="5402d-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>
4. <span data-ttu-id="5402d-144">Choose **Remove budget**.</span><span class="sxs-lookup"><span data-stu-id="5402d-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="5402d-145">Check current Azure spending</span><span class="sxs-lookup"><span data-stu-id="5402d-145">Check current Azure spending</span></span>

<span data-ttu-id="5402d-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span><span class="sxs-lookup"><span data-stu-id="5402d-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="5402d-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5402d-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5402d-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="5402d-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="5402d-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span><span class="sxs-lookup"><span data-stu-id="5402d-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="5402d-150">Notifications for budget limits</span><span class="sxs-lookup"><span data-stu-id="5402d-150">Notifications for budget limits</span></span>

<span data-ttu-id="5402d-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span><span class="sxs-lookup"><span data-stu-id="5402d-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="5402d-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span><span class="sxs-lookup"><span data-stu-id="5402d-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="5402d-153">This option helps you can keep an eye on your Azure bill.</span><span class="sxs-lookup"><span data-stu-id="5402d-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="5402d-154">To configure email notifications:</span><span class="sxs-lookup"><span data-stu-id="5402d-154">To configure email notifications:</span></span>

1. <span data-ttu-id="5402d-155">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="5402d-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="5402d-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="5402d-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="5402d-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span><span class="sxs-lookup"><span data-stu-id="5402d-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>
4. <span data-ttu-id="5402d-158">Choose **Change email address** to see the email address for notifications.</span><span class="sxs-lookup"><span data-stu-id="5402d-158">Choose **Change email address** to see the email address for notifications.</span></span>
5. <span data-ttu-id="5402d-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span><span class="sxs-lookup"><span data-stu-id="5402d-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="5402d-160">If the email address *is correct*, choose **Cancel**.</span><span class="sxs-lookup"><span data-stu-id="5402d-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="5402d-161">Itemized costs by service</span><span class="sxs-lookup"><span data-stu-id="5402d-161">Itemized costs by service</span></span>

<span data-ttu-id="5402d-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span><span class="sxs-lookup"><span data-stu-id="5402d-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="5402d-163">Melden Sie sich bei Partner Center an.</span><span class="sxs-lookup"><span data-stu-id="5402d-163">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="5402d-164">In the left-hand menu under **CSP**, choose **Customers**.</span><span class="sxs-lookup"><span data-stu-id="5402d-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="5402d-165">On the **Customers** page, select the customer's **Company name**.</span><span class="sxs-lookup"><span data-stu-id="5402d-165">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="5402d-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span><span class="sxs-lookup"><span data-stu-id="5402d-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>
5. <span data-ttu-id="5402d-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span><span class="sxs-lookup"><span data-stu-id="5402d-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
