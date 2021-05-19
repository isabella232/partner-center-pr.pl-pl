---
title: Rejestrowanie jako Panel sterowania dostawcy
description: Dowiedz się, jak zarejestrować się jako dostawca Panel sterowania (CPV) w u Partner Center, aby lepiej zintegrować systemy partnerskie programu CSP z Partner Center API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147143"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="32841-103">Zarejestruj się jako dostawca Panel sterowania, aby pomóc w integracji systemów partnerów programu CSP z Partner Center API</span><span class="sxs-lookup"><span data-stu-id="32841-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="32841-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="32841-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="32841-105">Dostawca Panel sterowania (CPV) to niezależny dostawca oprogramowania, który opracowuje aplikacje do użycia przez partnerów programu Dostawca rozwiązań w chmurze (CSP) w celu umożliwienia im integracji systemów z Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="32841-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="32841-106">Dostawca Panel sterowania nie jest partnerem CSP z bezpośrednim dostępem do pulpitu nawigacyjnego Partner Center lub Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="32841-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="32841-107">Niezależnie od tego, czy jesteś bieżącym dostawcą usługi Panel sterowania (CPV), czy też nowym dostawcą CPV, który chce współpracować z partnerami firmy Microsoft, firma Microsoft wymaga teraz zarejestrowania się w programie Partner Center w celu zarejestrowania aplikacji i pomocy technicznej Dostawca rozwiązań w chmurze partnerów.</span><span class="sxs-lookup"><span data-stu-id="32841-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="32841-108">Aby utworzyć konto, partner CPV może użyć istniejącej dzierżawy partnera CSP lub istniejącej dzierżawy CPV albo utworzyć nową dzierżawę w ramach procesu dołączania.</span><span class="sxs-lookup"><span data-stu-id="32841-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="32841-109">Jeśli partner CPV zdecyduje się na użycie istniejącej dzierżawy CSP, będzie musiał utworzyć oddzielne aplikacje wielodostępne i zarejestrować je w Partner Center dla działań CPV.</span><span class="sxs-lookup"><span data-stu-id="32841-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="32841-110">Aplikacji nie można zarejestrować zarówno jako aplikacji CSP, jak i CPV.</span><span class="sxs-lookup"><span data-stu-id="32841-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="32841-111">Po zarejestrowaniu w usłudze Partner Center i zarejestrowaniu aplikacji będziesz mieć dostęp do tych Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="32841-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="32841-112">Jeśli potrzebujesz konta piaskownicy, skontaktuj się z firmą Microsoft za pośrednictwem Pomoc techniczna Microsoft aplikacji.</span><span class="sxs-lookup"><span data-stu-id="32841-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="32841-113">Jeśli masz już konto piaskownicy, kontynuuj korzystanie z niego.</span><span class="sxs-lookup"><span data-stu-id="32841-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="32841-114">Nowa piaskownica nie będzie potrzebna</span><span class="sxs-lookup"><span data-stu-id="32841-114">You won't need a new sandbox</span></span>

<span data-ttu-id="32841-115">Zapoznaj się z [umową Panel sterowania microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="32841-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="32841-116">Praca w Partner Center</span><span class="sxs-lookup"><span data-stu-id="32841-116">Working in Partner Center</span></span>

<span data-ttu-id="32841-117">Po zarejestrowaniu się w Partner Center CPV i zaakceptowaniu umowy CPV można:</span><span class="sxs-lookup"><span data-stu-id="32841-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="32841-118">Zarządzanie aplikacjami wielodostępnych (dodawanie aplikacji do Azure Portal, rejestrowanie i wyrejestrowywuje aplikacje w Partner Center).</span><span class="sxs-lookup"><span data-stu-id="32841-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="32841-119">Procesory CPV muszą zarejestrować swoje aplikacje w Partner Center, aby uzyskać autoryzację dla Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="32841-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="32841-120">Dodawanie aplikacji tylko do Azure Portal nie powoduje autoryzowania aplikacji CPV dla Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="32841-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="32841-121">Wyświetlanie profilu CPV i zarządzanie tym profilem</span><span class="sxs-lookup"><span data-stu-id="32841-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="32841-122">Wyświetlanie użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzanie nimi.</span><span class="sxs-lookup"><span data-stu-id="32841-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="32841-123">Administrator globalny jest jedyną rolą, jaką może mieć protokół CPV.</span><span class="sxs-lookup"><span data-stu-id="32841-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="32841-124">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="32841-124">Next steps</span></span>

<span data-ttu-id="32841-125">-[Dodawanie kolejnych dzierżaw do konta Partner Center dzierżawy](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="32841-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>