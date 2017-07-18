---
title: "Einrichten eines Kundenbudgets für Azure-Kosten | Partner Center"
description: "In Partner Center können Sie für jeden Kunden ein monatliches Budget festlegen, sodass die Azure-Rechnung am Monatsende nicht zu einer Überraschung wird."
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.openlocfilehash: 873190885d83f70f6ff68e277f288d58cc74ca00
ms.sourcegitcommit: 0b00306bfb0b406e64ad857cb360de4533740e6a
ms.translationtype: HT
ms.contentlocale: de-DE
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="8f73d-103">Einrichten eines Kundenbudgets für Azure-Kosten</span><span class="sxs-lookup"><span data-stu-id="8f73d-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="8f73d-104">Betrifft</span><span class="sxs-lookup"><span data-stu-id="8f73d-104">Applies to</span></span>**

-  <span data-ttu-id="8f73d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="8f73d-105">Partner Center</span></span>
-  <span data-ttu-id="8f73d-106">Partner Center für Microsoft Cloud für US-Behörden</span><span class="sxs-lookup"><span data-stu-id="8f73d-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="8f73d-107">Partner Center für Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="8f73d-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="8f73d-108">Um Kunden bei der Verwaltung der Azure-Kosten behilflich zu sein, können Sie ein monatliches Budget festlegen, damit die Azure-Rechnung nicht höher, als erwartet ist.</span><span class="sxs-lookup"><span data-stu-id="8f73d-108">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="8f73d-109">Das Festlegen eines Kundenbudgets für Azure-Kosten ermöglicht Ihnen, die Azure-Kosten Ihres Kunden mit dem monatlichen Budget zu vergleichen.</span><span class="sxs-lookup"><span data-stu-id="8f73d-109">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="8f73d-110">Diese Funktion bietet folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="8f73d-110">With this feature, you can:</span></span> 

-   <span data-ttu-id="8f73d-111">Benachrichtigung per E-Mail, wenn die Ausgaben des Kunden das Budgetlimit erreicht.</span><span class="sxs-lookup"><span data-stu-id="8f73d-111">Be notified by email if a customer's spending is near the budget limit.</span></span>
-   <span data-ttu-id="8f73d-112">Überprüfen der geschätzten Azure-Kosten des Kunden pro Monat.</span><span class="sxs-lookup"><span data-stu-id="8f73d-112">Review your customers’ estimated Azure costs per month.</span></span>
-   <span data-ttu-id="8f73d-113">Prüfen Sie, ob ein Dienst falsch konfiguriert ist oder ob ungewöhnliche Verwendungstrends vorliegen, die auf Betrug hinweisen.</span><span class="sxs-lookup"><span data-stu-id="8f73d-113">Spot a misconfigured service, or unusual usage trends that might suggest fraud.</span></span>
-   <span data-ttu-id="8f73d-114">Ermitteln Sie mit dem Kunden zusammen die Ursache des Problems, und verwalten Sie zusammen die Kosten.</span><span class="sxs-lookup"><span data-stu-id="8f73d-114">Work with the customer to identify the root issue and manage costs.</span></span>
-   <span data-ttu-id="8f73d-115">Erhöhen Sie ggf. das Budget.</span><span class="sxs-lookup"><span data-stu-id="8f73d-115">Change the budget to a higher amount if you and your customer are comfortable with it.</span></span>

<span data-ttu-id="8f73d-116">Die Azure-Ausgaben sind nur ein Schätzwert, die aktuellen Abrechnungsbeträge können variieren, und der Betrag enthält keine Steuern, Gutschriften, Korrekturen oder andere Gebühren, die auftreten können.</span><span class="sxs-lookup"><span data-stu-id="8f73d-116">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="8f73d-117">Die Ausgaben werden einmal pro Tag aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="8f73d-117">Spending data is refreshed once per day.</span></span> <span data-ttu-id="8f73d-118">Ihre Kunden können Azure-Dienste und -Ressourcen weiterhin nutzen und diese in Rechnung stellen, solange Sie die Kontoeinstellungen im Azure-Portal nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="8f73d-118">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

><span data-ttu-id="8f73d-119">**Hinweis:**   Dieses Feature ist nicht in Sandbox oder bei TIP-Konten (Test in Production) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8f73d-119">**Note**   This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="8f73d-120">Aktivieren von E-Mail-Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="8f73d-120">Turn on email notifications</span></span>**

1.  <span data-ttu-id="8f73d-121">Wählen Sie im Menü „Dashboard“ die Option **Microsoft Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-121">From the Dashboard menu, select **Microsoft Azure spending**.</span></span>
2.  <span data-ttu-id="8f73d-122">Klicken Sie auf die Schaltfläche **E-Mails erhalten**, um sich benachrichtigen zu lassen, wenn Ihre Kunden mindestens 80 % ihres Budgets aufgebraucht haben.</span><span class="sxs-lookup"><span data-stu-id="8f73d-122">Click the **Get emails** button to be notified if your customers use 80% or more of their budget.</span></span> <span data-ttu-id="8f73d-123">Dadurch behalten Sie Ihre Azure-Rechnung im Blick.</span><span class="sxs-lookup"><span data-stu-id="8f73d-123">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="8f73d-124">Sie können die standardmäßige E-Mail-Adresse für den Empfang von Benachrichtigungen in eine persönliche oder beliebige andere E-Mail-Adresse ändern.</span><span class="sxs-lookup"><span data-stu-id="8f73d-124">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="8f73d-125"><a href="" id="setabudget"></a>
**Festlegen eines Budgets**</span><span class="sxs-lookup"><span data-stu-id="8f73d-125"><a href="" id="setabudget"></a>
**Set a budget**</span></span>

1.  <span data-ttu-id="8f73d-126">Wählen Sie im Menü „Dashboard“ die Option **Microsoft Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-126">From the Dashboard menu, select **Microsoft Azure spending**.</span></span>
2.  <span data-ttu-id="8f73d-127">Wählen Sie Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-127">Select customers from the list.</span></span>
3.  <span data-ttu-id="8f73d-128">Geben Sie einen Wert im Feld **Monatsbudget** ein, und wählen Sie **Übernehmen**.</span><span class="sxs-lookup"><span data-stu-id="8f73d-128">Enter a value in the **Monthly budget** field and select **Apply**.</span></span>
4.  <span data-ttu-id="8f73d-129">Zum Überprüfen der aktuellen Ausgaben kehren Sie zu dieser Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="8f73d-129">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="8f73d-130">Ein Budget kann auch auf der Verwaltungsseite für einen Kunden unter **Usage-based subscriptions** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8f73d-130">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="8f73d-131"><a href="" id="removeabudget"></a>
**Entfernen eines Budgets**</span><span class="sxs-lookup"><span data-stu-id="8f73d-131"><a href="" id="removeabudget"></a>
**Remove a budget**</span></span>

1.  <span data-ttu-id="8f73d-132">Wählen Sie im Menü „Dashboard“ die Option **Microsoft Azure-Ausgaben** aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-132">From the Dashboard menu, select **Microsoft Azure spending**.</span></span>
2.  <span data-ttu-id="8f73d-133">Wählen Sie Kunden aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-133">Select customers from the list.</span></span>
3.  <span data-ttu-id="8f73d-134">Wählen Sie **Remove budget**.</span><span class="sxs-lookup"><span data-stu-id="8f73d-134">Select **Remove budget**.</span></span>

<span data-ttu-id="8f73d-135"><a href="" id="seeitemizedcosts"></a>
**Detaillierte Kosten anzeigen**</span><span class="sxs-lookup"><span data-stu-id="8f73d-135"><a href="" id="seeitemizedcosts"></a>
**See itemized costs**</span></span>

1.  <span data-ttu-id="8f73d-136">Wählen Sie im Menü „Dashboard“ die Option **Kunden** aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-136">From the Dashboard menu, select **Customers**.</span></span>
2.  <span data-ttu-id="8f73d-137">Wählen Sie einen Kunden aus der Kundenliste.</span><span class="sxs-lookup"><span data-stu-id="8f73d-137">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="8f73d-138">Wählen Sie auf der Kundenverwaltungsseite unter **Usage-based subscriptions** ein Abonnement aus.</span><span class="sxs-lookup"><span data-stu-id="8f73d-138">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="8f73d-139">Die aktuelle geschätzte Verwendung und eine Liste der Einzelkosten pro Dienst werden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8f73d-139">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



