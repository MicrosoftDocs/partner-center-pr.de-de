---
title: Nutzungsbasierte Abrechnung
ms.topic: article
ms.date: 06/05/2020
Description: Erfahren Sie mehr über die nutzungsbasierte Abrechnung in Partner Center, bei der Ihnen monatliche Nutzungsgebühren in Rechnung gestellt werden.
author: sodeb
ms.author: sodeb
keywords: Abrechnung, Nutzungs basiert, Nutzung
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4e75e915d4728d021856b099b7c62434f6481254
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949084"
---
# <a name="understand-usage-based-billing-for-monthly-pay-as-you-go-consumption-of-services"></a><span data-ttu-id="756ab-104">Grundlegendes zur nutzungsbasierten Abrechnung für den monatlichen Verbrauch von Diensten mit Nutzungs basierter Bezahlung</span><span class="sxs-lookup"><span data-stu-id="756ab-104">Understand usage-based billing for monthly, pay-as-you-go consumption of services</span></span>

- <span data-ttu-id="756ab-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="756ab-105">Partner Center</span></span>
- <span data-ttu-id="756ab-106">Partner im CSP-Programm</span><span class="sxs-lookup"><span data-stu-id="756ab-106">Partners in the CSP program</span></span>

<span data-ttu-id="756ab-107">Wenn Sie Onlinedienste wie z. b. Azure-Abonnements erwerben, werden Ihnen monatliche Nutzungsraten in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="756ab-107">When you buy online services such as Azure subscriptions, you're billed for monthly usage rates.</span></span> <span data-ttu-id="756ab-108">Nutzungsbasierte Dienste wie Azure werden entsprechend den getakteten Dienstleistungspreisen, basierend auf dem Verbrauch, abgerechnet.</span><span class="sxs-lookup"><span data-stu-id="756ab-108">Usage-based services, such as Azure, are billed according to metered rates, based on consumption.</span></span>

<span data-ttu-id="756ab-109">Einige Microsoft-Produkte und -Dienste verwenden das Abrechnungsmodell „nutzungsbasierte Bezahlung“, bei dem Ihnen nur genutzte Dienste in Rechnung gestellt werden.</span><span class="sxs-lookup"><span data-stu-id="756ab-109">Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used.</span></span> <span data-ttu-id="756ab-110">Dieses Modell verwendet beispielsweise Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="756ab-110">For example, Microsoft Azure uses this model.</span></span> 

## <a name="usage-billing-frequency"></a><span data-ttu-id="756ab-111">Nutzungs Abrechnungs Häufigkeit</span><span class="sxs-lookup"><span data-stu-id="756ab-111">Usage billing frequency</span></span>

<span data-ttu-id="756ab-112">Nur die **monatliche Abrechnung** ist für nutzungsbasierte Produkte verfügbar.</span><span class="sxs-lookup"><span data-stu-id="756ab-112">Only **monthly billing** is available for usage-based products.</span></span> <span data-ttu-id="756ab-113">Weitere Informationen zur monatlichen Abrechnung finden Sie in den [monatlichen und jährlichen Abrechnungs unterschieden](billing-annual-monthly.md).</span><span class="sxs-lookup"><span data-stu-id="756ab-113">For more information on monthly billing, see [Monthly and annual billing differences](billing-annual-monthly.md).</span></span>

<span data-ttu-id="756ab-114">Nutzungsbasierte Abonnements werden monatlich nach dem **Abonnement Stichtag**in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="756ab-114">Usage-based subscriptions are billed monthly, in arrears, on the **subscription anniversary date**.</span></span> <span data-ttu-id="756ab-115">Wenn das Abonnement Jahrestag z. b. der 15. Januar ist, wird Ihnen der 15. Januar für den Dienst Zeitraum vom 15. Januar bis zum 14. Januar in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="756ab-115">For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period of December 15 to January 14.</span></span> <span data-ttu-id="756ab-116">Sie werden am 15. Februar für den Dienst Zeitraum vom 15. Januar bis zum 14. Februar in Rechnung gestellt.</span><span class="sxs-lookup"><span data-stu-id="756ab-116">You will be charged again on February 15 for the service period of January 15 to February 14.</span></span>

## <a name="usage-charges"></a><span data-ttu-id="756ab-117">Usage Charges</span><span class="sxs-lookup"><span data-stu-id="756ab-117">Usage charges</span></span>

<span data-ttu-id="756ab-118">Die Gebühren, die für das Abonnement Stichtag generiert werden, werden in der folgenden Rechnung und in der Abstimmungs [Datei](usage-based-recon-files.md)angezeigt.</span><span class="sxs-lookup"><span data-stu-id="756ab-118">The charges that are generated on the subscription anniversary date will appear on the following invoice and [reconciliation file](usage-based-recon-files.md).</span></span>

<span data-ttu-id="756ab-119">Gelegentlich bemerken Sie, dass einige Nutzungsgebühren in Ihrer Rechnung fehlen, oder dass die Nutzung aus einem vorherigen Monat in der Rechnung des aktuellen Monats abgerechnet wird.</span><span class="sxs-lookup"><span data-stu-id="756ab-119">You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice.</span></span> <span data-ttu-id="756ab-120">Dies ist kein Fehler. Es bedeutet lediglich, dass der Dienst mit einem Zeitstempel versehen wurde, nachdem die Dienste erfolgt sind.</span><span class="sxs-lookup"><span data-stu-id="756ab-120">This is not an error; it simply means that the service was timestamped after the services occurred.</span></span> <span data-ttu-id="756ab-121">Die innerhalb von 24 Stunden nach dem Ende des Abrechnungszeitraums gemeldete Nutzung wird auf der Rechnung des nächsten Monats angezeigt.</span><span class="sxs-lookup"><span data-stu-id="756ab-121">Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill.</span></span>

## <a name="cancelling-usage-based-subscriptions"></a><span data-ttu-id="756ab-122">Abbrechen von Verwendungs basierten Abonnements</span><span class="sxs-lookup"><span data-stu-id="756ab-122">Cancelling usage-based subscriptions</span></span>

<span data-ttu-id="756ab-123">Nutzungsbasierte Abonnements können jederzeit angehalten werden.</span><span class="sxs-lookup"><span data-stu-id="756ab-123">You can suspend usage-based subscriptions at any time.</span></span>

## <a name="pricing-for-usage"></a><span data-ttu-id="756ab-124">Preise für die Nutzung</span><span class="sxs-lookup"><span data-stu-id="756ab-124">Pricing for usage</span></span>

<span data-ttu-id="756ab-125">Die Azure-CSP-Preisliste wird monatlich veröffentlicht und ist auf der Partner Center-Seite „Verkaufen“ -> „Preise und Angebote“ zu finden.</span><span class="sxs-lookup"><span data-stu-id="756ab-125">The Azure CSP Price List is published monthly and can be found on the Partner Center Sell->Pricing and Offers page.</span></span> <span data-ttu-id="756ab-126">Bitte beachten Sie, dass die Preise sich täglich ändern können und auf der Registerkarte „Änderungsverlauf“ der Preisliste angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="756ab-126">Please note prices can change daily and are reflected on the Change History tab of the Price List.</span></span>

<span data-ttu-id="756ab-127">Nutzungsgebühren basieren auf Preisen pro Tag.</span><span class="sxs-lookup"><span data-stu-id="756ab-127">Usage charges are based on daily prices.</span></span> <span data-ttu-id="756ab-128">Wenn sich der Preis während des Dienstzeitraums ändert, sehen Sie eine Rechnungsposition für jeden anteiligen Dienstzeitraum und den anzuwendenden Preis.</span><span class="sxs-lookup"><span data-stu-id="756ab-128">If the price changes during the service period you will see a billing line for each prorated service period and applicable price.</span></span>
