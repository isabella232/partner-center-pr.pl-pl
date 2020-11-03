---
title: Wymagania dotyczące zabezpieczeń partnerów
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wprowadza wymagania dotyczące zabezpieczeń partnerów, aby umożliwić uwierzytelnianie wieloskładnikowe (MFA) i wdrożyć bezpieczną strukturę modelu aplikacji.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 351d0715645b6e43607279393cdc376d898a7f54
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132982"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Wymagania dotyczące zabezpieczeń w przypadku korzystania z interfejsów API Centrum partnerskiego lub platformy partnerskiej

**Dotyczy**

- Wszyscy partnerzy w programie dostawcy rozwiązań w chmurze
- Wszyscy dostawcy panelu sterowania
- Wszyscy klasyfikatory

**Odpowiednim użytkownikom**

- Wszyscy aktywni użytkownicy, w tym użytkownicy-Goście

W tym artykule wyjaśniono obowiązkowe wymagania dotyczące zabezpieczeń doradców, dostawców panelu sterowania i partnerów uczestniczących w programie dostawcy rozwiązań w chmurze, a także opcje uwierzytelniania i inne zagadnienia dotyczące zabezpieczeń. Bezpieczeństwo i zabezpieczenia prywatności znajdują się wśród naszych najważniejszych priorytetów. Wiemy, że najlepszą obroną jest zapobieganie i że jest to tylko silne rozwiązanie. Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie mogli działać i zapewnić odpowiednie zabezpieczenia.

## <a name="mandatory-security-requirements"></a>Obowiązkowe wymagania dotyczące zabezpieczeń

Partnerzy, którzy nie implementują obowiązkowych wymagań w zakresie zabezpieczeń, nie będą mogli wykonywać operacji Transact w programie dostawcy rozwiązań w chmurze ani zarządzać dzierżawcami klientów, korzystając z uprawnień delegowanych przez administratora. Ponadto partnerzy, którzy nie implementują wymagań związanych z bezpieczeństwem, mogą przystąpić do uczestnictwa w programach na ryzyko. Warunki związane z wymaganiami dotyczącymi zabezpieczeń partnerów zostały dodane do umowy partnerskiej firmy Microsoft. W miarę jak odnosi się do doradców, te same wymagania umowne będą spełnione.

Aby chronić użytkowników i klientów, firma Microsoft wymaga od razu podjęcia następujących działań:  

1. **Włącz uwierzytelnianie wieloskładnikowe (MFA) dla wszystkich kont użytkowników w dzierżawie partnera** . Musisz wymusić uwierzytelnianie wieloskładnikowe na wszystkich kontach użytkowników w dzierżawach partnerskich. Podczas logowania się do usług w chmurze komercyjnej firmy Microsoft lub w programie dostawcy rozwiązań w chmurze za pośrednictwem Centrum partnerskiego lub za pośrednictwem interfejsów API należy zakwestionować uwierzytelnianie wieloskładnikowe.

2. **Należy wdrożyć bezpieczną strukturę modelu aplikacji** . Wszyscy partnerzy, którzy integrują się z interfejsami API Centrum partnerskiego, muszą przyjmować [bezpieczną strukturę modelu aplikacji](/partner-center/develop/enable-secure-app-model) dla wszystkich aplikacji i aplikacji modelu uwierzytelniania użytkowników.

    > [!IMPORTANT]
    > Zdecydowanie zalecamy, aby partnerzy implementują bezpieczny model aplikacji na potrzeby integracji z interfejsem API firmy Microsoft, takimi jak Azure Resource Manager lub Microsoft Graph, lub w przypadku korzystania z automatyzacji, takiego jak program PowerShell, przy użyciu poświadczeń użytkownika, aby uniknąć przerw w działaniu usługi MFA.

Te wymagania dotyczące zabezpieczeń ułatwią ochronę infrastruktury i zabezpieczają dane klientów przed potencjalnymi zagrożeniami bezpieczeństwa, takimi jak identyfikowanie kradzieży lub innych zdarzeń oszustwa.  

## <a name="implementing-multi-factor-authentication"></a>Implementowanie uwierzytelniania wieloskładnikowego

Aby zapewnić zgodność z wymaganiami dotyczącymi zabezpieczeń partnerów, należy zaimplementować i wymusić uwierzytelnianie MFA dla każdego konta użytkownika w dzierżawie partnerskiej. Można to zrobić w następujący sposób:

- Implementowanie [domyślnych ustawień zabezpieczeń Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Więcej informacji znajduje się w [następnej sekcji](#security-defaults).

- Azure Active Directory — wersja Premium zakupów dla każdego konta użytkownika. Aby uzyskać więcej informacji, zobacz [Planowanie wdrożenia usługi Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-getstarted).

- Użyj rozwiązania innej firmy, aby wymusić uwierzytelnianie MFA dla każdego konta użytkownika w dzierżawie partnera. Aby zapewnić, że rozwiązanie zapewni oczekiwane rozwiązanie, zobacz [jak są wymuszane wymagania dotyczące zabezpieczeń](#how-the-requirements-are-enforced).

> [!NOTE]
> Chociaż uwierzytelnianie wieloskładnikowe nie jest objęte umową w przypadku instytucji suwerennych (rządowych Stanów Zjednoczonych i Niemiec), zdecydowanie zaleca się przyjęcie tych wymagań dotyczących zabezpieczeń.

### <a name="security-defaults"></a>Domyślne ustawienia zabezpieczeń

Jedną z opcji, które partnerzy mogą wdrożyć wymagania usługi MFA, jest włączenie ustawień domyślnych zabezpieczeń w usłudze Azure AD. Wartości domyślne zabezpieczeń oferują podstawowy poziom zabezpieczeń bez dodatkowych kosztów. Zapoznaj się z tematem Włączanie usługi MFA dla Twojej organizacji za pomocą usług Azure AD oraz najważniejszych zagadnień poniżej przed włączeniem ustawień domyślnych zabezpieczeń.

- Partnerzy, którzy już przyjęli zasady podstawowe, muszą podejmować działania w celu przejścia do domyślnych ustawień zabezpieczeń.

- Ustawienia domyślne zabezpieczeń to ogólna dostępność zasad dotyczących wersji zapoznawczej. Gdy Partner włącza ustawienia domyślne zabezpieczeń, nie będą już mogli włączać zasad bazowych.

- W przypadku ustawień domyślnych zabezpieczeń wszystkie zasady zostaną włączone jednocześnie.

- W przypadku partnerów, którzy korzystają z [dostępu warunkowego](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), [Ustawienia domyślne zabezpieczeń nie będą dostępne](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- W tej chwili nie zablokowano starszego uwierzytelniania. Jednak ponieważ większość zdarzeń związanych z tożsamościami złamanymi nie pochodzi z prób logowania przy użyciu starszego uwierzytelniania, zachęca się partnerów do przejścia od tych starszych protokołów.

- Konto synchronizacji Azure AD Connect jest wyłączone z domyślnych ustawień zabezpieczeń.

Aby uzyskać szczegółowe informacje, przeczytaj artykuł [Omówienie usługi Azure Multi-Factor Authentication dla organizacji](/azure/active-directory/authentication/concept-mfa-get-started) i [co to są wartości domyślne zabezpieczeń?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Domyślne ustawienia zabezpieczeń usługi Azure AD to ewolucja uproszczonych zasad ochrony. Jeśli zasady ochrony linii bazowej zostały już włączone, zdecydowanie zaleca się włączenie [ustawień domyślnych zabezpieczeń](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Istotne informacje dotyczące implementacji

Ponieważ te wymagania dotyczą wszystkich kont użytkowników w dzierżawie partnerskiej, należy wziąć pod uwagę kilka rzeczy, aby zapewnić płynne wdrożenie. Na przykład Zidentyfikuj konta użytkowników w usłudze Azure AD, które nie mogą wykonywać MFA, a także aplikacje i urządzenia w organizacji, które nie obsługują nowoczesnego uwierzytelniania.

Przed wykonaniem jakiejkolwiek akcji zalecamy wykonanie następujących walidacji. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Czy masz aplikację lub urządzenie, które nie obsługuje korzystania z nowoczesnego uwierzytelniania?

W przypadku wymuszania usługi MFA starsze uwierzytelnianie używa protokołów takich jak IMAP, POP3, SMTP itp., ponieważ nie obsługują usługi MFA. Aby rozwiązać ten limit, użyj funkcji [hasła aplikacji](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) , aby upewnić się, że aplikacja lub urządzenie nadal będzie się uwierzytelniać. Zapoznaj się z [zagadnieniami dotyczącymi używania haseł aplikacji](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) w celu ustalenia, czy mogą one być używane w danym środowisku.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Czy masz użytkowników pakietu Office 365 z licencjami skojarzonymi z dzierżawcą partnerskim?

Przed wdrożeniem jakichkolwiek rozwiązań zalecamy określenie, która wersja Microsoft Office użytkowników w dzierżawie partnerskiej jest używana. Istnieje możliwość, że użytkownicy będą napotykać problemy z łącznością z aplikacjami, takimi jak program Outlook. Przed wymuszeniem usługi MFA należy upewnić się, że korzystasz z programu Outlook 2013 z dodatkiem SP1 lub nowszego oraz że Twoja organizacja ma włączone nowoczesne uwierzytelnianie. Aby uzyskać więcej informacji, zobacz [Włączanie nowoczesnego uwierzytelniania w usłudze Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Aby włączyć nowoczesne uwierzytelnianie dla urządzeń z systemem Windows, na których zainstalowano Microsoft Office 2013, należy utworzyć dwa klucze rejestru. Zobacz [Włączanie nowoczesnego uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Czy istnieją zasady uniemożliwiające innym użytkownikom korzystanie z urządzeń przenośnych podczas pracy?

Ważne jest, aby zidentyfikować wszelkie zasady firmowe, które uniemożliwiają pracownikom korzystanie z urządzeń przenośnych w trakcie pracy, ponieważ wpłynie to na to, jakie rozwiązanie MFA zostało wdrożone. Istnieją rozwiązania, takie jak te udostępniane w ramach implementacji [ustawień zabezpieczeń usługi Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), które umożliwiają weryfikację tylko przy użyciu aplikacji uwierzytelniania. Jeśli organizacja ma zasady uniemożliwiające korzystanie z urządzeń przenośnych, należy wziąć pod uwagę jedną z następujących opcji:

- Wdróż jednogodzinną aplikację hasła podstawowego (TOTP), która może być uruchamiana w bezpiecznym systemie.

- Zaimplementuj rozwiązanie innych firm, które wymusza uwierzytelnianie MFA dla każdego konta użytkownika w dzierżawie partnera, który zapewnia najbardziej odpowiednią opcję weryfikacji.

- Kup licencje [Azure Active Directory — wersja Premium](https://azure.microsoft.com/pricing/details/active-directory/) dla użytkowników, których dotyczy problem.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Jakiej automatyzacji lub integracji musisz użyć poświadczeń użytkownika do uwierzytelniania?

Ponieważ wymuszamy uwierzytelnianie wieloskładnikowe dla każdego użytkownika, w tym konta usług, w katalogu partnerów będzie to miało wpływ na dowolną automatyzację lub integrację korzystającą z poświadczeń użytkownika w celu uwierzytelniania. Dlatego ważne jest, aby identyfikować, które konta są używane w takich sytuacjach. Zapoznaj się z następującą listą przykładowych aplikacji lub usług, które należy wziąć pod uwagę:

- Panel sterowania służący do udostępniania zasobów w imieniu klientów

- Integracja z dowolną platformą używaną do fakturowania (odnoszącej się do programu CSP) i obsługiwania klientów

- Skrypty programu PowerShell korzystające z modułów AZ, AzureRM, Azure AD, MS online itd.

Powyższa lista nie jest kompletna. W związku z tym ważne jest, aby przeprowadzić pełną ocenę wszelkich aplikacji lub usług w środowisku, które korzystają z poświadczeń użytkownika w celu uwierzytelniania. Aby będą konkurować o z wymaganiem uwierzytelniania wieloskładnikowego, należy zaimplementować wskazówki w [strukturze bezpiecznego modelu aplikacji](/partner-center/develop/enable-secure-app-model) , o ile jest to możliwe.

## <a name="accessing-your-environment"></a>Uzyskiwanie dostępu do środowiska

Aby lepiej zrozumieć, co lub kto jest uwierzytelniany bez wyzwania dla usługi MFA, zalecamy przejrzenie działania związanego z logowaniem. Za pomocą Azure Active Directory — wersja Premium można wykorzystać raport logowania. Aby uzyskać więcej informacji na temat tego tematu, zobacz [raporty dotyczące działań związanych z logowaniem w portalu Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Jeśli nie masz Azure Active Directory — wersja Premium lub wiesz, jak uzyskać te działania związane z logowaniem za pośrednictwem programu PowerShell, musisz użyć polecenia cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) w module [programu PowerShell Centrum partnerskiego](https://www.powershellgallery.com/packages/PartnerCenter/) .

## <a name="how-the-requirements-are-enforced"></a>Jak są wymuszane wymagania

Wymagania dotyczące zabezpieczeń partnerów są wymuszane przez usługę Azure AD, a w centrum partnerskim przez sprawdzenie obecności żądania MFA w celu zidentyfikowania przeprowadzenia weryfikacji MFA. Od 18 listopada 2019 firma Microsoft opracowała dodatkowe zabezpieczenia zabezpieczeń (wcześniej znane jako "wymuszanie techniczne") dla dzierżawców partnerskich.

Po aktywacji użytkownicy z dzierżawy partnerskiej są żądani do ukończenia weryfikacji MFA podczas wykonywania jakichkolwiek czynności administratora w imieniu (AOBO), uzyskiwania dostępu do portalu Centrum partnerskiego lub wywoływania interfejsów API Centrum partnerskiego. Aby uzyskać więcej informacji, zobacz temat [uwierzytelnianie wieloskładnikowe (MFA) dla dzierżawy partnerskiej](partner-security-requirements-mandating-mfa.md). 

Partnerzy, którzy nie spełniają wymagań, powinni wdrożyć te środki najszybciej, jak to możliwe, aby uniknąć przerw w działaniu firmy. Jeśli używasz usługi Azure Multi-Factor Authentication lub domyślnych ustawień zabezpieczeń usługi Azure AD, nie musisz wykonywać żadnych dodatkowych czynności.

Jeśli używasz rozwiązania MFA innej firmy, istnieje możliwość, że nie można wystawić żądania MFA. W przypadku braku tego żądania usługa Azure AD nie będzie w stanie określić, czy żądanie uwierzytelnienia zostało zakwestionowane przez usługę MFA. Aby uzyskać informacje o tym, jak sprawdzić, czy Twoje rozwiązanie wystawia oczekiwane zastrzeżenie, przeczytaj temat [wymagania dotyczące zabezpieczeń partnerów](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Jeśli rozwiązanie innej firmy nie wystawia oczekiwanego odszkodowania, należy skontaktować się z dostawcą, który opracował rozwiązanie, aby określić, jakie działania powinny zostać podjęte.

## <a name="resources-and-samples"></a>Zasoby i przykłady

Zapoznaj się z poniższymi zasobami, aby uzyskać pomoc techniczną i przykładowy kod:

- [Społeczność grupy wskazówek dotyczących zabezpieczeń Centrum partnerskiego](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): społeczności online Centrum partnerskiego — wskazówki dotyczące zabezpieczeń, które można poznać w przypadku nadchodzących wydarzeń i zadać pytania.
- [Przykłady platformy .NET Centrum partnerskiego](https://github.com/microsoft/partner-center-dotnet-samples): to repozytorium GitHub zawiera przykłady opracowane przy użyciu platformy .NET, które pokazują, jak można wdrożyć bezpieczną strukturę modelu aplikacji.
- [Przykłady środowiska Java Centrum partnerskiego](https://github.com/microsoft/partner-center-java-samples): to repozytorium GitHub zawiera przykłady opracowane przy użyciu języka Java, które pokazują, jak można wdrożyć bezpieczną strukturę modelu aplikacji.
- [Centrum partnerskie programu PowerShell — Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): ten Multi-Factor Authentication artykuł zawiera szczegółowe informacje na temat implementowania struktury bezpiecznego modelu aplikacji przy użyciu programu PowerShell.

## <a name="next-steps"></a>Następne kroki

- [Wymaganie uwierzytelniania wieloskładnikowego (MFA) dla dzierżawy partnerskiej](partner-security-requirements-mandating-mfa.md)