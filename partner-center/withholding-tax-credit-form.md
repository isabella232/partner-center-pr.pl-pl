---
title: Uzyskiwanie środków na podatek potrącony
ms.topic: article
ms.date: 06/05/2020
description: Odbierz kredyt na koncie Partner Center na potrącenie podatku. Informacje obejmują kroki przesyłania żądania potrącenia podatku.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2d0c1e05ff0e0b9c807dfc7beb1136cec87b4069
ms.sourcegitcommit: 8fe3b0f22d548bc6bcc1b87636216cd4d42b3ede
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/17/2021
ms.locfileid: "122297151"
---
# <a name="receive-credit-on-your-partner-center-account-for-tax-withholding"></a>Otrzymywanie środków na koncie Partner Center na potrącenie podatku

**Odpowiednie role:** Administrator konta | Administrator rozliczeń

## <a name="overview"></a>Omówienie

Dostawca rozwiązań w chmurze (CSP) w niektórych krajach otrzymują kwoty faktur, które obejmują podatki. Niektórzy z tych partnerów płacą za swój lokalny urząd podatkowy, a nie firmę Microsoft. Jeśli płacisz lokalnemu urzędowi podatkowemu, musisz przesłać żądanie potrącenia podatku, w tym certyfikat podatkowy, aby wyczyścić kwotę podatku z poprzednich faktur. Te wyczyszone kwoty są odzwierciedlane w kolumnie **Ostatnia** płatność na stronie **Rozliczenia w** Partner Center.

Partnerzy używali do przesyłania żądań potrącenia podatku przez utworzenie żądań obsługi (biletów pomocy technicznej partnera) w Partner Center. Ten proces zmienił się w styczniu 2020 r. Teraz partnerzy CSP powinni przesyłać żądania potrącenia podatku na **stronie Rozliczenia** zamiast tworzyć żądania pomocy technicznej.

> [!IMPORTANT]
> Partnerzy mogą przesyłać żądania podatku potrącanego tylko w przypadku częściowo płatnych faktur. W przypadku w pełni płatnych lub nieuprawnianych faktur skontaktuj się z pomocą [techniczną,](report-problems-with-partner-center.md) kontaktując się z pomocą techniczną, kontaktując się z certyfikatem potrącania podatku.

## <a name="submit-a-tax-withholding-request"></a>Przesyłanie żądania potrącenia podatku

Wykonaj następujące kroki, aby przesłać nową potrącenie podatku:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego.

2. W menu po lewej stronie wybierz pozycję **Rozliczenia** i przejdź do **pozycji Historia rozliczeń.**

3. Wybierz **pozycję Prześlij nową** obok faktury, dla której chcesz przesłać fakturę. Link prześlij nowy spowoduje, że zostaniesz przekierowyny do **strony Nowy wniosek o potrącenie podatku.**

   :::image type="content" source="images/wht1.png" alt-text="Prześlij nową potrącenie podatku dla faktury.":::

4. Przejrzyj szczegóły faktury, aby upewnić się, że przesyłasz żądanie prawidłowej faktury.

   :::image type="content" source="images/wht2.png" alt-text="Uzupełnij szczegóły potrącenia podatku dla faktury.":::

5. Wprowadź wartość "Suma potrąceń" w obszarze **Szczegóły potrącenia podatku.** "Suma potrąceń" to kwota, która ma zostać zasypowana.

6. **Dołącz** certyfikat podatkowy. W żądaniu potrącenia podatku  należy dołączyć cyfrową kopię certyfikatu podatku potrącanego.  Ten certyfikat został otrzymany od lokalnej urzędu skarbowego, gdy płacisz podatki lokalnemu urzędowi podatkowemu. Kwota podatku na podstawie faktury w certyfikacie podatku potrącanego musi być dopasowana do łącznej kwoty w żądaniu potrącenia podatku.

   > [!IMPORTANT]
   > Sumy zapewniane przez partnera powinny być zgodne z linią faktury z dołączonego certyfikatu podatkowego. Dołączone pliki certyfikatów podatkowych muszą być w jednym z następujących formatów plików: .PDF tylko obraz (. JPEG, .PNG i .GIF). Ponadto nazwy plików nie powinny zawierać spacji ani znaków specjalnych. Rozmiary plików nie mogą przekraczać 1 MB.

7. **Prześlij** żądanie potrącenia podatku.

   Po przesłaniu żądanie zostanie przekazane do procesu zatwierdzania, w którym zostanie zatwierdzone do ukończenia lub wysłane z powrotem w razie potrzeby poprawek. Wyświetl identyfikator i stan żądania oraz  historię rozliczeń, z której przesłaliśmy nowe żądanie.

   Jeśli żądanie zostanie wysłane z powrotem do Ciebie, będzie można zmienić kwotę potrącenia i zastąpić certyfikat, jeśli występuje z nim problem.

## <a name="update-request-and-resubmit"></a>Aktualizowanie żądania i ponowne prześlij

Zespół przeglądu może wymagać poprawek i ponownego prześlij żądanie, zanim będzie można je zatwierdzić. Zmienią stan na **Oczekująca akcja partnera.** Aby poprawić i ponownie przesłać żądanie:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego.

2. W menu po lewej stronie wybierz pozycję **Rozliczenia**

3. Na stronie **Historia** rozliczeń **znajdź** żądanie potrącenia podatku. Żądania, które wymagają Twojej uwagi, będą mieć stan "Oczekiwanie na akcję partnera".

4. Wybierz identyfikator żądania potrącenia podatku i stan, który umożliwia dostęp do strony żądania.

5. Wybierz **pozycję Aktualizuj i prześlij ponownie w** obszarze **Stan.**

6. Przejrzyj komentarze pozostawione przez recenzentów, zaznaczając, co należy zmienić.

7. Dokonaj korekt, ponownie prześlij zaktualizowany certyfikat lub dostosuj kwoty potrąceń.

8. **Prześlij** żądanie.

Przesłanie żądania spowoduje wysłanie go z powrotem do zespołu przeglądowego, w którym zatwierdzi lub poprosi o więcej zmian.

### <a name="approved-requests"></a>Zatwierdzone żądania

Zatwierdzone żądania potrącenia podatku będą wykonywane na następnej fakturze, co spowoduje zaniżanie należnej kwoty. Żądania oflagowane jako **Ukończone** powinny być stosowane w ciągu 10 dni roboczych. 

Wyczyszone kwoty zostaną odzwierciedlone w sekcji Historia rozliczeń **strony rozliczeniowej**. Kwoty wyczyszone będą wyświetlane w kolumnie **Ostatnia** płatność obok faktury, do których przesłano żądanie.

   > [!IMPORTANT]
   > Poprzednie faktury nie są ponownie wygenerowane ani ponownie wystawiane. Kwota wyczyść jest po prostu stosowana do płatności z poprzednich miesięcy.

Przetwarzanie żądań potrącenia podatku powinno potrwać dwa dni przy założeniu, że certyfikat podatkowy i kwota są poprawne. Jeśli są wymagane zmiany, będzie to trwać dłużej ze względu na poprawki, które należy wprowadzić i ponownie przesłać.

Jeśli masz pytania dotyczące procesu żądania kredytu z tytułu podatku potrącanego, prześlij bilet do pomocy technicznej partnera. Będziesz potrzebować identyfikatora żądania potrącenia podatku, aby odpowiedzieć na pytania.

## <a name="german-tax-withholding"></a>Niemiecki potrącenie podatku

Partnerzy, którzy przesyłają niemieckie żądania potrącenia podatku, powinni pamiętać o przesłaniu kopii certyfikatu z tytułu podatku potrącanego na następujący adres:

- ATTN: EOC Tax Team Suwne Gannon
- Microsoft EMEA Operations Centre
- One Microsoft Place,
- South County Business Park
- Dossztad, Dublin 18, Holandia

### <a name="questions-and-assistance-for-tax-withholding-requests"></a>Pytania i pomoc dotyczące żądań potrącenia podatku

Partnerzy powinni użyć nowego procesu opisanego powyżej, aby przesłać nowe żądania i nie używać już tworzenia żądań pomocy technicznej dla nowych żądań potrącenia podatku. Partnerzy, którzy mają więcej pytań dotyczących żądań potrącenia podatku, mogą [przesyłać wnioski o pomoc techniczną.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?stage=2&topicid=9227afa6-babf-3917-acee-67db7860f5ed) Żądania pomocy technicznej mają pomóc partnerom w przypadku istniejących żądań, więc muszą mieć swój identyfikator żądania, **aby** przesłać nowy bilet. Jeśli partnerzy nie mogą przesłać żądania przy użyciu nowego procesu, powinni wprowadzić jakieś liczby (wszystkie 1) w formularzu żądania pomocy technicznej. 

   > [!IMPORTANT]
   > Partnerzy nie muszą kontaktować się z pomocą techniczną, jeśli stan żądania to **Ukończono.** Ten stan jest przedstawiany w historii **rozliczeń** obok faktury do przesłania. **Ostatnie kwoty** płatności obok faktury powinny odzwierciedlać kwotę potrącenia podatku w ciągu 10 dni po oznaczeniu żądania jako **Ukończono.**
