---
title: Rozwiązywanie problemów z łącznikami poleceń do współpracy sprzedaży
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Poznaj odpowiedzi na często zadawane pytania dotyczące używania łączników wspólnej sprzedaży. Przeczytaj te często zadawane pytania dotyczące rozwiązywania problemów z łącznikami do współs sprzedaży.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: af5f54f1bc4b03fcea0d5aed62f8541c5202166793ab189e355bb2e560fd9f00
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115679976"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Rozwiązywanie problemów z łącznikami poleceń do współpracy sprzedaży

**Dotyczy:** Dynamics 365 CRM | Salesforce CRM

**Odpowiednie role:** Administrator poleceń | Administrator systemu lub customizer systemu w systemie CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Pytania i odpowiedzi dotyczące wymagań wstępnych

1. Czy możesz użyć próbnego rozwiązania łączników poleceń do współpracy sprzedaży w swoim środowisku?

Jeśli jesteś w środowisku testowym/przejściowym, możesz wybrać rozwiązanie w wersji próbnej. Płatna wersja łączników jest dostępna w usłudze AppSource w cenie 15 USD/miesiąc. W przypadku połączenia płatnego będziesz otrzymywać 10 000 wywołań interfejsu API dziennie. Łączniki są otoką na Partner Center interfejsów API poleceń. Zawsze, gdy rozwiązania  łącznika  są uruchamiane dla zdarzenia Utwórz lub Aktualizuj w przypadku szans sprzedaży Partner Center lub po stronie CRM, jest uruchamiane wywołanie interfejsu API.

2. Jaka rola jest potrzebna do tworzenia sekcji w środowisku CRM?

Użytkownicy, którzy są administratorami systemu lub osobami modyfikującymi system, mogą stosować zmiany dla wszystkich użytkowników. Jednak wszyscy użytkownicy aplikacji mogą personalizować system, a nawet udostępniać niektóre z ich dostosowań innym. 

3. Czy sprzedawcy partnerscy potrzebują specjalnych ról, aby pracować nad Partner Center?
 
Sprzedawcy partnerscy muszą mieć przypisaną rolę "Administrator poleceń". Aby uzyskać więcej informacji, zobacz [Omówienie uprawnień.](create-user-accounts-and-set-permissions.md)

4. Jakie pola należy najpierw skonfigurować w środowisku CRM? 

• Upewnij się, że Waluta jest odpowiednia dla Twojej lokalizacji i dokładnie znajduje się w środowisku CRM. • Twój zespół sprzedaży powinien być wymieniony w Twoim środowisku CRM jako użytkownicy CRM.

5. Jakie wymagania wstępne są wymagane do Power Automate środowiska?

Aby używać Power Automate, potrzebne są:

- Wymagana Power Automate licencji.
- Wymagany jest co najmniej 1 GB miejsca do magazynowania.

6.  Czy do korzystania z rozwiązania Łączniki usługi Salesforce potrzebujesz subskrypcji usługi Dynamics 365?

Rozwiązanie łącznika usługi Salesforce jest typu "Dynamics Flow", które obsługuje synchronizację z innymi systemami CRM. Rozwiązanie nie wymaga wystąpienia usługi Dynamics 365 ani subskrypcji. Podczas instalowania rozwiązania Salesforce może pojawić się lista rozwijana z istniejącym środowiskiem usługi CDS w firmie. Musisz wybrać to środowisko. Ponadto jeśli wystąpi błąd "Nie można odnaleźć organizacji usługi Dynamics 365 połączonej z zalogowanym użytkownikiem", konieczne będzie utworzenie nowego środowiska dla łącznika.

## <a name="questions-and-answers-about-configuration"></a>Pytania i odpowiedzi dotyczące konfiguracji

1. Co należy zrobić, jeśli podczas aktywowania przepływów na platformie Power Automate Platform wystąpi następujący błąd?

Błąd: Żądanie Azure Resource Manager nie powiodło się z błędem: "{"error":{"code":"WorkflowTriggerNotFound","message":"Nie można odnaleźć wyzwalacza "manual" przepływu pracy "e14d00f1-1fdf-4b1b-aaac-54a5064093d3". 

Wykonaj następujące kroki rozwiązywania problemów:

- Usuń połączenie usługi CDS, a następnie utwórz ponownie połączenia usługi CDS.
- Wyłączanie i włączanie przepływu podrzędnego 
- Usuń rozwiązanie, a następnie zainstaluj je ponownie. 

2.  Co należy zrobić, jeśli podczas dodawania łącznika Partner Center na platformie Power Automate Platform wystąpi błąd "Zaloguj się"?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Komunikat o błędzie wymagający zalogowania.":::

Wykonaj ten krok rozwiązywania problemów:

- Użyj swoich Partner Center, aby zalogować się do środowiska przepływu raz (flow.microsoft.com).


3. Co należy zrobić w przypadku wystąpienia następującego błędu podczas aktywowania przepływu Partner Center CRM na Power Automate Platformie?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Komunikat o błędzie wymagający aktualizacji.":::

Wykonaj następujące kroki rozwiązywania problemów:

- Aktywuj następujące dwa przepływy podrzędne przed aktywowania przepływu Partner Center do przepływu CRM.
      - Partner Center do programu CRM — pomocnik (niejawny program testów w wersji zapoznawczej)
      - Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)

4. Co należy zrobić, gdy nie możesz dodać połączeń do przepływu podczas próby edytowania przepływu?

Dodasz połączenia do przepływu, gdy przepływ jest uruchomiony, i dodasz je do każdego przepływu oddzielnie.  Jeśli okno dialogowe dodawania połączeń nie zostanie automatycznie otwarte podczas edytowania przepływu, możesz edytować poszczególne kroki i pode kroki przepływów osobno.

- Wybierz każdy przepływ i edytuj je indywidualnie.
- Rozwiń wszystkie kroki w przepływie 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kroki, które wymagają połączeń.":::

- Wybierz kroki, w których zobaczysz ikonę ostrzeżenia z prośbą o skojarzenie połączeń i dodanie połączeń. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edytuj przepływ krok po kroku.":::


5. Co należy zrobić, jeśli przepływy rozwiązania łączników poleceń do współpracy sprzedaży nie są włączane?

A. W Power Automate należy edytować przepływy w następującej kolejności i zaktualizować je, aby używać poprawnych połączeń:

- Partner Center rejestracji webhook (niejawny program testów w wersji zapoznawczej)
- Tworzenie poleceń do współpracy sprzedaży — salesforce do Partner Center (insider preview)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center do usługi Salesforce (niejawny program testów w wersji zapoznawczej)
- Salesforce to Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

 B. Dla każdego przepływu wybierz **opcję Uruchom tylko** użytkowników. Wybierz **pozycję Użyj połączenia** zamiast Dostarczone przez użytkownika tylko do **uruchamiania.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Aby aktywować przepływ.":::


C. Aktywuj wymienione poniżej przepływy:

 - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)

- Salesforce to Partner Center (Insider Preview)

    
D. Aktywuj wszystkie pozostałe przepływy.

E. W witrynie flow Partner Center webhook Registration (Rejestracja) wybierz pozycję **Run (Uruchom).** Podaj adres **URL HTTP** z pierwszej akcji w Partner Center **do przepływu usługi Salesforce.** Wybierz wszystkie cztery opcje w obszarze **Zdarzenia do zarejestrowania,** a następnie wybierz **pozycję Tak dla** opcji Zastąp.

## <a name="questions-and-answers-about-runmaintenance"></a>Pytania i odpowiedzi dotyczące uruchamiania/konserwacji

1. Jak rozwiązywać problemy z błędami podczas Power Automate przepływu pracy?

Aby upewnić się, Power Automate przepływy działają zgodnie z oczekiwaniami i rozwiązywać problemy z błędami podczas wykonywania, zobacz [Naprawianie błędów przepływu.](/power-automate/fix-flow-failures)

2. Co należy zrobić, jeśli widzisz polecenia, które nie są prawidłowo synchronizowane Partner Center środowisku CRM?
 
Aby określić stan synchronizacji od skierowań, wybierz pozycję **Przejmij inspekcję.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Jak synchronizować polecenia.":::

Upewnij się, że są spełnione następujące warunki:

- Identyfikator rozwiązania jest dostarczany w ramach szansy sprzedaży.

- Wymagany jest dwulitowy kod kraju.

- W przypadku wyboru pomocy firmy Microsoft dla szansy sprzedaży wymagane są informacje kontaktowe klienta.

3. Jak upewnić się, że polecenie będzie synchronizowane dwukierunkowo?

Wykonaj następujące czynności:

- Sprzedawcy partnerscy muszą upewnić się, że włączyli opcję **Synchronizuj z Partner Center** w sekcji CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Upewnij się, że włączono synchronizację.":::

- Sprzedawcy muszą podać przychód i datę zamknięcia podczas kwalifikowania potencjalnego klienta.

- Jeśli identyfikator CRM zostanie  podany  na etapie tworzenia lub aktualizacji szansy sprzedaży, ale szansa sprzedaży potencjalnego klienta z tym identyfikatorem nie zostanie znaleziona w programie CRM, aktualizacja lub tworzenie zostaną zignorowane.

- Upewnij się, że pole waluty polecenia jest skonfigurowane w środowisku usługi Salesforce. 

4. Co należy zrobić, jeśli łącznik zostanie odłączony i pominiesz synchronizację od skierowań?

Poniżej przedstawiono kilka opcji, które można wypróbować:

- Sprawdź, czy nazwa użytkownika lub hasło wygasły dla Partner Center z rolami administratora poleceń.

- Możesz przejść do niezsynchronizowanych szans sprzedaży, wprowadzić aktualizację pomocniczą i sprawdzić, czy polecenie zostało zsynchronizowane.

- Jeśli przepływy zostały uruchomione i zakończyły się niepowodzeniem, wybierz przepływ i prześlij ponownie przebieg, który zakończył się niepowodzeniem.

5. Co należy zrobić, gdy występują błędy odmowy dostępu?

Upewnij się, że istnieją odpowiednie role

- Rola administratora poleceń dla Partner Center sprzedawcy 
 
- Rola administratora systemu lub customizera systemu w wystąpieniu systemu CRM

- Upewnij się, Power Automate użytkownika przepływu danych loguje się https://flow.microsoft.com wcześniej co najmniej raz

6. Jeśli zobaczysz, że **brakuje** kodu kraju konta klienta podczas tworzenia możliwości współpracy sprzedaży, co należy zrobić?

Musisz dodać dwuliterowy kod kraju ISO do konta klienta w systemie CRM.

7. Co należy zrobić, jeśli zobaczysz błąd, że identyfikator rozwiązania **jest** wymagany podczas tworzenia możliwości współpracy sprzedaży?

Aby utworzyć polecenie do współpracy sprzedaży, potrzebujesz gotowego rozwiązania firmy Microsoft do współpracy. 

8. Co należy zrobić, gdy zobaczysz możliwości współpracy sprzedaży utworzone w Partner Center, które nie są zsynchronizowane z programem CRM, mimo że nie występują błędy przepływu?

Wykonaj następujące czynności:

- Po utworzeniu nowej transakcji sprzedaży w uciecie sprawdź Partner Center czy zostanie wywołany przepływ Partner Center dynamics 365 (może zostać wywołany wiele razy).

- Jeśli przepływ zostanie wywołany, sprawdź wszystkie wywołane przepływy i zidentyfikuj przebieg przepływu, który zaktualizuje system CRM. Możesz wykonać akcje i sprawdzić, czy system CRM został zaktualizowany, czy napotkał problem.

- Sprawdź **nową ofertę** w Partner Center, aby sprawdzić, czy zostanie ona wypełniona identyfikatorem CRM.

- Upewnij się, że transakcja nie została przypadkowo zamknięta jako **wygrana** lub **utracona** w Partner Center.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)
 
- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)
