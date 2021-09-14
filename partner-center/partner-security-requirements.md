---
title: Partner security requirements (Wymagania dotyczące zabezpieczeń partnerów)
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Wprowadzono wymagania dotyczące zabezpieczeń partnerów w celu włączenia uwierzytelniania wieloskładnikowego (MFA) i model aplikacji zabezpieczonych struktury.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 8966d744dfb70a7850ef6d3dd68d2051344fe9cd
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247419"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Wymagania dotyczące zabezpieczeń dotyczące korzystania z interfejsów API Partner Center lub Partner Center api

**Odpowiednie role:** wszyscy Partner Center użytkowników

W tym artykule wyjaśniono obowiązkowe wymagania dotyczące zabezpieczeń dla doradców, dostawców Panel sterowania i partnerów biorących udział w programie Dostawca rozwiązań w chmurze, a także opcje uwierzytelniania i inne zagadnienia dotyczące zabezpieczeń. Zabezpieczenia i ochrona prywatności należą do naszych najwyższych priorytetów. Wiemy, że najlepszą obroną jest zapobieganie i że jesteśmy tylko tak silni, jak nasze słabe łącze. Dlatego potrzebujemy wszystkich w naszym ekosystemie, aby działać i zapewnić odpowiednie zabezpieczenia.

## <a name="mandatory-security-requirements"></a>Obowiązkowe wymagania dotyczące zabezpieczeń

Partnerzy, którzy nie implementują obowiązkowych wymagań dotyczących zabezpieczeń, nie będą mogli wykonać transakcji w programie Dostawca rozwiązań w chmurze ani zarządzać dzierżawami klientów przy użyciu delegowanych praw administratora. Ponadto partnerzy, którzy nie wdrażają wymagań dotyczących zabezpieczeń, mogą stanowić zagrożenie dla ich uczestnictwa w programach. Warunki skojarzone z wymaganiami zabezpieczeń partnerów zostały dodane do Microsoft Partner Agreement. W odniesieniu do doradców zostaną spełnione te same wymagania umowne.

W celu ochrony Ciebie i Twoich klientów wymagamy od partnerów natychmiastowego podjęcia następujących działań:  

1. **Włącz uwierzytelnianie wieloskładnikowe (MFA) dla wszystkich kont użytkowników w dzierżawie partnera.** Należy wymusić uwierzytelniania wieloskładnikowego na wszystkich kontach użytkowników w dzierżawach partnera. Usługa MFA musi zakwestionować użytkowników podczas logowania się do komercyjnych usług w chmurze firmy Microsoft lub transakcji w programie Dostawca rozwiązań w chmurze za pośrednictwem usługi Partner Center lub za pośrednictwem interfejsów API.

2. **Przyjmij model aplikacji zabezpieczonych platformę .** Wszyscy partnerzy zintegrowani z interfejsami API Partner Center muszą przyjąć platformę [model aplikacji zabezpieczonych dla](/partner-center/develop/enable-secure-app-model) wszystkich aplikacji i aplikacji modelu uwierzytelniania użytkowników.

    > [!IMPORTANT]
    > Zdecydowanie zalecamy partnerom zaimplementowanie usługi model aplikacji zabezpieczonych w celu integracji z interfejsem API firmy Microsoft, takim jak Azure Resource Manager lub Microsoft Graph, lub w przypadku korzystania z automatyzacji, takiej jak program PowerShell, przy użyciu poświadczeń użytkownika, aby uniknąć zakłóceń w przypadku wymuszania uwierzytelniania wieloskładnikowego.

Te wymagania dotyczące zabezpieczeń pomogą chronić infrastrukturę i chronić dane klientów przed potencjalnym zagrożeniem bezpieczeństwa, takim jak identyfikowanie kradzieży lub innych zdarzeń związanych z oszustwem.  

## <a name="implementing-multi-factor-authentication"></a>Implementowanie uwierzytelniania wieloskładnikowego

Aby spełnić wymagania dotyczące zabezpieczeń partnerów, należy wdrożyć i wymusić uwierzytelniania wieloskładnikowego dla każdego konta użytkownika w dzierżawie partnera. Można to zrobić w jeden z następujących sposobów:

- [Zaim Azure Active Directory domyślne zabezpieczeń usługi Azure AD.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) Więcej informacji można znaleźć w [następnej sekcji](#security-defaults).

- Zakup Azure Active Directory — wersja Premium dla każdego konta użytkownika. Aby uzyskać więcej informacji, zobacz [Planowanie wdrożenia usługi Azure AD Multi-Factor Authentication.](/azure/active-directory/authentication/howto-mfa-getstarted)

- Użyj rozwiązania innej firmy, aby wymusić uwierzytelniania wieloskładnikowego dla każdego konta użytkownika w dzierżawie partnera. Aby upewnić się, że rozwiązanie zapewni oczekiwane rozwiązanie, zobacz, jak będą [wymuszane wymagania dotyczące zabezpieczeń.](#how-the-requirements-are-enforced)

> [!NOTE]
> Mimo że uwierzytelnianie wieloskładnikowe nie jest wymagane w umowie dla suwerennej chmury (dla instytucji rządowych USA i Niemiec), zdecydowanie zaleca się przyjęcie tych wymagań dotyczących zabezpieczeń.

### <a name="security-defaults"></a>Domyślne ustawienia zabezpieczeń

Jedną z opcji, które partnerzy mogą wybrać w celu zaimplementowania wymagań usługi MFA, jest włączenie ustawień domyślnych zabezpieczeń w usłudze Azure AD. Wartości domyślne zabezpieczeń oferują podstawowy poziom zabezpieczeń bez dodatkowych kosztów. Przed włączeniem ustawień domyślnych zabezpieczeń zapoznaj się ze instrukcjami włączania uwierzytelniania wieloskładnikowego dla organizacji za pomocą usługi Azure AD i zapoznaj się z kluczowymi zagadnieniami poniżej.

- Partnerzy, którzy już uchwalili zasady bazowe, muszą podjąć działania w celu przejścia na wartości domyślne zabezpieczeń.

- Wartości domyślne zabezpieczeń to ogólne zastąpienie zasad punktów odniesienia w wersji zapoznawczej. Gdy partner włączy wartości domyślne zabezpieczeń, nie będzie już mógł włączyć zasad bazowych.

- W przypadku wartości domyślnych zabezpieczeń wszystkie zasady zostaną włączone jednocześnie.

- W przypadku partnerów, którzy [korzystają](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)z [dostępu warunkowego, wartości domyślne zabezpieczeń nie będą dostępne.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)

- Obecnie starsze uwierzytelnianie nie jest blokowane. Jednak ze względu na to, że większość zdarzeń związanych z naruszonymi tożsamościami pochodzi z próby logowania przy użyciu starszego uwierzytelniania, zachęcamy partnerów do odejścia od tych starszych protokołów.

- Konto synchronizacji Połączenie azure AD jest wykluczone z ustawień domyślnych zabezpieczeń.

Aby uzyskać szczegółowe informacje, [przeczytaj Omówienie usługi Azure AD Multi-Factor Authentication dla](/azure/active-directory/authentication/concept-mfa-get-started) organizacji i Co to są ustawienia domyślne [zabezpieczeń?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Wartości domyślne zabezpieczeń usługi Azure AD to ewolucja uproszczonych zasad ochrony punktów odniesienia. Jeśli zasady ochrony punktów odniesienia zostały już włączone, zdecydowanie zaleca się włączenie [domyślnych wartości zabezpieczeń](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Istotne informacje dotyczące implementacji

Ponieważ te wymagania dotyczą wszystkich kont użytkowników w dzierżawie partnera, należy wziąć pod uwagę kilka rzeczy, aby zapewnić bezproblemowe wdrożenie. Możesz na przykład zidentyfikować konta użytkowników w usłudze Azure AD, które nie mogą wykonywać uwierzytelniania wieloskładnikowego, oraz aplikacje i urządzenia w organizacji, które nie obsługują nowoczesnego uwierzytelniania.

Przed wykonaniem jakiejkolwiek akcji zalecamy przeprowadzenie następujących weryfikacji. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Czy masz aplikację lub urządzenie, które nie obsługuje korzystania z nowoczesnego uwierzytelniania?

W przypadku wymuszania uwierzytelniania wieloskładnikowego starsze uwierzytelnianie będzie korzystać z protokołów, takich jak IMAP, POP3, SMTP i inne, ponieważ nie obsługują one usługi MFA. Aby rozwiązać ten limit, użyj [funkcji haseł aplikacji,](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) aby upewnić się, że aplikacja lub urządzenie nadal będą uwierzytelniane. Zapoznaj się [z zagadnieniami na temat używania haseł aplikacji,](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) aby określić, czy mogą być używane w Twoim środowisku.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Czy masz użytkowników Office 365 z licencjami skojarzonymi z dzierżawą partnera?

Przed zaimplementowaniem dowolnego rozwiązania zalecamy określenie, z których wersji aplikacji korzysta Microsoft Office użytkowników w dzierżawie partnera. Istnieje prawdopodobieństwo, że użytkownicy będą mieć problemy z łącznością z aplikacjami, Outlook. Przed wymuśm uwierzytelnianie wieloskładnikowe należy upewnić się, że używasz programu Outlook 2013 z dodatkiem SP1 lub nowszego oraz że Twoja organizacja ma włączone nowoczesne uwierzytelnianie. Aby uzyskać więcej informacji, zobacz [Włączanie nowoczesnego uwierzytelniania w Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Aby włączyć nowoczesne uwierzytelnianie dla urządzeń Windows z zainstalowanym programem Microsoft Office 2013, należy utworzyć dwa klucze rejestru. Zobacz [Włączanie nowoczesnego uwierzytelniania dla Office 2013 na Windows urządzeniach.](/office365/admin/security-and-compliance/enable-modern-authentication)

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Czy istnieją zasady uniemożliwiające użytkownikom korzystanie z urządzeń przenośnych podczas pracy?

Ważne jest, aby zidentyfikować wszelkie zasady firmowe, które uniemożliwiają pracownikom korzystanie z urządzeń przenośnych podczas pracy, ponieważ będą mieć wpływ na to, jakie rozwiązanie MFA zostanie zaimplementowane. Istnieją rozwiązania, takie jak te, które są udostępniane w ramach implementacji domyślnych ustawień zabezpieczeń usługi [Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), które zezwalają tylko na używanie aplikacji authenticator do weryfikacji. Jeśli twoja organizacja ma zasady uniemożliwiające korzystanie z urządzeń przenośnych, rozważ jedną z następujących opcji:

- Wdrażanie aplikacji jednorazowego hasła podstawowego (TOTP, time-based one-time base password), która może być uruchamiana w bezpiecznym systemie.

- Zaim implementowanie rozwiązania innej firmy, które wymusza uwierzytelniania wieloskładnikowego dla każdego konta użytkownika w dzierżawie partnera, które zapewnia najbardziej odpowiednią opcję weryfikacji.

- Kup [Azure Active Directory — wersja Premium](https://azure.microsoft.com/pricing/details/active-directory/) licencji dla użytkowników, których dotyczy problem.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Jaką automatyzację lub integrację należy wykorzystać do uwierzytelniania przy użyciu poświadczeń użytkownika?

Ponieważ wymuszamy uwierzytelnianie wieloskładnikowe dla każdego użytkownika, w tym kont usług, w katalogu partnera, będzie to miało wpływ na dowolną automatyzację lub integrację, która używa poświadczeń użytkownika do uwierzytelniania. Dlatego ważne jest, aby zidentyfikować konta, które są używane w takich sytuacjach. Zobacz następującą listę przykładowych aplikacji lub usług, które należy wziąć pod uwagę:

- Panel sterowania używany do aprowizowanie zasobów w imieniu klientów

- Integracja z dowolną platformą używaną do fakturowania (w odniesieniu do programu CSP) i obsługą klientów

- Skrypty programu PowerShell, które używają modułów Az, AzureRM, Azure AD, MS Online i innych

Powyższe listy nie są kompleksowe. Dlatego ważne jest, aby przeprowadzić pełną ocenę dowolnej aplikacji lub usługi w środowisku, która używa poświadczeń użytkownika do uwierzytelniania. Aby wziąć pod uwagę wymaganie uwierzytelniania wieloskładnikowego, należy zaimplementować wskazówki w [model aplikacji zabezpieczonych, jeśli](/partner-center/develop/enable-secure-app-model) jest to możliwe.

## <a name="accessing-your-environment"></a>Uzyskiwanie dostępu do środowiska

Aby lepiej zrozumieć, co lub kto uwierzytelnia bez konieczności uwierzytelniania wieloskładnikowego, zalecamy przejrzenie działania logowania. Za Azure Active Directory — wersja Premium możesz użyć raportu logowania. Aby uzyskać więcej informacji na ten temat, zobacz Raporty dotyczące działań [logowania w witrynie Azure Active Directory Portal.](/azure/active-directory/reports-monitoring/concept-sign-ins) Jeśli nie masz konta Azure Active Directory — wersja Premium lub szukasz sposobu uzyskania tego działania logowania za pomocą programu PowerShell, musisz użyć polecenia cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) z modułu [Partner Center PowerShell.](https://www.powershellgallery.com/packages/PartnerCenter/)

## <a name="how-the-requirements-are-enforced"></a>Jak są wymuszane wymagania

Partner security requirements are enforced by Azure AD, and Partner Center, by checking for the presence of the MFA claim to identify that MFA verification has place. Od 18 listopada 2019 r. firma Microsoft aktywowała dodatkowe zabezpieczenia (wcześniej znane jako "wymuszanie techniczne") dzierżawom partnerskim.

Po aktywacji użytkownicy w dzierżawie partnera są proszeni o ukończenie weryfikacji MFA podczas wykonywania jakichkolwiek operacji administratora w imieniu (AOBO), uzyskiwania dostępu do portalu Partner Center lub wywoływania interfejsów API Partner Center uwierzytelniania. Aby uzyskać więcej informacji, [zobacz Temat Wymuszanie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnera.](partner-security-requirements-mandating-mfa.md) 

Partnerzy, którzy nie spełnili wymagań, powinni wdrożyć te miary tak szybko, jak to możliwe, aby uniknąć zakłóceń w działalności biznesowej. Jeśli używasz usługi Azure Active Directory Multi-Factor Authentication lub ustawień domyślnych zabezpieczeń usługi Azure AD, nie musisz nic więcej zrobić.

Jeśli używasz rozwiązania MFA innej firmy, istnieje prawdopodobieństwo, że oświadczenie MFA nie zostanie wystawione. W przypadku braku tego oświadczenia usługa Azure AD nie będzie mogła określić, czy żądanie uwierzytelnienia zostało zakwestionowane przez usługę MFA. Aby uzyskać informacje na temat weryfikowania, czy rozwiązanie wystawia oczekiwane oświadczenie, przeczytaj temat Testing the Partner Security Requirements (Testowanie [wymagań zabezpieczeń partnera).](/powershell/partnercenter/test-partner-security-requirements) 

> [!IMPORTANT]
> Jeśli rozwiązanie innej firmy nie wystawia oczekiwanego oświadczenia, należy współpracować z dostawcą, który opracował rozwiązanie, aby określić, jakie działania należy podjąć.

## <a name="resources-and-samples"></a>Zasoby i przykłady

Zapoznaj się z następującymi zasobami, aby uzyskać pomoc techniczną i przykładowy kod:

- [Partner Center grupy wskazówek](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)dotyczących zabezpieczeń: społeczność grupy wskazówki dotyczące zabezpieczeń usługi Partner Center jest społecznością online, w której możesz dowiedzieć się więcej o nadchodzących wydarzeniach i zadawać dowolne pytania.
- [Partner Center przykładów dla programu .NET:](https://github.com/microsoft/partner-center-dotnet-samples)to repozytorium GitHub zawiera przykłady opracowane przy użyciu programu .NET, które pokazują, jak można zaimplementować model aplikacji zabezpieczonych platformę.
- [Partner Center przykładów dla języka Java:](https://github.com/microsoft/partner-center-java-samples)to GitHub zawiera przykłady opracowane przy użyciu języka Java, które pokazują, jak można zaimplementować model aplikacji zabezpieczonych platformę.
- [Partner Center PowerShell — Multi-Factor Authentication:](/powershell/partnercenter/multi-factor-auth)ten artykuł usługi Multi-Factor Authentication zawiera szczegółowe informacje na temat sposobu implementowania struktury model aplikacji zabezpieczonych przy użyciu programu PowerShell.

## <a name="next-steps"></a>Następne kroki

- [Upoważnianie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnera](partner-security-requirements-mandating-mfa.md)