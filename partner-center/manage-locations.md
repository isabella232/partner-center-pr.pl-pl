---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441335"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Zarządzanie lokalizacjami kont MPN i Dodawanie (usuwanie) lokalizacji


**Odpowiednie role**

- Administrator globalny
- Administrator konta

IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy. IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych. Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.

## <a name="the-following-scenario-is-typical"></a>Poniżej przedstawiono typowy scenariusz:

Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii. PGA jest zarejestrowaną firmą prawną, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi. Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA. W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory. PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt. Wypłaty są powiązane z określonymi lokalizacjami. 

>[!NOTE]
>Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Wymagania wstępne w celu dodania nowego konta dla firmy dostawcy CSP

Aby dodać nowe konto biznesowe dostawcy usług kryptograficznych, Zacznij od upewnienia się, że spełniono wymagania wstępne.

1. W kraju, w którym ma być prowadzone biznesowe Oprogramowanie CSP, musi znajdować się identyfikator MPN. Aby utworzyć nową lokalizację MPN, przeczytaj sekcję "Dodawanie lokalizacji MPN" poniżej.
  
1. Aby utworzyć nową dostawcę CSP pośredniego rejestracji odsprzedawcy, przeczytaj artykuł [współpraca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowego** konta dostawcy usług kryptograficznych. Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.

2. Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.

1. Jeśli chcesz zarejestrować się jako partner bezpośredniego rozliczania, zapoznaj się z [wymaganiami dotyczącymi bezpośrednich partnerów rozliczeniowych](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>Wyświetlanie lokalizacji MPN

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego przy użyciu poświadczeń konta MPN. (Poświadczenia MPN mogą się różnić od poświadczeń programu CSP) 
 
1. Na ikonie **ustawień** wybierz kolejno pozycje **Ustawienia konta**, **profil organizacji** i informacje **prawne**. 

1. Na karcie **partner** Sprawdź, czy nie jest wyświetlany komunikat o błędzie transparentu z prośbą o naprawienie zmigrowanych lokalizacji z PMC.  Jeśli lokalizacje nie zostały poprawnie skonfigurowane w kryterium PMC i nie zostały jeszcze przenoszone na komputer, musisz zaktualizować te lokalizacje.

:::image type="content" source="images/locations/location-two.png" alt-text="Zrzut ekranu przedstawiający pokazuje, jak aktualizować lokalizację.":::
 
4.  Na ekranie **Przejrzyj lokalizacje PMC** wybierz pozycję **Aktualizuj**.
Zaktualizuj następujące pola:

- **Nazwa pola**: Upewnij się, że nazwa lokalizacji firmy jest poprawna. Jeśli zostanie wyświetlony zduplikowany błąd, spróbuj zmienić z, na przykład contoso na contoso, Inc.

- **Pole podmiotu prawnego**: Upewnij się, że wybrano jednostkę prawną, z którą jest powiązana lokalizacja

- **Wiersz adresu 1 & 2 pola**: Upewnij się, że adres jest poprawny

- **Pola stanu/prowincji & miasto**: Upewnij się, że kombinacja między miastem a stanem jest poprawna. Istnieją kraje, w których zostanie zastosowane menu rozwijane służące do wybierania stanu/prowincji, a w innych krajach, w których pole będzie musiało zostać wstawione ręcznie.

- **Pole kod** pocztowy: Upewnij się, że pole kod pocztowy jest zgodne z określonym krajem, regionem, miastom lub adresem.

- **Podstawowe pola informacji kontaktowych**: Upewnij się, że pola Imię i nazwisko są wypełnione oraz że wskazany adres e-mail to służbowy adres e-mail, a nie osobisty (na przykład @outlook.com @live.com itp.).

- **Pole numeru telefonu**: Upewnij się, że numer telefonu nie zawiera znaków specjalnych, spacji ani kodu kraju. Wartość wprowadzona w polu numer telefonu zawsze będzie zawierać maksymalnie 10 znaków.

5. Jeśli nie ma komunikatu o błędzie, w obszarze  **Ustawienia** wybierz pozycję  **Ustawienia konta**, **profil organizacji**, **identyfikatory**.

6. Znajdź identyfikator MPN z typem "Location", który jest zgodny z krajem tego konta dostawcy CSP, i użyj go, aby zakończyć skojarzenie.

7. Jeśli nie możesz znaleźć MPN identyfikatora lokalizacji pasującego do konta dostawcy CSP, którego chcesz użyć, możesz dodać nową lokalizację, która utworzy nowy identyfikator MPN. Zobacz **Dodaj lokalizację MPN** poniżej.

## <a name="add-an-mpn-location"></a>Dodaj lokalizację MPN

1. Zaloguj się przy użyciu konta MPN w centrum partnerskim. (Poświadczenia MPN mogą się różnić od poświadczeń programu CSP). Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

1. Na **ikonie ustawień** wybierz **Ustawienia konta** , a następnie wybierz pozycję **profil organizacji**.

2. Wybierz pozycję **Legal** , a następnie na karcie **partner** wybierz pozycję **lokalizacje biznesowe,** a następnie kliknij pozycję **Dodaj lokalizację.**

3. Podaj wymagane szczegóły, takie jak nazwa firmy, adres i kontakt, dla lokalizacji, która ma zostać dodana do firmy.
 
1. Kliknij pozycję **Dodaj lokalizację**. Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, z której można korzystać w przypadku transakcji i zachęt dostawcy usług kryptograficznych.

:::image type="content" source="images/legal-biz.png" alt-text="Dodaj nową firmę prawną":::

> [!NOTE]
> Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć. Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.


## <a name="delete-a-location"></a>Usuwanie lokalizacji

Aby usunąć lokalizację z konta, musisz skontaktować się z [pomocą techniczną partnera](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Upewnij się, że rozumiesz wpływ tej akcji. Nie można pobrać usuniętych lokalizacji i wszystkie powiązane z tym identyfikatorem MPN nie będą już rozpoznawane ani nieaktywne dla Twojej firmy.

## <a name="change-country-of-partner-global-account"></a>Zmień kraj konta partnera globalnego 

1. Zaloguj się przy użyciu konta MPN w centrum partnerskim. (Poświadczenia MPN mogą się różnić od poświadczeń programu CSP). Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

2. Na karcie **partner** przejdź do **lokalizacji biznesowej** i sprawdź listę lokalizacji, aby upewnić się, że lokalizacja, która ma się pojawić jako podmiot prawny, jest wyświetlana. 
 
1. Aby dodać lokalizację, kliknij pozycję **Dodaj lokalizację**, a następnie w polu wylot wprowadź wymagane szczegóły, takie jak nazwa firmy, adres i kontakt podstawowy dla lokalizacji, która ma zostać dodana do firmy. 
 
1. Wybierz pozycję **Zmień kraj** obok listy rozwijanej **kraj/region** i postępuj zgodnie z instrukcjami. 

:::image type="content" source="images/lbp.png" alt-text="Brak danych profilu biznesowego firmy":::

5. Kliknij pozycję **Zapisz**.

6. Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.
  
## <a name="next-steps"></a>Następne kroki

- Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).
