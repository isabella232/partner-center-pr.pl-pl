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
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215853"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI


**Odpowiednie role**
-   Administrator globalny
-   Administrator użytkowników
-   Agent sprzedaży
-   Agent administracyjny

## <a name="before-you-begin"></a>Przed rozpoczęciem

Wybierz aplikację, która jest najbardziej odpowiednia dla Twojej firmy, z następującej listy dostępnych aplikacji Power BI:
- [Dostawca bezpośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Dostawca pośredni](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Pośredni odsprzedawca](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Przed zainstalowaniem wersji zapoznawczej usługi Partner Center można upewnić się, że spełniasz poniższe wymagania.

- Wybierasz poprawną Power BI aplikację dla swojej firmy.

- Masz licencję na Power BI Pro.

- Masz uprawnienia do instalowania aplikacji szablonów w dzierżawie.

- Możesz zalogować się do Power BI.

- Możesz zalogować się jako Administrator globalny, Agent administracyjny lub administrator rozliczeń do [dzierżawy Azure Active Directory firmy (Azure AD)](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Aby zainstalować aplikację

1. Kliknij odpowiednie łącze do źródła aplikacji (bezpośredni dostawca/pośredni Dostawca/pośredni odsprzedawcy) w powyższej sekcji.

2. Kliknij pozycję **Pobierz teraz**. 

3. Zaakceptuj warunki i postanowienia, klikając przycisk **Kontynuuj**.

4. W obszarze masz już konto? Wybierz pozycję **Zaloguj**.

5. Na następnej stronie Wprowadź nazwę użytkownika Power BI i hasło, a następnie wybierz pozycję Zaloguj się.

6. Zainstaluj obszar roboczy, podając nazwę obszaru roboczego.

7. Aplikacje szablonów zainstalowane w sekcji Aplikacje można znaleźć.

8. Kliknij pozycję aplikacje i wybierz zainstalowane aplikacje.

9. Rozpocznie się Rozpoczynanie pracy z nowym ekranem aplikacji.

10. Aby nawiązać połączenie z danymi, kliknij przycisk **Połącz**.

11. W oknie podręcznym **Połącz z centrum partnerskim** Sprawdź, czy **Metoda uwierzytelniania** jest ustawiona na **OAuth2** , lub wybierz pozycję **oAuth2** z listy, jeśli nie. 

> [!NOTE]  
>  Wyświetlenie tego okna może potrwać kilka minut.

12. Na stronie **łącznika analizy Centrum partnerskiego** Zaloguj się przy użyciu poświadczeń administratora globalnego, agenta administratora lub administratora rozliczeń dla dzierżawy usługi Azure AD firmy, a następnie wybierz pozycję **Zaloguj**.
 
13. Po wyświetleniu monitu o dostęp wybierz pozycję **Zaakceptuj**. 

Gdy usługa Centrum partnerskiego jest połączona z Power BI, rozpocznie się ładowanie danych. W zależności od ilości danych może to potrwać do 10 minut. 

Po zakończeniu ładowania danych możesz rozpocząć korzystanie z pulpitu nawigacyjnego aplikacji do analizy Centrum partnerskiego i raportów w programie Power BI.

## <a name="next-steps"></a>Następne kroki

[Wyświetl dane biznesowe za pomocą aplikacji analizy Centrum partnerskiego dla firmy Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
