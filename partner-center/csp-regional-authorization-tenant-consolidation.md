---
title: Konsolidacja dzierżawy autoryzacji regionalnej programu CSP
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-membership
description: Użyj tych instrukcji, aby skonsolidować dzierżawy dla różnych krajów/regionów. Obejmuje to kroki migracji kont klientów i subskrypcji klientów.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 1500525e49fd2585cd97cd4cf7999cba63ac9f30
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072336"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instrukcje dotyczące konsolidacji dzierżawy regionalnej autoryzacji dostawcy CSP

**Dotyczy:** Partner Center | Partner Center dla Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny | Agent administracyjny

\[Niektóre informacje odnoszą się do przedpremierowego produktu, który może zostać znacząco zmodyfikowany przed jego premierą komercyjną. Firma Microsoft nie udziela żadnych gwarancji, jawnych lub domniemanych, w odniesieniu do informacji podanych w tym miejscu.\]

Możesz konsolidować dzierżawy dla swojej firmy. Użyj tych instrukcji, aby skonsolidować dzierżawy dla różnych krajów/regionów.

>[!NOTE]  
>Musisz mieć świadomość wszystkich aprowowanych subskrypcji i liczby licencji dla każdego z klientów na koncie, z których przechodzisz. W ramach procesu migracji ponownie aprowizuje się te same dokładnie subskrypcje z tymi samymi liczbami licencji w ramach nowego konta centralnego CSP. Funkcja eksportowania listy pomaga utworzyć listę klientów, którzy przejdą do scentralizowanej dzierżawy.  Po zakończeniu konsolidacji nie można przywrócić poprzedniego stanu dzierżawy. Może być również wymagane działanie klienta.

## <a name="prepare-for-migration"></a>Przygotowanie do migracji

- Zaloguj się **do Partner Center**  przy użyciu konta przejściowego (to, które zostanie przejść na nowe konto) i przejrzyj informacje o wszystkich klientach i wszystkich usługach aprowowanych dla tych klientów.

- Wyloguj się z tego konta.

## <a name="migrate-customer-accounts"></a>Migrowanie kont klientów

1. Zaloguj się **do Partner Center**  przy użyciu konta **Transitioning** (nowe) (to, do których przekierowywujesz klientów).

2. Wybierz **kafelek Klienci.**

3. Wybierz **pozycję Request a reseller relationship (Zażądaj relacji odsprzedawcy).** Zostanie wyświetlony domyślny komunikat e-mail do wysłania do klientów. Ten komunikat zawiera adres URL z identyfikatorem organizacji unikatowym dla nowego Partner Center konta.

4. **Akcja klienta:** Upewnij się, że każdy z aktywnych klientów, których chcesz migrować, odwiedzi ten adres URL. Podczas otwierania adresu URL klient jest monitowany o zalogowanie się do Office 365 portal. Klient korzysta z tego samego identyfikatora organizacji, który jest przez niego Office 365 portalami administracyjnym.

5. Po zalogowaniu administrator globalny  dla konta klienta jest monitowany o przesłanie umowy, która daje delegowane uprawnienia administratora do nowego konta CSP. Jeśli użytkownik się zgadza, klient zaznacza pole wyboru i zgadza się na autoryzowanie relacji.

Klienci będą pojawiać się na liście klientów partnera po przesłaniu umowy jeden po drugiej.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrowanie Office 365 i subskrypcji spoza platformy Azure opartych na użyciu

1. Po podpisaniu umowy przez klienta możesz ponownie utworzyć jego subskrypcje w ramach dzierżawy scentralizowanego partnera.

2. W **Partner Center** wybierz pozycję **Klienci.**

3. Otwórz nazwę firmy klienta, którego chcesz zmigrować.

4. Wybierz **pozycję Dodaj subskrypcję.**

5. Dodaj prawidłowe subskrypcje i liczby licencji z katalogu. Zweryfikuj przy użyciu informacji podanych **w tece Przechodzenie z** kont partnerów.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="listy klientów.":::

6. Wybierz **pozycję Prześlij.**

   Usługi są teraz udostępniane klientowi z konta **przejścia do** partnera.

7. Powtórz te kroki, aby przeprowadzić migrację subskrypcji dla wszystkich dodatkowych klientów.

Przed przejściem do następnej sekcji upewnij się, że wszystkie subskrypcje klientów istniejące w obszarze Przechodzenie z kont partnerów są ponownie aprowowane w ramach konta Przejścia **do** partnera. 

> [!NOTE]
> Partnerzy muszą wstrzymać  subskrypcje na koncie Przechodzenie z dzierżawy partnera w programie Partner Center tego  samego dnia, gdy te subskrypcje zostały przenoszone i ustawione w ramach konta Przechodzenie do dzierżawy partnera w dzierżawie partnera w programie Partner Center, aby zagwarantować, że nie wystąpią podwójne rozliczenia. Żądania pomocy technicznej zostaną odrzucone w przypadku środków ze względu na nakładanie się rozliczeń, które nie wyłączają prawidłowo **przejścia z** subskrypcji.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Wyłączanie subskrypcji Office 365 w obszarze Przechodzenie z konta partnera

Wyłączenie subskrypcji CSP w obszarze **Przechodzenie z** kont partnerów zatrzymuje wszelkie przyszłe rozliczenia. Nie trzeba ręcznie wyłączać subskrypcji platformy Azure, ponieważ subskrypcje platformy Azure są automatycznie wyłączane podczas procesu migracji.

1. Zaloguj się do **Partner Center** przy użyciu konta **Przechodzenie z** CSP i przejdź do listy klientów.

2. Otwórz klienta z subskrypcjami do wyłączenia, a następnie wybierz pierwszą ofertę do wyłączenia.

3. Ustaw wstrzymaną **subskrypcję** na , a następnie wybierz pozycję **Prześlij.**

   >[!Note]
   >Wstrzymanie subskrypcji gwarantuje, że podwójne rozliczenia nie będą występować.

   Subskrypcja jest **wyświetlona jako wstrzymana** na liście subskrypcji.

4. Powtórz te kroki dla wszystkich subskrypcji w ramach klienta. Sprawdź, czy wszystkie są wyświetlane **jako zawieszone.**

5. Wybierz następnego klienta z listy i powtórz proces wyłączania wszystkich subskrypcji.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrowanie subskrypcji platformy Azure opartych na użyciu

W przeciwieństwie Office 365 CSP platformy Azure, subskrypcje CSP oparte na użyciu nie muszą być migrowane ręcznie. Microsoft Azure Pomoc techniczna zmigruje subskrypcje platformy Azure i wszystkie wdrożone usługi lub zasoby z konta przechodzenia z kont odsprzedawcy programu **CSP** do konta odsprzedawcy programu **CSP.** Podczas tego przejścia nie będzie żadnych zakłóceń w działaniu usługi dla klienta.

1. Upewnij się, że konta klientów, które będą mieć zmigrowane subskrypcje platformy Azure, zaakceptowały umowę skojarzoną z nowym kontem **przechodzenia do** programu CSP.

2. Użytkownik powiadomi firmę Microsoft o tym, które konta klientów są gotowe do migracji, i poda nazwy firm tych klientów.

3. Firma Microsoft migruje subskrypcje platformy Azure oparte na użyciu i powiadamia o zakończeniu migracji.

4. Musisz potwierdzić, że subskrypcja platformy Azure w ramach konta  odsprzedawcy przejścia z programu **CSP** jest teraz oznaczona jako Partner Center w sekcji subskrypcje klienta.

5. Upewnij się, że subskrypcja platformy Azure w ramach konta  odsprzedawcy przejścia do programu **CSP** Partner Center w sekcji subskrypcje klientów.

   >[!Note]
   > Wyłączenie subskrypcji w ramach klienta nie zmienia wyglądu klienta na liście Klienci. Obecnie nie ma możliwości usunięcia klientów z listy. Partnerzy powinni unikać dodawania subskrypcji z powrotem do tych klientów ze swojego konta **przejścia** z konta w przyszłości.

6. Powtórz te kroki dla wszystkich subskrypcji w ramach wszystkich  klientów, aby zatrzymać przyszłe opłaty na kontach przejścia z. Partner otrzyma jedną końcową fakturę ze środków za liczbę nieużywanych dni między dniem anulowania a ostatnim dniem okresu rozliczeniowego. Po tym końcowym okresie rozliczeniowym nie będą generowane żadne przyszłe faktury.

### <a name="additional-information"></a>Dodatkowe informacje

- Wyłączenie subskrypcji z konta przechodzenia z programu **CSP** nie ma wpływu na usługę klienta końcowego, o ile usługa została aprowizowana z konta Przechodzenie do programu **CSP** przed wyłączeniem subskrypcji.

- Klient nie może korzystać z subskrypcji i nie generuje opłat po wstrzymaniu lub anulowaniu.

- Obecnie nie ma możliwości całkowitego usunięcia klienta z **listy** Klienci.
- 
    >[!Note]
    > Partnerzy muszą wstrzymać  subskrypcje na koncie przechodzenia z dzierżawy partnera w programie Partner Center tego  samego dnia, w który te subskrypcje są przenoszone i ustawione w ramach konta Przechodzenie do, aby zagwarantować, że nie wystąpią podwójne rozliczenia. Firma Microsoft nie będzie obsługiwać żądań środków ze względu na  nakładanie się rozliczeń, które występują z powodu nieprawidłowo ustawionego przejścia z subskrypcji na wstrzymane.

### <a name="simplify-migration-using-export"></a>Upraszczanie migracji przy użyciu funkcji eksportowania

Za pomocą **funkcji Eksportuj** możesz przechwycić subskrypcje, których chcesz użyć w nowej skonsolidowanej strukturze:

1. Wybierz **pozycję** Klienci Partner Center, aby wyświetlić listę klientów. 

2. Otwórz nazwę żądanego klienta.

3. Na stronie **Subskrypcje** wybierz pozycję Eksportuj **subskrypcje,** aby wyeksportować szczegóły subskrypcji do Excel pliku.

4. Użyj tej listy, aby ponownie utworzyć subskrypcje w nowej skonsolidowanej dzierżawie.

### <a name="api-registration"></a>Rejestracja interfejsu API

Aby uzyskać więcej informacji na temat rejestracji interfejsu API, zobacz [Konfigurowanie dostępu do interfejsu API w Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Następne kroki

- [Dostawca rozwiązań w chmurze programów regionalnych i walut, w których można sprzedawać oferty CSP](regional-authorization-overview.md)
