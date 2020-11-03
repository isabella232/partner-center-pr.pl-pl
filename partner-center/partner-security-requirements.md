---
title: Wymagania dotyczące zabezpieczeń partnerów
ms.topic: article
ms.date: 10/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wprowadza Wymagania partnerskie umożliwiające włączenie uwierzytelniania wieloskładnikowego (MFA) i zastosowanie platformy bezpiecznego modelu aplikacji.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 361a36adf40af67769a9a24ba1c485f2ad95b98c
ms.sourcegitcommit: 8a4a3de728532533276a88b1fd40c82b7a4ebb15
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2020
ms.locfileid: "92530219"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Wymagania dotyczące bezpieczeństwa partnerów w przypadku partnerów przy użyciu Centrum partnerskiego lub interfejsów API Centrum partnerskiego

**Dotyczy**

- Wszyscy partnerzy w programie dostawcy rozwiązań w chmurze
  - Rachunek bezpośredni
  - Dostawca pośredni
  - Pośredni odsprzedawca
- Wszyscy dostawcy panelu sterowania
- Wszyscy klasyfikatory

**Odpowiednim użytkownikom**

- Wszyscy aktywni użytkownicy, w tym użytkownicy-Goście

Lepsze zabezpieczenia i bezpieczeństwo ochrony prywatności znajdują się wśród naszych najważniejszych priorytetów. Wiemy, że najlepszą obroną jest zapobieganie i że jest to tylko silne rozwiązanie. Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie mogli działać i zapewnić odpowiednie zabezpieczenia. Aby pomóc w zabezpieczeniu partnerów i klientów, wprowadzamy zestaw obowiązkowych wymagań w zakresie zabezpieczeń dla doradców, dostawców panelu sterowania i partnerów uczestniczących w programie dostawcy rozwiązań w chmurze.

## <a name="overview"></a>Omówienie

Partnerzy są zobowiązani do wymuszania uwierzytelniania wieloskładnikowego dla wszystkich kont użytkowników w dzierżawie partnera. Warunki związane z wymaganiami dotyczącymi zabezpieczeń partnerów zostały dodane do umowy partnerskiej firmy Microsoft. W miarę jak odnosi się do doradców, te same wymagania umowne będą spełnione.

Partnerzy, którzy nie implementują obowiązkowych wymagań w zakresie zabezpieczeń, nie będą mogli wykonywać operacji Transact w programie dostawcy rozwiązań w chmurze ani zarządzać dzierżawami klientów, korzystając z delegowanych praw administratora, gdy te wymagania zostaną wymuszone. Ponadto partnerzy, którzy nie implementują wymagań związanych z bezpieczeństwem, mogą przystąpić do uczestnictwa w programach na ryzyko.  

Aby chronić użytkowników i klientów, firma Microsoft wymaga od razu podjęcia następujących działań:  

1. **Włącz Multi-Factor Authentication (MFA) dla wszystkich kont użytkowników w dzierżawie partnera** . Podczas logowania się do komercyjnych usług w chmurze firmy Microsoft lub w programie Cloud Solution Provider za pośrednictwem usługi Partner Center lub interfejsów API należy zakwestionować wszystkie konta użytkowników w dzierżawach partnerskich.

2. **Należy wdrożyć bezpieczną strukturę modelu aplikacji** . Należy wdrożyć bezpieczną strukturę modelu aplikacji. Wszyscy partnerzy, którzy integrują się z interfejsem API Centrum partnerskiego, muszą przyjmować bezpieczną strukturę modelu aplikacji dla wszystkich aplikacji i aplikacji modelu uwierzytelniania użytkowników.

    > [!IMPORTANT]
    > Zdecydowanie zalecamy, aby partnerzy implementują bezpieczny model aplikacji na potrzeby integracji z interfejsem API firmy Microsoft, takim jak Azure Resource Manager, Microsoft Graph lub wykorzystując automatyzację, taką jak program PowerShell przy użyciu poświadczeń użytkownika, aby uniknąć przerw w działaniu usługi MFA.

Włączenie usługi Multi-Factor Authentication (MFA) i wdrożenie bezpiecznej struktury modelu aplikacji pomoże chronić infrastrukturę i chronić dane klientów przed potencjalnymi zagrożeniami bezpieczeństwa, takimi jak identyfikowanie kradzieży lub innych zdarzeń oszustwa.  

## <a name="actions-that-you-need-to-take"></a>Akcje, które należy wykonać

Aby zapewnić zgodność z wymaganiami dotyczącymi zabezpieczeń partnerów, należy wymusić uwierzytelnianie wieloskładnikowe dla każdego konta użytkownika w dzierżawie partnerskiej. Można to zrobić w następujący sposób:

- Implementowanie [domyślnych ustawień zabezpieczeń usługi Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Azure Active Directory — wersja Premium zakupów dla każdego konta użytkownika. Aby uzyskać więcej informacji, zobacz [Planowanie wdrożenia usługi Azure Multi-Factor Authentication opartej na chmurze](/azure/active-directory/authentication/howto-mfa-getstarted).

- Korzystanie z rozwiązania innej firmy w celu wymuszenia uwierzytelniania wieloskładnikowego dla każdego konta użytkownika w dzierżawie partnerskiej. Aby zapewnić, że rozwiązanie zapewni oczekiwane rozwiązanie, zobacz [jak są wymuszane wymagania dotyczące zabezpieczeń](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Mimo że uwierzytelnianie wieloskładnikowe nie jest objęte umową w chmurze suwerennej (21Vianet, Administracja USA i Niemcy), zdecydowanie zaleca się zastosowanie tych wymagań dotyczących zabezpieczeń.

## <a name="security-defaults"></a>Domyślne ustawienia zabezpieczeń

Zasady ustawień domyślnych zabezpieczeń są jedną z [opcji](#actions-that-you-need-to-take) , które partnerzy mogą wybrać wdrożenie usługi MFA w celu spełnienia wymagań dotyczących zabezpieczeń w zależności od potrzeb firmy. Oferuje on podstawowy poziom zabezpieczeń włączony bez dodatkowych kosztów. Zapoznaj się z tematem Włączanie usługi MFA dla Twojej organizacji za pomocą usług Azure AD oraz najważniejszych zagadnień poniżej przed włączeniem ustawień domyślnych zabezpieczeń.

- Zasady linii bazowej będą pozostawać w ciągu następnych kilku miesięcy i przestarzałe na koniec 2020 lutego.

- Partnerzy, którzy już przyjęli zasady podstawowe, muszą podejmować działania w celu przejścia do domyślnych ustawień zabezpieczeń.

- Ustawienia domyślne zabezpieczeń to ogólna dostępność zasad dotyczących wersji zapoznawczej. Gdy Partner włącza ustawienia domyślne zabezpieczeń, nie będą już mogli włączać zasad bazowych.

- W przypadku ustawień domyślnych zabezpieczeń wszystkie zasady zostaną włączone jednocześnie.

- W przypadku partnerów, którzy korzystają z [dostępu warunkowego](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), [Ustawienia domyślne zabezpieczeń nie będą dostępne](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Blokowanie starszego uwierzytelniania nie będzie wymuszane dla partnerów w tym momencie. Jednak ponieważ większość zdarzeń związanych z tożsamościami złamanymi nie pochodzi z prób logowania przy użyciu starszego uwierzytelniania, zachęca się partnerów do przejścia od tych starszych protokołów.

- Konto synchronizacji Azure AD Connect jest wyłączone z domyślnych ustawień zabezpieczeń.

- Aby uzyskać szczegółowe informacje, przeczytaj artykuł [włączanie Multi-Factor Authentication w organizacji](/azure/active-directory/authentication/concept-mfa-get-started) i [Azure Active Directory ustawień domyślnych zabezpieczeń](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Domyślne ustawienia zabezpieczeń usługi Azure AD to ewolucja uproszczonych zasad ochrony. Jeśli zasady ochrony linii bazowej zostały już włączone, zdecydowanie zaleca się włączenie ustawień domyślnych zabezpieczeń.

Aby przejść z zasad linii bazowej do domyślnych ustawień zabezpieczeń, Przeczytaj [co to są wartości domyślne zabezpieczeń?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Kwestie do rozważenia

Ponieważ te wymagania dotyczą wszystkich kont użytkowników w dzierżawie partnerskiej, należy wziąć pod uwagę kilka rzeczy, aby zapewnić płynne wdrożenie, w tym identyfikowanie kont użytkowników w Azure Active Directory, które nie mogą korzystać z uwierzytelniania wieloskładnikowego, a także aplikacje i urządzenia używane przez organizację, które nie obsługują nowoczesnego uwierzytelniania.

Przed wykonaniem jakiejkolwiek akcji zalecamy zidentyfikowanie następujących danych:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Czy masz aplikację lub urządzenie, które nie obsługuje korzystania z nowoczesnego uwierzytelniania?

W przypadku wymuszania uwierzytelniania wieloskładnikowego przy użyciu protokołów takich jak IMAP, POP3, SMTP itp. zostanie zablokowany, ponieważ nie obsługują uwierzytelniania wieloskładnikowego. Aby rozwiązać ten limit, funkcja nazywana [hasłami aplikacji](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) może służyć do upewnienia się, że aplikacja lub urządzenie nadal będzie się uwierzytelniać. Należy zapoznać się z zagadnieniami dotyczącymi używania haseł aplikacji opisanych [tutaj](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) , aby określić, czy mogą być używane w danym środowisku.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Czy użytkownicy korzystają z pakietu Office 365 dostarczonego przez licencje skojarzone z dzierżawcą partnerskim?

Przed wdrożeniem jakichkolwiek rozwiązań zalecamy określenie, która wersja Microsoft Office jest używana przez użytkowników w dzierżawie partnera. Istnieje możliwość, że użytkownicy będą napotykać problemy z łącznością z aplikacjami, takimi jak program Outlook. Przed wymuszeniem uwierzytelniania wieloskładnikowego należy upewnić się, że jest używany program Outlook 2013 z dodatkiem SP1 lub nowszy, a organizacja ma włączone nowoczesne uwierzytelnianie. Aby uzyskać więcej informacji, zobacz [Włączanie nowoczesnego uwierzytelniania w usłudze Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) .

Aby włączyć nowoczesne uwierzytelnianie dla wszystkich urządzeń z systemem Windows, na których zainstalowano Microsoft Office 2013, należy utworzyć dwa klucze rejestru. Zobacz [Włączanie nowoczesnego uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Czy istnieją zasady uniemożliwiające innym użytkownikom korzystanie z urządzeń przenośnych podczas pracy?

Ważne jest, aby zidentyfikować wszelkie zasady firmowe, które uniemożliwiają pracownikom korzystanie z urządzeń przenośnych w trakcie pracy, ponieważ wpłynie to na to, jakie rozwiązanie uwierzytelniania wieloskładnikowego zostanie wdrożone. Istnieją rozwiązania, takie jak te udostępniane w ramach implementacji [ustawień zabezpieczeń usługi Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), które umożliwiają weryfikację tylko przy użyciu aplikacji uwierzytelniania. Jeśli organizacja ma zasady uniemożliwiające korzystanie z urządzeń przenośnych, należy wziąć pod uwagę jedną z następujących opcji:

- Wdrażanie opartego na czasie jednorazowej aplikacji hasła podstawowego (TOTP), która może być uruchamiana w bezpiecznym systemie

- Implementowanie rozwiązania innej firmy, które wymusza uwierzytelnianie wieloskładnikowe dla każdego konta użytkownika w dzierżawie partnera, który zapewnia najbardziej odpowiednią opcję weryfikacji

- Kup licencje [Azure Active Directory — wersja Premium](https://azure.microsoft.com/pricing/details/active-directory/) dla użytkowników, których dotyczy problem

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Jakiej automatyzacji lub integracji musisz użyć poświadczeń użytkownika do uwierzytelniania?

Ponieważ wymaga to wymuszenia uwierzytelniania wieloskładnikowego dla każdego użytkownika, łącznie z kontami usług, w katalogu partnerskim będzie to miało wpływ na dowolną automatyzację lub integrację, która wykorzystuje poświadczenia użytkownika na potrzeby uwierzytelniania. Dlatego ważne jest, aby identyfikować, które konta są używane w takich sytuacjach. Zapoznaj się z następującą listą przykładowych aplikacji lub usług, które należy wziąć pod uwagę:

- Panel sterowania służący do udostępniania zasobów w imieniu klientów

- Integracja z dowolną platformą używaną do fakturowania (odnoszącej się do programu CSP) i obsługiwania klientów

- Skrypty programu PowerShell korzystające z modułów AZ, AzureRM, Azure AD, MS online itd.

Powyższa lista nie jest kompletna. W związku z tym ważne jest, aby przeprowadzić pełną ocenę wszelkich aplikacji lub usług w środowisku, które korzystają z poświadczeń użytkownika w celu uwierzytelniania. Aby będą konkurować o z wymaganiem uwierzytelniania wieloskładnikowego, należy zaimplementować wskazówki w [strukturze bezpiecznego modelu aplikacji](/partner-center/develop/enable-secure-app-model) , o ile jest to możliwe.

## <a name="accessing-your-environment"></a>Uzyskiwanie dostępu do środowiska

Aby lepiej zrozumieć, co lub kto jest uwierzytelniany bez wezwania do uwierzytelniania wieloskładnikowego, zalecamy przejrzenie działania związanego z logowaniem. Za pomocą Azure Active Directory — wersja Premium można wykorzystać raport logowania. Aby uzyskać więcej informacji [, zobacz raporty dotyczące działań związanych z logowaniem w portalu Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins) . Jeśli nie masz Azure Active Directory — wersja Premium lub wiesz, jak można to zrobić za pomocą programu PowerShell, musisz użyć polecenia cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity)  w module [programu PowerShell Centrum partnerskiego](https://www.powershellgallery.com/packages/PartnerCenter/) .

## <a name="how-the-requirements-will-be-enforced"></a>Jak zostaną wymuszone wymagania

Wymagania dotyczące zabezpieczeń partnerów będą wymuszane przez Azure Active Directory i w centrum partnerskim, sprawdzając obecność żądania MFA w celu zidentyfikowania, czy przeprowadzono weryfikację uwierzytelniania wieloskładnikowego. Od 18 listopada 2019 firma Microsoft będzie aktywować dodatkowe zabezpieczenia zabezpieczeń (wcześniej znane jako "wymuszanie techniczne") dla dzierżawców partnerskich. 

Po aktywacji użytkownicy z dzierżawy partnerskiej otrzymają żądanie przeprowadzenia weryfikacji uwierzytelniania wieloskładnikowego (MFA) podczas wykonywania jakichkolwiek czynności administracyjnych w imieniu (AOBO). Będziemy nadal rozszerzać zakres zabezpieczeń na dodatkowe scenariusze i role użytkowników, zapewniając partnerów z wyprzedzeniem. Aby uzyskać więcej informacji, zapoznaj się z tym dokumentem, który będzie często aktualizowany. Partnerzy, którzy nie spełniają wymagań, powinni wdrożyć te środki najszybciej, jak to możliwe, aby uniknąć przerw w działaniu firmy. 

Jeśli używasz usługi Azure Multi-Factor Authentication lub domyślnych ustawień zabezpieczeń usługi Azure AD, nie musisz wykonywać żadnych dodatkowych czynności.

W przypadku korzystania z rozwiązania do uwierzytelniania wieloskładnikowego innej firmy istnieje możliwość, że nie można wystawić żądania MFA. W przypadku braku tego żądania Azure Active Directory nie będzie można określić, czy żądanie uwierzytelnienia zostało zakwestionowane przez uwierzytelnianie wieloskładnikowe. Aby uzyskać informacje o tym, jak sprawdzić, czy Twoje rozwiązanie wystawia oczekiwane zastrzeżenie, przeczytaj temat [wymagania dotyczące zabezpieczeń partnerów](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Jeśli rozwiązanie innej firmy nie wystawia oczekiwanego odszkodowania, należy skontaktować się z dostawcą, który opracował rozwiązanie, aby określić, jakie działania powinny zostać podjęte.

## <a name="resources-and-support"></a>Zasoby i pomoc techniczna

Zapoznaj się z poniższymi zasobami, aby uzyskać pomoc techniczną i przykładowy kod:

- [Społeczność grupy wskazówek dotyczących zabezpieczeń Centrum partnerskiego](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): społeczności online Centrum partnerskiego — wskazówki dotyczące zabezpieczeń, które można poznać w przypadku nadchodzących wydarzeń i zadać pytania.
- [Przykłady platformy .NET Centrum partnerskiego](https://github.com/microsoft/partner-center-dotnet-samples): to repozytorium GitHub zawiera przykłady opracowane przy użyciu platformy .NET, które pokazują, jak można wdrożyć bezpieczną strukturę modelu aplikacji.
- [Przykłady środowiska Java Centrum partnerskiego](https://github.com/microsoft/partner-center-java-samples): to repozytorium GitHub zawiera przykłady opracowane przy użyciu języka Java, które pokazują, jak można wdrożyć bezpieczną strukturę modelu aplikacji.
- [Centrum partnerskie programu PowerShell — Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): ten Multi-Factor Authentication artykuł zawiera szczegółowe informacje na temat implementowania struktury bezpiecznego modelu aplikacji przy użyciu programu PowerShell.