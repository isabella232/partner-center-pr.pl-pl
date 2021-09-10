---
title: Zarządzanie lokalizacjami na koncie partnera
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-membership
description: Dowiedz się, jak dodać nową lokalizację i jak identyfikator MPN lokalizacji jest używany w programach zachęt, firmach CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66ca3a24a810f61eae9feece5e64440fa531cda5
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957910"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Zarządzanie lokalizacjami konta MPN i dodawanie (usuwanie) lokalizacji


**Odpowiednie role:** Administrator globalny | Administrator konta

Identyfikator MPN lokalizacji identyfikuje każdą określoną lokalizację firmy. Identyfikator MPN lokalizacji umożliwia rejestrację w programach zachęt, transakcje Dostawca rozwiązań w chmurze (CSP) i inne transakcje biznesowe. Globalny identyfikator MPN jest używany w przypadku działań nie transakcyjnych, takich jak żądania pomocy technicznej.

## <a name="the-following-scenario-is-typical"></a>Typowy jest następujący scenariusz:

Firma Contoso ma swoje globalne konto partnera (PGA) w Zjednoczonym Królestwie. PgA to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania całą działalnością nie transakcyjną. Firma Contoso ma również konta lokalizacji partnera (PLA) równoważne przedstawicielsjom lub oddziałom w innej lokalizacji w Zjednoczonym Królestwie, Francji i Stanach Zjednoczonych. W strukturze konta MPN te plasy są reprezentowane jako unikatowe identyfikatory MPN lokalizacji. Plas są używane dla transakcji biznesowych, takich jak CSP lub programy zachęt. Wypłaty są powiązane z określonymi lokalizacjami. 

>[!NOTE]
>Istnieje relacja 1–1 między dzierżawą CSP i identyfikatorem lokalizacji MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Wymagania wstępne dotyczące dodawania nowego konta dla dostawcy usług kryptograficznych

Aby dodać nowe konto biznesowe programu CSP, rozpocznij od upewniania się, że spełniliśmy wymagania wstępne.

1. Musisz mieć identyfikator MPN lokalizacji w kraju, w którym chcesz wykonać działalność w programie CSP. Aby utworzyć nową lokalizację MPN, przeczytaj "Dodaj lokalizację MPN" poniżej.
  
1. Aby utworzyć nową rejestrację CSP Indirect Reseller, przeczytaj [temat Praca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Pamiętaj, aby zalogować się **przy użyciu nowych** poświadczeń dla nowego **konta** CSP. Nie używaj istniejących poświadczeń, ponieważ Partner Center rozpozna, że masz już konto.

2. Zaakceptuj Microsoft Partner Agreement i aktywuj konto.

1. Jeśli chcesz zarejestrować się jako partner z rozliczeniami bezpośrednimi, przeczytaj [wymagania dotyczące partnerów rozliczanych bezpośrednio](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Wyświetlanie i aktualizowanie lokalizacji MPN

1. Zaloguj się na Partner Center [nawigacyjnym przy](https://partner.microsoft.com/dashboard/home) użyciu poświadczeń konta MPN. (Poświadczenia MPN mogą różnić się od poświadczeń CSP) 
 
1. Z **ikony Ustawienia** wybierz pozycję **Ustawienia konta,** **Profil organizacji,** **Prawne.** 

1. Na karcie **Partner** sprawdź, czy nie ma komunikatu o błędzie baneru z prośbą o naprawienie zmigrowanych lokalizacji z centrum PMC.  Jeśli lokalizacje nie zostały poprawnie skonfigurowane w programie PMC i nie zostały jeszcze przejść na komputer, należy zaktualizować te lokalizacje.

:::image type="content" source="images/locations/location-two.png" alt-text="Zrzut ekranu przedstawia sposób aktualizowania lokalizacji.":::
 
4.  Na **ekranie Review PMC locations (Przejrzyj lokalizacje PMC)** wybierz pozycję **Update (Aktualizuj).**
Zaktualizuj następujące pola:

- **Pole Nazwa:** upewnij się, że nazwa lokalizacji firmy jest poprawna. Jeśli zostanie wyświetlony zduplikowany błąd, spróbuj zmienić adres, na przykład Contoso na Contoso, Inc.

- **Pole Jednostka prawna:** upewnij się, że wybrano jednostkę prawna, z którym jest powiązana lokalizacja

- **Wiersz adresu 1 & 2 pola:** upewnij się, że adres jest poprawny

- **Miasto & pola Stan/Prowincja:** upewnij się, że kombinacja miasta i województwa jest poprawna. Istnieją kraje, w których będzie stosowane menu rozwijane służące do wybierania województwa, a w innych krajach należy ręcznie wstawić pole.

- **Zip/Postal code field (Kod** pocztowy): upewnij się, że pole Kod pocztowy jest zgodne ze wskazanym polem Country (Kraj), Region (Region), City (Miasto) lub Address (Adres).

- **Pola** podstawowych informacji kontaktowych: upewnij się, że wypełnione są pola imienia i nazwiska oraz że wskazany adres e-mail jest służbowym adresem e-mail, a nie osobistym (na przykład @outlook.com @live.com , itp.)

- **Telefon numer:** upewnij się, że Telefon nie zawiera znaków specjalnych, spacji ani kodu kraju. Wartość wprowadzona w polu Telefon Number zawsze będzie zawierać maksymalnie 10 znaków.

5. Jeśli nie ma komunikatu o błędzie, z Ustawienia **wybierz** pozycję Konto **Ustawienia,** **Profil organizacji,** **Identyfikatory**.

6. Znajdź identyfikator MPN z typem "Location" (Lokalizacja), który pasuje do kraju tego konta CSP, i użyj go do ukończenia skojarzenia.

7. Jeśli nie możesz znaleźć identyfikatora MPN lokalizacji, który odpowiada kontu CSP, którego chcesz użyć, możesz dodać nową lokalizację, co spowoduje utworzenie nowego identyfikatora MPN. Zobacz **Dodawanie lokalizacji MPN** poniżej.

## <a name="add-an-mpn-location"></a>Dodawanie lokalizacji MPN

1. Zaloguj się przy użyciu konta MPN w Partner Center. (Poświadczenia MPN mogą różnić się od poświadczeń CSP). Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

1. Z **ikony Ustawienia wybierz** pozycję **Ustawienia konta,** a następnie wybierz **pozycję Profil organizacji.**

2. Wybierz **pozycję Prawne,** a następnie na **karcie Partner** wybierz pozycję **Lokalizacje biznesowe i** wybierz pozycję Dodaj **lokalizację.**

3. Podaj wymagane szczegóły, w tym nazwę firmy, adres i kontakt dla lokalizacji, którą chcesz dodać do firmy.
 
1. Wybierz **pozycję Dodaj lokalizację**. Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, za pomocą których można korzystać z transakcji i zachęt CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Dodaj nową firmę z branży prawnej.":::

> [!NOTE]
> Po dodaniu lokalizacji w Partner Center nie można jej usunąć. Jeśli do logowania używasz poprawnego identyfikatora **MPN,** w menu po lewej Partner Center zostanie wyświetlony identyfikator MPN.

## <a name="add-the-registration-number-id"></a>Dodawanie identyfikatora numeru rejestracji

Jeśli jesteś dostawcą pośrednim, partnerem rozliczania bezpośredniego lub odsprzedawcą pośrednim i współpracujesz z nowymi lub istniejącymi klientami w następujących krajach, musisz podać numery identyfikatorów rejestracji dla swojej firmy. Jeśli kraj, w którym prowadzenia działalności biznesowej, nie jest wymieniony poniżej, identyfikator rejestracji jest opcjonalny.

- Armenia 
- Azerbejdżan 
- Białoruś 
- Brazylia 
- Węgry 
- Indie 
- Irak 
- Kazachstan 
- Kirgistan 
- Mołdawia 
- Myanmar 
- Polska 
- Rosja 
- Arabia Saudyjska 
- Republika Południowej Afryki 
- Sudan Południowy  
- Tadżykistan 
- Tajlandia
- Turcja 
- Ukraina 
- Zjednoczone Emiraty Arabskie 
- Uzbekistan 
- Wenezuela
- Wietnam 


Aby uzyskać więcej informacji, przeczytaj [informacje o numerze identyfikatora rejestracji](reg-number-id.md)

## <a name="delete-a-location"></a>Usuwanie lokalizacji

Aby usunąć lokalizację z konta, należy skontaktować się z pomocą [techniczną partnera](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Pamiętaj jednak, że takie działanie będzie miało określone skutki. Nie można pobrać usuniętych lokalizacji i wszystkie elementy powiązane z tym konkretnym identyfikatorem MPN nie będą już rozpoznawane ani aktywne dla Twojej firmy.

## <a name="change-country-of-partner-global-account"></a>Zmiana kraju konta globalnego partnera 

1. Zaloguj się przy użyciu konta MPN w Partner Center. (Poświadczenia MPN mogą różnić się od poświadczeń CSP). Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

2. Na karcie **Partner** przejdź  do pozycji Lokalizacje biznesowe i sprawdź listę lokalizacji, aby upewnić się, że na liście znajduje się lokalizacja, której chcesz użyć jako jednostki prawnej. 
 
1. Aby dodać lokalizację, kliknij pozycję Dodaj lokalizację **i** na wysuwanych polach podaj wymagane szczegóły, takie jak nazwa firmy, adres i podstawowy kontakt dla lokalizacji, którą chcesz dodać do firmy. 
 
1. Wybierz **pozycję Zmień kraj** obok listy rozwijanej **Kraj/region** i wykonaj kroki. 

:::image type="content" source="images/lbp.png" alt-text="Dane prawne profilu biznesowego są wysuwu.":::

5. Wybierz pozycję **Zapisz**.

6. Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.
  
## <a name="next-steps"></a>Następne kroki

- Dowiedz się więcej o [procesie weryfikacji.](verification-responses.md)
