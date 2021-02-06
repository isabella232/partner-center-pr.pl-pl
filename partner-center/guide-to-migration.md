---
title: Migrowanie z programu PMC do Centrum partnerskiego
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak migrować firmę z Centrum członkostwa partnerów (PMC) do Centrum partnerskiego, w tym czynności, które należy wykonać.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dd566a6d9ef60747eb7fd515b4d63d87d991da2a
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624191"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Przewodnik migracji z witryny PMC do Centrum partnerskiego

**Odpowiednie role**

- Administrator globalny

Witryna internetowa partnera firmy Microsoft pod adresem partner.microsoft.com to ujednolicone środowisko cyfrowe dla partnerów. W witrynie sieci Web partnera będziesz mieć możliwość eksplorowania możliwości i korzystania z przewodników, które ułatwiają tworzenie i sprzedawanie aplikacji oraz usług w firmie Microsoft. Korzystając z linku pulpitu nawigacyjnego dostępnego w witrynie sieci Web partnera, Członkowie Microsoft Partner Network mogą zalogować się do Centrum partnerskiego, w którym zarządzasz swoją relacją z firmą Microsoft, zarejestrować się w programach i utworzyć konto w celu uzyskania ofert.

Centrum członkostwa partnerów (PMC) jest likwidowane. Twoja firma została zaproszona do przejścia do Microsoft Partner Network zarządzania członkostwem w centrum partnerskim. Ten przewodnik przygotowuje się do tego, co powinno się spodziewać, gdy przejdziesz od PMC do Centrum partnerskiego.

>[!NOTE]
>Nawet jeśli Twoja firma ma więcej niż jedno konto lub lokalizacja, przechodzenie do Centrum partnerskiego rozpoczyna się od przeniesienia jednego (pierwszego) konta do Centrum partnerskiego.

## <a name="get-started"></a>Rozpoczęcie pracy

Przeniesienie rozpoczyna się w kryterium PMC. Administrator globalny otrzyma zaproszenie do rozpoczęcia przenoszenia.

### <a name="prepare-in-pmc"></a>Przygotuj w kryterium PMC

- Weryfikowanie szczegółów firmy
- Weryfikuj kontakt programu podstawowego
- Weryfikuj lokalizacje biznesowe
- Aktualizowanie zatwierdzonych użytkowników

### <a name="when-youre-ready"></a>Gdy wszystko będzie gotowe

Wybierz pozycję **Rozpocznij pracę** na Twoim zaproszeniu. Nastąpi przekierowanie do strony logowania Centrum partnerskiego.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Wprowadzenie":::

## <a name="start-with-your-work-email"></a>Zacznij od służbowego adresu e-mail

Jeśli firma nie dysponuje służbową pocztą e-mail i dzierżawą usługi AAD, możemy pomóc Ci skonfigurować ją podczas procesu logowania w centrum partnerskim. Podczas próby zalogowania się przy użyciu konta e-mail, które nie jest służbowym adresem e-mail, na przykład konta osobistego, nastąpi przekierowanie do podania informacji o firmie, aby można było skonfigurować dzierżawcę usługi AAD i służbowy adres e-mail. Te szczegóły firmy zostaną użyte do sfinalizowania Twojego konta w centrum partnerskim, dlatego należy się upewnić, że są dokładne.

>[!NOTE]
>Jeśli jesteś partnerem w Chinach i zarejestrowany zarówno w programie Microsoft Partner Network, jak i w programie Cloud Solution Provider (CSP), będziesz mieć osobną dzierżawę dla każdego konta. Twoje konto z programem dostawcy rozwiązań w chmurze jest zarządzane w chmurze krajowej, a konto Microsoft Partner Network jest zarządzane w chmurze globalnej. Nie można połączyć tych dwóch kont.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Powiedz nam o swojej firmie":::

Po zweryfikowaniu lub zaktualizowaniu informacji wybierz pozycję **Zaakceptuj i Kontynuuj**.
Warunki i postanowienia na tej stronie są **dokładnie takie same** , jak umowa, w której firma jest już podpisana.  
Ten krok inicjuje tworzenie dzierżawy usługi Azure AD i udostępnia konto służbowe.

Wybranie opcji **Akceptuj i Kontynuuj** wykonuje także następujące czynności:

- Migruje Twoje konto wraz ze wszystkimi lokalizacjami do Centrum partnerskiego

- Migruje wszelkie kompetencje lub mapy, które mogły zostać zakupione w ramach kryterium PMC

- Migruje wszystkie zasoby marketingowe, oferty i programy (MAPs, Silver, Gold), które zostały w PMC

## <a name="invite-employees-to-join-you"></a>Zapraszanie pracowników do dołączenia

Po utworzeniu nowej dzierżawy usługi Azure AD możesz zapraszać pracowników do logowania się do Centrum partnerskiego.

:::image type="content" source="images/migration/invite.png" alt-text="Zaproś pracowników":::

Jeśli zalogowano się za pomocą istniejącej dzierżawy usługi AAD, pracownicy zostaną przeniesieni do Ciebie. W takim przypadku należy przypisać role pracowników, które określają, co można zrobić w centrum partnerskim. 

>[!NOTE] 
>Role w centrum partnerskim są inne niż role w przystawce PMC. Aby uzyskać więcej informacji [, zobacz przechodzenie od PMC do Centrum partnerskiego](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Zweryfikuj domenę i Zostań administratorem globalnym  

Jeśli dzierżawca usługi AAD jest nowy, nikt nie ma przypisanej roli administratora globalnego. Aby stać się administratorem globalnym, należy zweryfikować własność domeny. Do tego celu może być potrzebny administrator domeny.

Chociaż możesz skorzystać z ofert, które zostały już zakupione, nie będziesz w stanie zakupić żadnych nowych ofert, dopóki nie ukończysz kroku przypisywania administratora globalnego.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Przejmij kontrolę":::

Gdy wybierzesz pozycję Rozpocznij, zobaczysz następujący ekran:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Weryfikowanie własności domeny":::

Rejestrator domeny zostanie już wypełniony. Tylko właściciel domeny może zaktualizować plik DNS, aby skopiować i dodać plik tekstowy do rekordu DNS, możemy sprawdzić, czy jesteś właścicielem. Aktualizacja może potrwać kilka minut. Musisz wylogować się z Centrum partnerskiego, a następnie zalogować się ponownie. Twoja rola zostanie zmieniona na administratora globalnego.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Zapoznaj się z pulpitem nawigacyjnym i centrum partnerskim

Zapoznaj się z pulpitem nawigacyjnym. W tym miejscu można zarządzać członkostwem, dodawać do nich profil biznesowy, rejestrować się w programie dostawcy rozwiązań w chmurze oraz powiadomienia i oferty odpowiednie dla Twojej firmy w dowolnym momencie, wybierając pozycję **pulpit nawigacyjny**. Możesz również zarządzać bodźcami, kupować je w portalu Marketplace, zarejestrować się w celu uzyskania usług na rynku i innych.  

:::image type="content" source="images/migration/fre.png" alt-text="Zapoznaj się z przewodnikiem":::

## <a name="sign-the-microsoft-partner-agreement"></a>Podpisz umowę partnera firmy Microsoft

Jeśli jesteś pośrednim odsprzedawcą, po skonfigurowaniu konta Centrum partnerskiego nadal musisz zarejestrować się w programie Cloud Solution Provider. Aby sprawdzić stan członkostwa, przejdź do [profilu prawnego](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) i Potwierdź typ konta. Następnie zarejestruj się w programie CSP jako [pośredni odsprzedawcy](enrolling-in-the-csp-program.md).

 Po zarejestrowaniu jako pośredni odsprzedawcy Zaakceptuj [żądanie relacji CSP z dostawcą pośrednim](indirect-reseller-tasks-in-partner-center.md).

Następnie zaakceptuj umowę partnera firmy Microsoft na [pulpicie nawigacyjnym](https://partner.microsoft.com/pvc/dashboard) Centrum partnerskiego, korzystając z poświadczeń administratora globalnego. Upewnij się, że została podpisana umowa partnerska firmy Microsoft w sekcji Informacje o programie profilu partnera. Ponadto zobaczysz powiadomienie na banerze potwierdzającym na stronie Przegląd dostawcy usług kryptograficznych. 

## <a name="next-steps"></a>Następne kroki

- [Znajdź administratora globalnego](become-global-admin.md)

- [Umowa partnerska firmy Microsoft](microsoft-partner-agreement.md)

- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)

- [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md)

- [Zarządzanie programami członkostwa](renew-mpn-offers.md)

- [Utwórz profil firmowy firmy](create-a-marketing-profile.md)

- [Łączenie się z klientami przy użyciu odwołań](manage-leads.md)

- [Przewodnik migracji wielu firm z programu PMC do Centrum partnerskiego](move-multiple-companies.md)
