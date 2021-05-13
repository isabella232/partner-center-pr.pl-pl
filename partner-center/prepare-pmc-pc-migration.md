---
title: Przechodzenie z Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Przejrzyj przydatne informacje i często zadawane pytania przed przeniesieniem firmy z Partner Membership Center do Partner Center.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f533240d5236f03fe277d4c6dfa02ed1c58b63c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855016"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Przygotowanie do przeniesienia z Partner Membership Center (PMC) do Partner Center

**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent sprzedaży | Agent administracyjny

Przenosimy zarządzanie członkostwem z Partner Membership Center (PMC) do Partner Center — pojedynczego miejsca docelowego do zarządzania relacjami biznesowymi z firmą Microsoft. Chcemy, aby Twoje przejście do Partner Center było tak wydajne i łatwe, jak to możliwe. Zidentyfikowaliśmy kilka obszarów, w których Partner Center różni się od PMC, i uważamy, że przed ich przeniesieniem należy je zrozumieć i przygotować.

## <a name="account-and-identity-setup"></a>Konfiguracja konta i tożsamości

Poniżej znajdują się odpowiedzi na często zadawane pytania dotyczące konfigurowania konta i tożsamości.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Co to jest konto Azure Active Directory (Azure AD)?

Konto służbowe platformy Azure to dedykowana i odizolowana wirtualna reprezentacja firmy w chmurze publicznej platformy Azure, utworzona automatycznie podczas subskrybowania usługi w chmurze firmy Microsoft, takiej jak Azure, Microsoft Intune lub Office 365.

Konto służbowe hostuje użytkowników usługi Azure AD oraz informacje o nich — ich pocztę e-mail, hasła, dane profilu, uprawnienia i tak dalej. Konto służbowe zawiera również grupy, aplikacje i inne informacje dotyczące firmy i jej zabezpieczeń. 

Służbowy adres e-mail jest częścią dzierżawy usługi Azure Active Directory. Aby mieć konto w Partner Center, musisz mieć dzierżawę usługi AAD. Aby uzyskać więcej informacji na Azure Active Directory, przeczytaj [tworzenie katalogu w usłudze Azure AD.](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)

W Partner Center użyjesz służbowego adresu e-mail, aby zalogować się do swojego konta, a nie do osobistego adresu e-mail.

- Twoje konto służbowe: john@contoso.com
- Twoje konto osobiste: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Za pomocą jakiego konta należy się zalogować Partner Center, jeśli masz dzierżawę usługi AAD z firmą Microsoft (na przykład dla usługi Office 365) i masz również dzierżawę dla swojej firmy CSP?

Możesz zalogować się do Partner Center przy użyciu konta CSP lub służbowego konta e-mail MPN. Jeśli zdecydujesz się zalogować się przy użyciu służbowego adresu e-mail CSP, na lewym pasku nawigacyjnym będą wyświetlane informacje o programie MPN i CSP. Jeśli zalogujesz się przy użyciu służbowego adresu e-mail dzierżawy usługi Azure AD w usłudze MPN, zobaczysz tylko informacje o programie MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Jeśli nie chcesz używać istniejącej dzierżawy usługi Azure AD usługi Office 365 dla usługi Partner Center, możesz utworzyć nową dzierżawę przed migracją z usługi PMC.

Istnieje wiele powodów, dla których nie chcesz używać istniejącej dzierżawy usługi Azure AD do skonfigurowania konta Partner Center usługi. Przed rozpoczęciem migracji do usługi Partner Center przejdź do [](https://ms.portal.azure.com/#home) strony Azure Portal, aby utworzyć nową dzierżawę usługi Azure AD. Postępuj zgodnie ze wskazówkami [z tematu Tworzenie nowej dzierżawy w Azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Użyj nowej dzierżawy usługi AAD, aby skonfigurować Partner Center usługi. Aby utworzyć dzierżawę, musisz być administratorem globalnym. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Role użytkowników, w tym role użytkowników-gości w Partner Center

Partner Center ma różne typy ról w zależności od rodzaju pracy, która musi zostać wykonana. Istnieją role, takie jak administrator globalny, które są rolami usługi Azure AD. Niektóre role są specyficzne dla programów, takich jak program dostawcy usług w chmurze lub zachęty, i istnieją role specyficzne dla programu MPN. Aby dowiedzieć się, czym są wszystkie Partner Center, zobacz [Przypisywanie ról i uprawnień użytkowników.](permissions-overview.md)

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Co się stanie z rolami moich użytkowników, gdy przejdą z pmc do Partner Center?

Z wyjątkiem administratora globalnego programu MPN lub osoby kontaktowej w programie podstawowym, który przeprowadza migrację, wszyscy użytkownicy w programie PMC utracą swoje role administratora. Osoba, która ukończy migrację, musi przypisać role w Partner Center. Role w Partner Center różnią się od ról w programie PMC. Przeczytaj [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md i [Moving from PMC to Partner Center](move-pmc-pc-map.md#user-roles) for more on user roles in Partner Center (Przypisywanie ról i uprawnień użytkowników)).

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Jaka jest różnica między moim profilem firmy i moim profilem biznesowym?

Profil firmy to informacje o firmie, takie jak adres, lokalizacje, podstawowa osoba kontaktowa, bank i szczegóły podatkowe.

Twój profil biznesowy przedstawia się klientom i jest stroną marketingową, na która jest wyświetlane logo, szczegółowe informacje dotyczące firmy, wiedzy specjalistycznej itp.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Co oznacza konsolidacja konta dla mojego konta?

Jeśli używasz tej samej dzierżawy usługi Azure AD do migrowania wielu kont MPN do usługi Partner Center, system automatycznie je rozpozna i poprosi o skonsolidowanie kont. Dotyczy to nawet przypadku, gdy z tą samą dzierżawą usługi Azure AD jest skojarzonych wiele domen. 

Nadal możesz zdecydować się na migrację do usługi Partner Center przy użyciu oddzielnych dzierżaw usługi AAD, ale zwróć uwagę na to, że skutkuje to izolowaną oceną Twoich kompetencji i dodatkowymi kosztami zakupu. Aby uzyskać więcej informacji na temat konsolidacji kont, przeczytaj [konsolidowanie kont firmowych](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Jeśli mam wiele dzierżaw usługi AAD i jedno konto MPN, czy istnieje możliwość połączenia ich w Partner Center?

Tak, w Partner Center można połączyć wiele dzierżaw usługi Azure AD z jednym Partner Center kontem.
Aby uzyskać więcej informacji na temat konsolidacji kont, przeczytaj [konsolidowanie kont firmowych](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Czy istnieją ograniczenia dotyczące dodawania wielu dzierżaw usługi Azure AD do jednego Partner Center konta?

Jeśli dzierżawa usługi Azure AD jest już skojarzona z istniejącym kontem usługi Partner Center, nie można jej skojarzyć z nowymi kontami usługi Partner Center przy użyciu funkcji wielodostępności. Innym sposobem, aby o tym myśleć, jest to, że dzierżawę usługi Azure AD można skojarzyć tylko z jednym kontem usługi Partner Center, ale konto usługi Partner Center może mieć skojarzonych wiele dzierżaw.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) 

Zapoznaj się z poniższymi odpowiedziami na często zadawane pytania dotyczące migracji członkostwa w programie MPN.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Kto może wykonać przeniesienie z pmc do Partner Center?

Administrator globalny programu MPN w firmie lub kontakt z programem podstawowym (te dwie role są często przechowywane przez tę samą osobę) może zainicjować i wykonać przeniesienie.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Czy osoba kończąca migrację stanie się główną osobą kontaktową w profilu prawnym firmy w Partner Center?

Niekoniecznie jednak podstawowym kontaktem musi być ktoś, kto ma autoryzację do podpisywania umów.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Czy firma Microsoft może migrować moje członkostwo w programie MPN?

Nie. Firma Microsoft nie może pomóc w przenoszeniu konta członkostwa do Centrum partnerskiego. Aby rozpocząć proces migracji, musisz przenieść konto, logując się do usługi PMC przy użyciu konta służbowego (poświadczenia logowania). Po ukończeniu kroków przenoszenia konta możesz rozpocząć zarządzanie członkostwem i przypisać role i uprawnienia użytkowników do zespołu, aby uzyskać dostęp do korzyści i ułatwić zarządzanie członkostwem. 

Firma Microsoft będzie automatycznie migrować bieżące kompetencje, korzyści, informacje o lokalizacji, informacje bankowe/podatkowe dla zachęt oraz skojarzenia MCP, w tym dostęp do witryny Partner University.

### <a name="how-will-the-renewal-policy-change"></a>Jak zmienią się zasady odnawiania?

W Partner Center okres odnawiania przypada od daty rocznicy do następnych 30 dni.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Czy nasze kompetencje pozostaną niezmienione po zmianie Partner Center?

Tak, przejście do Partner Center nie będzie mieć wpływu na kompetencje. Jeśli zauważysz rozbieżności, skontaktuj się z pomocą [techniczną.](https://partner.microsoft.com/support)

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Czy moje korzyści (w tym korzyści z chmury, pomoc techniczna, korzyści z oprogramowania, Visual Studio) zmienią się po zakończeniu przenoszenia?

Kwalifikujące się korzyści nie zmienią się. Jeśli zauważysz rozbieżności, skontaktuj się z pomocą [techniczną.](https://partner.microsoft.com/support)

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Czy nasze konta Microsoft, które Visual Studio alokacje korzyści, zostaną honorowane?

Tak. Visual Studio korzyści przydzielone do msa będą honorowane i zachowywane. Zostaną one również zachowane po odnowieniu w Partner Center. Jeśli jednak usuniesz alokację msa po migracji do Partner Center, nie będzie można jej dodać z powrotem do Partner Center.

W Partner Center partner może dodać konta służbowe i konta użytkowników-gości, które są kontami MSA z tej samej dzierżawy, w której partner jest administratorem MPN w dzierżawie usługi Azure AD. Jeśli partner jest administratorem globalnym w wielu dzierżawach usługi Azure AD i wszystkie te dzierżawy są skojarzone z tym samym kontem usługi Partner Center, partner może dodawać użytkowników we wszystkich tych dzierżawach do korzyści usługi Visual Studio i alokacji opartych na użyciu platformy Azure.

Mimo że użytkownicy-goście mogą mieć przypisane subskrypcje usługi Visual Studio oparte na użyciu przez administratora MPN lub administratora globalnego, użytkownicy-goście nie mogą logować się do usługi Partner Center przy użyciu konta MSA. Użytkownicy-goście mogą jednak zalogować się do platformy Azure i Visual Studio, aby zweryfikować i wykorzystać przypisane im korzyści.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Jak należy zarządzać naszymi skojarzeniami MCP i dostępem do uczelni Partner University?

Nie ma żadnych zmian skojarzeń MCP, które są zmieniane z PMC. Jednak nowi pracownicy po przeprowadzce do Partner Center będą musieli być skojarzone w Partner Center. Wszystkie twoje uprawnienia witryny Partner University dla istniejących użytkowników [](https://partner.microsoft.com/training) pozostaną, ale wszyscy nowi pracownicy powinni przejść do centrum szkoleniowego, aby uzyskać informacje na temat sposobu uzyskania dostępu do witryny Partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Jak mogę wyświetlić informacje dotyczące mcp po zakończeniu przechodzenia do Partner Center?

Wybierz **pozycję Kompetencje** w lewym okienku nawigacyjnym na pulpicie nawigacyjnym. Na **stronie Kompetencje** możesz pobrać raport umiejętności. Raport umiejętności będzie zawierał listę użytkowników, którzy zdobyli umiejętności związane z kompetencjami i programami w Partner Center. Jeśli użytkownicy zdobyli umiejętności, ale te umiejętności nie są istotne dla kompetencji, nad które pracujesz, nie zostaną oni wymienione w raporcie.

### <a name="are-customer-references-used-in-partner-center"></a>Czy odwołania klientów są używane w Partner Center?

Nie, nie potrzebujesz odwołań klientów, aby spełnić wymagania dotyczące kompetencji w Partner Center.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Czy skojarzenia partnerów rekordów zostaną Partner Center?

Tak, nie ma żadnych zmian w partnerze rekordów. Dowiedz się więcej na [temat łączenia identyfikatora partnera z klientami.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Czy przejście do Partner Center ma wpływ na zachęty?

Nie, nie ma to wpływu na zachęty, jeśli przeniesiono konto bez konsolidacji lokalizacji. Jeśli Twoja firma ma wiele kont w programie PMC i po przeprowadzce do usługi Partner Center zdecydujesz się na skonsolidowanie konta globalnego, nie będzie żadnych strat dla zachęt, ale może wystąpić opóźnienie w wypłatach zachęt. 

Jeśli nie przeniesiesz wszystkich kont PMC, które były zaangażowane w programy zachęt, możesz zatrzymać zdobywanie zachęt powiązanych z tymi kontami.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Jakie są role zachęt w Partner Center?

Role zachęt w Partner Center są oparte na lokalizacji i obejmują administratora zachęt i użytkownika zachęt. Aby uzyskać więcej informacji na temat tego, co mogą robić te role, zobacz [Przypisywanie ról i uprawnień użytkowników.](permissions-overview.md)

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Czy administratorzy zachęt mogą być przypisani na poziomie globalnym i na poziomie lokalizacji?

Tak. Możesz przypisać administratora zachęt, aby był administratorem zachęt dla wszystkich lokalizacji lub każda lokalizacja może mieć własnego administratora zachęt.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Czy zachęty mogą być opłacane na poziomie globalnym lub na poziomie lokalizacji?

Zachęty są opłacane tylko na poziomie lokalizacji.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Ile profilów biznesowych można utworzyć w odniesieniu do poleceń?

Firma może utworzyć tyle profilów biznesowych, ile jest potrzebnych do pełnego reprezentowania zainteresowań firmy. W każdym profilu biznesowym można wyświetlić listę maksymalnie pięciu lokalizacji, po jednej lokalizacji na kraj. Każdy z profilów biznesowych może odbierać polecenia dla każdej ze swoich lokalizacji.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Jak będą przypisywane polecenia, jakich zmian można oczekiwać? Jeśli na przykład mam globalną firmę na jednym rynku i w jednej lokalizacji na innych rynkach, w jaki sposób będą przypisywane polecenia?

Polecenia są przypisywane na podstawie parametrów wyszukiwania, które definiuje klient. Niezależnie od tego, czy masz jedną, czy wiele lokalizacji, jeśli klient określi żądaną lokalizację i masz tam firmę, która spełnia inne parametry, polecenie zostanie skierowana do tej lokalizacji.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Migruję do Partner Center z Poziomu Rosji. Otrzymuję komunikat o błędzie usługi Web Direct. Jak mogę kontynuować migrację?

Jeśli zostanie wyświetlony komunikat o błędzie z powodu uczestnictwa w programie Web Direct, wykonaj następujące czynności:

1. Zaloguj się do portalu. Azure.com i utwórz nową dzierżawę usługi Azure AD. Aby uzyskać więcej informacji, zobacz Create a new Azure AD tenant (Tworzenie [nowej dzierżawy usługi Azure AD).](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. Po utworzeniu nowej dzierżawy usługi Azure AD użyj jej do migracji z usługi Partner Membership Center do usługi Partner Center lub zarejestrowania się jako nową dzierżawę usługi Partner Center.