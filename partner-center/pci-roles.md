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
ms.openlocfilehash: 803c299311f129c4842a92a27abd9b9addb49f17
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854438"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="d4732-104">Kontrola dostępu oparta na rolach do pulpitu nawigacyjnego Partner Center Insights</span><span class="sxs-lookup"><span data-stu-id="d4732-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="d4732-105">**Odpowiednie role:** Administrator globalny | Agent administracyjny | Przeglądarka raportów | Przeglądarka raportów dla kierownictwa</span><span class="sxs-lookup"><span data-stu-id="d4732-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="d4732-106">Pulpit nawigacyjny szczegółowych informacji używa dwóch nowych ról w Partner Center do zarządzania dostępem pracowników do raportów — Executive Report Viewer i Report Viewer.</span><span class="sxs-lookup"><span data-stu-id="d4732-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="d4732-107">Użytkownicy z rolą Executive Report Viewer mają dostęp do wszystkich zestawów danych raportowania, natomiast użytkownicy w roli Osoby wyświetlającego raporty nie będą mieć dostępu do poufnych zestawów danych, takich jak dane osobowe przychodów i klientów/pracowników.</span><span class="sxs-lookup"><span data-stu-id="d4732-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="d4732-108">Podobnie jak Partner Center ról, administrator globalny lub administrator konta będzie mógł przypisywać użytkowników do tych ról na stronie Zarządzanie użytkownikami.</span><span class="sxs-lookup"><span data-stu-id="d4732-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="d4732-109">Role mogą być stosowane w całej firmie lub dla określonych lokalizacji MPN.</span><span class="sxs-lookup"><span data-stu-id="d4732-109">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="d4732-110">Role przypisane do określonych lokalizacji MPN ograniczają użytkownika do wyświetlania danych raportowania skojarzonych tylko z wybranymi lokalizacjami MPN.</span><span class="sxs-lookup"><span data-stu-id="d4732-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="d4732-111">Partner może wybrać jedną lub wiele lokalizacji z poniższego widoku.</span><span class="sxs-lookup"><span data-stu-id="d4732-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Przedstawia ustawienia ról szczegółowych Partner Center lokalizacji dla przeglądarki raportów i przeglądarki raportów kierownictwa.":::

>[!Note]
> <span data-ttu-id="d4732-113">Użytkownicy, którzy są administratorami MPN od 20 stycznia 2020 r., są automatycznie dodawana do roli osoby wyświetlającego raporty kierownictwa dla całej firmy dla wszystkich lokalizacji dla tej dzierżawy. </span><span class="sxs-lookup"><span data-stu-id="d4732-113">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="d4732-114">W ten sposób ci użytkownicy mogą uzyskać dostęp do raportów jako osoby przeglądają raporty kierownictwa bez żadnych jawnych działań wymaganych przez administratora globalnego lub administratora konta. Administratorzy globalni i administratorzy kont mogą zastąpić automatycznie przypisane role tych użytkowników, aby jeszcze bardziej zwiększyć lub ograniczyć ich możliwości.</span><span class="sxs-lookup"><span data-stu-id="d4732-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d4732-115">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="d4732-115">Next steps</span></span>

- <span data-ttu-id="d4732-116">Dowiedz się więcej [o Partner Center Insights](partner-center-insights.md) i jego różnych raportach.</span><span class="sxs-lookup"><span data-stu-id="d4732-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
