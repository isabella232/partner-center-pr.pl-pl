---
title: Konsolidacja dzierżawy regionalnej autoryzacji dostawcy usług kryptograficznych
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Te instrukcje służą do konsolidacji dzierżawców dla różnych krajów/regionów. Obejmuje to procedurę migrowania kont klientów i subskrypcji klientów.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502574"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instrukcje dotyczące konsolidacji dzierżawy regionalnej autoryzacji dostawcy CSP

**Dotyczy**

- Centrum partnerskie Microsoft Cloud for US Government

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny

\[Niektóre informacje odnoszą się do wstępnie wydanego produktu, który można w znacznym stopniu modyfikować przed udostępnieniem handlowym. Firma Microsoft nie udziela żadnych gwarancji, jawnych lub domniemanych, w odniesieniu do informacji podanych w tym miejscu.\]

Można skonsolidować dzierżawców dla swojej firmy. Te instrukcje służą do konsolidacji dzierżawców dla różnych krajów/regionów.

>[!NOTE]  
>Użytkownik musi mieć świadomość wszystkich zainicjowanych subskrypcji i liczby licencji dla każdego z klientów na koncie, z którego się przechodzi. Będziesz ponownie obsługiwać te same dokładne subskrypcje z tymi samymi liczbami licencji w ramach nowego centralnego konta CSP w ramach procesu migracji. Korzystając z funkcji Eksportuj listę, można utworzyć listę klientów, którzy mają przechodzenie do scentralizowanej dzierżawy.  Po zakończeniu konsolidacji nie można przywrócić poprzedniego stanu dzierżawy. Może być również wymagana akcja klienta.

## <a name="prepare-for-migration"></a>Przygotowanie do migracji

- Zaloguj się do **Centrum partnerskiego**  przy użyciu konta **przechodzenia** (zostanie ono przenoszone na nowe konto) i przejrzyj wszystkich klientów oraz wszystkie usługi zainicjowane dla tych klientów.

- Wyloguj się z tego konta.

## <a name="migrate-customer-accounts"></a>Migrowanie kont klientów

1. Zaloguj się do **Centrum partnerskiego**  przy użyciu konta **przechodzenia** (nowe) (do którego są przenoszone klienci).

2. Wybierz pozycję **Klienci**.

3. Wybierz pozycję **Żądaj relacji odsprzedawcy**. Zostanie wyświetlona domyślna wiadomość e-mail do wysłania do klientów. Ten komunikat zawiera adres URL z unikatowym IDENTYFIKATORem organizacji dla nowego konta Centrum partnerskiego.

4. **Akcja klienta:** Upewnij się, że każdy aktywny klient, który ma zostać zmigrowany, odwiedzi ten adres URL. Podczas otwierania adresu URL klient zostanie poproszony o zalogowanie się w portalu pakietu Office 365. Klient loguje się przy użyciu tego samego identyfikatora organizacji, który służy do uzyskiwania dostępu do portali administratorów platformy Azure i pakietu Office 365.

5. Po zalogowaniu Administrator globalny **konta klienta** zostanie poproszony o przesłanie umowy zapewniającej uprawnienia administratora delegowanego do nowego konta dostawcy CSP. Jeśli zgadzają się, klient wybierze pole wyboru i zgadza się na autoryzację relacji.

Po przesłaniu umowy klient zostanie wyświetlony na liście klientów partnera.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrowanie subskrypcji pakietu Office 365 i nie korzystających z platformy Azure

1. Po podpisaniu umowy przez klienta możesz ponownie utworzyć swoje subskrypcje w ramach dzierżawy scentralizowanego partnera.

2. W **centrum partnerskim** wybierz pozycję **klienci**.

3. Otwórz nazwę firmy dla klienta, który ma zostać zmigrowany.

4. Wybierz pozycję **Dodaj subskrypcję**.

5. Dodaj prawidłowe subskrypcje i liczby licencji z wykazu. Sprawdź informacje zawarte w **przejściu z** kont partnerów.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Lista klientów":::

6. Wybierz pozycję **Prześlij.**

   Usługi są teraz udostępniane klientowi z **przechodzenia do** konta partnera.

7. Powtórz te kroki, aby przeprowadzić migrację subskrypcji dla wszystkich dodatkowych klientów.

Przed przejściem do następnej sekcji upewnij się, że wszystkie subskrypcje klienta istniejące w ramach **przejścia z** kont partnerów są ponownie inicjowane w ramach **przejścia do** konta partnera.

> [!NOTE]
> Partnerzy muszą zawiesić subskrypcje dotyczące **przejścia z** konta dzierżawy partnera w centrum partnerskim tego samego dnia, w którym te subskrypcje są przenoszone i konfigurowane w ramach **przejścia do** konta dzierżawcy partnera w Centrum partnerskiego w celu zapewnienia podwójnego rozliczania. Żądania pomocy technicznej będą odrzucane w przypadku kredytów z powodu jakiegokolwiek nakładania się opłat, które wystąpiły od nieprawidłowego wyłączenia **przejścia z** subskrypcji.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Wyłączanie subskrypcji pakietu Office 365 w ramach przejścia z konta partnera

Wyłączenie subskrypcji dostawcy usług kryptograficznych w ramach **przejścia z** kont partnerskich powoduje zatrzymanie wszelkich przyszłych rozliczeń. Nie musisz ręcznie wyłączać subskrypcji platformy Azure, ponieważ subskrypcje platformy Azure są automatycznie wyłączane podczas procesu migracji.

1. Zaloguj się do **Centrum partnerskiego** przy użyciu **przejścia z** konta CSP i przejdź do listy klient.

2. Otwórz klienta z subskrypcjami, aby wyłączyć, a następnie wybierz pierwszą ofertę do wyłączenia.

3. Ustaw subskrypcję na **zawieszone**, a następnie wybierz pozycję **Prześlij**.

   >[!Note]
   >Wstrzymanie subskrypcji gwarantuje, że podwójne rozliczenie nie nastąpi.

   Subskrypcja zostanie **wyświetlona** na liście subskrypcje.

4. Powtórz te kroki dla wszystkich subskrypcji w ramach klienta. Sprawdź, czy wszystkie wyświetlanie zostały **zawieszone.**

5. Wybierz następnego klienta z listy i powtórz proces wyłączania wszystkich subskrypcji.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrowanie subskrypcji opartych na użyciu platformy Azure

W przeciwieństwie do subskrypcji programu CSP pakietu Office 365, Azure, subskrypcje programu CSP oparte na użyciu nie muszą być migrowane ręcznie. Obsługa Microsoft Azure przeprowadzi migrację subskrypcji platformy Azure i wszystkich wdrożonych usług lub zasobów z **przechodzenia z** kont odsprzedawcy programu CSP do **przejścia do** konta odsprzedawcy programu CSP. W trakcie tego przejścia nie będzie zakłócać działania usługi dla klienta.

1. Upewnij się, że konta klientów, dla których zostały zmigrowane subskrypcje platformy Azure, zaakceptowały umowę, która zostanie skojarzona z nowym **przejściem do** konta dostawcy CSP.

2. Powiadomimy firmę Microsoft o tym, które konta klientów są gotowe do migracji, i podają nazwy firmowe tego klienta.

3. Firma Microsoft migruje subskrypcje oparte na użyciu platformy Azure i powiadamia o zakończeniu migracji.

4. Musisz upewnić się, że subskrypcja platformy Azure w ramach **przejścia z** konta odsprzedawcy dostawcy CSP jest teraz oznaczona jako **zawieszona** w centrum partnerskim w sekcji subskrypcje klienta.

5. Upewnij się, że w ramach subskrypcji platformy Azure w ramach **przejścia do** konta odsprzedawcy CSP jest teraz wyświetlany stan **aktywny** w centrum partnerskim w sekcji subskrypcje klienta.

   >[!Note]
   > Wyłączenie subskrypcji w ramach klienta nie powoduje zmiany wyglądu klienta na liście klientów. Obecnie nie ma możliwości usunięcia klientów z listy. Partnerzy powinni unikać dodawania **subskrypcji z powrotem** do klientów w przyszłości.

6. Powtórz te kroki dla wszystkich subskrypcji w ramach wszystkich klientów, aby zrezygnować z przyszłych opłat za **przejście z** kont. Partner otrzyma jedną fakturę ostateczną ze środkiem za liczbę nieużywanych dni między dniem anulowania a ostatnim dniem okresu rozliczeniowego. Nie będą generowane żadne przyszłe faktury po upływie ostatecznego okresu rozliczeniowego.

### <a name="additional-information"></a>Dodatkowe informacje

- Wyłączenie **subskrypcji z konta CSP nie** ma wpływu na usługę klienta końcowego, o ile usługa została zainicjowana przy użyciu **przejścia do** konta CSP przed wyłączeniem subskrypcji.

- Nie można używać subskrypcji przez klienta i nie generują opłat po wstrzymaniu lub anulowaniu.

- Obecnie nie istnieje sposób na całkowite usunięcie klienta z listy **klientów** .
- 
    >[!Note]
    > Partnerzy muszą zawiesić subskrypcje dotyczące **przejścia z** konta dzierżawcy partnera w centrum partnerskim tego samego dnia, w którym subskrypcje są przenoszone i konfigurowane w ramach **przejścia do** konta w celu zapewnienia podwójnego rozliczania. Firma Microsoft nie będzie obsługiwać próśb o kredyty ze względu na to, że wystąpiły zmiany w rozliczeniach, które wynikają z nieprawidłowego ustawienia **przejścia z** subskrypcji na zawieszone.

### <a name="simplify-migration-using-export"></a>Uproszczenie migracji przy użyciu eksportu

Za pomocą **funkcji eksportu** można przechwytywać subskrypcje, których należy użyć w nowej strukturze skonsolidowanej:

1. Wybierz pozycję **klienci** w centrum partnerskim, aby wyświetlić listę klientów. 

2. Otwórz żądaną nazwę klienta.

3. Na stronie **subskrypcje** wybierz pozycję **Eksportuj subskrypcje** , aby wyeksportować szczegóły subskrypcji do pliku programu Excel.

4. Użyj tej listy, aby ponownie utworzyć subskrypcje w nowej konsolidowanej dzierżawie.

### <a name="api-registration"></a>Rejestracja interfejsu API

Aby uzyskać więcej informacji na temat rejestracji interfejsu API, zobacz [Konfigurowanie dostępu do interfejsu API w centrum partnerskim](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Następne kroki

- [Program dostawcy rozwiązań w chmurze — rynki regionalne i waluty, w których można sprzedawać oferty CSP](regional-authorization-overview.md)
