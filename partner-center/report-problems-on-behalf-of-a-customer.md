---
title: Zgłaszanie problemów w imieniu klienta
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, kiedy eskalować problem z obsługą klienta do firmy Microsoft i jak uzyskać bilet pomocy technicznej dla różnych typów usług firmy Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0cf8769bcf45ba90a714231a7c9db7660efce0b0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549060"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Zgłoś problem dotyczący usługi w imieniu klienta — w tym informacje o tym, kiedy i jak to zrobić

**Dotyczy**

- Centrum partnerskie w chmurze firmy Microsoft dla instytucji rządowych

**Odpowiednie role**

- Dostawca pośredni

Jeśli klient napotkał problem z usługą, którego nie można rozwiązać, i spełnia kryteria opisane w temacie [Eskalacja problemów do firmy Microsoft](escalate-problems-to-microsoft.md), Dostawca pośredni może w tym celu przekazać bilet pomocy technicznej. Ten proces jest również przydatny w przypadku eskalacji problemów z rozliczeniami lub sporów oraz w przypadku problemów związanych z oszustwem.

## <a name="submit-a-service-request-for-a-customer"></a>Prześlij żądanie obsługi dla klienta

1. W menu Centrum partnerskiego w obszarze dostawca usług kryptograficznych wybierz pozycję **klienci**

2. Na stronie klienci Wybierz lub Wyszukaj żądanego klienta
    
3. Z menu Klient wybierz pozycję **żądania obsługi**

4. Z menu rozwijanego **nowe żądanie** wybierz pozycję **Azure** lub **Office 365, Dynamics 365 i Enterprise Mobility Suite**. Nastąpi przekierowanie do Microsoft Azure Portal lub centrum administracyjnego pakietu Office 365.

>[!NOTE]
>W programie CSP są wymagane wsparcie dla partnerów operacyjnych obsługujących usługi Dynamics 365 w ramach umowy dotyczącej pomocy technicznej Advanced support for Partner (ASfP) lub wyższy. Ta umowa dotycząca pomocy technicznej jest wymagana do przesłania zdarzeń Dynamics 365 w imieniu klienta programu CSP. [Dowiedz się więcej](https://partner.microsoft.com/support/partnersupport) o opcjach umowy serwisowej.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Jeśli musisz utworzyć żądanie obsługi dla klienta na platformie Azure, weź pod uwagę następujące kwestie:
>
>- Aby zapewnić, że jako pośredni odsprzedawca do tworzenia żądań obsługi dla klienta na platformie Azure, Dostawca pośredni musi udzielić dostępu do konta platformy Azure klienta. Różni się to od administrowania w imieniu klientów pakietu Office 365.
>
>- Chociaż Administrator pomocy technicznej w centrum partnerskim nie może tworzyć żądań obsługi w portalu usługi Azure, co można zrobić, Utwórz grupę pomocy technicznej w portalu usługi Azure i nadaj im uprawnienia do rejestrowania żądań obsługi.

1. Wybierz pozycję **Nowe żądanie obsługi**.

2. Wypełnij żądanie pomocy technicznej odpowiednimi informacjami, a następnie wybierz pozycję **Utwórz**:

   - W sekcji **podstawowe** żądania obsługi upewnij się, że wybrano opcję **dostawca rozwiązań w chmurze** w polu **Plan pomocy technicznej** .

   - W sekcji informacje **kontaktowe** żądania pomocy technicznej wprowadź swoje informacje, a nie informacje o kliencie.

3. Później Przejrzyj żądania obsługi klienta w ramach Microsoft Azure Portal, wybierając pozycję **Zarządzaj żądaniami pomocy technicznej**.

Jeśli nie masz uprawnień administratora dla tego klienta, może być konieczne utworzenie żądania pomocy technicznej dla klienta. Może się to zdarzyć w jednym z dwóch scenariuszy:

- Nie zażądano uprawnień administratora podczas pierwszego ustanowienia relacji.
- Zarządzanie subskrypcjami platformy Azure klienta jest możliwe tylko wtedy, gdy nie masz uprawnień administracyjnych.
 
W każdym z tych przypadków można użyć następującej procedury, aby utworzyć żądanie obsługi. 

1. Skopiuj nazwę domeny klienta na stronie konta w centrum partnerskim.

2. Przejdź do https://portal.azure.com/ [customerdomainname]. 

3. Wybierz subskrypcję platformy Azure wymagającą pomocy technicznej.

4. Wybierz pozycję **nowe żądanie obsługi**, a następnie postępuj zgodnie z monitami, aby utworzyć żądanie. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. W sekcji **Tworzenie żądania obsługi** wybierz odpowiednią kategorię pomocy technicznej. Może być konieczne wybranie opcji **więcej...** , aby wyświetlić dodatkowe artykuły.

2. Wypełnij formularz żądanie obsługi, a następnie wybierz pozycję **Prześlij**.

   > [!TIP]
   > Pamiętaj o uwzględnieniu informacji kontaktowych, a nie Twojego klienta.

3. Później Przejrzyj żądania obsługi klienta, przechodząc do centrum administracyjnego pakietu Office 365 i wybierając pozycję **Pokaż wszystkie bilety pomocy technicznej**.

### <a name="support-for-commercial-marketplace-products"></a>Obsługa komercyjnych produktów Marketplace

Firma Microsoft nie zapewnia pomocy technicznej produktów dla komercyjnych produktów Marketplace. Musisz skontaktować się z niezależnym dostawcą oprogramowania (ISV), który opublikował produkt, aby uzyskać pomoc techniczną.

Aby znaleźć informacje kontaktowe niezależnego dostawcy oprogramowania:

1.  Na stronie **Marketplace** wybierz produkt, z którym chcesz uzyskać pomoc.

2.  Na stronie produktu znajdziesz informacje o kontakcie. Może to być co najmniej jedna z następujących opcji:

    - Link do punktu wejścia pomocy technicznej w witrynie sieci Web niezależnego dostawcy oprogramowania
    - Wiadomość e-mail z pomocą techniczną
    - Numer telefonu kontaktowego pomocy technicznej

## <a name="faq"></a>Często zadawane pytania

Zapoznaj się z poniższymi często zadawanymi pytaniami dotyczącymi żądań obsługi, które można przesłać w imieniu klienta. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Co obejmuje uprawnienie do pomocy technicznej?

Żądania obsługi powinny być zgłaszane przez centrum partnerskie. Są one dostępne na platformie Azure, Microsoft Office 365, Microsoft Dynamics CRM Online i Enterprise Mobility Suite. Jako partner, który uczestniczy w programie dostawcy rozwiązań w chmurze, można oczekiwać, że priorytet ma czas odpowiedzi na główne problemy.

Obsługa własnej dzierżawy partnerskiej nie jest uwzględniona w ramach korzyści z pomocy technicznej dostawcy usług kryptograficznych. Jednak pakiety Office 365, Microsoft Dynamics CRM Online i Enterprise Mobility Suite nie naliczają odrębnej opłaty za subskrypcję pomocy technicznej dla partnerów lub klientów. Na platformie Azure jest naliczana opłata, ale jeśli masz uprawnienia do pomocy technicznej w chmurze lub innych korzyściach związanych z Microsoft Partner Network (MPN), możesz użyć ich do płacenia tej opłaty.

Ta korzyść ma zastosowanie do wszystkich partnerów uczestniczących w programie dostawcy rozwiązań w chmurze, bez względu na to, czy jest płatny, czy w okresie próbnym. Pomoc dotycząca rozliczeń i subskrypcji jest również dostępna jako bezpłatny składnik tego pakietu.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Jak szybko uzyskamy wstępną odpowiedź?

Początkowe czasy reakcji zależą od ważności przesłanego zdarzenia. Ważność problemu jest określana przez wskazanie wpływu na działalność biznesową podczas przesyłania żądania obsługi.

Czas wstępnej reakcji dla **zdarzeń naprawy awarii technicznej**:

- Krytyczny wpływ (ważność A): dwie godziny (znacząca utrata lub spadek poziomu usług). Usługi produkcyjne)
- Średni wpływ (ważność B): cztery godziny (średnia utrata lub spadek poziomu usług). Usługi produkcyjne częściowo dotknięte problemem).
- Minimalny wpływ (ważność C): osiem godzin (minimalna utrata lub spadek poziomu usług). Usługi są nadal dostępne lub nie zostały uwzględnione.

Czasy wstępnej reakcji są przeznaczone wyłącznie dla pomocy technicznej w języku angielskim. Obsługa języka lokalnego jest dostępna w godzinach pracy.
W przypadku incydentów, które znajdują się w granicach uprawnień do świadczenia pomocy technicznej, ale nie są uważane za zdarzenia związane z uszkodzeniem, czas wstępnej reakcji może należeć do jednego dnia roboczego.

### <a name="can-i-submit-a-service-request-by-phone"></a>Czy mogę przesłać żądanie obsługi przez telefon?

Nie, pomoc techniczna dla telefonów nie jest oferowana dla tego programu.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Co się stanie w przypadku zalogowania się do Azure Portal i obejścia Centrum partnerskiego?

Jeśli zalogujesz się do Microsoft Azure Portal bezpośrednio, zobaczysz centrum w swoim kontekście, a nie kontekst klienta. Dlatego należy zalogować się bezpośrednio do Microsoft Azure Portal podczas tworzenia żądania obsługi dla własnych subskrypcji.

Uprawnienie do obsługi programu CSP nie zapewnia pomocy technicznej w ramach Twojej subskrypcji partnerskiej. W związku z tym należy podać ważne uprawnienie do planu pomocy technicznej podczas tworzenia żądania obsługi, które dotyczy własnej subskrypcji partnera. Przykłady obejmują identyfikator kontraktu MPN, Premier lub plan pomocy technicznej systemu Azure. Aby uzyskać więcej informacji, zobacz [często zadawane pytania dotyczące pomocy technicznej platformy Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Co się stanie, jeśli zaloguję się do portalu Centrum administracyjnego pakietu Office 365 i obejść centrum partnerskie?

Jeśli zalogujesz się bezpośrednio do centrum administracyjnego pakietu Office 365, zobaczysz centrum w swoim kontekście, a nie kontekst klienta. Dlatego należy podpisać go bezpośrednio w centrum administracyjnym pakietu Office 365 podczas tworzenia żądania obsługi dla własnych subskrypcji.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Jak mogę uzyskać dodatkową pomoc techniczną dla systemu Dynamics 365?

Jeśli występują problemy związane z usługą: Dynamics 365 planowanie subskrypcji, licencjonowania, rozliczeń, finansów & operacji, licencji produktu Dynamics 365 lub potrzebujesz dalszej pomocy technicznej:
 
Skontaktuj się z [pomocą techniczną systemu Dynamics](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Następne kroki

- [Zapewnianie pomocy technicznej dla klientów](customer-support.md)
- [Sprawdzanie kondycji usługi](check-service-health.md)
