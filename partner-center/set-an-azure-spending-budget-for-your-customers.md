---
title: Einrichten eines Kundenbudgets für Azure-Kosten | Partner Center
description: In Partner Center können Sie für jeden Kunden ein monatliches Budget festlegen, sodass die Azure-Rechnung am Monatsende nicht zu einer Überraschung wird.
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 7e7fd895c3c8e0acda51fb79ab142a7723ecb227
ms.sourcegitcommit: 5b720c2ad126ec52564ad5264596ca1cf6a12489
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/05/2018
ms.locfileid: "4377472"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="c3468-103">Einrichten eines Kundenbudgets für Azure-Kosten</span><span class="sxs-lookup"><span data-stu-id="c3468-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="c3468-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="c3468-104">Applies to</span></span>**

-  <span data-ttu-id="c3468-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c3468-105">Partner Center</span></span>
-  <span data-ttu-id="c3468-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c3468-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="c3468-107">Partner Center für Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="c3468-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="c3468-108">Um Kunden bei der Verwaltung der Azure-Kosten behilflich zu sein, können Sie ein monatliches Budget festlegen, damit die Azure-Rechnung nicht höher, als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="c3468-108">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="c3468-109">Das Festlegen eines Kundenbudgets für Azure-Kosten ermöglicht Ihnen, die Azure-Kosten Ihres Kunden mit dem monatlichen Budget zu vergleichen.</span><span class="sxs-lookup"><span data-stu-id="c3468-109">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="c3468-110">Diese Funktion bietet folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="c3468-110">With this feature, you can:</span></span> 

-   <span data-ttu-id="c3468-111">Benachrichtigung per E-Mail, wenn die Ausgaben des Kunden das Budgetlimit erreichen</span><span class="sxs-lookup"><span data-stu-id="c3468-111">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="c3468-112">Überprüfen der geschätzten Azure-Kosten des Kunden pro Monat</span><span class="sxs-lookup"><span data-stu-id="c3468-112">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="c3468-113">Ermitteln eines falsch konfigurierten Service oder eines ungewöhnlichen Nutzungstrends, der auf Betrug hinweisen könnten</span><span class="sxs-lookup"><span data-stu-id="c3468-113">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="c3468-114">Zusammenarbeit mit dem Kunden, um das Grundproblem zu identifizieren und die Kosten zu verwalten</span><span class="sxs-lookup"><span data-stu-id="c3468-114">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="c3468-115">Budgeterhöhung, wenn Sie und der Kunde einverstanden sind</span><span class="sxs-lookup"><span data-stu-id="c3468-115">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="c3468-116">Die Azure-Ausgaben sind nur ein Schätzwert, die aktuellen Abrechnungsbeträge können variieren, und der Betrag enthält keine Steuern, Gutschriften, Korrekturen oder andere Gebühren, die auftreten können.</span><span class="sxs-lookup"><span data-stu-id="c3468-116">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="c3468-117">Die Ausgaben werden einmal pro Tag aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c3468-117">Spending data is refreshed once per day.</span></span> <span data-ttu-id="c3468-118">Ihre Kunden können Azure-Dienste und -Ressourcen weiterhin nutzen und diese in Rechnung stellen, solange Sie die Kontoeinstellungen im Azure-Portal nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="c3468-118">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="c3468-119">Dieses Feature ist nicht in Sandbox oder Test in Production (TIP) Konten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c3468-119">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="c3468-120">Aktivieren von E-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="c3468-120">Turn on email notifications</span></span>**
1.  <span data-ttu-id="c3468-121">Wählen Sie im Dashboardmenü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="c3468-121">From the Dashboard menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="c3468-122">Aktivieren Sie die Option **E-Mails erhalten**, um sich benachrichtigen zu lassen, wenn Ihre Kunden mindestens 80 % ihres Budgets aufgebraucht haben.</span><span class="sxs-lookup"><span data-stu-id="c3468-122">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="c3468-123">Dadurch behalten Sie Ihre Azure-Rechnung im Blick.</span><span class="sxs-lookup"><span data-stu-id="c3468-123">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="c3468-124">Sie können die standardmäßige E-Mail-Adresse für den Empfang von Benachrichtigungen in eine persönliche oder beliebige andere E-Mail-Adresse ändern.</span><span class="sxs-lookup"><span data-stu-id="c3468-124">You can change the default email address to a personal or any other email to receive notifications.</span></span>

**<span data-ttu-id="c3468-125">Festlegen eines Budgets</span><span class="sxs-lookup"><span data-stu-id="c3468-125">Set a budget</span></span>**
1.  <span data-ttu-id="c3468-126">Wählen Sie im Dashboardmenü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="c3468-126">From the Dashboard menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="c3468-127">Wählen Sie die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="c3468-127">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="c3468-128">Geben Sie einen Wert im Feld **Monatsbudget** ein, und wählen Sie dann **Übernehmen**.</span><span class="sxs-lookup"><span data-stu-id="c3468-128">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="c3468-129">Zum Überprüfen der aktuellen Ausgaben kehren Sie zu dieser Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="c3468-129">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="c3468-130">Ein Budget kann auch auf der Verwaltungsseite für einen Kunden unter **Usage-based subscriptions** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c3468-130">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

**<span data-ttu-id="c3468-131">Entfernen eines Budgets</span><span class="sxs-lookup"><span data-stu-id="c3468-131">Remove a budget</span></span>**
1.  <span data-ttu-id="c3468-132">Wählen Sie im Dashboardmenü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="c3468-132">From the Dashboard menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="c3468-133">Wählen Sie Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="c3468-133">Select customers from the list.</span></span>
3.  <span data-ttu-id="c3468-134">Wählen Sie **Remove budget**.</span><span class="sxs-lookup"><span data-stu-id="c3468-134">Select **Remove budget**.</span></span>

**<span data-ttu-id="c3468-135">Detaillierte Kosten anzeigen</span><span class="sxs-lookup"><span data-stu-id="c3468-135">See itemized costs</span></span>**
1.  <span data-ttu-id="c3468-136">Wählen Sie im Menü „Dashboard“ die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="c3468-136">From the Dashboard menu, select **Customers**.</span></span>
2.  <span data-ttu-id="c3468-137">Wählen Sie einen Kunden aus der Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="c3468-137">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="c3468-138">Wählen Sie auf der Kundenverwaltungsseite unter **Usage-based subscriptions** ein Abonnement aus.</span><span class="sxs-lookup"><span data-stu-id="c3468-138">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="c3468-139">Die aktuelle geschätzte Verwendung und eine Liste der Einzelkosten pro Dienst werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c3468-139">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



