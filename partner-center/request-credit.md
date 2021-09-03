---
title: Żądanie środków od firmy Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Poznaj korzyści, ograniczenia i procedury związane z żądaniem od firmy Microsoft środków w umowie dotyczącej poziomu usług (SLA), jeśli klienci wystąpią w przypadku usterek usługi.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 51c5b896564e7eb915814c43a6931e48f1777ffc
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/03/2021
ms.locfileid: "123457960"
---
# <a name="how-and-when-to-request-a-credit-from-microsoft"></a>Jak i kiedy zażądać środków od firmy Microsoft

**Odpowiednie role:** Agent administracyjny | Administrator globalny

Możesz zażądać od firmy Microsoft środków w umowie dotyczącej poziomu usług **(SLA),** jeśli w usłudze, która jest udostępniana klientom, ma ona erudycyjną pracę.

## <a name="sla-credit-calculation"></a>Obliczanie środków w umowach SLA

Środki firmy Microsoft na umowy SLA są określane na podstawie usług, których to miało wpływ. Jeśli na przykład klient ma pakiet Office 365, ale wystąpiła tylko SharePoint, kredyt sla jest zatwierdzany tylko dla SharePoint, a nie całego planu klienta.

*Środki są proporcjonalnie oceniane na podstawie usługi, na która ma to wpływ, oraz czasu trwania 3000 000 000 000 000 000 000 000 000 000* Aby wyświetlić typy scenariuszy, które kwalifikują się do środków w umowy SLA, zobacz dokument [Online Services Consolidated SLA (Skonsolidowana umowa SLA usług online).](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Te informacje dotyczą również usług sprzedawanych za pośrednictwem programu Dostawca rozwiązań w chmurze (CSP).


## <a name="request-an-sla-credit"></a>Żądanie środków w umowach SLA

*Partner CSP musi przesłać roszczenie i wszystkie wymagane informacje do końca miesiąca kalendarzowego następującego po miesiącu, w którym wystąpiło zdarzenie.* Na przykład jeśli zdarzenie miało miejsce 15 lutego, firma Microsoft musi otrzymać roszczenie i wszystkie wymagane informacje do 31 marca. Klienci końcowi i odsprzedawcy pośredni nie mogą przesyłać roszczeń kredytowych w ramach umowy SLA; Dostawca pośredni lub bezpośredni partner na rachunku musi przesłać roszczenia w ich imieniu.

> [!NOTE]
> Zdarzenia doradcze zazwyczaj nie kwalifikują się do środków w umowach SLA. Zdarzenie opublikowane na pulpicie nawigacyjnym usługi Service Health  wskazuje, że może to mieć wpływ na dzierżawę i reprezentuje najlepsze informacje, które firma Microsoft ma w czasie publikowania. Dane strony kondycji reprezentują ogólną dostępność usługi. Wpływ poszczególnych usług, środki zaradcze i rozwiązania mogą się różnić. Aby uzyskać więcej informacji, możesz przejrzeć końcowy przegląd zdarzenia po zdarzeniu i po zdarzeniu. Aby [uzyskać więcej informacji, zobacz Jak Microsoft 365](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) kondycji usługi.

### <a name="required-information"></a>Wymagane informacje

Nazwa klienta, identyfikator dzierżawy, numer biletu partnera i sygnatura czasowa utworzenia biletu nie są wystarczające do przetworzenia oświadczenia.

Przed [przesłaniem żądania środków w umowy](#submit-sla-credit-request)  SLA do firmy Microsoft należy zebrać wszystkie następujące informacje, które mają zostać zawarte w bilecie pomocy technicznej:

- Identyfikator GUID dzierżawy klienta
- Identyfikator [zdarzenia outage](#outage-incident-identifier)?
- Dowód na to, że na klienta miała wpływ owa niepamięć i zażądano środków w umowach SLA.
- Czy subskrypcje, których to miało wpływ, zostały zakupione za pośrednictwem CSP? *(tak* lub *nie)*

#### <a name="evidence-that-proves-customer-impact"></a>Dowód, który potwierdza wpływ na klienta

- Informacje dotyczące czasu i czasu przestoju
- Liczba i lokalizacje użytkowników, których dotyczy problem (jeśli dotyczy)
- Opisy prób rozwiązania zdarzenia w momencie wystąpienia zdarzenia
- Wiadomość e-mail od klienta, na który ma to wpływ, z prośbą o pomoc techniczną, a następnie z żądaniem środków
- Numer biletu pomocy technicznej i szczegóły kontaktu z klientem w odniesieniu do rozwiązywania problemów związanych z usługą


#### <a name="outage-incident-identifier"></a>Identyfikator zdarzenia 3D

Identyfikator zdarzenia outage można znaleźć na stronie **Service Health** w centrum administracyjne platformy Microsoft 365. Identyfikator **zdarzenia 3D** jest liczbą poprzedzoną dwuliterowy skrót, który wskazuje usługi, których dotyczy (na przykład *EX25194* dla Exchange Online ścieki). W poniższej tabeli opisano typowe skróty usług:

| Dwuliterowy skrót | Usługa firmy Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype dla firm Online (wcześniej Lync Online) |
| System operacyjny | Office Subskrypcji |
| PB | Usługa Power BI dla Office 365 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Błąd portalu |

### <a name="submit-sla-credit-request"></a>Przesyłanie żądania środków w umowy SLA

Aby przesłać żądanie środków w ramach umowy SLA do firmy Microsoft za pośrednictwem Partner Center nawigacyjnego:

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.
2. W menu po lewej stronie wybierz pozycję **Żądania obsługi,** a następnie wybierz **pozycję Żądania pomocy technicznej dla partnerów.**
3. Na stronie **Żądanie partnera** wybierz pozycję **Nowe żądanie.**
4. Na stronie **Uruchamianie żądania** znajdź sekcję **CSP — customers, orders and subscriptions (CSP — klienci, zamówienia i subskrypcje).** W tej sekcji wybierz pozycję **Wybierz typ problemu, a** następnie wybierz pozycję Żądania środków na usługi **klienta.**
5. Na stronie **Zalecane rozwiązania** w obszarze Czy potrzebujesz **więcej pomocy?** wybierz **pozycję Tak.**
6. Na stronie **Szczegóły** wypełnij sekcję **Szczegóły** problemu. W polu **tekstowym** Szczegóły wprowadź [](#required-information) zebrane wcześniej wymagane informacje.
7. Wybierz **pozycję Prześlij,** aby wysłać żądanie środków w umowy SLA.

## <a name="next-steps"></a>Następne kroki

- [Zgłaszanie problemów w imieniu klienta](report-problems-on-behalf-of-a-customer.md)
