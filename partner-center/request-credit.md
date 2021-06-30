---
title: Request an SLA credit from Microsoft (Żądanie kredytu SLA od firmy Microsoft)
ms.topic: article
ms.date: 03/31/2021
description: Poznaj korzyści, ograniczenia i procedury związane z żądaniem od firmy Microsoft środków w umowie dotyczącej poziomu usług (SLA), jeśli klienci wystąpią w przypadku 355 000 000 000 000 000 000 000 000 000 000 000 000 000 000 00
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: f521e55869d60987fb46cd5d570bf206939e0782
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080643"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Jak i kiedy zażądać środków z umowy dotyczącej poziomu usług (SLA) od firmy Microsoft

**Odpowiednie role:** Agent administracyjny | Administrator globalny

Możesz zażądać od firmy Microsoft środków w umowie dotyczącej poziomu usług **(SLA),** jeśli w usłudze, która jest udostępniana klientom, nie będzie można jej użyć.

## <a name="sla-credit-calculation"></a>Obliczanie środków w umowach SLA

Środki na umowy SLA od firmy Microsoft są określane na podstawie usług, których to miało wpływ. Jeśli na przykład klient ma pakiet usługi Office 365, ale wystąpiła tylko przeoowa w programie SharePoint, punkty umowy SLA są zatwierdzane tylko dla programu SharePoint, a nie całego planu klienta.

*Środki są proporcjonalnie oceniane na podstawie usługi, na która ma to wpływ, oraz czasu trwania 3000 000 000 000 000 000 000 000 000 000* Aby wyświetlić typy scenariuszy, które kwalifikują się do środków w umowy SLA, zobacz dokument [Online Services Consolidated SLA (Skonsolidowana umowa SLA usług online).](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Te informacje dotyczą również usług sprzedawanych za pośrednictwem programu Dostawca rozwiązań w chmurze (CSP).


## <a name="request-an-sla-credit"></a>Żądanie środków w umowach SLA

*Partner CSP musi przesłać roszczenie i wszystkie wymagane informacje do końca miesiąca kalendarzowego następującego po miesiącu, w którym wystąpiło zdarzenie.* Na przykład jeśli zdarzenie miało miejsce 15 lutego, firma Microsoft musi otrzymać roszczenie i wszystkie wymagane informacje do 31 marca. Klienci końcowi i odsprzedawcy pośredni nie mogą przesyłać roszczeń kredytowych w ramach umowy SLA; Dostawca pośredni lub bezpośredni partner na rachunku musi przesłać roszczenia w ich imieniu.

> [!NOTE]
> Zdarzenia doradcze nie kwalifikują się do środków w umowach SLA. Zdarzenie opublikowane na pulpicie nawigacyjnym usługi Service Health  wskazuje, że może to mieć wpływ na dzierżawę i reprezentuje najlepsze informacje, które firma Microsoft ma w czasie publikowania. Dane strony kondycji reprezentują ogólną dostępność usługi. Wpływ poszczególnych usług, środki zaradcze i rozwiązania mogą się różnić. Aby uzyskać więcej informacji, możesz zapoznać się z końcowymi informacjami na temat zdarzenia po zdarzeniu i przeglądu po zdarzeniu. Zobacz [Jak sprawdzić kondycję Microsoft 365,](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) aby uzyskać więcej informacji.

### <a name="required-information"></a>Wymagane informacje

Nazwa klienta, identyfikator dzierżawy, numer biletu partnera i sygnatura czasowa utworzenia biletu nie są wystarczające do przetworzenia oświadczenia.

Przed [przesłaniem żądania środków w umowy](#submit-sla-credit-request)  SLA do firmy Microsoft należy zebrać wszystkie następujące informacje, które mają zostać zawarte w bilecie pomocy technicznej:

- Identyfikator GUID dzierżawy klienta
- Identyfikator [zdarzenia outage](#outage-incident-identifier)?
- Dowód na to, że błąd miał wpływ na klienta i zażądał środków w umowach SLA.
- Czy subskrypcje, których to miało wpływ, zostały zakupione za pośrednictwem CSP? *(tak* lub *nie)*

#### <a name="evidence-that-proves-customer-impact"></a>Dowód, który potwierdza wpływ na klientów

- Informacje dotyczące czasu i czasu przestoju
- Liczba i lokalizacje użytkowników, których dotyczy problem (jeśli dotyczy)
- Opisy prób rozwiązania zdarzenia w momencie wystąpienia zdarzenia
- Wiadomość e-mail od klienta, na który ma to wpływ, z prośbą o pomoc techniczną, a następnie z żądaniem środków
- Numer biletu pomocy technicznej i szczegóły kontaktu z klientem w odniesieniu do rozwiązywania problemów związanych z usługą


#### <a name="outage-incident-identifier"></a>Identyfikator zdarzenia 3D

Identyfikator zdarzenia outage można znaleźć na stronie **Service Health** w centrum administracyjne platformy Microsoft 365. Identyfikator zdarzenia 3.0 to liczba poprzedzona dwuliterową skrótem, która wskazuje usługę, na przykład *EX25194* w przypadku 3000 000 000 000 000 000 000 000 000 000 000 000 000 000 000 000 000 000 0000 000 000  W poniższej tabeli opisano typowe skróty usług:

| Dwuliterowy skrót | Usługa firmy Microsoft |
| ----------------------- | ----------------- |
| Ex | Exchange Online |
| Fo | Exchange Online Protection |
| Sb | Skype dla firm Online (wcześniej Lync Online) |
| System operacyjny | Subskrypcja pakietu Office |
| PB | Usługa Power BI dla Office 365 |
| Sp | SharePoint Online |
| Ya | Yammer Enterprise |
| MO | Błąd portalu |

### <a name="submit-sla-credit-request"></a>Przesyłanie żądania środków w umowy SLA

Aby przesłać żądanie środków w ramach umowy SLA do firmy Microsoft za pośrednictwem Partner Center nawigacyjnego:

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.
2. W menu po lewej stronie wybierz pozycję **Żądania obsługi,** a następnie wybierz **pozycję Żądania pomocy technicznej dla partnerów.**
3. Na stronie **Żądanie partnera** wybierz pozycję **Nowe żądanie.**
4. Na stronie **Uruchamianie żądania** znajdź sekcję **CSP — customers, orders and subscriptions (CSP — klienci, zamówienia i subskrypcje).** W tej sekcji wybierz pozycję **Wybierz typ problemu, a** następnie wybierz pozycję Żądania środków na usługi **klienta.**
5. Na stronie **Zalecane rozwiązania** w obszarze Czy potrzebujesz **więcej pomocy?** wybierz pozycję **Tak.**
6. Na stronie **Szczegóły** wypełnij **sekcję Szczegóły** problemu. W polu **tekstowym** Szczegóły wprowadź [](#required-information) zebrane wcześniej wymagane informacje.
7. Wybierz **pozycję Prześlij,** aby wysłać żądanie środków w umowy SLA.

## <a name="next-steps"></a>Następne kroki

- [Zgłaszanie problemów w imieniu klienta](report-problems-on-behalf-of-a-customer.md)
