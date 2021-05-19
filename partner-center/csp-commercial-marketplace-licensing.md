---
title: Zarządzanie licencjonowaniem w ofertach platformy handlowej
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak skonfigurować licencjonowanie dla ofert platformy handlowej dla isV i zarządzać nimi.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147959"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Zarządzanie licencjonowaniem w ofertach platformy handlowej

**Odpowiednie role:** Administrator globalny | Administrator konta

W tym artykule o mowa o procesie konfigurowania oferty w u Partner Center, jej Microsoft AppSource, a następnie zarządzania licencjami dla tej oferty.  

>[!IMPORTANT]
>Możliwości w tym artykule są obecnie dostępne w publicznej wersji zapoznawczej.

## <a name="before-you-begin"></a>Zanim rozpoczniesz

### <a name="commercial-marketplace-basics"></a>Podstawy komercyjnej platformy handlowej

Przed rozpoczęciem tego procesu należy zapoznać się z podstawami platformy handlowej. Artykuły w poniższej tabeli pomogą Ci rozpocząć pracę. 

| Temat  | Artykuł  |
|-------|--------|
|Plany komercyjnej platformy handlowej | [Plany i cennik ofert komercyjnej platformy handlowej](/azure/marketplace/plans-pricing)    |
|Oferty komercyjnej platformy handlowej  | [Typy ofert](/azure/marketplace/determine-your-listing-type)    |
|Konta komercyjnej platformy handlowej |  [Tworzenie konta komercyjnej platformy handlowej w Partner Center](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Określanie identyfikatora oferty

W poniższych procedurach zostanie wyświetlony monit o wprowadzenie identyfikatora oferty. Poślij teraz trochę czasu, aby wymyślić odpowiedni identyfikator oferty, pamiętając o następujących kwestiach:

- Ten identyfikator jest widoczny dla klientów w adresie internetowym oferty marketplace i Azure Resource Manager, jeśli ma to zastosowanie.
- Identyfikator oferty w połączeniu z identyfikatorem wydawcy musi mieć długość poniżej 40 znaków.
- Użyj tylko małych liter i cyfr. Identyfikator oferty może zawierać łączniki i podkreślenia, ale nie może zawierać spacji. Jeśli na przykład identyfikator wydawcy to , a po wprowadzeniu adresu `testpublisherid` , adres internetowy oferty będzie miał wartość `test-offer-1` `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Tego identyfikatora nie można zmienić po wybraniu opcji **Utwórz**.

### <a name="determine-your-offer-alias"></a>Określanie aliasu oferty

Alias oferty to nazwa używana dla oferty w Partner Center. Będziesz również potrzebować odpowiedniego aliasu oferty, który jest zgodny z poniższymi wytycznymi:

- Ta nazwa nie jest używana na platformie handlowej i różni się od nazwy oferty i innych wartości wyświetlanych klientom.
- Tej nazwy nie można zmienić po wybraniu opcji Utwórz.

## <a name="create-your-offer"></a>Tworzenie oferty

Pierwszym krokiem procesu licencjonowania jest utworzenie oferty platformy handlowej. 

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).
2. W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/przegląd.**
3. W górnej części strony Przegląd wybierz pozycję Nowa **oferta,** a następnie wybierz pozycję **Dynamics 365 for Customer Engagement & PowerApps.**
4. Wprowadź utworzone **wcześniej identyfikator oferty** i **alias** oferty.
5. Wybierz **pozycję Utwórz,** aby wygenerować ofertę i kontynuować.
6. Wybierz opcje licencjonowania.

    - Aby włączyć zarządzanie licencjami dla oferty, wybierz pozycję **Włącz zarządzanie licencjami aplikacji za pośrednictwem firmy Microsoft.** Jest to ustawienie raz i nie można go zmienić po opublikowaniu oferty.

    - Możesz również umożliwić klientom uruchamianie podstawowych funkcji aplikacji bez licencji oraz uruchamianie funkcji Premium po zakupie licencji. W tym celu wybierz pozycję **Zezwalaj klientom na instalowanie mojej aplikacji,** nawet jeśli licencje nie są przypisane.

    - Jeśli nie chcesz, aby Twoja oferta zawierała włączone zarządzanie licencjami, wybierz pozycję Pobierz teraz **(wersja bezpłatna),** Bezpłatna wersja **próbna** lub **Skontaktuj się ze mną.**

## <a name="create-your-plan"></a>Tworzenie planu

W tych krokach zdefiniujesz plan lub plany, które chcesz włączyć dla oferty.

1. W menu nawigacji po lewej stronie wybierz **pozycję Plan overview**, a następnie wybierz pozycję Utwórz nowy **plan.**
2. Wprowadź identyfikator **planu i** **nazwę planu,** a następnie wybierz pozycję **Utwórz**.
3. Na stronie **listy Plan** wprowadź opis **planu**.
4. Aby zapisać opis i zakończyć go później, wybierz pozycję **Zapisz roboczą.**

5. Po zakończeniu wybierz pozycję **Przejrzyj i opublikuj**. Informacje o planie będą teraz wyświetlane na stronie appsource.microsoft.com w obszarze oferty (sekcja planów).

6. Po utworzeniu wszystkich planów dla tej oferty należy skopiować identyfikator usługi każdego planu. Wybierz **pozycję Plan overview** (Omówienie planu) w górnej części strony z listą planów. Skopiuj identyfikator usługi dla każdego planu do bezpiecznej lokalizacji.

## <a name="add-service-ids-to-your-solution"></a>Dodawanie identyfikatorów usług do rozwiązania

Następnym krokiem jest zaktualizowanie rozwiązania przez dodanie identyfikatorów usług dla każdego skopiowanego planu. Aby uzyskać wskazówki dotyczące tego problemu, zobacz Create an AppSource Package for your solution (Tworzenie [pakietu usługi AppSource dla rozwiązania).](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Przekazywanie pakietu i publikowanie oferty

1. W okienku nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa,** a następnie wybierz **pozycję Konfiguracja techniczna.**
2. W **obszarze Podstawowy model licencji** wybierz pozycję **Użytkownik.**
3. W **obszarze Pakiet CRM** wprowadź adres URL lokalizacji pakietu.
4. Użyj innych kart w okienku nawigacji po lewej stronie, aby wprowadzić inne wymagane informacje. Gdy wszystko będzie gotowe, wybierz pozycję **Przejrzyj i opublikuj.**

Po opublikowaniu oferty przejmiemy i zweryfikujemy Twoje informacje. W przypadku jakichkolwiek problemów z tym procesem powiadomimy Cię. Gdy wszystkie problemy zostaną rozwiązane, otrzymasz powiadomienie o tym, że oferta jest dostępna w usłudze AppSource. W tym momencie można ją udostępnić.

## <a name="make-your-offer-live-in-partner-center"></a>Udostępnij swoją ofertę w Partner Center

W poniższej procedurze przedstawiono proces tworzenia oferty na żywo w usłudze AppSource. Aby dowiedzieć się więcej na temat tego procesu, [zobacz Wprowadzenie do opcji listy](/azure/marketplace/determine-your-listing-type).

>[!NOTE]
>Po opublikowaniu oferty jej opublikowanie potrwa 4–6 godzin.

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).
2. W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/przegląd.**
3. Na **stronie Przegląd** znajdź szukaną ofertę. Oferty gotowe do opublikowania będą mieć stan Wersja **zapoznawcza.** Wybierz ofertę.
4. Na stronie **Omówienie oferty** wybierz pozycję Przejdź **na żywo.**
Oferta będzie żywa w ciągu 4–6 godzin.
5. Aby wyświetlić ofertę oferty w usłudze AppSource, wybierz link **AppSource** w dolnej części **strony Omówienie** oferty.

    - **W przypadku ofert z włączoną** licencją: jeśli Oferta wymaga sprawdzenia licencji, użytkownicy będą mogli wprowadzić potencjalnego klienta tylko przez kliknięcie pozycji Skontaktuj się ze **mną,** aby móc się z nimi komunikować.

    - **W przypadku ofert** z włączoną licencją z opcją instalacji bezpłatnej: jeśli oferta nie wymaga sprawdzenia licencji, administratorzy zobaczą przycisk Pobierz **teraz** oprócz opcji Skontaktuj się **ze mną.** Użytkownicy, którzy chcą wypróbować bezpłatną opcję instalacji, powinni kliknąć pozycję Pobierz **teraz,** aby zainstalować ofertę w Power Platform administracyjnym. Użytkownicy mogą nadal używać funkcji Skontaktuj się **ze mną,** jeśli mają pytania lub chcą podwyżsić plan do planu płatnego.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Rejestrowanie transakcji isv connect w rejestracji transakcji

Aby można było przypisać licencje do klienta, każda sprzedaż musi być zarejestrowana w Partner Center. Aby to zrobić, zobacz [Rejestrowanie transakcji.](register-deals.md)

## <a name="invite-the-customer"></a>Zapraszanie klienta

Użyj poniższej procedury, aby zaprosić klienta do wzięcia udziału w tej transakcji.  

1. Zaloguj się do [pulpitu nawigacyjnego Centrum partnerskiego](https://partner.microsoft.com/dashboard/).
2. W menu nawigacji po lewej stronie wybierz pozycję **Komercyjna platforma handlowa/Przegląd.**
3. W menu nawigacji po lewej stronie wybierz **pozycję Polecenia**, a następnie wybierz pozycję **Rejestracja transakcji.**
4. **Odfiltruj** przesłane transakcje, wybierz **kartę W** toku, a następnie wybierz transakcję, której potrzebujesz.
5. Na stronie przeglądu tej transakcji wybierz pozycję **Zarządzaj licencjami.**
6. W **oknie Zarządzanie licencjami** wybierz klienta z **listy rozwijanej Szczegóły** klienta. Jeśli relacja z klientem jeszcze nie istnieje, wybierz **pozycję +Zaproś nowego klienta do wyrażenia zgody.**
7. Skopiuj wyświetlony link.
8. Wyślij ten link pocztą e-mail do administratora rozliczeń lub administratora globalnego klienta i za pomocą tego linku uzyskaj dostęp do usługi admin.microsoft.com oraz zaakceptuj i autoryzuj nawiązywaną relację.

    >[!NOTE]
    >Relacja nie zostanie ustanowiona, dopóki klient nie wykona tego kroku.

## <a name="activate-manage-and-remove-your-licenses"></a>Aktywowanie i usuwanie licencji oraz zarządzanie nimi

Po autoryzowaniu relacji z Tobem przez klienta możesz rozpocząć dodawanie planów z oferty i przypisywanie licencji do każdego planu.

1. W oknie Zarządzanie licencjami dla tej transakcji wybierz **pozycję +Dodaj plan**.
2. Wypełnij pola **Plany dla tego rozwiązania i** Liczba **licencji,** a następnie wybierz **pozycję Aktualizuj licencje.** Licencje będą dostępne na stronie admin.microsoft.com, aby klienci mogą zarządzać pracownikami i przypisywać je do pracowników.

    - Aby zmienić liczbę licencji dla istniejącego planu, wprowadź nową liczbę w polu Liczba licencji, a następnie wybierz **pozycję Aktualizuj licencje.** 

    - Aby dezaktywować lub usunąć licencje dla transakcji,  wybierz ikonę kosza w polu Akcje, a następnie wybierz **pozycję Aktualizuj licencje.**

## <a name="next-steps"></a>Następne kroki

[Zasoby licencjonowania](support-resources-licensing.md)