---
title: Berechnung des effektiven Preises pro Einheit
ms.topic: how-to
ms.date: 04/02/2021
description: Erfahren Sie mehr über den effektiven Einzelpreis und seine Berechnung. Dieser Artikel enthält auch eine Beispielberechnung.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528571"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="6dfc8-104">Effektive Berechnung des Einzelpreis für den Azure-Planverbrauch</span><span class="sxs-lookup"><span data-stu-id="6dfc8-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="6dfc8-105">Der effektive Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="6dfc8-105">The effective unit price</span></span>

<span data-ttu-id="6dfc8-106">Der effektive Einzelpreis wird auf Verbrauchseinheitsebene (im Gegensatz zur Ressourcenebene) berechnet und täglich entsprechend der Verbrauchseinheitsnutzung angepasst.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="6dfc8-107">Wir berechnen den effektiven Einzelpreis anhand der folgenden drei Faktoren:</span><span class="sxs-lookup"><span data-stu-id="6dfc8-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="6dfc8-108">Verbrauch, der während des abrechnungszyklus täglich überwacht wird</span><span class="sxs-lookup"><span data-stu-id="6dfc8-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="6dfc8-109">Arechnungsfähige Kosten für die Verbrauchsanzeige</span><span class="sxs-lookup"><span data-stu-id="6dfc8-109">Billable cost for the meter</span></span>
- <span data-ttu-id="6dfc8-110">Tiering (falls zutreffend)</span><span class="sxs-lookup"><span data-stu-id="6dfc8-110">Tiering (if applicable)</span></span>

<span data-ttu-id="6dfc8-111">Da der Verbrauch während des abrechnungszyklus täglich überwacht wird, schwankt der effektive Einzelpreis.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="6dfc8-112">Der Endpreis für einen bestimmten Abrechnungszyklus ist verfügbar, nachdem wir die Verbrauchsberechnung beenden und den Abrechnungszeitraum geschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="6dfc8-113">Nach der vierten oder fünften Dezimalstelle werden die meisten Änderungen im Verbrauch angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="6dfc8-114">Finden Sie heraus, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="6dfc8-115">Wenn Sie nicht wissen, ob Ihre Verbrauchsanzeige mehrstufige Preise verwendet, gehen Sie wie folgt vor, um dies herauszufinden.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="6dfc8-116">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6dfc8-117">Wählen **Sie Verkaufen** aus, wählen Sie Preise und **Angebote** aus, und wählen Sie dann Preise **für Azure-Plan aus.**</span><span class="sxs-lookup"><span data-stu-id="6dfc8-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="6dfc8-118">Suchen Sie ihre Verbrauchsanzeige nach ID, und laden Sie dann Ihre Preisdaten herunter.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="6dfc8-119">Beispielberechnung</span><span class="sxs-lookup"><span data-stu-id="6dfc8-119">Sample calculation</span></span>

<span data-ttu-id="6dfc8-120">Die folgende Tabelle enthält ein Beispiel dafür, wie wir den effektiven Einzelpreis während des offenen Zeitraums berechnen.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="6dfc8-121">In der Tabelle gelten die folgenden Werte:</span><span class="sxs-lookup"><span data-stu-id="6dfc8-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="6dfc8-122">**UP** = Einzelpreis der Ressource/Stunde = 0,868</span><span class="sxs-lookup"><span data-stu-id="6dfc8-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="6dfc8-123">**BCU** = Abrechenbare Verbrauchseinheit für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="6dfc8-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="6dfc8-124">**BC** = Abrechenbare Kosten für die Verbrauchsmessung = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="6dfc8-125">Dies spiegelt eine Anpassung des PEC-Rabatts von 15 % wider.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="6dfc8-126">Wir verwenden dann die untere Grenze der Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den Mindestbetrag zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="6dfc8-127">**Effektiver Einzelpreis** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="6dfc8-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="6dfc8-128">Hinweis: Die Verbrauchseinheit in diesem Beispiel verfügt nicht über Tarife für Preise oder andere Rabatte– die Effektiven Preiseinheitenfaktoren in Rabattprozentsätzen und andere Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="6dfc8-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="6dfc8-129">Date</span><span class="sxs-lookup"><span data-stu-id="6dfc8-129">Date</span></span> | <span data-ttu-id="6dfc8-130">BCU (Abrechenbare Verbrauchseinheit)</span><span class="sxs-lookup"><span data-stu-id="6dfc8-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="6dfc8-131">BC (Abrechenbare Kosten)</span><span class="sxs-lookup"><span data-stu-id="6dfc8-131">BC (Billable cost)</span></span> | <span data-ttu-id="6dfc8-132">Effektiver Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="6dfc8-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="6dfc8-133">3-Aug</span><span class="sxs-lookup"><span data-stu-id="6dfc8-133">3-Aug</span></span> | <span data-ttu-id="6dfc8-134">29</span><span class="sxs-lookup"><span data-stu-id="6dfc8-134">29</span></span> | <span data-ttu-id="6dfc8-135">21.39</span><span class="sxs-lookup"><span data-stu-id="6dfc8-135">21.39</span></span> | <span data-ttu-id="6dfc8-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="6dfc8-136">0.737586206896552</span></span> |
| <span data-ttu-id="6dfc8-137">10-Aug</span><span class="sxs-lookup"><span data-stu-id="6dfc8-137">10-Aug</span></span> | <span data-ttu-id="6dfc8-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="6dfc8-138">210.950039</span></span> | <span data-ttu-id="6dfc8-139">155.63</span><span class="sxs-lookup"><span data-stu-id="6dfc8-139">155.63</span></span> | <span data-ttu-id="6dfc8-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="6dfc8-140">0.737757626107858</span></span> |
| <span data-ttu-id="6dfc8-141">25-Aug</span><span class="sxs-lookup"><span data-stu-id="6dfc8-141">25-Aug</span></span> | <span data-ttu-id="6dfc8-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="6dfc8-142">555.950039</span></span> | <span data-ttu-id="6dfc8-143">410.17</span><span class="sxs-lookup"><span data-stu-id="6dfc8-143">410.17</span></span> | <span data-ttu-id="6dfc8-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="6dfc8-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="6dfc8-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="6dfc8-145">Next steps</span></span>

- [<span data-ttu-id="6dfc8-146">Abrechnung und Steuern</span><span class="sxs-lookup"><span data-stu-id="6dfc8-146">Billing and taxes</span></span>](billing.md)
