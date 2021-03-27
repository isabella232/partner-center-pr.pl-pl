---
title: Zainstaluj usługę Partner Center Analytics dla Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wykonaj kroki opisane w tym artykule, aby zainstalować i wyświetlić podgląd aplikacji analizy Centrum partnerskiego dla Power BI (dla partnerów bezpośrednich w dostawcy CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633696"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="06ef0-103">Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="06ef0-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="06ef0-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="06ef0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="06ef0-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="06ef0-105">Global admin</span></span>
- <span data-ttu-id="06ef0-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="06ef0-106">User management admin</span></span>
- <span data-ttu-id="06ef0-107">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="06ef0-107">Sales agent</span></span>
- <span data-ttu-id="06ef0-108">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="06ef0-108">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="06ef0-109">Zanim rozpoczniesz</span><span class="sxs-lookup"><span data-stu-id="06ef0-109">Before you begin</span></span>

<span data-ttu-id="06ef0-110">Wybierz aplikację, która jest najbardziej odpowiednia dla Twojej firmy, z następującej listy dostępnych aplikacji Power BI:</span><span class="sxs-lookup"><span data-stu-id="06ef0-110">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>

- [<span data-ttu-id="06ef0-111">Dostawca bezpośredni</span><span class="sxs-lookup"><span data-stu-id="06ef0-111">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="06ef0-112">Dostawca pośredni</span><span class="sxs-lookup"><span data-stu-id="06ef0-112">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="06ef0-113">Pośredni odsprzedawca</span><span class="sxs-lookup"><span data-stu-id="06ef0-113">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="06ef0-114">Przed zainstalowaniem wersji zapoznawczej usługi Partner Center można upewnić się, że spełniasz poniższe wymagania.</span><span class="sxs-lookup"><span data-stu-id="06ef0-114">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="06ef0-115">Wybierasz poprawną Power BI aplikację dla swojej firmy.</span><span class="sxs-lookup"><span data-stu-id="06ef0-115">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="06ef0-116">Masz licencję na Power BI Pro.</span><span class="sxs-lookup"><span data-stu-id="06ef0-116">You have a Power BI pro license.</span></span>

- <span data-ttu-id="06ef0-117">Masz uprawnienia do instalowania aplikacji szablonów w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="06ef0-117">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="06ef0-118">Możesz zalogować się do Power BI.</span><span class="sxs-lookup"><span data-stu-id="06ef0-118">You can sign in to Power BI.</span></span>

- <span data-ttu-id="06ef0-119">Możesz zalogować się jako Administrator globalny, Agent administracyjny lub administrator rozliczeń do [dzierżawy Azure Active Directory firmy (Azure AD)](azure-active-directory-tenants-and-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="06ef0-119">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="06ef0-120">Aby zainstalować aplikację</span><span class="sxs-lookup"><span data-stu-id="06ef0-120">To install the app</span></span>

1. <span data-ttu-id="06ef0-121">Wybierz odpowiednie łącze do źródła aplikacji (bezpośredni dostawca/pośredni Dostawca/pośredni odsprzedawcy) w powyższej sekcji.</span><span class="sxs-lookup"><span data-stu-id="06ef0-121">Select the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="06ef0-122">Wybierz pozycję **Pobierz teraz**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-122">Select **GET IT NOW**.</span></span> 

3. <span data-ttu-id="06ef0-123">Zaakceptuj warunki i postanowienia, wybierając pozycję **Kontynuuj**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-123">Agree terms and conditions by selecting **Continue**.</span></span>

4. <span data-ttu-id="06ef0-124">W obszarze masz już konto? Wybierz pozycję **Zaloguj**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-124">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="06ef0-125">Na następnej stronie Wprowadź nazwę użytkownika Power BI i hasło, a następnie wybierz pozycję **Zaloguj się**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-125">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span>

6. <span data-ttu-id="06ef0-126">Zainstaluj obszar roboczy, podając nazwę obszaru roboczego.</span><span class="sxs-lookup"><span data-stu-id="06ef0-126">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="06ef0-127">Aplikacje szablonów zainstalowane w sekcji Aplikacje można znaleźć.</span><span class="sxs-lookup"><span data-stu-id="06ef0-127">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="06ef0-128">Wybierz pozycję **aplikacje** i wybierz zainstalowane aplikacje.</span><span class="sxs-lookup"><span data-stu-id="06ef0-128">Select **Apps** and choose the installed apps.</span></span>

9. <span data-ttu-id="06ef0-129">Rozpocznie się Rozpoczynanie pracy z nowym ekranem aplikacji.</span><span class="sxs-lookup"><span data-stu-id="06ef0-129">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="06ef0-130">Aby nawiązać połączenie z danymi, wybierz pozycję **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-130">To connect to the data, select **Connect**.</span></span>

11. <span data-ttu-id="06ef0-131">W oknie podręcznym **Połącz z centrum partnerskim** Sprawdź, czy **Metoda uwierzytelniania** jest ustawiona na **OAuth2** , lub wybierz pozycję **oAuth2** z listy, jeśli nie.</span><span class="sxs-lookup"><span data-stu-id="06ef0-131">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="06ef0-132">Wyświetlenie tego okna może potrwać kilka minut.</span><span class="sxs-lookup"><span data-stu-id="06ef0-132">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="06ef0-133">Na stronie **łącznika analizy Centrum partnerskiego** Zaloguj się przy użyciu poświadczeń administratora globalnego, agenta administratora lub administratora rozliczeń dla dzierżawy usługi Azure AD firmy, a następnie wybierz pozycję **Zaloguj**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-133">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="06ef0-134">Po wyświetleniu monitu o dostęp wybierz pozycję **Zaakceptuj**.</span><span class="sxs-lookup"><span data-stu-id="06ef0-134">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="06ef0-135">Gdy usługa Centrum partnerskiego jest połączona z Power BI, rozpocznie się ładowanie danych.</span><span class="sxs-lookup"><span data-stu-id="06ef0-135">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="06ef0-136">W zależności od ilości danych może to potrwać do 10 minut.</span><span class="sxs-lookup"><span data-stu-id="06ef0-136">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="06ef0-137">Po zakończeniu ładowania danych możesz rozpocząć korzystanie z pulpitu nawigacyjnego aplikacji do analizy Centrum partnerskiego i raportów w programie Power BI.</span><span class="sxs-lookup"><span data-stu-id="06ef0-137">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="06ef0-138">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="06ef0-138">Next steps</span></span>

[<span data-ttu-id="06ef0-139">Wyświetl dane biznesowe za pomocą aplikacji analizy Centrum partnerskiego dla firmy Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="06ef0-139">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
