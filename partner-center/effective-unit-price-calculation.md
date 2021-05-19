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
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147121"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="11e81-104">Effektive Berechnung des Einzelpreises für die Nutzung des Azure-Plans</span><span class="sxs-lookup"><span data-stu-id="11e81-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="11e81-105">**Geeignete Rollen:** Abrechnungsadministrator</span><span class="sxs-lookup"><span data-stu-id="11e81-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="11e81-106">Der effektive Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="11e81-106">The effective unit price</span></span>

<span data-ttu-id="11e81-107">Der effektive Einzelpreis wird auf Verbrauchseinheitsebene (im Gegensatz zur Ressourcenebene) berechnet und täglich entsprechend der Verbrauchseinheit angepasst.</span><span class="sxs-lookup"><span data-stu-id="11e81-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="11e81-108">Wir berechnen den effektiven Einzelpreis anhand der folgenden drei Faktoren:</span><span class="sxs-lookup"><span data-stu-id="11e81-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="11e81-109">Verbrauch, der während des gesamten Abrechnungszyklus täglich überwacht wird</span><span class="sxs-lookup"><span data-stu-id="11e81-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="11e81-110">Abrechenbare Kosten für die Verbrauchsmessung</span><span class="sxs-lookup"><span data-stu-id="11e81-110">Billable cost for the meter</span></span>
- <span data-ttu-id="11e81-111">Tiering (falls zutreffend)</span><span class="sxs-lookup"><span data-stu-id="11e81-111">Tiering (if applicable)</span></span>

<span data-ttu-id="11e81-112">Da der Verbrauch während des gesamten Abrechnungszyklus täglich überwacht wird, schwankt der effektive Einzelpreis.</span><span class="sxs-lookup"><span data-stu-id="11e81-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="11e81-113">Der Endpreis für einen bestimmten Abrechnungszyklus ist verfügbar, nachdem wir die Verbrauchsberechnung beendet und den Abrechnungszeitraum geschlossen haben.</span><span class="sxs-lookup"><span data-stu-id="11e81-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="11e81-114">Nach der vierten oder fünften Dezimalstelle werden die meisten Verbrauchsänderungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="11e81-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="11e81-115">Ermitteln, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet</span><span class="sxs-lookup"><span data-stu-id="11e81-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="11e81-116">Wenn Sie nicht wissen, ob Ihre Verbrauchsmessung mehrstufige Preise verwendet, verwenden Sie das folgende Verfahren, um dies zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="11e81-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="11e81-117">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="11e81-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="11e81-118">Wählen Sie **Verkaufen** aus, wählen Sie **Preise und Angebote** aus, und wählen Sie dann **Azure-Planpreise** aus.</span><span class="sxs-lookup"><span data-stu-id="11e81-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="11e81-119">Suchen Sie Ihre Verbrauchsnummer nach ID, und laden Sie dann Ihre Preisdaten herunter.</span><span class="sxs-lookup"><span data-stu-id="11e81-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="11e81-120">Beispielberechnung</span><span class="sxs-lookup"><span data-stu-id="11e81-120">Sample calculation</span></span>

<span data-ttu-id="11e81-121">Die folgende Tabelle enthält ein Beispiel dafür, wie wir den effektiven Einzelpreis während des Öffnungszeitraums berechnen.</span><span class="sxs-lookup"><span data-stu-id="11e81-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="11e81-122">In der Tabelle gelten die folgenden Werte:</span><span class="sxs-lookup"><span data-stu-id="11e81-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="11e81-123">**UP** = Einzelpreis der Ressource/Stunde = 0,868</span><span class="sxs-lookup"><span data-stu-id="11e81-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="11e81-124">**BCU** = Arechnungsfähige Verbrauchseinheit für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="11e81-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="11e81-125">**BC** = Arechnungsfähige Kosten für die Verbrauchsanzeige = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="11e81-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="11e81-126">Dies spiegelt eine Anpassung des PEC-Rabatts von 15 % wider.</span><span class="sxs-lookup"><span data-stu-id="11e81-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="11e81-127">Wir verwenden dann die untere Grenze der Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den Mindestbetrag zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="11e81-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="11e81-128">**Effektiver Einzelpreis** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="11e81-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="11e81-129">Hinweis: Die Verbrauchseinheit in diesem Beispiel verfügt nicht über Tarife für Preise oder andere Rabatte– die Effektiven Einzelpreisfaktoren in Rabattprozentsätzen und andere Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="11e81-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="11e81-130">Date</span><span class="sxs-lookup"><span data-stu-id="11e81-130">Date</span></span> | <span data-ttu-id="11e81-131">BCU (Arechnungsfähige Verbrauchseinheit)</span><span class="sxs-lookup"><span data-stu-id="11e81-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="11e81-132">BC (agerechnete Kosten)</span><span class="sxs-lookup"><span data-stu-id="11e81-132">BC (Billable cost)</span></span> | <span data-ttu-id="11e81-133">Effektiver Einzelpreis</span><span class="sxs-lookup"><span data-stu-id="11e81-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="11e81-134">3:00 Uhr</span><span class="sxs-lookup"><span data-stu-id="11e81-134">3-Aug</span></span> | <span data-ttu-id="11e81-135">29</span><span class="sxs-lookup"><span data-stu-id="11e81-135">29</span></span> | <span data-ttu-id="11e81-136">21.39</span><span class="sxs-lookup"><span data-stu-id="11e81-136">21.39</span></span> | <span data-ttu-id="11e81-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="11e81-137">0.737586206896552</span></span> |
| <span data-ttu-id="11e81-138">10:00 Uhr</span><span class="sxs-lookup"><span data-stu-id="11e81-138">10-Aug</span></span> | <span data-ttu-id="11e81-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="11e81-139">210.950039</span></span> | <span data-ttu-id="11e81-140">155.63</span><span class="sxs-lookup"><span data-stu-id="11e81-140">155.63</span></span> | <span data-ttu-id="11e81-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="11e81-141">0.737757626107858</span></span> |
| <span data-ttu-id="11e81-142">25:00 Uhr</span><span class="sxs-lookup"><span data-stu-id="11e81-142">25-Aug</span></span> | <span data-ttu-id="11e81-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="11e81-143">555.950039</span></span> | <span data-ttu-id="11e81-144">410.17</span><span class="sxs-lookup"><span data-stu-id="11e81-144">410.17</span></span> | <span data-ttu-id="11e81-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="11e81-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="11e81-146">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="11e81-146">Next steps</span></span>

- [<span data-ttu-id="11e81-147">Abrechnung und Steuern</span><span class="sxs-lookup"><span data-stu-id="11e81-147">Billing and taxes</span></span>](billing.md)
