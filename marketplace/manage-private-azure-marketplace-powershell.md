---
title: 'Schnellstart: Verwalten einer privaten Azure Marketplace mithilfe von PowerShell'
description: In dieser Schnellstartanleitung erfahren Sie, wie Sie Angebote in einem privaten Azure Marketplace mithilfe von Azure PowerShell verwalten.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412453"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Schnellstart: Verwalten einer privaten Azure Marketplace mithilfe von PowerShell

In diesem Artikel wird beschrieben, wie Sie Angebote in einem privaten Azure Marketplace mit dem PowerShell-Modul " [AZ. Marketplace](/powershell/module/az.marketplace) " verwalten können.

> [!IMPORTANT]
> Der private Azure Marketplace befindet sich derzeit in der öffentlichen Vorschau Phase. Diese Vorschauversion wird ohne Vereinbarung zum Servicelevel bereitgestellt. Für Produktionsworkloads wird sie nicht empfohlen. Manche Funktionen werden möglicherweise nicht unterstützt oder sind nur eingeschränkt verwendbar. Weitere Informationen finden Sie unter [Zusätzliche Nutzungsbestimmungen für Microsoft Azure-Vorschauen](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Requirements (Anforderungen)

* Wenn Sie kein Azure-Abonnement besitzen, können Sie ein [kostenloses Konto](https://azure.microsoft.com/free/) erstellen, bevor Sie beginnen.

* Bei lokaler Verwendung von Azure PowerShell:
  * [Installieren Sie das Az-Modul von PowerShell](/powershell/azure/install-az-ps).
  * Stellen Sie eine Verbindung mit Ihrem Azure-Konto mit dem Cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) her.
* Bei Verwendung von Azure Cloud Shell:
  * Weitere Informationen finden Sie in der [Übersicht über Azure Cloud Shell](/azure/cloud-shell/overview).

  > [!IMPORTANT]
  > Während sich das PowerShell-Modul " **AZ. Marketplace** " in der Vorschau Phase befindet, müssen Sie es separat mithilfe des `Install-Module` Cmdlets installieren. Sobald dieses PowerShell-Modul allgemein verfügbar ist, wird es in die zukünftigen Releases des Az PowerShell-Moduls integriert und in Azure Cloud Shell standardmäßig zur Verfügung gestellt.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Wenn Sie über mehrere Azure-Abonnements verfügen, müssen Sie das entsprechende Abonnement auswählen, in dem die Ressourcen fakturiert werden sollen. Wählen Sie mit dem Cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext) ein bestimmtes Abonnement aus.

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Private Filialen auflisten

Zum Abrufen einer Liste privater Speicher verwenden Sie das Cmdlet [Get-azmarketplaceprivatestore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) . Im folgenden Beispiel werden private Filialen aufgelistet, die im Mandanten Bereich erstellt wurden.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Hinzufügen eines Angebots zu einem privaten Marketplace

Zum Hinzufügen eines Angebots zu einem privaten Speicher verwenden Sie das Cmdlet [Set-azmarketplaceprivatestoreoffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) . Im folgenden Beispiel wird das angegebene Angebot einem privaten Marketplace für einen privaten Store hinzugefügt, der im Mandanten Bereich erstellt wird.

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

## <a name="get-private-store-offers"></a>Private Store-Angebote erhalten

Verwenden Sie das Cmdlet " [Get-azmarketplaceprivatestoreoffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) ", um ein oder mehrere private Store-Angebote zu erhalten. Im folgenden Beispiel werden Angebote abgerufen, die dem angegebenen privaten Speicher zugeordnet sind, die unter dem Mandanten Bereich hinzugefügt wurden.

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

## <a name="remove-an-offer"></a>Entfernen eines Angebots

Wenn Sie ein Angebot aus einem privaten Speicher entfernen möchten, verwenden Sie das Cmdlet [Remove-azmarketplaceprivatestoreoffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) . Im folgenden Beispiel wird ein Angebot aus einem privaten Speicher entfernt, der im Mandanten Bereich erstellt wurde.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Nächste Schritte

[Erstellen und verwalten Sie private Azure Marketplace](create-manage-private-azure-marketplace.md).