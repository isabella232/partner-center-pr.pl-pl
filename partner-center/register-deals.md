---
title: Rejestracja transakcji
ms.topic: article
ms.date: 09/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Zarejestrowanie transakcji, która zwyciężyła w Partner Center, ułatwia firmie Microsoft zapewnienie większej liczby możliwości w przyszłości.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: 22dcf93c5028716fc3810c826abe1819459e58e1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248196"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Rejestrowanie transakcji, które zostały wygrane w Partner Center

**Odpowiednie role:** Administrator poleceń

Możesz zarejestrować transakcje, które zostały Partner Center, podając dodatkowe informacje o kontrakcie. Te informacje pomagają nam zapewnić więcej możliwości w przyszłości.

Istnieją dwie ścieżki, które prowadzą do rejestracji transakcji:

- Utworzono nową ofertę w sekcji **Możliwości** współpracy sprzedaży, a Twoja transakcja spełnia kryteria rejestracji transakcji.
- Chcesz zgłosić zamkniętą umowę Połączenie isv, która nie została sprzedana razem z firmą Microsoft.

> [!IMPORTANT]
> Jeśli transakcja kwalifikuje się do rejestracji transakcji, upewnij się, że istnieje przerwa 72 godzin między utworzeniem transakcji i oznaczeniem transakcji jako wygranych. Zamknięcie transakcji jako wygranych wcześniej może spowodować odrzucenie rejestracji transakcji.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Rejestrowanie transakcji pochodzącej z szansy sprzedaży

Jeśli chcesz zarejestrować ofertę pochodzącą z możliwości współpracy sprzedaży, Twoja transakcja musi spełniać następujące wymagania dotyczące uprawnień:

- Typ transakcji to współpraca lub współpraca (wybrano, aby zezwolić sprzedawcom firmy Microsoft na wyświetlanie tej transakcji).
- Wartość transakcji jest większa lub równa 25 000 USD. Konwersja waluty jest oparta na miesięcznych [kursach wymiany publikowanych](https://www.reuters.com/markets/currencies) przez firmę Reuters.
- Konto klienta wybrane do transakcji jest zarządzane przez firmę Microsoft. Są to konta, w których zespół sprzedaży firmy Microsoft ma istniejącą relację z firmą.
- W transakcji istnieje co najmniej jedno rozwiązanie kwalifikujące się do zachęt. Rozwiązanie kwalifikuje się do zachęty, jeśli zawiera co najmniej jeden z następujących tagów:
  - Wspólna sprzedaż IP platformy Azure
  - Business Applications Premium
  - Business Applications Standard
- Stan transakcji to Won **(Wygrana).**
- Jeśli typ transakcji to Co-sell, firma Microsoft musi zaakceptować zaproszenie lub oznaczyła ofertę jako wygraną. Stan firmy Microsoft można sprawdzić, patrząc na kartę Microsoft poniżej szczegółów transakcji.

> [!Important]
> Zarejestruj ofertę tylko wtedy, gdy nazwa firmy i kwalifikujące się do zachęty rozwiązanie w transakcji są wyraźnie wymienione w umowie z klientem.

Jeśli zostały spełnione wymagania dotyczące uprawnień, zostanie automatycznie wyświetlony monit o  zarejestrowanie transakcji przy użyciu przycisku Zarejestruj teraz wyświetlanego na pasku postępu transakcji:

:::image type="content" source="images/register-deals.png" alt-text="Zrzut ekranu przedstawiający pasek postępu transakcji.":::

> [!NOTE]
> Jeśli element **rejestracji transakcji** nie jest pokazywany na pasku postępu transakcji dla Twojej transakcji, transakcja nie spełnia wszystkich wymagań dotyczących rejestracji transakcji.

Możesz zarejestrować ofertę natychmiast po oznaczaniu transakcji jako wygraną lub w późniejszym momencie za pomocą przycisku Zarejestruj teraz cyklu życia transakcji. Po zarejestrowaniu transakcji możesz wyświetlić postęp weryfikacji transakcji z tego samego cyklu życia. Jeśli w firmie są wymagane jakiekolwiek działania, w widoku cyklu życia transakcji są wyświetlane odpowiednie błędy. Transakcja przechodzi w stan zamknięty po zakończeniu walidacji transakcji.

### <a name="combinations"></a>Kombinacji

W poniższej tabeli przedstawiono kombinacje osób, które mogą zostać zaproszone na tym etapie transakcji.

|**Oryginalny typ transakcji**|**KtoTo można zapraszać**|**Uwagi**|
|-----|:-----|:-----|
|Prywatny|Firma Microsoft i/lub inni partnerzy|Transakcja zostanie uaktualniona do współs sprzedaży, jeśli zostanie zaproszona firma Microsoft.|
|Prywatny|Zespół sprzedaży firmy Microsoft do wyświetlania transakcji|Transakcja zostanie uaktualniona do zespołu prowadzonego przez partnera, gdy zespół sprzedaży firmy Microsoft będzie miał wgląd w transakcje.|
|Prowadzone przez partnera|Firma Microsoft i/lub inni partnerzy|Transakcja zostanie uaktualniona do współs sprzedaży, jeśli zostanie zaproszona firma Microsoft.|
|Co-sell (Współsieć)|Inni partnerzy|Innych partnerów można zaprosić tylko wtedy, gdy Twoja firma zainicjowała umowę. Partnerom nie można zapraszać na transakcje na karcie Przychodzące.|
|Partner to partner without Microsoft|Microsoft|Transakcja zostanie uaktualniona do transakcji co-sell.|
|Partner to partner without Microsoft|Inni partnerzy||

Po kliknięciu **przycisku** Zarejestruj teraz nastąpi przekierowanie do strony Rejestracja transakcji i zostanie wyświetlony monit o wypełnienie formularza, który zawiera wstępnie wypełnione informacje o kliencie i rozwiązaniu. Wypełnij formularz, korzystając z poniższych instrukcji, a następnie kliknij pozycję **Zarejestruj.**

Podczas rejestracji zostanie utworzony jeden lub dwa rekordy rejestracji transakcji w zależności od rozwiązania.

- Jeśli Twoje rozwiązanie kwalifikuje się do korzystania z programu ISV Connect, zostanie utworzony rekord rejestracji programu ISV Connect. Ten rekord rejestracji transakcji będzie używany na potrzeby fakturowania.
- Jeśli Twoje rozwiązanie kwalifikuje się do zachęt do współpracy sprzedaży ip, zostanie utworzony rekord rejestracji umowy dotyczącej współpracy sprzedaży dla adresu IP. Ten rekord rejestracji transakcji zostanie przejrzony i zatwierdzony lub odrzucony przez zespół do przeglądu transakcji sprzedaży.

## <a name="report-a-closed-isv-connect-deal"></a>Zgłaszanie zamkniętej umowy dotyczącej Połączenie isv

Aby zgłosić zamkniętą umowę Połączenie isv, przejdź do karty Rejestracja transakcji i kliknij pozycję + Zgłoś zamkniętego  **isv Połączenie transakcji.** Wypełnij wymagane pola i kliknij pozycję **Zarejestruj.** Ten rekord rejestracji transakcji będzie używany na potrzeby fakturowania.

## <a name="fill-out-the-deal-registration-form"></a>Wypełnij formularz rejestracji transakcji

> [!NOTE]
> Transakcje można filtrować według nazwy klienta, stanu i typu transakcji. W tym celu kliknij przycisk **Filtruj** w górnej części strony Rejestracja transakcji.

Niezależnie od tego, czy masz do czynienia z rejestracją transakcji z możliwości współpracy sprzedaży, czy zgłaszasz zamkniętą umowę isv Połączenie, która nie została sprzedana razem z firmą Microsoft, zostanie wyświetlony monit o wypełnienie następujących pól w formularzu rejestracji transakcji.

- **Szczegóły klienta:** wprowadź **nazwę firmy** dla klienta i wybierz jego **kraj/region.** Następnie wprowadź nazwę **City (Miasto)** **i State/Province (Województwo).**
- **Rozwiązanie:** Wybierz rozwiązanie, które będzie używane dla transakcji. Jeśli nie widzisz odpowiedniego rozwiązania na liście, skontaktuj się z pomocą techniczną.
- **Typ kontraktu:** określ, czy ta transakcja jest **nową umową,** **czy** odnowieniem poprzedniego kontraktu.
- **Łączna wartość kontraktu:** łączna oczekiwana wartość dla zaangażowania. Ta wartość powinna obejmować wszystkie opłaty za oprogramowanie i usługę, ale nie koszty sprzętu. Pamiętaj, aby wybrać odpowiednią walutę.
- **Wartość rozwiązania:** łączna wartość rozwiązania w chmurze, które zostanie użyte w transakcji. Pamiętaj, aby uwzględnić wszystkie koszty związane z opłatami za oprogramowanie i konserwację, ale nie obejmują elementów z możliwością ponownego zwrotu, cyklicznych opłat za dostosowywanie ani bezpośrednio skojarzonych opłat licencyjnych CSP zapłaconych przez firmę Microsoft.
- **Czy rozwiązanie zostanie wdrożone na platformie Azure? Jeśli nie, wybierz pozycję Inne:** wybierz pozycję **Azure** lub **Inne.**
- **Czy zużycie rozwiązania będzie działać w** dzierżawie partnera lub dzierżawie klienta? : Wybierz dzierżawę Klient lub  **Dzierżawę partnera.**
- **Data rozpoczęcia kontraktu:** data rozpoczęcia kontraktu. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty pierwszej faktury. Domyślnie Partner Center nie pozwala na wprowadzenie daty rozpoczęcia wcześniejszej niż data podpisania kontraktu. Może to mieć wpływ na niektóre transakcje, takie jak wdrożenia adresów IP, które rozpoczną się przed datą podpisania. Aby pomyślnie wprowadzić te transakcje, użyj  daty podpisania kontraktu w polach daty podpisania i daty rozpoczęcia podczas przesyłania. (Kontrakt powinien jawnie określić czas trwania transakcji, aby można było prawidłowo obliczyć wartość ACV).
- **Data zakończenia kontraktu:** jeśli kontrakt zakończy się w określonej dacie, wybierz pozycję Ma **datę zakończenia** i podaj tę datę. Jeśli kontrakt nie ma określonej daty zakończenia, wybierz pozycję **Bezterminowe**. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty ostatniej lub najnowszej faktury.
- **Data podpisania** kontraktu: data podpisania umowy końcowej przez organizację i klienta. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty pierwszej faktury.
- **Osoba kontaktowa** rejestracji: **imię,** **nazwisko,** **Telefon** i  adres e-mail osoby w organizacji, z którą możemy się skontaktować, jeśli potrzebujemy więcej szczegółowych informacji na temat podanych tutaj informacji.

Po ukończeniu wszystkich sekcji strony kliknij pozycję **Zarejestruj.**

- Jeśli transakcja jest złożona z Połączenie isv, można zauważyć, że stan transakcji to **Przesłana, Ukończono.** W przypadku tego rekordu rejestracji transakcji nie są wymagane żadne dalsze działania. Ten rekord zostanie użyty do fakturowania.
- Jeśli transakcja jest ofertą sprzedaży typu IP, możesz zauważyć, że stan transakcji to **Przesłana.** Zespół reenzentów transakcji sprzedaży firmy Microsoft przejmie informacje podane w rekordzie rejestracji transakcji. W razie potrzeby zespół reenzentów zażąda od Ciebie więcej akcji lub bezpośrednio zatwierdzi lub odrzuci ofertę.
- Jeśli rejestrujesz ofertę pochodzącą z możliwości współpracy sprzedaży i zobaczysz, że utworzono dwa rekordy rejestracji transakcji, oznacza to, że rozwiązanie w Twojej transakcji kwalifikuje się zarówno do sprzedaży dla isv Połączenie, jak i do współsieć ip. Rekord dostawcy Połączenie będzie używać do fakturowania. Rekord współs sprzedaży dla adresu IP zostanie przejrzęcy przez zespół weryfikacji transakcji sprzedaży.

## <a name="simplified-deal-registration-for-commercial-marketplace-transactions"></a>Uproszczona rejestracja transakcji dla transakcji na platformie handlowej

Transakcje na platformie handlowej zwyciężą w zakresie sprzedaży, co spowoduje znaczne uproszczenie formularza rejestracji transakcji. [](/azure/marketplace/)  Ponadto transakcje w ramach komercyjnej platformy handlowej nie będą wymagać wywołań dodatkowego przeglądu transakcji, co pozwoli zaoszczędzić czas operacyjny i nakład pracy.

Wystarczy podać tylko trzy informacje:

1. Wskaż, zaznaczając pole wyboru, jeśli transakcja jest transakcją lub będzie transakcją za pośrednictwem platformy handlowej.
2. Szacowana data transakcji (w `mm-dd-yyyy` formacie).
3. Rejestrowanie danych kontaktowych partnera na wypadek pytań dotyczących transakcji.
