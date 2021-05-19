---
title: Partner security requirements FAQ
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Często zadawane pytania dotyczące wymagań dotyczących zabezpieczeń partnerów — co to są, jak partnerzy powinni je zaimplementować i jak wiesz, czy zostały spełnione.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 174c56ce9bb5fb3d9d92c1ef18af73479619f4bb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145885"
---
# <a name="common-questions-about-partner-security-requirements"></a>Często zadawane pytania dotyczące wymagań dotyczących zabezpieczeń partnerów

**Odpowiednie role:** wszyscy Partner Center użytkowników

W tym artykule znajdują się odpowiedzi na niektóre często zadawane pytania dotyczące [wymagań dotyczących zabezpieczeń partnera.](partner-security-requirements.md)

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Jakie są wymagania dotyczące zabezpieczeń partnerów i dlaczego należy je zaimplementować?

Większe i stałe zabezpieczenia i ochrona prywatności należą do naszych głównych priorytetów i nadal pomagamy partnerom chronić swoich klientów i dzierżawców. Nadal widzimy bardziej zaawansowane, zwiększające się liczby ataków na zabezpieczenia, przede wszystkim związanych ze zdarzeniami naruszenia zabezpieczeń tożsamości. Ponieważ środki zapobiegawcze odgrywają kluczową rolę w ogólnej strategii obrony [](partner-security-requirements.md) w celu zapobiegania atakom na zabezpieczenia, w 2019 r. wprowadziliśmy obowiązkowe wymagania dotyczące zabezpieczeń. Wszyscy partnerzy biorący udział w programie Dostawca rozwiązań w chmurze (CSP), dostawcy Panel sterowania i doradcy muszą zaimplementować wymagania, aby zachować zgodność.

### <a name="what-are-the-key-timelines-and-milestones"></a>Jakie są kluczowe osie czasu i kamienie milowe?

Terminy związane z tymi wymaganiami w zakresie zabezpieczeń, w tym osie czasu i kamienie milowe, są zawarte w [Microsoft Partner Agreement](microsoft-partner-agreement.md). Aby zachować zgodność z uczestnictwem w programie CSP, należy jak najszybciej zaimplementować te wymagania dotyczące zabezpieczeń.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Co się stanie, jeśli te wymagania dotyczące zabezpieczeń partnera nie zostaną zaimplementowane?

Usługa Microsoft Partner Agreement wymaga wymuszenia uwierzytelniania wieloskładnikowego dla kont użytkowników i przyjęcia modelu bezpiecznej aplikacji do interakcji z interfejsem API Partner Center API. 

Partnerzy, którzy nie przestrzegają tych praktyk w zakresie zabezpieczeń, mogą utracić możliwość wykonywania transakcji w programie CSP lub zarządzania dzierżawami klientów przy użyciu delegowanych praw administratora.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Czy wymagania dotyczące zabezpieczeń mają zastosowanie do wszystkich lokalizacji geograficznych?

Tak, wymagania dotyczące zabezpieczeń mają zastosowanie do wszystkich lokalizacji geograficznych. Zdecydowanie zaleca się, aby wszyscy partnerzy w ramach transakcji za pośrednictwem suwerennej chmury (rząd STANÓW Zjednoczonych i Niemcy) natychmiast zastosują te nowe wymagania dotyczące zabezpieczeń. Jednak ci partnerzy nie są obecnie zobowiązani do spełnienia wymagań dotyczących zabezpieczeń. Firma Microsoft udostępni dodatkowe szczegóły dotyczące wymuszania tych wymagań dotyczących zabezpieczeń suwerennych chmur w przyszłości.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Czy istnieje możliwość uzyskania wykluczenia dla konta?

Nie, nie można wykluczyć żadnego konta użytkownika z wymagania wymuszania uwierzytelniania wieloskładnikowego (MFA). Biorąc pod uwagę wysoce uprzywilejowany charakter partnera, Microsoft Partner Agreement wymaga, aby uwierzytelnianie wieloskładnikowe było wymuszane dla każdego konta użytkownika w dzierżawie partnera.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Jak mogę czy spełniliśmy wymagania dotyczące zabezpieczeń partnera?

Wykonaj poniższe czynności:

- Musisz spełnić wszystkie wymagania opisane w wymaganiach dotyczących [zabezpieczeń partnera.](partner-security-requirements.md)
- Należy upewnić się, że wszystkie konta użytkowników w dzierżawie partnera mają wymuszone uwierzytelnianie wieloskładnikowe.

Aby ułatwić zidentyfikowanie kluczowych obszarów, w [](https://partner.microsoft.com/commerce/security/compliance) których można podjąć działania, udostępniamy raport o stanie wymagań dotyczących zabezpieczeń, który jest dostępny za pośrednictwem Partner Center.

Aby uzyskać więcej informacji na temat raportu o stanie, zobacz [Partner security requirements status (Stan wymagań zabezpieczeń partnera).](partner-security-compliance.md)

## <a name="required-actions"></a>Wymagane akcje

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Jakie są kluczowe akcje, które należy podjąć, aby spełnić wymagania?

Wszyscy partnerzy w programie CSP (rachunek bezpośredni, dostawca pośredni i odsprzedawca pośredni), doradcy i dostawcy Panel sterowania muszą spełniać wymagania.

1. **Wymuszanie uwierzytelniania wieloskładnikowego dla wszystkich użytkowników**

    Wszyscy partnerzy w programie CSP, doradcy i dostawcy Panel sterowania są zobowiązani do wymuszania uwierzytelniania wieloskładnikowego dla wszystkich użytkowników w dzierżawie partnera.

    Dodatkowe kwestie do rozważenia:

    - Dostawcy pośredni muszą współpracować z odsprzedawcami pośrednimi, aby doćć do Partner Center, jeśli jeszcze tego nie zrobili, i zachęcić odsprzedawców do spełnienia wymagań.
    - Usługa Azure MFA jest dostępna dla wszystkich użytkowników w dzierżawie partnera bez poniesień kosztów dzięki domyślnym wartościom zabezpieczeń usługi Azure AD z jedyną metodą weryfikacji aplikacji wystawcy uwierzytelnień, która obsługuje jednorazowe hasła oparte na czasie (TOTP).
    - Dodatkowe metody weryfikacji są dostępne za [pośrednictwem Azure Active Directory — wersja Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU, jeśli są wymagane inne metody, takie jak połączenie telefoniczne lub wiadomość SMS.
    - Partnerzy mogą również używać rozwiązania mfa innej firmy dla każdego konta podczas uzyskiwania dostępu do komercyjnych usług w chmurze firmy Microsoft.

2. **Adopt the model aplikacji zabezpieczonych framework**

    Wszyscy partnerzy, którzy opracowali integrację niestandardową przy użyciu dowolnych interfejsów API (takich jak Azure Resource Manager, Microsoft Graph, Partner Center API itp.) lub wdrożyli automatyzację niestandardową przy użyciu narzędzi takich jak program PowerShell, będą musieli wdrożyć platformę [model aplikacji zabezpieczonych](/partner-center/develop/enable-secure-app-model) w celu integracji z usługami w chmurze firmy Microsoft. Niewykonanie tej pracy może spowodować zakłócenie z powodu wdrożenia usługi MFA. Poniższe zasoby zawierają omówienie i wskazówki dotyczące sposobu przyjęcia modelu.

    - [model aplikacji zabezpieczonych omówienie](/partner-center/develop/enable-secure-app-model)
    - [Partner Center: model aplikacji zabezpieczonych przewodnik](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partnerzy w programie CSP: przykładowy kod dla programu .NET umożliwiający model aplikacji zabezpieczonych](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partnerzy w programie CSP: przykładowy kod Java umożliwiający włączenie model aplikacji zabezpieczonych](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Partner Center uwierzytelniania](/partner-center/develop/partner-center-authentication)
    - [Partner Center dokumentu usługi Multi-Factor Authentication (MFA) programu PowerShell](/powershell/partnercenter/multi-factor-auth)

    Skontaktuj się z dostawcą, jeśli używasz panelu sterowania w zakresie wdrożenia model aplikacji zabezpieczonych platformie.

    Dostawcy panelu sterowania [](enroll-as-cpv.md) muszą do nich do Partner Center jako dostawca panelu sterowania i natychmiast rozpocząć wdrażanie tego wymagania. Zapoznaj się z [Partner Center: model aplikacji zabezpieczonych framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dostawcy panelu sterowania muszą zaakceptować zgodę partnerów CSP i zarządzać nimi zamiast poświadczeń i przeczyścić poświadczenia wszystkich istniejących partnerów CSP.

## <a name="multi-factor-authentication"></a>Uwierzytelnianie wieloskładnikowe

### <a name="what-is-multi-factor-authentication-mfa"></a>Co to jest uwierzytelnianie wieloskładnikowe (MFA)?

Uwierzytelnianie wieloskładnikowe to mechanizm zabezpieczeń do uwierzytelniania osób za pomocą więcej niż jednej wymaganej procedury zabezpieczeń i weryfikacji. Działa to przez wymaganie co najmniej dwóch następujących metod uwierzytelniania:

- Coś, co znasz (zwykle hasło)
- Coś, co masz (zaufane urządzenie, które nie jest łatwo zduplikowane, na przykład telefon)
- Coś, co jest (biometria)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Jaki jest koszt włączania usługi MFA?

Firma Microsoft udostępnia uwierzytelniania wieloskładnikowego bez poniesienie kosztów dzięki implementacji ustawień domyślnych zabezpieczeń usługi Azure AD. Jedyną opcją weryfikacji dostępną przy użyciu tej wersji uwierzytelniania wieloskładnikowego jest aplikacja wystawcy uwierzytelniań. Jeśli wymagane jest połączenie telefoniczne lub wiadomość SMS, [należy Azure Active Directory — wersja Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) licencję usługi. Alternatywnie można użyć rozwiązania innej firmy, aby zapewnić uwierzytelniania wieloskładnikowego dla każdego użytkownika w dzierżawie partnera — w tym przypadku odpowiedzialność za zapewnienie wymuszania i zgodności rozwiązania mfa.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Jakie akcje należy wykonać, jeśli mam już rozwiązanie MFA?

Dzięki tym wymaganiom dotyczącym zabezpieczeń użytkownicy w dzierżawie partnera będą zobowiązani do uwierzytelniania przy użyciu usługi MFA podczas uzyskiwania dostępu do komercyjnych usług w chmurze firmy Microsoft. Rozwiązania innych firm mogą służyć do spełnienia tych wymagań. Firma Microsoft nie zapewnia już testowania poprawności niezależnym dostawcom tożsamości w celu zapewnienia zgodności z Azure Active Directory. Aby przetestować współdziałanie produktu, zapoznaj się z tymi [wytycznymi.](https://www.microsoft.com/download/details.aspx?id=56843)

> [!IMPORTANT]
> W przypadku korzystania z rozwiązania innej firmy ważne jest, aby sprawdzić, czy rozwiązanie wystawia oświadczenie odwołania do metody uwierzytelniania (AMR), które zawiera wartość usługi MFA. Zobacz [Testing the Partner Security Requirements (Testowanie](/powershell/partnercenter/test-partner-security-requirements) wymagań zabezpieczeń partnera), aby uzyskać szczegółowe informacje na temat sposobu wystawiania oczekiwanego oświadczenia przez rozwiązanie innej firmy.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Do transakcji używam wielu dzierżaw partnerów. Czy muszę zaimplementować uwierzytelniania wieloskładnikowego na nich wszystkich?

Tak, należy wymusić uwierzytelniania wieloskładnikowego dla każdej dzierżawy Azure Active Directory skojarzonej z programem CSP lub programem Advisor. Aby kupić licencję Azure Active Directory — wersja Premium, musisz zakupić licencję Azure Active Directory dla użytkowników w każdej Azure Active Directory dzierżawie. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Czy każde konto użytkownika w dzierżawie partnera musi mieć wymuszone uwierzytelniania wieloskładnikowego?

Tak, każdy użytkownik musi mieć wymuszone uwierzytelniania wieloskładnikowego. Jeśli jednak używasz ustawień domyślnych zabezpieczeń usługi Azure AD, nie jest wymagane żadne dodatkowe działanie, ponieważ ta funkcja wymusza uwierzytelniania wieloskładnikowego dla wszystkich kont użytkowników. Włączenie wartości domyślnych zabezpieczeń jest bezpłatnym i łatwym sposobem zapewnienia, że konta użytkowników są zgodne z usługą MFA i nie mają na nie wpływu, gdy uwierzytelniania wieloskładnikowego jest wymuszane.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Jestem bezpośrednim partnerem w firmie Microsoft. Co mam zrobić?

Bezpośredni partnerzy Dostawca rozwiązań w chmurze muszą wymuszać uwierzytelniania wieloskładnikowego dla każdego użytkownika w dzierżawie partnera.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Jestem odsprzedawcą pośrednim i transakcję mogę tylko za pośrednictwem dystrybutora. Czy nadal muszę włączyć usługę MFA?

Wszyscy odsprzedawcy pośredni są zobowiązani do wymuszenia uwierzytelniania wieloskładnikowego dla każdego użytkownika w dzierżawie partnera. Odsprzedawca pośredni musi włączyć usługę MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Nie używam interfejsu API Partner Center. Czy nadal muszę zaimplementować uwierzytelniania wieloskładnikowego?

Tak, to wymaganie dotyczące zabezpieczeń dotyczy wszystkich użytkowników, w tym administratorów partnerów i użytkowników końcowych w dzierżawie partnera.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Którzy dostawcy innych firm zapewniają rozwiązania MFA zgodne z Azure Active Directory?

Podczas przeglądania dostawców i rozwiązań usługi MFA partnerzy muszą upewnić się, że wybierane rozwiązanie jest zgodne z Azure Active Directory.

Firma Microsoft nie zapewnia już testowania poprawności niezależnym dostawcom tożsamości w celu zapewnienia zgodności z Azure Active Directory. Jeśli chcesz przetestować współdziałanie produktu, zapoznaj się z tymi [wytycznymi.](https://www.microsoft.com/download/details.aspx?id=56843)

Aby uzyskać więcej informacji, zobacz listę [zgodności federacji usługi Azure AD.](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Jak przetestować usługę MFA w piaskownicy integracji?

Należy włączyć funkcję ustawień domyślnych zabezpieczeń usługi Azure AD lub użyć rozwiązania innej firmy, które korzysta z federacji.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Czy włączenie uwierzytelniania wieloskładnikowego będzie miało wpływ na sposób interakcji z dzierżawą klienta?

Nie. Spełnienie tych wymagań dotyczących zabezpieczeń nie będzie miało wpływu na sposób zarządzania klientami. Możliwość wykonywania delegowanych operacji administracyjnych nie zostanie przerwana.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Czy moi klienci podlegają wymogom zabezpieczeń partnera?

Nie, nie jest wymagane wymuszanie uwierzytelniania wieloskładnikowego dla każdego użytkownika w dzierżawach usługi Azure AD klienta. Zaleca się jednak, aby we współpracy z każdym klientem określić najlepszą ochronę użytkowników.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Czy dowolny użytkownik może zostać wykluczony z wymagania uwierzytelniania wieloskładnikowego?

Nie, każdy użytkownik, w tym konta usług, w dzierżawie partnera będzie wymagany do uwierzytelniania przy użyciu usługi MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Czy wymagania dotyczące zabezpieczeń partnerów mają zastosowanie do piaskownicy integracji?

Tak, wymagania dotyczące zabezpieczeń partnerów mają zastosowanie do piaskownicy integracji. Oznacza to, że konieczne będzie wdrożenie odpowiedniego rozwiązania MFA dla użytkowników w dzierżawie piaskownicy integracji. Zaleca się zaimplementowanie ustawień domyślnych zabezpieczeń usługi Azure AD w celu zapewnienia uwierzytelniania wieloskładnikowego.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Jak mogę skonfigurować konto dostępu awaryjnego ?.

Najlepszym rozwiązaniem jest utworzenie jednego lub dwóch kont dostępu awaryjnego, aby zapobiec przypadkowemu zablokowaniu dzierżawy usługi Azure AD. W odniesieniu do wymagań dotyczących zabezpieczeń partnera wymagane jest, aby każdy użytkownik uwierzytelnił się przy użyciu usługi MFA. To wymaganie oznacza, że musisz zmodyfikować definicję konta dostępu awaryjnego. Może to być konto, które korzysta z rozwiązania innej firmy do uwierzytelniania wieloskładnikowego.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Czy usługa Active Directory usługa federacyjna (ADFS) jest wymagana, jeśli korzystam z rozwiązania innej firmy?

Nie, jeśli używasz rozwiązania innej firmy, nie jest wymagane używanie usługi Active Directory usługa federacyjna (ADFS). Zaleca się, aby we współpracy z dostawcą rozwiązania określić, jakie są wymagania dotyczące jego rozwiązania.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Czy wymagane jest włączenie wartości domyślnych zabezpieczeń usługi Azure AD?

Nie. Nie jest wymagane włączenie domyślnych ustawień zabezpieczeń usługi Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Czy można użyć dostępu warunkowego, aby spełnić wymaganie uwierzytelniania wieloskładnikowego?

Tak, możesz użyć dostępu warunkowego, aby wymusić uwierzytelniania wieloskładnikowego dla każdego użytkownika, w tym kont usług, w dzierżawie partnera. Jednak ze względu na wysoce uprzywilejowany charakter partnera musimy upewnić się, że każdy użytkownik ma zadanie uwierzytelniania wieloskładnikowego dla każdego pojedynczego uwierzytelniania. Oznacza to, że nie będzie można korzystać z funkcji dostępu warunkowego, która pomija wymaganie uwierzytelniania wieloskładnikowego.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Czy na konto usługi używane przez Azure AD Connect będą miały wpływ wymagania dotyczące zabezpieczeń partnera?

Nie, na konto usługi używane przez Azure AD Connect nie będą miały wpływu wymagania dotyczące zabezpieczeń partnera. Jeśli wystąpi problem z usługą Azure AD Connect w wyniku wymuszania uwierzytelniania wieloskładnikowego, otwórz wniosek o pomoc techniczną do pomocy technicznej firmy Microsoft.

## <a name="secure-application-model"></a>model aplikacji zabezpieczonych

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Kto powinien przyjąć bezpieczny model aplikacji, aby spełnić wymagania?

Firma Microsoft wprowadza bezpieczną, skalowalną platformę do uwierzytelniania partnerów Dostawca rozwiązań w chmurze (CSP) i dostawców Panel sterowania (CPV), która korzysta z uwierzytelniania wieloskładnikowego. Aby uzyskać więcej informacji, zobacz [model aplikacji zabezpieczonych przewodniku .](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Wszyscy partnerzy, którzy opracowali niestandardową integrację przy użyciu dowolnych interfejsów API (takich jak Azure Resource Manager, Microsoft Graph, Partner Center API itp.) lub wdrożyli automatyzację niestandardową przy użyciu narzędzi takich jak program PowerShell, będą musieli wdrożyć platformę [model aplikacji zabezpieczonych](/partner-center/develop/enable-secure-app-model) w celu integracji z usługami w chmurze firmy Microsoft.

### <a name="what-is-the-secure-application-model"></a>Co to jest model aplikacji zabezpieczonych?

Firma Microsoft wprowadza bezpieczną, skalowalną platformę do uwierzytelniania partnerów Dostawca rozwiązań w chmurze (CSP) i dostawców Panel sterowania (CPV), która korzysta z uwierzytelniania wieloskładnikowego. Zobacz przewodnik [model aplikacji zabezpieczonych, aby](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) uzyskać więcej informacji.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Jak mogę zaimplementować model aplikacji zabezpieczonych?

Wszyscy partnerzy, którzy opracowali integrację niestandardową przy użyciu dowolnych interfejsów API (takich jak Azure Resource Manager, Microsoft Graph, Partner Center API itp.) lub wdrożyli automatyzację niestandardową przy użyciu narzędzi takich jak program PowerShell, będą musieli wdrożyć platformę [model aplikacji zabezpieczonych](/partner-center/develop/enable-secure-app-model) w celu integracji z usługami w chmurze firmy Microsoft. Niewykonanie tej pracy może spowodować zakłócenie z powodu wdrożenia usługi MFA. Poniższe zasoby zawierają omówienie i wskazówki dotyczące sposobu przyjęcia modelu.

- [model aplikacji zabezpieczonych omówienie](/partner-center/develop/enable-secure-app-model)
- [Partner Center: model aplikacji zabezpieczonych przewodnik](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerzy w programie CSP: przykładowy kod dla programu .NET umożliwiający model aplikacji zabezpieczonych](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerzy w programie CSP: przykładowy kod Java umożliwiający włączenie model aplikacji zabezpieczonych](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partner Center uwierzytelniania](/partner-center/develop/partner-center-authentication)
- [Partner Center dokumentu usługi Multi-Factor Authentication (MFA) programu PowerShell](/powershell/partnercenter/multi-factor-auth)

Jeśli używasz panelu sterowania, musisz skonsultować się z dostawcą w sprawie wdrożenia model aplikacji zabezpieczonych framework.

Dostawcy panelu sterowania [](enroll-as-cpv.md) muszą do nich do Partner Center jako dostawca panelu sterowania i natychmiast rozpocząć wdrażanie tego wymagania. Zapoznaj się z [Partner Center: model aplikacji zabezpieczonych framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dostawcy panelu sterowania muszą zaakceptować zgodę partnerów CSP i zarządzać nimi zamiast poświadczeń i przeczyścić poświadczenia wszystkich istniejących partnerów CSP.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Czy model aplikacji zabezpieczonych musi być zaimplementowany tylko dla interfejsu API/zestawu SDK Partner Center?

Wymuszanie uwierzytelniania wieloskładnikowego dla wszystkich kont użytkowników będzie miało wpływ na automatyzację lub integrację, która ma być uruchamiana nieinterakcyjnie. Chociaż wymagania dotyczące zabezpieczeń partnerów wymagają włączenia bezpiecznego modelu aplikacji dla interfejsu API usługi Partner Center, można go użyć do rozwiązania potrzeby drugiego czynnika uwierzytelniania z automatyzacją i integracją.

>[!Note] 
>Zasoby, do których uzyskuje się dostęp, muszą obsługiwać uwierzytelnianie oparte na tokenach dostępu.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Korzystam z narzędzi automatyzacji, takich jak program PowerShell. Jak mogę zaimplementować model aplikacji zabezpieczonych?

Jeśli automatyzacja ma być uruchamiana nieinterakcyjnie i opiera się na poświadczeniach użytkownika na potrzeby model aplikacji zabezpieczonych uwierzytelniania, konieczne będzie zaimplementowanie tej funkcji. Zobacz [model aplikacji zabezpieczonych | Partner Center programu PowerShell,](/powershell/partnercenter/multi-factor-auth) aby uzyskać wskazówki dotyczące sposobu implementacji tej struktury.  

>[!Note] 
>Nie wszystkie narzędzia automatyzacji zapewniają możliwość uwierzytelniania przy użyciu tokenów dostępu. Jeśli potrzebujesz pomocy w zrozumieniu, jakie zmiany należy [wprowadzić,](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) opublikuj komunikat w grupie wskazówki dotyczące zabezpieczeń usługi Partner Center. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Jakie poświadczenia użytkownika powinien podać administrator aplikacji podczas procesu wyrażania zgody?

Zalecane jest użycie konta usługi, do których przypisano najmniej uprzywilejowane uprawnienia. W odniesieniu do Partner Center API należy użyć konta, które zostało przypisane do roli Agent sprzedaży lub Agenci administracyjni.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Dlaczego administrator aplikacji nie powinien poświadczeń użytkownika administratora globalnego podczas wykonywania procesu wyrażania zgody?

Najlepszym rozwiązaniem jest użycie tożsamości z najmniejszymi uprawnieniami.  Spowoduje to zmniejszenie ryzyka. Nie zaleca się używania konta z uprawnieniami administratora globalnego, ponieważ zapewniałoby to więcej uprawnień niż jest to wymagane.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Jestem partnerem programu CSP. Jak mogę, czy mój Panel sterowania (CPV) pracuje nad wdrożeniem rozwiązania?

W przypadku partnerów korzystających z rozwiązania dostawcy Panel sterowania (CPV) do transakcji w programie Dostawca rozwiązań w chmurze (CSP) odpowiadasz za skonsultowanie się z dostawcą CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Kto jest dostawcą Panel sterowania (CPV)?

Dostawca Panel sterowania to niezależny dostawca oprogramowania, który opracowuje aplikacje do użycia przez partnerów programu CSP w celu integracji z Partner Center API. Dostawca Panel sterowania nie jest partnerem programu CSP z bezpośrednim dostępem do pulpitu nawigacyjnego Partner Center lub interfejsów API. Szczegółowy opis jest dostępny w [przewodniku Partner Center: Model bezpiecznych aplikacji.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Jestem CPV. Jak mogę zarejestrować?

Aby zarejestrować się jako dostawca panelu sterowania (CPV), postępuj zgodnie z wytycznymi w tym [miejscu.](enroll-as-cpv.md)

W celu otrzymania linku rejestracji lub podania sponsora pracownika firmy Microsoft, który ma relację biznesową z kontem CPV lub zna swoją firmę, musi skontaktować się z działem [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) firmy Microsoft. Na przykład Partner Development Manager (PDM).

Po zarejestrowaniu Partner Center i zarejestrowaniu aplikacji będziesz mieć dostęp do Partner Center API. Informacje o piaskownicy otrzymasz za pośrednictwem Partner Center, jeśli jesteś nowym użytkownikiem CPV. Po zakończeniu rejestracji jako konto CPV firmy Microsoft i zaakceptowaniu umowy CPV można:

1. Zarządzanie aplikacją wielodostępną (dodawanie aplikacji do Azure Portal oraz rejestrowanie i wyrejestrowynie aplikacji w Partner Center).

   >[!Note]
   >Aby uzyskać autoryzację dla interfejsów API Partner Center CPV, Partner Center rejestrować swoje aplikacje w Partner Center. Dodawanie aplikacji tylko do Azure Portal nie powoduje autoryzowania aplikacji CPV dla Partner Center API.

1. Wyświetlanie profilu CPV i zarządzanie tym profilem.

1. Wyświetlanie użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzanie nimi. Protokół CPV może mieć tylko rolę Administrator globalny.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Korzystam z zestaw SDK Centrum partnerskiego. Czy zestaw SDK automatycznie zastosuje model aplikacji zabezpieczonych?

Nie, należy postępować zgodnie z wytycznymi w przewodniku model aplikacji zabezpieczonych [usługi](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Czy mogę wygenerować token odświeżania dla modelu bezpiecznej aplikacji z kontami, które nie mają włączonej usługi MFA?

Tak, token odświeżania można wygenerować przy użyciu konta, które nie ma wymuszania uwierzytelniania wieloskładnikowego. Należy tego jednak unikać. Token wygenerowany przy użyciu konta, które nie ma włączonej usługi MFA, nie będzie mógł uzyskać dostępu do zasobów ze względu na wymaganie uwierzytelniania wieloskładnikowego.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Jak moja aplikacja powinna uzyskać token dostępu, jeśli włączymy usługę MFA?

Należy postępować zgodnie z [model aplikacji zabezpieczonych,](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) który zawiera szczegółowe informacje na temat tego, jak to zrobić przy zachowaniu zgodności z nowymi wymaganiami w zakresie zabezpieczeń. Przykładowy kod .NET można znaleźć [tutaj,](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) a przykładowy kod Java można [znaleźć tutaj.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Czy w ramach protokołu CPV mogę utworzyć aplikację usługi Azure AD w dzierżawie CPV, czy dzierżawie partnera CSP?

Protokół CPV musi utworzyć aplikację Azure Active Directory dzierżawie skojarzoną z rejestracją jako CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Jestem CSP, który korzysta z uwierzytelniania tylko aplikacji. Czy muszę wprowadzić jakieś zmiany?

Nie ma to wpływu na uwierzytelnianie tylko aplikacji, ponieważ poświadczenia użytkownika nie są używane do żądania tokenu dostępu. Jeśli poświadczenia użytkownika są udostępniane, dostawcy panelu sterowania muszą [](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) przyjąć platformę model aplikacji zabezpieczonych i przeczyścić wszystkie istniejące poświadczenia partnera, które mają.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Czy jako protokół CPV mogę wykorzystać styl uwierzytelniania tylko aplikacji, aby uzyskać tokeny dostępu?

Nie, Panel sterowania dostawcy nie mogą używać stylu uwierzytelniania tylko aplikacji do żądania tokenów dostępu w imieniu partnera. Powinni oni zaimplementować bezpieczny model aplikacji, który wykorzystuje styl uwierzytelniania aplikacji i użytkownika.

## <a name="technical-enforcement"></a>Wymuszanie techniczne

### <a name="what-is-the-activation-of-security-safeguards"></a>Co to jest aktywacja zabezpieczeń?

Wszyscy partnerzy biorący udział w programie Dostawca rozwiązań w chmurze (CSP), dostawcy Panel sterowania (CPV) i doradcy powinni zaimplementować obowiązkowe wymagania dotyczące zabezpieczeń, aby zachować zgodność.

Aby zapewnić dodatkową ochronę, firma Microsoft rozpoczęła aktywację zabezpieczeń, które pomagają partnerom w zabezpieczaniu ich dzierżaw i klientów przez upoważnianie weryfikacji uwierzytelniania wieloskładnikowego (MFA) w celu zapobiegania nieautoryzowanemu dostępowi.  

Pomyślnie ukończyliśmy aktywację funkcji admin-on-behalf-of (AOBO) dla wszystkich dzierżaw partnerów. Aby jeszcze bardziej ułatwić ochronę partnerów i klientów w drugim kwartale 2020 r., rozpoczniemy aktywację dla transakcji usługi Partner Center w programie CSP, pomagając partnerom chronić firmy i klientów przed zdarzeniami związanymi z kradzieżą tożsamości.

Aby uzyskać więcej informacji, [odwiedź stronę Wymuszanie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy](partner-security-requirements-mandating-mfa.md) partnera.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Korzystam z rozwiązania uwierzytelniania wieloskładnikowego innej firmy i mam zablokowaną możliwość. Co mam zrobić?

Aby sprawdzić, czy konto, do których uzyskuje dostęp do zasobów, [](https://tools.ietf.org/html/rfc8176) zostało zakwestionowane w celu uwierzytelnienia wieloskładnikowego, sprawdzimy oświadczenie referencyjne metody uwierzytelniania, aby sprawdzić, czy uwierzytelnianie wieloskładnikowe jest wyświetlane. Niektóre rozwiązania innych firm nie wystawiają tego oświadczenia lub nie zawierają wartości uwierzytelniania wieloskładnikowego. Jeśli brakuje oświadczenia lub wartość uwierzytelniania wieloskładnikowego nie jest wymieniona, nie ma możliwości ustalenia, czy uwierzytelnione konto zostało zakwestionowane na potrzeby uwierzytelniania wieloskładnikowego. Należy współpracować z dostawcą rozwiązania innej firmy, aby określić, jakie działania należy podjąć, aby rozwiązanie wystawiało oświadczenie referencyjne metody uwierzytelniania.

Zobacz [Temat Testing the Partner Security Requirements](/powershell/partnercenter/test-partner-security-requirements) if you'm unsure if your third-party solution is issuing the expected claim or not (Testowanie wymagań zabezpieczeń partnera, jeśli nie masz pewności, czy twoje rozwiązanie innej firmy wystawia oczekiwane oświadczenie).

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>Uwierzytelniania wieloskładnikowego blokuje mi obsługę mojego klienta przy użyciu AOBO. Co mam zrobić?

Wymuszanie techniczne wymagań dotyczących zabezpieczeń partnera zostanie sprawdzone, jeśli uwierzytelnione konto zostało zakwestionowane w celu uwierzytelnienia wieloskładnikowego. Jeśli konto nie zostało, nastąpi przekierowanie do strony logowania i ponownie wyświetlony monit o uwierzytelnienie. Zapoznaj się z dodatkowymi wskazówkami i wskazówkami w tej dokumentacji dzierżawy partnera w zakresie uwierzytelniania [wieloskładnikowego (MFA).](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) W scenariuszu, w którym domena nie jest federowana, po pomyślnym uwierzytelnieniu zostanie wyświetlony monit o skonfigurowanie uwierzytelniania wieloskładnikowego. Po zakończeniu będzie można zarządzać klientami przy użyciu funkcji AOBO. W scenariuszu, w którym domena jest federowana, należy upewnić się, że konto jest wymagane do uwierzytelniania wieloskładnikowego.

## <a name="security-defaults-transition"></a>Przejście ustawień domyślnych zabezpieczeń

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Jak przejść z zasad bazowych do ustawień domyślnych zabezpieczeń lub innych rozwiązań MFA?

Azure Active Directory "linii [bazowej"](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) (Azure AD) są usuwane i zastępowane "wartościami domyślnymi zabezpieczeń", czyli bardziej kompleksowym zestawem zasad ochrony dla Ciebie i Twoich klientów. [Wartości domyślne zabezpieczeń mogą](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) pomóc w ochronie organizacji przed atakami bezpieczeństwa związanymi z kradzieżą tożsamości.

Implementacja uwierzytelniania wieloskładnikowego (MFA) zostanie usunięta z powodu wycofania zasad bazowych, jeśli nie została przełączona z zasad bazowych do zasad domyślnych zabezpieczeń lub innych opcji implementacji usługi [MFA.](partner-security-requirements.md#implementing-multi-factor-authentication) Każdy użytkownik w dzierżawach partnerskich wykonujący operacje chronione za pomocą uwierzytelniania wieloskładnikowego będzie żądał ukończenia weryfikacji uwierzytelniania wieloskładnikowego. Zapoznaj się z bardziej szczegółowymi [wskazówkami tutaj.](partner-security-requirements-mandating-mfa.md)
Aby zachować zgodność i zminimalizować zakłócenia, należy podjąć jedną z następujących czynności:

- Przejście do ustawień domyślnych zabezpieczeń
    - Zasady wartości domyślnych zabezpieczeń to jedna z opcji, które partnerzy mogą zdecydować się na wdrożenie usługi MFA. Oferuje ona podstawowy poziom zabezpieczeń włączony bez dodatkowych kosztów.
    - Dowiedz się, jak włączyć uwierzytelniania wieloskładnikowego dla organizacji za pomocą usługi Azure AD i zapoznaj się z [kluczowymi zagadnieniami na temat ustawień domyślnych zabezpieczeń.](partner-security-requirements.md#security-defaults)
    - Włącz domyślne zasady zabezpieczeń, jeśli spełniają one potrzeby biznesowe.
- Przejście do dostępu warunkowego
    - Jeśli zasady domyślne zabezpieczeń nie są potrzebne, włącz dostęp warunkowy. Aby uzyskać więcej informacji, zapoznaj się z dokumentacją dostępu warunkowego usługi Azure AD.

## <a name="key-resources"></a>Kluczowe zasoby

### <a name="how-to-get-started"></a>Jak zacząć

- [Wymagania dotyczące zabezpieczeń partnerów: przewodnik krok po kroku.](partner-security-requirements.md)
- Pytania i opinie należy kierować do tej [grupy Partner Center Security Guidance Group.](https://aka.ms/MPCSecurityGuidance)
- Weź udział w nadchodzących godzinach pracy partnera i seminariach internetowych. Szczegółowe informacje [o harmonogramie i zasobach można sprawdzić tutaj.](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)

### <a name="resources-for-adopting-secure-application-model"></a>Zasoby dotyczące adoptowania bezpiecznego modelu aplikacji

- [model aplikacji zabezpieczonych omówienie](/partner-center/develop/enable-secure-app-model)
- [Partner Center: model aplikacji zabezpieczonych przewodnik](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerzy w programie CSP: przykładowy kod programu .NET umożliwiający model aplikacji zabezpieczonych](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerzy w programie CSP: przykładowy kod Java umożliwiający model aplikacji zabezpieczonych](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partner Center uwierzytelniania](/partner-center/develop/partner-center-authentication)
- [Partner Center dokumentu usługi Multi-Factor Authentication (MFA) programu PowerShell](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Pomoc techniczna

### <a name="where-can-i-get-support"></a>Gdzie mogę uzyskać pomoc techniczną?

Aby uzyskać zasoby pomocy technicznej spełniające wymagania dotyczące zabezpieczeń, jeśli masz zaawansowaną pomoc techniczną dla partnerów (ASfP), skontaktuj się z menedżerem konta usługi. W przypadku umowy Pomocy technicznej Premier dla partnerów (PSfP) skontaktuj się z menedżerem kont usług i menedżerem ds. technicznych kont.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Jak mogę uzyskać informacje techniczne i pomoc techniczną, które pomogą mi w przyjęcie bezpiecznej struktury modelu aplikacji?

Opcje pomocy technicznej produktu Azure Active Directory są dostępne za pośrednictwem twoich korzyści związanych z mpn. Partnerzy z dostępem do aktywnej subskrypcji ASfP lub PSfP mogą współpracować ze skojarzonym menedżerem kont (SAM/TAM), aby najlepiej zrozumieć dostępne opcje.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Jak mogę skontaktować się z pomocą techniczną, jeśli utraciłem dostęp do Partner Center?

Jeśli utracisz dostęp z powodu problemu z usługą MFA, skontaktuj się z administratorem globalnym dzierżawy. Wewnętrzny dział IT będzie mógł poinformować Cię, kim jest administrator globalny. 

Jeśli nie pamiętasz hasła, przeczytaj [nie można zalogować się, aby](unable-to-sign-in.md) uzyskać pomoc.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Gdzie można znaleźć więcej informacji na temat typowych problemów technicznych?

Informacje dotyczące typowych problemów technicznych można znaleźć w te tematach Partner security requirements for partners using Partner Center or Partner Center APIs (Wymagania dotyczące zabezpieczeń partnerów korzystających z interfejsów API Partner Center [lub Partner Center partnerów)](partner-security-requirements.md)