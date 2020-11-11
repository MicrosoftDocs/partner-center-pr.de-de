---
title: Berechnung der effektiven Einheiten Preise
ms.topic: how-to
ms.date: 11/10/2020
description: Erfahren Sie mehr über die effektive Preis Einheit und deren Berechnung. Schließt eine Beispiel Berechnung ein.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498567"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="3ad78-104">Berechnung der effektiven Einheiten Preise für die Nutzung des Azure-Plans</span><span class="sxs-lookup"><span data-stu-id="3ad78-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="3ad78-105">Der effektive Einheitspreis</span><span class="sxs-lookup"><span data-stu-id="3ad78-105">The effective unit price</span></span>

<span data-ttu-id="3ad78-106">Der Preis für die effektive Einheit wird auf der Verbrauchseinheit berechnet (im Gegensatz zur Ressourcenebene) und entsprechend der Verbrauchseinheit täglich angepasst.</span><span class="sxs-lookup"><span data-stu-id="3ad78-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="3ad78-107">Wir berechnen den effektiven Einzelpreis mithilfe der folgenden drei Faktoren:</span><span class="sxs-lookup"><span data-stu-id="3ad78-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="3ad78-108">Verbrauch, der täglich im gesamten Abrechnungszeitraum überwacht wird</span><span class="sxs-lookup"><span data-stu-id="3ad78-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="3ad78-109">Abrechnungskosten für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="3ad78-109">Billable cost for the meter</span></span>
- <span data-ttu-id="3ad78-110">Tiering (falls zutreffend)</span><span class="sxs-lookup"><span data-stu-id="3ad78-110">Tiering (if applicable)</span></span>

<span data-ttu-id="3ad78-111">Da wir die tägliche Nutzung im gesamten Abrechnungszeitraum überwachen, schwankt der effektive Einzelpreis.</span><span class="sxs-lookup"><span data-stu-id="3ad78-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="3ad78-112">Der endgültige Preis für einen bestimmten Abrechnungszeitraum ist verfügbar, nachdem die Verbrauchs Berechnung angehalten und der Abrechnungszeitraum geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="3ad78-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="3ad78-113">Die meisten Änderungen am Verbrauch werden nach dem vierten oder fünften Dezimaltrennzeichen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3ad78-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="3ad78-114">Erfahren Sie, ob Ihre Verbrauchseinheit mehrstufige Preise verwendet.</span><span class="sxs-lookup"><span data-stu-id="3ad78-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="3ad78-115">Wenn Sie nicht wissen, ob Ihre Verbrauchseinheit mehrstufige Preise verwendet, verwenden Sie das unten beschriebene Verfahren, um sich zu informieren.</span><span class="sxs-lookup"><span data-stu-id="3ad78-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="3ad78-116">Melden Sie sich beim [Partner Center-Dashboard](https://partner.microsoft.com/dashboard/) an.</span><span class="sxs-lookup"><span data-stu-id="3ad78-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="3ad78-117">Wählen Sie **verkaufen** aus, wählen Sie **Preise und Angebote** aus, und wählen Sie dann **Azure-Plan Preise** aus.</span><span class="sxs-lookup"><span data-stu-id="3ad78-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="3ad78-118">Suchen Sie nach ihrer ID, und laden Sie dann Ihre Preisdaten herunter.</span><span class="sxs-lookup"><span data-stu-id="3ad78-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="3ad78-119">Beispiel Berechnung</span><span class="sxs-lookup"><span data-stu-id="3ad78-119">Sample calculation</span></span>

<span data-ttu-id="3ad78-120">In der folgenden Tabelle finden Sie ein Beispiel dafür, wie der effektive Einzelpreis während des Öffnungs Zeitraums berechnet wird.</span><span class="sxs-lookup"><span data-stu-id="3ad78-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="3ad78-121">In der Tabelle gelten die folgenden Werte:</span><span class="sxs-lookup"><span data-stu-id="3ad78-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="3ad78-122">**Up** = Einheitspreis der Ressource/Stunde = 0,868</span><span class="sxs-lookup"><span data-stu-id="3ad78-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="3ad78-123">**BCU** = abrechenbare Verbrauchseinheit für die Verbrauchseinheit</span><span class="sxs-lookup"><span data-stu-id="3ad78-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="3ad78-124">**BC** = Abrechnungskosten für die Verbrauchseinheit = BCU \* up \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="3ad78-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="3ad78-125">Dies spiegelt eine Anpassung für den 15% PEC-Rabatt wider.</span><span class="sxs-lookup"><span data-stu-id="3ad78-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="3ad78-126">Wir verwenden dann den unteren Grenzwert der-Funktion, um den Wert auf zwei Ziffern nach dem Dezimaltrennzeichen zu beschränken, um den minimalen Betrag zu berechnen.</span><span class="sxs-lookup"><span data-stu-id="3ad78-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="3ad78-127">**Effektiver Einheitspreis** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="3ad78-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="3ad78-128">Hinweis: die Verbrauchseinheit in diesem Beispiel enthält keine Tarife in den Preisen.</span><span class="sxs-lookup"><span data-stu-id="3ad78-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="3ad78-129">Datum</span><span class="sxs-lookup"><span data-stu-id="3ad78-129">Date</span></span> | <span data-ttu-id="3ad78-130">BCU (abrechenbare Verbrauchseinheit)</span><span class="sxs-lookup"><span data-stu-id="3ad78-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="3ad78-131">BC (Abrechnungskosten)</span><span class="sxs-lookup"><span data-stu-id="3ad78-131">BC (Billable cost)</span></span> | <span data-ttu-id="3ad78-132">Effektiver Einheitspreis</span><span class="sxs-lookup"><span data-stu-id="3ad78-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="3ad78-133">3. Aug</span><span class="sxs-lookup"><span data-stu-id="3ad78-133">3-Aug</span></span> | <span data-ttu-id="3ad78-134">29</span><span class="sxs-lookup"><span data-stu-id="3ad78-134">29</span></span> | <span data-ttu-id="3ad78-135">21,39</span><span class="sxs-lookup"><span data-stu-id="3ad78-135">21.39</span></span> | <span data-ttu-id="3ad78-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="3ad78-136">0.737586206896552</span></span> |
| <span data-ttu-id="3ad78-137">10. Aug</span><span class="sxs-lookup"><span data-stu-id="3ad78-137">10-Aug</span></span> | <span data-ttu-id="3ad78-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="3ad78-138">210.950039</span></span> | <span data-ttu-id="3ad78-139">155,63</span><span class="sxs-lookup"><span data-stu-id="3ad78-139">155.63</span></span> | <span data-ttu-id="3ad78-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="3ad78-140">0.737757626107858</span></span> |
| <span data-ttu-id="3ad78-141">25. Aug</span><span class="sxs-lookup"><span data-stu-id="3ad78-141">25-Aug</span></span> | <span data-ttu-id="3ad78-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="3ad78-142">555.950039</span></span> | <span data-ttu-id="3ad78-143">410,17</span><span class="sxs-lookup"><span data-stu-id="3ad78-143">410.17</span></span> | <span data-ttu-id="3ad78-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="3ad78-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="3ad78-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="3ad78-145">Next steps</span></span>

- [<span data-ttu-id="3ad78-146">Abrechnung und Steuern</span><span class="sxs-lookup"><span data-stu-id="3ad78-146">Billing and taxes</span></span>](billing.md)
