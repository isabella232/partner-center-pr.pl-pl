---
title: Zestawienia wypłat
description: Dowiedz się więcej o zestawieniach i podsumowaniach wypłat oraz o tym, jak wyświetlać i eksportować dane dotyczące płatności z usługi Microsoft Partner Center
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: b905d422b10e0b82225966fa5379283ea0b83a69
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958581"
---
# <a name="payout-statements"></a>Zestawienia wypłat

**Odpowiednie role:** Administrator konta | Administrator globalny

Zestawienie **wypłat zawiera** omówienie wypłat z ofert sprzedawanych za pośrednictwem platformy handlowej. Pokazuje historię transakcyjną zarobków, szacuje następną płatność i pokazuje trendy płatności. Możesz również pobrać historię transakcji i zestawienia płatności. W tym artykule wyjaśniono, jak uzyskać dostęp do zestawienia wypłat oraz różnych stron wypłat i plików do pobrania dostępnych w Partner Center.

>[!NOTE]
>Zobaczysz tylko dane dotyczące identyfikatorów MPN i programów, z które są skojarzone. Jeśli chcesz wyświetlić dodatkowe dane, we współpracy z administratorem konta w celu zachowania uprawnień. 

## <a name="roles-and-permissions"></a>Role i uprawnienia

Aby uzyskać dostęp do zestawienia wypłat, musisz mieć przypisaną rolę Właściciel **konta** lub **Współautor finansowy.**

| Raporty/strony | Właściciel konta | Menedżer | Deweloper | Współautor biznesowy | Współautor finansowy | Marketer |
| --- | --- | --- | --- | --- | --- | --- |
| Raport pozyskiwania (w tym dane niemal w czasie rzeczywistym) | Można wyświetlać | Można wyświetlać | Brak dostępu | Brak dostępu | Można wyświetlać | Brak dostępu |
| Raport/odpowiedzi dotyczące opinii | Może wyświetlać i wysyłać opinie | Może wyświetlać i wysyłać opinie | Może wyświetlać i wysyłać opinie | Brak dostępu | Brak dostępu | Może wyświetlać i wysyłać opinie |
| Raport kondycji (w tym dane niemal w czasie rzeczywistym) | Można wyświetlać | Można wyświetlać | Można wyświetlać | Można wyświetlać | Brak dostępu | Brak dostępu |
| Raport użycia | Można wyświetlać | Można wyświetlać | Można wyświetlać | Można wyświetlać | Brak dostępu | Brak dostępu |
| Konto wypłaty | Można aktualizować | Brak dostępu | Brak dostępu | Brak dostępu | Można aktualizować | Brak dostępu |
| Profil podatkowy | Można aktualizować | Brak dostępu | Brak dostępu | Brak dostępu | Można aktualizować | Brak dostępu |
| Podsumowanie wypłaty | Można wyświetlać | Brak dostępu | Brak dostępu | Brak dostępu | Można wyświetlać | Brak dostępu |
|

## <a name="access-your-payout-statement"></a>Uzyskiwanie dostępu do zestawienia wypłat

Zaloguj się do [Partner Center](https://partner.microsoft.com/dashboard/home) i wybierz ikonę wypłaty w prawym górnym rogu ekranu, aby uzyskać dostęp do tych różnych podsumowań:

- Historia transakcji
- Płatności
- Eksportowanie danych

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ilustruje ikonę Wypłaty w prawym górnym rogu Partner Center Portal.":::

Możesz również użyć interfejsu API wypłat [partnera,](/rest/api/partner-center/partner-payouts) aby nawiązać połączenie i uzyskać dane dotyczące transakcji wypłat i płatności bezpośrednio. Aby dowiedzieć się [więcej, zobacz Manage payouts using the Payout Service API (Zarządzanie wypłatami przy użyciu interfejsu API usługi wypłat).](/partner-center/develop/manage-payouts)


## <a name="transaction-history"></a>Historia transakcji

Strona **Historia transakcji** zawiera podsumowanie zarobków, szacowaną następną płatność oraz trend zarobków i płatności w ciągu ostatnich 36 miesięcy. Szczegóły transakcji można również pobrać z tej sekcji.<br><br>Ten raport przedstawia wszystkie zarobki kwalifikujące się do wypłaty, w tym płatności, które nie zostały jeszcze wysłane. Zarobki kwalifikują się do wypłaty, gdy isv has completed all bank and tax information in Partner Center, has earned >$50, the ISV account is active, and the customer has been billed (for EA transactions) or the payment has been received (for non-EA transactions).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Przegląd transakcji.":::

- **Zarobki wysłane w tym roku** — łączne zarobki i podział zarobków, które zostały zapłacone i zostaną opłacone w nadchodzącym miesiącu.
- **Szacowany miesiąc płatności —** łączne zarobki oczekiwane w nadchodzących miesiącach.
- **Trend zarobków i płatności** — miesięczne zarobki i kwoty płatności z ostatnich 36 miesięcy.
- **Pobierz** — pobierz szczegóły transakcji w .csv lub tsv.

Użyj opcji wyboru zakresu dat w prawym górnym rogu strony, aby odfiltrować dane wyjściowe strony w celu pokazania ostatnich 3, 6, 12 lub 36 miesięcy. Możesz też wybrać niestandardowy zakres dat do 36 miesięcy. Domyślny zakres dat to 12 miesięcy. Możesz również filtrować według identyfikatora rejestracji, programu, identyfikatora płatności, typu zarobków, lever i stanu. Dane są dostępne dla bieżącego roku obrachunkowego (1 lipca — 30 czerwca) i poprzednich dwóch lat obrachunkowych.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Filtr wyszukiwania w prawym górnym rogu strony.":::

Aby wyświetlić więcej szczegółów dotyczących zarobków, wybierz strzałkę w dół w prawej części strony. Spowoduje to wyświetlenie uchwytu, kwoty przychodu, produktu i klienta. Jeśli z jakiegoś powodu jakiekolwiek z tych danych są niedostępne, ale potrzebujesz do nich dostępu, skontaktuj się z pomocą techniczną. Jeśli zarobki są wynikiem korekty, a nie transakcji, pola Produkt i Klient nie będą wyświetlane.

### <a name="transaction-history-summary"></a>Podsumowanie historii transakcji

Ten widok przedstawia szczegóły zarobków, w tym pochodzenie zarobków z daty zarobków sprzedanych produktów, stan i szacowany miesiąc płatności.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historia transakcji.":::

- **Data osiągnięcia** — data zakupu.
- **Typ zarobków** — typ zarobków, na przykład Sprzedaż, Przyniesienie lub Współpraca.
- **Łączna** kwota — kwota zarobków netto. Na platformie handlowej oznacza to po odjęeniu standardowej opłaty za platformę handlową.
- **Stan** — ma trzy opcje:
    - **Nadchodzące** — zarobki są w okresie oczekiwania na chłodzenie.
    - **Przetworzone** — zarobki są przygotowane do następnej płatności.
    - **Wysłane** — zarobki zostały zapłacone.
- **Szacowany miesiąc** płatności — miesiąc, w ciągu których zarobki powinny zostać zapłacone. Aby uzyskać [więcej informacji, zobacz](#estimated-payment-month) następną sekcję.

Transakcje zarobków są wyświetlane, gdy transakcja spełnia uprawnienia do wypłaty. Aby zrozumieć, dlaczego brakuje Ci lub niespodziewane zarobki, zobacz Typowe pytania [dotyczące wypłat na platformie handlowej.](payout-faq.yml#why-are-my-earnings-missing-)

#### <a name="estimated-payment-month"></a>Szacowany miesiąc płatności

Na stronie Historia transakcji znajduje się teraz tabela przedstawiająca szacowane kwoty płatności w ciągu następnych kilku miesięcy. Te informacje można również wyświetlać i pobierać w eksportach Historia transakcji i Raport podsumowania. Te informacje ułatwiają uzgadnianie i projekcje płatności.

Szacowany miesiąc płatności jest obliczany na podstawie reguł i osi czasu konfiguracji programu i jest przetwarzany w następnym/nadchodzącym cyklu płatności.

Szacowany miesiąc płatności jest obecnie dostępny dla wszystkich typów zarobków z wyjątkiem współpracy, która będzie wyświetlana jako **Nie dotyczy.** W przypadku zarobków przed 1 lipca 2020 r. szacowany miesiąc płatności będzie wyświetlany jako **Niedostępny.**

W poniższej tabeli przedstawiono przykład szacowanego miesiąca płatności.

| Month (Miesiąc) | Kwota |
| ------ | :-----------: |
|  Wrzesień 2020 r. |  7273,99 USD   |
|  Październik 2020 r. | 8692,30 USD  |
|  Listopad 2020 r. | 107,89 USD  |

Szacowana kwota może się różnić od rzeczywistej z różnych powodów:

- Ponowne obliczanie zarobków: jeśli zarobki zostaną ponownie wyliczone, rzeczywista kwota będzie inna
- Korekty: Rzeczywista kwota różni się w zależności od korekt, które wystąpiły lub zostały przesłane.
- Zmiana reguł: Zmiana reguł może odzwierciedlać ponowne obliczanie rzeczywistej kwoty zapłaconej
- Zobowiązania: W przypadku niepowodzenia płatności rzeczywista kwota może się różnić

Pamiętaj, że płatność jest zwalniana w prognozowanych miesiącach tylko wtedy, gdy są spełnione zasady dotyczące progu programu i uprawnień do płatności. Reguły te obejmują, ale nie są ograniczone do poniższej listy:

- Twój profil podatkowy musi być aktualny
- Zarobki muszą spełniać lub przekraczać minimalny próg zarobków zdefiniowany w przewodniku po programie.
- Wstrzymana wypłata: jeśli wybierzesz opcję "Hold my Payment" (Przytrzymaj moją płatność) na stronie przypisywania profilów.
- Instrument wypłaty jest niedostępny: Profil płatności lub/i profil podatkowy nie został ukończony.

### <a name="transaction-history-download"></a>Pobieranie historii transakcji

Aby wyświetlić więcej szczegółów dotyczących zarobków, wybierz **pozycję Pobierz** w górnej części strony. W poniższej tabeli wyjaśniono każdą kolumnę w raporcie.

>[!NOTE]
>Eksport pobierania historii transakcji ma dwa nowe pola od sierpnia 2020 r.:
>
>- **lastPaymentCurrency**  Waluta, w której otrzymano najnowszą płatność, we wszystkich sieciach MPN, do których ma dostęp partner, który jest aktualnie zalogowany. Jeśli żadna płatność nie zostanie odebrana, ostatnia waluta płatności będzie w dolarach amerykańskich.
>- **earningAmountInLastPaymentCurrency**  Kwota zarobków w ostatniej walucie płatności.

| Nazwa kolumny | Opis | Zastosowanie programów zachęt/platform handlowych |
| --- | --- | --- |
| agreementEndDate | Data zakończenia umowy | Zachęty — tylko niektóre programy |
| agreementNumber | Numer umowy | Zachęty — tylko niektóre programy |
| agreementStartDate | Data rozpoczęcia umowy | Zachęty — tylko niektóre programy |
| calculationDate | Data obliczenia zarobków w systemie | Wszystko |
| claimId | Unikatowy identyfikator oświadczenia | Zachęty — tylko niektóre programy |
| customerCountry | Kraj/region klienta | Rynkach |
| customerEmail |  |  |
| Customername | Może być pusta | Tylko programy zachęt (wyjątek: OEM) i platformy handlowe. W przypadku transakcji CSP na platformach handlowych będzie pokazywana nazwa programu CSP |
| customerTenantId |  |  |
| distributorId | Identyfikator dystrybutora | Zachęty — tylko niektóre programy |
| distributorName | Nazwa dystrybutora | Zachęty — tylko niektóre programy |
| earningAmount | Kwota zarobków w oryginalnej walucie transakcji | Wszystko |
| earningAmountInLastPaymentCurrency | Kwota zarobków w ostatniej walucie płatności (pole będzie puste, jeśli żadne wcześniejsze płatności nie zostały opłacone) |  |
| earningAmountUSD | Zarobki w USD | Wszystko |
| earningDate | Data zarobku | Wszystko |
| earningExchangeRate | Exchange używana do pokazania odpowiedniej kwoty w USD | Wszystko |
| earningId | Unikatowy identyfikator dla każdego zarobku | Wszystko |
| earningRate | Stawka zachęt zastosowana do kwoty transakcji w celu wygenerowania zarobków | Wszystko |
| earningType | Wskazuje, czy jest to opłata, pomówienie, współpraca, sprzedaż i tak dalej | Wszystko |
| exchangeRateDate | Exchange stawki używanej do obliczania wartości EarningAmount USD | Wszystko |
| externalReferenceId | Unikatowy identyfikator programu | Programy z płatnością bezpośrednią (zachęty i platformy handlowe) |
| externalReferenceIdLabel | Unikatowa etykieta identyfikatora | Programy z płatnością bezpośrednią (zachęty i platformy handlowe) |
| instantNegoateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Numer faktury (dotyczy tylko przedsiębiorstwa) | Zachęty i platformy handlowe — tylko niektóre programy |
| lastPaymentCurrency | Ostatnia waluta płatności (pole będzie puste, jeśli nie została opłacona żadna wcześniejsza płatność) |  |
| Dźwignia | Wskazuje regułę biznesową dla zarobków | Wszystko |
| LicensingProgramName | Nazwa programu licencjonowania |  |
| LineItemId | Pojedynczy wiersz na fakturze klienta |  |
| localProviderSeller | Lokalny dostawca/sprzedawca rekordu |  |
| Miesiąc dojrzałości | Szacowany miesiąc płatności | Wszystko |
| OrderId (Identyfikator zamówienia) | Odnosi się do faktury klienta  | Rynkach |
| parentProductId | Unikatowy nadrzędny identyfikator produktu. Jeśli dla transakcji nie ma produktu nadrzędnego, oznacza to, że nadrzędny identyfikator produktu = identyfikator produktu. | Rynkach |
| parentProductName (nazwa_elementu_nadrzędnego) | Nazwa produktu nadrzędnego. Jeśli dla transakcji nie ma produktu nadrzędnego, nazwa produktu nadrzędnego = nazwa produktu. | Rynkach |
| participantId | Podstawowa tożsamość partnera zarobków w ramach programu | Wszystko |
| typ-uczestnika | Głównie identyfikator programu dla programów zachęt i sprzedawców IF dla platform handlowych | Wszystko |
| nazwa uczestnika | Nazwa partnera zarobków | Wszystko |
| partnerCountryCode | Lokalizacja/kraj/region partnera zarobków | Wszystko |
| partNumber | Zawsze będzie pusta | Niektóre programy zachęt i platformy handlowe |
| paymentId | Unikatowy identyfikator korelowania wszystkich transakcji w raporcie transakcji z określoną płatnością w raporcie płatności | Wszystko |
| paymentStatus | Stan płatności | Wszystko |
| paymentStatusDescription | Przyjazny opis stanu płatności | Wszystko |
| productId | Unikatowy identyfikator produktu | Rynkach |
| Productname | Nazwa produktu połączona z transakcją | Wszystko |
| productType | Typ produktu, na przykład Aplikacja, Dodatek lub Gra | Rynkach |
| Kod programu | Ciąg do mapowania na nazwę programu |  |
| nazwa_programu | Nazwa programu zachęty/sklepu | Wszystko |
| purchaseOrderCoverageEndDate | Zawsze będzie pusta | Program zachęt — CRI |
| purchaseOrderCoverageStartDate | Zawsze będzie pusta | Program zachęt — CRI |
| purchaseOrderType | Zawsze będzie pusta | Program zachęt — CRI |
| purchaseTypeCode | Zawsze będzie pusta | Program zachęt — CRI |
| quantity | Różni się w zależności od programu. Wskazuje rozliczaną ilość dla programów transakcyjnych | Wszystko |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identyfikator odsprzedawcy | Zachęty — tylko niektóre programy |
| resellerName (nazwa odsprzedawcy) | Nazwa odsprzedawcy |  |
| SkuId | Identyfikator SKU zdefiniowany podczas publikowania. Oferta może mieć wiele jednostki SKU, ale jednostkę SKU można skojarzyć tylko z jedną ofertą. Zachęty — tylko niektóre programy |  |
| storeFee | Kwota zachowywana przez firmę Microsoft jako opłata za korzystanie z aplikacji lub dodatku w Sklepie | Rynkach |
| subscriptionEndDate | Data zakończenia subskrypcji | Zachęty — tylko niektóre programy |
| subscriptionId | Identyfikator subskrypcji skojarzony z klientem | Zachęty — tylko niektóre programy |
| subscriptionStartDate | Data rozpoczęcia subskrypcji | Zachęty — tylko niektóre programy |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Strona odpowiedzialna za remitowanie podatków (sprzedaż, użycie lub podatki VAT/GST) | Rynkach |
| taxRemitted | Kwota uchwalonego podatku (sprzedaż, użycie lub podatki VAT/GST) | Rynkach |
| taxState | Stan klienta |  |
| taxZipCode | Kod pocztowy klienta |  |
| tpan | Wskazuje sieć ad innej firmy | Marketplaces Tylko reklamy |
| transactionAmount | Kwota transakcji w oryginalnej walucie transakcji w oparciu o wygenerowanie zarobków | Wszystko |
| transactionAmountUSD | Kwota transakcji w USD | Wszystko |
| transactionCountryCode | Kod kraju/regionu, w którym miała miejsce transakcja |  |
| transactionCurrency | Waluta, w której miała miejsce pierwotna transakcja klienta (nie jest to waluta lokalizacji partnera) | Wszystko |
| Transactiondate | Data transakcji. Przydatne w przypadku programów, w których wiele transakcji przyczynia się do jednego zarobku | Wszystko |
| transactionExchangeRate | Exchange stawka używana do pokazania odpowiedniej kwoty transakcji w USD | Wszystko |
| transactionId | Unikatowy identyfikator transakcji | Wszystko |
| transactionPaymentMethod | Instrument płatniczy klienta używany do transakcji, taki jak karta, rozliczenia operatora sieci komórkowej lub PayPal | Rynkach |
| Transactiontype | Typ transakcji, taki jak zakup, zwrot, zwrot lub obciążenie zwrotne | Rynkach |
| workload | Obciążenie | Zachęty — tylko niektóre programy |
|

### <a name="transaction-adjustment-codes"></a>Kody korekt transakcji

W poniższej tabeli wymieniono kody przyczyn korekt i ich opisy.

|**Kod przyczyny**   |**Opis**   |
|------------------|:-------------------------------------|
| Zgodność ar | Korekta, która zmniejsza zarobki, gdy faktury firmy Microsoft nie są opłacane na czas przez partnera. |
| Przewłaszczane współoperacyjne | Korekta, która przenosi zarobki w związku z współpraca na inny okres lub konwertuje zarobki w kooperacji na chętnych. |
| Korekta operacyjna | Korekta, która poprawia błędy obliczeń systemu firmy Microsoft. |
| Niepoprawne oblicze korekty operacyjności firmy Microsoft | Korekta, która poprawia błędy obliczania. |
| Korekty korekty operacyjna nieprawidłowa rejestracja firmy Microsoft | Korekta błędnych obliczeń związanych z rejestracją. |
| Mapowanie partnerów (subskrypcja) MCI/CSP | Korekta, która koryguje niedorównanie subskrypcji. |
| Wyjątek zasad | Korekta zastępująca regułę programu.  |
| Zarobki w poprzednim okresie | Korekta zarobków poza bieżącym okresem zarobków. |

## <a name="payments"></a>Płatności

Strona **Płatności** zawiera szczegółowe informacje o pieniędzy, które zostały uzyskane przez firmę Microsoft. Pokazuje również, kiedy i ile będziesz zapłacił.

>[!Note]
> Aby kwalifikować się do wypłaty, twoje wpływy muszą osiągnąć [próg](payment-thresholds-methods-timeframes.md) płatności 50 USD. Aby uzyskać więcej informacji, zobacz [umowę Microsoft Publisher agreement.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Ekran przeglądu płatności.":::

- **Łączna kwota zapłacona** w tym roku — łączna łączna kwota zapłacona w tym roku w dolarach amerykańskich dla wszystkich programów.
- **Następna szacowana płatność** — pojedyncza następna płatność do Ciebie (nawet jeśli wkrótce będą dostępne inne) w dolarach amerykańskich.
- **Ostatnia płatność** — kwota (w dolarach amerykańskich), nazwa programu i program ostatniej płatności.
- **Płatność według źródła** — kwota płatności (w dolarach amerykańskich), na program, w ciągu ostatnich 12 miesięcy.

### <a name="payments-list"></a>Lista płatności

Tabela **Lista płatności zawiera płatności** płatne i oczekujące. Możesz pobrać informacje podatkowe dotyczące opłaty za usługę w formacie PDF i wyświetlić szczegóły zarobków dla danej płatności.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Eksportowanie historii transakcji.":::

- **Płatne** — wszystkie płatności wysłane pomyślnie. Wybierz rok z menu rozwijanego, aby odfiltrować płatności wydane w tym roku.
- **Oczekujące** — nadchodzące płatności.
- **Podatek od opłaty za usługę (formularz PDF)** — dostępny dla płatności podlegających opodatkowaniu opłaty za usługę. Podatki z tytułu opłaty za usługę są pokazane w **tece Inne podatki.**
- **Widok** — przekierowuje do historii transakcji z listą zarobków uwzględnionych w płatności.

Aby zrozumieć, dlaczego brakuje Ci lub nieoczekiwane zarobki, zobacz Typowe pytania [dotyczące wypłat na platformie handlowej.](payout-faq.yml#why-are-my-earnings-missing-)

### <a name="payment-status"></a>Stan płatności

W poniższej tabeli wyjaśniono różne stany zarobków.

| Stan zarobków | Przyczyna | Wymagana jest akcja partnera? |
| --- | --- | --- |
| Nieprzetworzonych | Zarobki kwalifikują się do płatności. Pozostaje w tym stanie przez okres chłodzenia zgodnie z definicją w przewodniku programu dla Program zachęt. | Nie |
| Nadchodzących | Wygenerowane zamówienie płatności oczekujące na przeglądy wewnętrzne przed przetworzeniem płatności. | Nie |
| Oczekująca faktura podatkowe | Faktura podatkowe jest niekompletna lub nieprawidłowa. | Aby można było zapłacić fakturę podatkowej, musisz ją zaktualizować |
| Odrzucone podczas przeglądu | Płatność została odrzucona podczas przeglądu. | Aby uzyskać szczegółowe informacje, skontaktuj się z pomocą techniczną firmy Microsoft |
| Niepowodzenie | Płatność nie powiodła się z powodu błędu systemu firmy Microsoft. | Aby uzyskać szczegółowe informacje, skontaktuj się z pomocą techniczną firmy Microsoft |
| W toku | Trwa płatność. | Nie |
| Nieprawidłowa płatność | Trwa cofanie płatności. | Nie |
| Wysłane | Płatność została wysłana do Twojego banku. | Nie |
| Ponownego przetwarzania | Płatność napotkała błąd systemu firmy Microsoft i jest przetwarzana ponownie. | Nie |
| Reversed | Płatność została wycofana przez bank i zostanie wysłana ponownie w następnym cyklu płatności. | Nie |
| Faktura podatku została odrzucona | Faktura podatkowe została odrzucona podczas przeglądu. Wszystkie oczekujące płatności będą wstrzymane do czasu ukończenia przeglądu faktury podatkowej. | Aby uzyskać szczegółowe informacje, skontaktuj się z pomocą techniczną firmy Microsoft |
| Faktura podatkowe w trakcie przeglądu | Faktura podatkowe jest przeglądana. Płatność zostanie zwolniona po zatwierdzeniu faktury podatkowej. | Nie |
| Odrzucone | Płatność została odrzucona przez bank. | Aby uzyskać szczegółowe informacje, skontaktuj się z bankiem. |
|

### <a name="payments-download"></a>Pobieranie płatności

 W poniższej tabeli wyjaśniono każdą kolumnę w raporcie. Aby wyświetlić więcej szczegółów dotyczących płatności, wybierz **pozycję Pobierz** w górnej części strony Płatności.

| Nazwa kolumny | Opis |
| --- | --- |
| participantID | Podstawowa tożsamość partnera zarobków w ramach programu |
| participantIDType | Zazwyczaj identyfikator programu dla programów zachęt i identyfikator sprzedawcy dla programów ze Sklepu |
| nazwa uczestnika | Nazwa partnera zarobków |
| nazwa_programu | Zachęty/nazwa programu sklepu |
| Zdobył | Kwota uzyskane w walucie Płatności na dla tego programu/uczestnikaID |
| earnedUSD | Kwota uzyskanej za identyfikator programu/uczestnika w USD |
| withheldTax | Kwota podatku nieutrzymana w walucie płatności zgodnie z programem/wartością uczestnika |
| salesTax | Łączna kwota podatku od sprzedaży w walucie Płatność zgodnie z programem/wartością uczestnika (dotyczy tylko programów zachęt) |
| serviceFeeTax | Łączna kwota usługiFeeTax w walucie płatności zgodnie z programem/wartością uczestnika (dotyczy tylko programów Azure Marketplace sklepów) |
| totalPayment | Łączna płatność w walucie lokalnej z wyłączeniem podatku potrącanego i z uwzględnieniem podatku od sprzedaży (jeśli ma zastosowanie) dla programu/uczestnikaID |
| currencyCode | Kod waluty płatności |
| paymentMethod (metoda płatności) | Metoda używana do płacenia partnerowi, na przykład elektroniczne przelewy bankowe, nota kredytowa |
| paymentID | Unikatowy identyfikator płatności. Ta liczba jest zwykle widoczna w wyciągu z banku (dotyczy tylko płatności SAP). |
| paymentStatus | Stan płatności |
| paymentStatusDescription | Przyjazny opis stanu płatności |
| paymentDate | Data wysłania płatności od firmy Microsoft |
|

## <a name="export-data"></a>Eksportowanie danych

Strona **Eksportowanie** danych nie jest odświeżana samodzielnie. W celu zobaczenia najnowszych danych może być konieczne ręczne odświeżenie strony. Wybierz jedną z trzech kart, aby wyeksportować historię **transakcji,** **płatności,** **podsumowanie transakcji** lub **zestawienie historyczne.**

Filtr może spowodować błąd **Brak dostępnych** danych. Może się to zdarzyć, jeśli pozostawisz domyślny okres wybrany na trzy miesiące, a następnie wybierzesz identyfikator płatności z zarobków spoza tego okresu. W takim przypadku rozwiń swój okres i spróbuj ponownie.

Oto przykładowy eksport płatności:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Eksportowanie raportu płatności.":::

### <a name="historical-statements"></a>Instrukcje historyczne

Podsumowanie **Eksportowanie** danych zapewnia również dostęp do instrukcji historycznych.

> [!NOTE]
> Instrukcja historyczna jest migawką i nie jest odświeżana. Skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/support/v2/?stage=1) i w razie potrzeby zażądaj najnowszych danych.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Eksportowanie instrukcji historycznych.":::

- Historia transakcji przed 1 lipca 2019 r. jest obsługiwany oddzielnie i używa różnych pól z nowszych raportów historii.
- Starsza historia transakcji zawiera kolumnę o nazwie "Reserved", która odpowiada kolumnie "Zarobki" w nowoczesnej historii, z tą różnicą, że wyklucza wszystkie zarobki ze stanem "Wysłane płatności".
- Filtry, takie jak 3M, 6M lub 12M, nie będą stosowane do sekcji Instrukcje historyczne.

### <a name="historical-statement-downloads"></a>Pobieranie instrukcji historycznych

W poniższej tabeli wyjaśniono każdą kolumnę w instrukcji historycznej.

| Nazwa pola | Opis |
| --- | --- |
| Źródło przychodu | Źródło przychodu na podstawie miejsca, w którym wystąpiła transakcja, na przykład Microsoft Store, Windows Phone Store, Windows Store 8 lub reklam |
| Identyfikator zamówienia | Unikatowy identyfikator zamówienia. Ten identyfikator umożliwia identyfikowanie transakcji zakupu z odpowiednimi transakcjami niekupu, takimi jak zwroty lub obciążenia zwrotne. Oba będą mieć ten sam identyfikator zamówienia. Ponadto jeśli istnieje opłata podzielona, w przypadku której wiele metod płatności zostało użytych w ramach pojedynczego zakupu, można połączyć transakcje zakupu. |
| Transaction ID (Identyfikator transakcji) | Unikatowy identyfikator transakcji. |
| Data i godzina transakcji | Data i godzina transakcji (UTC). |
| Nadrzędny identyfikator produktu | Unikatowy nadrzędny identyfikator produktu. Jeśli dla transakcji nie ma produktu nadrzędnego, oznacza to, że nadrzędny identyfikator produktu = identyfikator produktu. |
| Identyfikator produktu | Unikatowy identyfikator produktu. |
| Nazwa produktu nadrzędnego | Nazwa produktu nadrzędnego. Jeśli dla transakcji nie ma produktu nadrzędnego, nazwa produktu nadrzędnego = nazwa produktu. |
| Nazwa produktu | Nazwa produktu |
| Typ produktu | Typ produktu, na przykład Aplikacja, Dodatek lub Gra |
| Liczba | Gdy źródło przychodu jest Microsoft Store dla Firm, wartość Quantity reprezentuje liczbę zakupionych licencji. W przypadku wszystkich innych źródeł przychodów ilość będzie zawsze wynosić 1. Nawet jeśli pojedyncza transakcja zostanie podzielona na dwa pozycje, ponieważ zostały użyte dwie różne formy płatności, każdy element wiersza będzie pokazywać wartość Quantity (Ilość) 1. |
| Typ transakcji | Typ transakcji, na przykład zakup, zwrot, zwrot lub obciążenie zwrotne |
| Formy płatności | Instrument płatniczy klienta używany do transakcji, taki jak karta, rozliczenia operatora sieci komórkowej lub PayPal |
| Kraj/region | Kraj/region, w którym wystąpiła transakcja |
| Dostawca lokalny/sprzedawca | Lokalny dostawca/sprzedawca rekordu |
| Waluta transakcji | Waluta transakcji |
| Kwota transakcji | Kwota transakcji |
| Tax Remitted | Kwota emitowanych podatków (sprzedaż, użycie lub podatki VAT/GST) |
| Net Receipts | Kwota transakcji mniejsza niż liczba emitowanych podatków |
| Opłata za sklep | Wartość procentowa wpływów netto zachowywanych przez firmę Microsoft jako opłata za korzystanie z aplikacji lub dodatku w Sklepie |
| Kontynuuje działania aplikacji | Wpływy netto pomniejszone o opłatę za sklep |
| Podatki nieudyskcjone | Kwota potrącanego podatku dochodowego (uwzględniona w **zastrzeżonym pliku** CSV) |
| Płatność | Przychód w aplikacji jest mniejszy niż ewentualne potrącenie podatku dochodowego (kwota wyświetlana w walucie transakcji). Nie uwzględniono w **zarezerwowanym** pliku CSV. |
| Stawka FX | Kurs wymiany obcej używany do konwersji waluty transakcji na walutę płatności |
| Waluta płatności | Waluta, w której dokonano płatności |
| Przekonwertowana płatność | Kwota płatności przekonwertowana na walutę płatności przy użyciu stawki FX |
| Model zwolnienia z podatku | Strona odpowiedzialna za remitowanie podatków (sprzedaż, użycie lub podatki VAT/GST) |
| Data i godzina uprawnień | Data i godzina kontynuowania transakcji kwalifikują się do wypłaty (UTC). Po utworzeniu wypłaty obejmuje ona transakcję z datą uprawnień (o godzinie) przed datą utworzenia wypłaty (uwzględnioną tylko w **zastrzeżonym** pliku CSV). |
| Opłaty | Przedstawia podział wszystkich szczegółów opłat zagregowanych w kolumnie Kwota transakcji (uwzględnionych tylko dla Azure Marketplace; nieujętego w pliku **CSV** zarezerwowanym). |
|||

## <a name="next-steps"></a>Następne kroki

- [Interfejs Partner Payout API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Szczegóły zasad wypłat](payout-policy-details.md)
- Aby uzyskać pomoc techniczną w związku z rozliczeniami, skontaktuj się z pomocą techniczną [wydawcy komercyjnej platformy handlowej.](https://partner.microsoft.com/support/v2/?stage=1)
