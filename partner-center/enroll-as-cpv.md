---
title: Rejestracja jako dostawca panelu sterowania
description: Dowiedz się, jak zarejestrować się jako dostawca panelu sterowania (CPV) w centrum partnerskim, aby lepiej zintegrować systemy partnerskie CSP z interfejsami API Centrum partnerskiego.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560514"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="f9f4c-103">Zarejestruj się jako dostawca panelu sterowania, aby ułatwić integrację systemów partnerskich programu CSP z interfejsami API Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="f9f4c-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="f9f4c-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="f9f4c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f9f4c-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="f9f4c-105">Global admin</span></span>

<span data-ttu-id="f9f4c-106">Dostawca panelu sterowania (CPV) to niezależny dostawca oprogramowania, który opracowuje aplikacje do użycia przez partnerów dostawcy rozwiązań w chmurze (CSP), aby umożliwić im integrację systemów z interfejsem API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="f9f4c-107">Dostawca panelu sterowania nie jest partnerem dostawcy usług kryptograficznych, który ma bezpośredni dostęp do pulpitu nawigacyjnego Centrum partnerskiego lub interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="f9f4c-108">Bez względu na to, czy jesteś bieżącym dostawcą (CPV), czy nowym CPV, który chce współpracować z partnerami firmy Microsoft, firma Microsoft wymaga, aby zarejestrować się w centrum partnerskim w celu zarejestrowania aplikacji i obsługi partnerów dostawcy rozwiązań w chmurze.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="f9f4c-109">Aby utworzyć konto, partner CPV może użyć istniejącej dzierżawcy partnera CSP lub istniejącej dzierżawy CPV lub utworzyć nową dzierżawę jako część procesu dołączania.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="f9f4c-110">Jeśli partner CPV zdecyduje się na korzystanie z istniejącej dzierżawy CSP, należy utworzyć osobne aplikacje wielodostępne i zarejestrować je w centrum partnerskim dla działań CPV.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="f9f4c-111">Nie można zarejestrować aplikacji jako dostawcy usług kryptograficznych i CPV.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="f9f4c-112">Po zarejestrowaniu się w centrum partnerskim i zarejestrowaniu aplikacji będziesz mieć dostęp do interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="f9f4c-113">Jeśli potrzebujesz konta piaskownicy, skontaktuj się z firmą Microsoft za pomocą żądania pomoc techniczna firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="f9f4c-114">Jeśli masz już konto piaskownicy, Kontynuuj korzystanie z niego.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="f9f4c-115">Nie będziesz potrzebować nowej piaskownicy</span><span class="sxs-lookup"><span data-stu-id="f9f4c-115">You won't need a new sandbox</span></span>

<span data-ttu-id="f9f4c-116">Przejrzyj [umowę dostawcy panelu sterowania firmy Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="f9f4c-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="f9f4c-117">Praca w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="f9f4c-117">Working in Partner Center</span></span>

<span data-ttu-id="f9f4c-118">Po zarejestrowaniu się w doświadczeniu w centrum partnerskim i zaakceptowaniu umowy CPV można:</span><span class="sxs-lookup"><span data-stu-id="f9f4c-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="f9f4c-119">Zarządzanie aplikacjami wielodostępnymi (Dodawanie aplikacji do Azure Portal, rejestrowanie i wyrejestrowywanie aplikacji w centrum partnerskim).</span><span class="sxs-lookup"><span data-stu-id="f9f4c-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="f9f4c-120">CPVs muszą zarejestrować swoje aplikacje w centrum partnerskim, aby uzyskać autoryzację dla interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="f9f4c-121">Dodawanie aplikacji do Azure Portal samej nie powoduje autoryzacji aplikacji CPV dla interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="f9f4c-122">Wyświetl swój profil CPV i Zarządzaj nim</span><span class="sxs-lookup"><span data-stu-id="f9f4c-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="f9f4c-123">Wyświetlaj użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzaj nimi.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="f9f4c-124">Administrator globalny jest jedyną rolą, którą może mieć element CPV.</span><span class="sxs-lookup"><span data-stu-id="f9f4c-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9f4c-125">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="f9f4c-125">Next steps</span></span>

<span data-ttu-id="f9f4c-126">-[Dodawanie dodatkowych dzierżawców do konta Centrum partnerskiego](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="f9f4c-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>