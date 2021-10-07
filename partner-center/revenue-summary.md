---
title: Podsumowanie przychodów na pulpicie Partner Center nawigacyjnym
description: Możesz użyć podsumowania Przychody, aby zrozumieć, w jaki sposób przychód generowany przez użycie usług platformy Azure przez klientów wpływa na twoje zarobki i dlaczego niektóre przychody mogą być określone jako niekwalifikują się do zarobków.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 11e58324adf38e92fc892ec5dd62933e6372f2cb
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593348"
---
# <a name="revenue-summary"></a>Podsumowanie przychodu

Możesz użyć podsumowania Przychody, aby zrozumieć, w jaki sposób przychód generowany przez użycie usług platformy Azure przez klientów wpływa na twoje zarobki i dlaczego niektóre przychody mogą być określone jako niekwalifikują się do zarobków.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Diagram przedstawiający sposób, w jaki przychód jest oceniany i raportowany na Partner Center":::

Podsumowanie Revenue (Przychód) jest aktualizowane dopiero po ocenie transakcji, więc zużycie platformy Azure, które ma miejsce w październiku, nie jest wyświetlane na przykład w podsumowaniu Revenue (Przychód) do listopada.

Podsumowanie Przychody znajduje się w obszarze roboczym Wypłaty wraz ze stroną [Historia transakcji](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) [i Płatności.](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)

## <a name="using-the-revenue-summary"></a>Korzystanie z podsumowania przychodów

Korzystając z podsumowania Przychody, możesz:

- Sprawdź kwalifikowany przychód i kwotę wynikowych zarobków według klienta lub subskrypcji.
- Uzupełnij informacje z historii [transakcji o](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  szczegółowe informacje o podstawowych kwotach przychodów.
- Sprawdź wszelkie niekwalifikowane przychody i dowiedz się, dlaczego ten przychód został sklasyfikowany jako niekwalifikuje się.
- Eksportuj dane dotyczące transakcji, które [](#ineligibility-reasons) nie są kwalifikowane, w tym przyczyny niekwalifikowalności i atrybuty [,](#exported-data-attributes)co pomaga zrozumieć, dlaczego te transakcje nie zdobywały zachęt.

## <a name="access-roles-and-permissions"></a>Role i uprawnienia dostępu

Użytkownicy zachęt i administratorzy zachęt mają dostęp do podsumowania Przychody.
Informacje dostępne w podsumowaniu zależą od kombinacji programów i Microsoft Partner Network (MPN), do których ci użytkownicy i administratorzy mają dostęp (podobnie jak w przypadku stron Historia transakcji i Płatności). (Zobacz [Przypisywanie ról i uprawnień,](permissions-overview.md) aby dowiedzieć się więcej o ustawianiu użytkowników przy użyciu ról i haseł).

## <a name="when-data-is-available"></a>Gdy dane są dostępne

Dane użycia platformy Azure są zwykle oceniane kilka tygodni po miesiącu, w którym występują transakcje. Podsumowanie przychodów jest aktualizowane tylko po zakończeniu tej oceny. Powoduje to opóźnienie między wystąpieniami transakcji a ich raportem, dlatego nie będzie można zobaczyć zużycia dla bieżącego miesiąca w podsumowaniu Przychody. Na przykład dane z marca są zwykle oceniane w trzecim tygodniu kwietnia, a informacje podsumowania przychodu są zwykle aktualizowane wkrótce później.

## <a name="customer-summary-view"></a>Widok podsumowania klienta

Widok Podsumowanie klienta przedstawia zagregowany przychód według nazwy klienta i programu/zaangażowania.

Szczegółowe informacje dotyczące podsumowania klientów obejmują:

- **10 najlepszych według kwalifikujących się przychodów** pokazuje 10 klientów, którzy najbardziej przyczyniają się do maksymalnego kwalifikowania się przychodu.
- **10 najlepszych według niekwalifikujące** się przychodów pokazuje 10 najlepszych klientów, którzy przyczyniają się do maksymalnego przychodu bez kwalifikowania się.
- **10 najlepszych według zarobków pokazuje** 10 najlepszych klientów, którzy mają wpływ na maksymalne zarobki.

W podsumowaniu klienta możesz wyszukać informacje o dowolnym kliencie, a nie tylko o 10 najlepszych.

## <a name="eligible-transactions"></a>Kwalifikujące się transakcje

*Kwalifikujące się transakcje* to transakcje, które dają przychód, który kwalifikuje się do płatności zarobków.

Możesz wyszukać informacje o kwalifikujących się transakcjach według identyfikatora klienta lub identyfikatora subskrypcji. Nie można jednak eksportować danych dotyczących kwalifikujących się transakcji.

## <a name="ineligible-transactions"></a>Transakcje bez kwalifikowania

*Transakcje, które nie są* kwalifikowane, to transakcje, które nie są kwalifikowane do płatności zarobków.

- Przyczyny, dla których wszelkie transakcje są uznawane za niekwalifikują się do zarobków, są wymienione w sekcji [Przyczyny](#ineligibility-reasons) niekwalifikowalności tego artykułu.
- Możesz wyszukiwać  [i](#exporting-data) eksportować dane dotyczące transakcji, które nie są kwalifikowane, aby dowiedzieć się, dlaczego nie zostały uzyskane zachęty MCI.
- W podsumowaniu Revenue (Przychód) jest zawsze wyświetlana najnowsza klasyfikacja przychodów (więc nie widzisz, jak transakcja została sklasyfikowana miesiąc wcześniej). Transakcja oznaczona jako niekwalifikowalna przez jeden miesiąc może zostać oznaczona jako kwalifikująca się w następnym miesiącu.

Transakcje bez kwalifikowania wymienione w podsumowaniu Przychody mają atrybuty, które obejmują:

- product
- niekwalifikuje się przychód
- [przyczyna niekwalifikowalności](#ineligibility-reasons)
- subscription ID
- nazwa klienta (zazwyczaj dostępna po zafakturowej subskrypcji po raz pierwszy)

Transakcje, które nie są kwalifikowane, można wyszukiwać według nazwy klienta i identyfikatora subskrypcji. (Liczba wyświetlanych rekordów jest ograniczona do 10). Jeśli informacje, które znajdziesz, nie odpowiadają na Twoje pytania, skontaktuj się z pomocą techniczną, aby uzyskać pomoc.

## <a name="ineligibility-reasons"></a>Przyczyny niekwalifikowalności

*Przyczyny kwalifikacji w* poniższych tabelach wskazują, dlaczego przychód został sklasyfikowany jako niekwalifikuje się do zarobków. Każdy wiersz w tabelach zawiera również wyjaśnienie, czy i w jaki sposób partner z niekwalifikowymi zarobkami może ponownie kwalifikować się do zarobków.

Niektóre przyczyny niekwalifikowalności w tych tabelach mogą nie mieć zastosowania do określonego zaangażowania.

Istnieją trzy kategorie uprawnień:

- [Klient bez kwalifikowania się](#ineligible-customer)
- [Partner bez kwalifikowania się](#ineligible-partner)
- [Bez kwalifikowania się transakcji](#ineligible-transaction)

### <a name="ineligible-customer"></a>Klient bez kwalifikowania się

|Przyczyna niekwalifikowalności|Wymagana jest akcja partnera?|Jak ponownie zakwalifikować się|
|---------|---------|---------|
|Klient jest sektorem publicznym|Tak, jeśli klient znajduje się w Stany Zjednoczone, Portoryko lub Indiach|Jeśli odpowiedź na żądanie weryfikacji wykonania (POE) została odrzucona, nie można ponownie kwalifikować się. (Po odrzuceniu wytłaniania jest wysyłana wiadomość e-mail z wyjaśnieniem, dlaczego).<br><br>Możesz zażądać kolejnego zakupu zakupu w ciągu 90 dni od daty transakcji/zarobków. (Pamiętaj, aby potwierdzić odebranie wiadomości e-mail z potwierdzeniem zakupu zakupu po jej odebraniu). W ciągu 90 dni możesz również zakwestionować kwalifikowalność, kontaktując się z pomocą techniczną w sprawie przyczyny kwalifikowalności, subskrypcji i informacji o klientach oraz przyczyny sporów.|
|Przychody w Chinach nie powinny należeć do partnera spoza Chin|Nie|Partner nie może ponownie kwalifikować się przez zasady.|

### <a name="ineligible-partner"></a>Partner bez kwalifikowania się

|Przyczyna niekwalifikowalności|Wymagana akcja partnera|Jak ponownie zakwalifikować się|
|---------|---------|---------|
|Zaawansowane wymaganie dotyczące specjalizacji nie jest spełnione|Tak|[Dowiedz się więcej o zaawansowanych specjalizacjach](advanced-specializations.md)|
|Stan kompetencji nie został spełniony lub wygasł|Tak|Wyświetl stan kompetencji na stronie [Competencies (Kompetencje).](https://partner.microsoft.com/pcv/partnership/competencies) Wyświetl wymagane kompetencje dla swojego zaangażowania na [stronie Incentives Engagements (Zachęty i zaangażowanie)](https://partner.microsoft.com/dashboard/incentives/engagements/ux)|
|Umowa MPA wygasła lub nie została podpisana|Tak|Zweryfikuj i podpisz umowę MPA, korzystając [ze wskazówek Microsoft Partner Agreement dla partnerów programu CSP](microsoft-partner-agreement.md)|
|Uprawnienie do współpracy sprzedaży wygasło lub nie ustanowiono|Tak|Zobacz Co-sell with Microsoft sales teams and partners overview (Wspólna sprzedaż [z zespołami sprzedaży i partnerami firmy Microsoft — omówienie)](/azure/marketplace/co-sell-overview)|
|Lokalizacja partnera nie kwalifikuje się do zachęt|Nie|Partner nie może ponownie kwalifikować się przez zasady|
|Identyfikator MPN, który nie kwalifikuje się do uczestnictwa w angażowania|Nie|Partner nie może ponownie kwalifikować się przez zasady|

### <a name="ineligible-transaction"></a>Bez kwalifikowania się transakcji

|Przyczyna niekwalifikowalności|Wymagana jest akcja partnera?|Jak ponownie zakwalifikować się|
|---------|---------|---------|
|Potwierdzenie wykonania nie jest zatwierdzone|Tak, jeśli nie odpowiadasz na wiadomość e-mail firmy Microsoft na potrzeby weryfikacji wykonania (POE, proof of execution required) partnera cyfrowego|Żądanie potwierdzenia wykonania ma zastosowanie tylko do sektora publicznego lub DPOR. Od 1 października 2021 r. DPOR nie jest już nakierowany na platformę Azure, dlatego żądania poe nie są wysyłane.<br><br>Jeśli na wiadomość e-mail z tematem "Wymagana jest potwierdzenie wykonania" i twoja odpowiedź została odrzucona, nie możesz ponownie kwalifikować się.|

## <a name="exporting-data"></a>Eksportowanie danych

Możesz pobrać informacje o transakcjach, które nie są uprawnione (ale niekwalifikują się) w podsumowaniu przychodu.

:::image type="content" source="images/revenue-summary/export-data-page.png" alt-text="Zrzut ekranu przedstawiający stronę Eksportowanie danych w Partner Center":::

### <a name="exported-data-attributes"></a>Atrybuty wyeksportowanych danych

Atrybuty transakcji, które nie są kwalifikowane:

|Nazwa atrybutu  |Opis  |
|---------|---------|
|agreementNumber|Numer umowy (dostępny tylko w odpowiednich przypadkach)|
|customerId|Tożsamość klienta skojarzonego z subskrypcją/zasobem. (W przypadku użycia platformy Azure te informacje nie są dostępne przez pierwsze 30–45 dni nowej subskrypcji, chyba że utworzono pierwszą fakturę).|
|customerIdType|Identyfikator TPID lub MCAPI|
|Customername|Nazwa klienta|
|invoiceNumber|Numer faktury (dostępny tylko dla partnerów, kierowanych przez pola i kierowanych przez klienta)|
|partnerCountryCode|Zarejestrowanej lokalizacji MPN|
|partnerId|Identyfikator MPN zarejestrowanego partnera|
|nazwa_partnera|Nazwa partnera|
|productId|Nazwa produktu handlowego|
|productFamily|Rodzina produktów|
|reason|Przyczyna niekwalifikowalności|
|subscriptionId|Identyfikator subskrypcji|
|transactionAmountUSD|Kwota zużycia w dolarach amerykańskich|
|Transactiondate|Data zużycia lub rozliczenia
|unearnedId|Unikatowy identyfikator, który może pomóc w utworzeniu zapytania o pomoc techniczną|
|workload|Nazwa usługi lub nazwa obciążenia|

## <a name="next-steps"></a>Następne kroki

Aby uzyskać więcej informacji o transakcjach, przychodach, zarobkach i płatnościach, zobacz następujące artykuły.

- Wyświetl stronę [Historia transakcji,](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) aby wyświetlić zarobki i powiązane szczegóły transakcji dla wszystkich programów z odpowiednim stanem płatności.
- Wyświetl stronę [Płatności, aby](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments) wyświetlić ukończone i oczekujące płatności dla wszystkich programów.
- Wyświetl stronę [Zestawienia wypłat,](payout-statement.md) aby uzyskać przegląd wypłat z ofert sprzedawanych za pośrednictwem platformy handlowej.
