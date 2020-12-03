---
title: 'Schnellstart: Verwalten einer privaten Azure Marketplace mithilfe von PowerShell'
description: In dieser Schnellstartanleitung erfahren Sie, wie Sie Angebote in einem privaten Azure Marketplace mithilfe von Azure PowerShell verwalten.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536079"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="5a2e1-103">Schnellstart: Verwalten einer privaten Azure Marketplace mithilfe von PowerShell</span><span class="sxs-lookup"><span data-stu-id="5a2e1-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="5a2e1-104">In diesem Artikel wird beschrieben, wie Sie Angebote in einem privaten Azure Marketplace mit dem PowerShell-Modul " [AZ. Marketplace](/powershell/module/az.marketplace) " verwalten können.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5a2e1-105">Der private Azure Marketplace befindet sich derzeit in der öffentlichen Vorschau Phase.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="5a2e1-106">Diese Vorschauversion wird ohne Vereinbarung zum Servicelevel bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="5a2e1-107">Für Produktionsworkloads wird sie nicht empfohlen.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="5a2e1-108">Manche Funktionen werden möglicherweise nicht unterstützt oder sind nur eingeschränkt verwendbar.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="5a2e1-109">Weitere Informationen finden Sie unter [Zusätzliche Nutzungsbestimmungen für Microsoft Azure-Vorschauen](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="5a2e1-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="5a2e1-110">Requirements (Anforderungen)</span><span class="sxs-lookup"><span data-stu-id="5a2e1-110">Requirements</span></span>

* <span data-ttu-id="5a2e1-111">Wenn Sie kein Azure-Abonnement besitzen, können Sie ein [kostenloses Konto](https://azure.microsoft.com/free/) erstellen, bevor Sie beginnen.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="5a2e1-112">Bei lokaler Verwendung von Azure PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5a2e1-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="5a2e1-113">[Installieren Sie das Az-Modul von PowerShell](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="5a2e1-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="5a2e1-114">Stellen Sie eine Verbindung mit Ihrem Azure-Konto mit dem Cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) her.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="5a2e1-115">Bei Verwendung von Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="5a2e1-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="5a2e1-116">Weitere Informationen finden Sie in der [Übersicht über Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="5a2e1-116">See [Overview of Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="5a2e1-117">Während sich das PowerShell-Modul " **AZ. Marketplace** " in der Vorschau Phase befindet, müssen Sie es separat mithilfe des `Install-Module` Cmdlets installieren.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="5a2e1-118">Sobald dieses PowerShell-Modul allgemein verfügbar ist, wird es in die zukünftigen Releases des Az PowerShell-Moduls integriert und in Azure Cloud Shell standardmäßig zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="5a2e1-119">Wenn Sie über mehrere Azure-Abonnements verfügen, müssen Sie das entsprechende Abonnement auswählen, in dem die Ressourcen fakturiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="5a2e1-120">Wählen Sie mit dem Cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext) ein bestimmtes Abonnement aus.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="5a2e1-121">Private Filialen auflisten</span><span class="sxs-lookup"><span data-stu-id="5a2e1-121">List private stores</span></span>

<span data-ttu-id="5a2e1-122">Zum Abrufen einer Liste privater Speicher verwenden Sie das Cmdlet [Get-azmarketplaceprivatestore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="5a2e1-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="5a2e1-123">Im folgenden Beispiel werden private Filialen aufgelistet, die im Mandanten Bereich erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="5a2e1-124">Hinzufügen eines Angebots zu einem privaten Marketplace</span><span class="sxs-lookup"><span data-stu-id="5a2e1-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="5a2e1-125">Zum Hinzufügen eines Angebots zu einem privaten Speicher verwenden Sie das Cmdlet [Set-azmarketplaceprivatestoreoffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="5a2e1-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="5a2e1-126">Im folgenden Beispiel wird das angegebene Angebot einem privaten Marketplace für einen privaten Store hinzugefügt, der im Mandanten Bereich erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="5a2e1-127">Private Store-Angebote erhalten</span><span class="sxs-lookup"><span data-stu-id="5a2e1-127">Get private store offers</span></span>

<span data-ttu-id="5a2e1-128">Verwenden Sie das Cmdlet " [Get-azmarketplaceprivatestoreoffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) ", um ein oder mehrere private Store-Angebote zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="5a2e1-129">Im folgenden Beispiel werden Angebote abgerufen, die dem angegebenen privaten Speicher zugeordnet sind, die unter dem Mandanten Bereich hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="5a2e1-130">Entfernen eines Angebots</span><span class="sxs-lookup"><span data-stu-id="5a2e1-130">Remove an offer</span></span>

<span data-ttu-id="5a2e1-131">Wenn Sie ein Angebot aus einem privaten Speicher entfernen möchten, verwenden Sie das Cmdlet [Remove-azmarketplaceprivatestoreoffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="5a2e1-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="5a2e1-132">Im folgenden Beispiel wird ein Angebot aus einem privaten Speicher entfernt, der im Mandanten Bereich erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="5a2e1-133">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="5a2e1-133">Next steps</span></span>

<span data-ttu-id="5a2e1-134">[Erstellen und verwalten Sie private Azure Marketplace](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="5a2e1-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>
