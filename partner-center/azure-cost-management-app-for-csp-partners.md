---
title: Azure Cost Management według Cloudyn dla dostawców CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak zarejestrować aplikację sieci Web Cloudyn i użyć klucza tajnego w centrum partnerskim, aby można było używać aplikacji do śledzenia użycia i kosztów platformy Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529269"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="8eb45-103">Śledzenie użycia i kosztów platformy Azure za pomocą aplikacji Azure Cost Management dla partnerów CSP</span><span class="sxs-lookup"><span data-stu-id="8eb45-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="8eb45-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="8eb45-104">**Applies to**</span></span>

- <span data-ttu-id="8eb45-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="8eb45-105">Partner Center</span></span>
- <span data-ttu-id="8eb45-106">Partnerzy programu dla dostawców rozwiązań w chmurze</span><span class="sxs-lookup"><span data-stu-id="8eb45-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="8eb45-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="8eb45-107">**Appropriate roles**</span></span>

- <span data-ttu-id="8eb45-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="8eb45-108">Global admin</span></span>
- <span data-ttu-id="8eb45-109">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="8eb45-109">Admin agent</span></span>

[<span data-ttu-id="8eb45-110">Uzyskaj więcej informacji na temat Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="8eb45-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="8eb45-111">Przed rozpoczęciem</span><span class="sxs-lookup"><span data-stu-id="8eb45-111">Before you begin</span></span>
<span data-ttu-id="8eb45-112">Przed rozpoczęciem korzystania z Azure Cost Management upewnij się, że spełniasz następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="8eb45-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="8eb45-113">Jesteś partnerem w programie dostawcy rozwiązań w chmurze.</span><span class="sxs-lookup"><span data-stu-id="8eb45-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="8eb45-114">Można utworzyć aplikację internetową interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="8eb45-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="8eb45-115">Omówienie</span><span class="sxs-lookup"><span data-stu-id="8eb45-115">Overview</span></span>

<span data-ttu-id="8eb45-116">Cloudyn to aplikacja internetowa, która umożliwia śledzenie i zarządzanie ilością klientów korzystających z platformy Azure oraz kosztami tego użycia.</span><span class="sxs-lookup"><span data-stu-id="8eb45-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="8eb45-117">Jest on używany za pomocą interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="8eb45-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="8eb45-118">Zarejestruj swoją aplikację sieci Web w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="8eb45-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="8eb45-119">Po zarejestrowaniu aplikacji internetowej Azure Active Directory w centrum partnerskim zostanie włączony dostęp do interfejsu API Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="8eb45-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="8eb45-120">Zaloguj się do [Centrum partnerskiego](https://partnercenter.microsoft.com/pcv/dashboard/overview) przy użyciu [konta administratora globalnego lub agenta administratora](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="8eb45-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="8eb45-121">W **centrum partnerskim** wybierz pozycję **Ustawienia konta** &gt; **[Zarządzanie aplikacjami](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="8eb45-121">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="8eb45-122">W sekcji **aplikacja sieci Web** kliknij pozycję **Dodaj nową aplikację sieci Web**.</span><span class="sxs-lookup"><span data-stu-id="8eb45-122">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="8eb45-123">**Uwaga**: Jeśli wcześniej utworzono aplikację sieci Web, możesz pominąć krok 3.</span><span class="sxs-lookup"><span data-stu-id="8eb45-123">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="8eb45-124">Skopiuj i Zapisz identyfikator GUID **identyfikatora** i **Identyfikator aplikacji** dla aplikacji sieci Web.</span><span class="sxs-lookup"><span data-stu-id="8eb45-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="8eb45-125">Do korzystania z 30-dniowej bezpłatnej wersji próbnej aplikacji Azure Cost Management wymagane są oba identyfikatory.</span><span class="sxs-lookup"><span data-stu-id="8eb45-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="8eb45-126">Dodawanie klucza tajnego do aplikacji</span><span class="sxs-lookup"><span data-stu-id="8eb45-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="8eb45-127">Na liście rozwijanej obok przycisku **Dodaj klucz** wybierz czas trwania wynoszący 1 lub 2 lata.</span><span class="sxs-lookup"><span data-stu-id="8eb45-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="8eb45-128">Kliknij przycisk **Dodaj klucz**.</span><span class="sxs-lookup"><span data-stu-id="8eb45-128">Click **Add key**.</span></span> 
3. <span data-ttu-id="8eb45-129">Skopiuj i Zapisz wartość klucza tajnego.</span><span class="sxs-lookup"><span data-stu-id="8eb45-129">Copy and save the secret key value.</span></span> <span data-ttu-id="8eb45-130">Będzie to konieczne w przypadku 30-dniowej bezpłatnej wersji próbnej.</span><span class="sxs-lookup"><span data-stu-id="8eb45-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="8eb45-131">Klucze tajne aplikacji są podobne do haseł z dłuższymi datami ważności.</span><span class="sxs-lookup"><span data-stu-id="8eb45-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="8eb45-132">Zapisz wartość klucza w bezpiecznej lokalizacji do użycia w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="8eb45-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8eb45-133">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="8eb45-133">Next steps</span></span>
<span data-ttu-id="8eb45-134">Rozpocznij [30-dniową bezpłatną wersję próbną](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="8eb45-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="8eb45-135">Aby rozpocząć okres próbny, potrzebne są następujące szczegóły:</span><span class="sxs-lookup"><span data-stu-id="8eb45-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="8eb45-136">Poświadczenia logowania do Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="8eb45-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="8eb45-137">Identyfikator GUID identyfikatora Commerce</span><span class="sxs-lookup"><span data-stu-id="8eb45-137">Commerce ID GUID</span></span>
- <span data-ttu-id="8eb45-138">Identyfikator GUID identyfikatora aplikacji</span><span class="sxs-lookup"><span data-stu-id="8eb45-138">App ID GUID</span></span>
- <span data-ttu-id="8eb45-139">Wartość klucza tajnego aplikacji</span><span class="sxs-lookup"><span data-stu-id="8eb45-139">Application secret key value</span></span>
