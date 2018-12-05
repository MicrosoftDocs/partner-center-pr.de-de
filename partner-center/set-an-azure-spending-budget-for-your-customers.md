---
title: Einrichten eines Kundenbudgets für Azure-Kosten | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: In Partner Center können Sie für jeden Kunden ein monatliches Budget festlegen, sodass die Azure-Rechnung am Monatsende nicht zu einer Überraschung wird.
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 3158679d8a435a8252ad7dfb60d5cccc5cfa2f1f
ms.sourcegitcommit: d3613d23bd177a53381ebf32b4f1075201f8f7f7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/05/2018
ms.locfileid: "8683439"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="493ee-103">Einrichten eines Kundenbudgets für Azure-Kosten</span><span class="sxs-lookup"><span data-stu-id="493ee-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="493ee-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="493ee-104">Applies to</span></span>**

-  <span data-ttu-id="493ee-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="493ee-105">Partner Center</span></span>
-  <span data-ttu-id="493ee-106">Partner Center für Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="493ee-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="493ee-107">Um Kunden bei der Verwaltung der Azure-Kosten behilflich zu sein, können Sie ein monatliches Budget festlegen, damit die Azure-Rechnung nicht höher, als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="493ee-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="493ee-108">Das Festlegen eines Kundenbudgets für Azure-Kosten ermöglicht Ihnen, die Azure-Kosten Ihres Kunden mit dem monatlichen Budget zu vergleichen.</span><span class="sxs-lookup"><span data-stu-id="493ee-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="493ee-109">Diese Funktion bietet folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="493ee-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="493ee-110">Benachrichtigung per E-Mail, wenn die Ausgaben des Kunden das Budgetlimit erreichen</span><span class="sxs-lookup"><span data-stu-id="493ee-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="493ee-111">Überprüfen der geschätzten Azure-Kosten des Kunden pro Monat</span><span class="sxs-lookup"><span data-stu-id="493ee-111">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="493ee-112">Ermitteln eines falsch konfigurierten Service oder eines ungewöhnlichen Nutzungstrends, der auf Betrug hinweisen könnten</span><span class="sxs-lookup"><span data-stu-id="493ee-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="493ee-113">Zusammenarbeit mit dem Kunden, um das Grundproblem zu identifizieren und die Kosten zu verwalten</span><span class="sxs-lookup"><span data-stu-id="493ee-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="493ee-114">Budgeterhöhung, wenn Sie und der Kunde einverstanden sind</span><span class="sxs-lookup"><span data-stu-id="493ee-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="493ee-115">Die Azure-Ausgaben sind nur ein Schätzwert, die aktuellen Abrechnungsbeträge können variieren, und der Betrag enthält keine Steuern, Gutschriften, Korrekturen oder andere Gebühren, die auftreten können.</span><span class="sxs-lookup"><span data-stu-id="493ee-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="493ee-116">Die Ausgaben werden einmal pro Tag aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="493ee-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="493ee-117">Ihre Kunden können Azure-Dienste und -Ressourcen weiterhin nutzen und diese in Rechnung stellen, solange Sie die Kontoeinstellungen im Azure-Portal nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="493ee-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="493ee-118">Dieses Feature ist nicht in Sandbox oder Test in Production (TIP) Konten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="493ee-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="493ee-119">Aktivieren von E-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="493ee-119">Turn on email notifications</span></span>**
1.  <span data-ttu-id="493ee-120">Wählen Sie im Partner Center-Menü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="493ee-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="493ee-121">Aktivieren Sie die Option **E-Mails erhalten**, um sich benachrichtigen zu lassen, wenn Ihre Kunden mindestens 80 % ihres Budgets aufgebraucht haben.</span><span class="sxs-lookup"><span data-stu-id="493ee-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="493ee-122">Dadurch behalten Sie Ihre Azure-Rechnung im Blick.</span><span class="sxs-lookup"><span data-stu-id="493ee-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="493ee-123">Sie können die standardmäßige E-Mail-Adresse für den Empfang von Benachrichtigungen in eine persönliche oder beliebige andere E-Mail-Adresse ändern.</span><span class="sxs-lookup"><span data-stu-id="493ee-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

**<span data-ttu-id="493ee-124">Festlegen eines Budgets</span><span class="sxs-lookup"><span data-stu-id="493ee-124">Set a budget</span></span>**
1.  <span data-ttu-id="493ee-125">Wählen Sie im Partner Center-Menü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="493ee-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="493ee-126">Wählen Sie die Kunden aus, für die Sie ein Budget festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="493ee-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="493ee-127">Geben Sie einen Wert im Feld **Monatsbudget** ein, und wählen Sie dann **Übernehmen**.</span><span class="sxs-lookup"><span data-stu-id="493ee-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="493ee-128">Zum Überprüfen der aktuellen Ausgaben kehren Sie zu dieser Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="493ee-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="493ee-129">Ein Budget kann auch auf der Verwaltungsseite für einen Kunden unter **Usage-based subscriptions** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="493ee-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

**<span data-ttu-id="493ee-130">Entfernen eines Budgets</span><span class="sxs-lookup"><span data-stu-id="493ee-130">Remove a budget</span></span>**
1.  <span data-ttu-id="493ee-131">Wählen Sie im Partner Center-Menü **Azure-Ausgaben**.</span><span class="sxs-lookup"><span data-stu-id="493ee-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="493ee-132">Wählen Sie Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="493ee-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="493ee-133">Wählen Sie **Remove budget**.</span><span class="sxs-lookup"><span data-stu-id="493ee-133">Select **Remove budget**.</span></span>

**<span data-ttu-id="493ee-134">Detaillierte Kosten anzeigen</span><span class="sxs-lookup"><span data-stu-id="493ee-134">See itemized costs</span></span>**
1.  <span data-ttu-id="493ee-135">Wählen Sie im Partner Center-Menü **Kunden**aus.</span><span class="sxs-lookup"><span data-stu-id="493ee-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="493ee-136">Wählen Sie einen Kunden aus der Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="493ee-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="493ee-137">Wählen Sie auf der Kundenverwaltungsseite unter **Usage-based subscriptions** ein Abonnement aus.</span><span class="sxs-lookup"><span data-stu-id="493ee-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="493ee-138">Die aktuelle geschätzte Verwendung und eine Liste der Einzelkosten pro Dienst werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="493ee-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



