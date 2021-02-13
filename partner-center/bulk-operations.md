---
title: Operacje zbiorcze za pośrednictwem plików programu Excel w odwołaniach
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak pobierać, tworzyć i aktualizować możliwości wspólnej sprzedaży przy użyciu plików programu Excel
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 831fbc294bfd82caef77489f74747bb32cf0b12c
ms.sourcegitcommit: 64b43ad8fb7bb56628450bea06b9cd2606c36b03
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2021
ms.locfileid: "100334592"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Operacje zbiorcze dla wspólnych możliwości sprzedaży przy użyciu plików z wartościami rozdzielanymi przecinkami (CSV)

**Odpowiednie role**

- Administrator odwołań
- Użytkownik z odwołaniami

Operacje zbiorcze w centrum partnerskim mogą pomóc firmie eksportować i importować dane z możliwością sprzedaży. Przejdź do strony z możliwością współsprzedaży, aby znaleźć linki importu i eksportu w prawym górnym rogu transparentu tytułu strony. Korzystając z tej funkcji, użytkownicy z uprawnieniami **administratora** i odniesień do użytkowników mogą korzystać z tego **konta** .

> [!IMPORTANT]
> Akcje create/Update wykonywane za pomocą importu zbiorczego nie są odwracalne. Podczas modyfikowania lub tworzenia dużej liczby rekordów należy zachować ostrożność. Po utworzeniu transakcji można modyfikować tylko podzestaw pól. **Żadna akcja nie będzie dozwolona, gdy jakakolwiek transakcja osiągnie stan terminalu, taki jak odrzucone/wygasłe/wykorzystane/utracone.**

## <a name="exporting-co-sell-opportunities"></a>Eksportowanie możliwości wspólnej sprzedaży

Poniżej znajdują się szczegółowe informacje o funkcji eksportu

- Aby wyeksportować **maksymalnie 5000 rekordów** , kliknij przycisk Eksportuj.
- Pobrane transakcje będą oparte na poziomach dostępu. Administratorzy odwołań i użytkownicy odwołań mogą uzyskać różne wyniki w zależności od ich zakresu i włączenia jako członków zespołu w ramach transakcji. Dowiedz się więcej o [uprawnieniach odwołań](permissions-overview.md#manage-referrals).
- Funkcja eksportu przyjmuje do konta bieżącą kartę na stronie możliwości wspólnej sprzedaży i filtry, które zostały zastosowane.
- Zostanie wygenerowany plik CSV ze wszystkimi danymi opartymi na zastosowanych filtrach.
- Pobranie rekordów może potrwać do 1 minuty.
- Nie musisz czekać na ukończenie akcji pobierania. Nawet jeśli przejdziesz do innych stron w centrum partnerskim, plik zostanie pobrany zaraz po zakończeniu eksportu funkcji.
- Pobrany plik można ponownie wykorzystać, aby zmodyfikować szczegóły dotyczące transakcji i przekazać je w celu zaktualizowania wszystkich rekordów.

## <a name="importing-co-sell-opportunities"></a>Importowanie możliwości wspólnej sprzedaży

- Można utworzyć lub zaktualizować **maksymalnie 1000 rekordów** przy użyciu funkcji importowania.
- Możesz utworzyć szablon od podstaw, pobierając szablon ze strony importu w centrum partnerskim.
- Możesz również użyć funkcji eksportu, aby pobrać istniejące rekordy i zaktualizować je.
- Jeśli plik ma więcej niż 1000 rekordów, nie można go przetworzyć.
- Po przetworzeniu pliku zostanie wyświetlone podsumowanie zawierające liczbę odwołań, które zostały utworzone, zaktualizowane i nieprzetwarzane, w ostatniej karcie pliku przetwarzania.
- Możesz pobrać szczegóły przetworzonych rekordów, naprawić wszystkie błędy i przekazać ten sam plik, aby utworzyć lub zaktualizować rekordy, które nie powiodły się w poprzednim uruchomieniu. **Usuń wszystkie pomyślne rekordy z pliku przed przekazaniem poprawionych rekordów, które nie powiodły się w poprzednim przebiegu.**
- Aby dodać więcej rozwiązań, Dodaj dodatkowe kolumny obok rozwiązania 1 i użyj nazwy kolumny jako rozwiązania X, gdzie X reprezentuje liczbę rozwiązań w ramach transakcji. Na przykład rozwiązanie 2, rozwiązanie 3.
- Do rozpatrzenia można dodać do 50 rozwiązań.
- Aby dodać więcej członków zespołu, Dodaj dodatkowe kolumny obok pozycji członek zespołu 1 i użyj nazwy kolumny jako członka zespołu X, gdzie X reprezentuje liczbę członków zespołu w ramach transakcji. Na przykład członek zespołu 2, członek zespołu 3.
- Do transakcji możesz dodać maksymalnie 50 członków zespołu.

> [!NOTE]
> Nie musisz czekać na ukończenie przetwarzania. Szczegóły ostatnio przetworzonego pliku będą dostępne do pobrania po zakończeniu przetwarzania. **W przypadku przekazywania plików z 1000 rekordów może upłynąć do 10 minut.**

> [!IMPORTANT]
> Przeczytaj uważnie wszystkie instrukcje i sprawdź format każdej kolumny w poniższej tabeli przed utworzeniem lub aktualizacją transakcji przy użyciu plików CSV w centrum partnerskim.

|**Nazwa kolumny**|**Czy jest to wymagane?**|**Opis**|**Przykładowe wartości**|
|-----|:-----|:---------|:---|
błędy|Nie|Błędy, Jeśli dowolne powiązane z operacjami tworzenia/aktualizacji w. r. t do odwołań zostaną uwzględnione w tej kolumnie. Jeśli występuje wiele błędów, wszystkie z nich zostaną wyświetlone oddzielone średnikami.|Brak obowiązkowego rozwiązania pola 1|
Identyfikator zaangażowania|Nie|Identyfikator zaangażowania jest generowany przez system odwołań Centrum partnerskiego firmy Microsoft. Nie jest wymagane do utworzenia nowego odwołania. Jeśli aktualizujesz rekord, możesz użyć istniejącego identyfikatora zaangażowania.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Identyfikator polecenia|Nie|Identyfikator odwołania jest generowany przez system odwołań Centrum partnerskiego firmy Microsoft. Nie jest wymagane do utworzenia nowego odwołania. Wypełnij ją IDENTYFIKATORem odwołania, jeśli aktualizujesz istniejący rekord.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nazwa transakcji|Tak|Przyjazna nazwa dla transakcji dla odwołania.|Transakcja wiosny Zjednoczonego Królestwa
Nazwa klienta|Tak|Nazwa firmy klienta. Użyj prawnej nazwy organizacji do szybkiego dopasowania po stronie firmy Microsoft.|Contoso Corporation
Wiersz adresu klienta 1|Tak|Wiersz adresu 1 firmy klienta. |Jeden sposób firmy Contoso
Wiersz adresu klienta 2|Nie|Wiersz adresu 2 firmy klienta.|NE 148
Miasto klienta|Tak|Miasto, w którym znajduje się organizacja klienta.|Redmond
Stan klienta|Nie|Stan, w którym znajduje się organizacja klienta.|Waszyngton
Kod pocztowy klienta|Nie|Kod pocztowy regionu, w którym znajduje się organizacja klienta.|98052
Kraj klienta|Tak|Kraj/region, w którym znajduje się organizacja klienta. Użyj trzech kodów krajów, jak wspomniano [tutaj]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|USA
Identyfikator klienta D-N-S|Nie|Spróbuj pobrać identyfikator DUNS organizacji klienta. Pomoże to w szybszym dopasowaniu organizacji klienta po stronie firmy Microsoft, co pomaga szybciej przypisywać sprzedającemu. Identyfikator DUNS można bezpłatnie uzyskać z tej [witryny sieci Web](https://www.dnb.com/duns-number/lookup.html).|81466849
Imię kontaktu z klientem|Zależy od|Imię jest wymagane tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Imię kontaktu podstawowego od organizacji klienta pracującego nad tym postępowaniem.|Michał
Nazwisko osoby kontaktowej klienta|Zależy od|Nazwisko jest wymagane tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Nazwisko głównej osoby kontaktowej w organizacji klienta, która pracuje nad tym postępowaniem.|Customer
Numer telefonu kontaktowego klienta|Zależy od|Numer telefonu jest wymagany tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Numer telefonu podstawowego kontaktu z organizacji klienta pracującego nad tym postępowaniem.|9999999999
Adres E-mail osoby kontaktowej klienta|Zależy od|Adres e-mail jest wymagany tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Adres e-mail kontaktu podstawowego od organizacji klienta pracującego nad tym postępowaniem.|john.customer@contoso.com
Stan odwołania partnera|Tak|Wskazuje stan transakcji z perspektywy firmy. Wymagane, jeśli próbujesz utworzyć lub zmodyfikować odwołanie. Jeśli próbujesz utworzyć nową transokazję, użyj **nowej** . Akceptowane wartości są udokumentowane w [tym miejscu](https://docs.microsoft.com/partner/develop/referral-resources#referralstatus).|Aktywna
Stan pododwołania do partnera|Tak|Wskazuje dokładny stan transakcji. Użyj **zaakceptowanych** w przypadku próby utworzenia nowej transakcji. Jest również wymagane, jeśli modyfikujesz istniejące odwołanie. Akceptowane wartości są udokumentowane w [tym miejscu](https://docs.microsoft.com/partner/develop/referral-resources#referralsubstatus).|Zaakceptowano
Stan odwołania firmy Microsoft|Zależy od|Wskazuje stan żądania współsprzedawcy wysłanego do pomocy firmy Microsoft. Jest to pole tylko do odczytu. Wszelkie zmiany wprowadzone w tym polu podczas importowania danych zostaną zignorowane.| Oczekiwanie
Przyczyna odrzucenia/utraty|Zależy od| Te informacje są wymagane tylko w przypadku zmiany stanu podrzędnego pola na odrzucone lub utracone. W przeciwnym razie można zignorować tę kolumnę. <br/> **Wprowadź liczbę na podstawie poniższych opcji** <br/><br/> **1**— budżet projektu jest nieodpowiedni  <br/> **2**— klient nie odpowiedział  <br/> **3**— klient wybrał innego dostawcę  <br/> **4** — wymagania klienta nie zostały spełnione  <br/> **5** — nie do klienta <br/> **6**— proponowany wiersz czasu był zbyt krótki <br/> **7** — raportowanie jako nadużycia, spam lub wyłudzanie informacji <br/> **8** — inne |6|
Etap sprzedaży|Nie|Jest to pole wskazujące szczegółowy etap sprzedaży odwołania. Przeczytaj więcej na temat etapów sprzedaży [tutaj](https://aka.ms/salesStages)|40
Szacowana wartość transakcji|Tak|"Wartość transakcji na podstawie początkowych rozmów z klientem. Tę zmianę można zmienić, dopóki transakcja osiągnie jeden z Stanów końcowych| wygrane lub utracone ".|12563
Waluta|Tak|Waluta, w której wprowadzono wartość transakcji. Kody walut można znaleźć [tutaj](https://en.wikipedia.org/wiki/ISO_4217).|USD
Szacowana data zamknięcia|Tak|Szacowana data zamknięcia transakcji w oparciu o początkowe rozmowy z klientem w formacie MM/DD/RRRR. <br/> **Data powinna być w strefie czasowej UTC. Wszystkie daty wyświetlane w interfejsie użytkownika Centrum partnerskiego są oparte na zlokalizowanych strefach czasowych. W interfejsie użytkownika Centrum partnerskiego może istnieć +/-jeden dzień, Jeśli przeglądasz odwołanie, dla którego podałeś datę w strefie czasowej UTC.**|1/30/2020
IDENTYFIKATOR PROGRAMU CRM|Nie|Identyfikator tego konkretnego odwołania w systemie CRM, jeśli istnieje. To jest pole wprowadzania tekstu w postaci bezpłatnej.|34234324-sdfsdf-345345-SFD
Identyfikator kampanii marketingowej|Nie|To pole wskazuje kampanię marketingową, która spowodowała to konkretne odwołanie. Zwykle używane do obliczania zwrotu z inwestycji|BingSummer2020
Uwagi|Nie|Szczegółowe informacje wskazujące aktualizacje powiązane z odwołaniem|To jest przykładowa Uwaga
Pomoc firmy Microsoft jest wymagana?|Tak|Wskazuje to, czy chcesz, aby firma Microsoft mogła pomóc Ci w tworzeniu tego żądania współsprzedażowego|Tak
Którą konkretną pomoc firma Microsoft?|Zależy od|Jednym z sześciu różnych sposobów może Ci pomóc firma Microsoft. Ma to zastosowanie tylko w przypadku wybrania opcji nie dla pytania "pomoc Microsoft wymagana? " <br/> **Wprowadź liczbę na podstawie poniższych opcji** <br/><br/> **1**— propozycja wartości specyficznej dla obciążenia  <br/> **2**— architektura techniczna klienta  <br/> **3**— Weryfikacja koncepcji/demo  <br/> **4**— oferty i Licencjonowanie  <br/> **5**— powodzenie po sprzedaży klienta  <br/> **6**— ogólne lub inne|1|
Udostępnianie z zespołem ds. sprzedaży firmy Microsoft|Tak|Wskazuje to, czy chcesz udostępnić szczegóły dotyczące transakcji z zespołem sprzedaży firmy Microsoft, czy nie. Ma to zastosowanie tylko w przypadku wybrania opcji nie dla pytania "pomoc Microsoft wymagana? "|Tak
Uwagi do firmy Microsoft|Nie|Dowolnych uwag do firmy Microsoft, jeśli potrzebujesz pomocy od firmy Microsoft|Potrzebna pomoc dotycząca weryfikacji koncepcji dla klientów firmy Contoso
Wyrażanie zgody na udostępnianie klientowi/partnerowi|Tak|Wyraża zgodę na udostępnienie szczegółowych informacji kontaktowych klienta i pracowników firmy, którzy pracują nad pracą. **W przypadku wybrania tej kolumny nie można tworzyć ani aktualizować transakcji.** |Tak
Rozwiązanie 1|Tak|Identyfikator rozwiązania (wymagane), waluta (opcjonalnie), w którym została wprowadzona wartość transakcji. W [tym miejscu](https://en.wikipedia.org/wiki/ISO_4217)można znaleźć kody walutowe, cenę jednostki SKU (opcjonalnie) i ilość jednostki SKU (opcjonalnie).  |PERUWIAŃSKI-1234-PQRS, USD, 10, 100
Członek zespołu 1|Tak|Imię, nazwisko, numer telefonu komórkowego i identyfikator poczty e-mail odpowiedniego członka zespołu.| Robert, partner, 999999, Bob.partner@Contoso.com
