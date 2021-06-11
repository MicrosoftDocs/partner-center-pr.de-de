---
title: Private Pläne in Microsoft AppSource
description: Einrichten privater Pläne in Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008530"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="2afb7-103">Private Pläne in Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="2afb7-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="2afb7-104">Mit privaten Plänen stellen Herausgeber bestimmten Kunden benutzerdefinierte Pläne zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="2afb7-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="2afb7-105">Diese Option ist jetzt in der Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="2afb7-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="2afb7-106">Private Pläne können auf AppSource für SaaS-Angebote (Software-as-a-Service) mit der Aktion Jetzt herunterladen verkauft werden. </span><span class="sxs-lookup"><span data-stu-id="2afb7-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="2afb7-107">Bitten Sie Ihren ISV um einen privaten Plan.</span><span class="sxs-lookup"><span data-stu-id="2afb7-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="2afb7-108">Damit ein privater Plan in AppSource verfügbar ist, müssen Sie sich direkt an den ISV wenden und einen benutzerdefinierten Preis und technische Spezifikationen aushandeln.</span><span class="sxs-lookup"><span data-stu-id="2afb7-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="2afb7-109">Nachdem die Bedingungen des privaten Plans vereinbart wurden, erstellt der ISV einen Plan für Sie und weist ihn der Mandanten-ID Ihrer Organisation zu, die Sie bereitstellen müssen.</span><span class="sxs-lookup"><span data-stu-id="2afb7-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="2afb7-110">Suchen Ihrer Mandanten-ID</span><span class="sxs-lookup"><span data-stu-id="2afb7-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="2afb7-111">Wählen Sie in AppSource in der oberen rechten Ecke Ihr Kontoprofilsymbol und dann **Mandanten anzeigen aus.**</span><span class="sxs-lookup"><span data-stu-id="2afb7-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="2afb7-112">Kopieren Sie die Mandanten-ID, und stellen Sie sie dem ISV zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="2afb7-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Zeigt, wie Sie Ihre Mandanten-ID finden.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="2afb7-114">Suchen eines privaten Plans in AppSource</span><span class="sxs-lookup"><span data-stu-id="2afb7-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="2afb7-115">Es kann bis zu 48 Stunden dauern, nachdem der ISV den neuen privaten Plan veröffentlicht hat, bevor er in AppSource angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="2afb7-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="2afb7-116">Um private Pläne zu finden, die Ihrer Mandanten-ID zugeordnet sind, wählen Sie oben rechts in AppSource **Private** Pläne (Symbol "Sperren") aus.</span><span class="sxs-lookup"><span data-stu-id="2afb7-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Zeigt das Sperrsymbol (Vorhängeschloss) in der oberen Symbolleiste an.":::

<span data-ttu-id="2afb7-118">Wenn Sie nicht angemeldet sind, werden Sie in einer Meldung dazu aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="2afb7-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="2afb7-119">Anschließend können Sie die privaten Pläne, die Ihrer Mandanten-ID zugeordnet sind, auf der **Registerkarte Pläne + Preise** erwerben.</span><span class="sxs-lookup"><span data-stu-id="2afb7-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Zeigt private Angebote auf der Registerkarte &quot;Plan und Preise&quot; an.":::

<span data-ttu-id="2afb7-121">Wenn private Pläne für Ihren Mandanten nicht verfügbar sind, wird in einer Meldung angezeigt, dass Sie keine privaten Pläne oder Angebote haben.</span><span class="sxs-lookup"><span data-stu-id="2afb7-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="2afb7-122">Erwerben eines privaten Plans</span><span class="sxs-lookup"><span data-stu-id="2afb7-122">Purchase a private plan</span></span>

<span data-ttu-id="2afb7-123">Ein ISV kann einen oder mehrere private Pläne in einem Angebot enthalten.</span><span class="sxs-lookup"><span data-stu-id="2afb7-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="2afb7-124">Jedes Angebot kann sowohl öffentliche als auch private Pläne haben, aber private Pläne werden unter einer separaten Angebotsliste angezeigt, auf die über das Symbol Private Angebote (Vorhängeschloss) oben rechts auf der Seite zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="2afb7-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="2afb7-125">Verfügbare private Pläne werden auf der Registerkarte **Pläne + Preise** angezeigt. Private Pläne verfügen über einen blauen Badge.</span><span class="sxs-lookup"><span data-stu-id="2afb7-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Zeigt den Badge für ein blaues privates Angebot neben privaten Angeboten an.":::

<span data-ttu-id="2afb7-127">Um einen ausgewählten Plan zu erwerben, wählen **Sie Jetzt erwerben aus,** und führen Sie die angegebenen Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="2afb7-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2afb7-128">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="2afb7-128">Next steps</span></span>

- [<span data-ttu-id="2afb7-129">Was is Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="2afb7-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
