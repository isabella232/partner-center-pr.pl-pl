---
title: Usuwanie relacji odsprzedawcy z klientem
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak bezpośredni partnerzy firmy Microsoft mogą usuwać klientów z listy, usuwać delegowane uprawnienia administratora i przestać wspierać lub kupować dla klienta.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551473"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="e6c5a-103">Jak przenieść relację odsprzedawcy z klientem w Centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="e6c5a-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="e6c5a-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="e6c5a-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e6c5a-105">W tym artykule opisano sposób usuwania relacji odsprzedawcy z klientem w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="e6c5a-106">Bezpośredni partnerzy lub dostawcy pośredni: jeśli nie masz już transakcji z klientem, możesz usunąć relację w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="e6c5a-107">Usunięcie relacji ma następujące konsekwencje:</span><span class="sxs-lookup"><span data-stu-id="e6c5a-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="e6c5a-108">Usunięcie klienta z listy klientów w Centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="e6c5a-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="e6c5a-109">Usuwa Użytkownika z listy [dostępnych kontaktów pomocy technicznej](assign-support-contacts.md) dla klienta</span><span class="sxs-lookup"><span data-stu-id="e6c5a-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="e6c5a-110">Usunięcie uprawnień administratora delegowania dla klienta</span><span class="sxs-lookup"><span data-stu-id="e6c5a-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="e6c5a-111">Uniemożliwienie klientowi dokonywania zakupów w przyszłości</span><span class="sxs-lookup"><span data-stu-id="e6c5a-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="e6c5a-112">Jak usunąć relację</span><span class="sxs-lookup"><span data-stu-id="e6c5a-112">How to remove a relationship</span></span>

<span data-ttu-id="e6c5a-113">Aby usunąć relację, musisz najpierw anulować rezerwacje wystąpień zarezerwowanych platformy Azure, anulować zakupy oprogramowania i wstrzymać wszystkie pozostałe aktywne subskrypcje.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="e6c5a-114">**Wstrzymaj wszystkie aktywne subskrypcje.**</span><span class="sxs-lookup"><span data-stu-id="e6c5a-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="e6c5a-115">Z Partner Center przejdź do strony **Klienci** i wybierz klienta</span><span class="sxs-lookup"><span data-stu-id="e6c5a-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="e6c5a-116">W **obszarze Subskrypcje** wybierz subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="e6c5a-117">Wybierz pozycję **Wstrzymano**</span><span class="sxs-lookup"><span data-stu-id="e6c5a-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="e6c5a-118">Powtórz te kroki dla każdej aktywnej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="e6c5a-119">**Usuń relację z Partner Center:**</span><span class="sxs-lookup"><span data-stu-id="e6c5a-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="e6c5a-120">a.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-120">a.</span></span> <span data-ttu-id="e6c5a-121">Z Partner Center wybierz pozycję **Klienci** i wybierz klienta.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="e6c5a-122">b.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-122">b.</span></span> <span data-ttu-id="e6c5a-123">Wybierz **konto**.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-123">Select the **Account**.</span></span>

   <span data-ttu-id="e6c5a-124">c.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-124">c.</span></span> <span data-ttu-id="e6c5a-125">Wybierz **pozycję Usuń relację odsprzedawcy.**</span><span class="sxs-lookup"><span data-stu-id="e6c5a-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="e6c5a-126">Jeśli jakiekolwiek subskrypcje są nadal aktywne, link **Usuń relację** odsprzedawcy będzie nieaktywny.</span><span class="sxs-lookup"><span data-stu-id="e6c5a-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e6c5a-127">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="e6c5a-127">Next steps</span></span>

- [<span data-ttu-id="e6c5a-128">Żądanie lub ponowne ustanowienie relacji z klientem</span><span class="sxs-lookup"><span data-stu-id="e6c5a-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
