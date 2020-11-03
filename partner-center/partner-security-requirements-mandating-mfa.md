---
title: Wymaganie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnerskiej
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak mandat usługi MFA dla dzierżawców partnerskich pomoże Ci zabezpieczyć dostęp do zasobów klientów. Obejmuje przykładowe scenariusze.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b6985054e927dd777d61ae30bd435ab4c6c4ea8c
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133121"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Wymaganie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnerskiej

**Dotyczy**

- Wszyscy partnerzy w programie dostawcy rozwiązań w chmurze
- Wszyscy dostawcy panelu sterowania
- Wszyscy klasyfikatory

**Zmodyfikowane role**

- Agent administracyjny
- Agent sprzedaży
- Agent pomocy technicznej
- Administrator rozliczeń
- Administrator globalny

W tym artykule przedstawiono szczegółowe przykłady i wskazówki dotyczące przyciągania uwierzytelniania wieloskładnikowego (MFA) w centrum partnerskim. Celem tej funkcji jest ułatwienie partnerom bezpiecznego dostępu do zasobów klientów przed naruszeniem poświadczeń. Partnerzy są zobowiązani do wymuszania uwierzytelniania wieloskładnikowego dla wszystkich kont użytkowników w dzierżawie partnera, w tym dla użytkowników-Gości. Użytkownicy będą mogli ukończyć weryfikację MFA dla następujących obszarów:

- [Pulpit nawigacyjny Centrum partnerskiego](#partner-center-dashboard)
- [Interfejs API Centrum partnerskiego](#partner-center-api)
- [Administracja delegowana przez partnera](#partner-delegated-administration)

Większe i aktualne zabezpieczenia dotyczące zabezpieczeń i ochrony prywatności znajdują się wśród naszych najważniejszych priorytetów i będziemy nadal pomagać partnerom chronić klientów i dzierżawców. Wszyscy partnerzy uczestniczący w programie dostawcy rozwiązań w chmurze (CSP), dostawcy panelu sterowania (CPVs) i doradcy powinni zaimplementować [wymagania dotyczące zabezpieczeń partnerów](partner-security-requirements.md) , aby zachować zgodność.

Aby pomóc partnerom w ochronie firm i klientów przed kradzieżą tożsamości i nieautoryzowanym dostępem, firma Microsoft opracowała dodatkowe zabezpieczenia dla dzierżawców partnerów, którzy będą mieć uprawnienia i weryfikują uwierzytelnianie wieloskładnikowe. 

## <a name="partner-center-dashboard"></a>Pulpit nawigacyjny Centrum partnerskiego

Niektóre strony na pulpicie nawigacyjnym Centrum partnerskiego będą chronione za pomocą usługi MFA, w tym:

- Wszystkie strony na karcie **klienci** , na przykład wszystkie strony, do których można uzyskać dostęp za pomocą następującego adresu URL: https://partner.microsoft.com/commerce/*
- Wszystkie strony na karcie **> żądania klienta** , na przykład strona, do której uzyskano dostęp w ramach https://partner.microsoft.com/dashboard/support/csp/customers/*
- Strona rozliczeń

W poniższej tabeli przedstawiono typy użytkowników autoryzowane do uzyskiwania dostępu do tych stron chronionych przez usługę MFA (w związku z czym ma to wpływ na tę funkcję).


| Strona chroniona przez usługę MFA       | Agenci administracyjni      |  Agenci sprzedaży     |   Agenci pomocy technicznej     | Administrator globalny      |  Administrator rozliczeń     | 
|---    |---    |---    |---    |---    |---    |
| Wszystkie strony na karcie klienci      |   x    |    x   |  x     |       |       |
| Wszystkie strony w obszarze Pomoc techniczna > karcie żądania klientów     | x      |       |    x   |       |       |
| Strona rozliczeń     |   x    |       |       |    x   |   x    |

Jeśli spróbujesz uzyskać dostęp do dowolnej z tych stron, a weryfikacja usługi MFA nie została wcześniej zakończona, konieczne będzie wykonanie tej czynności. Inne strony w centrum partnerskim, takie jak strona przegląd, Service Health sprawdzania stanu nie wymagają uwierzytelniania wieloskładnikowego.

## <a name="verification-examples"></a>Przykłady weryfikacji

Aby zilustrować, jak weryfikacja działa na pulpicie nawigacyjnym Centrum partnerskiego, weź pod uwagę następujące przykłady.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Przykład 1: partner zaimplementował usługę Azure AD MFA

1. Janina działa dla dostawcy CSP contoso. Firma Contoso zaimplementował usługę MFA dla wszystkich użytkowników w dzierżawie partnera contoso przy użyciu usługi Azure Active Directory (Azure AD) MFA.

2. Joanna uruchamia nową sesję przeglądarki i przechodzi do strony omówienia pulpitu nawigacyjnego Centrum partnerskiego (która nie jest chroniona przez usługę MFA). Usługa Partner Center przekierowuje do usługi Azure AD, aby się zalogować.

3. Ze względu na istniejącą konfigurację usługi Azure AD MFA przez firmę Contoso, firma Janina jest wymagana do ukończenia weryfikacji MFA. Po pomyślnym zalogowaniu się i sprawdzeniu MFA nastąpi przekierowanie do strony Przegląd pulpitu nawigacyjnego Centrum partnerskiego.

4. Joanna próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w centrum partnerskim. Ponieważ Janina już ukończył weryfikację MFA podczas logowania, Jan może uzyskać dostęp do strony chronionej za pomocą usługi MFA bez konieczności ponownego przechodzenia przez weryfikację MFA.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Przykład 2: partner zaimplementował uwierzytelnianie wieloskładnikowe innej firmy przy użyciu federacji tożsamości

1. Trent działa dla dostawcy usług kryptograficznych Wingtip. Wingtip zaimplementował uwierzytelnianie MFA dla wszystkich użytkowników w dzierżawie usługi Wingtip partner korzystający z funkcji MFA innej firmy, która jest zintegrowana z usługą Azure AD za pośrednictwem federacji tożsamości.

2. Trent uruchamia nową sesję przeglądarki i przechodzi do strony omówienia pulpitu nawigacyjnego Centrum partnerskiego (która nie jest chroniona przez usługę MFA). Centrum partnerskie przekierowuje Trent do usługi Azure AD, aby się zalogować.

3. Ponieważ Wingtip ma konfigurację federacji tożsamości, usługa Azure AD przekierowuje Trent do dostawcy tożsamości federacyjnych, aby ukończyć weryfikację logowania i uwierzytelnianie wieloskładnikowe. Po pomyślnym zalogowaniu się i weryfikacji MFA Trent zostaje przekierowany z powrotem do usługi Azure AD, a następnie na stronie Przegląd pulpitu nawigacyjnego Centrum partnerskiego.

4. Trent próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w centrum partnerskim. Ponieważ Trent już ukończył weryfikację MFA podczas logowania, Trent może uzyskać dostęp do chronionej strony usługi MFA bez konieczności ponownego przechodzenia przez weryfikację MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Przykład 3: partner nie zaimplementował MFA

1. Jan współpracuje z programem CSP fabrikam. Firma Fabrikam nie zaimplementował uwierzytelniania wieloskładnikowego dla każdego użytkownika w ramach dzierżawy partnera fabrikam.

2. Jan uruchamia nową sesję przeglądarki i przechodzi do strony omówienia pulpitu nawigacyjnego Centrum partnerskiego (która nie jest chroniona przez usługę MFA). Centrum partnerskie przekierowuje Jan do usługi Azure AD, aby się zalogować.

3. Ponieważ firma Fabrikam nie zaimplementował MFA, Jan nie jest wymagana do ukończenia weryfikacji MFA. Po pomyślnym zalogowaniu Jan zostaje przekierowany z powrotem na stronę omówienia pulpitu nawigacyjnego Centrum partnerskiego.

4. Jan próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w centrum partnerskim. Ponieważ Jan nie ukończył weryfikacji MFA, centrum partnerskie przekierowuje Jan do usługi Azure AD, aby ukończyć weryfikację uwierzytelniania MFA. Ponieważ jest to pierwszy raz Jan wymagany do zakończenia uwierzytelniania MFA, Jan jest również proszony o [rejestrację usługi MFA](#mfa-registration-experience). Po pomyślnym zarejestrowaniu usługi MFA i weryfikacji MFA Jan może teraz uzyskiwać dostęp do strony chronionej za pomocą usługi MFA.

5. Drugi dzień przed wdrożeniem MFA przez firmę Fabrikam dla dowolnego użytkownika Jan uruchamia nową sesję przeglądarki i przechodzi do strony omówienia pulpitu nawigacyjnego Centrum partnerskiego (która nie jest chroniona przez usługę MFA). Centrum partnerskie przekierowuje Jan do usługi Azure AD, aby zalogować się bez monitu MFA. 

6. Jan próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w centrum partnerskim. Ponieważ Jan nie ukończył weryfikacji MFA, centrum partnerskie przekierowuje Jan do usługi Azure AD, aby ukończyć weryfikację uwierzytelniania MFA. Ze względu na to, że Jan zarejestrował uwierzytelnianie MFA, więc poprosimy o ukończenie weryfikacji MFA.

> [!NOTE]
>Akcja: Administratorzy firmy mają [trzy opcje](partner-security-requirements.md#implementing-multi-factor-authentication) implementowania usługi MFA.

## <a name="partner-center-api"></a>Interfejs API Centrum partnerskiego

Interfejs API Centrum partnerskiego obsługuje zarówno uwierzytelnianie aplikacji, jak i uwierzytelnianie użytkowników i aplikacji. 

W przypadku użycia uwierzytelniania aplikacji + użytkownika centrum partnerskie będzie wymagało weryfikacji MFA. Dokładniej mówiąc, gdy aplikacja partnerska chce wysłać żądanie interfejsu API do Centrum partnerskiego, musi zawierać token dostępu w nagłówku autoryzacji żądania. 

> [!NOTE]
>Mechanizm [Secure Application model Framework](/partner-center/develop/enable-secure-app-model) to skalowalna platforma służąca do uwierzytelniania partnerów CSP i CPVs przy użyciu architektury Microsoft Azure MFA podczas wywoływania interfejsów API Centrum partnerskiego. Musisz zaimplementować tę strukturę przed włączeniem uwierzytelniania MFA w dzierżawie. 

Gdy centrum partnerskie odbiera żądanie interfejsu API z tokenem dostępu uzyskanym przy użyciu aplikacji i uwierzytelniania użytkownika, interfejs API Centrum partnerskiego sprawdzi obecność wartości *MFA* w żądaniu *metody uwierzytelniania (AMR)* . Aby sprawdzić, czy token dostępu zawiera oczekiwaną wartość odwołania metody uwierzytelniania (AMR), można użyć dekodera JWT:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Jeśli wartość jest obecna, centrum partnerskie zawiera zakończenie weryfikacji usługi MFA i przetwarzanie żądania interfejsu API. Jeśli wartość nie jest obecna, interfejs API Centrum partnerskiego odrzuci żądanie z następującą odpowiedzią:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

W przypadku użycia uwierzytelniania App-Only interfejsy API obsługujące uwierzytelnianie App-Only będą stale działać bez konieczności korzystania z usługi MFA.

## <a name="partner-delegated-administration"></a>Administracja delegowana przez partnera

Konta partnerów, w tym agenci administracyjni i agenci pomocy technicznej, mogą korzystać z uprawnień administratora delegowanego przez partnera do zarządzania zasobami klienta za pośrednictwem portali usług online firmy Microsoft, interfejsu wiersza polecenia (CLI) i interfejsów API (przy użyciu aplikacji i uwierzytelniania użytkowników).

### <a name="using-service-portals"></a>Korzystanie z portali usług

W przypadku uzyskiwania dostępu do portali usług online firmy Microsoft przy użyciu uprawnień administratora delegowanego przez partnera (administratora w imieniu) do zarządzania zasobami klienta wiele z tych portali wymaga, aby konto partnera było uwierzytelniane interaktywnie, a dzierżawa usługi Azure AD ustawiona jako kontekst uwierzytelniania — wymagane jest konto partnera do logowania się do dzierżawy klienta.

Gdy usługa Azure AD odbiera takie żądania uwierzytelniania, będzie wymagało, aby konto partnera kończyło weryfikację MFA. Istnieją dwa możliwe środowiska użytkownika, w zależności od tego, czy konto partnera jest tożsamością zarządzaną, czy federacyjną:

- Jeśli konto partnera jest tożsamością **zarządzaną** , usługa Azure AD będzie bezpośrednio monitować użytkownika o ukończenie weryfikacji uwierzytelniania MFA. Jeśli konto partnera nie zostało wcześniej zarejestrowane w usłudze Azure AD, użytkownik zostanie poproszony o [ukończenie rejestracji MFA](#mfa-registration-experience) w pierwszej kolejności.

- Jeśli konto partnera jest tożsamością **federacyjną** , środowisko jest zależne od tego, jak administrator partnera skonfigurował Federacji w usłudze Azure AD. Podczas konfigurowania Federacji w usłudze Azure AD administrator partnerski może wskazać usługę Azure AD, czy dostawca tożsamości federacyjnych obsługuje uwierzytelnianie wieloskładnikowe, czy nie. Jeśli tak, usługa Azure AD przekieruje użytkownika do dostawcy tożsamości federacyjnych, aby ukończyć weryfikację MFA. W przeciwnym razie usługa Azure AD będzie bezpośrednio monitować użytkownika o zakończenie weryfikacji uwierzytelniania MFA. Jeśli konto partnera nie zostało wcześniej zarejestrowane w usłudze Azure AD, użytkownik zostanie poproszony o [ukończenie rejestracji MFA](#mfa-registration-experience) w pierwszej kolejności.

Ogólne środowisko jest podobne do scenariusza, w którym dzierżawa klienta końcowego wdrożyła uwierzytelnianie wieloskładnikowe dla administratorów. Na przykład dzierżawa klienta włączyła [Ustawienia domyślne zabezpieczeń usługi Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), które wymagają, aby wszystkie konta z uprawnieniami administracyjnymi mogli logować się do dzierżawy klienta z weryfikacją MFA, w tym agentami administracyjnymi i agentami pomocy technicznej. W celach testowych partnerzy mogą włączyć [wartości domyślne zabezpieczeń usługi Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) w dzierżawie klienta, a następnie próbować uzyskać dostęp do dzierżawy klienta przy użyciu uprawnień administracji delegowanej przez partnera.

> [!NOTE]
> Nie wszystkie portale usług online firmy Microsoft wymagają kont partnerskich do logowania się do dzierżawy klienta podczas uzyskiwania dostępu do zasobów klienta przy użyciu uprawnień administratora delegowanego przez partnera. Zamiast tego wymagają tylko kont partnerskich do logowania się do dzierżawy partnerskiej. Przykładem jest centrum administracyjne programu Exchange. Z upływem czasu oczekujemy, że te portale będą wymagały logowania się do dzierżawy klienta przy użyciu uprawnień administratora delegowanego przez partnera.

### <a name="using-service-apis"></a>Korzystanie z interfejsów API usług

Niektóre interfejsy API usług online firmy Microsoft (takie jak Azure Resource Manager, Azure AD Graph, Microsoft Graph itp.) obsługują partnerów przy użyciu uprawnień administratora delegowanego przez partnera do programistycznego zarządzania zasobami klientów. Aby korzystać z uprawnień administratora delegowanego przez partnera z tymi interfejsami API, aplikacja partnerska musi zawierać token dostępu w nagłówku autoryzacji żądania interfejsu API, gdzie token dostępu jest uzyskiwany za pomocą konta użytkownika partnerskiego do uwierzytelnienia w usłudze Azure AD, z zestawem klienta usługi Azure AD jako kontekstem uwierzytelniania. Aplikacja partnerska musi zalogować się do dzierżawy klienta przy użyciu konta użytkownika partnera.

Gdy usługa Azure AD odbiera takie jak żądanie uwierzytelnienia, usługa Azure AD będzie wymagać konta użytkownika partnera, aby ukończyć weryfikację uwierzytelniania MFA. Jeśli konto użytkownika partnera nie zostało wcześniej zarejestrowane na potrzeby usługi MFA, najpierw zostanie wyświetlony monit o ukończenie rejestracji usługi MFA.

Ta funkcja ma wpływ na wszystkie aplikacje partnerskie zintegrowane z tymi interfejsami API przy użyciu uprawnień administratora delegowanego przez partnera. Aby zapewnić, że aplikacje partnerskie mogą nadal korzystać z tych interfejsów API bez przeszkód:

- Partner musi unikać używania nieinteraktywnej metody uwierzytelniania użytkowników w usłudze Azure AD w celu uzyskania tokenu dostępu. W przypadku korzystania z metody uwierzytelniania użytkowników nieinterakcyjnych, takich jak [przepływ haseł](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), usługa Azure AD nie będzie mogła monitować użytkownika o ukończenie weryfikacji MFA. Partner musi przełączyć się do korzystania z metody interaktywnego uwierzytelniania użytkowników, takiej jak [OpenID Connect Connect Flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) .

- Podczas interaktywnej metody uwierzytelniania użytkowników Partner powinien używać konta użytkownika partnera, które jest już włączone dla usługi MFA. Alternatywnie, po wyświetleniu monitu przez usługę Azure AD partner może ukończyć rejestrację uwierzytelniania MFA i weryfikację uwierzytelniania wieloskładnikowego podczas logowania.

- Jest to podobne do scenariusza, w którym dzierżawa klienta końcowego wdrożyła uwierzytelnianie wieloskładnikowe dla administratorów. Na przykład dzierżawa klienta włączyła [Ustawienia domyślne zabezpieczeń usługi Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), które wymagają, aby wszystkie konta użytkowników z uprawnieniami administracyjnymi mogli logować się do dzierżawy klienta z weryfikacją MFA, w tym agentami administracyjnymi i agentami pomocy technicznej. W celach testowych partnerzy mogą włączyć [wartości domyślne zabezpieczeń usługi Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) w dzierżawie klienta, a następnie spróbować użyć uprawnień administracji delegowanej przez partnera, aby programowo uzyskać dostęp do dzierżawy klienta.

### <a name="mfa-registration-experience"></a>Środowisko rejestracji usługi MFA

Jeśli podczas weryfikacji MFA konto partnera nie zostało wcześniej zarejestrowane w usłudze MFA, usługa Azure AD wyświetli monit o ukończenie rejestracji MFA w pierwszej kolejności:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Rejestracja usługi MFA — krok 1":::

Po kliknięciu **przycisku Dalej** użytkownik zostanie poproszony o wybranie z listy metod weryfikacji.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Rejestracja usługi MFA — krok 1":::

Po pomyślnej rejestracji użytkownik jest zobowiązany do ukończenia weryfikacji MFA na podstawie weryfikacji wybranej przez użytkownika.
 
## <a name="list-of-common-issues"></a>Lista typowych problemów

Przed zastosowaniem do [wyjątku technicznego](#how-to-submit-a-request-for-technical-exception) z wymogu usługi MFA Przejrzyj listę typowych problemów zgłoszonych przez innych partnerów, aby zrozumieć, czy Twoje żądanie jest prawidłowe.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problem 1: Partner potrzebuje więcej czasu na wdrożenie usługi MFA dla swoich agentów partnerskich
Partner nie został uruchomiony lub nadal trwa proces wdrażania usługi MFA dla swoich agentów partnerskich, którzy potrzebują dostępu do portali usług online firmy Microsoft przy użyciu uprawnień administracji delegowanej przez partnera do zarządzania zasobami klienta. Partner potrzebuje więcej czasu na ukończenie implementacji usługi MFA. Czy ten problem występuje w przypadku wyjątku technicznego?

**Odpowiedź** : nie. Partner musi wykonać plany wdrożenia usługi MFA dla swoich użytkowników, aby uniknąć przerw w działaniu.

> [!NOTE]
> Mimo że partner nie zaimplementował uwierzytelniania wieloskładnikowego dla swoich agentów partnerskich, agenci partnerów mogą nadal uzyskiwać dostęp do portali usług online firmy Microsoft przy użyciu uprawnień administracji delegowanej przez partnera, pod warunkiem, że po wyświetleniu monitu o zalogowanie się do dzierżawy klienta będzie można ukończyć rejestrację MFA Zakończenie rejestracji MFA nie powoduje automatycznego włączenia użytkownika do usługi MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problem 2: partner nie zaimplementował uwierzytelniania wieloskładnikowego dla kont użytkowników niekorzystających z uprawnień administratora delegowanego
Partner ma niektórych użytkowników w dzierżawach partnerskich, którzy nie wymagają dostępu do portali usług Microsoft Online Services w celu zarządzania zasobami klienta przy użyciu uprawnień administracji delegowanej przez partnera. Partner jest w trakcie wdrażania uwierzytelniania MFA dla tych użytkowników i potrzebuje więcej czasu. Czy ten problem występuje w przypadku wyjątku technicznego?

**Odpowiedź** : nie. Ponieważ te konta użytkowników nie korzystają z uprawnień administracji delegowanej przez partnera do zarządzania zasobami klienta, nie będą one wymagane do zalogowania się do dzierżawy klienta. Nie będzie to miało wpływ na usługę Azure AD wymagającą weryfikacji MFA podczas logowania się do dzierżawy klienta.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3: partner nie zaimplementował uwierzytelniania wieloskładnikowego dla kont usługi użytkownika
Partner ma niektóre konta użytkowników w dzierżawach partnerskich, które są używane przez urządzenia jako konta usług. Są to niskie konta uprzywilejowane, które nie wymagają centrum partnera dostępu ani portali usług online firmy Microsoft do zarządzania zasobami klienta przy użyciu uprawnień administracji delegowanej przez partnera. Czy ten problem występuje w przypadku wyjątku technicznego?

**Odpowiedź** : nie. Ponieważ te konta użytkowników nie korzystają z uprawnień administracji delegowanej przez partnera do zarządzania zasobami klienta, nie będą one wymagane do zalogowania się do dzierżawy klienta. Nie będzie to miało wpływ na usługę Azure AD wymagającą weryfikacji MFA podczas logowania się do dzierżawy klienta.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4: partner nie może zaimplementować usługi MFA przy użyciu aplikacji MS Authenticator
Partner ma zasady "Clean Desk", które nie pozwalają pracownikom na przełączanie osobistych urządzeń przenośnych do obszaru pracy. Bez dostępu do osobistych urządzeń przenośnych pracownicy nie mogą zainstalować aplikacji MS Authenticator, która jest jedyną weryfikacją MFA obsługiwaną przez domyślne ustawienia zabezpieczeń usługi Azure AD. Czy ten problem występuje w przypadku wyjątku technicznego?

**Odpowiedź** : nie, to nie jest prawidłowa przyczyna wyjątku technicznego. Partner powinien wziąć pod uwagę następujące alternatywy, dzięki czemu pracownicy mogą nadal zakończyć weryfikację MFA podczas uzyskiwania dostępu do Centrum partnerskiego:
- Partner może również zarejestrować się w celu uzyskania Azure AD — wersja Premium lub rozwiązań MFA innych firm (zgodnych z usługą Azure AD), które mogą zapewnić dodatkowe metody weryfikacji.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5: partner nie może zaimplementować uwierzytelniania MFA ze względu na użycie starszych protokołów uwierzytelniania
Partner ma niektórych agentów partnerskich, którzy nadal korzystają ze starszych protokołów uwierzytelniania, które nie są zgodne z uwierzytelnianiem MFA. Na przykład użytkownicy nadal korzystają z programu Outlook 2010, który jest oparty na starszych protokołach uwierzytelniania. Włączenie usługi MFA dla tych agentów partnerskich spowoduje zakłócenie użycia starszych protokołów uwierzytelniania.

**Odpowiedź** : nie, to nie jest prawidłowa przyczyna wyjątku technicznego. Partnerzy są zdecydowanie zachęcani do przejścia od używania starszych protokołów uwierzytelniania ze względu na potencjalne implikacje zabezpieczeń, ponieważ te protokoły nie mogą być chronione za pomocą weryfikacji MFA i są znacznie bardziej podatne na złamanie poświadczeń. Jeśli nie jest to możliwe, partnerzy powinni rozważyć zarejestrowanie się w usłudze Azure AD — wersja Premium, co umożliwia korzystanie z haseł aplikacji. Hasła aplikacji są hasłami generowanymi przez system jednorazowy i są zwykle silniejszymi niż hasła generowane przez człowieka. Przy użyciu haseł aplikacji partnerzy mogą zaimplementować uwierzytelnianie wieloskładnikowe dla swoich użytkowników, jednocześnie powracając do haseł aplikacji tylko dla starszych protokołów uwierzytelniania.

Przeczytaj wpis dotyczący [uwierzytelniania podstawowego i usługi Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) , aby zrozumieć najnowszy plan na potrzeby obsługi starszej wersji programu Outlook i postępować zgodnie z [blogiem zespołu programu Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) w celu uzyskania nadchodzących wiadomości. 

> [!NOTE]
> Mimo że partner nie zaimplementował uwierzytelniania wieloskładnikowego dla swoich agentów partnerskich, agenci partnerów mogą nadal uzyskiwać dostęp do portali usług online firmy Microsoft przy użyciu uprawnień administracji delegowanej przez partnera, pod warunkiem, że po wyświetleniu monitu o zalogowanie się do dzierżawy klienta będzie można ukończyć rejestrację MFA Zakończenie rejestracji MFA nie powoduje automatycznego włączenia użytkownika do usługi MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problem 6: partner zaimplementował MFA innej firmy, który nie jest rozpoznawany przez usługę Azure AD
Partner zaimplementował uwierzytelnianie wieloskładnikowe dla swoich użytkowników przy użyciu rozwiązania MFA innej firmy. Jednak partner nie może prawidłowo skonfigurować rozwiązania MFA innej firmy w celu przekazania do usługi Azure AD, że weryfikacja MFA została ukończona podczas uwierzytelniania użytkownika. Czy jest to prawidłowy powód dotyczący wyjątku technicznego?

**Odpowiedź** : tak, ten problem może być traktowany jako prawidłowy powód wyjątku technicznego. Przed przesłaniem żądania dotyczącego wyjątku technicznego należy potwierdzić u dostawcy rozwiązań MFA innej firmy, że nie można skonfigurować rozwiązania MFA do przepływu żądania *authenticationmethodsreferences* (z wartością *Multipleauthn* ) do usługi Azure AD, aby wskazać, że weryfikacja usługi MFA została ukończona podczas uwierzytelniania użytkownika. Podczas przesyłania żądania dotyczącego wyjątku technicznego należy podać szczegóły używanego rozwiązania MFA innej firmy i wskazać metodę integracji (na przykład za pomocą federacji tożsamości lub użyć kontrolki niestandardowej usługi Azure AD) i podać następujące informacje w żądaniu wyjątku technicznego jako dokumenty pomocnicze:

- Konfiguracje usługi MFA innych firm.

- Wynik [testowania wymagań dotyczących zabezpieczeń partnerów](/powershell/partnercenter/test-partner-security-requirements) uruchomionych przez konto z obsługą usługi MFA innej firmy.

- Zamówienie zakupu używanego rozwiązania MFA innej firmy lub planowane do użycia.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Jak przesłać żądanie dla wyjątku technicznego

Partnerzy mogą zastosować do wyjątku technicznego, aby pominąć weryfikację MFA, jeśli wystąpią problemy techniczne z usługami online firmy Microsoft i nie ma żadnego możliwego rozwiązania lub obejścia tego problemu. Przed wykonaniem tej czynności Przejrzyj [listę typowych problemów](#list-of-common-issues) w poprzedniej sekcji.

Aby przesłać żądanie dotyczące wyjątku technicznego:

1. Zaloguj się do Centrum partnerskiego jako Administrator globalny lub Agent administracyjny.

2. Utwórz nowe żądanie obsługi partnera, przechodząc do **pomocy**  >  **technicznej partner** Request i klikając pozycję **nowe żądanie** .

3. Wyszukaj uwierzytelnianie **MFA — Żądaj wyjątku** w polu wyszukiwania. lub wybierz pozycję **dostawca CSP** z kategorii, a następnie wybierz pozycję **konta,** dołączanie, dostęp z tematu, a następnie wybierz pozycję **MFA-żądanie dla wyjątku** z tematu podrzędnego, a następnie wybierz pozycję **Następny krok** .

4. Podaj szczegóły żądane do przesłania żądania obsługi dla wyjątku technicznego, a następnie kliknij przycisk **Prześlij** .

Firma Microsoft może potrwać do trzech dni roboczych, aby zapewnić odpowiedź na żądanie wyjątku technicznego.

## <a name="next-steps"></a>Następne kroki

 - [Stan wymagań dotyczących zabezpieczeń partnerów](partner-security-compliance.md)