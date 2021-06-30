---
title: Rejestracja transakcji
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zarejestrowanie transakcji, która wygrała w Partner Center, ułatwia firmie Microsoft zapewnienie większej liczby możliwości w przyszłości.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080669"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Rejestrowanie transakcji, które zostały wygrane w Partner Center

**Odpowiednie role:** Administrator poleceń

Możesz zarejestrować transakcje, które zostały Partner Center, podając dodatkowe informacje o kontrakcie. Te informacje pomagają nam zapewnić więcej możliwości w przyszłości.

Istnieją dwie ścieżki, które prowadzą do rejestracji transakcji:

- Utworzono nową ofertę w sekcji **Możliwości** współpracy sprzedaży, a Twoja transakcja spełnia kryteria rejestracji transakcji.
- Chcesz zgłosić zamkniętą umowę programu ISV Connect, która nie została sprzedana razem z firmą Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Rejestrowanie transakcji pochodzącej z szansy sprzedaży

Jeśli chcesz zarejestrować ofertę pochodzącą z możliwości współpracy sprzedaży, Twoja transakcja musi spełniać następujące wymagania dotyczące uprawnień:

- Typ transakcji jest typu "co sell" lub "led" przez partnera (wybrano, aby umożliwić sprzedawcom firmy Microsoft wyświetlanie tej transakcji).
- W transakcji istnieje co najmniej jedno rozwiązanie kwalifikujące się do zachęt. Rozwiązanie kwalifikuje się do zachęty, jeśli zawiera co najmniej jeden z następujących tagów:
  - Współsieć adresów IP platformy Azure
  - Business Applications Premium
  - Business Applications Standardowa
- Stan transakcji to "Won".
- Jeśli typ transakcji to współpraca sprzedaży, firma Microsoft musi zaakceptować zaproszenie lub oznaczone jako wygrane. Stan firmy Microsoft można sprawdzić, patrząc na kartę Microsoft poniżej szczegółów transakcji.

Jeśli zostały spełnione wymagania dotyczące uprawnień, zostanie automatycznie wyświetlony monit o  zarejestrowanie transakcji przy użyciu przycisku Zarejestruj teraz wyświetlanego na pasku postępu transakcji:

:::image type="content" source="images/register-deals.png" alt-text="Zrzut ekranu przedstawiający pasek postępu transakcji.":::

> [!NOTE]
> Jeśli element **rejestracji transakcji** nie jest pokazywany na pasku postępu transakcji dla Twojej transakcji, transakcja nie spełnia wszystkich wymagań dotyczących rejestracji transakcji.

Po kliknięciu **przycisku** Zarejestruj teraz nastąpi przekierowanie do strony Rejestracja transakcji i zostanie wyświetlony monit o wypełnienie formularza, który zawiera wstępnie wypełnione informacje o kliencie i rozwiązaniu. Wypełnij formularz, korzystając z poniższych instrukcji, a następnie kliknij pozycję **Zarejestruj.**

Podczas rejestracji zostanie utworzony jeden lub dwa rekordy rejestracji transakcji w zależności od rozwiązania.

- Jeśli Twoje rozwiązanie kwalifikuje się do korzystania z programu ISV Connect, zostanie utworzony rekord rejestracji transakcji programu ISV Connect. Ten rekord rejestracji transakcji będzie używany do fakturowania.
- Jeśli Twoje rozwiązanie kwalifikuje się do zachęt do współpracy sprzedaży ip, zostanie utworzony rekord rejestracji transakcji sprzedaży dla adresu IP. Ten rekord rejestracji transakcji zostanie przejrzony i zatwierdzony lub odrzucony przez zespół do przeglądu transakcji sprzedaży.

## <a name="report-a-closed-isv-connect-deal"></a>Zgłaszanie zamkniętej transakcji isv connect

Aby zgłosić zamkniętą umowę programu ISV Connect, przejdź do karty **Rejestracja** transakcji i kliknij pozycję + Zgłoś zamkniętą ofertę **programu ISV Connect.** Wypełnij wymagane pola i kliknij pozycję **Zarejestruj.** Ten rekord rejestracji transakcji będzie używany do fakturowania.

## <a name="fill-out-the-deal-registration-form"></a>Wypełnij formularz rejestracji transakcji

> [!NOTE]
> Transakcje można filtrować według nazwy klienta, stanu i typu transakcji. W tym celu kliknij przycisk **Filtruj** w górnej części strony Rejestracja transakcji.

Niezależnie od tego, czy przyszliśmy do rejestracji transakcji z możliwości sprzedaży, czy zgłaszasz zamkniętą ofertę programu ISV Connect, która nie została sprzedana razem z firmą Microsoft, zostanie wyświetlony monit o wypełnienie poniższych pól w formularzu rejestracji transakcji.

- **Szczegóły klienta:** wprowadź **nazwę firmy** dla klienta i wybierz jego **kraj/region.** Następnie wprowadź nazwę **City (Miasto)** **i State/Province (Województwo).**
- **Rozwiązanie:** Wybierz rozwiązanie, które będzie używane dla transakcji. Jeśli nie widzisz odpowiedniego rozwiązania na liście, skontaktuj się z pomocą techniczną.
- **Typ kontraktu:** określ, czy ta transakcja jest **nową umową,** **czy** odnowieniem poprzedniego kontraktu.
- **Łączna wartość kontraktu:** łączna oczekiwana wartość dla zaangażowania. Ta wartość powinna obejmować wszystkie opłaty za oprogramowanie i usługę, ale nie koszty sprzętu. Pamiętaj, aby wybrać odpowiednią walutę.
- **Wartość rozwiązania:** łączna wartość rozwiązania w chmurze, które zostanie użyte w transakcji. Pamiętaj, aby uwzględnić wszystkie koszty związane z opłatami za oprogramowanie i konserwację, ale nie obejmują elementów z możliwością ponownego zwrotu, cyklicznych opłat za dostosowywanie ani bezpośrednio skojarzonych opłat licencyjnych CSP zapłaconych przez firmę Microsoft.
- **Czy rozwiązanie zostanie wdrożone na platformie Azure? Jeśli nie, wybierz pozycję Inne:** wybierz pozycję **Azure** lub **Inne.**
- **Czy zużycie rozwiązania będzie działać w dzierżawie partnera** lub dzierżawie klienta? : Wybierz dzierżawę Klient **lub** **Dzierżawę partnera.**
- **Data rozpoczęcia kontraktu:** data rozpoczęcia kontraktu. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty pierwszej faktury. Domyślnie Partner Center nie pozwala na wprowadzenie daty rozpoczęcia wcześniejszej niż data podpisania kontraktu. Może to mieć wpływ na niektóre transakcje, takie jak wdrożenia adresów IP, które rozpoczną się przed datą podpisania. Aby pomyślnie wprowadzić te transakcje, użyj  daty podpisania kontraktu w polach daty podpisania i daty rozpoczęcia podczas przesyłania. (Kontrakt powinien jawnie określić czas trwania transakcji, aby można było prawidłowo obliczyć wartość ACV).
- **Data zakończenia kontraktu:** jeśli kontrakt zakończy się w określonej dacie, wybierz pozycję Ma **datę zakończenia** i podaj tę datę. Jeśli kontrakt nie ma określonej daty zakończenia, wybierz pozycję **Bezterminowe**. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty ostatniej lub najnowszej faktury.
- **Data podpisania** kontraktu: data podpisania umowy końcowej przez organizację i klienta. W przypadku transakcji z płatnością zgodnie z użyciem (PAYG, pay-as-you-go) użyj daty pierwszej faktury.
- **Osoba kontaktowa** rejestracji: **imię,** **nazwisko,**  **numer** telefonu i adres e-mail osoby w organizacji, z którą możemy się skontaktować, jeśli potrzebujemy dodatkowych informacji na temat dowolnej z podanych tutaj informacji.

Po ukończeniu wszystkich sekcji strony kliknij pozycję **Zarejestruj.**

- Jeśli transakcja to transakcja isV Connect, zauważysz, że stan transakcji to "Przesłane, Ukończone". W przypadku tego rekordu rejestracji transakcji nie są wymagane żadne dalsze działania. Ten rekord zostanie użyty do fakturowania.
- Jeśli transakcja jest transakcja sprzedaży typu IP, możesz zauważyć, że stan transakcji to "Przesłane". Zespół reenzentów transakcji sprzedaży firmy Microsoft przejmie informacje podane w rekordzie rejestracji transakcji. W razie potrzeby zespół reenzentów zażąda od Ciebie więcej akcji lub bezpośrednio zatwierdzi/odrzuci ofertę.
- Jeśli rejestrujesz ofertę pochodzącą z możliwości współpracy sprzedaży i zobaczysz, że utworzono dwa rekordy rejestracji transakcji, oznacza to, że rozwiązanie w Twojej transakcji kwalifikuje się zarówno do programu ISV Connect, jak i do współsiezyny adresów IP. Rekord ISV Connect będzie używać do fakturowania. Rekord współs sprzedaży dla adresu IP zostanie przejrzęcy przez zespół weryfikacji transakcji sprzedaży.

