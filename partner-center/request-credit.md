---
title: Request an SLA credit from Microsoft (Żądanie kredytu SLA od firmy Microsoft)
ms.topic: article
ms.date: 04/28/2020
description: Zapoznaj się z korzyściami, ograniczeniami i procedurami, aby zażądać środków w ramach umowy dotyczącej poziomu usług (SLA) firmy Microsoft, jeśli klienci napotykają awarię usługi.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/14/2020
ms.locfileid: "92529224"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Jak i kiedy należy zażądać kredytu dla umowy dotyczącej poziomu usług (SLA) firmy Microsoft

Możesz zażądać kredytów z **umowy dotyczącej poziomu usług (SLA)** firmy Microsoft, jeśli usługa oferowana klientom ma awarię.

## <a name="sla-credit-calculation"></a>Obliczanie środków SLA

Kredyty SLA od firmy Microsoft są określane na podstawie tego, które usługi miały wpływ. Na przykład jeśli klient ma pakiet Office 365, ale tylko wystąpił przestój programu SharePoint, środki SLA są zatwierdzane wyłącznie dla programu SharePoint, a nie całego planu.

*Kredyty są oceniane proporcjonalnie do liczby zaatakowanych usług oraz czasu trwania przestojów.* Aby zobaczyć typy scenariuszy, które kwalifikują się do kredytów SLA, zobacz [dokument skonsolidowanej umowy SLA usług Online Services](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Te informacje dotyczą również usług sprzedawanych za pomocą programu dostawcy rozwiązań w chmurze.

## <a name="request-an-sla-credit"></a>Żądaj środków umowy SLA

*Partner dostawcy rozwiązań w chmurze musi przesłać żądanie i wszystkie wymagane informacje do końca miesiąca kalendarzowego następującego po miesiącu, w którym wystąpiło zdarzenie.* Na przykład jeśli zdarzenie wystąpiło 15 lutego, firma Microsoft musi odebrać to żądanie i wszystkie wymagane informacje do 31 marca. Klienci końcowi i pośrednii odsprzedawcy nie mogą przesyłać roszczeń z tytułu umów SLA. Dostawca pośredni lub bezpośredni partner Bill muszą przesłać oświadczenia w ich imieniu.

### <a name="required-information"></a>Wymagane informacje

Przed [przesłaniem żądania kredytowego umowy SLA](#submit-sla-credit-request) do firmy Microsoft należy zebrać następujące informacje, które mają zostać dołączone do biletu pomocy technicznej:

- Identyfikator GUID dzierżawy klienta
- [Identyfikator zdarzenia przestoju](#outage-incident-identifier)?
- Czy objęte subskrypcje są zakupione w ramach dostawcy CSP? (*tak* lub *nie*)

#### <a name="outage-incident-identifier"></a>Identyfikator zdarzenia przestoju

Identyfikator zdarzenia przestoju można znaleźć na stronie **Service Health** w centrum administracyjnym Microsoft 365. **Identyfikator zdarzenia przestoju** jest numerem poprzedzonym dwuliterowym skrótem wskazującym usługę, której dotyczy problem (na przykład *EX25194* w przypadku awarii usługi Exchange Online). W poniższej tabeli opisano typowe skróty usługi:

| Dwuliterowy skrót | Usługa firmy Microsoft |
| ----------------------- | ----------------- |
| UPRZEDNI | Exchange Online |
| CZCIONKI | Ochrona usługi Exchange Online |
| SB | Skype dla firm Online (dawniej Lync online) |
| System operacyjny | Subskrypcja pakietu Office |
| PB | Usługa Power BI dla Office 365 |
| REQUIREMENT | SharePoint Online |
| YA | Usługa Yammer Enterprise |
| MO | Błąd portalu |

### <a name="submit-sla-credit-request"></a>Prześlij żądanie kredytowe w umowie SLA

Aby przesłać żądanie kredytowe dotyczące umowy SLA do firmy Microsoft za pomocą pulpitu nawigacyjnego Centrum partnerskiego:

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.
2. W menu po lewej stronie wybierz pozycję **żądania obsługi**, a następnie wybierz pozycję **żądania obsługi partnerów**.
3. Na stronie **żądanie partnera** wybierz pozycję **nowe żądanie**.
4. Na stronie **Uruchamianie żądania** Znajdź sekcję **CSP — Customers, zamówienia i subskrypcje**. W tej sekcji Wybierz **pozycję Wybierz typ problemu**, a następnie wybierz pozycję **usługi klienta żądania kredytowe**.
5. Na stronie **zalecane rozwiązania** w obszarze **czy potrzebujesz więcej pomocy?** wybierz opcję **tak**.
6. Na stronie **szczegóły** Wypełnij sekcję **Szczegóły problemu** . W polu tekstowym **szczegóły** Pamiętaj o wprowadzeniu [wymaganych informacji](#required-information) , które zostały zebrane wcześniej.
7. Wybierz pozycję **Prześlij** , aby wysłać żądanie kredytowe w ramach umowy SLA.
