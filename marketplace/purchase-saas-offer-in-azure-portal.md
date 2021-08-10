---
title: Jak kupić ofertę SaaS w Azure Portal
description: Dowiedz się, jak znaleźć i zakupić ofertę SaaS w Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: 5c5c1565f8e1f2703e82bd75881e9920a1fc71d611d78ef282f771cfb30fcd00
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688373"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Kupowanie oferty SaaS w Azure Portal

W tym artykule wyjaśniono różne opcje i wymagania dotyczące wyszukiwania, wypróbowania i kupowania oferty SaaS (oprogramowanie jako usługa) w Azure Portal.

## <a name="create-a-saas-subscription"></a>Tworzenie subskrypcji SaaS

Aby kupić subskrypcję SaaS, musisz mieć konto użytkownika platformy Azure z dostępem do odpowiedniej subskrypcji platformy Azure. Ta subskrypcja będzie używana do rozliczeń, a także do przedziałów zakupionych zasobów w chmurze. Aby dowiedzieć się więcej na temat subskrypcji platformy Azure, [zobacz Tworzenie dodatkowej subskrypcji platformy Azure.](/azure/cost-management-billing/manage/create-subscription)

W witrynie Azure Portal wybierz żądaną ofertę SaaS w sekcji **Marketplace.**

Subskrypcja oprogramowania jako usługi zapewnia prawo do korzystania z usługi przez określony czas za pośrednictwem subskrypcji online zamiast instalacji lokalnej na poszczególnych komputerach. Subskrypcja to umowa na korzystanie z co najmniej jednej platformy lub usług w chmurze, za które opłaty są naliczane na podstawie opłaty licencyjnej za użytkownika lub użycia zasobów opartych na chmurze. Organizacja może mieć wiele subskrypcji SaaS.

Ograniczenia dotyczące subskrypcji SaaS obejmują:

- Brak subskrypcji dla uczniów.
- Brak Visual Studio Enterprise subskrypcji.
- Brak bezpłatnych subskrypcji kredytowych.
- W przypadku ofert płatnych wymagany jest instrument płatniczy.

## <a name="saas-offers-discovery-in-azure-portal"></a>Usługa SaaS oferuje odnajdywanie w Azure Portal

Po zakończeniu pracy Azure Portal istnieje kilka sposobów zawężenia wyszukiwania, aby skoncentrować się na ofertach SaaS.

### <a name="narrowing-your-search"></a>Zawężanie wyszukiwania

Na stronie głównej w obszarze **Usługi platformy Azure** wybierz pozycję + Utwórz **zasób lub** pozycję **Marketplace.** Możesz też użyć **skrótu G + N w** dowolnym miejscu na platformie.

- Zawęzij wyniki do ofert SaaS przy użyciu **filtru Typ** oferty, a następnie wybierz **pozycję SaaS.**
- Użyj paska wyszukiwanie globalne w górnym obszarze nawigacji, aby znaleźć określoną ofertę SaaS.

Znajdź [prywatną ofertę SaaS,](./private-offers.md) wybierając baner w górnej części strony **głównej witryny** Marketplace. Nie wszystkie oferty lub plany są dostępne we wszystkich lokalizacjach geograficznych, a niektóre mogą być wyświetlane tylko dla niektórych dzierżaw.

Filtrowany widok przedstawia każdą dostępną ofertę SaaS reprezentowaną przez tytuł. Wybierz jedną z nich, aby wyświetlić stronę szczegółów produktu. Obejmuje to następujące sekcje:

- Przegląd — szczegółowe informacje o usłudze, materiałach marketingowych i edukacyjnych
- Plany i ceny — każda oferta będzie zawierać co najmniej jeden plan z różnymi warunkami i cenami rozliczeń
- Informacje o użyciu i pomoc techniczna — Publisher, identyfikator oferty i identyfikator planu
- Ocena i przeglądy określonej oferty SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Dostępne modele rozliczeń (plany/jednostki SKU) dla ofert SaaS

Każda oferta SaaS będzie mieć co najmniej jeden plan. Z każdą ofertą jest skojarzony model cen: stawka płaska lub za użytkownika. Każda cena planu to opłata cykliczna, która może być równa zero dolarów (wszystkie wymienione ceny są przeznaczone wyłącznie do celów i nie mają odzwierciedlać rzeczywistych kosztów). Ta opłata to stawka płaska lub cena za użytkownika. Dostępne typy planów:

- **Plany miesięczne** — cykliczna opłata miesięczna; opłata płaska lub miesięczna za użytkownika, która jest opłacana w cyklu miesięcznym. Po zakończeniu okresu plan zostanie odnowiony automatycznie.
- **Plany roczne** — cykliczna opłata roczna; opłata roczna za użytkownika, która jest opłacana w cyklu rocznym. Po zakończeniu okresu plan zostanie odnowiony automatycznie.
- **Mierniki** niestandardowe — wraz z opłatami cyklicznmi plan stawki stałej może również obejmować opcjonalne niestandardowe mierzone wymiary użycia opłat za użycie usług nieujmowane w stawce stałej. Każdy wymiar reprezentuje rozliczaną jednostkę. Jest to zmienny koszt, który zmienia się w zależności od użycia jednostek mierzonych, takich jak: przepustowość, bilety lub przetworzone wiadomości e-mail. Opłata zostanie naliczona zgodnie z zużyciem tych wymiarów co miesiąc. Należy pamiętać, że zużycie nadgorętowe rozpoczyna się tylko w przypadku użycia wszystkich jednostek mierzonych uwzględnionych w stawce zryczałtowej.
- **Bezpłatna** wersja próbna — w niektórych przypadkach plan obejmuje miesięczny okres próbny, w którym można bezpłatnie korzystać z oprogramowania.  Po zakończeniu okresu próbnego opłata zostanie naliczona zgodnie z planem. Oferty wersji próbnej nie są zgodne z miernikami niestandardowymi.

Te modele cenowe są dostępne zarówno dla planów publicznych, jak i prywatnych.

## <a name="saas-purchase-experience"></a>Środowisko zakupu saaS

1. Na stronie produktu wybierz plan spełniający Twoje potrzeby i kontynuuj konfigurowanie **+ subskrybowanie**
2. W ramach procesu zakupu nastąpi przekierowanie do karty  Podstawowe informacje i wymagane będzie:
    1. *Zdefiniuj subskrypcję,* której chcesz użyć do rozliczeń. Subskrypcja platformy Azure, która jest w użyciu, powinna mieć zdefiniowaną prawidłową metodę zakupu. Musisz mieć odpowiedni poziom uprawnień lub grupę zasobów w ramach tej subskrypcji z odpowiednim poziomem uprawnień. Ponadto kraj rozliczeniowy powinien być tym, w którym oferta jest dostępna do zakupu. Subskrypcji platformy Azure bez ważnej formy płatności (na przykład subskrypcji MSDN) można używać tylko do zakupu bezpłatnych planów
    1. Wybierz lub utwórz **grupę zasobów,* do której będzie należeć zasób SaaS.
    1. Wpisz nazwę *subskrypcji* SaaS, aby łatwo ją później zidentyfikować. Po zakupie nie można zmienić nazwy.
    1. W **obszarze** Plan zobaczysz wybrany plan na stronie szczegółowej produktu (PDP). Jeśli nie dokonano aktywnego wyboru w pdp, zostanie wyświetlony plan domyślny. Możesz zmienić wybór, wybierając link **Zmień plan.** Wybierz odpowiedni okres rozliczeniowy, a następnie wybierz inny plan. Możesz zmienić plan po zakupie, jeśli wydawca go obsługuje. Nie będzie można jednak zmienić okresu z miesięcznego na roczny ani z rocznego na miesięczny.
    1. W przypadkach, gdy model cenowy jest *określony dla użytkownika,* może być konieczne określenie liczby *użytkowników*. Cena, która zostanie wyświetlony, zmieni się w zależności od wybranej subskrypcji, planu i okresu.
3. Przejdź do **karty Tagi** — *tagi to* zdefiniowane przez użytkownika pary klucz/wartość, które można umieścić bezpośrednio w zasobie lub grupie zasobów. Tagów możesz użyć, aby później łatwo znaleźć zasób SaaS. Platforma Azure obsługuje obecnie maksymalnie 50 tagów na zasób i grupę zasobów. Tagi mogą być umieszczane w zasobie w czasie tworzenia lub dodawane do istniejącego zasobu.
4. Przejdź do **tematu Przeglądanie + subskrybowanie,** aby zapoznać się ze szczegółami oferty i planu.
    1. Zapoznaj *Warunki użytkowania,* *poprawkami* i *zasadami* ochrony prywatności wydawcy, a także ich Azure Marketplace
    1. Może pojawić się monit o dodanie danych kontaktowych
    1. Przejrzyj *podstawowe informacje i* szczegóły *tagów*
5. Po potwierdzeniu wybierz pozycję **Subskrybuj**.

## <a name="saas-subscription-and-configuration"></a>Subskrypcja i konfiguracja saaS

Po wybraniu opcji subskrybowania zostanie wyświetlony komunikat "Twoja subskrypcja SaaS jest w toku". Ten proces powinien potrwać kilka minut. Nie zamykaj okna, dopóki nie zostanie zakończone.

Po zakończeniu subskrypcji zostanie wyświetlony komunikat informujący o zakończeniu subskrypcji SaaS. Należy skonfigurować konto, aby rozpocząć zakup. Otrzymasz również wiadomość e-mail z prośbą o aktywowanie nowej subskrypcji. Jeśli nie jesteś osobą, która skonfiguruje konto SaaS, przekaż tę wiadomość e-mail do odpowiedniej osoby.

Aby ukończyć ten proces i rozpocząć korzystanie z modelu SaaS, musisz rozpocząć konfigurowanie subskrypcji. Wybranie **przycisku Konfiguruj teraz konto** spowoduje przekierowanie do witryny internetowej wydawcy.

Możesz również sprawdzić stan subskrypcji, wybierając ikonę "dzwonka" w prawym górnym rogu nagłówka.

Jeśli nie ukończysz procesu konfiguracji w ciągu *30* dni, ta subskrypcja SaaS zostanie automatycznie *usunięta.* Rozliczenia będą rozpoczynane po skonfigurowaniu konta w witrynie internetowej wydawcy.

Komunikaty o błędach, które mogą wystąpić podczas tego procesu:

- Nie można *kupić nazwy wybranego planu* w ramach bezpłatnej subskrypcji
  - Uaktualnij swoje konto. https://aka.ms/UpgradeFreeSub Aby uzyskać więcej informacji, zobacz .

- Zakup nie powiódł się, ponieważ nie można odnaleźć prawidłowej karty kredytowej ani formy płatności skojarzonej z subskrypcją platformy Azure.
  - Użyj innej subskrypcji platformy Azure lub dodaj/zaktualizuj bieżącą kartę kredytową lub formę płatności dla tej subskrypcji i spróbuj ponownie.

- Nazwa *planu wybranego dla oferty* nazwa  oferty według wydawcy oferty nie jest dostępna do zakupu zgodnie z regułami ustawionymi przez administratora IT. 
  - Skontaktuj się z administratorem IT.

- Nazwa *planu wybranego przez* wydawcę  oferty wybranego przez wydawcę oferty nie jest dostępna do zakupu ze względu na ustawienia prywatnej platformy handlowej wprowadzone przez administratora IT twojej dzierżawy. 
  - Skontaktuj się z administratorem IT

- Zakup nie powiódł się, ponieważ żądany okres rozliczeniowy jest pusty lub nieprawidłowy.
  - Spróbuj kupić inny plan/okres rozliczeniowy.

- Zakup nie powiódł się, ponieważ nie można zweryfikować logowania w umowie prawnej.
  - Ponów próbę. Jeśli błąd będzie się powtarzać, spróbuj dokonać zakupu przy użyciu innej subskrypcji platformy Azure lub skontaktuj się z pomocą techniczną.

- Zakup oferty *offerID według* *wydawcy publisherID* nie powiódł się. Ta oferta nie jest obecnie dostępna do zakupu.
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

- Jeśli już zakupiono ofertę na platformie handlowej, przejdź do [tematu Rozliczenia i fakturowanie](./billing-invoicing.md)
- Możesz również dowiedzieć się więcej o [opcjach planów prywatnych.](./private-offers.md)