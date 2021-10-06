---
title: Sprzedaż oprogramowania lokalnego za pośrednictwem programu CSP
ms.topic: how-to
ms.date: 03/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak partnerzy w programie CSP mogą kupować, sprzedawać i anulować lokalne subskrypcje oprogramowania oraz zarządzać nimi w imieniu klientów w Partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f58f120d376b98f9fa054f0bec87f324874ce0bb
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129584902"
---
# <a name="sell-on-premises-software-through-the-cloud-solution-provider-csp-program"></a>Sprzedaż oprogramowania lokalnego za pośrednictwem programu Dostawca rozwiązań w chmurze (CSP)

**Odpowiednie role:** Agent administracyjny | Administrator globalny

Oprogramowanie lokalne w programie CSP obsługuje bezproblemowe przejście do chmury przez wprowadzenie oprogramowania lokalnego w programie skoncentrowanym na chmurze. Ta nowa oferta ułatwia dodanie partnera o wartości dodanej do każdego scenariusza zakupu, ponieważ zapewnia jedną platformę do transakcji wszystkich produktów firmy Microsoft. Jako CSP możesz teraz sprzedawać oprogramowanie lokalne za pośrednictwem usługi Partner Center jako dodatek do programów Open, EA i innych, które są obecnie w użyciu.  
 
Zapewniając najlepszą ogólną wartość klienta przy użyciu opcji licencjonowania oprogramowania lokalnego, model biznesowy został również tak przyjazny dla partnerów, jak to możliwe. Proste licencjonowanie oprogramowania lokalnego w programie CSP oznacza przewidywalność kosztów i usprawniony proces sprzedaży. Ten nowy model biznesowy ułatwia nabywanie i wycenę lokalnego oprogramowania oraz zarządzanie nim, co pozwala skoncentrować się na zdobyciu korzyści biznesowych dzięki rozbudowanym portfolio rozwiązań do zarządzania zasobami IT o wartości dodanej.

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Kupowanie subskrypcji oprogramowania w imieniu klientów

Aby kupić subskrypcje oprogramowania w imieniu klienta, przejdź do strony szczegółów klienta, wybierz pozycję Dodaj produkty, a następnie postępuj zgodnie z wyświetlanymi instrukcjami, aby utworzyć zamówienie i zapłacić za nie.

> [!NOTE]
> Aby uzyskać więcej informacji, zobacz ten [przewodnik dotyczący zamawiania i](https://partner.microsoft.com/resources/detail/guide-to-ordering-and-fulfillment-through-partner-center-pdf)realizacji za pośrednictwem Partner Center .

## <a name="activate-and-manage-software-subscriptions"></a>Aktywowanie subskrypcji oprogramowania i zarządzanie nimi

Po zakupie oprogramowania Ty lub Twoi klienci muszą je pobrać (partnerzy korzystający z usługi Partner Center; klienci korzystający z centrum Administracja Microsoft 365). Użyj poniższej procedury w tym celu. Ważne jest, aby zrozumieć czynniki ryzyka związane z kopiowaniem linków i pobieraniem oprogramowania. Aby uzyskać więcej informacji, zobacz Używanie usługi **Partner Center** do pobierania oprogramowania klienta i kluczy licencji w [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).

> [!NOTE]
> Musisz być agentem administratora w Partner Center, aby uzyskać link do kluczy i plików do pobrania.

1. Przejdź do strony szczegółów klienta, a następnie wybierz pozycję **Oprogramowanie**. Zostanie wyświetlona lista wszystkich programów zakupionych w imieniu klienta.

2. Wybierz wersję **produktu,** **język,** **bit** i wybierz pozycję **Pobierz klucze i pliki do pobrania.** 

3. Wybierz **pozycję Pobierz klucz,** aby wyświetlić 32-cyfrowy produkt w oknie podręcznym, które można skopiować i wysłać do klienta. 

4. Wybierz **pozycję Pobierz,** aby pobrać bity. 

5. Wybierz **pozycję Kopiuj link,** jeśli chcesz wysłać klientowi link do pobierania bitów. 

6. Możesz również **anulować** zamówienie na oprogramowanie i otrzymać 100% środków (jeśli zostanie to zrobione w ciągu 60-dniowego okresu zasad anulowania).

> [!NOTE]
> Tylko klienci mają dostęp do uzyskiwania dostępu do kluczy produktów i pobierania informacji w centrum Administracja Microsoft 365 (wymagana jest rola administratora globalnego). Partnerzy muszą użyć Partner Center, aby wyświetlić te informacje.

> [!NOTE]
> Zakupy w ramach programu CSP są aktywowane za pośrednictwem klucza aktywacji wielokrotnej (MAK). usługa zarządzania kluczami (KMS) są niedozwolone, nawet na żądanie. 

## <a name="move-a-customers-on-premises-license-from-vl-to-csp-with-no-downtime"></a>Przenoszenie licencji lokalnej klienta z licencjonowania zbiorowego do CSP bez przestojów

Mimo że KMS kluczy nie są dostępne w programie CSP, nadal możesz przenieść licencje lokalne klienta z licencjonowania zbiorowego do CSP i zapobiec przestojom spowodowanym przez przełączenie kanału zakupu. KMS dystrybuuje licencje do klientów i zazwyczaj pozostają aktywne przez 180 dni, zanim urządzenie spróbuje odnowić aktywację. Oznacza to, że urządzenie zostanie już aktywowane i będzie działać przez pewien czas, zanim pojawią się jakiekolwiek problemy. 

Jeśli klient wdroży nowy kod MAK w tym czasie ręcznie lub w sposób skryptowy (przy użyciu polecenia ), nie `slmgr.vbs` wystąpi przestój. Jeśli klient nie wdroży nowego zestawu MAK w tym czasie i spróbuje odnowić licencję później, urządzenie może zostać ograniczone lub zablokowane w niektórych funkcjach do momentu ponownego aktywowania. 

Aby uzyskać więcej informacji, przejdź do [tematu Activate clients running Windows 10 (Windows 10) - Windows Deployment](/windows/deployment/volume-activation/activate-windows-10-clients-vamt#key-management-service-activation-renewal)(Aktywowanie klientów z systemem Windows 10 ) — Windows Deployment . Aby uzyskać pomoc w zakresie tego typu wdrożenia, możesz przesłać żądanie technicznych usług [przedsprzedażowych i wdrożeniowych.](/partner-center/technical-benefits#submit-a-technical-presales-and-deployment-services-request)

## <a name="cancel-a-purchase"></a>Anulowanie zakupu

Aby anulować zakup, użyj poniższej procedury. Po zakończeniu anulowania klucz oprogramowania zostanie odwołany.

> [!NOTE]
> Aby anulować zakup, musisz być agentem administratora. 

1.  Przed rozpoczęciem procesu upewnij się, że masz następujące elementy: 
    - Identyfikator GUID dzierżawy klienta lub nazwa domeny
    - Identyfikator zamówienia lub subskrypcji
    - Przyczyna zwrotu pieniędzy
    - Żądana kwota

2.  Na stronie szczegółów klienta wybierz pozycję **Oprogramowanie**. Zostanie wyświetlona lista wszystkich zakupionych programów. 

3.  Znajdź oprogramowanie, które chcesz anulować, a następnie wybierz pozycję **Anuluj.** Zostanie **otwarta strona Zgłoś problem Partner Center** aplikacji. 

4.  W **obszarze** Szczegóły na **liście Typ problemu** wybierz pozycję **CSP Purchase/Refund on behalf of customers (Zakup/zwrot w imieniu klientów).**

5.  Wypełnij pola  Wpływ **i** Tytuł. 

6.  W **polu** Opis podaj następujące informacje: 
    -   Identyfikator GUID dzierżawy klienta lub nazwa domeny
    -   Identyfikator zamówienia lub subskrypcji
    -   Przyczyna zwrotu pieniędzy
    -   Żądana kwota

7.  W polu **Kontakt** wprowadź swoje imię i nazwisko, adres e-mail i numer telefonu. 

8.  Jeśli z jakiegoś powodu musisz dołączyć plik, wybierz **pozycję Dodaj pliki.** Ta czynność jest opcjonalna. 

9.  Po zakończeniu wybierz pozycję **Prześlij.**
