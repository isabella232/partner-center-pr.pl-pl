---
title: Partner Center insights — dostęp oparty na rolach
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o określonych rolach potrzebnych do Partner Center szczegółowych informacji. Są to między innymi role osoby wyświetlającego raporty dla kierownictwa i osoby wyświetlającego raporty.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120787"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="d84e9-104">Kontrola dostępu oparta na rolach do pulpitu nawigacyjnego Partner Center Insights</span><span class="sxs-lookup"><span data-stu-id="d84e9-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="d84e9-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="d84e9-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d84e9-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="d84e9-106">Global admin</span></span>
- <span data-ttu-id="d84e9-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="d84e9-107">Admin agent</span></span>
- <span data-ttu-id="d84e9-108">Przeglądarka raportów</span><span class="sxs-lookup"><span data-stu-id="d84e9-108">Report viewer</span></span>
- <span data-ttu-id="d84e9-109">Przeglądarka raportów dla kierownictwa</span><span class="sxs-lookup"><span data-stu-id="d84e9-109">Executive report viewer</span></span>

<span data-ttu-id="d84e9-110">Pulpit nawigacyjny szczegółowych informacji używa dwóch nowych ról w Partner Center do zarządzania dostępem pracowników do raportów — Executive Report Viewer i Report Viewer.</span><span class="sxs-lookup"><span data-stu-id="d84e9-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="d84e9-111">Użytkownicy z rolą Executive Report Viewer mają dostęp do wszystkich zestawów danych raportowania, natomiast użytkownicy w roli Osoby wyświetlającego raporty nie będą mieć dostępu do poufnych zestawów danych, takich jak dane osobowe przychodów i klientów/pracowników.</span><span class="sxs-lookup"><span data-stu-id="d84e9-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="d84e9-112">Podobnie jak Partner Center ról, administrator globalny lub administrator konta będzie mógł przypisywać użytkowników do tych ról na stronie Zarządzanie użytkownikami.</span><span class="sxs-lookup"><span data-stu-id="d84e9-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="d84e9-113">Role mogą być stosowane w całej firmie lub w określonych lokalizacjach MPN.</span><span class="sxs-lookup"><span data-stu-id="d84e9-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="d84e9-114">Role przypisane do określonych lokalizacji MPN ograniczają użytkownika do wyświetlania danych raportowania skojarzonych tylko z wybranymi lokalizacjami MPN.</span><span class="sxs-lookup"><span data-stu-id="d84e9-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="d84e9-115">Partner może wybrać jedną lub wiele lokalizacji z poniższego widoku.</span><span class="sxs-lookup"><span data-stu-id="d84e9-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Przedstawia ustawienia ról szczegółowych Partner Center lokalizacji dla przeglądarki raportów i przeglądarki raportów kierownictwa.":::

>[!Note]
> <span data-ttu-id="d84e9-117">Użytkownicy, którzy są administratorami MPN od 20 stycznia 2020 r., są automatycznie dodawana do roli Osoby wyświetlającego raporty kierownictwa dla całej firmy dla wszystkich lokalizacji dla tej dzierżawy. </span><span class="sxs-lookup"><span data-stu-id="d84e9-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="d84e9-118">Dzięki temu użytkownicy ci mogą uzyskać dostęp do raportów jako osoby przeglądają raporty kierownictwa bez żadnych jawnych działań wymaganych przez administratora globalnego lub administratora konta. Administratorzy globalni i administratorzy kont mogą zastąpić automatycznie przypisane role tych użytkowników, aby jeszcze bardziej zwiększyć lub ograniczyć ich możliwości.</span><span class="sxs-lookup"><span data-stu-id="d84e9-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d84e9-119">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="d84e9-119">Next steps</span></span>

- <span data-ttu-id="d84e9-120">Dowiedz się więcej [o Partner Center Insights](partner-center-insights.md) i jego różnych raportach.</span><span class="sxs-lookup"><span data-stu-id="d84e9-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
