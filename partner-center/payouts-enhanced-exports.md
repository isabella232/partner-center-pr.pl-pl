---
title: Strona eksportowania danych wypłat
description: Wyjaśnia, jak używać rozszerzonej strony eksportowania danych do generowania dostosowanych raportów historii transakcji
author: Satinder37
ms.author: sabajaj
ms.topic: how-to
ms.date: 10/04/2021
ms.custom: template-how-to
ms.openlocfilehash: 9ac19a8ea42020b4ec2543d9f4ef197eb95e3a61
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528638"
---
# <a name="payouts-export-data-page"></a>Strona eksportowania danych wypłat
**Odpowiednie role:** Zachęty dla administratorów | Zachęty użytkownika

W tym artykule omówiono ulepszenia funkcji eksportowania danych dla wypłat **w** Partner Center. To środowisko z przewodnikiem zawiera nowe szablony domyślne do eksportowania raportów historii transakcji. Ma ona również funkcję dynamiczną, która umożliwia tworzenie własnych, dostosowanych szablonów dla raportów historii transakcji.

## <a name="access-the-export-data-page"></a>Uzyskiwanie dostępu do strony eksportowania danych
1.  Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego.
2.  Wybierz **pozycję Wypłaty,** a następnie wybierz **pozycję Eksport zachęt** lub Historia **transakcji** z menu.

> [!Note] 
> Będziesz mieć dostęp do tej strony, jeśli jesteś administratorem [zachęt lub użytkownikiem zachęty.](/payout-statement#roles-and-permissionsData) To, co zobaczysz, będzie zależeć od tego, do którego programu  i Microsoft Partner Network (MPN), do których masz dostęp (podobnie jak w przypadku historii transakcji **i stron** płatności).

## <a name="export-your-data"></a>Eksportowanie danych
1.   Wybierz typ danych, które chcesz wyeksportować. 
      - W przypadku raportu historii transakcji wybierz **pozycję Zarobki, transakcja, szczegóły stanu płatności.**  Należy **pamiętać, że szczegóły zarobków, transakcji i stanu** płatności (dźwignie wzrostu) nie mają zastosowania do platform komercyjnych. 
      - W przypadku raportu płatności wybierz pozycję **Szczegóły płatności.**
   :::image type="content" source="images/payouts/type-of-data.png" lightbox="images/payouts/type-of-data.png" alt-text="Zrzut ekranu przedstawiający typ wybranych danych.":::

2.   Wybierz typ szablonu raportu.

      :::image type="content" source="images/payouts/report-template-type.png" lightbox="images/payouts/report-template-type.png" alt-text="Zrzut ekranu przedstawiający wybrane typy szablonów raportu.":::

      Wybór dla kroku 1 określi opcje szablonu dla kroku 2. Jeśli na przykład w kroku 1 wybierzesz szczegóły **zarobków,** transakcji i stanu płatności, zobaczysz cztery różne opcje szablonu:
      - **Domyślna historia transakcji:** ten raport przedstawia wszystkie możliwe atrybuty dostępne w raporcie we wszystkich programach (zachęty, platformy handlowe i platformy handlowe dla konsumentów). Był to szablon pobierania dostępny przed październikiem 2021 r.
      - **Domyślny rynek:** ten raport przedstawia wszystkie atrybuty wymagane dla członków MPN zarejestrowanych w programach platformy handlowej, takich jak Azure Marketplace. 
      - **Magazyn domyślny:** ten raport przedstawia wszystkie atrybuty wymagane przez członków MPN zarejestrowanych w programach sklepów konsumenckich, takie jak Microsoft Store, Minecraft i MS Flight Simulator. 
      - **Niestandardowa historia transakcji:** ten raport umożliwia dostosowanie raportu historii transakcji.

      W przypadku **wybrania w** kroku 1 szczegółów zarobków, transakcji i stanu płatności będzie można wybrać szablon Podsumowanie **transakcji** w kroku 2. W przypadku wybrania **opcji Szczegóły płatności** w kroku 1 zobaczysz jeden szablon "Płatności" w kroku 2. Jeśli w kroku 1 wybierzesz pozycję Szczegóły przychodu z **AGI,** będzie można wybrać między wartością  **Przychód** programu lub Klient dodaje szablony w kroku 2.

3. Wybierz format pliku raportu.
   
      :::image type="content" source="images/payouts/report-file-format.png" lightbox="images/payouts/report-file-format.png" alt-text="Zrzut ekranu przedstawiający wybrane formaty plików raportu.":::

4.   Wybierz okres i zastosuj inne filtry, a następnie wybierz **pozycję Pobierz dane.**
   
      :::image type="content" source="images/payouts/time-period-filters.png" lightbox="images/payouts/time-period-filters.png" alt-text="Zrzut ekranu przedstawiający wybór i opcję filtrowania okresu w raporcie.":::

> [!Note] 
> Możesz eksportować dane i zarządzać żądaniami z **tabeli Żądania** pobierania.

## <a name="create-your-customized-transaction-history-report"></a>Tworzenie dostosowanego raportu historii transakcji

Dostosuj raport uzgadniania historii transakcji do swoich potrzeb. Można utworzyć maksymalnie pięć szablonów raportów i zarządzać nimi. 

1.  Wybierz **pozycję + Niestandardowa historia transakcji,** aby skonfigurować nowy szablon uzgodnień. 
   
      :::image type="content" source="images/payouts/custom-trans-history.png" lightbox="images/payouts/custom-trans-history.png" alt-text="Zrzut ekranu przedstawiający konfigurację niestandardowej historii transakcji.":::


2.   Wprowadź nazwę szablonu i krótki opis, a następnie wybierz pozycję **Dalej.**
   
      :::image type="content" source="images/payouts/template-name.png" lightbox="images/payouts/template-name.png" alt-text="Zrzut ekranu przedstawiający nowe pola szablonu uzgodnień niestandardowych.":::


3.  Wybierz kolumny danych, które chcesz dołączyć, i przejrzyj kolumny domyślne, które są już wymienione w raporcie. Wybierz opcję **Dalej**.
   
     :::image type="content" source="images/payouts/data-selection.png" lightbox="images/payouts/data-selection.png" alt-text="Zrzut ekranu przedstawiający opcje wyboru danych nowego szablonu uzgodnień niestandardowych.":::

4.  Przejrzyj szczegóły szablonu i wybrane dane, w razie potrzeby dokonaj edycji, a następnie wybierz **pozycję Utwórz szablon niestandardowy.**
   
      :::image type="content" source="images/payouts/new-custom-template.png" lightbox="images/payouts/new-custom-template.png" alt-text="Zrzut ekranu przedstawiający ekran potwierdzenia dla nowego niestandardowego szablonu uzgodnień.":::

5.  Wybierz **pozycję** Pobierz z następnego ekranu, aby wyeksportować dane. Możesz również dodawać, edytować, pobierać i usuwać inne szablony z tego ekranu.
   
      :::image type="content" source="images/payouts/download-manage-templates.png" lightbox="images/payouts/download-manage-templates.png" alt-text="Zrzut ekranu przedstawiający opcje zarządzania szablonami i pobierania danych.":::

## <a name="next-steps"></a>Następne kroki
- [Omówienie wypłat](non-payment-fraud-misuse.md)
- [Podsumowanie przychodów](revenue-summary.md)
- [Zestawienia wypłat](payout-statement.md)
- [Typowe pytania dotyczące wypłat i podatków](payout-faq.yml)
