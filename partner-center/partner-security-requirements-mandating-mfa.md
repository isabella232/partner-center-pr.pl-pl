---
title: Upoważnianie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnera
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Dowiedz się, jak wymuszanie uwierzytelniania wieloskładnikowego dla dzierżaw partnerów pomoże zabezpieczyć dostęp do zasobów klienta. Obejmuje przykładowe scenariusze.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c29e59118f4b50cd25fbe0f1560519bb178768e2
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247432"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Upoważnianie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnera

**Odpowiednie role:** Administrator | Agent sprzedaży | Agent pomocy technicznej | Administrator rozliczeń | Administrator globalny

Ten artykuł zawiera szczegółowe przykłady i wskazówki dotyczące wymuszania uwierzytelniania wieloskładnikowego (MFA) w Partner Center. Celem tej funkcji jest pomoc partnerom w zabezpieczania dostępu do zasobów klientów przed naruszeniami poświadczeń. Partnerzy muszą wymuszać uwierzytelniania wieloskładnikowego dla wszystkich kont użytkowników w dzierżawie partnera, w tym dla użytkowników-gości. Użytkownicy zostaną upoważnione do ukończenia weryfikacji uwierzytelniania wieloskładnikowego w następujących obszarach:

- [Partner Center nawigacyjny](#partner-center-dashboard)
- [Interfejs API Centrum partnerskiego](#partner-center-api)
- [Administracja delegowana partnera](#partner-delegated-administration)

Większe i stałe zabezpieczenia i ochrona prywatności należą do naszych głównych priorytetów, a my nadal pomagamy partnerom chronić swoich klientów i dzierżawców. Wszyscy partnerzy biorący udział w programie Dostawca rozwiązań w chmurze (CSP), dostawcy Panel sterowania (CPV) i [](partner-security-requirements.md) doradcy powinni wdrożyć wymagania dotyczące zabezpieczeń partnerów, aby zachować zgodność.

Aby pomóc partnerom chronić firmy i klientów przed kradzieżą tożsamości i nieautoryzowanym dostępem, aktywowaliśmy dodatkowe zabezpieczenia dla dzierżaw partnerów, które nakażają i weryfikują usługę MFA. 

## <a name="partner-center-dashboard"></a>Partner Center nawigacyjny

Niektóre strony na pulpicie Partner Center nawigacyjnym będą chronione przez uwierzytelniania wieloskładnikowego, w tym:

- Wszystkie strony na karcie **Klienci,** np. wszystkie strony, do których można uzyskać dostęp za pośrednictwem następującego adresu URL: https://partner.microsoft.com/commerce/*
- Wszystkie strony na karcie **żądania > pomocy technicznej,** np. strona dostępna w obszarze https://partner.microsoft.com/dashboard/support/csp/customers/*
- Strona rozliczeń

W poniższej tabeli przedstawiono, które typy użytkowników są autoryzowane do uzyskiwania dostępu do tych stron chronionych przez usługę MFA (i w związku z tym ta funkcja ma na nie wpływ).


| Strona chroniona przez uwierzytelniania wieloskładnikowego       | Agenci administracyjni      |  Agenci sprzedaży     |   Agenci pomocy technicznej     | Administrator globalny      |  Administrator rozliczeń     | 
|---    |---    |---    |---    |---    |---    |
| Wszystkie strony na karcie Klienci      |   x    |    x   |  x     |       |       |
| Wszystkie strony na karcie Support > Customer requests (Żądania klientów pomocy technicznej)     | x      |       |    x   |       |       |
| Strona rozliczeń     |   x    |       |       |    x   |   x    |

Jeśli spróbujesz uzyskać dostęp do dowolnej z tych stron, a weryfikacja uwierzytelniania wieloskładnikowego nie została ukończona wcześniej, będzie to konieczne. Inne strony w Partner Center, takie jak strona Przegląd, Service Health sprawdzanie stanu nie wymagają uwierzytelniania wieloskładnikowego.

## <a name="verification-examples"></a>Przykłady weryfikacji

Aby zilustrować działanie weryfikacji na Partner Center nawigacyjnym, rozważ poniższe przykłady.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Przykład 1: Partner zaimplementował usługę Azure AD MFA

1. Magda pracuje dla firmy Contoso w firmie CSP. Firma Contoso wdrożyła usługę MFA dla wszystkich swoich użytkowników w dzierżawie partnera firmy Contoso przy użyciu Azure Active Directory (Azure AD).

2. Magna rozpoczyna nową sesję przeglądarki i przechodzi do Partner Center przeglądu pulpitu nawigacyjnego (która nie jest chroniona przez usługę MFA). Partner Center użytkownika Jane do usługi Azure AD w celu zalogowania się.

3. Ze względu na istniejącą konfigurację usługi Azure AD MFA firmy Contoso Jane jest wymagana do ukończenia weryfikacji uwierzytelniania wieloskładnikowego. Po pomyślnym zalogowaniu i weryfikacji uwierzytelniania wieloskładnikowego Magda zostanie przekierowana z powrotem Partner Center strony przeglądu pulpitu nawigacyjnego.

4. Magna próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w Partner Center. Ponieważ Magda zakończyła już weryfikację MFA podczas wcześniejszego logowania, może uzyskać dostęp do strony chronionej przez usługę MFA bez konieczności wcześniejszego ukończenia weryfikacji mfa.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Przykład 2: Partner zaimplementował usługę MFA innej firmy przy użyciu federacji tożsamości

1. Trent działa dla etykietki Wingtip dla CSP. Usługa Wingtip zaimplementowała usługę MFA dla wszystkich swoich użytkowników w dzierżawie partnera Wingtip przy użyciu usługi MFA innej firmy, która jest zintegrowana z usługą Azure AD za pośrednictwem federacji tożsamości.

2. Trent uruchamia nową sesję przeglądarki i przechodzi do Partner Center przeglądu pulpitu nawigacyjnego (która nie jest chroniona przez usługę MFA). Partner Center przekierowuje trent do usługi Azure AD, aby się zalogować.

3. Ponieważ usługa Wingtip ma federację tożsamości konfiguracji, usługa Azure AD przekierowuje trent do dostawcy tożsamości federacji w celu ukończenia logowania i weryfikacji uwierzytelniania wieloskładnikowego. Po pomyślnym zalogowaniu i weryfikacji uwierzytelniania wieloskładnikowego trent jest przekierowywany z powrotem do usługi Azure AD, a Partner Center strony przeglądu pulpitu nawigacyjnego.

4. Trent próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w Partner Center. Ponieważ trent zakończył już weryfikację MFA podczas wcześniejszego logowania, Trent może uzyskać dostęp do strony chronionej przez usługę MFA bez konieczności wcześniejszego ukończenia weryfikacji MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Przykład 3: Partner nie zaimplementował usługi MFA

1. Jan pracuje dla firmy Fabrikam w firmie CSP. Firma Fabrikam nie zaimplementowała usługi MFA dla żadnego użytkownika w dzierżawie partnera firmy Fabrikam.

2. Jan uruchamia nową sesję przeglądarki i przechodzi do Partner Center przeglądu pulpitu nawigacyjnego (która nie jest chroniona przez usługę MFA). Partner Center użytkownika Jan do usługi Azure AD w celu zalogowania się.

3. Ponieważ firma Fabrikam nie zaimplementowała usługi MFA, Jan nie jest wymagany do ukończenia weryfikacji mfa. Po pomyślnym zalogowaniu Jan zostanie przekierowany z powrotem do Partner Center przeglądu pulpitu nawigacyjnego.

4. Jan próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w Partner Center. Ponieważ Jan nie ukończył weryfikacji mfa, Partner Center przekierowuje Johna do usługi Azure AD w celu ukończenia weryfikacji MFA. Ponieważ jest to pierwszy raz, gdy Jan jest wymagany do ukończenia uwierzytelniania wieloskładnikowego, Jan jest również żądany do [zarejestrowania się w celu uwierzytelniania wieloskładnikowego.](#mfa-registration-experience) Po pomyślnej rejestracji uwierzytelniania wieloskładnikowego i weryfikacji uwierzytelniania wieloskładnikowego Jan może teraz uzyskać dostęp do strony chronionej przez usługę MFA.

5. Dzień przed wdrożeniem usługi MFA dla dowolnego użytkownika w firmie Fabrikam Jan rozpoczyna nową sesję przeglądarki i przechodzi do strony przeglądu pulpitu nawigacyjnego usługi Partner Center (która nie jest chroniona przez usługę MFA). Partner Center przekierowanie Johna do usługi Azure AD w celu zalogowania się bez monitu uwierzytelniania wieloskładnikowego. 

6. Jan próbuje uzyskać dostęp do jednej ze stron chronionych przez usługę MFA w Partner Center. Ponieważ Jan nie ukończył weryfikacji mfa, Partner Center przekierowuje Johna do usługi Azure AD w celu ukończenia weryfikacji MFA. Ponieważ Jan zarejestrował uwierzytelniania wieloskładnikowego, tym razem zostanie poproszony tylko o ukończenie weryfikacji usługi MFA.

> [!NOTE]
>Akcja: Administratorzy firmy mają [trzy opcje](partner-security-requirements.md#implementing-multi-factor-authentication) wdrażania usługi MFA.

## <a name="partner-center-api"></a>Interfejs API Centrum partnerskiego

Interfejs API Partner Center obsługuje zarówno uwierzytelnianie tylko aplikacji, jak i uwierzytelnianie aplikacji i użytkownika. 

W przypadku korzystania z uwierzytelniania app+user Partner Center będzie wymagać weryfikacji MFA. Dokładniej mówiąc, gdy aplikacja partnerska chce wysłać żądanie interfejsu API do usługi Partner Center, musi dołączyć token dostępu w nagłówku autoryzacji żądania. 

> [!NOTE]
>Ta [model aplikacji zabezpieczonych](/partner-center/develop/enable-secure-app-model) to skalowalna architektura do uwierzytelniania partnerów i procesorów CSP za pośrednictwem architektury Microsoft Azure MFA podczas wywoływania interfejsów API Partner Center. Należy zaimplementować tę platformę przed włączeniem uwierzytelniania wieloskładnikowego w dzierżawie. 

Gdy usługa Partner Center odbierze żądanie interfejsu API z tokenem dostępu uzyskanymi przy użyciu uwierzytelniania app+user, interfejs API usługi Partner Center sprawdzi obecność wartości *uwierzytelniania* wieloskładnikowego w oświadczeniem odwołania do metody uwierzytelniania *(AMR).* Możesz użyć dekodera JWT, aby sprawdzić, czy token dostępu zawiera oczekiwaną wartość odwołania do metody uwierzytelniania (AMR):

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

Jeśli ta wartość jest obecna, Partner Center stwierdzi, że weryfikacja MFA została ukończona i przetwarza żądanie interfejsu API. Jeśli wartość nie jest obecna, interfejs API Partner Center odrzuci żądanie z następującą odpowiedzią:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

W App-Only uwierzytelniania interfejsy API, które obsługują uwierzytelnianie App-Only, będą stale działać bez konieczności uwierzytelniania wieloskładnikowego.

## <a name="partner-delegated-administration"></a>Administracja delegowana partnera

Konta partnerów, w tym agenci administracyjni i agenci pomocy technicznej, mogą używać swoich delegowanych uprawnień administratora partnera do zarządzania zasobami klienta za pośrednictwem portali usług Microsoft Online Services, interfejsu wiersza polecenia (CLI) i interfejsów API (przy użyciu uwierzytelniania app+user).

### <a name="using-service-portals"></a>Korzystanie z portali usług

W przypadku uzyskiwania dostępu do portali usług Online Services firmy Microsoft przy użyciu delegowanych uprawnień administratora partnera (Admin-On-Behalf-Of) do zarządzania zasobami klientów wiele z tych portali wymaga interaktywnego uwierzytelniania konta partnera z dzierżawą usługi Azure AD klienta ustawioną jako kontekst uwierzytelniania — konto partnera jest wymagane do zalogowania się do dzierżawy klienta.

Gdy usługa Azure AD odbiera takie żądania uwierzytelniania, będzie wymagać konta partnera do ukończenia weryfikacji uwierzytelniania wieloskładnikowego. Istnieją dwa możliwe środowisko użytkownika w zależności od tego, czy konto partnera jest tożsamością zarządzaną, czy federacyjną:

- Jeśli konto partnera jest tożsamością **zarządzaną,** usługa Azure AD będzie bezpośrednio monitować użytkownika o ukończenie weryfikacji usługi MFA. Jeśli konto partnera nie zostało wcześniej zarejestrowane w usłudze Azure AD w usłudze MFA, użytkownik zostanie poproszony o ukończenie rejestracji w usłudze [MFA.](#mfa-registration-experience)

- Jeśli konto partnera jest **tożsamością federacyjną,** środowisko jest zależne od tego, jak administrator partnera skonfigurował federację w usłudze Azure AD. Podczas konfigurowania federacji w usłudze Azure AD administrator partnera może wskazać usłudze Azure AD, czy dostawca tożsamości federacji obsługuje usługę MFA, czy nie. Jeśli tak, usługa Azure AD przekieruje użytkownika do dostawcy tożsamości federacji w celu ukończenia weryfikacji usługi MFA. W przeciwnym razie usługa Azure AD będzie bezpośrednio monitować użytkownika o ukończenie weryfikacji uwierzytelniania wieloskładnikowego. Jeśli konto partnera nie zostało wcześniej zarejestrowane w usłudze MFA w usłudze Azure AD, użytkownik zostanie poproszony o ukończenie [rejestracji uwierzytelniania wieloskładnikowego.](#mfa-registration-experience)

Ogólne środowisko jest podobne do scenariusza, w którym dzierżawa klienta końcowego zaimplementowała usługę MFA dla swoich administratorów. Na przykład dzierżawa klienta włączyła domyślne ustawienia zabezpieczeń usługi [Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)co wymaga, aby wszystkie konta z uprawnieniami administracyjnymi logowały się do dzierżawy klienta przy użyciu weryfikacji MFA, w tym agentów administracyjnych i agentów pomocy technicznej. W celach testowych partnerzy mogą włączyć wartości domyślne zabezpieczeń usługi [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) w dzierżawie klienta, a następnie spróbować użyć uprawnień administracji delegowanej partnera w celu uzyskania dostępu do dzierżawy klienta.

> [!NOTE]
> Nie wszystkie portale usługi online firmy Microsoft wymagają kont partnerów w celu zalogowania się do dzierżawy klienta podczas uzyskiwania dostępu do zasobów klientów przy użyciu delegowanych uprawnień administratora partnera. Zamiast tego wymagają tylko kont partnerów do zalogowania się do dzierżawy partnera. Przykładem jest centrum Exchange administracyjnego. W czasie oczekujemy, że te portale będą wymagać od kont partnerów logowania się do dzierżawy klienta w przypadku korzystania z delegowanych uprawnień administratora partnera.

### <a name="using-service-apis"></a>Korzystanie z interfejsów API usługi

Niektóre interfejsy API usług Online Services firmy Microsoft (takie jak Azure Resource Manager, Azure AD Graph, Microsoft Graph itp.) obsługują partnerów przy użyciu delegowanych uprawnień administratora partnera do programowego zarządzania zasobami klientów. Aby używać delegowanych uprawnień administratora partnera z tymi interfejsami API, aplikacja partnerska musi uwzględnić token dostępu w nagłówku autoryzacji żądania interfejsu API, w którym token dostępu jest uzyskiwany przez posiadanie konta użytkownika partnera do uwierzytelniania w usłudze Azure AD, przy użyciu klienta usługi Azure AD ustawionego jako kontekst uwierzytelniania. Aplikacja partnerska musi mieć konto użytkownika partnera zalogowane do dzierżawy klienta.

Gdy usługa Azure AD odbiera takie żądanie uwierzytelniania, usługa Azure AD będzie wymagać konta użytkownika partnera do ukończenia weryfikacji uwierzytelniania wieloskładnikowego. Jeśli konto użytkownika partnera nie zostało wcześniej zarejestrowane w celu uwierzytelniania wieloskładnikowego, zostanie najpierw wyświetlony monit o ukończenie rejestracji uwierzytelniania wieloskładnikowego.

Ta funkcja ma wpływ na wszystkie aplikacje partnerów zintegrowane z tymi interfejsami API przy użyciu delegowanych uprawnień administratora partnera. Aby zapewnić, że aplikacje partnerów będą nadal działać z tymi interfejsami API bez zakłóceń:

- Partner musi unikać używania metody uwierzytelniania użytkownika nieinterakcyjnego w usłudze Azure AD w celu uzyskania tokenu dostępu. W przypadku korzystania z metody uwierzytelniania użytkownika nieinterakcyjnego, takiej jak [Password Flow,](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)usługa Azure AD nie będzie mogła monitować użytkownika o ukończenie weryfikacji mfa. Partner musi zamiast tego przełączyć się na używanie metody uwierzytelniania użytkownika interakcyjnego, takiej [Połączenie OpenID.](/azure/active-directory/develop/v1-protocols-openid-connect-code)

- Podczas metody uwierzytelniania użytkownika interakcyjnego partner powinien używać konta użytkownika partnera, które jest już włączone dla usługi MFA. Alternatywnie po wyświetleniu monitu przez usługę Azure AD partner może ukończyć rejestrację uwierzytelniania wieloskładnikowego i weryfikację uwierzytelniania wieloskładnikowego podczas logowania.

- Jest to podobne do scenariusza, w którym dzierżawa klienta końcowego zaimplementowała usługę MFA dla swoich administratorów. Na przykład dzierżawa klienta włączyła wartości domyślne zabezpieczeń usługi [Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)co wymaga, aby wszystkie konta użytkowników z uprawnieniami administracyjnymi logowały się do dzierżawy klienta przy użyciu weryfikacji MFA, w tym agentów administracyjnych i agentów pomocy technicznej. W celach testowych partnerzy mogą włączyć wartości domyślne zabezpieczeń usługi [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) w dzierżawie klienta, a następnie spróbować użyć uprawnień administracji delegowanej partnera, aby programowo uzyskać dostęp do dzierżawy klienta.

### <a name="mfa-registration-experience"></a>Środowisko rejestracji uwierzytelniania wieloskładnikowego

Jeśli konto partnera nie zostało wcześniej zarejestrowane w celu uwierzytelniania wieloskładnikowego podczas weryfikacji uwierzytelniania wieloskładnikowego, usługa Azure AD wyświetli monit o ukończenie rejestracji uwierzytelniania wieloskładnikowego:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Krok 1 rejestracji uwierzytelniania wieloskładnikowego.":::

Po kliknięciu **przycisku** Dalej użytkownik zostanie poproszony o wybranie z listy metod weryfikacji.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Krok 2 rejestracji uwierzytelniania wieloskładnikowego.":::

Po pomyślnej rejestracji użytkownik musi ukończyć weryfikację MFA na podstawie weryfikacji wybranej przez użytkownika.
 
## <a name="list-of-common-issues"></a>Lista typowych problemów

Przed zgłoszeniem [wyjątku technicznego](#how-to-submit-a-request-for-technical-exception) z wymagania uwierzytelniania wieloskładnikowego zapoznaj się z listą typowych problemów zgłaszanych przez innych partnerów, aby dowiedzieć się, czy twoje żądanie jest prawidłowe.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problem 1. Partner potrzebuje więcej czasu na wdrożenie usługi MFA dla swoich agentów partnerskich
Partner nie został uruchomiony lub nadal jest w trakcie wdrażania uwierzytelniania wieloskładnikowego dla agentów partnerskich, którzy wymagają dostępu do portali usług Online Services firmy Microsoft przy użyciu delegowanych uprawnień administracyjnych partnera do zarządzania zasobami klienta. Partner potrzebuje więcej czasu na ukończenie implementacji usługi MFA. Czy ten problem jest prawidłową przyczyną wyjątku technicznego?

**Odpowiedź:** Nie. Partner musi planować wdrożenie uwierzytelniania wieloskładnikowego dla swoich użytkowników, aby uniknąć zakłóceń.

> [!NOTE]
> Mimo że partner nie zaimplementował usługi MFA dla swoich agentów partnerskich, agenci partnerscy nadal mogą uzyskać dostęp do portali usług online firmy Microsoft przy użyciu delegowanych uprawnień administracyjnych partnera, pod warunkiem że mogą ukończyć rejestrację uwierzytelniania MFA i weryfikację uwierzytelniania WIELOSKŁADNIKowego po wyświetleniu monitu podczas logowania do dzierżawy klienta. Ukończenie rejestracji uwierzytelniania wieloskładnikowego nie umożliwia użytkownikowi automatycznego uwierzytelniania wieloskładnikowego.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problem 2. Partner nie zaimplementował uwierzytelniania wieloskładnikowego dla kont użytkowników, które nie korzystały z delegowanych uprawnień administratora
Partner ma niektórych użytkowników w dzierżawach partnerów, którzy nie wymagają dostępu do portali usług Online Services firmy Microsoft w celu zarządzania zasobami klientów przy użyciu delegowanych uprawnień administracyjnych partnera. Partner jest w trakcie implementowania usługi MFA dla tych użytkowników i potrzebuje więcej czasu na ukończenie. Czy ten problem jest prawidłową przyczyną wyjątku technicznego?

**Odpowiedź:** Nie. Ponieważ te konta użytkowników nie są przy użyciu uprawnień administracji delegowanej partnera do zarządzania zasobami klientów, nie będą wymagane do logowania się do dzierżawy klienta. Usługa Azure AD nie będzie wymagać weryfikacji MFA podczas logowania do dzierżawy klienta.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3. Partner nie zaimplementował uwierzytelniania wieloskładnikowego dla kont usług użytkowników
Partner ma niektóre konta użytkowników w dzierżawach partnerów, które są używane przez urządzenia jako konta usług. Są to konta o niskich uprawnieniach, które nie wymagają dostępu do Partner Center ani portali usług Online Services firmy Microsoft w celu zarządzania zasobami klientów przy użyciu delegowanych uprawnień administracyjnych partnera. Czy ten problem jest prawidłową przyczyną wyjątku technicznego?

**Odpowiedź:** Nie. Ponieważ te konta użytkowników nie są przy użyciu uprawnień administracji delegowanej partnera do zarządzania zasobami klientów, nie będą wymagane do logowania się do dzierżawy klienta. Usługa Azure AD nie będzie wymagać weryfikacji MFA podczas logowania do dzierżawy klienta.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4. Partner nie może zaimplementować usługi MFA przy użyciu aplikacji MS Authenticator App
Partner ma zasady "czystego biurka", które nie zezwalają pracownikom na przynoszenie osobistych urządzeń przenośnych do obszaru roboczego. Bez dostępu do swoich osobistych urządzeń przenośnych pracownicy nie mogą zainstalować aplikacji MS Authenticator App, która jest jedyną weryfikacją MFA obsługiwaną przez ustawienia domyślne zabezpieczeń usługi Azure AD. Czy ten problem jest prawidłową przyczyną wyjątku technicznego?

**Odpowiedź:** Nie, nie jest to prawidłowa przyczyna wyjątku technicznego. Partner powinien rozważyć następujące alternatywy, aby jego pracownicy nadal mogą ukończyć weryfikację uwierzytelniania wieloskładnikowego podczas uzyskiwania dostępu do Partner Center:
- Partner może również zarejestrować się w celu Azure AD — wersja Premium lub rozwiązań MFA innych firm (zgodnych z usługą Azure AD), które mogą zapewnić dodatkowe metody weryfikacji.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5. Partner nie może zaimplementować usługi MFA ze względu na użycie starszych protokołów uwierzytelniania
Partner ma niektórych agentów partnerów, którzy nadal używa starszych protokołów uwierzytelniania, które nie są zgodne z usługą MFA. Na przykład użytkownicy nadal będą korzystać z programu Outlook 2010, który jest oparty na starszych protokołach uwierzytelniania. Włączenie uwierzytelniania wieloskładnikowego dla tych agentów partnerskich spowoduje zakłócenie korzystania ze starszych protokołów uwierzytelniania.

**Odpowiedź:** Nie, nie jest to prawidłowa przyczyna wyjątku technicznego. Partnerzy są zdecydowanie zachęcani do odejścia od korzystania ze starszych protokołów uwierzytelniania ze względu na potencjalne implikacje dla bezpieczeństwa, ponieważ nie można chronić tych protokołów za pomocą weryfikacji MFA i są one znacznie bardziej podatne na naruszenia poświadczeń. Jeśli odejście od korzystania ze starszych protokołów uwierzytelniania nie jest opcją, partnerzy powinni rozważyć zarejestrowanie się w Azure AD — wersja Premium, która obsługuje korzystanie z haseł aplikacji. Hasła aplikacji są hasłami generowanymi przez system i zazwyczaj są silniejsze niż hasła generowane przez człowieka. Korzystając z haseł aplikacji, partnerzy mogą zaimplementować uwierzytelnianie wieloskładnikowe dla swoich użytkowników, jednocześnie wracając do haseł aplikacji tylko w przypadku starszych protokołów uwierzytelniania.

Przeczytaj wpis na temat uwierzytelniania podstawowego i usługi [Exchange Online,](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) aby zrozumieć najnowszy plan obsługi starszego uwierzytelniania dla usługi Outlook, a następnie postępuj zgodnie z [blogiem](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) zespołu Exchange, aby uzyskać nadchodzące wiadomości. 

> [!NOTE]
> Mimo że partner nie zaimplementował usługi MFA dla swoich agentów partnerskich, agenci partnerscy nadal mogą uzyskać dostęp do portali usług online firmy Microsoft przy użyciu delegowanych uprawnień administracyjnych partnera, pod warunkiem że mogą ukończyć rejestrację uwierzytelniania MFA i weryfikację uwierzytelniania WIELOSKŁADNIKowego po wyświetleniu monitu podczas logowania do dzierżawy klienta. Ukończenie rejestracji uwierzytelniania wieloskładnikowego nie umożliwia użytkownikowi automatycznego uwierzytelniania wieloskładnikowego.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problem 6. Partner zaimplementował usługę MFA innej firmy, która nie jest rozpoznawana przez usługę Azure AD
Partner zaimplementował usługę MFA dla swoich użytkowników przy użyciu rozwiązania mfa innej firmy. Jednak partner nie może poprawnie skonfigurować rozwiązania mfa innej firmy do przekazywania do usługi Azure AD, że weryfikacja uwierzytelniania wieloskładnikowego została ukończona podczas uwierzytelniania użytkownika. Czy jest to prawidłowa przyczyna wyjątku technicznego?

**Odpowiedź:** Tak, ten problem może być traktowany jako prawidłowa przyczyna wyjątku technicznego. Przed przesłaniem żądania wyjątku technicznego potwierdź u dostawcy rozwiązania MFA innej firmy, że nie można skonfigurować rozwiązania MFA do przepływu oświadczenia *authenticationmethodsreferences* (z wartością *multipleauthn*) do usługi Azure AD, aby wskazać, że weryfikacja MFA została ukończona podczas uwierzytelniania użytkownika. Przesyłając żądanie wyjątku technicznego, musisz podać szczegóły używanego rozwiązania MFA innej firmy i wskazać metodę integracji (np. za pośrednictwem federacji tożsamości lub użycia niestandardowej kontroli usługi Azure AD) i podać następujące informacje w żądaniu wyjątku technicznego jako dokumenty dodatkowe:

- Konfiguracje usługi MFA innej firmy.

- Wynik testu wymagań [zabezpieczeń partnera uruchomionych](/powershell/partnercenter/test-partner-security-requirements) przez konto z włączoną usługą MFA innej firmy.

- Zamówienie zakupu rozwiązania MFA innej firmy, z których korzystasz lub które zamierzasz użyć.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Jak przesłać żądanie wyjątku technicznego

Partnerzy mogą wystąpić o wyjątek techniczny, aby pominąć weryfikację MFA, jeśli napotkają problemy techniczne z usługami Online Services firmy Microsoft i nie ma możliwego rozwiązania ani obejścia. Zanim to zrobisz, [zapoznaj się z listą typowych problemów](#list-of-common-issues) w poprzedniej sekcji.

Aby przesłać żądanie wyjątku technicznego:

1. Zaloguj się do Partner Center jako administrator globalny lub agent administratora.

2. Utwórz nowe żądanie obsługi partnera, przechodząc do opcji **Żądania** pomocy technicznej dla  >  **partnerów** pomocy technicznej i wybierając pozycję Nowe **żądanie.**

3. Wyszukiwanie **uwierzytelniania wieloskładnikowego — żądanie wyjątku** w polu wyszukiwania; lub wybierz **pozycję CSP** z kategorii, wybierz pozycję **Konta, Dołączanie,** Dostęp z tematu, a następnie wybierz pozycję **MFA** — żądanie wyjątku z podtematu, a następnie wybierz **następny krok.**

4. Podaj szczegóły wymagane do przesyłania żądania obsługi dotyczące wyjątku technicznego, a następnie wybierz pozycję **Prześlij**.

Firma Microsoft może potrwać do trzech dni roboczych, aby udzielić odpowiedzi na żądanie wyjątku technicznego.

## <a name="next-steps"></a>Następne kroki

 - [Stan wymagań dotyczących zabezpieczeń partnerów](partner-security-compliance.md)