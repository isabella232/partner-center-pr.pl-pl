---
title: Instalowanie Partner Center Analytics dla Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wykonaj kroki opisane w tym artykule, aby zainstalować i wyświetlić podgląd aplikacja statystyczna Centrum partnerskiego dla usługi Power BI (dla bezpośrednich partnerów w programie CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854489"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI


**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent sprzedaży | Agent administracyjny

## <a name="before-you-begin"></a>Zanim rozpoczniesz

Wybierz aplikację, która jest najbardziej odpowiednią dla Twojej firmy, z poniższej listy dostępnych Power BI aplikacji:

- [Dostawca bezpośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Dostawca pośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Odsprzedawca pośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Przed zainstalowaniem wersji zapoznawczej Partner Center Analytics upewnij się, że spełniasz następujące wymagania.

- Wybierasz właściwą aplikację Power BI dla Twojej firmy.

- Masz licencję Power BI Pro.

- Masz uprawnienia do instalowania aplikacji szablonu w dzierżawie.

- Możesz zalogować się do Power BI.

- Możesz zalogować się jako administrator globalny, agent administratora lub administrator rozliczeń w dzierżawie usługi [Azure Active Directory (Azure AD).](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Aby zainstalować aplikację

1. Wybierz link źródła aplikacji podany w powyższej sekcji (Dostawca bezpośredni/Dostawca pośredni/Odsprzedawca pośredni).

2. Wybierz **pozycję POBIERZ TERAZ.** 

3. Uzgodnij warunki i postanowienia, wybierając pozycję **Kontynuuj.**

4. W obszarze Masz już konto? Wybierz **pozycję Zaloguj się.**

5. Na następnej stronie wprowadź nazwę Power BI użytkownika i hasło, a następnie wybierz **pozycję Zaloguj się.**

6. Zainstaluj obszar roboczy, podając nazwę obszaru roboczego.

7. Aplikacje szablonów zainstalowane w sekcji Aplikacje.

8. Wybierz **pozycję** Aplikacje i wybierz zainstalowane aplikacje.

9. Rozpocznij zostanie otwarty ekran nowej aplikacji.

10. Aby nawiązać połączenie z danymi, wybierz pozycję **Połącz**.

11. W **oknie podręcznym Connect to Partner Center Analytics** (Łączenie z usługą Partner Center Analytics) sprawdź, czy dla opcji **Metoda** uwierzytelniania ustawiono wartość **oAuth2,** lub wybierz pozycję **oAuth2** z listy, jeśli tak nie jest. 

> [!NOTE]  
>  Może to potrwać kilka minut.

12. Na stronie **Partner Center Analytics Connector** zaloguj się przy użyciu poświadczeń administratora globalnego, agenta administratora lub administratora rozliczeń dla dzierżawy usługi Azure AD firmy, a następnie wybierz pozycję Zaloguj **się.**
 
13. Po wyświetleniu monitu o dostęp wybierz pozycję **Zaakceptuj**. 

Gdy usługa Partner Center Analytics zostanie połączona z Power BI, rozpocznie się ładowanie danych. W zależności od ilości danych może to potrwać do 10 minut. 

Po zakończeniu ładowania danych możesz rozpocząć korzystanie z pulpitu nawigacyjnego i raportów Partner Center Analytics w Power BI.

## <a name="next-steps"></a>Następne kroki

[Wyświetlanie danych biznesowych za pomocą aplikacji Partner Center Analytics dla firmy Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
