---
title: Nazwa główna usługi Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodać jednostkę usługi do dzierżawy usługi Azure AD. Oznacza to dodanie aplikacji usługi Azure AD (nazwy głównej usługi) w centrum partnerskim.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028472"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="acbb6-104">Dodawanie aplikacji usługi Azure AD (nazwy głównej usługi) w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="acbb6-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="acbb6-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="acbb6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="acbb6-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="acbb6-106">Global admin</span></span>

<span data-ttu-id="acbb6-107">W programie komercyjnym Marketplace w centrum partnerskim możesz teraz dodać aplikację usługi Azure AD (nazwę główną usługi) jako użytkownika na koncie Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="acbb6-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="acbb6-108">(Wcześniej można było to zrobić w portal Cloud Partner lub CPP.</span><span class="sxs-lookup"><span data-stu-id="acbb6-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="acbb6-109">Teraz, gdy przeprowadzono migrację do Centrum partnerskiego, konto CPP jest tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="acbb6-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="acbb6-110">Nazwa główna usługi jest równoznaczna z aplikacją usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="acbb6-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="acbb6-111">Dodawanie aplikacji usługi Azure AD (nazwy głównej usługi)</span><span class="sxs-lookup"><span data-stu-id="acbb6-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="acbb6-112">Na pulpicie nawigacyjnym Centrum partnerskiego wybierz pozycję **Ustawienia** , a następnie wybierz pozycję **Ustawienia dewelopera**.</span><span class="sxs-lookup"><span data-stu-id="acbb6-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="acbb6-113">Wybierz pozycję **Użytkownicy** , a następnie wybierz pozycję **Dodaj aplikacje usługi Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="acbb6-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="acbb6-114">Wybierz istniejącą aplikację usługi Azure AD lub Utwórz nową.</span><span class="sxs-lookup"><span data-stu-id="acbb6-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="acbb6-115">Jeśli tworzysz nową aplikację usługi Azure AD, uwzględnij następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="acbb6-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="acbb6-116">**Adres URL odpowiedzi**: adres URL, pod którym użytkownicy mogą się logować, aby korzystać z aplikacji usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="acbb6-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="acbb6-117">**Identyfikator URI aplikacji**: Identyfikator logiczny dla aplikacji usługi Azure AD, który jest prezentowany podczas wysyłania żądania logowania jednokrotnego do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="acbb6-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="acbb6-118">**Role zabezpieczeń**: **Menedżer** ról (taki sam jak rola "właściciel" w programie CPP) i **deweloper** (taka sama jak rola "Współautor" w programie CPP) ma zastosowanie do komercyjnego programu Marketplace w centrum partnerskim i można je SKOJARZYĆ z tą aplikacją usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="acbb6-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="acbb6-119">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="acbb6-119">Next steps</span></span>

- [<span data-ttu-id="acbb6-120">Omówienie portalu komercyjnego w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="acbb6-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)