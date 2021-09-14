---
title: Zbiorcze eksportowanie i importowanie możliwości współpracy sprzedaży za pośrednictwem plików Excel/CSV w poleceniach
description: Dowiedz się, jak pobierać, tworzyć i aktualizować możliwości współpracy sprzedaży przy użyciu plików Excel (CSV) w Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 09/08/2021
ms.openlocfilehash: eb0f85eab9340d08a1f121c27f9a1956f5b71635
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246267"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Operacje zbiorcze dotyczące możliwości sprzedaży zbiorczej przy użyciu plików wartości rozdzielanych przecinkami (CSV)

**Odpowiednie role:** Administrator poleceń | Użytkownik poleceń

Operacje zbiorcze w Centrum partnerskim pomagają firmie eksportować i importować dane dotyczące szans wspólnej sprzedaży. Przejdź do strony **szans wspólnej sprzedaży**, aby znaleźć linki dotyczące **importu** i **eksportu** w prawym górnym rogu baneru tytułu strony. Z tej funkcji mogą korzystać użytkownicy z uprawnieniami **Administrator poleceń** i **Użytkownik poleceń**.

> [!IMPORTANT]
> Akcje tworzenia/aktualizacji wykonywane za pośrednictwem importu zbiorczego są nieodwracalne. Podczas modyfikowania lub tworzenia dużej liczby rekordów należy zachować ostrożność. Po utworzeniu transakcji można zmodyfikować tylko podzestaw pól. **Żadne akcje nie będą dozwolone, gdy dowolna transakcja osiągnie stan końcowy, taki jak odrzucona/wygasła/zawarta/utracona.**

## <a name="export-co-sell-opportunities"></a>Eksportowanie możliwości wspólnej sprzedaży

Poniżej opisano funkcje eksportowania:

- Klikając przycisk eksportu, można wyeksportować maksymalnie **5000** **rekordów.**
- Pobierane transakcje będą oparte na poziomach dostępu. Administratorzy poleceń i użytkownicy poleceń mogą uzyskać różne wyniki w zależności od ich zakresu i dołączania jako członkowie zespołu w transakcji. Dowiedz się więcej o [uprawnieniach poleceń](permissions-overview.md#manage-referrals).
- Funkcja eksportu uwzględnia bieżącą kartę na stronie możliwości sprzedaży i zastosowane filtry.
- Zostanie wygenerowany plik CSV ze wszystkimi danymi na podstawie zastosowanych filtrów.
- Pobieranie rekordów może potrwać do jednej minuty.
- Nie musisz czekać na ukończenie akcji pobierania. Nawet w przypadku przechodzenia do innych stron w Partner Center plik zostanie pobrany zaraz po zakończeniu działania funkcji eksportowania.
- Pobranego pliku można użyć ponownie w celu zmodyfikowania szczegółów transakcji i przekazania w celu zaktualizowania wszystkich rekordów.

## <a name="import-co-sell-opportunities"></a>Importowanie możliwości wspólnej sprzedaży

- Za pomocą funkcji importowania można utworzyć lub zaktualizować **maksymalnie 1000** rekordów.
- Szablon można skompilować od podstaw, pobierając go ze strony Importowanie w Partner Center.
- Możesz również użyć funkcji Eksportuj, aby pobrać istniejące rekordy i zaktualizować je.
- Jeśli plik zawiera więcej niż 1000 rekordów, nie można go przetworzyć.
- Po przetworzeniu pliku na ostatniej karcie pliku procesu zostanie wyświetlone podsumowanie z liczbą poleceń, które zostały utworzone, zaktualizowane i nie zostały przetworzone.
- Możesz pobrać szczegóły przetworzonych rekordów, naprawić wszelkie błędy i przekazać ten sam plik, aby utworzyć lub zaktualizować rekordy, które nie powiodły się w poprzednim uruchomieniu. **Usuń wszystkie rekordy pomyślne z pliku przed przekazaniem poprawionych rekordów, które nie powiodły się w poprzednim uruchomieniu.**
- Aby dodać więcej rozwiązań, dodaj dodatkowe kolumny obok rozwiązania 1 i użyj nazwy kolumny jako rozwiązania X, gdzie X reprezentuje liczbę rozwiązania w transakcji. Na przykład Rozwiązanie 2, Rozwiązanie 3.
- Do transakcji można dodać maksymalnie 50 rozwiązań.
- Aby dodać kolejnych członków zespołu, dodaj dodatkowe kolumny obok pola Członek zespołu 1 i użyj nazwy kolumny jako członka zespołu X, gdzie X reprezentuje liczbę członków zespołu w transakcji. Na przykład członek zespołu 2, członek zespołu 3.
- Do transakcji można dodać maksymalnie 50 członków zespołu.

> [!NOTE]
> Nie musisz czekać na ukończenie przetwarzania. Szczegóły ostatniego przetworzonego pliku będą dostępne do pobrania po zakończeniu przetwarzania. **Przekazanie plików ze 1000 rekordami może potrwać do 10 minut.**

> [!IMPORTANT]
> Przeczytaj dokładnie wszystkie instrukcje i sprawdź format każdej kolumny z poniższej tabeli przed utworzeniem lub zaktualizowaną transakcjami przy użyciu plików CSV w Partner Center.

|**Nazwa kolumny**|**Czy jest to obowiązkowe?**|**Opis**|**Przykładowe wartości**|
|-----|:-----|:---------|:---|
błędy|Nie|Błędy, jeśli jakiekolwiek związane z operacjami tworzenia/aktualizacji w.r.t do od skierowań zostaną uwzględnione w tej kolumnie. Jeśli istnieje wiele błędów, wszystkie z nich zostaną wyświetlone rozdzielone średnikami.|Brak obowiązkowego pola Rozwiązanie 1|
Identyfikator zaangażowania|Nie|Identyfikator zaangażowania jest generowany przez system poleceń Partner Center Microsoft. Nie jest wymagane do tworzenia nowych poleceń. Jeśli aktualizujesz rekord, możesz użyć istniejącego identyfikatora zaangażowania.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Identyfikator polecenia|Nie|Identyfikator polecenia jest generowany przez system poleceń Partner Center Microsoft. Nie jest wymagane do tworzenia nowych poleceń. Wypełnij go identyfikatorem odwołania, jeśli aktualizujesz istniejący rekord.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nazwa transakcji|Tak|Przyjazna nazwa transakcji dla Twojej odwołania.|Uk spring deal
Nazwa klienta|Tak|Nazwa firmy klienta. Użyj prawnej nazwy organizacji, aby szybko dopasować po stronie firmy Microsoft.|Contoso Corporation
Wiersz 1 adresu klienta|Tak|Wiersz 1 adresu firmy klienta. |One Contoso Way
Wiersz 2 adresu klienta|Nie|Adres 2 firmy klienta.|NE 148, ulica
Customer City|Tak|Miasto, w którym znajduje się organizacja klienta.|Redmond
Stan klienta|Nie|Stan, w którym znajduje się organizacja klienta.|Waszyngton
Kod pocztowy klienta|Nie|Kod pocztowy regionu, w którym znajduje się organizacja klienta.|98052
Kraj klienta|Tak|Kraj/region, w którym znajduje się organizacja klienta. Użyj dwulitowych kodów krajów, jak wspomniano [tutaj.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|USA
Identyfikator D-U-S klienta|Nie|Spróbuj pobrać identyfikator DUNS organizacji klienta. Pomoże to w szybszym dopasowaniu organizacji klienta po stronie firmy Microsoft, co ułatwia szybsze przypisywanie sprzedawców. Identyfikator DUNS ID możesz uzyskać bezpłatnie z tej witryny [internetowej.](https://www.dnb.com/duns-number/lookup.html)|81466849
Imię i nazwisko osoby kontaktowej klienta|Zależy|Imię jest obowiązkowe tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Imię głównej osoby kontaktowej z organizacji klienta, która pracuje nad tą ofertą.|Michał
Nazwisko osoby kontaktowej klienta|Zależy|Nazwisko jest obowiązkowe tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Nazwisko głównej osoby kontaktowej z organizacji klienta, która pracuje nad tą ofertą.|Customer
Numer Telefon klienta|Zależy|Telefon jest wymagany tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Telefon głównej osoby kontaktowej z organizacji klienta, która pracuje nad tą ofertą.|9999999999
Adres e-mail osoby kontaktowej klienta|Zależy|Adres e-mail jest wymagany tylko wtedy, gdy potrzebujesz pomocy firmy Microsoft. Adres e-mail głównej osoby kontaktowej z organizacji klienta, która pracuje nad tą ofertą.|john.customer@contoso.com
Stan polecenia partnera|Tak|Wskazuje stan transakcji z perspektywy firmy. Wymagane, jeśli próbujesz utworzyć lub zmodyfikować polecenie. Użyj **nowego,** jeśli próbujesz utworzyć nową ofertę. Akceptowane wartości są udokumentowane [tutaj.](/partner/develop/referral-resources#referralstatus)|Aktywna
Podstatus poleceń partnera|Tak|Wskazuje dokładny stan transakcji. Użyj **zaakceptowanych,** jeśli próbujesz utworzyć nową ofertę. Jest to również wymagane w przypadku modyfikowania istniejącego odwołania. Akceptowane wartości są udokumentowane [tutaj.](/partner/develop/referral-resources#referralsubstatus)|Zaakceptowano
Stan poleceń firmy Microsoft|Zależy|Wskazuje stan żądania współpracy sprzedaży wysłanego do firmy Microsoft poszukując pomocy. Jest to pole tylko do odczytu. Wszelkie zmiany wprowadzone w tym polu podczas importowania danych zostaną zignorowane.| Oczekiwanie
Odrzucona/utracona przyczyna|Zależy| Musisz podać te informacje tylko wtedy, gdy zmieniasz stan podrzędny pola na Odrzucone lub Utracone. W przeciwnym razie możesz zignorować tę kolumnę. <br/> **Wprowadź liczbę na podstawie poniższych opcji** <br/><br/> **1**— Project budżetu nie jest odpowiedni  <br/> **2**— Klient nie odpowiedział  <br/> **3**— Klient wybrał innego dostawcę  <br/> **4** — Wymagania klienta nie zostały spełnione  <br/> **5** — Nie jest klientem <br/> **6**— Proponowana linia czasowa była za krótka <br/> **7 —** Zgłaszanie jako nadużycie, spam lub wyłudzanie informacji <br/> **8** — Inne |6|
Etap sprzedaży|Nie|Jest to pole wskazujące szczegółowy etap sprzedaży polecenia. Dowiedz się więcej o etapach [sprzedaży tutaj](./manage-co-sell-opportunities.md)|40
Szacowana wartość transakcji|Tak|Wartość transakcji na podstawie początkowych konwersacji z klientem. Można ją zmienić, dopóki transakcja nie osiągnie jednego z stanów końcowych, które **zostały wygrane** lub **utracone.**|12563
Waluta|Tak|Waluta, w której wprowadzana jest wartość transakcji. Kody walut można znaleźć [tutaj.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Szacowana data zamknięcia|Tak|Szacowana data zamknięcia transakcji na podstawie początkowych konwersacji z klientem w formacie MM/DD/YYYY. <br/> **Data powinna być w strefie czasowej UTC. Wszystkie daty wyświetlane w interfejsie Partner Center są oparte na zlokalizowanych strefach czasowych. Jeśli patrzysz na polecenie, dla którego podano datę w strefie czasowej UTC, w interfejsie użytkownika może być Partner Center jeden dzień różnicy.**|1/30/2020
Identyfikator CRM|Nie|Identyfikator tego konkretnego odwołania w systemie CRM, jeśli takie są. Jest to pole wprowadzania tekstu w postaci bezpłatnej.|34234324-sdfsdf-345345-sfd
Identyfikator kampanii marketingowej|Nie|To pole wskazuje kampanię marketingową, co zaowocowała tym konkretnym poleceniem. Zwykle używany do obliczania zwrotu z inwestycji|BingSummer2020
Uwagi|Nie|Szczegółowe uwagi wskazujące aktualizacje związane z poleceniem|To jest przykładowa uwaga
Wymagana jest pomoc firmy Microsoft?|Tak|Ma to na celu wskazanie, czy chcesz, aby firma Microsoft pomogła Ci w zrzucie wniosku o współs sprzedaży|Tak
Jaka jest pomoc firmy Microsoft?|Zależy|Jeden z sześciu różnych sposobów, w jakie firma Microsoft może Ci pomóc. Ma to zastosowanie tylko w przypadku wybrania opcji Tak dla pytania "Wymagana pomoc firmy Microsoft? " <br/> **Wprowadź liczbę na podstawie poniższych opcji** <br/><br/> **1**— Obciążenie — konkcyjna wartość  <br/> **2 —** Architektura techniczna klienta  <br/> **3**— Proof of concept /Demo  <br/> **4 —** Oferty i licencjonowanie  <br/> **5**— Post — sukces klientów sprzedaży  <br/> **6**— Ogólne lub inne|1|
Udostępnianie zespołowi sprzedaży firmy Microsoft|Tak|Ma to na celu wskazanie, czy chcesz udostępnić szczegóły transakcji zespołowi sprzedaży firmy Microsoft, czy nie. Ma to zastosowanie tylko w przypadku wybrania opcji Nie dla pytania "Wymagana pomoc firmy Microsoft? "|Tak
Uwagi do firmy Microsoft|Nie|Wszelkie uwagi dotyczące firmy Microsoft, jeśli potrzebujesz pomocy od firmy Microsoft|Potrzebna pomoc z usługą POC dla klienta firmy Contoso
Zgoda na udostępnianie kontaktu klienta/partnera|Tak|Zgoda na udostępnianie danych kontaktowych klienta i danych kontaktowych pracowników firmy, którzy pracują nad ofertą. **Transakcje nie będą tworzone ani aktualizowane, jeśli dla tej kolumny wybierzesz pozycję Nie.** |Tak
Numer CLA|Zależy|Numer CLA nie jest wymagany podczas tworzenia lub aktualizowania transakcji IOT. Staje się to wymagane po przechodzeniu do etapu wygrania projektu.
Kategoria urządzenia|Nie|Lista wszystkich kategorii urządzeń IoT. Wybierz kategorię z poniższych opcji <br>Urządzenie do gier dla konsumentów <br> Bankomaty <br> Systemy transportowe & transportowych w przemyśle samochodowym <br> Azure Sphere tablicy<br> Azure Sphere, składnik <br> Azure Sphere Guardian<br> Azure Sphere modułu <br> Automatyzacja budowania<br> Casino Gaming Device <br> Urządzenia komunikacyjne<br> Consumer Internet Device <br> Consumer Wearable<br> Digital Picture Frame <br> Znak cyfrowy <br> Brama <br> HHT/Mobile<br> Industrial Automation Device<br> Tablet branżowy (bez pos) <br> Kiosk<br> Media Player<br> Urządzenie multimedialne <br> Mobilny pos <br> Urządzenie nawigacyjne<br> Projektor sieciowy<br> Inne<br> Inne urządzenie bankowe<br> Inne urządzenie elektroniczne konsumenta<br> Inne urządzenie<br> Inne Enterprise urządzenia<br>  Inny czujnik/węzeł <br> Urządzenie w punkcie sprzedaży<br> Urządzenie drukowania <br> Zabezpieczenia/nadzór <br>  Serwer<br> Set-Top Box<br> Smart TV <br> Urządzenie testowe i pomiarowe<br> Urządzenie klienckie zuzenkiem <br/>
Typ krzemu|Nie|Wprowadź informacje o modelu mikroukładu, wybierając opcję z poniższej listy <br> AMD –A10 <br> AMD – A4 <br> AMD – A6 <br> AMD – A8 <br> AMD – E2 <br> AMD — FX 7500 <br> AMD — FX 7600P <br> AMD — FX 9370 <br> AMD — FX 9590 <br> AMD — seria G <br> AMD — inne <br> AMD — seria R <br> AMD — pozostałe modele FX <br> Intel — Atom <br> Intel — Celeron — N1900 <br> Intel — Celeron — N2807 <br> Intel — Celeron — N2930 <br> Intel — Celeron — N3060 <br> Intel — Celeron — N3160 <br> Intel — Core i3 <br> Intel — Core i5 <br> Intel — Core i7 <br> Intel — Core M <br> Intel — inne <br> Intel — Pentium <br> Intel — reszta celeronu <br> Intel — XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Inne <br/>
Certyfikowane urządzenie platformy Azure|Nie|Ma to na celu wskazanie, czy certyfikat zgodności platformy Azure został osiągnięty dla urządzenia
Dołączanie usług|Nie|Ma to na celu wskazanie, czy usługi platformy Azure mają być powiązane z rozwiązaniem IoT podczas wdrażania
Microsoft MSX ID|Nie|Identyfikator transakcji w systemie Microsoft MSX, dostępny tylko w przypadku możliwości współpracy sprzedaży
Migrowany identyfikator transakcji PSC|Nie|Identyfikator transakcji PSC, dostępny tylko dla transakcji migrowanych z psc na komputer
Identyfikator MPN|Nie|Identyfikator MPN organizacji, dla której są tworzone możliwości sprzedaży
Rozwiązanie 1|Tak|Identyfikator rozwiązania (wymagane), waluta (opcjonalnie), w której wprowadzono wartość transakcji. Możesz znaleźć kody [walut,](https://en.wikipedia.org/wiki/ISO_4217)cenę sku (opcjonalnie) i ilość (opcjonalnie)  |SOL-1234-PQRS, USD, 10, 100
Członek zespołu 1|Tak|Imię, nazwisko, numer telefonu komórkowego i identyfikator e-mail odpowiedniego członka zespołu.| Bob, Partner, 999999, Bob.partner@Contoso.com
Członek zespołu firmy Microsoft 1|Nie|Imię, nazwisko, numer telefonu komórkowego i identyfikator e-mail odpowiedniego członka zespołu firmy Microsoft, który pracuje nad szansą sprzedaży.| Sam, Seller, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Następne kroki

Tych łączników można Partner Center do współs sprzedaży z firmą Microsoft z poziomu systemów CRM.

- [Łącznik do współpracy sprzedaży dla usługi Dynamics 365 CRM — omówienie](connector-dynamics.md)
- [Łącznik do współsprzedaży dla rozwiązania Salesforce CRM — omówienie](connector-salesforce.md)
