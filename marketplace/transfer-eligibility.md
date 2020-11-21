---
title: Übertragungs Berechtigung – Richtlinien für die Übertragung eines Abonnements zwischen Abrechnungskonten, Azure Marketplace
description: Richtlinien für kommerzielle Überprüfungen vor der Übertragung eines Abonnements zwischen Abrechnungskonten in der Azure-Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007222"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="17cf2-103">Übertragungs Berechtigung für ein Abonnement zwischen Abrechnungskonten</span><span class="sxs-lookup"><span data-stu-id="17cf2-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="17cf2-104">Sie können [ein Abonnement](/azure/cost-management-billing/understand/subscription-transfer) im Abrechnungs Abschnitt des Azure-Portal von einem Abrechnungskonto in ein anderes Konto übertragen.</span><span class="sxs-lookup"><span data-stu-id="17cf2-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="17cf2-105">Vor der Übertragung wird das Abonnement auf Produkte von Drittanbietern überprüft.</span><span class="sxs-lookup"><span data-stu-id="17cf2-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="17cf2-106">Die Übertragung ist nur zulässig, wenn *alle* Produkte für die Übertragung gelöscht werden (siehe nachfolgende [Kriterien](#criteria-for-transfer-approval-or-denial) ).</span><span class="sxs-lookup"><span data-stu-id="17cf2-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="17cf2-107">Das System generiert relevante Fehlermeldungen für die apps, die nicht gelöscht werden konnten, um Sie bei der Ermittlung der nächsten Schritte zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="17cf2-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="17cf2-108">Dieser Artikel gilt nicht für SaaS-Angebote, da SaaS-Ressourcen an einen Mandanten, nicht an ein Abonnement angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="17cf2-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="17cf2-109">Saas-Ressourcen sind von einem Abrechnungskonto auf ein anderes übertragbar, dies erfolgt jedoch pro Ressource und Azure-Support als Supportanfrage.</span><span class="sxs-lookup"><span data-stu-id="17cf2-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="17cf2-110">Kriterien für die Übertragung oder Ablehnung</span><span class="sxs-lookup"><span data-stu-id="17cf2-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="17cf2-111">Ein Abonnement kann nicht übertragen werden, wenn eine der Drittanbieter-apps eines der folgenden Kriterien erfüllt:</span><span class="sxs-lookup"><span data-stu-id="17cf2-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="17cf2-112">Das Zielkonto ist kommerziell, und die APP ist für den Verkauf über Partner deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="17cf2-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="17cf2-113">Die APP ist für ausgewählte Partner aktiviert, und das Zielkonto ist nicht in der Zulassungsliste enthalten.</span><span class="sxs-lookup"><span data-stu-id="17cf2-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="17cf2-114">Das Angebot war in der Vergangenheit ein Vorschau Angebot für ausgewählte Abonnements oder ein privates Angebot, und das Abonnement ist nicht mehr in der Zulassungsliste enthalten.</span><span class="sxs-lookup"><span data-stu-id="17cf2-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="17cf2-115">Das neue Abrechnungskonto befindet sich in einer Region, von der das Angebot verkauft wird, und das Angebot wird nicht in dieser Region verkauft.</span><span class="sxs-lookup"><span data-stu-id="17cf2-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="17cf2-116">Eine blockierte Übertragung bleibt wirksam, bis Sie die Ressource aus dem Abonnement entfernen. Anschließend können Sie die Übertragung erneut versuchen.</span><span class="sxs-lookup"><span data-stu-id="17cf2-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17cf2-117">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="17cf2-117">Next steps</span></span>

[<span data-ttu-id="17cf2-118">Unterstützung für Microsoft AppSource und Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="17cf2-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

