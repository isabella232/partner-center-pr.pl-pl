---
title: Raport stanu wymagań dotyczących zabezpieczeń
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak sprawdzić zgodność wymagań zabezpieczeń z raportem o stanie wymagań zabezpieczeń i raport MFA Centrum partnerskiego
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: d56b9675ea405b29190f68420037ea9a92f3d831
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086553"
---
# <a name="security-requirements-status-report"></a>Raport stanu wymagań dotyczących zabezpieczeń

**Odpowiednie role**
- Administrator CPV
- Administrator globalny

W tym artykule opisano raport o stanie wymagań zabezpieczeń w centrum partnerskim. Ten raport zawiera metryki dotyczące zgodności z [wymaganiami dotyczącymi zabezpieczeń partnerów](partner-security-requirements.md) dla uwierzytelniania wieloskładnikowego (MFA) dla użytkowników w dzierżawie partnera.

Aby uzyskać dostęp do tego raportu w [centrum partnerskim](https://partner.microsoft.com/dashboard), przejdź do pozycji **Ustawienia**  >  **Ustawienia konta**  >  **wymagania dotyczące zabezpieczeń**. Raport jest aktualizowany codziennie i odzwierciedla dane logowania z ostatnich siedmiu dni.

>[!NOTE]
>Raport o stanie wymagań dotyczących zabezpieczeń jest obsługiwany tylko w centrum partnerskim. Nie jest on dostępny w Microsoft Cloud dla instytucji rządowych USA ani Microsoft Cloud Niemiec. Zdecydowanie zalecamy, aby wszyscy partnerzy zajmujący się prowadzeniem działalności w chmurze suwerennej (rząd USA i Niemcy) automatycznie wdrażali te nowe wymagania dotyczące zabezpieczeń. Jednak ci partnerzy nie są obecnie zobowiązani do spełnienia nowych wymagań w zakresie zabezpieczeń. Firma Microsoft zapewni dodatkowe szczegóły dotyczące wymuszania tych wymagań w zakresie bezpieczeństwa dla suwerennych chmur w przyszłości.

## <a name="security-status-metrics"></a>Metryki stanu zabezpieczeń

Raport o stanie wymagań dotyczących zabezpieczeń zawiera szczegółowe informacje dotyczące implementacji usługi MFA partnera i zawiera metryki dotyczące konfiguracji usługi MFA i działań Centrum partnerskiego w dzierżawach partnerów. W poniższych sekcjach opisano te metryki bardziej szczegółowo.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Konfiguracja usługi MFA w dzierżawie partnera

Procent metryk **włączonych kont użytkowników z uwierzytelnianiem MFA przy użyciu opcji wymienionych tutaj:** pokazuje procent włączonych kont użytkowników w dzierżawie partnerskiej z wymuszaniem uwierzytelniania wieloskładnikowego. Aby zapewnić zgodność, można użyć jednej z tych [opcji MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) . Te dane są codziennie przechwytywane i raportowane. Na przykład:

- Firma Contoso to partner dostawcy usług kryptograficznych z 110 kontami użytkowników w dzierżawie. 10 z tych kont użytkownika jest wyłączonych. 
- Poza pozostałymi kontami użytkowników 100, 90 są wymuszane usługi MFA przy użyciu dostarczonych [opcji usługi MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). W związku z tym Metryka pokazuje 90%. 

### <a name="partner-center-requests-with-mfa"></a>Żądania Centrum partnerskiego z usługą MFA

Za każdym razem, gdy pracownicy logują się do Centrum partnerskiego, aby móc korzystać z interfejsów API, uzyskiwać i wysyłać dane za poorednictwem Centrum partnerskiego, ich stan zabezpieczeń jest zakwestionowana i śledzony. W funkcji śledzenia stanu zabezpieczeń są również używane aplikacje i wszystkie aplikacje dostawcy w panelu sterowania. Te dane są wyświetlane w metrykach w obszarze **procent żądań do Centrum partnerskiego z** uwierzytelnianiem MFA i odzwierciedlają ostatnie siedem dni.

#### <a name="dashboard-mfa-verification"></a>Weryfikacja usługi MFA pulpitu nawigacyjnego

Metryka w **portalu Centrum partnerskiego** jest związana z działaniami na pulpicie nawigacyjnym Centrum partnerskiego. Mierzy procent operacji wykonanych przez użytkowników, którzy ukończyli weryfikację MFA. Na przykład:

- Firma Contoso to partner programu CSP z dwoma agentami administratora, Janina i Jan.
- Pierwszego dnia Jan zalogował się do pulpitu nawigacyjnego Centrum partnerskiego bez weryfikacji MFA i wykonał trzy operacje.
- Drugi dzień Jan zalogował się do pulpitu nawigacyjnego Centrum partnerskiego bez weryfikacji MFA i wykonał pięć operacji.
- Trzeci dzień Jan zalogował się do pulpitu nawigacyjnego Centrum partnerskiego z weryfikacją usługi MFA i wykonał dwie operacje.
- Nie wykonano żadnych operacji w żadnym z agentów w pozostałych czterech dniach.
- Z 10 operacji wykonanych w oknie siedmiu dni dwa wystąpienia zostały wykonane przez użytkownika z weryfikacją MFA. W związku z tym Metryka pokazuje 20%.

Aby zrozumieć, który użytkownik zalogował się do pulpitu nawigacyjnego Centrum partnerskiego bez weryfikowania MFA, oraz czas ostatniego odwiedzania w oknie raportowanie, należy użyć **portalu plików bez usługi MFA** .

#### <a name="appuser-mfa-verification"></a>Weryfikacja usługi MFA dla aplikacji i użytkownika

Metryka **za pomocą interfejsu API lub zestawu SDK** jest związana z uwierzytelnianiem aplikacji i użytkownika za pomocą żądań interfejsu API usługi Partner Center. Mierzy procent żądań interfejsu API, które zostały wykonane przy użyciu tokenu dostępu z użyciem żądania MFA. Na przykład:

- Fabrikam to partner programu CSP i ma aplikację dostawcy usług kryptograficznych, która używa kombinacji uwierzytelniania aplikacji i użytkowników oraz metod uwierzytelniania opartych na aplikacji.
- Pierwszego dnia aplikacja wykonał trzy żądania interfejsu API, które były obsługiwane przez token dostępu uzyskany za pomocą metody uwierzytelniania App + User bez weryfikacji MFA.
- Drugi dzień aplikacja wykonał pięć żądań interfejsu API, które były obsługiwane przez token dostępu uzyskany przy użyciu uwierzytelniania tylko aplikacji.
- Trzeci dzień aplikacja wykonał dwa żądania interfejsu API, które były obsługiwane przez token dostępu uzyskany przy użyciu metody uwierzytelniania App + User przy użyciu weryfikacji MFA.
- Nie wykonano żadnych operacji w żadnym z agentów w pozostałych czterech dniach.
- Pięć żądań interfejsu API w drugim dniu, które były obsługiwane przez token dostępu uzyskany za pośrednictwem uwierzytelniania tylko aplikacji, jest pomijany w metryce, ponieważ nie korzysta z poświadczeń użytkownika. W przypadku pozostałych pięciu operacji dla dwóch z nich utworzono token dostępu uzyskany za pomocą weryfikacji MFA. W związku z tym Metryka pokazuje 40%.

Aby zrozumieć, które działania aplikacji + użytkownika mają wynik w przypadku braku 100% tej metryki, Użyj plików:

- **Podsumowanie żądań interfejsu API** w celu zrozumienia ogólnego stanu usługi MFA według aplikacji.
- **Wszystkie żądania interfejsu API** aby zrozumieć szczegóły poszczególnych żądań interfejsu API podejmowanych przez użytkowników dzierżawy, wynik jest ograniczony do maksymalnie 10 000 najnowszych żądań w celu lepszego pobierania.

## <a name="actions-for-mfa-status-below-100"></a>Akcje dotyczące stanu usługi MFA poniżej 100%

Niektórzy partnerzy z zaimplementowaną MFA mogą zobaczyć metryki raportów poniżej 100%. Aby zrozumieć, dlaczego, należy rozważyć kilka czynników.

> [!NOTE]
> Konieczne będzie skontaktowanie się z osobą z organizacji, która zna Zarządzanie tożsamościami i implementację usługi MFA dla dzierżawy partnerskiej.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Zaimplementowana MFA dla dzierżawy partnerskiej

Aby uzyskać zgodność, należy wdrożyć usługę MFA dla dzierżawy partnerskiej. Aby uzyskać szczegółowe informacje na temat implementowania usługi MFA, zobacz [wymagania dotyczące zabezpieczeń w przypadku używania interfejsów API Centrum partnerskiego lub platformy partnerskiej](partner-security-requirements.md).

>[!NOTE]
> Metryki usługi MFA są obliczane codziennie i należy wziąć pod uwagę operacje wykonywane w ciągu ostatnich siedmiu dni. Jeśli niedawno ukończono implementację usługi MFA dla dzierżawcy partnera, metryki nie pokażą jeszcze 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Weryfikowanie usługi MFA na wszystkich kontach użytkowników

Dowiedz się, czy bieżąca implementacja usługi MFA obejmuje wszystkie konta użytkowników, czy tylko niektóre. Niektóre rozwiązania MFA są oparte na zasadach i obsługują wykluczanie użytkowników, podczas gdy inne mogą wymagać jawnego włączenia uwierzytelniania MFA na poszczególnych użytkowników. Sprawdź, czy nie wykluczono żadnego użytkownika z bieżącej implementacji usługi MFA. Wszystkie konta użytkowników, które są wykluczone i logują się do Centrum partnerskiego w celu wykonania dowolnego działania związanego z dostawcą usług kryptograficznych, CPV lub Advisor, mogą spowodować, że metryki nie będą 100%.

### <a name="review-your-mfa-conditions"></a>Przejrzyj warunki uwierzytelniania MFA

Dowiedz się, czy bieżąca implementacja wymusza tylko uwierzytelnianie wieloskładnikowe tylko w określonych warunkach. Niektóre rozwiązania MFA zapewniają elastyczność tylko w przypadku spełnienia określonych warunków. Na przykład użytkownik uzyskuje dostęp z nieznanego urządzenia lub nieznanej lokalizacji. Użytkownik, który włączył usługę MFA, ale nie jest wymagany do ukończenia weryfikacji MFA podczas uzyskiwania dostępu do Centrum partnerskiego, może spowodować, że metryki nie będą 100%.

>[!NOTE]
>W przypadku partnerów, którzy zaimplementowali uwierzytelnianie wieloskładnikowe przy użyciu domyślnych ustawień zabezpieczeń usługi Azure AD, należy pamiętać, że w przypadku kont użytkowników niebędących administratorami będzie wymuszana usługa uwierzytelniania wieloskładnikowego na podstawie ryzyka. Użytkownicy będą monitowani o uwierzytelnianie wieloskładnikowe tylko podczas ryzykownych prób logowania (na przykład użytkownik loguje się z innej lokalizacji). Ponadto użytkownicy będą musieli rejestrować do 14 dni na potrzeby uwierzytelniania wieloskładnikowego. Użytkownicy, którzy nie ukończyli rejestracji usługi MFA, nie będą zarejestrowani przez weryfikację MFA w okresie 14 dni. W związku z tym oczekuje się, że metryki nie mogą być 100% dla partnerów, którzy zaimplementowali uwierzytelnianie wieloskładnikowe przy użyciu domyślnych ustawień zabezpieczeń usługi Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Przejrzyj konfiguracje usługi MFA innych firm

W przypadku korzystania z rozwiązania MFA innej firmy należy określić sposób ich integracji z usługą Azure AD. Ogólnie rzecz biorąc istnieją dwie metody, w tym federacyjne i kontrolki niestandardowe:

* **Tożsamość Federacji** — gdy usługa Azure AD odbierze żądanie uwierzytelnienia, usługa Azure AD przekieruje użytkownika do federacyjnego dostawcy tożsamości w celu uwierzytelnienia. Po pomyślnym uwierzytelnieniu dostawca tożsamości federacyjnej przekierowuje użytkownika z powrotem do usługi Azure AD wraz z tokenem SAML. Aby usługa Azure AD mogła rozpoznać, że użytkownik ukończył weryfikację MFA podczas uwierzytelniania w federacyjnym dostawcy tożsamości, token SAML musi zawierać *authenticationmethodsreferences* (z wartością *multipleauthn*). Sprawdź, czy federacyjny dostawca tożsamości obsługuje wydawanie takiego żądania. Jeśli tak jest, sprawdź, czy federacyjny dostawca tożsamości został skonfigurowany tak, aby to zrobić. W przypadku braku żądania usługa Azure AD (w związku z tym centrum partnerskie) nie wie, że użytkownik ukończył weryfikację MFA i brakuje tego żądania, może to spowodować, że Metryka nie wynosi 100%.

* **Kontrolka niestandardowa** — kontrolka niestandardowa usługi Azure AD nie może służyć do określenia, czy użytkownik ukończył weryfikację MFA za pomocą rozwiązania MFA innej firmy. W związku z tym każdy użytkownik, który ukończył weryfikację MFA za pomocą kontrolki niestandardowej, będzie zawsze wyświetlany w usłudze Azure AD (i w centrum partnerskim) bez ukończonej weryfikacji MFA. Jeśli jest to możliwe, zaleca się przełączenie się do korzystania z federacji tożsamości zamiast kontroli niestandardowej podczas integrowania z usługą Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identyfikowanie użytkowników zalogowanych do Centrum partnerskiego bez usługi MFA

Pomocne może być zidentyfikowanie użytkowników logujących się do Centrum partnerskiego bez weryfikacji MFA i zweryfikowanie ich względem bieżącej implementacji usługi MFA. Możesz użyć [raportu logowania do usługi Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) , aby dowiedzieć się, czy użytkownik ukończył weryfikację uwierzytelniania MFA. Raport logowania w usłudze Azure AD jest obecnie dostępny tylko dla partnerów, którzy subskrybują Azure AD — wersja Premium lub dowolną jednostkę SKU usługi O365, która obejmuje Azure AD — wersja Premium (na przykład EMS).

## <a name="next-steps"></a>Następne kroki

- [Społeczność grupy wskazówek dotyczących zabezpieczeń Centrum partnerskiego](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Wymagania dotyczące zabezpieczeń Centrum partnerskiego](partner-security-requirements.md)
- [Wymagania dotyczące zabezpieczeń Centrum partnerskiego — często zadawane pytania](partner-security-requirements-faq.md)
