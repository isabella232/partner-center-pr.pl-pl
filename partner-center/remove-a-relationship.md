---
title: Usuń relację odsprzedawcy z klientem
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, w jaki sposób partnerzy firmy Microsoft mogą usunąć klientów z listy, usunąć uprawnienia administratora delegowanego i zatrzymać obsługę lub kupowanie dla klienta.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 133df7a2e6fdcf9aad48d3937b04dac33c93122a
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549094"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="08632-103">Jak przenieść relację odsprzedawcy z klientem w Centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="08632-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="08632-104">W tym artykule opisano sposób usuwania relacji odsprzedawcy z klientem w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="08632-104">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="08632-105">Bezpośredni partnerzy lub dostawcy pośrednii: Jeśli klient nie jest już transakcyjny, możesz usunąć tę relację w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="08632-105">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="08632-106">Usunięcie relacji ma następujące konsekwencje:</span><span class="sxs-lookup"><span data-stu-id="08632-106">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="08632-107">Usunięcie klienta z listy klientów w Centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="08632-107">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="08632-108">Usuwa użytkownika z [listy dostępnych kontaktów pomocy technicznej](assign-support-contacts.md) dla klienta</span><span class="sxs-lookup"><span data-stu-id="08632-108">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="08632-109">Usunięcie uprawnień administratora delegowania dla klienta</span><span class="sxs-lookup"><span data-stu-id="08632-109">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="08632-110">Uniemożliwienie klientowi dokonywania zakupów w przyszłości</span><span class="sxs-lookup"><span data-stu-id="08632-110">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="08632-111">Jak usunąć relację</span><span class="sxs-lookup"><span data-stu-id="08632-111">How to remove a relationship</span></span>

<span data-ttu-id="08632-112">Aby usunąć relację, należy anulować rezerwacje na platformie Azure, anulować zakupy oprogramowania i najpierw zawiesić wszystkie pozostałe aktywne subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="08632-112">To remove the relationship, you'll need to cancel Azure RI reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="08632-113">**Zawieś wszystkie aktywne subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="08632-113">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="08632-114">W centrum partnerskim przejdź do pozycji **klienci** i wybierz klienta</span><span class="sxs-lookup"><span data-stu-id="08632-114">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="08632-115">W obszarze **subskrypcje** wybierz subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="08632-115">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="08632-116">Wybierz **wstrzymanie**</span><span class="sxs-lookup"><span data-stu-id="08632-116">Select **Suspended**</span></span>

   4. <span data-ttu-id="08632-117">Powtórz te kroki dla każdej aktywnej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="08632-117">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="08632-118">**Usuń relację w centrum partnerskim:**</span><span class="sxs-lookup"><span data-stu-id="08632-118">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="08632-119">a.</span><span class="sxs-lookup"><span data-stu-id="08632-119">a.</span></span> <span data-ttu-id="08632-120">W centrum partnerskim przejdź do pozycji **klienci** i wybierz klienta.</span><span class="sxs-lookup"><span data-stu-id="08632-120">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="08632-121">b.</span><span class="sxs-lookup"><span data-stu-id="08632-121">b.</span></span> <span data-ttu-id="08632-122">Wybierz **konto**.</span><span class="sxs-lookup"><span data-stu-id="08632-122">Select the **Account**.</span></span>

   <span data-ttu-id="08632-123">c.</span><span class="sxs-lookup"><span data-stu-id="08632-123">c.</span></span> <span data-ttu-id="08632-124">Wybierz pozycję **Usuń relację odsprzedawcy**.</span><span class="sxs-lookup"><span data-stu-id="08632-124">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="08632-125">Jeśli wszystkie subskrypcje są nadal aktywne, link **Usuń relację odsprzedawcy** będzie nieaktywny.</span><span class="sxs-lookup"><span data-stu-id="08632-125">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="08632-126">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="08632-126">Next steps</span></span>

- [<span data-ttu-id="08632-127">Żądanie lub ponowne nawiązanie relacji z klientem</span><span class="sxs-lookup"><span data-stu-id="08632-127">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
