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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172216"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="f7d9a-104">Effektive Berechnung des Einzelpreises für die Nutzung des Azure-Plans</span><span class="sxs-lookup"><span data-stu-id="f7d9a-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="f7d9a-105">**Geeignete Rollen**</span><span class="sxs-lookup"><span data-stu-id="f7d9a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f7d9a-106">Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="f7d9a-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="f7d9a-107">Der effektive Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="f7d9a-107">The effective unit price</span></span>

<span data-ttu-id="f7d9a-108">Der effektive Einzelpreis wird auf Verbrauchseinheitsebene (im Gegensatz zur Ressourcenebene) berechnet und täglich entsprechend der Verbrauchseinheit angepasst.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="f7d9a-109">Wir berechnen den effektiven Einzelpreis anhand der folgenden drei Faktoren:</span><span class="sxs-lookup"><span data-stu-id="f7d9a-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="f7d9a-110">Verbrauch, der während des gesamten Abrechnungszyklus täglich überwacht wird</span><span class="sxs-lookup"><span data-stu-id="f7d9a-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="f7d9a-111">Abrechenbare Kosten für die Verbrauchsmessung</span><span class="sxs-lookup"><span data-stu-id="f7d9a-111">Billable cost for the meter</span></span>
- <span data-ttu-id="f7d9a-112">Tiering (falls zutreffend)</span><span class="sxs-lookup"><span data-stu-id="f7d9a-112">Tiering (if applicable)</span></span>

<span data-ttu-id="f7d9a-113">Da der Verbrauch während des gesamten Abrechnungszyklus täglich überwacht wird, schwankt der effektive Einzelpreis.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="f7d9a-114">Der Endpreis für einen bestimmten Abrechnungszyklus ist verfügbar, nachdem wir die Verbrauchsberechnung beendet und den Abrechnungszeitraum geschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="f7d9a-115">Nach der vierten oder fünften Dezimalstelle werden die meisten Verbrauchsänderungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="f7d9a-116">Ermitteln, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet</span><span class="sxs-lookup"><span data-stu-id="f7d9a-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="f7d9a-117">Wenn Sie nicht wissen, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet, verwenden Sie das folgende Verfahren, um dies zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="f7d9a-118">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f7d9a-119">Wählen Sie **Verkaufen** aus, wählen Sie **Preise und Angebote** aus, und wählen Sie dann Preise für den **Azure-Plan** aus.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="f7d9a-120">Suchen Sie Ihre Verbrauchsnummer nach ID, und laden Sie dann Ihre Preisdaten herunter.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="f7d9a-121">Beispielberechnung</span><span class="sxs-lookup"><span data-stu-id="f7d9a-121">Sample calculation</span></span>

<span data-ttu-id="f7d9a-122">Die folgende Tabelle enthält ein Beispiel dafür, wie wir den effektiven Einzelpreis während des Öffnungszeitraums berechnen.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="f7d9a-123">In der Tabelle gelten die folgenden Werte:</span><span class="sxs-lookup"><span data-stu-id="f7d9a-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="f7d9a-124">**UP** = Einzelpreis der Ressource/Stunde = 0,868</span><span class="sxs-lookup"><span data-stu-id="f7d9a-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="f7d9a-125">**BCU** = Arechnungsfähige Verbrauchseinheit für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="f7d9a-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="f7d9a-126">**BC** = Arechnungsfähige Kosten für die Verbrauchsanzeige = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="f7d9a-127">Dies spiegelt eine Anpassung des PEC-Rabatts von 15 % wider.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="f7d9a-128">Wir verwenden dann die Untergrenze der Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den Mindestbetrag in Rechnung zu stellen.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="f7d9a-129">**Effektiver Einzelpreis** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="f7d9a-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="f7d9a-130">Hinweis: Die Verbrauchseinheit in diesem Beispiel verfügt nicht über Tarife für Preise oder andere Rabatte– die Effektiven Einzelpreisfaktoren in Rabattprozentsätzen und andere Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="f7d9a-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="f7d9a-131">Date</span><span class="sxs-lookup"><span data-stu-id="f7d9a-131">Date</span></span> | <span data-ttu-id="f7d9a-132">BCU (Arechnungsfähige Verbrauchseinheit)</span><span class="sxs-lookup"><span data-stu-id="f7d9a-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="f7d9a-133">BC (agerechnete Kosten)</span><span class="sxs-lookup"><span data-stu-id="f7d9a-133">BC (Billable cost)</span></span> | <span data-ttu-id="f7d9a-134">Effektiver Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="f7d9a-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="f7d9a-135">3:00 Uhr</span><span class="sxs-lookup"><span data-stu-id="f7d9a-135">3-Aug</span></span> | <span data-ttu-id="f7d9a-136">29</span><span class="sxs-lookup"><span data-stu-id="f7d9a-136">29</span></span> | <span data-ttu-id="f7d9a-137">21.39</span><span class="sxs-lookup"><span data-stu-id="f7d9a-137">21.39</span></span> | <span data-ttu-id="f7d9a-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="f7d9a-138">0.737586206896552</span></span> |
| <span data-ttu-id="f7d9a-139">10:00 Uhr</span><span class="sxs-lookup"><span data-stu-id="f7d9a-139">10-Aug</span></span> | <span data-ttu-id="f7d9a-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="f7d9a-140">210.950039</span></span> | <span data-ttu-id="f7d9a-141">155.63</span><span class="sxs-lookup"><span data-stu-id="f7d9a-141">155.63</span></span> | <span data-ttu-id="f7d9a-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="f7d9a-142">0.737757626107858</span></span> |
| <span data-ttu-id="f7d9a-143">25:00 Uhr</span><span class="sxs-lookup"><span data-stu-id="f7d9a-143">25-Aug</span></span> | <span data-ttu-id="f7d9a-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="f7d9a-144">555.950039</span></span> | <span data-ttu-id="f7d9a-145">410.17</span><span class="sxs-lookup"><span data-stu-id="f7d9a-145">410.17</span></span> | <span data-ttu-id="f7d9a-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="f7d9a-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="f7d9a-147">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f7d9a-147">Next steps</span></span>

- [<span data-ttu-id="f7d9a-148">Abrechnung und Steuern</span><span class="sxs-lookup"><span data-stu-id="f7d9a-148">Billing and taxes</span></span>](billing.md)
