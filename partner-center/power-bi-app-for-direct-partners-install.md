---
title: Instalowanie Partner Center Analytics dla Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Wykonaj kroki opisane w tym artykule, aby zainstalować i wyświetlić podgląd aplikacja statystyczna Centrum partnerskiego dla usługi Power BI (dla bezpośrednich partnerów w programie CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a07742a55df088842f6bac1a1cbdd65bf0db8282
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959601"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI


**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent sprzedaży | Agent administracyjny

## <a name="before-you-begin"></a>Zanim rozpoczniesz

Wybierz aplikację, która jest najbardziej odpowiedni dla Twojej firmy, z następującej listy dostępnych aplikacji Power BI Microsoft:

- [Dostawca bezpośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Dostawca pośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Odsprzedawca pośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Przed zainstalowaniem aplikacji Partner Center Analytics w wersji zapoznawczej upewnij się, że spełniasz następujące wymagania.

- Wybierasz właściwą aplikację Power BI dla Swojej firmy.

- Masz licencję Power BI Pro.

- Masz uprawnienia do instalowania aplikacji szablonu w dzierżawie.

- Możesz zalogować się do Power BI.

- Możesz zalogować się jako administrator globalny, agent administratora lub administrator rozliczeń w dzierżawie usługi [Azure Active Directory (Azure AD).](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Aby zainstalować aplikację

1. Wybierz podany link źródła aplikacji (Dostawca bezpośredni/Dostawca pośredni/Odsprzedawca pośredni) w powyższej sekcji.

2. Wybierz **pozycję POBIERZ TERAZ.** 

3. Uzgodnij warunki i postanowienia, wybierając pozycję **Kontynuuj.**

4. W obszarze Masz już konto? Wybierz **pozycję Zaloguj się.**

5. Na następnej stronie wprowadź nazwę Power BI użytkownika i hasło, a następnie wybierz **pozycję Zaloguj się.**

6. Zainstaluj obszar roboczy, podając nazwę obszaru roboczego.

7. Aplikacje szablonu zainstalowane w sekcji Aplikacje.

8. Wybierz **pozycję** Aplikacje i wybierz zainstalowane aplikacje.

9. Wprowadzenie zostanie otwarty ekran nowej aplikacji.

10. Aby nawiązać połączenie z danymi, wybierz **pozycję Połączenie**.

11. W **oknie podręcznym** Połączenie Partner Center Analytics sprawdź, czy  dla opcji Metoda uwierzytelniania ustawiono wartość **oAuth2,** lub wybierz pozycję **oAuth2** z listy, jeśli tak nie jest. 

> [!NOTE]  
>  Może to potrwać kilka minut.

12. Na stronie **Partner Center Analytics Connector** zaloguj się przy użyciu poświadczeń administratora globalnego, agenta administratora lub administratora rozliczeń dla dzierżawy usługi Azure AD firmy, a następnie wybierz pozycję Zaloguj **się.**
 
13. Po wyświetleniu monitu o dostęp wybierz pozycję **Zaakceptuj**. 

Gdy usługa Partner Center Analytics zostanie połączona z Power BI, rozpocznie się ładowanie danych. W zależności od ilości danych może to potrwać do 10 minut. 

Po zakończeniu ładowania danych możesz rozpocząć korzystanie z pulpitu nawigacyjnego i raportów aplikacji Partner Center Analytics w Power BI.

## <a name="next-steps"></a>Następne kroki

[Wyświetlanie danych biznesowych za pomocą aplikacji Partner Center Analytics dla usługi Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
