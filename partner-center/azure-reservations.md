---
title: Sprzedaj klientów Microsoft Azure rezerwacje
description: Jako dostawca rozwiązań w chmurze możesz kupować, sprzedawać i zarządzać rezerwacjami platformy Azure dla klientów. Użyj Centrum partnerskiego, Azure Portal lub interfejsu API Centrum partnerskiego.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534900"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="6eb34-104">Sprzedawaj Microsoft Azure rezerwacje klientom przy użyciu Centrum partnerskiego, Azure Portal lub interfejsów API</span><span class="sxs-lookup"><span data-stu-id="6eb34-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="6eb34-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="6eb34-105">**Appropriate roles**</span></span>

- <span data-ttu-id="6eb34-106">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="6eb34-106">Admin agent</span></span>
- <span data-ttu-id="6eb34-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="6eb34-107">Global admin</span></span>
- <span data-ttu-id="6eb34-108">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="6eb34-108">Helpdesk agent</span></span>
- <span data-ttu-id="6eb34-109">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="6eb34-109">Sales agent</span></span>
- <span data-ttu-id="6eb34-110">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="6eb34-110">User management admin</span></span>

<span data-ttu-id="6eb34-111">Jako partner w programie dostawcy rozwiązań w chmurze (CSP) możesz kupować i sprzedawać i zarządzać rezerwacjami platformy Azure dla klientów.</span><span class="sxs-lookup"><span data-stu-id="6eb34-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="6eb34-112">Użyj Centrum partnerskiego, Azure Portal lub interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="6eb34-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="6eb34-113">Ten artykuł ma zastosowanie tylko do partnerów w dostawcy usług kryptograficznych.</span><span class="sxs-lookup"><span data-stu-id="6eb34-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="6eb34-114">Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="6eb34-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="6eb34-115">Partnerzy w programie CSP mogą zaoferować swoim klientom Microsoft Azure rezerwacje.</span><span class="sxs-lookup"><span data-stu-id="6eb34-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="6eb34-116">Klienci mogą uzyskać znaczne oszczędności w przypadku zarezerwowania z wyprzedzeniem.</span><span class="sxs-lookup"><span data-stu-id="6eb34-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="6eb34-117">Rezerwacje platformy Azure oferują klientom prostotę i elastyczność w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="6eb34-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="6eb34-118">Jednoroczne warunki rezerwacji</span><span class="sxs-lookup"><span data-stu-id="6eb34-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="6eb34-119">Łatwe rozpoczęcie pracy; Instalacja zakończona w sekundach</span><span class="sxs-lookup"><span data-stu-id="6eb34-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="6eb34-120">Anuluj lub Zarezerwuj wystąpienia w dowolnym momencie w celu skorygowania zwrotu</span><span class="sxs-lookup"><span data-stu-id="6eb34-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="6eb34-121">Zarządzanie użyciem wystąpień zarezerwowanych na poziomie organizacji lub poszczególnych działów</span><span class="sxs-lookup"><span data-stu-id="6eb34-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="6eb34-122">Rezerwacje platformy Azure mogą odwoływać się do klientów w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="6eb34-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="6eb34-123">Rezerwacje mogą oferować znaczne oszczędności w porównaniu z cennikiem płatność zgodnie z rzeczywistym użyciem</span><span class="sxs-lookup"><span data-stu-id="6eb34-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="6eb34-124">Lepsze budżetowanie i prognozowanie przy użyciu płatności z góry za rok lub trzy lata</span><span class="sxs-lookup"><span data-stu-id="6eb34-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="6eb34-125">Priorytetowe zdolności obliczeniowe w regionie świadczenia usługi Azure najbliżej ich biur</span><span class="sxs-lookup"><span data-stu-id="6eb34-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="6eb34-126">Rezerwacje platformy Azure stanowią podstawę kompleksowych rozwiązań infrastruktury w połączeniu z oprogramowaniem takim jak Microsoft Windows Server i Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="6eb34-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="6eb34-127">Możesz kupować i sprzedawać rezerwacje platformy Azure oraz zarządzać nimi zarówno w centrum partnerskim, jak i w Azure Portal, a także za pomocą interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="6eb34-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="6eb34-128">Możesz również dać swoim klientom uprawnienia do kupowania własnych rezerwacji platformy Azure z subskrypcji platformy Azure, która została zakupiona.</span><span class="sxs-lookup"><span data-stu-id="6eb34-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="6eb34-129">Skorzystaj z poniższych linków, aby dowiedzieć się, jak.</span><span class="sxs-lookup"><span data-stu-id="6eb34-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="6eb34-130">Zasoby rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="6eb34-130">Azure reservations resources</span></span>

|<span data-ttu-id="6eb34-131">**Aby uzyskać informacje na temat**</span><span class="sxs-lookup"><span data-stu-id="6eb34-131">**For information about**</span></span>   |<span data-ttu-id="6eb34-132">**Przeczytaj to**</span><span class="sxs-lookup"><span data-stu-id="6eb34-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="6eb34-133">Dokumentacja usługi Azure zastrzeżeń dla swoich klientów</span><span class="sxs-lookup"><span data-stu-id="6eb34-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="6eb34-134">Co to są rezerwacje platformy Azure?</span><span class="sxs-lookup"><span data-stu-id="6eb34-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="6eb34-135">Kupowanie rezerwacji platformy Azure dla klientów w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="6eb34-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="6eb34-136">Kupowanie rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="6eb34-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="6eb34-137">Zarządzanie rezerwacjami platformy Azure w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="6eb34-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="6eb34-138">Zarządzanie rezerwacjami platformy Azure w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="6eb34-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="6eb34-139">Określanie prawidłowego rozmiaru maszyny wirtualnej i Sprawdzanie użycia maszyn wirtualnych klienta</span><span class="sxs-lookup"><span data-stu-id="6eb34-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="6eb34-140">Rozmiar maszyny wirtualnej dla maksymalnego użycia zastrzeżenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="6eb34-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="6eb34-141">Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="6eb34-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="6eb34-142">[Zakup Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji dla deweloperów Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="6eb34-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="6eb34-143">Przyznanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure z subskrypcji programu CSP.</span><span class="sxs-lookup"><span data-stu-id="6eb34-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="6eb34-144">Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="6eb34-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |