---
title: "Einrichten eines Kundenbudgets für Azure-Kosten | Partner Center"
description: "In Partner Center können Sie für jeden Kunden ein monatliches Budget festlegen, sodass die Azure-Rechnung am Monatsende nicht zu einer Überraschung wird."
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.openlocfilehash: 5e6b34031f9bdd5a3532a7f1a8b862a4f0618ad7
ms.sourcegitcommit: b64a8977e92673cd00f776379be6cb78c4ebd1f1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2018
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="16c25-103">Einrichten eines Kundenbudgets für Azure-Kosten</span><span class="sxs-lookup"><span data-stu-id="16c25-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="16c25-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="16c25-104">Applies to</span></span>**

-  <span data-ttu-id="16c25-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="16c25-105">Partner Center</span></span>
-  <span data-ttu-id="16c25-106">Partner Center für Microsoft Cloud für US-Behörden</span><span class="sxs-lookup"><span data-stu-id="16c25-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="16c25-107">Partner Center für Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="16c25-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="16c25-108">Um Kunden bei der Verwaltung der Azure-Kosten behilflich zu sein, können Sie ein monatliches Budget festlegen, damit die Azure-Rechnung nicht höher, als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="16c25-108">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="16c25-109">Das Festlegen eines Kundenbudgets für Azure-Kosten ermöglicht Ihnen, die Azure-Kosten Ihres Kunden mit dem monatlichen Budget zu vergleichen.</span><span class="sxs-lookup"><span data-stu-id="16c25-109">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="16c25-110">Diese Funktion bietet folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="16c25-110">With this feature, you can:</span></span> 

-   <span data-ttu-id="16c25-111">Benachrichtigung per E-Mail, wenn die Ausgaben des Kunden das Budgetlimit erreichen</span><span class="sxs-lookup"><span data-stu-id="16c25-111">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="16c25-112">Überprüfen der geschätzten Azure-Kosten des Kunden pro Monat</span><span class="sxs-lookup"><span data-stu-id="16c25-112">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="16c25-113">Ermitteln eines falsch konfigurierten Service oder eines ungewöhnlichen Nutzungstrends, der auf Betrug hinweisen könnten</span><span class="sxs-lookup"><span data-stu-id="16c25-113">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="16c25-114">Zusammenarbeit mit dem Kunden, um das Grundproblem zu identifizieren und die Kosten zu verwalten</span><span class="sxs-lookup"><span data-stu-id="16c25-114">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="16c25-115">Budgeterhöhung, wenn Sie und der Kunde einverstanden sind</span><span class="sxs-lookup"><span data-stu-id="16c25-115">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="16c25-116">Die Azure-Ausgaben sind nur ein Schätzwert, die aktuellen Abrechnungsbeträge können variieren, und der Betrag enthält keine Steuern, Gutschriften, Korrekturen oder andere Gebühren, die auftreten können.</span><span class="sxs-lookup"><span data-stu-id="16c25-116">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="16c25-117">Die Ausgaben werden einmal pro Tag aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="16c25-117">Spending data is refreshed once per day.</span></span> <span data-ttu-id="16c25-118">Ihre Kunden können Azure-Dienste und -Ressourcen weiterhin nutzen und diese in Rechnung stellen, solange Sie die Kontoeinstellungen im Azure-Portal nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="16c25-118">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

><span data-ttu-id="16c25-119">**Hinweis:**   Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="16c25-119">**Note**   This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="16c25-120">Aktivieren von E-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="16c25-120">Turn on email notifications</span></span>**
1.  <span data-ttu-id="16c25-121">Wählen Sie im Dashboardmenü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="16c25-121">From the Dashboard menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="16c25-122">Aktivieren Sie die Option **E-Mails erhalten**, um sich benachrichtigen zu lassen, wenn Ihre Kunden mindestens 80 % ihres Budgets aufgebraucht haben.</span><span class="sxs-lookup"><span data-stu-id="16c25-122">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="16c25-123">Dadurch behalten Sie Ihre Azure-Rechnung im Blick.</span><span class="sxs-lookup"><span data-stu-id="16c25-123">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="16c25-124">Sie können die standardmäßige E-Mail-Adresse für den Empfang von Benachrichtigungen in eine persönliche oder beliebige andere E-Mail-Adresse ändern.</span><span class="sxs-lookup"><span data-stu-id="16c25-124">You can change the default email address to a personal or any other email to receive notifications.</span></span>

**<span data-ttu-id="16c25-125">Festlegen eines Budgets</span><span class="sxs-lookup"><span data-stu-id="16c25-125">Set a budget</span></span>**
1.  <span data-ttu-id="16c25-126">Wählen Sie im Dashboardmenü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="16c25-126">From the Dashboard menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="16c25-127">Wählen Sie die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="16c25-127">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="16c25-128">Geben Sie einen Wert im Feld **Monatsbudget** ein, und wählen Sie dann **Übernehmen**.</span><span class="sxs-lookup"><span data-stu-id="16c25-128">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="16c25-129">Zum Überprüfen der aktuellen Ausgaben kehren Sie zu dieser Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="16c25-129">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="16c25-130">Ein Budget kann auch auf der Verwaltungsseite für einen Kunden unter **Usage-based subscriptions** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="16c25-130">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

**<span data-ttu-id="16c25-131">Entfernen eines Budgets</span><span class="sxs-lookup"><span data-stu-id="16c25-131">Remove a budget</span></span>**
1.  <span data-ttu-id="16c25-132">Wählen Sie im Dashboardmenü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="16c25-132">From the Dashboard menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="16c25-133">Wählen Sie Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="16c25-133">Select customers from the list.</span></span>
3.  <span data-ttu-id="16c25-134">Wählen Sie **Remove budget**.</span><span class="sxs-lookup"><span data-stu-id="16c25-134">Select **Remove budget**.</span></span>

**<span data-ttu-id="16c25-135">Detaillierte Kosten anzeigen</span><span class="sxs-lookup"><span data-stu-id="16c25-135">See itemized costs</span></span>**
1.  <span data-ttu-id="16c25-136">Wählen Sie im Menü „Dashboard“ die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="16c25-136">From the Dashboard menu, select **Customers**.</span></span>
2.  <span data-ttu-id="16c25-137">Wählen Sie einen Kunden aus der Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="16c25-137">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="16c25-138">Wählen Sie auf der Kundenverwaltungsseite unter **Usage-based subscriptions** ein Abonnement aus.</span><span class="sxs-lookup"><span data-stu-id="16c25-138">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="16c25-139">Die aktuelle geschätzte Verwendung und eine Liste der Einzelkosten pro Dienst werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="16c25-139">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



