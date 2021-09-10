---
title: Jak sprzedawać oferty klientom edukacyjnym
description: Dowiedz się, jak utworzyć klienta edukacyjnego i sprzedawać im oferty w Partner Center. Obejmuje potwierdzenie stanu weryfikacji dla klienta edukacyjnego.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2d9924b8d361be4237c613467a1d36db29cf7d9e
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958774"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Jak sprzedawać oferty klientom edukacyjnym i jak utworzyć klienta edukacyjnego w Partner Center

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Agent sprzedaży

## <a name="create-an-education-customer"></a>Tworzenie klienta edukacyjnego

W tym artykule wyjaśniono, jak utworzyć klienta edukacyjnego w Partner Center i sprzedawać im produkty edukacyjne. Opisano w nim również sposób wyświetlania stanu weryfikacji i ponownego prześlij żądanie weryfikacji w razie potrzeby. Oferty edukacyjne są obecnie **dostępne tylko dla usług opartych** na licencjach, takich jak Microsoft 365, Dynamics, Intune itp. Nie jest ona dostępna dla innych typów (subskrypcji oprogramowania, oprogramowania bezterminowego lub produktów platformy Azure).

> [!IMPORTANT]
> Firma Microsoft sprawdza każdą nowo utworzoną dzierżawę klienta edukacyjnego, aby upewnić się, że są oni zakwalifikowani do ofert edukacyjnych.  Upewnij się, że wprowadzasz wymagane informacje tak dokładnie i całkowicie, jak to możliwe, aby zapobiec opóźnieniom w procesie weryfikacji.

1. Zaloguj się do Centrum partnerskiego.

2. Wybierz **pozycję Klienci,** a następnie **wybierz pozycję Dodaj klienta.** Wybierz **pozycję Edukacja** z listy **rozwijanej Kwalifikacje** specjalne.  Wypełnij pozostałe informacje o koncie zgodnie z potrzebami.  Kluczowe pola, które pomagają w procesie weryfikacji, obejmują:

   - **Nazwa firmy:** WPROWADŹ NAZWĘ JEDNOSTKI PRAWNEJ — wymagana do weryfikacji
   - **Kraj/region i wiersze adresów:** WPROWADŹ PEŁNY ADRES POCZTOWY JEDNOSTKI — wymagany do weryfikacji
   - **Adres e-mail:** wprowadź wiadomość e-mail należącą do jednostki — nie bezpłatną ani on.microsoft.com e-mail — wymaganą do weryfikacji
   - **Informacje kontaktowe klienta:** te szczegóły będą używane w procesie weryfikacji
   - **Nazwa domeny podstawowej:** służy do tworzenia konta klienta i adresów e-mail.  Wybierz nazwę podobną do nazwy firmy bez spacji ani znaków specjalnych.  Tej nazwy nie można później zmienić.

3. Po zakończeniu wybierz pozycję **Przejrzyj**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Konto klienta edukacyjnego.":::

4. Po potwierdzeniu **weryfikacji** w programie zostanie wyświetlony stan **InReview (Wprzejrzysz),** jeśli przesłane informacje są prawidłowe. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Konto klienta edukacyjnego w przeglądzie."lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Potwierdzanie stanu weryfikacji klienta edukacyjnego

Na stronie Konto klienta **zobacz Specjalny** **stan kwalifikacji**.
Przykłady stanu:

- Jeśli klient przeszedł weryfikację: Edukacja

   :::image type="content" source="images/edupassedvetting.png" alt-text="Weryfikacja edukacji powiodła się.":::

- Jeśli klient nie przejdzie weryfikacji: nie jest klientem edukacyjnym

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Weryfikacja edukacji nie powiodła się." lightbox="images/edu/fail-reason-expanded.png":::

- Jeśli klient nie został otagowany jako klient edukacyjny: Brak

   :::image type="content" source="images/edu/account-one.png" alt-text="klient edukacyjny nie jest w związku z tym otagowany." lightbox="images/edu/account-one-expanded.png":::

- Jeśli klient jest przeglądany jako klient edukacyjny: W przeglądzie

    :::image type="content" source="images/edu/in-review.png" alt-text="education customer is in review." lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Poprawianie informacji o koncie klienta i ponowne ich prześlij do weryfikacji

Jeśli klient nie powiedzie się podczas wstępnej weryfikacji, możesz teraz poprawić informacje i ponownie je przesłać.

### <a name="correct-the-customer-account-information"></a>Poprawianie informacji o koncie klienta

Aby zaktualizować informacje o kliencie, musisz mieć uprawnienia administratora globalnego. Zaktualizuj informacje w portalu Office 365, ponieważ tych danych nie można zaktualizować z Partner Center portalu.

1. Na **stronie Konto** zobaczysz informacje z informacją, że kwalifikacja klienta jest uważana za "Nie jest klientem edukacyjnym".

2. Odśwież przeglądarkę, aby zresetować stronę. Zostanie ustawiony przycisk **Aktualizuj,** a **stan Kwalifikacje specjalne** zostanie ustawiony na **wartość Brak.**

3. Wybierz pozycję **Aktualizuj**. Na stronie **Zarządzanie usługami** wybierz pozycję **Office 365**.

4. Nastąpi przekierowanie do centrum Office 365 na nowej karcie przeglądarki. Może pojawić się prośba o zalogowanie się przy użyciu swoich poświadczeń.

5. Wybierz pozycję **Ustawienia**.

6. Wybierz **kartę Organization profile (Profil** organizacji) w górnej części ekranu, a następnie pozycję **Organization information (Informacje o organizacji).** Teraz możesz zaktualizować szczegóły klienta.

7. Wybierz **pozycję Zapisz** zmiany w dolnej części paska bocznego.  

### <a name="resubmit-for-verification"></a>Prześlij ponownie do weryfikacji

1. Przejdź na kartę Partner Center i do strony **konta** klienta. Odśwież przeglądarkę i sprawdź, czy strona Firmy została zaktualizowana do nowych informacji. Wybierz **przycisk Aktualizuj,** aby poprosić o ponowną weryfikację edukacji.

2. Jeśli zaktualizowane szczegóły klienta kwalifikują się do ofert edukacyjnych, zobaczysz, że kwalifikacje **specjalne** zostały zaktualizowane do **oferty Education**. Jeśli nadal widzisz element **Nie dla** klientów edukacyjnych, skontaktuj się z pomocą techniczną w celu weryfikacji ręcznej.

## <a name="next-steps"></a>Następne kroki

- [Sprzedaż w specjalistycznych branżach](get-special-pricing-for-offers.md)

- [Dodawanie nowego klienta](add-a-new-customer.md)

- [Sprzedaż Minecraft: Education Edition subskrypcji dla klientów edukacyjnych](minecraft-subscriptions.md)
