---
title: Raport o stanie wymagań dotyczących zabezpieczeń
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Dowiedz się, jak sprawdzić zgodność wymagań dotyczących zabezpieczeń z raportem o stanie wymagań dotyczących zabezpieczeń i raportem Partner Center MFA
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 15e2792a38f8fc90612282ff30ad57dc320fc96a
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959314"
---
# <a name="security-requirements-status-report"></a>Raport o stanie wymagań dotyczących zabezpieczeń

**Odpowiednie role:** administrator CPV | Administrator globalny

W tym artykule wyjaśniono raport o stanie wymagań dotyczących zabezpieczeń w Partner Center. Ten raport zawiera metryki dotyczące zgodności z wymaganiami [partnerów](partner-security-requirements.md) w zakresie uwierzytelniania wieloskładnikowego (MFA) dla użytkowników w dzierżawie partnera.

Aby uzyskać dostęp do tego raportu [w Partner Center](https://partner.microsoft.com/dashboard), przejdź do **Ustawienia**  >  **Ustawienia konta** Stan wymagań  >  **zabezpieczeń.** Raport jest aktualizowany codziennie i odzwierciedla dane logowania z ostatnich siedmiu dni.

>[!NOTE]
>Raport o stanie wymagań dotyczących zabezpieczeń jest obsługiwany tylko w Partner Center. Nie jest ona dostępna w witrynie Microsoft Cloud for US Government Microsoft Cloud w Niemczech. Zdecydowanie zalecamy, aby wszyscy partnerzy w ramach transakcji za pośrednictwem suwerennej chmury (rząd USA i Niemcy) natychmiast przyjmowały te nowe wymagania dotyczące zabezpieczeń. Jednak obecnie ci partnerzy nie muszą spełniać nowych wymagań dotyczących zabezpieczeń. Firma Microsoft udostępni dodatkowe szczegóły dotyczące wymuszania tych wymagań dotyczących zabezpieczeń suwerennych chmur w przyszłości.

## <a name="security-status-metrics"></a>Metryki stanu zabezpieczeń

Raport o stanie wymagań dotyczących zabezpieczeń oferuje wgląd w implementację usługi MFA partnera oraz metryki dotyczące konfiguracji usługi MFA i Partner Center działań w dzierżawach partnerów. W poniższych sekcjach opisano te metryki bardziej szczegółowo.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Konfiguracja usługi MFA w dzierżawie partnera

Metryka **Procent włączonych** kont użytkowników z usługą MFA wymuszonych przy użyciu opcji wymienionych tutaj: przedstawia wartość procentową włączonych kont użytkowników w dzierżawie partnera, które mają wymuszone uwierzytelniania wieloskładnikowego. Aby uzyskać zgodność, [](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) można użyć jednej z tych opcji uwierzytelniania wieloskładnikowego. Te dane są przechwytywane i raportowane codziennie. Na przykład:

- Firma Contoso jest partnerem CSP z 110 kontami użytkowników w dzierżawie. 10 z nich jest wyłączonych. 
- Z pozostałych 100 kont użytkowników 90 jest wymuszanych przy użyciu dostarczonych [opcji uwierzytelniania wieloskładnikowego.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) W związku z tym metryka pokazuje 90%. 

### <a name="partner-center-requests-with-mfa"></a>Partner Center żądania za pomocą usługi MFA

Za każdym razem, gdy pracownicy logują się do Partner Center pracy lub za pośrednictwem interfejsów API, odbierają lub wysyłają dane za pośrednictwem Partner Center, ich stan zabezpieczeń jest zakwestionowany i śledzony. Śledzenie stanu zabezpieczeń obejmuje również aplikacje i wszelkie aplikacje dostawcy panelu sterowania. Te dane są wyświetlane w metrykach w obszarze **Procent** żądań do Partner Center z uwierzytelniania wieloskładnikowego i odzwierciedlają ostatnie siedem dni.

#### <a name="dashboard-mfa-verification"></a>Weryfikacja uwierzytelniania wieloskładnikowego pulpitu nawigacyjnego

Metryka **Za pośrednictwem Partner Center portal jest** powiązana z działaniami w ramach Partner Center nawigacyjnego. Mierzy ona procent operacji wykonywanych przez użytkowników, którzy ukończyli weryfikację uwierzytelniania wieloskładnikowego. Na przykład:

- Firma Contoso jest partnerem programu CSP z dwoma agentami administracyjnymi, Jane i John.
- Pierwszego dnia Magda zalogowała się do pulpitu nawigacyjnego Partner Center bez weryfikacji uwierzytelniania wieloskładnikowego i dokonała trzech operacji.
- Drugiego dnia Jan zalogował się do pulpitu nawigacyjnego Partner Center bez weryfikacji uwierzytelniania wieloskładnikowego i dokonał pięciu operacji.
- Trzeciego dnia Magda zalogowała się do pulpitu Partner Center z weryfikacją uwierzytelniania wieloskładnikowego i dokonała dwóch operacji.
- W ciągu ostatnich czterech dni nie zostały wykonane żadne operacje wykonane przez żadnego z agentów.
- Z 10 operacji wykonanych w 7-dniowym oknie użytkownik z weryfikacją MFA dokonał dwóch operacji. W związku z tym metryka pokazuje 20%.

Użyj żądań  portalu plików bez uwierzytelniania wieloskładnikowego, aby zrozumieć, który użytkownik zalogował się na pulpicie nawigacyjnym usługi Partner Center bez weryfikacji uwierzytelniania WIELOSKŁADNIKowego, oraz czas ostatniej wizyty w oknie raportowania.

#### <a name="appuser-mfa-verification"></a>Weryfikacja uwierzytelniania wieloskładnikowego aplikacji i użytkownika

Metryka **Za pośrednictwem interfejsu API lub zestawu SDK** jest powiązana z uwierzytelnianiem aplikacji i użytkownika za pośrednictwem Partner Center API. Mierzy on procent żądań interfejsu API wykonanych przy użyciu tokenu dostępu z oświadczeniem MFA. Na przykład:

- Firma Fabrikam jest partnerem CSP i ma aplikację CSP, która używa kombinacji metod uwierzytelniania App+User i uwierzytelniania tylko dla aplikacji.
- Pierwszego dnia aplikacja zażądała trzech żądań interfejsu API, które zostały pozyskane za pomocą tokenu dostępu uzyskanego za pośrednictwem metody uwierzytelniania App+User bez weryfikacji mfa.
- Drugiego dnia aplikacja zażądała pięciu żądań interfejsu API, które zostały pozyskane przy użyciu tokenu dostępu uzyskanego przy użyciu uwierzytelniania tylko aplikacji.
- Trzeciego dnia aplikacja przesłała dwa żądania interfejsu API, których kopię zapasową stanowi token dostępu uzyskany przy użyciu metody uwierzytelniania App+User z weryfikacją MFA.
- W ciągu ostatnich czterech dni nie zostały wykonane żadne operacje wykonane przez żadnego z agentów.
- Pięć żądań interfejsu API drugiego dnia, które zostały pozyskane przez token dostępu uzyskany za pośrednictwem uwierzytelniania tylko dla aplikacji, zostanie pominiętych w metryce, ponieważ nie korzysta z poświadczeń użytkownika. Z pozostałych pięciu operacji dwie z nich zostały pozyskane przy użyciu tokenu dostępu uzyskanego podczas weryfikacji MFA. W związku z tym metryka pokazuje 40%.

Jeśli chcesz zrozumieć, które działania związane z aplikacją i użytkownikiem skutkują nie 100% dla tej metryki, użyj plików:

- **Podsumowanie żądań interfejsu API** w celu zrozumienia ogólnego stanu usługi MFA według aplikacji.
- **Wszystkie żądania interfejsu API** służące do zrozumienia szczegółów poszczególnych żądań interfejsu API poszczególnych użytkowników dzierżawy, wynik jest ograniczony do maksymalnie 10 000 najnowszych żądań w celu lepszego pobierania.

## <a name="actions-for-mfa-status-below-100"></a>Akcje dotyczące stanu usługi MFA poniżej 100%

Niektórzy partnerzy, którzy zaimplementowali uwierzytelniania wieloskładnikowego, mogą zobaczyć metryki raportów poniżej 100%. Aby zrozumieć, dlaczego, należy wziąć pod uwagę kilka czynników.

> [!NOTE]
> Musisz współpracować z osobami z twojej organizacji, które znają zarządzanie tożsamościami i implementację uwierzytelniania wieloskładnikowego dla dzierżawy partnera.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Zaimplementowano uwierzytelniania wieloskładnikowego dla dzierżawy partnera

Aby zapewnić zgodność, należy zaimplementować uwierzytelniania wieloskładnikowego dla dzierżawy partnera. Aby uzyskać szczegółowe informacje na temat implementowania uwierzytelniania wieloskładnikowego, zobacz Security [requirements for using Partner Center or Partner Center APIs](partner-security-requirements.md)(Wymagania dotyczące zabezpieczeń Partner Center lub Partner Center API).

>[!NOTE]
> Metryki usługi MFA są obliczane codziennie i uwzględniane są operacje wykonywane w ciągu ostatnich siedmiu dni. Jeśli niedawno ukończono implementację usługi MFA dla dzierżawy partnera, metryki mogą jeszcze nie pokazywać 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Weryfikowanie uwierzytelniania wieloskładnikowego na wszystkich kontach użytkowników

Dowiedz się, czy bieżąca implementacja usługi MFA obejmuje wszystkie konta użytkowników, czy tylko niektóre z nich. Niektóre rozwiązania uwierzytelniania wieloskładnikowego są oparte na zasadach i obsługują wykluczanie użytkowników, podczas gdy inne mogą wymagać jawnego włączenia uwierzytelniania wieloskładnikowego dla każdego użytkownika. Sprawdź, czy nie wykluczono żadnego użytkownika z bieżącej implementacji usługi MFA. Każde konto użytkownika, które jest wykluczone i loguje się do usługi Partner Center, aby wykonać dowolną aktywność związaną z CSP-, CPV-lub Advisor, może spowodować, że metryki nie będą w 100%.

### <a name="review-your-mfa-conditions"></a>Przeglądanie warunków uwierzytelniania wieloskładnikowego

Dowiedz się, czy bieżąca implementacja wymusza uwierzytelniania wieloskładnikowego tylko w określonych warunkach. Niektóre rozwiązania MFA zapewniają elastyczność wymuszania uwierzytelniania wieloskładnikowego tylko wtedy, gdy zostaną spełnione określone warunki. Na przykład użytkownik uzyskuje dostęp z nieznanego urządzenia lub nieznanej lokalizacji. Użytkownik, który ma włączoną usługę MFA, ale nie jest wymagany do ukończenia weryfikacji MFA podczas uzyskiwania dostępu do usługi Partner Center, może spowodować, że metryki nie będą w 100%.

>[!NOTE]
>W przypadku partnerów, którzy zaimplementowali uwierzytelnianie wieloskładnikowe przy użyciu ustawień domyślnych zabezpieczeń usługi Azure AD, należy pamiętać, że w przypadku kont użytkowników niebędących administratorami uwierzytelnianie wieloskładnikowe będzie wymuszane na podstawie ryzyka. Użytkownicy będą monitować o uwierzytelniania wieloskładnikowego tylko podczas ryzykownych prób logowania (na przykład użytkownik loguje się z innej lokalizacji). Ponadto użytkownicy będą mieć do 14 dni na zarejestrowanie się w celu uwierzytelniania wieloskładnikowego. Użytkownicy, którzy nie ukończyli rejestracji usługi MFA, nie będą mieli uwierzytelniania MFA w ciągu 14-dniowego okresu. W związku z tym oczekuje się, że metryki mogą nie być w 100% dla partnerów, którzy zaimplementowali usługę MFA przy użyciu ustawień domyślnych zabezpieczeń usługi Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Przeglądanie konfiguracji usługi MFA innych firm

Jeśli używasz rozwiązania mfa innej firmy, zidentyfikuj sposób integrowania go z usługą Azure AD. Ogólnie rzecz biorąc, istnieją dwie metody, w tym kontrolki federacji i niestandardowe:

* **Federacja tożsamości** — gdy usługa Azure AD odbierze żądanie uwierzytelnienia, usługa Azure AD przekieruje użytkownika do dostawcy tożsamości federacji w celu uwierzytelnienia. Po pomyślnym uwierzytelnieniu dostawca tożsamości federacji przekieruje użytkownika z powrotem do usługi Azure AD wraz z tokenem SAML. Aby usługa Azure AD rozpoznała, że użytkownik zakończył weryfikację MFA podczas uwierzytelniania u dostawcy tożsamości federskiej, token SAML musi zawierać oświadczenie *authenticationmethodsreferences* (z wartością *multipleauthn*). Sprawdź, czy dostawca tożsamości federacji obsługuje wystawianie takiego oświadczenia. Jeśli tak, sprawdź, czy dostawca tożsamości federacji został do tego skonfigurowany. W przypadku braku oświadczenia usługa Azure AD (Partner Center) nie będzie wiedzieć, że użytkownik zakończył weryfikację uwierzytelniania wieloskładnikowego i brak oświadczenia może spowodować, że metryka nie będzie w 100%.

* **Kontrolka niestandardowa** — kontrolki niestandardowej usługi Azure AD nie można użyć do określenia, czy użytkownik zakończył weryfikację uwierzytelniania wieloskładnikowego za pośrednictwem rozwiązania mfa innej firmy. W związku z tym każdy użytkownik, który ukończył weryfikację MFA za pomocą kontrolki niestandardowej, będzie zawsze wyświetlany w usłudze Azure AD (i z kolei Partner Center) jako bez ukończenia weryfikacji MFA. Jeśli to możliwe, zaleca się przejście na federację tożsamości w przeciwieństwie do kontroli niestandardowej podczas integracji z usługą Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Określanie, którzy użytkownicy zalogowali się do usługi Partner Center bez uwierzytelniania wieloskładnikowego

Pomocne może być zidentyfikowanie użytkowników, którzy logują się do usługi Partner Center bez weryfikacji uwierzytelniania wieloskładnikowego, i zweryfikowanie ich pod względem bieżącej implementacji usługi MFA. Możesz użyć raportu [logowania usługi Azure AD,](/azure/active-directory/reports-monitoring/concept-sign-ins) aby dowiedzieć się, czy użytkownik zakończył weryfikację uwierzytelniania wieloskładnikowego. Raport logowania usługi Azure AD jest obecnie dostępny tylko dla partnerów, którzy zasubskrybowali usługę Azure AD — wersja Premium lub dowolną usługę O365 SKU, w tym Azure AD — wersja Premium (na przykład EMS).

## <a name="next-steps"></a>Następne kroki

- [Partner Center grupy wskazówek dotyczących zabezpieczeń](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Wymagania dotyczące zabezpieczeń Centrum partnerskiego](partner-security-requirements.md)
- [Partner Center — często zadawane pytania dotyczące wymagań dotyczących zabezpieczeń](partner-security-requirements-faq.yml)
