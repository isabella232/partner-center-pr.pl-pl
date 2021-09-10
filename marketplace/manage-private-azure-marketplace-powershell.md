---
title: 'Szybki start: zarządzanie prywatną usługą Azure Marketplace pomocą programu PowerShell'
description: W tym przewodniku Szybki start pokazano, jak zarządzać ofertami w prywatnej Azure Marketplace użyciu Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123937010"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Szybki start: zarządzanie prywatną usługą Azure Marketplace pomocą programu PowerShell

W tym artykule opisano, jak można zarządzać ofertami w prywatnej Azure Marketplace użyciu [modułu Az.Marketplace](/powershell/module/az.marketplace) programu PowerShell.

> [!IMPORTANT]
> Prywatne Azure Marketplace jest obecnie w publicznej wersji zapoznawczej. Ta wersja zapoznawcza jest dostępna bez umowy dotyczącej poziomu usług. Nie jest ona zalecana w przypadku obciążeń produkcyjnych. Niektóre funkcje mogą nie być obsługiwane lub mogą mieć ograniczone możliwości. Aby uzyskać więcej informacji, zobacz [Uzupełniające warunki korzystania z wersji zapoznawczych platformy Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Wymagania

* Jeśli nie masz subskrypcji platformy Azure, przed rozpoczęciem utwórz [bezpłatne](https://azure.microsoft.com/free/) konto.

* Jeśli zdecydujesz się używać Azure PowerShell lokalnego:
  * [Zainstaluj moduł Az programu PowerShell.](/powershell/azure/install-az-ps)
  * Połączenie konta platformy Azure przy użyciu [polecenia cmdlet Połączenie-AzAccount.](/powershell/module/az.accounts/connect-azaccount)
* Jeśli zdecydujesz się używać Azure Cloud Shell:
  * Aby [uzyskać więcej informacji,](/azure/cloud-shell/overview) zobacz Overview of Azure Cloud Shell (Omówienie Azure Cloud Shell).

  > [!IMPORTANT]
  > Gdy moduł **Az.Marketplace** programu PowerShell jest w wersji zapoznawczej, należy zainstalować go oddzielnie przy użyciu `Install-Module` polecenia cmdlet . Gdy ten moduł programu PowerShell stanie się ogólnie dostępny, będzie częścią przyszłych wydań modułu Az programu PowerShell i będzie domyślnie dostępny z poziomu usługi Azure Cloud Shell.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Jeśli masz wiele subskrypcji platformy Azure, wybierz odpowiednią subskrypcję, w ramach której mają być naliczane opłaty za zasoby. Wybierz określoną subskrypcję przy użyciu polecenia cmdlet [Set-AzContext.](/powershell/module/az.accounts/set-azcontext)

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Lista sklepów prywatnych

Aby pobrać listę magazynów prywatnych, użyj polecenia cmdlet [Get-AzMarketplacePrivateStore.](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) Poniższy przykład zawiera listę magazynów prywatnych, które zostały utworzone w zakresie dzierżawy.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Dodawanie oferty do prywatnej platformy handlowej

Aby dodać ofertę do magazynu prywatnego, użyj polecenia cmdlet [Set-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) Poniższy przykład dodaje określoną ofertę do prywatnej platformy handlowej dla magazynu prywatnego utworzonego w ramach zakresu dzierżawy.

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

## <a name="get-private-store-offers"></a>Uzyskiwanie ofert sklepu prywatnego

Aby uzyskać co najmniej jedną ofertę sklepu prywatnego, użyj polecenia cmdlet [Get-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) Poniższy przykład pobiera oferty skojarzone z określonym magazynem prywatnym, które zostały dodane w zakresie dzierżawy.

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

## <a name="remove-an-offer"></a>Usuwanie oferty

Aby usunąć ofertę z magazynu prywatnego, użyj polecenia cmdlet [Remove-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) Poniższy przykład usuwa ofertę z magazynu prywatnego, który został utworzony w zakresie dzierżawy.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Następne kroki

[Tworzenie aplikacji prywatnych i zarządzanie Azure Marketplace](create-manage-private-azure-marketplace.md).