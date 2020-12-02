---
title: Przypisywanie subskrypcji platformy Azure do klientów
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przypisać subskrypcje platformy Azure klientom w centrum partnerskim i jak umożliwić klientom zarządzanie własnymi subskrypcjami.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473955"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="97522-103">Przypisywanie subskrypcji platformy Azure klientom w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="97522-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="97522-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="97522-104">**Appropriate roles**</span></span>

- <span data-ttu-id="97522-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="97522-105">Global admin</span></span>
- <span data-ttu-id="97522-106">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="97522-106">Sales agent</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="97522-107">Przypisywanie subskrypcji platformy Azure do klientów</span><span class="sxs-lookup"><span data-stu-id="97522-107">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="97522-108">Wybierz pozycję **klienci** z menu **Centrum partnerskiego** i Znajdź klienta, którym chcesz zarządzać.</span><span class="sxs-lookup"><span data-stu-id="97522-108">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="97522-109">Wybierz strzałkę w dół na końcu wiersza, aby rozwinąć rekord klienta, a następnie wybierz pozycję **Portal zarządzania Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="97522-109">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="97522-110">Nastąpi przekierowanie do [Azure Portal](https://portal.azure.com/) , w którym można zarządzać subskrypcjami klienta.</span><span class="sxs-lookup"><span data-stu-id="97522-110">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="97522-111">W Azure Portal wybierz pozycję **subskrypcje**.</span><span class="sxs-lookup"><span data-stu-id="97522-111">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="97522-112">Wybierz subskrypcję, którą chcesz przypisać, a następnie wybierz pozycję **Access Control**.</span><span class="sxs-lookup"><span data-stu-id="97522-112">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="97522-113">Wybierz pozycję **Dodaj** , aby dodać użytkownika do subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="97522-113">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="97522-114">Po dodaniu użytkownika do subskrypcji można przypisać użytkownikowi rolę i określone konto, do którego użytkownik będzie miał dostęp.</span><span class="sxs-lookup"><span data-stu-id="97522-114">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="97522-115">Umożliwienie klientom zarządzania swoimi subskrypcjami platformy Azure</span><span class="sxs-lookup"><span data-stu-id="97522-115">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="97522-116">Po utworzeniu subskrypcji Microsoft Azure dla klienta można umożliwić im Zarządzanie subskrypcją.</span><span class="sxs-lookup"><span data-stu-id="97522-116">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="97522-117">Aby to zrobić, należy zalogować się do portalu zarządzania Microsoft Azure klienta.</span><span class="sxs-lookup"><span data-stu-id="97522-117">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="97522-118">Aby otworzyć Azure Portal klienta, rozwiń listę klientów na liście klientów lub wybierz nazwę klienta, a następnie wybierz pozycję **Portal zarządzania Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="97522-118">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="97522-119">Jeśli zostanie wyświetlony monit o zalogowanie się do Azure Portal, użytkownik nie może mieć delegowanych uprawnień administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="97522-119">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="97522-120">Wybierz pozycję **Żądaj relacji** , aby zaprosić klienta do identyfikacji użytkownika jako partnera rekordu.</span><span class="sxs-lookup"><span data-stu-id="97522-120">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="97522-121">Po zaakceptowaniu zaproszenia przez klienta zostaną automatycznie przyznane delegowane uprawnienia administracyjne.</span><span class="sxs-lookup"><span data-stu-id="97522-121">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="97522-122">W Azure Portal Otwórz listę subskrypcje klienta i wybierz subskrypcję platformy Azure klienta.</span><span class="sxs-lookup"><span data-stu-id="97522-122">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="97522-123">Przypisz rolę wszystkim użytkownikom klienta, aby mogli tworzyć zasoby w ramach ich subskrypcji i zarządzać nimi.</span><span class="sxs-lookup"><span data-stu-id="97522-123">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="97522-124">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="97522-124">Next steps</span></span>

- [<span data-ttu-id="97522-125">Jak partnerzy CSP mogą sprzedawać subskrypcje klientom</span><span class="sxs-lookup"><span data-stu-id="97522-125">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="97522-126">Jak uzyskać uprawnienia do zarządzania usługą lub subskrypcjami klienta</span><span class="sxs-lookup"><span data-stu-id="97522-126">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
