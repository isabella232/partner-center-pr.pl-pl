---
title: Wymagania dotyczące zabezpieczeń partnerów — często zadawane pytania
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Często zadawane pytania dotyczące wymagań związanych z bezpieczeństwem partnerów — co to są, w jaki sposób partnerzy powinni je zaimplementować oraz jak wiadomo, czy zostały one spełnione.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f2bf6823fdd976632fb8ad9c8f11ce99835d76a5
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087080"
---
# <a name="common-questions-about-partner-security-requirements"></a>Często zadawane pytania dotyczące wymagań dotyczących zabezpieczeń partnerów

**Odpowiednie role**

- Wszyscy użytkownicy Centrum partnerskiego

Ten artykuł zawiera odpowiedzi na niektóre często zadawane pytania dotyczące [wymagań dotyczących zabezpieczeń partnerów](partner-security-requirements.md).

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Jakie są wymagania dotyczące zabezpieczeń partnerów i Dlaczego partnerzy implementują je?

Większe i aktualne zabezpieczenia dotyczące zabezpieczeń i ochrony prywatności znajdują się wśród naszych najważniejszych priorytetów i będziemy nadal pomagać partnerom chronić klientów i dzierżawców. Nadal widzimy bardziej zaawansowane, zwiększając liczbę ataków na zabezpieczenia, głównie związanych ze zdarzeniami naruszenia tożsamości. Ponieważ kontrole prewencyjne odgrywają kluczową rolę w ogólnej strategii obrony przed atakami z wykorzystaniem zabezpieczeń, wprowadziliśmy [obowiązkowe wymagania dotyczące bezpieczeństwa](partner-security-requirements.md) w 2019. Wszyscy partnerzy uczestniczący w programie dostawcy rozwiązań w chmurze (CSP), dostawcy panelu sterowania i doradcy muszą zaimplementować wymagania, aby zachować zgodność.

### <a name="what-are-the-key-timelines-and-milestones"></a>Jakie są kluczowe osie czasu i punkty kontrolne?

Warunki związane z tymi wymaganiami dotyczącymi zabezpieczeń, w tym osie czasu i punkty kontrolne, są zawarte w [umowie partnerskiej firmy Microsoft](microsoft-partner-agreement.md). Należy zaimplementować te wymagania dotyczące zabezpieczeń tak szybko, jak to możliwe, aby zachować zgodność z uczestnictwem w programie CSP.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Co się stanie, jeśli nie zostaną zaimplementowane te wymagania dotyczące zabezpieczeń partnerów?

Umowa partnerska firmy Microsoft wymaga wymuszenia uwierzytelniania wieloskładnikowego dla kont użytkowników i przyjęcia bezpiecznego modelu aplikacji na potrzeby współpracy z interfejsem API Centrum partnerskiego. 

Partnerzy, którzy nie przestrzegają tych praktyk w zakresie zabezpieczeń, mogą utracić możliwość wykonywania operacji Transact w programie CSP lub zarządzać dzierżawcami klientów przy użyciu delegowania praw administratora.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Czy wymagania dotyczące zabezpieczeń mają zastosowanie do wszystkich lokalizacje geograficzne?

Tak, wymagania dotyczące zabezpieczeń mają zastosowanie do wszystkich lokalizacje geograficzne. Zdecydowanie zalecamy, aby wszyscy partnerzy zajmujący się prowadzeniem działalności w chmurze suwerennej (rząd Stanów Zjednoczonych i Niemcy) bezzwłocznie zadziałali i przyjmują nowe wymagania dotyczące zabezpieczeń. Jednak ci partnerzy nie są obecnie zobowiązani do spełnienia wymagań dotyczących zabezpieczeń. Firma Microsoft zapewni dodatkowe szczegóły dotyczące wymuszania tych wymagań w zakresie bezpieczeństwa dla suwerennych chmur w przyszłości.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Czy jest możliwe wykluczenie konta?

Nie, nie jest możliwe wykluczenie żadnego konta użytkownika z wymogu posiadania uwierzytelniania wieloskładnikowego (MFA). Mając wysoce uprzywilejowany charakter partnera, umowa partnerska firmy Microsoft wymaga, aby uwierzytelnianie wieloskładnikowe było wymuszane dla każdego konta użytkownika w dzierżawie partnerskiej.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Jak mogę sprawdzić, czy zostały spełnione wymagania dotyczące zabezpieczeń partnerów?

Wykonaj poniższe czynności:

- Musisz spełnić wszystkie wymagania opisane w [wymaganiach dotyczących zabezpieczeń partnerów](partner-security-requirements.md).
- Musisz upewnić się, że wszystkie konta użytkowników w dzierżawie partnera mają wymuszone uwierzytelnianie wieloskładnikowe.

Aby ułatwić zidentyfikowanie kluczowych obszarów, w których można podjąć działania, udostępniamy [raport o stanie wymagań dotyczących zabezpieczeń](https://partner.microsoft.com/commerce/security/compliance) , który jest dostępny za pomocą Centrum partnerskiego.

Aby uzyskać więcej informacji na temat raportu o stanie, zobacz [stan wymagań dotyczących zabezpieczeń partnerów](partner-security-compliance.md).

## <a name="required-actions"></a>Wymagane akcje

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Jakie kluczowe akcje należy wykonać, aby spełnić wymagania?

Wszyscy partnerzy w programie CSP (bezpośredni rachunek, Dostawca pośredni i pośredni odsprzedawca), doradcy i dostawcy panelu sterowania muszą spełniać wymagania.

1. **Wymuś uwierzytelnianie wieloskładnikowe dla wszystkich użytkowników**

    Wszyscy partnerzy w programie CSP, doradcy i dostawcy panelu sterowania muszą wymusić uwierzytelnianie wieloskładnikowe dla wszystkich użytkowników w dzierżawie partnera.

    Dodatkowe kwestie do rozważenia:

    - Dostawcy pośrednim muszą współpracować z pośrednimi odsprzedawcami, aby dołączyć do Centrum partnerskiego, jeśli nie zostało to jeszcze zrobione i zachęcić odsprzedawcy do spełnienia wymagań.
    - Usługa Azure MFA jest udostępniana dla wszystkich użytkowników w dzierżawie partnerów bez żadnych kosztów za pośrednictwem wartości domyślnych zabezpieczeń usługi Azure AD z jedyną metodą weryfikacji dla aplikacji wystawcy, która obsługuje hasła jednorazowe (TOTP).
    - Dodatkowe metody weryfikacji są dostępne za pomocą jednostek SKU [Azure Active Directory — wersja Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) , jeśli są wymagane inne metody, takie jak połączenie telefoniczne lub wiadomości SMS.
    - Partnerzy mogą również używać rozwiązania MFA innej firmy dla każdego konta podczas uzyskiwania dostępu do komercyjnych usług w chmurze firmy Microsoft.

2. **Zastosuj strukturę modelu bezpiecznej aplikacji**

    Wszyscy partnerzy, którzy utworzyli integrację niestandardową przy użyciu dowolnych interfejsów API (na przykład Azure Resource Manager, Microsoft Graph, interfejsu API centrum partnera itp.) lub zaimplementowano automatyzację niestandardową przy użyciu narzędzi takich jak program PowerShell, będą musieli wdrożyć [bezpieczną strukturę modelu aplikacji](/partner-center/develop/enable-secure-app-model) w celu integracji z usługami w chmurze firmy Microsoft. Niewykonanie tej czynności może skutkować zakłóceniem ze względu na wdrożenie usługi MFA. Poniższe zasoby zawierają omówienie i wskazówki dotyczące sposobu wdrażania modelu.

    - [Omówienie bezpiecznego modelu aplikacji](/partner-center/develop/enable-secure-app-model)
    - [Centrum partnerskie: bezpieczny model aplikacji — przewodnik](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partnerzy w programie CSP: przykładowy kod platformy .NET do włączenia bezpiecznego modelu aplikacji](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partnerzy w programie CSP: przykładowy kod w języku Java do włączenia bezpiecznego modelu aplikacji](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Dokument uwierzytelniania Centrum partnerskiego](/partner-center/develop/partner-center-authentication)
    - [Dokument programu PowerShell Centrum partnerskiego Multi-Factor Authentication (MFA)](/powershell/partnercenter/multi-factor-auth)

    Należy skontaktować się z dostawcą, jeśli używasz panelu sterowania dotyczącego wdrażania bezpiecznego środowiska modelu aplikacji.

    Aby [dołączyć](enroll-as-cpv.md) do Centrum partnerskiego jako dostawcę panelu sterowania i rozpocząć wdrażanie tego wymagania, wymagane są dostawcy panelu sterowania. Zapoznaj się z [centrum partnerskim: Secure Application model Framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dostawcy panelu sterowania muszą akceptować i zarządzać "zgodą partnerów usług kryptograficznych" zamiast poświadczeń i czyścić wszystkie istniejące poświadczenia partnerów programu CSP.

## <a name="multi-factor-authentication"></a>Uwierzytelnianie wieloskładnikowe

### <a name="what-is-multi-factor-authentication-mfa"></a>Co to jest uwierzytelnianie wieloskładnikowe (MFA)?

MFA to mechanizm zabezpieczeń służący do uwierzytelniania osób przez więcej niż jedną wymaganą procedurę zabezpieczeń i walidacji. Działa przez wymaganie co najmniej dwóch następujących metod uwierzytelniania:

- Coś, co wiesz (zazwyczaj hasło)
- Coś, co masz (zaufane urządzenie, które nie jest łatwo duplikowane, takie jak telefon)
- Coś, co masz (biometria)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Jaki jest koszt włączenia usługi MFA?

Firma Microsoft bezpłatnie zapewnia uwierzytelnianie wieloskładnikowe w ramach implementacji ustawień zabezpieczeń usługi Azure AD. Jedyną opcją weryfikacji dostępną przy użyciu tej wersji usługi MFA jest aplikacja do wystawcy. Jeśli jest wymagane połączenie telefoniczne lub wiadomość SMS, należy zakupić licencję [Azure Active Directory — wersja Premiumową](/azure/active-directory/fundamentals/active-directory-get-started-premium) . Alternatywnie możesz użyć rozwiązania innej firmy w celu zapewnienia MFA dla każdego użytkownika w dzierżawie partnerskiej — w tym przypadku jest odpowiedzialny za zapewnienie, że Twoje rozwiązanie MFA jest wymuszane i jest zgodne.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Jakie akcje muszę wykonać, jeśli mam już rozwiązanie MFA?

W przypadku uzyskiwania dostępu do komercyjnych usług w chmurze firmy Microsoft wymagane jest uwierzytelnienie użytkowników w dzierżawie partnerskiej za pośrednictwem usługi MFA. Rozwiązania innych firm mogą służyć do spełnienia tych wymagań. Firma Microsoft nie zapewnia już testów weryfikacyjnych niezależnym dostawcom tożsamości w celu zapewnienia zgodności z Azure Active Directory. Aby przetestować produkt pod kątem współdziałania, zapoznaj się z tymi [wskazówkami](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> W przypadku korzystania z rozwiązania innej firmy ważne jest, aby sprawdzić, czy rozwiązanie wystawia odwołanie metody uwierzytelniania (AMR), które zawiera wartość MFA. Aby uzyskać szczegółowe informacje na temat weryfikacji rozwiązań innych firm, należy zapoznać się z tematem [testowanie wymagań dotyczących zabezpieczeń partnerów](/powershell/partnercenter/test-partner-security-requirements) .

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Używam wielu dzierżawców partnerskich do języka Transact. Czy muszę zaimplementować na nich wszystkie usługi MFA?

Tak, należy wymusić uwierzytelnianie wieloskładnikowe dla każdej dzierżawy usługi Azure Active Directory skojarzonej z programem CSP lub programem Advisor. Aby kupić licencję na Azure Active Directory — wersja Premium, musisz zakupić licencję Azure Active Directory dla użytkowników w każdej Azure Active Directory dzierżawie. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Czy każde konto użytkownika w dzierżawie partnerskiej musi mieć wymuszane uwierzytelnianie wieloskładnikowe?

Tak, każdy użytkownik musi mieć wymuszone uwierzytelnianie wieloskładnikowe. Jeśli jednak używasz domyślnych ustawień zabezpieczeń usługi Azure AD, nie ma potrzeby wykonywania dodatkowych czynności, ponieważ ta funkcja wymusza uwierzytelnianie wieloskładnikowe dla wszystkich kont użytkowników. Włączenie ustawień domyślnych zabezpieczeń jest bezpłatnym i łatwym sposobem zapewnienia, że konta użytkowników są zgodne z usługą MFA i nie mają wpływu na działanie usługi MFA.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Jestem partnerem rozliczeniowym z firmą Microsoft. Co mam zrobić?

Partnerzy dostawcy rozwiązań w chmurze z bezpośrednią opłatą muszą wymusić uwierzytelnianie MFA dla każdego użytkownika w dzierżawie partnera.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Jestem odsprzedawcą pośrednim i tylko transactię, chociaż dystrybutorem. Czy muszę włączyć usługę MFA?

Wszyscy pośredniemu odsprzedawcy są zobowiązani do wymuszania uwierzytelniania wieloskładnikowego dla każdego użytkownika w dzierżawie partnera. Pośredni odsprzedawca musi włączyć usługę MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Nie korzystam z interfejsu API Centrum partnerskiego. Czy nadal muszę wdrożyć usługę MFA?

Tak, to wymaganie zabezpieczeń dotyczy wszystkich użytkowników, w tym użytkowników z uprawnieniami administratora partnera i użytkowników końcowych w dzierżawie partnera.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Którzy dostawcy innych firm dostarczają rozwiązania MFA zgodne z Azure Active Directory?

Podczas przeglądania dostawców i rozwiązań usługi MFA partnerzy muszą upewnić się, że wybrane rozwiązanie jest zgodne z Azure Active Directory.

Firma Microsoft nie zapewnia już testów weryfikacyjnych niezależnym dostawcom tożsamości w celu zapewnienia zgodności z Azure Active Directory. Jeśli chcesz przetestować produkt pod kątem współdziałania, zapoznaj się z tymi [wskazówkami](https://www.microsoft.com/download/details.aspx?id=56843).

Aby uzyskać więcej informacji, zobacz [listę zgodności Federacji usługi Azure AD](/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Jak można testować usługę MFA w naszym piaskownicie integracji?

Należy włączyć funkcję ustawień zabezpieczeń usługi Azure AD lub alternatywnie użyć rozwiązania innej firmy korzystającej z Federacji.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Czy włączenie usługi MFA będzie miało wpływ na sposób współpracy z dzierżawcą klienta?

Nie. Spełnienie tych wymagań dotyczących zabezpieczeń nie będzie miało wpływu na sposób zarządzania klientami. Możliwość wykonywania delegowanych operacji administracyjnych nie zostanie przerwana.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Czy moi klienci podlegają wymaganiom dotyczącym zabezpieczeń partnerów?

Nie. nie jest wymagane, aby wymusić uwierzytelnianie MFA dla każdego użytkownika w dzierżawach usługi Azure AD klienta. Zaleca się jednak współdziałanie z każdym klientem, aby określić, jak najlepiej chronić swoich użytkowników.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Czy każdy użytkownik może zostać wykluczony z wymogu MFA?

Nie, każdy użytkownik, w tym konta usług, w dzierżawie partnerskiej będzie wymagał uwierzytelniania przy użyciu usługi MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Czy wymagania dotyczące zabezpieczeń partnerów dotyczą piaskownicy integracji?

Tak, wymagania dotyczące zabezpieczeń partnerów dotyczą piaskownicy integracji. Oznacza to, że należy zaimplementować odpowiednie rozwiązanie MFA dla użytkowników w dzierżawie piaskownicy integracji. Zalecane jest zaimplementowanie ustawień domyślnych zabezpieczeń usługi Azure AD w celu zapewnienia uwierzytelniania wieloskładnikowego.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Jak mogę skonfigurować konto dostępu awaryjnego (Break Glass)?

Najlepszym rozwiązaniem jest utworzenie jednego lub dwóch kont dostępu awaryjnego, aby zapobiec niezamierzonemu zablokowaniu dzierżawy usługi Azure AD. W odniesieniu do wymagań dotyczących zabezpieczeń partnerów wymagane jest, aby każdy użytkownik uwierzytelniał się przy użyciu usługi MFA. To wymaganie należy zmodyfikować definicję konta dostępu awaryjnego. Może to być konto, które używa rozwiązania innej firmy dla usługi MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Czy w przypadku korzystania z rozwiązania innej firmy jest wymagana Active Directory usługa federacyjna (ADFS)?

Nie, nie musisz mieć Active Directory usługa federacyjna (ADFS), jeśli używasz rozwiązania innej firmy. Zaleca się, aby skontaktować się z dostawcą rozwiązania, ustalić, jakie są wymagania dotyczące ich rozwiązania.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Czy jest wymagane włączenie ustawień zabezpieczeń usługi Azure AD?

Nie, nie jest wymagane włączenie ustawień zabezpieczeń usługi Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Czy dostęp warunkowy może być używany w celu spełnienia wymagań usługi MFA?

Tak, możesz użyć dostępu warunkowego, aby wymusić uwierzytelnianie MFA dla każdego użytkownika, w tym konta usług, w dzierżawie partnera. Jednak ze względu na wysoce uprzywilejowany charakter partnera musimy upewnić się, że każdy użytkownik ma wyzwanie usługi MFA dla każdego pojedynczego uwierzytelniania. Oznacza to, że nie będzie można korzystać z funkcji dostępu warunkowego, która omija wymóg uwierzytelniania wieloskładnikowego.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Czy konto usługi używane przez Azure AD Connect ma wpływ na wymagania dotyczące zabezpieczeń partnerów?

Nie, wymagania dotyczące zabezpieczeń partnerów nie będą miały wpływu na konto usługi używane przez Azure AD Connect. Jeśli wystąpi problem z Azure AD Connect w wyniku wymuszania usługi MFA, Otwórz żądanie pomocy technicznej w pomocy technicznej firmy Microsoft.

## <a name="secure-application-model"></a>Bezpieczny model aplikacji

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Kto powinien przyjąć bezpieczny model aplikacji, aby spełniał wymagania?

Firma Microsoft wprowadza bezpieczną i skalowalną platformę do uwierzytelniania partnerów dostawcy rozwiązań w chmurze (CSP) i dostawców panelu sterowania (CPV), które używają Multi-Factor Authentication. Aby uzyskać więcej informacji, zobacz [Przewodnik po modelu bezpiecznej aplikacji](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Wszyscy partnerzy, którzy utworzyli integrację niestandardową przy użyciu dowolnych interfejsów API (na przykład Azure Resource Manager, Microsoft Graph, interfejsu API centrum partnera itp.) lub zaimplementowano automatyzację niestandardową przy użyciu narzędzi takich jak program PowerShell, będą musieli wdrożyć [bezpieczną strukturę modelu aplikacji](/partner-center/develop/enable-secure-app-model) w celu integracji z usługami w chmurze firmy Microsoft.

### <a name="what-is-the-secure-application-model"></a>Co to jest model bezpiecznego stosowania aplikacji?

Firma Microsoft wprowadza bezpieczną i skalowalną platformę do uwierzytelniania partnerów dostawcy rozwiązań w chmurze (CSP) i dostawców panelu sterowania (CPV), które wykorzystują Multi-Factor Authentication. Aby uzyskać więcej informacji, zobacz [Przewodnik po modelu bezpiecznej aplikacji](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Jak mogę wdrożyć bezpieczny model aplikacji?

Wszyscy partnerzy, którzy utworzyli integrację niestandardową przy użyciu dowolnych interfejsów API (na przykład Azure Resource Manager, Microsoft Graph, interfejsu API centrum partnera itp.) lub zaimplementowano automatyzację niestandardową przy użyciu narzędzi takich jak program PowerShell, będą musieli wdrożyć [bezpieczną strukturę modelu aplikacji](/partner-center/develop/enable-secure-app-model) w celu integracji z usługami w chmurze firmy Microsoft. Niewykonanie tej czynności może skutkować zakłóceniem ze względu na wdrożenie usługi MFA. Poniższe zasoby zawierają omówienie i wskazówki dotyczące sposobu wdrażania modelu.

- [Omówienie bezpiecznego modelu aplikacji](/partner-center/develop/enable-secure-app-model)
- [Centrum partnerskie: bezpieczny model aplikacji — przewodnik](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerzy w programie CSP: przykładowy kod platformy .NET do włączenia bezpiecznego modelu aplikacji](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerzy w programie CSP: przykładowy kod w języku Java do włączenia bezpiecznego modelu aplikacji](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokument uwierzytelniania Centrum partnerskiego](/partner-center/develop/partner-center-authentication)
- [Dokument programu PowerShell Centrum partnerskiego Multi-Factor Authentication (MFA)](/powershell/partnercenter/multi-factor-auth)

Jeśli używasz panelu sterowania, musisz skontaktować się z dostawcą, aby uzyskać informacje na temat wdrażania bezpiecznej struktury modelu aplikacji.

Aby [dołączyć](enroll-as-cpv.md) do Centrum partnerskiego jako dostawcę panelu sterowania i rozpocząć wdrażanie tego wymagania, wymagane są dostawcy panelu sterowania. Zapoznaj się z [centrum partnerskim: Secure Application model Framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dostawcy panelu sterowania muszą akceptować i zarządzać "zgodą partnerów usług kryptograficznych" zamiast poświadczeń i czyścić wszystkie istniejące poświadczenia partnerów programu CSP.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Czy model bezpiecznego aplikacji musi być zaimplementowany tylko dla interfejsu API/zestawu SDK Centrum partnerskiego?

Wymuszanie uwierzytelniania wieloskładnikowego dla wszystkich kont użytkowników może mieć wpływ na dowolną automatyzację lub integrację, która jest przeznaczona do uruchamiania nieinteraktywnie. Wymagania dotyczące zabezpieczeń partnerów wymagają włączenia bezpiecznego modelu aplikacji dla interfejsu API Centrum partnerskiego. mogą one służyć do rozwiązywania potrzeby drugiego czynnika uwierzytelniania z automatyzacją i integracją.

>[!Note] 
>Zasoby, do których uzyskuje się dostęp, muszą obsługiwać uwierzytelnianie oparte na tokenach.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Korzystam z narzędzi automatyzacji, takich jak PowerShell. Jak mogę wdrożyć bezpieczny model aplikacji?

Należy zaimplementować bezpieczny model aplikacji, jeśli Automatyzacja ma być uruchomiona nieinteraktywnie i opiera się na poświadczeniach użytkownika na potrzeby uwierzytelniania. Zobacz [bezpieczny model aplikacji | Centrum partnerskie programu PowerShell](/powershell/partnercenter/multi-factor-auth) , aby uzyskać wskazówki dotyczące implementowania tej struktury.  

>[!Note] 
>Nie wszystkie narzędzia automatyzacji zapewniają możliwość uwierzytelniania przy użyciu tokenów dostępu. Opublikuj wiadomość w grupie [wskazówek dotyczących zabezpieczeń Centrum partnerskiego](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) , aby uzyskać pomoc w zrozumieniu, jakie zmiany należy wprowadzić. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Jakie poświadczenia użytkownika należy podać administrator aplikacji podczas przeprowadzania procesu wyrażania zgody?

Zaleca się użycie konta usługi, któremu przypisano uprawnienia najniższych uprawnień. W odniesieniu do interfejsu API Centrum partnerskiego należy użyć konta, które zostało przypisane do roli agent sprzedaży lub agenci administracyjni.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Dlaczego administrator aplikacji nie udostępnia poświadczeń administratora globalnego podczas przeprowadzania procesu wyrażania zgody?

Najlepszym rozwiązaniem jest użycie tożsamości o najniższych uprawnieniach.  Spowoduje to zredukowanie ryzyka. Nie zaleca się korzystania z konta, które ma uprawnienia administratora globalnego, ponieważ spowodowałoby to dostarczenie większej liczby uprawnień niż to, co jest wymagane.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Jestem partnerem programu CSP. Jak mogę wiedzieć, czy mój dostawca panelu sterowania (CPV) pracuje nad implementacją rozwiązania lub nie?

W przypadku partnerów korzystających z rozwiązania dostawcy panelu sterowania (CPV) do wykonywania operacji Transact w programie w programie Cloud Solution Provider (CSP) jest odpowiedzialny za konsultacje z Twoim CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Kto jest dostawcą panelu sterowania (CPV)?

Dostawca panelu sterowania jest niezależnym dostawcą oprogramowania, który opracowuje aplikacje do użycia przez partnerów CSP do integracji z interfejsami API Centrum partnerskiego. Dostawca panelu sterowania nie jest partnerem dostawcy usług kryptograficznych, który ma bezpośredni dostęp do pulpitu nawigacyjnego lub interfejsów API Centrum partnerskiego. Szczegółowy opis jest dostępny w [przewodniku w centrum partnerskim: Secure Applications model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Jestem CPV. Jak mogę zarejestrować?

Aby zarejestrować się jako dostawca panelu sterowania (CPV), postępuj zgodnie ze wskazówkami podanymi w [tym miejscu](enroll-as-cpv.md).

CPVs musi skontaktować się z użytkownikiem [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) , aby otrzymać link rejestracji i udostępnić sponsora pracownika firmy Microsoft, który ma związek biznesowy z CPV lub wie swoją działalność. Na przykład Menedżer ds. partnerów (PDM).

Po zarejestrowaniu się w centrum partnerskim i zarejestrowaniu aplikacji będziesz mieć dostęp do interfejsów API Centrum partnerskiego. Informacje o piaskownicy są odbierane za pośrednictwem powiadomienia Centrum partnerskiego, jeśli jesteś nowym CPV. Po zakończeniu rejestracji jako CPV firmy Microsoft i zaakceptowaniu umowy CPV można:

1. Zarządzaj aplikacjami wielodostępnymi (Dodaj aplikacje do Azure Portal i zarejestruj i Wyrejestruj aplikacje w centrum partnerskim).

   >[!Note]
   >CPVs muszą zarejestrować swoje aplikacje w centrum partnerskim, aby uzyskać autoryzację dla interfejsów API Centrum partnerskiego. Dodawanie aplikacji do Azure Portal samej nie powoduje autoryzacji aplikacji CPV dla interfejsów API Centrum partnerskiego.

1. Wyświetl swój profil CPV i Zarządzaj nim.

1. Wyświetlaj użytkowników, którzy potrzebują dostępu do funkcji CPV, i zarządzaj nimi. CPV może mieć tylko administratora globalnego roli.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Używam zestawu SDK Centrum partnerskiego. Czy zestaw SDK będzie automatycznie wdrażać bezpieczny model aplikacji?

Nie, należy postępować zgodnie ze wskazówkami podanymi w [przewodniku po modelu bezpiecznej aplikacji](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Czy mogę wygenerować token odświeżania dla bezpiecznego modelu aplikacji z kontami, na których nie jest włączona funkcja MFA?

Tak, token odświeżania można wygenerować przy użyciu konta, które nie ma wymuszonego uwierzytelniania wieloskładnikowego. Należy jednak to uniknąć. Każdy token wygenerowany przy użyciu konta, które nie ma włączonej usługi MFA, nie będzie mógł uzyskać dostępu do zasobów ze względu na wymaganie uwierzytelniania wieloskładnikowego.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Jak moja aplikacja ma uzyskać token dostępu w przypadku włączenia usługi MFA?

Należy postępować zgodnie z [przewodnikiem bezpiecznego modelu aplikacji](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) , który zawiera szczegółowe informacje na temat tego, jak to zrobić, przy jednoczesnym zapewnieniu zgodności z nowymi wymaganiami dotyczącymi zabezpieczeń. [W tym miejscu możesz](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) znaleźć przykładowy kod platformy .NET i kod [Java.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Jako CPV, czy mogę utworzyć aplikację usługi Azure AD w ramach dzierżawy CPV lub dzierżawcy partnera CSP?

CPV będzie musiał utworzyć aplikację Azure Active Directory w dzierżawie skojarzonej z ich rejestracją jako CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Jestem dostawcą CSP korzystającym tylko z uwierzytelniania aplikacji. Czy muszę wprowadzić jakiekolwiek zmiany?

Nie ma to wpływu na uwierzytelnianie tylko aplikacji, ponieważ poświadczenia użytkownika nie są używane do żądania tokenu dostępu. Jeśli poświadczenia użytkownika są udostępniane, a następnie w panelu sterowania dostawcy (CPVs) muszą zastosować [bezpieczną strukturę modelu aplikacji](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) i przeczyścić wszystkie istniejące poświadczenia partnera.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Jak CPV może wykorzystać styl uwierzytelniania tylko dla aplikacji, aby uzyskać tokeny dostępu?

Nie, partnerzy dostawcy panelu sterowania nie mogą korzystać z stylu uwierzytelniania tylko aplikacja, aby żądać tokenów dostępu w imieniu partnera. Powinny implementować bezpieczny model aplikacji, który wykorzystuje styl uwierzytelniania aplikacji i użytkownika.

## <a name="technical-enforcement"></a>Wymuszanie techniczne

### <a name="what-is-the-activation-of-security-safeguards"></a>Co to jest aktywacja zabezpieczenia zabezpieczeń?

Wszyscy partnerzy uczestniczący w programie dostawcy rozwiązań w chmurze (CSP), dostawcy panelu sterowania (CPVs) i doradcy powinni zaimplementować obowiązkowe wymagania dotyczące zabezpieczeń, aby zachować zgodność.

Aby zapewnić dodatkową ochronę, firma Microsoft rozpoczęła aktywację zabezpieczeń, które pomagają partnerom w zabezpieczaniu dzierżawców i ich klientów przez zagwarantowanie weryfikacji uwierzytelniania wieloskładnikowego (MFA) w celu zapobiegania nieautoryzowanemu dostępowi.  

Pomyślnie ukończono aktywację funkcji administrator-w-imieniu (AOBO) do wszystkich dzierżawców partnerów. Aby zapewnić lepszą ochronę partnerów i klientów, przeznaczenie do kwartału Q2 CY2020, rozpocznie się aktywacja dla transakcji Centrum partnerskiego w dostawcy usług kryptograficznych, pomagając partnerom chronić swoje firmy i klientów przed zdarzeniami związanymi z kradzieżą tożsamości.

Aby uzyskać więcej informacji, odwiedź stronę [dotyczącą uwierzytelniania wieloskładnikowego (MFA) dla Twojej dzierżawy partnerskiej](partner-security-requirements-mandating-mfa.md) .

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Korzystam z rozwiązania MFA innej firmy i jestem blokowany, co mam zrobić?

Aby sprawdzić, czy dla konta uzyskującego dostęp do zasobów zarejestrowano uwierzytelnianie wieloskładnikowe, sprawdzimy [odwołanie do metody uwierzytelniania](https://tools.ietf.org/html/rfc8176) , aby zobaczyć, czy jest wyświetlana lista MFA. Niektóre rozwiązania innych firm nie wystawiają tego żądania lub nie obejmują wartości MFA. W przypadku braku żądania lub wartości MFA nie ma na liście, nie ma możliwości ustalenia, czy uwierzytelnione konto zostało zakwestionowane do uwierzytelniania wieloskładnikowego. Należy skontaktować się z dostawcą rozwiązania innej firmy, aby określić, jakie działania należy podjąć, aby rozwiązanie wystawia odwołanie do metody uwierzytelniania.

Zapoznaj się z tematem [testowanie wymagań dotyczących zabezpieczeń partnerów](/powershell/partnercenter/test-partner-security-requirements) , jeśli nie masz pewności, czy rozwiązanie innej firmy wystawia oczekiwane lub nie.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>Uwierzytelnianie wieloskładnikowe uniemożliwia mi obsługę mojego klienta przy użyciu AOBO, co należy zrobić?

Należy sprawdzić techniczne wymagania dotyczące zabezpieczeń partnerów, jeśli uwierzytelnione konto zostało zakwestionowane na potrzeby uwierzytelniania wieloskładnikowego. Jeśli konto nie zostało, nastąpi przekierowanie do strony logowania i zostanie wyświetlony monit o ponowne uwierzytelnienie. Zapoznaj się z dodatkowym doświadczeniem i wskazówkami zawartymi w tym [upoważnieniu do obsługi uwierzytelniania wieloskładnikowego (MFA) na potrzeby dokumentacji dzierżawy partnerskiej](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) . W scenariuszu, w którym domena nie jest federacyjna, po pomyślnym uwierzytelnieniu zostanie wyświetlony monit o skonfigurowanie uwierzytelniania wieloskładnikowego. Po zakończeniu tej operacji będziesz mieć możliwość zarządzania klientami przy użyciu usługi AOBO. W scenariuszu, w którym domena jest federacyjna, należy upewnić się, że konto jest wyzwaniem do uwierzytelniania wieloskładnikowego.

## <a name="security-defaults-transition"></a>Domyślne przejście zabezpieczeń

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Jak przejść z zasad linii bazowej do domyślnych ustawień zabezpieczeń lub innych rozwiązań MFA?

Zasady "podstawowe" usługi Azure Active Directory (Azure AD) [są usuwane i zastępowane](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) "ustawieniami domyślnymi zabezpieczeń", tym bardziej kompleksowym zestawem zasad ochrony dla Ciebie i Twoich klientów. [Wartości domyślne zabezpieczeń](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) mogą pomóc w ochronie organizacji przed atakami z wykorzystaniem zabezpieczeń związanych z kradzieżą tożsamości.

Implementacja uwierzytelniania wieloskładnikowego (MFA) zostanie usunięta z powodu wycofania zasad bazowych, jeśli nie przeszedł z zasad odniesienia do zasad ustawień domyślnych zabezpieczeń lub [innych opcji implementacji usługi MFA](partner-security-requirements.md#implementing-multi-factor-authentication). Wszyscy użytkownicy w dzierżawach partnerskich, którzy wykonują operacje chronione przez usługę MFA, będą żądać wykonania weryfikacji MFA. Szczegółowe wskazówki znajdziesz [tutaj](partner-security-requirements-mandating-mfa.md).
Aby zachować zgodność i zminimalizować zakłócenia, wykonaj jedną z następujących czynności:

- Przejście do domyślnych ustawień zabezpieczeń
    - Zasady ustawień domyślnych zabezpieczeń są jedną z opcji, które partnerzy mogą wybrać wdrożenie usługi MFA. Oferuje on podstawowy poziom zabezpieczeń włączony bez dodatkowych kosztów.
    - Dowiedz się, jak włączyć usługę MFA dla Twojej organizacji za pomocą usługi Azure AD, a następnie zapoznaj się z [zagadnieniami dotyczącymi kluczy domyślnych](partner-security-requirements.md#security-defaults)
    - Włącz zasady ustawień zabezpieczeń, jeśli spełnią Twoje potrzeby biznesowe.
- Przejście do dostępu warunkowego
    - Jeśli zasady ustawień zabezpieczeń nie spełniają Twoich wymagań, Włącz dostęp warunkowy. Aby uzyskać więcej informacji, zapoznaj się z dokumentacją dostępu warunkowego usługi Azure AD.

## <a name="key-resources"></a>Najważniejsze zasoby

### <a name="how-to-get-started"></a>Jak zacząć

- [Wymagania dotyczące zabezpieczeń partnerów: Przewodnik krok po kroku](partner-security-requirements.md).
- Skieruj swoje pytania i opinie do tej [grupy wskazówek dotyczących zabezpieczeń Centrum partnerskiego](https://aka.ms/MPCSecurityGuidance).
- Uczestnictwo w nadchodzących godzinach biura i seminaria internetoweów partnerów. Zapoznaj się z [szczegółowym harmonogramem i zasobami w tym miejscu](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Zasoby do wdrażania bezpiecznego modelu aplikacji

- [Omówienie bezpiecznego modelu aplikacji](/partner-center/develop/enable-secure-app-model)
- [Centrum partnerskie: bezpieczny model aplikacji — przewodnik](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerzy w programie CSP: przykładowy kod platformy .NET do włączenia bezpiecznego modelu aplikacji](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerzy w programie CSP: przykładowy kod w języku Java do włączenia bezpiecznego modelu aplikacji](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokument uwierzytelniania Centrum partnerskiego](/partner-center/develop/partner-center-authentication)
- [Dokument programu PowerShell Centrum partnerskiego Multi-Factor Authentication (MFA)](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Pomoc techniczna

### <a name="where-can-i-get-support"></a>Gdzie mogę uzyskać pomoc techniczną?

Aby zasoby pomocy technicznej spełniały wymagania dotyczące zabezpieczeń, jeśli masz zaawansowaną pomoc techniczną dla partnerów (ASfP), skontaktuj się z menedżerem konta usługi. Aby uzyskać umowę pomoc techniczna Premium for Partners (PSfP), skontaktuj się z menedżerem konta usługi i menedżerem ds. klientów.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Jak mogę uzyskać informacje techniczne i pomoc techniczną, aby pomóc mi zastosować bezpieczną strukturę modelu aplikacji?

Opcje pomocy technicznej dla Azure Active Directory są dostępne w ramach korzyści MPN. Partnerzy z dostępem do aktywnej subskrypcji ASfP lub PSfP mogą współdziałać z zarządzanym menedżerem kont (SAM/KONSULTANTem), aby najlepiej zrozumieć dostępne opcje.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Jak mogę skontaktować się z pomocą techniczną, jeśli mam dostęp do Centrum partnerskiego?

Jeśli utracisz dostęp z powodu problemu z usługą MFA, skontaktuj się z administratorem globalnym dzierżawy. Wewnętrzny dział INFORMATYCZNy będzie mógł powiedzieć, kto jest administratorem globalnym. 

Jeśli nie pamiętasz hasła, zapoznaj [się z artykułem nie można zalogować](unable-to-sign-in.md) się w celu uzyskania pomocy.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Gdzie można znaleźć więcej informacji na temat typowych problemów technicznych?

Informacje o typowych problemach technicznych można znaleźć w temacie [wymagania dotyczące zabezpieczeń partnerów dla partnerów przy użyciu Centrum partnerskiego lub interfejsów API Centrum partnerskiego](partner-security-requirements.md) .