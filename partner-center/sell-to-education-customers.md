---
title: Jak sprzedawać oferty dla klientów edukacyjnych
description: Dowiedz się, jak utworzyć klienta edukacyjnego i sprzedawać oferty w centrum partnerskim. Obejmuje potwierdzenie stanu weryfikacji dla klienta edukacyjnego.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e0c8812683a038ce1f869cb3cb6750424d49ec05
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028371"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Jak sprzedawać oferty dla klientów edukacyjnych i jak utworzyć odbiorcę edukacji w centrum partnerskim

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny
- Agent sprzedaży

## <a name="create-an-education-customer"></a>Tworzenie klienta edukacyjnego

W tym artykule wyjaśniono, jak utworzyć klienta edukacji w centrum partnerskim i sprzedawać do nich produkty edukacyjne. Opisano w nim również, jak wyświetlić stan weryfikacji i ponownie przesłać żądanie weryfikacji, jeśli jest to konieczne. Oferty edukacyjne są obecnie **dostępne tylko dla usług opartych na licencji** , takich jak Microsoft 365, Dynamics, Intune itd. Nie jest ona dostępna dla innych typów (subskrypcje oprogramowania, bezterminowego oprogramowania lub produktów platformy Azure).

> [!IMPORTANT]
> Firma Microsoft weryfikuje każdą nowo utworzoną dzierżawcę klientów edukacyjnych, aby upewnić się, że są one kwalifikowane dla ofert edukacyjnych.  Upewnij się, że wprowadzasz wymagane informacje jako dokładne i pełne, jak to możliwe, aby uniknąć opóźnień w procesie weryfikacji.

1. Zaloguj się do Centrum partnerskiego.

2. Wybierz pozycję **klienci** , a następnie wybierz pozycję **Dodaj klienta**. Wybierz pozycję **Edukacja** na liście rozwijanej **specjalne kwalifikacje** .  Wprowadź pozostałe informacje o koncie zgodnie z wymaganiami.  Kluczowe pola, które ułatwiają proces weryfikacji, obejmują:

   - **Nazwa firmy**: Wprowadź nazwę podmiotu prawnego — wymagana do weryfikacji
   - **Wiersze kraju/regionu i adresu**: wprowadź pełny adres korespondencyjny jednostki — wymagany do weryfikacji
   - **Adres e-mail**: Wprowadź wiadomość e-mail będącą właścicielem jednostki — nie jest to bezpłatna ani on.Microsoft.Coma wiadomość e-mail — wymagana do weryfikacji
   - **Informacje kontaktowe klienta**: te szczegóły będą używane w ramach procesu weryfikacji
   - **Podstawowa nazwa domeny**: służy do tworzenia konta klienta i adresów e-mail.  Wybierz nazwę podobną do nazwy firmy bez spacji i znaków specjalnych.  Tej nazwy nie można zmienić później.

3. Po zakończeniu wybierz pozycję **Przegląd**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Konto klienta edukacyjnego":::

4. Po potwierdzeniu **przeglądu** zostanie wyświetlony stan **nieprzeglądu** , jeśli przesłane informacje są prawidłowe. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Przekształcenie konta klienta w przegląd"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Potwierdzenie stanu weryfikacji klienta edukacyjnego

Na stronie **konto** klienta zapoznaj się z tematem **specjalne kwalifikacje**.
Przykłady stanu:

- Jeśli klient przeszedł weryfikację: Education

   :::image type="content" source="images/edupassedvetting.png" alt-text="Weryfikacja edukacji zakończyła się pomyślnie":::

- Jeśli klient nie przeszedł weryfikacji: nie jest to klient edukacyjny

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Weryfikacja edukacji zakończyła się niepowodzeniem" lightbox="images/edu/fail-reason-expanded.png":::

- Jeśli klient nie został oznaczony jako klient edukacyjny: brak

   :::image type="content" source="images/edu/account-one.png" alt-text="Klient edukacyjny nie jest oznakowany jako taki" lightbox="images/edu/account-one-expanded.png":::

- Jeśli klient jest przeglądany jako klient edukacyjny: w przeglądzie

    :::image type="content" source="images/edu/in-review.png" alt-text="przegląd dla klienta edukacyjnego" lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Popraw informacje o koncie klienta i prześlij je ponownie w celu weryfikacji

Jeśli klient nie przejdzie do początkowej weryfikacji, można teraz skorygować informacje i ponownie przesłać go.

### <a name="correct-the-customer-account-information"></a>Poprawianie informacji o koncie klienta

Aby zaktualizować informacje o kliencie, musisz mieć uprawnienia administratora globalnego. Informacje są aktualizowane w portalu pakietu Office 365, ponieważ nie można zaktualizować tych danych za pomocą portalu Centrum partnerskiego.

1. Na stronie **konto** zostaną wyświetlone informacje stwierdzające, że kwalifikacja klienta jest uznawana za "nie jest to klient edukacyjny".

2. Odśwież przeglądarkę, aby zresetować stronę. Będzie dostępny przycisk **aktualizacji** , a dla opcji **specjalne kwalifikacje** zostanie ustawiona wartość **Brak**.

3. Wybierz pozycję **Aktualizuj**. Na stronie **Zarządzanie usługami** wybierz pozycję **Office 365**.

4. Nastąpi przekierowanie do centrum administracyjnego pakietu Office 365 na nowej karcie przeglądarki. Być może zażądano zalogowania się przy użyciu swoich poświadczeń.

5. Wybierz pozycję **Ustawienia**.

6. Wybierz kartę **profil organizacji** w górnej części ekranu, a następnie **Informacje o organizacji**. Teraz możesz zaktualizować szczegóły klienta.

7. Wybierz pozycję **Zapisz zmiany** w dolnej części paska bocznego.  

### <a name="resubmit-for-verification"></a>Prześlij ponownie w celu weryfikacji

1. Przejdź do karty Centrum partnerskiego i na stronie **konto** klienta. Odśwież przeglądarkę i sprawdź, czy strona firmy została zaktualizowana o nowe informacje. Wybierz przycisk **Aktualizuj** , aby zażądać ponownej weryfikacji edukacji.

2. Jeśli zaktualizowane szczegóły klienta są uprawnione do korzystania z ofert edukacyjnych, zostaną wyświetlone **specjalne zastrzeżenia** , które zostały zaktualizowane do **edukacji**. Jeśli nadal nie widzisz **klienta edukacyjnego**, skontaktuj się z pomocą techniczną w celu weryfikacji ręcznej.

## <a name="next-steps"></a>Następne kroki

- [Sprzedaż w specjalistycznych branżach](get-special-pricing-for-offers.md)

- [Dodawanie nowego klienta](add-a-new-customer.md)

- [Sprzedaj Minecraft: subskrypcje wersji edukacyjnej dla klientów edukacyjnych](minecraft-subscriptions.md)
