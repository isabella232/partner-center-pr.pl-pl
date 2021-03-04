---
title: Zestawienia wypłat
description: Dowiedz się więcej na temat zestawień i podsumowań wypłaty oraz jak wyświetlać i eksportować dane dotyczące płatności z Centrum partnerskiego firmy Microsoft
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 10/29/2020
ms.openlocfilehash: 4a511dc026e3c71f05c5b18ca6d8915bd2654826
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756171"
---
# <a name="payout-statements"></a>Zestawienia wypłat

**Odpowiednie role:**

- Administrator konta
- Administrator globalny

**Instrukcja wypłaty** zawiera przegląd wypłat z ofert sprzedawanych za pośrednictwem komercyjnej witryny Marketplace. Pokazuje on transakcyjną historię zarobków, szacuje następną płatność i przedstawia trendy płatności. Możesz również pobrać historię transakcji i instrukcje płatności. W tym artykule wyjaśniono, jak uzyskać dostęp do rachunku wypłaty i różne strony wypłaty oraz pliki do pobrania dostępne w centrum partnerskim.

>[!NOTE]
>Zobaczysz tylko dane dotyczące identyfikatorów MPN i programów, z którymi masz skojarzone. Aby wyświetlić dodatkowe dane, należy skontaktować się z administratorem konta w celu uzyskania uprawnień. 

## <a name="roles-and-permissions"></a>Role i uprawnienia

Aby uzyskać dostęp do instrukcji wypłaty, musisz mieć przypisany **właściciel konta** lub rola **współautor finansów** .

| Raporty/strony | Właściciel konta | Menedżer | Deweloper | Współautor firmy | Współautor finansów | Wiodący |
| --- | --- | --- | --- | --- | --- | --- |
| Raport pozyskiwania (w tym dane niemal w czasie rzeczywistym) | Może wyświetlać | Może wyświetlać | Brak dostępu | Brak dostępu | Może wyświetlać | Brak dostępu |
| Raport/odpowiedzi na Opinie | Może wyświetlać i przesyłać opinie | Może wyświetlać i przesyłać opinie | Może wyświetlać i przesyłać opinie | Brak dostępu | Brak dostępu | Może wyświetlać i przesyłać opinie |
| Raport o kondycji (łącznie z danymi niemal w czasie rzeczywistym) | Może wyświetlać | Może wyświetlać | Może wyświetlać | Może wyświetlać | Brak dostępu | Brak dostępu |
| Raport użycia | Może wyświetlać | Może wyświetlać | Może wyświetlać | Może wyświetlać | Brak dostępu | Brak dostępu |
| Konto wypłaty | Może aktualizować | Brak dostępu | Brak dostępu | Brak dostępu | Może aktualizować | Brak dostępu |
| Profil podatkowy | Może aktualizować | Brak dostępu | Brak dostępu | Brak dostępu | Może aktualizować | Brak dostępu |
| Podsumowanie wypłaty | Może wyświetlać | Brak dostępu | Brak dostępu | Brak dostępu | Może wyświetlać | Brak dostępu |
|

## <a name="access-your-payout-statement"></a>Uzyskaj dostęp do instrukcji wypłaty

Zaloguj się do [Centrum partnerskiego](https://partner.microsoft.com/dashboard/home) i wybierz ikonę wypłaty w prawym górnym rogu ekranu, aby uzyskać dostęp do tych różnych podsumowań:

- Historia transakcji
- Płatności
- Eksportowanie danych

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Przedstawia ikonę wypłaty w prawym górnym rogu portalu Centrum partnerskiego":::

Możesz również użyć [interfejsu API wypłaty partnera](https://apidocs.microsoft.com/services/partnerpayouts) , aby połączyć się i uzyskać bezpośrednią transakcję oraz dane dotyczące płatności.


## <a name="transaction-history"></a>Historia transakcji

Na stronie **Historia transakcji** są wyświetlane podsumowanie zarobków, Szacowana kolejna płatność oraz Trend zysków i płatności w ciągu ostatnich 36 miesięcy. Możesz również pobrać szczegóły transakcji z tej sekcji.


:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Przegląd transakcji.":::

- **Dochody są wysyłane w tym roku** — łączne dochody i podział zarobków, które zostały opłacone i zostaną spłacone w nadchodzącym miesiącu.
- **Szacowany miesiąc płatności** — łączne dochody oczekiwane w nadchodzących miesiącach.
- **Tendencje zarobkowe i płatnicze** — miesięczne kwoty związane z płatnościami w ciągu ostatnich 36 miesięcy.
- **Pobierz** — pobiera szczegóły transakcji w formacie CSV lub TSV.

Użyj wyboru zakresu dat w prawym górnym rogu strony, aby odfiltrować dane wyjściowe strony, aby wyświetlić ostatnich 3, 6, 12 lub 36 miesięcy. Lub wybierz niestandardowy zakres dat do 36 miesięcy. Domyślny zakres dat to 12 miesięcy. Możesz również filtrować według identyfikatora rejestracji, programu, identyfikatora płatności, typu zdobywania, dźwigni i stanu. Dane są dostępne dla bieżącego roku obrachunkowego (1 lipca, 30 czerwca) i poprzednich dwóch lat obrachunkowych.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Filtr wyszukiwania w prawym górnym rogu strony.":::

Aby wyświetlić więcej szczegółów na temat zdobywania, wybierz strzałkę w dół znajdującą się po prawej stronie. Spowoduje to wyświetlenie dźwigni, kwoty przychodu, produktu i klienta. Jeśli z jakiegoś powodu wszystkie te dane są niedostępne, ale potrzebujesz do nich dostępu, skontaktuj się z pomocą techniczną. Jeśli zdobywanie wyników jest wynikiem korekty, a nie transakcji, pola produkt i klient nie będą wyświetlane.

### <a name="transaction-history-summary"></a>Podsumowanie historii transakcji

Pokazuje to szczegółowe informacje, w tym pochodzenie z prezentów od daty sprzedaży produktu, stanu i szacowanego miesiąca płatności.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historia transakcji.":::

- **Data wypracowana** — Data zakupu.
- **Typ zdobywania** — typ zdobywania, np. sprzedaż, Rabat lub współdziałanie.
- **Łączna kwota** — kwota nakładu netto. W komercyjnej witrynie Marketplace oznacza to po potrąceniu standardowej opłaty za witrynę Marketplace.
- **Status** — ma trzy opcje:
    - **Nadchodzące** — dochody są w trakcie oczekiwania na okres chłodzenia.
    - **Przetworzone** — dochody są przygotowywane do następnej płatności.
    - **Wysłano** — dochody zostały opłacone.
- **Szacowany miesiąc płatności** — miesiąc, w którym należy zapłacić zyski. Aby uzyskać więcej informacji, zobacz [następną sekcję](#estimated-payment-month) .

Transakcje związane z zdobywaniem danych są wyświetlane, gdy transakcja spełni uprawnienia do wypłaty. Aby zrozumieć, dlaczego być może brakuje lub nieoczekiwanych zarobków, zobacz [często zadawane pytania dotyczące komercyjnych wypłat rynkowych](payout-faq.md#why-are-my-earnings-missing).

#### <a name="estimated-payment-month"></a>Szacowany miesiąc płatności

Strona Historia transakcji zawiera teraz tabelę przedstawiającą szacowane kwoty płatności w ciągu następnych kilku miesięcy. Te informacje można również wyświetlać i pobierać w raportach Historia transakcji i raporty podsumowujące. Te informacje ułatwiają uzgadnianie i projekcje płatności.

Szacowany miesiąc płatności jest obliczany na podstawie zasad konfiguracji programu i osi czasu i jest przetwarzany w następnym/przyszłym cyklu płatności.

Szacowany miesiąc płatności jest obecnie dostępny dla wszystkich typów zdobywania, z wyjątkiem współpracy, która będzie wyświetlana jako **nie dotyczy**. W przypadku zarobków przed 1 lipca 2020 szacowany miesiąc płatności zostanie **wyświetlony jako niedostępny**.

W poniższej tabeli przedstawiono szacunkowy przykład miesiąca płatności.

| Month (Miesiąc) | Kwota |
| ------ | :-----------: |
|  Wrz-2020 |  $7 273,99   |
|  Paź-2020 | $8 692,30  |
|  Lis-2020 | $107,89  |

Szacowana kwota może różnić się od rzeczywistej wartości z różnych powodów:

- Przestananie zarobków: w przypadku ponownego obliczania zarobków rzeczywista wartość będzie różna
- Korekty: rzeczywista wartość różni się w zależności od zmian, które wystąpiły lub zostały przesłane.
- Zmiana reguł: zmiana w regułach może odzwierciedlać ponowne obliczenie w rzeczywistej kwocie
- Płatne: Jeśli wystąpi błąd płatności, rzeczywista kwota może być różna

Należy pamiętać, że płatność jest dostępna tylko w przewidywanym miesiącu, jeśli spełnione są reguły dotyczące progów i uprawnień do płatności programu. Te reguły obejmują, ale nie są ograniczone do poniższej listy:

- Twój profil podatkowy musi mieć aktualną datę
- Twoje zarobki muszą być zgodne lub przekraczać minimalny próg zdobywania zdefiniowany w przewodniku programu.
- Wypłata w dniu wstrzymania: w przypadku wybrania opcji "Przechowuj moją płatność" na stronie przypisanie profilów.
- Instrument wypłaty nie jest dostępny: Profil płatności lub/i podatek nie został ukończony.

### <a name="transaction-history-download"></a>Pobieranie historii transakcji

Aby wyświetlić więcej szczegółów na temat zdobywania, wybierz pozycję **Pobierz** w górnej części strony. W poniższej tabeli opisano każdą kolumnę w raporcie.

>[!NOTE]
>Eksport do pobrania historii transakcji ma dwa nowe pola od sierpnia 2020:
>
>- **lastPaymentCurrency**  Waluta, w której otrzymano najnowszą płatność, we wszystkich usługi mpnsach, do których aktualnie zalogowany jest dostęp. Jeśli płatność nie zostanie odebrana, Ostatnia waluta płatności będzie wynosić dolarów amerykańskich.
>- **earningAmountInLastPaymentCurrency**  Kwota zdobywania w ostatniej walucie płatności.

| Nazwa kolumny | Opis | Możliwość zastosowania w przypadku programów zachęty/rynków Marketplace |
| --- | --- | --- |
| agreementEndDate | Data zakończenia umowy | Zachęty — tylko niektóre programy |
| agreementNumber | Numer umowy | Zachęty — tylko niektóre programy |
| agreementStartDate | Data rozpoczęcia obowiązywania umowy | Zachęty — tylko niektóre programy |
| calculationDate | Data obliczenia okresu zdobywania w systemie | Wszystko |
| claimId | Unikatowy identyfikator dla żądania | Zachęty — tylko niektóre programy |
| customerCountry | Kraj/region klienta | platform handlowych |
| customerEmail |  |  |
| customerName | Może być puste | Tylko programy motywacyjne (wyjątek: OEM) i Marketplace. W przypadku transakcji dostawcy CSP w witrynie Marketplace zostanie wyświetlona nazwa dostawcy usług kryptograficznych. |
| customerTenantId |  |  |
| distributorId | Identyfikator dystrybutora | Zachęty — tylko niektóre programy |
| dystrybutorname | Nazwa dystrybutora | Zachęty — tylko niektóre programy |
| earningAmount | Kwota zdobywania w pierwotnej walucie transakcji | Wszystko |
| earningAmountInLastPaymentCurrency | Kwota zarobków w ostatniej walucie płatności (pole będzie puste, jeśli nie zostały uiszczone żadne wcześniejsze płatności) |  |
| earningAmountUSD | Kwota zdobywania w USD | Wszystko |
| earningDate | Data okresu zdobywania | Wszystko |
| earningExchangeRate | Kurs wymiany używany do wyświetlania odpowiedniej ilości USD | Wszystko |
| earningId | Unikatowy identyfikator dla każdego zdobywania | Wszystko |
| earningRate | Stawka zachęt zastosowana do kwoty transakcji w celu wygenerowania zdobywania | Wszystko |
| Pozostały | Wskazuje, czy jest to opłata, Rabat, współdziałanie, sprzedaż itd. | Wszystko |
| exchangeRateDate | Data kursu wymiany używana do obliczania EarningAmount USD | Wszystko |
| externalReferenceId | Unikatowy identyfikator programu | Bezpośrednie wynagrodzenie programów (zachęty i rynki Marketplace) |
| externalReferenceIdLabel | Etykieta unikatowego identyfikatora | Bezpośrednie wynagrodzenie programów (zachęty i rynki Marketplace) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Numer faktury (dotyczy tylko przedsiębiorstwa) | Zachęty i witryny Marketplace — tylko niektóre programy |
| lastPaymentCurrency | Waluta ostatniej płatności (pole będzie puste, jeśli nie zapłacisz żadnej wcześniejszej płatności) |  |
| górę | Oznacza regułę biznesową dla zdobywania | Wszystko |
| LicensingProgramName | Nazwa programu licencjonowania |  |
| LineItemId | Pojedynczy wiersz faktury klienta |  |
| localProviderSeller | Dostawca lokalny/sprzedawca rekordu |  |
| Miesiąc zapadalności | Szacowany miesiąc płatności | Wszystko |
| OrderId (Identyfikator zamówienia) | Odnosi się do faktury klienta  | platform handlowych |
| parentProductId | Unikatowy identyfikator nadrzędnego produktu. Jeśli nie ma produktu nadrzędnego dla transakcji, identyfikator produktu nadrzędny = identyfikator produktu. | platform handlowych |
| parentProductName | Nazwa produktu nadrzędnego. Jeśli nie ma produktu nadrzędnego dla transakcji, nazwa produktu nadrzędnego = Nazwa produktu. | platform handlowych |
| participantId | Podstawowa tożsamość ponosząca partnera w ramach programu | Wszystko |
| participantIdType | Przede wszystkim IDENTYFIKATORem programu dla programów zachęt i sprzedawcy, jeśli w przypadku witryny Marketplace | Wszystko |
| uczestnikname | Nazwa partnera zdobywania | Wszystko |
| partnerCountryCode | Lokalizacja/kraj/region partnera zdobywania | Wszystko |
| partNumber | Zawsze będzie puste | Niektóre programy motywacyjne i Marketplace |
| paymentId | Unikatowy identyfikator płatności. Ta liczba jest zwykle widoczna w wyrażeniu bankowym | Tylko płatności SAP |
| paymentStatus | Stan płatności | Wszystko |
| paymentStatusDescription | Przyjazny opis stanu płatności | Wszystko |
| productId | Unikatowy identyfikator produktu | platform handlowych |
| productName | Nazwa produktu połączona z transakcją | Wszystko |
| productType | Typ produktu, taki jak aplikacja, dodatek lub gra | platform handlowych |
| Kod programu | Ciąg do mapowania przy użyciu nazwy programu |  |
| programName | Nazwa programu zachęty/sklepu | Wszystko |
| purchaseOrderCoverageEndDate | Zawsze będzie puste | Program zachęty — CRI |
| purchaseOrderCoverageStartDate | Zawsze będzie puste | Program zachęty — CRI |
| purchaseOrderType | Zawsze będzie puste | Program zachęty — CRI |
| purchaseTypeCode | Zawsze będzie puste | Program zachęty — CRI |
| quantity | Różni się w zależności od programu. Wskazuje liczbę rozliczeń dla programów transakcyjnych | Wszystko |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identyfikator odsprzedawcy | Zachęty — tylko niektóre programy |
| Nazwa odsprzedawcy | Nazwa odsprzedawcy |  |
| Identyfikatora skuId | Identyfikator jednostki SKU zdefiniowany podczas publikowania. Oferta może mieć wiele jednostek SKU, ale jednostka SKU może być skojarzona tylko z jedną ofertą. Zachęty — tylko niektóre programy |  |
| storeFee | Kwota zachowywana przez firmę Microsoft jako opłata za udostępnienie aplikacji lub dodatku w sklepie | platform handlowych |
| subscriptionEndDate | Data zakończenia subskrypcji | Zachęty — tylko niektóre programy |
| subscriptionId | Identyfikator subskrypcji skojarzony z klientem | Zachęty — tylko niektóre programy |
| subscriptionStartDate | Data rozpoczęcia subskrypcji | Zachęty — tylko niektóre programy |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Osoba odpowiedzialna za przekazaną podatki (sprzedaż, użycie lub podatki VAT/GST () | platform handlowych |
| taxRemitted | Kwota przekazanego podatku (sprzedaż, użycie lub podatki VAT/GST () | platform handlowych |
| taxState | Stan klienta |  |
| taxZipCode | Kod pocztowy klienta |  |
| tpan | Wskazuje sieć usługi AD innej firmy | tylko reklamy w witrynie Marketplace |
| transactionAmount | Kwota transakcji w pierwotnej walucie transakcji oparta na wygenerowanym wykorzystaniu | Wszystko |
| transactionAmountUSD | Kwota transakcji w USD | Wszystko |
| transactionCountryCode | Kod kraju/regionu, w którym wystąpiła transakcja |  |
| transactionCurrency | Waluta, w której wystąpiła oryginalna transakcja klienta (nie jest to waluta lokalizacji partnera) | Wszystko |
| transactionDate | Data transakcji. Przydatne w przypadku programów, w których wiele transakcji przyczynia się do jednego zdobywania | Wszystko |
| transactionExchangeRate | Data kursu wymiany używana do wyświetlania odpowiedniej kwoty (USD) transakcji | Wszystko |
| transactionId | Unikatowy identyfikator transakcji | Wszystko |
| transactionPaymentMethod | Instrument płatniczy klienta używany do transakcji, taki jak karta, rozliczenia przez przewoźnika komórkowego lub w systemie PayPal | platform handlowych |
| transactionType | Typ transakcji, taki jak zakup, zwrot, odwrócenie lub obciążenia zwrotnego | platform handlowych |
| workload | Obciążenie | Zachęty — tylko niektóre programy |
|

### <a name="transaction-adjustment-codes"></a>Kody korekty transakcji

Poniższa tabela zawiera listę kodów przyczyn korekt i ich opisy.

|**Kod przyczyny**   |**Opis**   |
|------------------|:-------------------------------------|
| CZ zgodność | Dostosowanie zmniejszające zyski w przypadku, gdy partner firmy Microsoft nie zapłacił na czas. |
| Przerzucanie operacji współpracujących | Korekta, która przenosi zyski ze współpracowników do innego okresu lub konwertuje zarobki współpracujące na rabat. |
| Korekta Ops | Korekta, która koryguje błędy obliczeń systemu firmy Microsoft. |
| Korekta Ops Microsoft — nieprawidłowe obliczenie | Korekta, która poprawia błędne obliczenia. |
| Korekta Ops niepoprawna Rejestracja firmy Microsoft | Korekta dotycząca nieudanych obliczeń związanych z rejestracją. |
| Mapowanie partnera (subskrypcja) MCI/CSP | Korekta, która poprawia niezgodność subskrypcji. |
| Wyjątek zasad | Dopasowanie, które zastępuje regułę programu.  |
| Dochody z poprzedniego okresu | Korekta dochodów poza bieżącym okresem zdobywania. |

## <a name="payments"></a>Płatności

Na stronie **płatności** znajdują się szczegóły dotyczące pieniędzy uzyskanych w firmie Microsoft. Przedstawiono w nim również czas i ilość płatności.

>[!Note]
> Aby można było skorzystać z wypłat, Twoje przejścia muszą osiągać [próg płatności](payment-thresholds-methods-timeframes.md) wynoszący $50. Aby uzyskać więcej informacji, zapoznaj się z [umową wydawcy firmy Microsoft](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Ekran przegląd płatności.":::

- **Łączny rok w tym roku** — łączna kwota płatna w tym roku w dolarach amerykańskich dla wszystkich programów.
- **Kolejna Szacowana płatność** — pojedyncza płatność, która jest już dostępna, nawet jeśli w dolarach amerykańskich istnieją inne osoby.
- **Ostatnia płatność** — kwota (w dolarach amerykańskich), nazwa programu i program z ostatniej płatności.
- **Płatność według źródła** — kwota płatności (w dolarach amerykańskich) na program w ciągu ostatnich 12 miesięcy.

### <a name="payments-list"></a>Lista płatności

W tabeli **listy płatności** są wyświetlane płatne i oczekujące płatności. Informacje podatkowe dotyczące opłat za usługę można pobrać w formacie PDF i wyświetlić szczegółowe informacje o podanej płatności.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Eksportuj historię transakcji":::

- **Płatność** — wszystkie płatności zostały pomyślnie wysłane. Wybierz rok z menu rozwijanego, aby odfiltrować do płatności wydanych w danym roku.
- **Oczekiwanie** — nadchodzące płatności.
- **Podatek z tytułu opłaty za usługę (formularz PDF)** — jest dostępny dla płatności objętych podatkiem za usługę. Podatki z opłatami za usługę są pokazywane w **innych podatkach**.
- **Widok** — przekieruje do historii transakcji z listą zarobków uwzględnionych w płatności.

Aby zrozumieć, dlaczego być może brakuje lub nieoczekiwanych zarobków, zobacz [często zadawane pytania dotyczące komercyjnych wypłat rynkowych](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Stan płatności

W poniższej tabeli objaśniono różne stany zdobywania.

| Stan zdobywania | Przyczyna | Wymagana jest akcja partnerska? |
| --- | --- | --- |
| Nieprzetworzone | Zdobywanie oferty kwalifikuje się do płatności. Pozostaje w tym stanie przez okres chłodzenia, zgodnie z definicją w przewodniku programu dla programu zachęty. | Nie |
| Nowego | Zamówienie płatności wygenerowało oczekujące przeglądy wewnętrzne przed przetworzeniem płatności. | Nie |
| Oczekująca faktura podatkowa | Twoja faktura podatkowa jest niekompletna lub nieprawidłowa. | Aby można było zapłacić, musisz zaktualizować fakturę podatkową |
| Odrzucone podczas przeglądu | Płatność została odrzucona podczas przeglądu. | Skontaktuj się z pomocą techniczną firmy Microsoft, aby uzyskać |
| Niepowodzenie | Płatność nie powiodła się z powodu błędu systemu firmy Microsoft. | Skontaktuj się z pomocą techniczną firmy Microsoft, aby uzyskać |
| W toku | Płatność jest w toku. | Nie |
| Nieprawidłowa płatność | Trwa odliczanie płatności. | Nie |
| Wysłane | Płatność została wysłana do Twojego banku. | Nie |
| Ponowne przetwarzanie | Płatność napotkała błąd systemu firmy Microsoft i trwa jego przetwarzanie. | Nie |
| Reversed | Płatność została anulowana przez Bank i zostanie wysłana ponownie w następnym cyklu płatności. | Nie |
| Faktura podatkowa została odrzucona | Twoja faktura podatkowa została odrzucona podczas przeglądu. Wszystkie oczekujące płatności zostaną wstrzymane do momentu zakończenia przeglądu faktury podatkowej. | Skontaktuj się z pomocą techniczną firmy Microsoft, aby uzyskać |
| Faktura podatkowa poddana przeglądowi | Trwa przegląd faktury podatkowej. Płatność zostanie wydana po zatwierdzeniu faktury podatkowej. | Nie |
| Odrzucone | Płatność została odrzucona przez Bank. | Aby uzyskać szczegółowe informacje, skontaktuj się z bankiem. |
|

### <a name="payments-download"></a>Pobieranie płatności

 W poniższej tabeli opisano każdą kolumnę w raporcie. Aby wyświetlić więcej szczegółów na temat płatności, wybierz pozycję **Pobierz** w górnej części strony płatności.

| Nazwa kolumny | Opis |
| --- | --- |
| participantID | Podstawowa tożsamość ponosząca partnera w ramach programu |
| participantIDType | Zwykle identyfikator programu dla programów Zachęts i identyfikator sprzedawcy dla programów do magazynowania |
| uczestnikname | Nazwa partnera zdobywania |
| programName | Zachęty/Nazwa programu w sklepie |
| procent | Kwota uzyskana w walucie płatnej dla tego programu/participantID |
| earnedUSD | Kwota uzyskana dla identyfikatora programu/uczestnika w USD |
| withheldTax | Kwota podatku potrąconego w walucie płatnej na wartość program/participantID |
| salesTax | Łączna kwota podatku od sprzedaży w walucie płatnej za program/participantID (dotyczy tylko programów zachęty) |
| serviceFeeTax | Łączna kwota serviceFeeTax w walucie płatnej dla programu/participantID (dotyczy tylko programów do magazynowania i portalu Azure Marketplace) |
| totalPayment | Całkowita płatność w walucie lokalnej z wyłączeniem potrąconego potrącenia, w tym podatek sprzedaży (jeśli dotyczy) dla programu/participantID |
| currencyCode | Płatność na kod waluty |
| paymentMethod | Metoda używana do płacenia partnera, na przykład elektronicznego przelewu bankowego, faktury kredytowej |
| paymentID | Unikatowy identyfikator płatności. Ta liczba jest zazwyczaj widoczna w sprawozdaniu bankowym (dotyczy tylko płatności SAP). |
| paymentStatus | Stan płatności |
| paymentStatusDescription | Przyjazny opis stanu płatności |
| paymentDate | Data płatności została wysłana od firmy Microsoft |
|

## <a name="export-data"></a>Eksportowanie danych

Strona **Eksportowanie danych** nie jest odświeżana samodzielnie. Może być konieczne ręczne odświeżenie strony, aby zobaczyć najnowsze dane. Wybierz jedną z trzech kart, aby wyeksportować **historię transakcji**, **płatności**, **Podsumowanie transakcji** lub **instrukcję historyczną**.

Filtr może spowodować błąd **braku dostępnych danych** . Może się tak zdarzyć, jeśli pozostały domyślny okres wybrany przez trzy miesiące, a następnie wybrano identyfikator płatności z okresu, który znajduje się poza tym okresem. Jeśli tak się stanie, rozwiń swój przedział czasu i spróbuj ponownie.

Oto przykład eksportu płatności:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Eksportuj raport płatności.":::

### <a name="historical-statements"></a>Historyczne instrukcje

Podsumowanie **eksport danych** zapewnia również dostęp do historycznych instrukcji.

> [!NOTE]
> Instrukcja historyczna jest migawką i nie jest odświeżana. W razie konieczności skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/support/v2/?stage=1) i zażądaj najnowszych danych.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Eksportuj instrukcje historyczne.":::

- Historia transakcji od dnia 1 lipca 2019 jest obsługiwana osobno i używa różnych pól z późniejszych raportów historii.
- Historia starszej transakcji zawiera kolumnę o nazwie "zarezerwowana", która odnosi się do kolumny "zarobki" w nowoczesnej historii, z tą różnicą, że wyklucza wszystkie zyski ze stanem równym "płatności wysłane".
- Filtry takie jak 3M, 6 min lub 12M nie będą miały zastosowania do sekcji Instrukcje historyczne.

### <a name="historical-statement-downloads"></a>Pobieranie instrukcji historycznych

W poniższej tabeli opisano każdą kolumnę w instrukcji historycznej.

| Nazwa pola | Opis |
| --- | --- |
| Źródło przychodu | Źródło przychodu na podstawie miejsca, w którym wystąpiła transakcja, taka jak Microsoft Store, Windows Phone Store, Sklep Windows 8 lub reklama |
| Identyfikator zamówienia | Unikatowy identyfikator zamówienia. Ten identyfikator umożliwia zidentyfikowanie transakcji zakupu z odpowiednimi transakcjami niezwiązanych z zakupami, takimi jak zwroty lub obciążeń zwrotnych. Oba będą mieć ten sam identyfikator zamówienia. Ponadto, jeśli istnieje opłata z podziałem, w przypadku której do pojedynczego zakupu użyto wielu metod płatności, umożliwia ona łączenie transakcji zakupu. |
| Transaction ID (Identyfikator transakcji) | Unikatowy identyfikator transakcji. |
| Data i godzina transakcji | Data i godzina wystąpienia transakcji (UTC). |
| Identyfikator produktu nadrzędnego | Unikatowy identyfikator nadrzędnego produktu. Jeśli nie ma produktu nadrzędnego dla transakcji, identyfikator produktu nadrzędny = identyfikator produktu. |
| Identyfikator produktu | Unikatowy identyfikator produktu. |
| Nazwa produktu nadrzędnego | Nazwa produktu nadrzędnego. Jeśli nie ma produktu nadrzędnego dla transakcji, nazwa produktu nadrzędnego = Nazwa produktu. |
| Nazwa produktu | Nazwa produktu |
| Typ produktu | Typ produktu, taki jak aplikacja, dodatek lub gra |
| Liczba | Gdy źródło przychodu jest Microsoft Store dla firm, ilość reprezentuje liczbę zakupionych licencji. Dla wszystkich innych źródeł przychodu wartość ta będzie zawsze wynosić 1. Nawet wtedy, gdy pojedyncza transakcja jest dzielona na dwa elementy wiersza, ponieważ użyto dwóch różnych metod płatności, każdy element wiersza będzie wyświetlał liczbę 1. |
| Typ transakcji | Typ transakcji, taki jak zakup, zwrot, odwrócenie lub obciążenia zwrotnego |
| Forma płatności | Instrument płatniczy klienta używany do transakcji, taki jak karta, rozliczenia przez przewoźnika komórkowego lub w systemie PayPal |
| Kraj/region | Kraj/region, w którym wystąpiła transakcja |
| Dostawca/sprzedawca lokalny | Dostawca lokalny/sprzedawca rekordu |
| Waluta transakcji | Waluta transakcji |
| Kwota transakcji | Kwota transakcji |
| Podatek przekazany | Kwota przekazanego podatku (sprzedaż, użycie lub podatki VAT/GST () |
| Przychody netto | Kwota transakcji pomniejszona o podatek |
| Opłata za Sklep | Odsetek potwierdzeń netto przechowywanych przez firmę Microsoft jako opłata za tworzenie aplikacji lub dodatków dostępnych w sklepie |
| Dalsze aplikacje | Przychody netto pomniejszone o opłatę za Sklep |
| Potrącone podatki | Kwota potrąconego podatku dochodowego (z uwzględnieniem **zastrzeżonego** pliku CSV) |
| Płatność | Aplikacja pozyskuje mniejsze kwoty dotyczące potrącenia podatku dochodowego (kwota pokazana w walucie transakcji). Nie uwzględniono w **zastrzeżonym** pliku CSV. |
| Szybkość FX | Obcy kurs wymiany używany do konwersji waluty transakcji na walutę płatności |
| Waluta płatności | Waluta, w której dokonywana jest płatność |
| Przekonwertowana płatność | Kwota płatności konwertowana na walutę płatności przy użyciu kursu FX |
| Model przyliczania podatku | Osoba odpowiedzialna za przekazaną podatki (sprzedaż, użycie lub podatki VAT/GST () |
| Data i godzina kwalifikacji | Data i godzina, kiedy transakcja będzie kontynuowała płatności (UTC). Gdy zostanie utworzona wypłata, obejmuje ona transakcje, które są uwzględniane przed datą utworzenia wypłaty (tylko w **zastrzeżonym** pliku CSV). |
| Opłaty | Pokazuje podział wszystkich szczegółów opłaty zagregowanych w kolumnie kwota transakcji (uwzględnionych tylko w portalu Azure Marketplace), które nie znajdują się w **zastrzeżonym** pliku CSV. |
|||

## <a name="next-steps"></a>Następne kroki

- [Interfejs Partner Payout API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Szczegóły zasad wypłat](payout-policy-details.md)
- Aby uzyskać pomoc techniczną, skontaktuj się z działem [pomocy technicznej wydawcy](https://partner.microsoft.com/support/v2/?stage=1)w portalu Marketplace.
