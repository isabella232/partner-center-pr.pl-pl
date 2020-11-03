---
title: Rozwiązywanie problemów dotyczących współsprzedawanych łączników
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Poznaj odpowiedzi na często zadawane pytania dotyczące korzystania z łączników współsprzedawanych. Przeczytaj ten temat często zadawanych pytań dotyczących rozwiązywania problemów z łącznikami współsprzedawanymi.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530304"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Rozwiązywanie problemów dotyczących współsprzedawanych łączników

**Dotyczy:**

- Centrum partnerskie
- Dynamics 365 CRM
- Aplikacja Salesforce CRM

**Odpowiednie role**

- Administrator odwołań
- Administrator systemu lub Konfigurator systemu w programie CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Pytania i odpowiedzi dotyczące wymagań wstępnych

1. Czy można korzystać z wersji próbnej do współtworzenia łączników odwołań dla danego środowiska?

Jeśli pracujesz w środowisku testowym/przejściowym, możesz wybrać rozwiązanie próbne. Płatna wersja łączników jest dostępna w AppSource w Stanach Zjednoczonych $15 miesięcznie. Dzięki połączeniu płatnym będzie można uzyskać 10 tys. wywołań interfejsu API dziennie. Łączniki są otokami na podstawie interfejsów API odwołań Centrum partnerskiego. Za każdym razem, gdy zostaną uruchomione rozwiązania łącznika w celu **utworzenia** lub **zaktualizowania** zdarzenia dotyczącego możliwości w centrum partnerskim lub po stronie programu CRM, wykonywane jest wywołanie interfejsu API.

2. Jaką rolę należy utworzyć w środowisku programu CRM?

Użytkownicy będący administratorami systemu lub konfiguratorami systemu mogą stosować zmiany dla wszystkich użytkowników. Wszyscy użytkownicy aplikacji mogą jednak personalizować system i nawet udostępniać niektóre dostosowania innym osobom. 

3. Czy sprzedawcy w ramach partnerów potrzebują specjalnych ról do pracy w centrum partnerskim?
 
Sprzedawcy z partnerami muszą mieć przypisaną rolę "Administrator odwołań". Aby uzyskać więcej informacji, zobacz następujące [omówienie uprawnień) (Create-User-Account-and-Set-Permissions).

4. Jakie pola należy najpierw skonfigurować w środowisku programu CRM? 

• Upewnij się, że Twoja waluta jest odpowiednia dla Twojej lokalizacji i że znajduje się w środowisku programu CRM. • Zespół ds. sprzedaży powinien być wymieniony w środowisku programu CRM jako użytkownicy programu CRM.

5. Jakie wymagania wstępne są wymagane do utworzenia środowiska w celu zautomatyzowania pracy?

Aby móc korzystać ze środowiska automatyzacji, potrzebne są:

- Wymagana jest licencja na automatyzację.
- Wymagany jest co najmniej 1 GB pamięci masowej.

6.  Potrzebujesz subskrypcji usługi Dynamics 365 do korzystania z rozwiązania usługi Salesforce?

Rozwiązanie łącznika usługi Salesforce jest typu "Dynamics Flow", które obsługuje synchronizację z innymi systemami CRM. Rozwiązanie nie wymaga posiadania wystąpienia usługi Dynamics 365 lub subskrypcji. Podczas instalowania rozwiązania Salesforce może pojawić się lista rozwijana z istniejącym środowiskiem dysków CD w firmie. Musisz wybrać to środowisko. Ponadto jeśli zostanie wyświetlony komunikat o błędzie "nie można odnaleźć organizacji usługi Dynamics 365 podłączonej do zalogowanego użytkownika", należy utworzyć nowe środowisko dla łącznika.

## <a name="questions-and-answers-about-configuration"></a>Pytania i odpowiedzi dotyczące konfiguracji

1. Co należy zrobić, jeśli podczas aktywowania przepływów na platformie automatyzacji w programie zawarto następujące błędy?

Błąd: żądanie do Azure Resource Manager nie powiodło się z powodu błędu: "{" błąd ": {" Code ":" WorkflowTriggerNotFound "," Message ":" nie można odnaleźć wyzwalacza "Manual" przepływu pracy "e14d00f1-1fdf-4b1b-aaac-54a5064093d3". "}}". 

Wykonaj następujące kroki rozwiązywania problemów:

- Usuń połączenie z DYSKami CD, a następnie ponownie utwórz połączenia z DYSKami CD.
- Włączanie i wyłączanie przepływu podrzędnego 
- Usuń rozwiązanie, a następnie ponownie zainstaluj rozwiązanie. 

2.  Co należy zrobić, jeśli podczas dodawania łącznika Centrum partnerskiego na platformie automatyzacji jest zależeć błąd "Logowanie"?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Komunikat o błędzie wymagający zalogowania":::

Wykonaj ten krok rozwiązywania problemów:

- Użyj poświadczeń Centrum partnerskiego, aby zalogować się do środowiska przepływu raz (flow.microsoft.com).


3. Co należy zrobić, jeśli wystąpi następujący błąd podczas aktywowania Centrum partnerskiego do przepływu CRM w ramach platformy w automatyzowaniu?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Komunikat o błędzie wymagający zalogowania":::

Wykonaj następujące kroki rozwiązywania problemów:

- Przed aktywowaniem Centrum partnerskiego do przepływu CRM należy najpierw aktywować dwa następujące przepływy podrzędne.
      - Partner Center do CRM — pomocnik (wersja zapoznawcza)
      - Centrum partnerskie — aktualizacje odwołań towarzyszące firmie Microsoft do programu CRM (wersja zapoznawcza)

4. Co należy zrobić, jeśli nie będziesz w stanie dodać połączeń do przepływu podczas próby edytowania przepływu?

Można dodać połączenia do przepływu, gdy przepływ jest uruchomiony, i oddzielnie dodać do każdego przepływu.  Jeśli okno dialogowe dodawania połączeń nie jest automatycznie otwierane podczas edytowania przepływu, można edytować poszczególne kroki i podrzędne etapy przepływów osobno.

- Zaznacz każdy przepływ i edytuj je pojedynczo.
- Rozwiń wszystkie kroki w przepływie 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Komunikat o błędzie wymagający zalogowania":::

- Wybierz kroki, w których zostanie wyświetlona ikona ostrzeżenia z prośbą o skojarzenie połączeń i Dodawanie połączeń. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Komunikat o błędzie wymagający zalogowania":::


5. Co należy zrobić, jeśli nie można włączyć rozwiązania łączników odwołań współsprzedawanych?

A. W programie w celu zautomatyzowania należy edytować przepływy w następującej kolejności i zaktualizować je, aby korzystały z prawidłowych połączeń:

- Rejestracja elementu webhook Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Utwórz odwołanie do towarzyszącej usługi Salesforce do Centrum partnerskiego (wersja zapoznawcza programu testowego)
- Centrum partnerskie — aktualizacje referencyjne firmy Microsoft do usługi Salesforce (wersja zapoznawcza programu testowego)
- Centrum partnerskie do usługi Salesforce (wersja zapoznawcza programu testowego)
- Centrum usług Salesforce dla partnerów partnerskich (wersja zapoznawcza)
- Okazja do Centrum partnerskiego w usłudze Salesforce (wersja zapoznawcza)
- Rozwiązania firmy Microsoft do Centrum partnerskiego (wersja zapoznawcza)

 B. Dla każdego przepływu wybierz opcję **Uruchom tylko użytkownicy** . Wybierz pozycję **Użyj połączenia** zamiast **podanej przez użytkownika tylko do uruchomienia** .  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Komunikat o błędzie wymagający zalogowania":::


C. Aktywuj poniższe przepływy:

 - Centrum partnerskie — aktualizacje referencyjne firmy Microsoft do usługi Salesforce (wersja zapoznawcza programu testowego)

- Centrum usług Salesforce dla partnerów partnerskich (wersja zapoznawcza)

    
D. Aktywuj wszystkie pozostałe przepływy.

E. W obszarze Rejestracja elementu webhook Centrum partnerskiego w usłudze Flow wybierz pozycję **Uruchom** . Podaj **adres URL protokołu HTTP** od pierwszej akcji w **centrum partnerskim do** przepływu usługi Salesforce. Zaznacz wszystkie cztery opcje w obszarze **zdarzenia do zarejestrowania** i wybierz pozycję **tak** dla opcji Zastąp.

## <a name="questions-and-answers-about-runmaintenance"></a>Pytania i odpowiedzi dotyczące uruchamiania/konserwacji

1. Jak rozwiązywać problemy w przypadku awarii podczas wykonywania przepływu w ramach automatyzacji

Aby upewnić się, że przepływy Automatyzuj działają zgodnie z oczekiwaniami i rozwiązywanie problemów podczas wykonywania, zapoznaj się z tematem [usuwanie błędów przepływu](/power-automate/fix-flow-failures).

2. Co należy zrobić, Jeśli zobaczysz odwołania, które nie są prawidłowo zsynchronizowane w centrum partnerskim lub w środowisku programu CRM?
 
Aby określić stan synchronizacji odwołań, wybierz pozycję **Inspekcja** . 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Komunikat o błędzie wymagający zalogowania":::

Upewnij się, że zostały spełnione następujące warunki:

- Identyfikator rozwiązania jest dostarczany jako część szansy sprzedaży.

- Wymagany jest dwuliterowy kod kraju.

- Jeśli dla szansy sprzedaży została wybrana Pomoc firmy Microsoft, wymagane są informacje kontaktowe klienta.

3. Jak upewnić się, że odwołanie zostanie zsynchronizowane dwukierunkowo?

Wykonaj następujące czynności:

- Sprzedawcy partnerów muszą mieć pewność, że włączyli opcję **Synchronizuj z Centrum partnerskiego** w sekcji CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Komunikat o błędzie wymagający zalogowania" w centrum partnerskim.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie potencjalnymi klientami](manage-leads.md)
 
- [Manage co-sell opportunities (Zarządzanie możliwościami wspólnego sprzedawania)](manage-co-sell-opportunities.md)