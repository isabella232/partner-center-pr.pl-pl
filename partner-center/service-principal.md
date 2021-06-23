---
title: Jednostkę usługi Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodać jednostkę usługi do dzierżawy usługi Azure AD. Oznacza to dodanie aplikacji usługi Azure AD (jednostki usługi) w Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551558"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="2a833-104">Dodawanie aplikacji usługi Azure AD (jednostki usługi) w usłudze Partner Center</span><span class="sxs-lookup"><span data-stu-id="2a833-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="2a833-105">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="2a833-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="2a833-106">W programie komercyjnej platformy handlowej w usłudze Partner Center możesz teraz dodać aplikację usługi Microsoft Azure Active Directory (Azure AD) (jednostkę usługi) jako użytkownika na Partner Center konta.</span><span class="sxs-lookup"><span data-stu-id="2a833-106">In the Commercial Marketplace program in Partner Center, you are now able to add a Microsoft Azure Active Directory (Azure AD) application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="2a833-107">(Wcześniej można było to zrobić na koncie Cloud Partner Portal (CPP).</span><span class="sxs-lookup"><span data-stu-id="2a833-107">(You were able to do so previously in your Cloud Partner Portal (CPP) account.</span></span> <span data-ttu-id="2a833-108">Teraz, po migracji do Partner Center, konto CPP jest tylko do odczytu).</span><span class="sxs-lookup"><span data-stu-id="2a833-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="2a833-109">Jednostkę usługi należy do aplikacji usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2a833-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="2a833-110">Dodawanie aplikacji usługi Azure AD (jednostki usługi)</span><span class="sxs-lookup"><span data-stu-id="2a833-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="2a833-111">Na pulpicie Partner Center nawigacyjnym wybierz pozycję **Ustawienia,** a następnie pozycję **Ustawienia dewelopera.**</span><span class="sxs-lookup"><span data-stu-id="2a833-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="2a833-112">Wybierz **pozycję Użytkownicy,** a następnie **wybierz pozycję Dodaj aplikacje usługi Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="2a833-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="2a833-113">Wybierz istniejącą aplikację usługi Azure AD lub utwórz nową.</span><span class="sxs-lookup"><span data-stu-id="2a833-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="2a833-114">Jeśli tworzysz nową aplikację usługi Azure AD, dołącz następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="2a833-114">If you create a new Azure AD application, include the following information:</span></span>  

   - <span data-ttu-id="2a833-115">**Adres URL odpowiedzi:** adres URL, pod którym użytkownicy mogą logować się w celu korzystania z aplikacji usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2a833-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="2a833-116">**Identyfikator URI identyfikatora aplikacji:** identyfikator logiczny aplikacji usługi Azure AD, który jest prezentowany podczas wysyłanie żądania logowania pojedynczego do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2a833-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="2a833-117">**Role zabezpieczeń:** Role Menedżer **(taki** sam jak rola "Właściciel" w programie CPP) i Deweloper **(takie** same jak rola "Współautor" w programie CPP) mają zastosowanie do programu komercyjnej platformy handlowej w programie Partner Center i można je skojarzyć z tą aplikacją usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2a833-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="2a833-118">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="2a833-118">Next steps</span></span>

- [<span data-ttu-id="2a833-119">Omówienie platformy handlowej w Partner Center</span><span class="sxs-lookup"><span data-stu-id="2a833-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)