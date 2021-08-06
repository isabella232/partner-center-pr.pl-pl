---
title: Rejestracja transakcji
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Zarejestrowanie transakcji, która zwyciężyła w Partner Center, ułatwia firmie Microsoft zapewnienie większej liczby możliwości w przyszłości.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: 085e3418ee6689203dfb7be699acb9955e7ed7f3
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101620"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Rejestrowanie transakcji, które zostały wygrane w Partner Center

**Odpowiednie role:** Administrator poleceń

Możesz zarejestrować transakcje, które zostały Partner Center, podając dodatkowe informacje o kontrakcie. Te informacje pomagają nam zapewnić więcej możliwości w przyszłości.

Istnieją dwie ścieżki, które prowadzą do rejestracji transakcji:

- Utworzono nową ofertę w sekcji **Możliwości** współpracy sprzedaży, a Twoja transakcja spełnia kryteria rejestracji transakcji.
- Chcesz zgłosić zamkniętą umowę Połączenie isv, która nie została sprzedana razem z firmą Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Rejestrowanie transakcji pochodzącej z szansy sprzedaży

Jeśli chcesz zarejestrować ofertę pochodzącą z możliwości sprzedaży, Twoja transakcja musi spełniać następujące wymagania dotyczące uprawnień:

- Typ transakcji jest typu "co sell" lub "led" przez partnera (wybrano, aby umożliwić sprzedawcom firmy Microsoft wyświetlanie tej transakcji).
- W transakcji istnieje co najmniej jedno rozwiązanie kwalifikujące się do zachęt. Rozwiązanie kwalifikuje się do zachęty, jeśli zawiera co najmniej jeden z następujących tagów:
  - Wspólna sprzedaż IP platformy Azure
  - Business Applications Premium
  - Business Applications Standard
- Stan transakcji to "Won".
- Jeśli typ transakcji to współpraca sprzedaży, firma Microsoft musi zaakceptować zaproszenie lub oznaczać ofertę jako wygraną. Stan firmy Microsoft można sprawdzić, patrząc na kartę Microsoft poniżej szczegółów transakcji.

Jeśli spełniliśmy wymagania dotyczące uprawnień, zostanie automatycznie wyświetlony monit o zarejestrowanie transakcji przy użyciu przycisku Zarejestruj teraz wyświetlanego na pasku postępu transakcji: 

:::image type="content" source="images/register-deals.png" alt-text="Zrzut ekranu przedstawiający pasek postępu transakcji.":::

> [!NOTE]
> Jeśli element **rejestracji transakcji** nie jest pokazywany na pasku postępu transakcji dla Twojej transakcji, transakcja nie spełnia wszystkich wymagań dotyczących rejestracji transakcji.

Po kliknięciu **przycisku** Zarejestruj się teraz nastąpi przekierowanie do strony Rejestracja transakcji i zostanie wyświetlony monit o wypełnienie formularza, który zawiera wstępnie wypełnione informacje dotyczące klienta i rozwiązania. Wypełnij formularz, korzystając z poniższych instrukcji, a następnie kliknij pozycję **Zarejestruj.**

Podczas rejestracji zostanie utworzony jeden lub dwa rekordy rejestracji transakcji w zależności od rozwiązania.

- Jeśli Twoje rozwiązanie kwalifikuje się do korzystania z programu ISV Connect, zostanie utworzony rekord rejestracji programu ISV Connect. Ten rekord rejestracji transakcji będzie używany na potrzeby fakturowania.
- Jeśli Twoje rozwiązanie kwalifikuje się do zachęt do współpracy sprzedaży adresów IP, zostanie utworzony rekord rejestracji transakcji sprzedaży typu IP. Ten rekord rejestracji transakcji zostanie przejrzony i zatwierdzony lub odrzucony przez zespół oceniania transakcji sprzedaży.

## <a name="report-a-closed-isv-connect-deal"></a>Zgłaszanie zamkniętej umowy dotyczącej Połączenie isv

Aby zgłosić zamkniętą umowę Połączenie **isV,** przejdź do karty Rejestracja transakcji i kliknij pozycję + Zgłoś zamknięte umowy isv Połączenie transakcji.  Wypełnij wymagane pola i kliknij pozycję **Zarejestruj.** Ten rekord rejestracji transakcji będzie używany na potrzeby fakturowania.

## <a name="fill-out-the-deal-registration-form"></a>Wypełnij formularz rejestracji transakcji

> [!NOTE]
> Transakcje można filtrować według nazwy klienta, stanu i typu transakcji. W tym celu kliknij przycisk **Filtruj** w górnej części strony Rejestracja transakcji.

Niezależnie od tego, czy przyszliśmy do rejestracji transakcji ze względu na możliwość sprzedaży, czy zgłaszasz zamkniętą umowę ISV Połączenie, która nie została sprzedana razem z firmą Microsoft, zostanie wyświetlony monit o wypełnienie następujących pól w formularzu rejestracji transakcji.

- **Szczegóły klienta:** wprowadź **nazwę firmy** dla klienta i wybierz jego **kraj/region.** Następnie wprowadź wartość **city (miasto)** **i state/province (województwo).**
- **Rozwiązanie:** Wybierz rozwiązanie, które będzie używane dla transakcji. Jeśli nie widzisz odpowiedniego rozwiązania na liście, skontaktuj się z pomocą techniczną.
- **Typ kontraktu:** określ, czy ta transakcja jest **nową umową,** **czy** odnowieniem poprzedniego kontraktu.
- **Łączna wartość kontraktu:** łączna oczekiwana wartość dla zaangażowania. Ta wartość powinna obejmować wszystkie opłaty za oprogramowanie i usługę, ale nie koszty sprzętu. Pamiętaj, aby wybrać odpowiednią walutę.
- **Wartość rozwiązania:** łączna wartość rozwiązania w chmurze, które zostanie użyte w transakcji. Pamiętaj, aby uwzględnić wszystkie koszty związane z opłatami za oprogramowanie i konserwację, ale nie uwzględniać elementów zwrotnych, nie cyklicznych opłat za dostosowywanie ani bezpośrednio powiązanych opłat licencyjnych CSP zapłaconych przez firmę Microsoft.
- **Czy rozwiązanie zostanie wdrożone na platformie Azure? Jeśli nie, wybierz pozycję Inne:** wybierz pozycję **Azure** lub **Inne.**
- **Czy zużycie rozwiązania będzie działać w** dzierżawie partnera lub dzierżawie klienta? : Wybierz dzierżawę Klienta lub  **Dzierżawę partnera.**
- **Data rozpoczęcia kontraktu:** data rozpoczęcia kontraktu. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty pierwszej faktury. Domyślnie Partner Center nie pozwala na wprowadzenie daty rozpoczęcia wcześniejszej niż data podpisania kontraktu. Może to mieć wpływ na niektóre transakcje, takie jak wdrożenia adresów IP, które rozpoczynają się przed datą podpisania. Aby pomyślnie wprowadzić te transakcje, użyj  daty podpisywania kontraktu dla pól daty podpisywania i daty rozpoczęcia podczas przesyłania. (Kontrakt powinien jawnie określić czas trwania transakcji, aby można było prawidłowo obliczyć wartość ACV).
- **Data zakończenia kontraktu:** jeśli kontrakt zakończy się w określonej dacie, wybierz pozycję Ma **datę zakończenia** i podaj tę datę. Jeśli kontrakt nie ma określonej daty zakończenia, wybierz pozycję **Bezterminowy**. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty ostatniej lub najnowszej faktury.
- **Data podpisania** kontraktu: data podpisania umowy końcowej przez organizację i klienta. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty pierwszej faktury.
- **Osoba kontaktowa** rejestracji: **imię,** **nazwisko,** **Telefon**  numer i adres e-mail osoby w organizacji, z którą możemy się skontaktować, jeśli potrzebujemy więcej szczegółowych informacji na temat podanych tutaj informacji.

Po ukończeniu wszystkich sekcji strony kliknij pozycję **Zarejestruj**.

- Jeśli transakcja jest isv isv Połączenie deal, zauważysz, że stan transakcji to "Przesłane, Ukończone". W przypadku tego rekordu rejestracji transakcji nie są wymagane żadne dalsze działania. Ten rekord będzie używany do fakturowania.
- Jeśli transakcja jest ofertą sprzedaży typu IP, zauważysz, że stan transakcji to "Przesłane". Zespół przeglądów transakcji dotyczących współpracy sprzedaży firmy Microsoft przejmie informacje podane w tym rekordzie rejestracji transakcji. W razie potrzeby zespół reenzentów zażąda od Ciebie większej liczby akcji lub bezpośrednio zatwierdzi/odrzuci umowę.
- Jeśli rejestrujesz ofertę pochodzącą z szansy sprzedaży i zobaczysz, że utworzono dwie rekordy rejestracji transakcji, oznacza to, że rozwiązanie w Twojej transakcji kwalifikuje się zarówno do sprzedaży isv Połączenie, jak i do współsieć ip. Rekord isV Połączenie będzie używać do fakturowania. Rekord współsieć ip będzie przeglądany przez zespół weryfikacji transakcji sprzedaży.

## <a name="simplified-deal-registration-for-commercial-marketplace-transactions"></a>Uproszczona rejestracja transakcji dla transakcji na platformie handlowej

Co-Sell transakcje za pośrednictwem [](/azure/marketplace/) platformy handlowej skorzystają na znacznym uproszczeniu formularza rejestracji transakcji.  Ponadto transakcje w ramach transakcji za pośrednictwem komercyjnej platformy handlowej nie będą wymagały wywołań dodatkowego przeglądu transakcji, co pozwoli zaoszczędzić czas operacyjny i nakład pracy.

Wystarczy podać tylko trzy informacje:

1. Wskaż (pole wyboru) transakcję za transakcję lub będzie ona zawierana za pośrednictwem platformy handlowej.
2. Szacowana data transakcji (MM-DD-YYYY).
3. Rejestrowanie danych kontaktowych partnera na wypadek pytań dotyczących transakcji.
