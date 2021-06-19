---
title: Jak kupić ofertę SaaS w Azure Portal
description: Dowiedz się, jak znaleźć i zakupić ofertę SaaS w Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: b73a9acb7b9cf9eee1151de1f8e45f6fd6ef256f
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373493"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Kupowanie oferty SaaS w Azure Portal

W tym artykule wyjaśniono różne opcje i wymagania dotyczące wyszukiwania, wypróbowania i kupowania oferty SaaS (oprogramowanie jako usługa) z Azure Portal.

## <a name="saas-offers-discovery-in-azure-portal"></a>Usługa SaaS oferuje odnajdywanie w Azure Portal

Po zakończeniu pracy Azure Portal istnieje kilka sposobów zawężenia wyszukiwania w celu skoncentrowania się na ofertach SaaS.

### <a name="narrowing-your-search"></a>Zawężanie wyszukiwania

Na stronie głównej w obszarze Usługi platformy  **Azure** wybierz pozycję + Utwórz **zasób lub Marketplace.** Możesz też użyć **skrótu G + N w** dowolnym miejscu na platformie.

- Zawęzij wyniki do ofert SaaS przy użyciu **filtru Typ** oferty, a następnie wybierz **pozycję SaaS.**
- Użyj paska wyszukiwanie globalne w górnym obszarze nawigacji, aby znaleźć określoną ofertę SaaS.

Znajdź [prywatną ofertę SaaS,](/marketplace/private-offers) wybierając baner w górnej części strony **głównej witryny** Marketplace. Nie wszystkie oferty lub plany są dostępne we wszystkich lokalizacjach geograficznych, a niektóre mogą być wyświetlane tylko dla określonych dzierżaw.

Filtrowany widok przedstawia każdą dostępną ofertę SaaS reprezentowaną przez tytuł. Wybierz jedną z nich, aby wyświetlić stronę szczegółów produktu. Obejmuje to następujące sekcje:

- Omówienie — szczegółowe informacje o usłudze, marketingu i materiałach edukacyjnych
- Plany i ceny — każda oferta będzie zawierać co najmniej jeden plan z różnymi warunkami i cenami rozliczeń
- Informacje o użyciu i pomoc techniczna — obejmuje identyfikator wydawcy, identyfikator oferty i identyfikator planu
- Ocena i przeglądy określonej oferty SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Dostępne modele rozliczeń (plany/jednostki SKU) dla ofert SaaS

Każda oferta SaaS będzie mieć co najmniej jeden plan. Z każdą ofertą jest skojarzony model cen: stawka płaska lub za użytkownika. Każda cena planu to opłata cykliczna, która może być równa zero dolarów (wszystkie wymienione ceny są przeznaczone tylko do celów i nie mają odzwierciedlać rzeczywistych kosztów). Ta opłata jest stawką zryczałtową lub ceną za użytkownika. Dostępne typy planów:

- **Plany miesięczne** — cykliczna opłata miesięczna; opłata płaska lub miesięczna za użytkownika, która jest opłacana w cyklu miesięcznym. Po zakończeniu okresu plan zostanie odnawiany automatycznie.
- **Plany roczne** — cykliczna opłata roczna; opłata płaska lub roczna opłata za użytkownika, która jest opłacana w cyklu rocznym. Po zakończeniu okresu plan zostanie odnawiany automatycznie.
- **Mierniki** niestandardowe — wraz z opłatami cyklicznmi plan stawki stałej może również obejmować opcjonalne niestandardowe mierzone wymiary dla użycia opłat za użycie zasobów, które nie jest uwzględnione w stawce stałej. Każdy wymiar reprezentuje rozliczaną jednostkę. Jest to zmienny koszt, który zmienia się w zależności od użycia jednostek mierzonych, takich jak: przepustowość, bilety lub przetworzone wiadomości e-mail. Opłata zostanie naliczona zgodnie z zużyciem tych wymiarów co miesiąc. Należy pamiętać, że zużycie nadgorętowe zaczyna się tylko wtedy, gdy zostały użyte wszystkie mierzone jednostki uwzględnione w stawce zryczałtowej.
- **Bezpłatna** wersja próbna — w niektórych przypadkach plan obejmuje miesięczny okres próbny, w którym można bezpłatnie korzystać z oprogramowania.  Po zakończeniu okresu próbnego opłata zostanie naliczona zgodnie z planem. Oferty wersji próbnej nie są zgodne z miernikami niestandardowymi.

Te modele cenowe są dostępne zarówno dla planów publicznych, jak i prywatnych.

## <a name="saas-purchase-experience"></a>Środowisko zakupu saaS

1. Na stronie produktu wybierz plan spełniający Twoje potrzeby i kontynuuj konfigurowanie **+ subskrybowanie**
2. W ramach procesu zakupu nastąpi przekierowanie do karty  Podstawy i wymagane będzie:
    1. *Zdefiniuj subskrypcję,* której chcesz użyć do rozliczeń. Subskrypcja platformy Azure powinna mieć zdefiniowaną prawidłową metodę zakupu. Musisz mieć odpowiedni poziom uprawnień lub grupę zasobów w ramach tej subskrypcji z odpowiednim poziomem uprawnień. Ponadto kraj rozliczeniowy powinien być kraju, w którym oferta jest dostępna do zakupu. Subskrypcje platformy Azure bez ważnej formy płatności (na przykład subskrypcji MSDN) mogą być używane tylko do zakupu bezpłatnych planów
    1. Wybierz lub utwórz **grupę zasobów,* do której będzie należeć zasób SaaS.
    1. Wpisz nazwę *subskrypcji* SaaS, aby łatwo ją później zidentyfikować. Po zakupie nie można zmienić nazwy.
    1. W **obszarze** Plan zobaczysz wybrany plan na stronie szczegółów produktu (PDP). Jeśli w pliku PDP nie dokonano aktywnego wyboru, zostanie wyświetlony plan domyślny. Możesz zmienić wybór, wybierając link **Zmień plan.** Wybierz odpowiedni okres rozliczeniowy, a następnie wybierz inny plan. Możesz zmienić plan po zakupie, jeśli wydawca go obsługuje. Nie będzie można jednak zmienić okresu z miesięcznego na roczny ani z rocznego na miesięczny.
    1. W przypadkach, gdy model cenowy jest określony dla *użytkownika,* może być konieczne określenie liczby *użytkowników*. Zobaczysz, że cena zmieni się w zależności od wybranej subskrypcji, planu i okresu.
3. Przejdź do **karty Tagi** — *tagi* są zdefiniowanymi przez użytkownika parami klucz/wartość, które można umieścić bezpośrednio w zasobie lub grupie zasobów. Tagi mogą być używane do późniejszego łatwego znalezienia zasobu SaaS. Platforma Azure obsługuje obecnie maksymalnie 50 tagów na zasób i grupę zasobów. Tagi mogą być umieszczane w zasobie w czasie tworzenia lub dodawane do istniejącego zasobu.
4. Przejdź do **tematu Przeglądanie + subskrybowanie,** aby zapoznać się ze szczegółami oferty i planu.
    1. Przejrzyj *Warunki użytkowania,* *poprawki* i *zasady* ochrony prywatności wydawcy, a także ich Azure Marketplace
    1. Może pojawić się prośba o dodanie danych kontaktowych
    1. Zapoznaj *się ze szczegółami* *podstawowych i tagów*
5. Po potwierdzeniu wybierz pozycję **Subskrybuj**.

## <a name="saas-subscription-and-configuration"></a>Subskrypcja i konfiguracja SaaS

Po wybraniu opcji subskrybowania zostanie wyświetlony komunikat "Twoja subskrypcja SaaS jest w toku". Ten proces powinien potrwać kilka minut. Nie zamykaj okna, dopóki nie zostanie zakończone.

Po zakończeniu subskrypcji zostanie wyświetlony komunikat informujący o ukończeniu subskrypcji SaaS. Należy skonfigurować konto, aby rozpocząć zakup. Otrzymasz również wiadomość e-mail z prośbą o aktywowanie nowej subskrypcji. Jeśli nie jesteś osobą, która skonfiguruje konto SaaS, przekaż tę wiadomość e-mail do odpowiedniej osoby.

Aby ukończyć ten proces i rozpocząć korzystanie z modelu SaaS, musisz rozpocząć konfigurowanie subskrypcji. Wybranie **przycisku Konfiguruj teraz konto** spowoduje przekierowanie do witryny internetowej wydawcy.

Możesz również sprawdzić stan subskrypcji, wybierając ikonę "dzwonka" w prawym górnym rogu nagłówka.

Jeśli nie ukończysz procesu konfiguracji w ciągu *30* dni, ta subskrypcja SaaS zostanie automatycznie *usunięta.* Rozliczenia będą rozpoczynać się po skonfigurowaniu konta w witrynie internetowej wydawcy.

Komunikaty o błędach, które mogą wystąpić podczas tego procesu:

- Nie można *kupić nazwy wybranego planu* w ramach bezpłatnej subskrypcji
  - Uaktualnij swoje konto. Aby https://aka.ms/UpgradeFreeSub uzyskać więcej informacji, zobacz .

- Zakup nie powiódł się, ponieważ nie można odnaleźć prawidłowej karty kredytowej ani formy płatności skojarzonej z Subskrypcją platformy Azure.
  - Użyj innej subskrypcji platformy Azure lub dodaj\zaktualizuj bieżącą kartę kredytową lub formę płatności dla tej subskrypcji i spróbuj ponownie.

- Nazwa *planu wybranej oferty według* wydawcy oferty nie jest dostępna do zakupu zgodnie z regułami ustawionymi przez administratora IT.  
  - Skontaktuj się z administratorem IT.

- Nazwa *planu wybranego przez* wydawcę  oferty nie jest dostępna do zakupu ze względu na ustawienia prywatnej platformy handlowej wprowadzone przez administratora IT twojej dzierżawy. 
  - Skontaktuj się z administratorem IT

- Zakup nie powiódł się, ponieważ żądany okres rozliczeniowy jest pusty lub nieprawidłowy.
  - Spróbuj kupić inny plan/okres rozliczeniowy.

- Zakup nie powiódł się, ponieważ nie można zweryfikować logowania w umowie prawnej.
  - Ponów próbę. Jeśli błąd będzie się powtarzać, spróbuj dokonać zakupu przy użyciu innej subskrypcji platformy Azure lub skontaktuj się z pomocą techniczną.

- Zakup *offerID według wydawcy* *publisherID* nie powiódł się. Ta oferta nie jest obecnie dostępna do zakupu.
  - Spróbuj ponownie później. Jeśli po godzinie ten komunikat o błędzie będzie nadal wyświetlany, skontaktuj się z pomocą techniczną.  

- Zakup planu *planID oferty* *offerID* według *wydawcy publisherID* nie powiódł się. Ten plan nie jest obecnie dostępny do zakupu.
  - Spróbuj ponownie później. Jeśli po godzinie ten komunikat o błędzie będzie nadal wyświetlany, skontaktuj się z pomocą techniczną. 

- Adres *e-mail klienta* o identyfikatorze *obiektu ObjectID* nie ma autoryzacji do wykonania akcji *DeploymentValidationAction* w zakresie *ResourceGroup; DeploymentScope* lub zakres jest nieprawidłowy.  
  - Ten komunikat zostanie wyświetlony, jeśli nie masz odpowiednich uprawnień do subskrypcji/grupy zasobów platformy Azure.  
    Jeśli niedawno udzielono dostępu, odśwież swoje poświadczenia.  
    Aby wdrożyć zasoby w grupie zasobów, musisz mieć co najmniej dostęp współautora. Sprawdź stan dostępu w obszarze **Grupy zasobów,** a **następnie** Access Control . To pokazuje, kim jest "Właściciel", którego możesz poprosić o przypisanie Cię jako "współautora".

- Subskrypcja używana do tego zakupu nie zezwala na zakupy w witrynie Marketplace.  
  - Użyj innej subskrypcji lub poproś administratora o zmianę definicji tej subskrypcji i ponów próbę.

## <a name="next-steps"></a>Następne kroki

- Jeśli sprzedajesz swoją ofertę za pośrednictwem firmy Microsoft, przejdź do tematu Jak dodać odbiorców wersji zapoznawczej oferty [SaaS.](/azure/marketplace/create-new-saas-offer-preview)
- W przeciwnym razie przejdź do [tematu Jak sprzedawać ofertę SaaS.](/azure/marketplace/create-new-saas-offer-marketing)
