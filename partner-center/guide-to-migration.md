---
title: Migrowanie z pmc do Partner Center
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przeprowadzić migrację firmy z Partner Membership Center (PMC) do Partner Center, w tym czynności, które należy wykonać.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 511612042f7da5e43d045d2991fa7d5251612726
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150747"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Przewodnik migracji z witryny PMC do Centrum partnerskiego

**Odpowiednie role:** Administrator globalny

Witryna internetowa partnerów firmy Microsoft w partner.microsoft.com to ujednolicone środowisko cyfrowe dla partnerów. W witrynie internetowej partnera będzie można eksplorować możliwości i korzystać z przewodników, które ułatwiają firmie tworzenie i sprzedawanie aplikacji i usług w firmie Microsoft. Korzystając z linku pulpitu nawigacyjnego dostępnego w witrynie internetowej partnera, członkowie portalu Microsoft Partner Network mogą zalogować się do Centrum partnerskiego, w którym zarządzasz relacją z firmą Microsoft, rejestrujesz się w programach i rejestrujesz się w ofertach.

Partner Membership Center (PMC) jest likwidowane. Twoja firma została zaproszona do zmiany zarządzania Microsoft Partner Network członkostwem w Partner Center. Ten przewodnik przygotuje Cię do tego, czego można oczekiwać podczas przechodzenia z usługi PMC do Partner Center.

>[!NOTE]
>Nawet jeśli firma ma więcej niż jedno konto lub lokalizację, przejście do usługi Partner Center rozpoczyna się od przeniesienia jednego (pierwszego) konta do Partner Center.

## <a name="get-started"></a>Rozpoczęcie pracy

Przeniesienie rozpoczyna się od pmc. Administrator globalny otrzyma zaproszenie do rozpoczęcia przenoszenia.

### <a name="prepare-in-pmc"></a>Przygotowywanie w programie PMC

- Weryfikowanie szczegółów firmy
- Weryfikowanie kontaktu z programem podstawowym
- Weryfikowanie lokalizacji biznesowych
- Aktualizowanie zatwierdzonych użytkowników

### <a name="when-youre-ready"></a>Gdy wszystko będzie gotowe

Wybierz **pozycję Wprowadzenie** w zaproszeniu. Zostaniesz przekierowyny do Partner Center logowania.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Wprowadzenie":::

## <a name="start-with-your-work-email"></a>Rozpoczynanie pracy z służbową pocztą e-mail

Jeśli Twoja firma nie ma służbowej poczty e-mail i dzierżawy usługi AAD, możemy pomóc Ci skonfigurować ją podczas Partner Center procesu logowania. Podczas próby zalogowania się przy użyciu konta e-mail, które nie jest służbowym adresem e-mail, takim jak konto osobiste, zostaniesz skierowany do Ciebie, aby podać informacje o twojej firmie, dzięki czemu będziemy w stanie skonfigurować dzierżawę usługi AAD i służbowy adres e-mail. Te szczegóły firmy zostaną użyte do sfinalizowania konta w Partner Center, dlatego upewnij się, że są one dokładne.

>[!NOTE]
>Jeśli jesteś partnerem w Chinach i jesteś zarejestrowanym w programie Microsoft Partner Network i Dostawca rozwiązań w chmurze (CSP), będziesz mieć oddzielną dzierżawę dla każdego konta. Twoje konto w programie Dostawca rozwiązań w chmurze jest zarządzane w chmurze krajowej, a Twoje Microsoft Partner Network zarządzane w chmurze globalnej. Nie można połączyć tych dwóch kont.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Poinformuj nas o swojej firmie":::

Po zweryfikowaniu lub zaktualizowania informacji wybierz pozycję **Zaakceptuj i kontynuuj.**
Warunki i postanowienia na tej stronie są dokładnie takie **same** jak umowa, która została już podpisana przez Twoją firmę w chmurze PMC.  
Ten krok inicjuje tworzenie dzierżawy usługi Azure AD i zapewnia konto służbowe.

Wybranie **przycisku Akceptuj i** kontynuuj powoduje również następujące czynności:

- Migruje konto wraz ze WSZYSTKIMI jego lokalizacjami do Partner Center

- Migruje wszelkie kompetencje lub makity, które mogły zostać zakupione w programie PMC

- Migruje wszelkie zasoby marketingowe, oferty i programy (MAPs, Silver, Gold), które były dostępne w programie PMC

## <a name="invite-employees-to-join-you"></a>Zapraszanie pracowników do dołączenia do Ciebie

Po utworzeniu nowej dzierżawy usługi Azure AD możesz zaprosić pracowników do zalogowania się do Partner Center.

:::image type="content" source="images/migration/invite.png" alt-text="Zapraszanie pracowników":::

Jeśli zalogowano się przy użyciu istniejącej dzierżawy usługi AAD, twoi pracownicy przeniosą się wraz z Toem. W takim przypadku przypisz pracownikom role, aby zarządzać tym, co mogą robić w Partner Center. 

>[!NOTE] 
>Role w Partner Center są inne niż role w programie PMC. Aby uzyskać więcej informacji, [zobacz Moving from PMC to Partner Center (Przechodzenie](move-pmc-pc-map.md)z pmc do Partner Center ).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Weryfikowanie domeny i zostań administratorem globalnym  

Jeśli dzierżawa usługi AAD jest nowa, nikt nie ma przypisanej roli administratora globalnego. Aby zostać administratorem globalnym, musisz zweryfikować własność domeny. Administrator domeny może Ci w tym pomóc.

Możesz korzystać z już zakupionych ofert, ale nie będzie można kupować żadnych nowych ofert, dopóki nie ukończysz kroku przypisywania administratora globalnego.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Przejmij kontrolę":::

Po wybraniu opcji Rozpoczynanie pracy zostanie wyświetlony następujący ekran:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Weryfikowanie własności domeny":::

Rejestrator domen zostanie już wypełniony. Tylko właściciel domeny może zaktualizować plik DNS, dlatego kopiując i dodając plik tekstowy do rekordu DNS, możemy sprawdzić, czy jesteś właścicielem. Aktualizacja potrwa kilka minut. Musisz wylogować się z Partner Center a następnie zalogować się ponownie. Twoja rola zostanie zmieniona na administratora globalnego.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Zapoznaj się z pulpitem nawigacyjnym i Partner Center

Zobacz przewodnik po pulpicie nawigacyjnym. W tym miejscu możesz zarządzać członkostwem, dodać profil biznesowy dla poleceń, zarejestrować się w programie Dostawca rozwiązań w chmurze oraz wyświetlić powiadomienia i oferty dotyczące Twojej firmy w dowolnym momencie, wybierając pozycję Pulpit **nawigacyjny**. Możesz również zarządzać zachętami, kupować na platformie handlowej, samodzielnie korzystać z usług na rynku i nie tylko.  

:::image type="content" source="images/migration/fre.png" alt-text="Zobacz przewodnik":::

## <a name="sign-the-microsoft-partner-agreement"></a>Podpisywanie Microsoft Partner Agreement

Jeśli jesteś odsprzedawcą pośrednim, po skonfigurowaniu konta Partner Center nadal musisz oficjalnie zarejestrować się w programie Dostawca rozwiązań w chmurze rejestracji. Aby sprawdzić stan członkostwa, przejdź do profilu [prawnego](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) i potwierdź typ konta. Następnie zarejestruj się w programie CSP jako [odsprzedawca pośredni.](enrolling-in-the-csp-program.md)

 Po zarejestrowaniu się jako odsprzedawca pośredni zaakceptuj żądanie relacji [CSP z dostawcą pośrednim](indirect-reseller-tasks-in-partner-center.md).

Następnie zaakceptuj informacje na Microsoft Partner Agreement na Partner Center [nawigacyjnym przy](https://partner.microsoft.com/pvc/dashboard) użyciu poświadczeń administratora globalnego. Upewnij się, że masz podpis Microsoft Partner Agreement w sekcji Informacje o programie w profilu partnera. Ponadto na stronie Przeglądu CSP zostanie wyświetlony baner z potwierdzeniem. 

## <a name="next-steps"></a>Następne kroki

- [Znajdowanie administratora globalnego](become-global-admin.md)

- [Umowa partnerska firmy Microsoft](microsoft-partner-agreement.md)

- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)

- [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md)

- [Zarządzanie programami członkostwa](renew-mpn-offers.md)

- [Tworzenie profilu biznesowego firmy](create-a-marketing-profile.md)

- [Nawiązywanie połączenia z klientami za pośrednictwem poleceń](manage-leads.md)

- [Przewodnik migracji wielu firm z pmc do Partner Center](move-multiple-companies.md)
