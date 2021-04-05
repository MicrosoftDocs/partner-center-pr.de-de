---
title: Berechnung des effektiven Preises pro Einheit
ms.topic: how-to
ms.date: 04/02/2021
description: Erfahren Sie mehr über den effektiven Einzelpreis und seine Berechnung. Dieser Artikel enthält auch eine Beispiel Berechnung.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374390"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="07273-104">Berechnung der effektiven Einheiten Preise für die Nutzung des Azure-Plans</span><span class="sxs-lookup"><span data-stu-id="07273-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="07273-105">Der effektive Einheitspreis</span><span class="sxs-lookup"><span data-stu-id="07273-105">The effective unit price</span></span>

<span data-ttu-id="07273-106">Der Preis für die effektive Einheit wird auf der Verbrauchseinheit berechnet (im Gegensatz zur Ressourcenebene) und entsprechend der Verbrauchseinheit täglich angepasst.</span><span class="sxs-lookup"><span data-stu-id="07273-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="07273-107">Wir berechnen den effektiven Einzelpreis mithilfe der folgenden drei Faktoren:</span><span class="sxs-lookup"><span data-stu-id="07273-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="07273-108">Verbrauch, der täglich im gesamten Abrechnungszeitraum überwacht wird</span><span class="sxs-lookup"><span data-stu-id="07273-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="07273-109">Abrechnungskosten für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="07273-109">Billable cost for the meter</span></span>
- <span data-ttu-id="07273-110">Tiering (falls zutreffend)</span><span class="sxs-lookup"><span data-stu-id="07273-110">Tiering (if applicable)</span></span>

<span data-ttu-id="07273-111">Da wir die tägliche Nutzung im gesamten Abrechnungszeitraum überwachen, schwankt der effektive Einzelpreis.</span><span class="sxs-lookup"><span data-stu-id="07273-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="07273-112">Der endgültige Preis für einen bestimmten Abrechnungszeitraum ist verfügbar, nachdem die Verbrauchs Berechnung angehalten und der Abrechnungszeitraum geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="07273-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="07273-113">Die meisten Änderungen am Verbrauch werden nach dem vierten oder fünften Dezimaltrennzeichen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="07273-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="07273-114">Erfahren Sie, ob Ihre Verbrauchseinheit mehrstufige Preise verwendet.</span><span class="sxs-lookup"><span data-stu-id="07273-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="07273-115">Wenn Sie nicht wissen, ob Ihre Verbrauchseinheit mehrstufige Preise verwendet, verwenden Sie das unten beschriebene Verfahren, um sich zu informieren.</span><span class="sxs-lookup"><span data-stu-id="07273-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="07273-116">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="07273-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="07273-117">Wählen Sie **verkaufen** aus, wählen Sie **Preise und Angebote** aus, und wählen Sie dann **Azure-Plan Preise** aus.</span><span class="sxs-lookup"><span data-stu-id="07273-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="07273-118">Suchen Sie nach ihrer ID, und laden Sie dann Ihre Preisdaten herunter.</span><span class="sxs-lookup"><span data-stu-id="07273-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="07273-119">Beispiel Berechnung</span><span class="sxs-lookup"><span data-stu-id="07273-119">Sample calculation</span></span>

<span data-ttu-id="07273-120">In der folgenden Tabelle finden Sie ein Beispiel dafür, wie der effektive Einzelpreis während des Öffnungs Zeitraums berechnet wird.</span><span class="sxs-lookup"><span data-stu-id="07273-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="07273-121">In der Tabelle gelten die folgenden Werte:</span><span class="sxs-lookup"><span data-stu-id="07273-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="07273-122">**Up** = Einheitspreis der Ressource/Stunde = 0,868</span><span class="sxs-lookup"><span data-stu-id="07273-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="07273-123">**BCU** = abrechenbare Verbrauchseinheit für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="07273-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="07273-124">**BC** = Abrechnungskosten für die Verbrauchseinheit = BCU \* up \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="07273-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="07273-125">Dies spiegelt eine Anpassung für den 15% PEC-Rabatt wider.</span><span class="sxs-lookup"><span data-stu-id="07273-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="07273-126">Wir verwenden dann den unteren Grenzwert der-Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den minimalen Betrag zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="07273-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="07273-127">**Effektiver Einheitspreis** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="07273-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="07273-128">Die Verbrauchseinheit in diesem Beispiel enthält keine Tarife in den Preisen.</span><span class="sxs-lookup"><span data-stu-id="07273-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="07273-129">Die effektiven Einheiten Preisfaktoren in Rabatt Prozentsätzen und anderen Anpassungen.</span><span class="sxs-lookup"><span data-stu-id="07273-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="07273-130">Date</span><span class="sxs-lookup"><span data-stu-id="07273-130">Date</span></span> | <span data-ttu-id="07273-131">BCU (abrechenbare Verbrauchseinheit)</span><span class="sxs-lookup"><span data-stu-id="07273-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="07273-132">BC (Abrechnungskosten)</span><span class="sxs-lookup"><span data-stu-id="07273-132">BC (Billable cost)</span></span> | <span data-ttu-id="07273-133">Effektiver Einheitspreis</span><span class="sxs-lookup"><span data-stu-id="07273-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="07273-134">3. Aug</span><span class="sxs-lookup"><span data-stu-id="07273-134">3-Aug</span></span> | <span data-ttu-id="07273-135">29</span><span class="sxs-lookup"><span data-stu-id="07273-135">29</span></span> | <span data-ttu-id="07273-136">21,39</span><span class="sxs-lookup"><span data-stu-id="07273-136">21.39</span></span> | <span data-ttu-id="07273-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="07273-137">0.737586206896552</span></span> |
| <span data-ttu-id="07273-138">10. Aug</span><span class="sxs-lookup"><span data-stu-id="07273-138">10-Aug</span></span> | <span data-ttu-id="07273-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="07273-139">210.950039</span></span> | <span data-ttu-id="07273-140">155,63</span><span class="sxs-lookup"><span data-stu-id="07273-140">155.63</span></span> | <span data-ttu-id="07273-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="07273-141">0.737757626107858</span></span> |
| <span data-ttu-id="07273-142">25. Aug</span><span class="sxs-lookup"><span data-stu-id="07273-142">25-Aug</span></span> | <span data-ttu-id="07273-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="07273-143">555.950039</span></span> | <span data-ttu-id="07273-144">410,17</span><span class="sxs-lookup"><span data-stu-id="07273-144">410.17</span></span> | <span data-ttu-id="07273-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="07273-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="07273-146">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="07273-146">Next steps</span></span>

- [<span data-ttu-id="07273-147">Abrechnung und Steuern</span><span class="sxs-lookup"><span data-stu-id="07273-147">Billing and taxes</span></span>](billing.md)
