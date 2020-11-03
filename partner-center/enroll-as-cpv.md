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
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530387"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="f5cd4-103">Zarejestruj się jako dostawca panelu sterowania, aby ułatwić integrację systemów partnerskich programu CSP z interfejsami API Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="f5cd4-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="f5cd4-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="f5cd4-104">**Applies to**</span></span>

- <span data-ttu-id="f5cd4-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="f5cd4-105">Partner Center</span></span>

<span data-ttu-id="f5cd4-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="f5cd4-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f5cd4-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="f5cd4-107">Global admin</span></span>

<span data-ttu-id="f5cd4-108">Dostawca panelu sterowania (CPV) to niezależny dostawca oprogramowania, który opracowuje aplikacje do użycia przez partnerów dostawcy rozwiązań w chmurze (CSP), aby umożliwić im integrację systemów z interfejsem API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="f5cd4-109">Dostawca panelu sterowania nie jest partnerem dostawcy usług kryptograficznych, który ma bezpośredni dostęp do pulpitu nawigacyjnego Centrum partnerskiego lub interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="f5cd4-110">Bez względu na to, czy jesteś bieżącym dostawcą (CPV), czy nowym CPV, który chce współpracować z partnerami firmy Microsoft, firma Microsoft wymaga, aby zarejestrować się w centrum partnerskim w celu zarejestrowania aplikacji i obsługi partnerów dostawcy rozwiązań w chmurze.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="f5cd4-111">Aby utworzyć konto, partner CPV może użyć istniejącej dzierżawcy partnera CSP lub istniejącej dzierżawy CPV lub utworzyć nową dzierżawę jako część procesu dołączania.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="f5cd4-112">Jeśli partner CPV zdecyduje się na korzystanie z istniejącej dzierżawy CSP, należy utworzyć osobne aplikacje wielodostępne i zarejestrować je w centrum partnerskim dla działań CPV.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="f5cd4-113">Nie można zarejestrować aplikacji jako dostawcy usług kryptograficznych i CPV.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="f5cd4-114">Po zarejestrowaniu się w centrum partnerskim i zarejestrowaniu aplikacji będziesz mieć dostęp do interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="f5cd4-115">Firma Microsoft skontaktuje się z Tobą za pośrednictwem powiadomienia Centrum partnerskiego z informacjami w piaskownicy.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="f5cd4-116">Jeśli masz już konto piaskownicy, Kontynuuj korzystanie z niego.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="f5cd4-117">Nie będziesz potrzebować nowej piaskownicy.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="f5cd4-118">Przejrzyj [umowę dostawcy panelu sterowania firmy Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="f5cd4-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="f5cd4-119">Praca w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="f5cd4-119">Working in Partner Center</span></span>
<span data-ttu-id="f5cd4-120">Po zarejestrowaniu się w doświadczeniu w centrum partnerskim i zaakceptowaniu umowy CPV można:</span><span class="sxs-lookup"><span data-stu-id="f5cd4-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="f5cd4-121">Zarządzanie aplikacjami wielodostępnymi (Dodawanie aplikacji do Azure Portal, rejestrowanie i wyrejestrowywanie aplikacji w centrum partnerskim).</span><span class="sxs-lookup"><span data-stu-id="f5cd4-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="f5cd4-122">CPVs muszą zarejestrować swoje aplikacje w centrum partnerskim, aby uzyskać autoryzację dla interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="f5cd4-123">Dodawanie aplikacji do Azure Portal samej nie powoduje autoryzacji aplikacji CPV dla interfejsów API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="f5cd4-124">Wyświetl swój profil CPV i Zarządzaj nim</span><span class="sxs-lookup"><span data-stu-id="f5cd4-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="f5cd4-125">Wyświetlaj użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzaj nimi.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="f5cd4-126">Administrator globalny jest jedyną rolą, którą może mieć element CPV.</span><span class="sxs-lookup"><span data-stu-id="f5cd4-126">Global admin is the only role a CPV can have.</span></span>


