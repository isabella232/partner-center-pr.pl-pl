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
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529913"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="9bb89-104">Sprzedawaj Microsoft Azure rezerwacje klientom przy użyciu Centrum partnerskiego, Azure Portal lub interfejsów API</span><span class="sxs-lookup"><span data-stu-id="9bb89-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="9bb89-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="9bb89-105">**Applies to**</span></span>

- <span data-ttu-id="9bb89-106">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="9bb89-106">Partner Center</span></span>
- <span data-ttu-id="9bb89-107">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="9bb89-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="9bb89-108">Partnerzy w programie CSP</span><span class="sxs-lookup"><span data-stu-id="9bb89-108">Partners in the CSP program</span></span>

<span data-ttu-id="9bb89-109">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="9bb89-109">**Appropriate roles**</span></span>

- <span data-ttu-id="9bb89-110">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="9bb89-110">Admin agent</span></span>
- <span data-ttu-id="9bb89-111">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="9bb89-111">Global admin</span></span>
- <span data-ttu-id="9bb89-112">Agent pomocy technicznej</span><span class="sxs-lookup"><span data-stu-id="9bb89-112">Helpdesk agent</span></span>
- <span data-ttu-id="9bb89-113">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="9bb89-113">Sales agent</span></span>
- <span data-ttu-id="9bb89-114">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="9bb89-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="9bb89-115">Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="9bb89-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="9bb89-116">Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="9bb89-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="9bb89-117">Partnerzy w programie CSP mogą zaoferować swoim klientom Microsoft Azure rezerwacje.</span><span class="sxs-lookup"><span data-stu-id="9bb89-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="9bb89-118">Klienci mogą uzyskać znaczne oszczędności w przypadku zarezerwowania z wyprzedzeniem.</span><span class="sxs-lookup"><span data-stu-id="9bb89-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="9bb89-119">Rezerwacje platformy Azure oferują klientom prostotę i elastyczność w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="9bb89-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="9bb89-120">Jednoroczne warunki rezerwacji</span><span class="sxs-lookup"><span data-stu-id="9bb89-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="9bb89-121">Łatwe rozpoczęcie pracy; Instalacja zakończona w sekundach</span><span class="sxs-lookup"><span data-stu-id="9bb89-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="9bb89-122">Anuluj lub Zarezerwuj wystąpienia w dowolnym momencie w celu skorygowania zwrotu</span><span class="sxs-lookup"><span data-stu-id="9bb89-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="9bb89-123">Zarządzanie użyciem wystąpień zarezerwowanych na poziomie organizacji lub poszczególnych działów</span><span class="sxs-lookup"><span data-stu-id="9bb89-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="9bb89-124">Rezerwacje platformy Azure mogą odwoływać się do klientów w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="9bb89-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="9bb89-125">Rezerwacje mogą oferować znaczne oszczędności w porównaniu z cennikiem płatność zgodnie z rzeczywistym użyciem</span><span class="sxs-lookup"><span data-stu-id="9bb89-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="9bb89-126">Lepsze budżetowanie i prognozowanie przy użyciu płatności z góry za rok lub trzy lata</span><span class="sxs-lookup"><span data-stu-id="9bb89-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="9bb89-127">Priorytetowe zdolności obliczeniowe w regionie świadczenia usługi Azure najbliżej ich biur</span><span class="sxs-lookup"><span data-stu-id="9bb89-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="9bb89-128">Rezerwacje platformy Azure stanowią podstawę kompleksowych rozwiązań infrastruktury w połączeniu z oprogramowaniem takim jak Microsoft Windows Server i Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="9bb89-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="9bb89-129">Możesz kupować i sprzedawać rezerwacje platformy Azure oraz zarządzać nimi zarówno w centrum partnerskim, jak i w Azure Portal, a także za pomocą interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="9bb89-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="9bb89-130">Możesz również dać swoim klientom uprawnienia do kupowania własnych rezerwacji platformy Azure z subskrypcji platformy Azure, która została zakupiona.</span><span class="sxs-lookup"><span data-stu-id="9bb89-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="9bb89-131">Skorzystaj z poniższych linków, aby dowiedzieć się, jak.</span><span class="sxs-lookup"><span data-stu-id="9bb89-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="9bb89-132">Zasoby rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9bb89-132">Azure reservations resources</span></span>

|<span data-ttu-id="9bb89-133">**Aby uzyskać informacje na temat**</span><span class="sxs-lookup"><span data-stu-id="9bb89-133">**For information about**</span></span>   |<span data-ttu-id="9bb89-134">**Przeczytaj to**</span><span class="sxs-lookup"><span data-stu-id="9bb89-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="9bb89-135">Dokumentacja usługi Azure zastrzeżeń dla swoich klientów</span><span class="sxs-lookup"><span data-stu-id="9bb89-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="9bb89-136">Co to są rezerwacje platformy Azure?</span><span class="sxs-lookup"><span data-stu-id="9bb89-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="9bb89-137">Kupowanie rezerwacji platformy Azure dla klientów w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="9bb89-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="9bb89-138">Kupowanie rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9bb89-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="9bb89-139">Zarządzanie rezerwacjami platformy Azure w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="9bb89-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="9bb89-140">Zarządzanie rezerwacjami platformy Azure w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="9bb89-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="9bb89-141">Określanie prawidłowego rozmiaru maszyny wirtualnej i Sprawdzanie użycia maszyn wirtualnych klienta</span><span class="sxs-lookup"><span data-stu-id="9bb89-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="9bb89-142">Rozmiar maszyny wirtualnej dla maksymalnego użycia zastrzeżenia platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9bb89-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="9bb89-143">Kupowanie rezerwacji platformy Azure przy użyciu interfejsu API Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9bb89-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="9bb89-144">[Zakup Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) w dokumentacji dla deweloperów Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="9bb89-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="9bb89-145">Przyznanie klientom uprawnień do zakupu własnych rezerwacji platformy Azure z subskrypcji programu CSP.</span><span class="sxs-lookup"><span data-stu-id="9bb89-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="9bb89-146">Przyznaj klientom uprawnienia do kupowania własnych rezerwacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="9bb89-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |