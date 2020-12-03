---
title: 'Szybki Start: Zarządzanie prywatnym portalem Azure Marketplace przy użyciu programu PowerShell'
description: W tym przewodniku szybki start przedstawiono, jak zarządzać ofertami w prywatnym portalu Azure Marketplace przy użyciu Azure PowerShell.
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
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536265"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="d45cc-103">Szybki Start: Zarządzanie prywatnym portalem Azure Marketplace przy użyciu programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="d45cc-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="d45cc-104">W tym artykule opisano, jak zarządzać ofertami w prywatnym portalu Azure Marketplace przy użyciu modułu [AZ. Marketplace](/powershell/module/az.marketplace) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d45cc-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d45cc-105">Prywatny Portal Azure Marketplace jest obecnie w publicznej wersji zapoznawczej.</span><span class="sxs-lookup"><span data-stu-id="d45cc-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="d45cc-106">Ta wersja zapoznawcza jest dostępna bez umowy dotyczącej poziomu usług.</span><span class="sxs-lookup"><span data-stu-id="d45cc-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="d45cc-107">Nie jest ona zalecana w przypadku obciążeń produkcyjnych.</span><span class="sxs-lookup"><span data-stu-id="d45cc-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="d45cc-108">Niektóre funkcje mogą nie być obsługiwane lub mogą mieć ograniczone możliwości.</span><span class="sxs-lookup"><span data-stu-id="d45cc-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="d45cc-109">Aby uzyskać więcej informacji, zobacz [Uzupełniające warunki korzystania z wersji zapoznawczych platformy Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="d45cc-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="d45cc-110">Wymagania</span><span class="sxs-lookup"><span data-stu-id="d45cc-110">Requirements</span></span>

* <span data-ttu-id="d45cc-111">Jeśli nie masz subskrypcji platformy Azure, przed rozpoczęciem utwórz [bezpłatne](https://azure.microsoft.com/free/) konto.</span><span class="sxs-lookup"><span data-stu-id="d45cc-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="d45cc-112">Jeśli zdecydujesz się używać Azure PowerShell lokalnie:</span><span class="sxs-lookup"><span data-stu-id="d45cc-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="d45cc-113">[Zainstaluj moduł AZ PowerShell module](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="d45cc-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="d45cc-114">Połącz się z kontem platformy Azure przy użyciu polecenia cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="d45cc-115">Jeśli zdecydujesz się używać Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="d45cc-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="d45cc-116">Aby uzyskać więcej informacji [, zobacz omówienie Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-116">See [Overview of Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="d45cc-117">Gdy moduł programu PowerShell **AZ. Marketplace** jest w wersji zapoznawczej, należy go zainstalować oddzielnie przy użyciu `Install-Module` polecenia cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d45cc-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="d45cc-118">Po ogólnym udostępnieniu tego modułu programu PowerShell będzie on częścią przyszłych wydań modułu AZ PowerShell i dostępne domyślnie z poziomu Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="d45cc-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="d45cc-119">Jeśli masz wiele subskrypcji platformy Azure, wybierz odpowiednią subskrypcję, w której będą naliczane opłaty za zasoby.</span><span class="sxs-lookup"><span data-stu-id="d45cc-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="d45cc-120">Wybierz określoną subskrypcję za pomocą polecenia cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="d45cc-121">Utwórz listę magazynów prywatnych</span><span class="sxs-lookup"><span data-stu-id="d45cc-121">List private stores</span></span>

<span data-ttu-id="d45cc-122">Aby pobrać listę magazynów prywatnych, należy użyć polecenia cmdlet [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="d45cc-123">Poniższy przykład zawiera listę magazynów prywatnych, które zostały utworzone w ramach zakresu dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="d45cc-123">The following example lists private stores that were created under the tenant scope.</span></span>

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

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="d45cc-124">Dodawanie oferty do prywatnego portalu Marketplace</span><span class="sxs-lookup"><span data-stu-id="d45cc-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="d45cc-125">Aby dodać ofertę do magazynu prywatnego, należy użyć polecenia cmdlet [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d45cc-126">Poniższy przykład dodaje określoną ofertę do prywatnej witryny Marketplace dla prywatnego magazynu, który jest tworzony w ramach zakresu dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="d45cc-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

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

## <a name="get-private-store-offers"></a><span data-ttu-id="d45cc-127">Pobierz oferty sklepu prywatnego</span><span class="sxs-lookup"><span data-stu-id="d45cc-127">Get private store offers</span></span>

<span data-ttu-id="d45cc-128">Aby uzyskać co najmniej jedną ofertę magazynu prywatnego, należy użyć polecenia cmdlet [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d45cc-129">Poniższy przykład pobiera oferty skojarzone z określonym magazynem prywatnym, który został dodany w ramach zakresu dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="d45cc-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

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

## <a name="remove-an-offer"></a><span data-ttu-id="d45cc-130">Usuwanie oferty</span><span class="sxs-lookup"><span data-stu-id="d45cc-130">Remove an offer</span></span>

<span data-ttu-id="d45cc-131">Aby usunąć ofertę z magazynu prywatnego, należy użyć polecenia cmdlet [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d45cc-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d45cc-132">Poniższy przykład usuwa ofertę z prywatnego magazynu, który został utworzony w zakresie dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="d45cc-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="d45cc-133">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="d45cc-133">Next steps</span></span>

<span data-ttu-id="d45cc-134">[Utwórz prywatny Portal Azure Marketplace i Zarządzaj nim](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="d45cc-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>
