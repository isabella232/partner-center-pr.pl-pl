---
title: Dostęp oparty na rolach usługi Partner Center
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o określonych rolach wymaganych do wyświetlenia raportów usługi Partner Center Insights. Obejmują one role programu Executive Report Viewer i Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2020
ms.locfileid: "92529669"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="df633-104">Kontrola dostępu oparta na rolach na pulpicie nawigacyjnym usługi Partner Center Insights</span><span class="sxs-lookup"><span data-stu-id="df633-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="df633-105">Pulpit nawigacyjny usługi Insights używa dwóch nowych ról w centrum partnerskim do zarządzania dostępem pracowników do raportów — programu Executive raportów i raportów.</span><span class="sxs-lookup"><span data-stu-id="df633-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="df633-106">Użytkownicy w roli programu Executive Report Viewer mają dostęp do wszystkich zestawów danych raportowania, a użytkownicy w roli przeglądarki raportów nie będą mieli dostępu do poufnych zestawów dane, takich jak dochody i dane osobowe dotyczące odbiorców/pracowników.</span><span class="sxs-lookup"><span data-stu-id="df633-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="df633-107">Podobnie jak w przypadku innych ról Centrum partnerskiego, Administrator globalny lub administrator konta będzie mógł przypisywać użytkowników do tych ról na stronie Zarządzanie użytkownikami.</span><span class="sxs-lookup"><span data-stu-id="df633-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="df633-108">Role mogą być stosowane w całej firmie lub dla określonych lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="df633-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="df633-109">Role przypisane do określonych lokalizacji MPN ograniczają użytkownika do wyświetlania danych raportowania skojarzonych tylko z wybranymi lokalizacjami MPN.</span><span class="sxs-lookup"><span data-stu-id="df633-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="df633-110">Partner może wybrać jedną lub wiele lokalizacji z poziomu poniższego widoku.</span><span class="sxs-lookup"><span data-stu-id="df633-110">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Przedstawia ustawienia ról usługi Partner Center dla konkretnych lokalizacji dla przeglądarki raportów i programu Executive Report Viewer.":::

>[!Note]
> <span data-ttu-id="df633-112">Użytkownicy, którzy są administratorami MPN od dwudziestu 20 stycznia 2020 są automatycznie dodawani do roli programu **Executive Report** w całej firmie dla wszystkich lokalizacji dla tej dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="df633-112">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="df633-113">Ci użytkownicy mogą w ten sposób uzyskiwać dostęp do raportów w postaci programu Executive Report Viewer bez jawnej akcji wymaganej przez administratora globalnego lub administratora konta. Administratorzy globalni i Administratorzy konta mogą zastąpić automatyczne przypisane role tych użytkowników, aby zwiększyć lub ograniczyć ich możliwości.</span><span class="sxs-lookup"><span data-stu-id="df633-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="df633-114">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="df633-114">Next steps</span></span>

- <span data-ttu-id="df633-115">Dowiedz się więcej na temat usługi [Partner Center szczegółowe](partner-center-insights.md) informacje i jej różne raporty.</span><span class="sxs-lookup"><span data-stu-id="df633-115">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
