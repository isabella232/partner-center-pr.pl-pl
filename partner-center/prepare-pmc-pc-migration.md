---
title: Przeniesienie z Centrum członkostwa w partnerze
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zapoznaj się z przydatnymi informacjami i często zadawanymi pytaniami przed przeniesieniem firmy z Centrum partnerskiego do usługi Partner Center.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: be4250864bd07e555b0eb2079c28f3dfb4920805
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529873"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Przygotuj się do przeniesienia z Centrum członkostwa partnera (PMC) do Centrum partnerskiego

**Odpowiednie role**
- Administrator globalny
- Administrator użytkowników
- Agent sprzedaży
- Agent administracyjny

Przenosimy zarządzanie członkostwem z Centrum członkostwa partnerów (PMC) do Centrum partnerskiego — pojedyncze miejsce docelowe do zarządzania relacją biznesową z firmą Microsoft. Chcemy, aby przeniesienie do Centrum partnerskiego było jak najbardziej wydajne i łatwe. Zidentyfikowano niektóre obszary, w których centrum partnerskie różni się od PMC i dlatego należy je zrozumieć i przygotować przed rozpoczęciem przenoszenia.

## <a name="account-and-identity-setup"></a>Konfiguracja konta i tożsamości

Poniżej znajdują się odpowiedzi na często zadawane pytania dotyczące konfiguracji konta i tożsamości.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Co to jest konto służbowe Azure Active Directory (Azure AD)?

Konto służbowe platformy Azure to dedykowana i izolowana wirtualna reprezentacja firmy w chmurze publicznej platformy Azure, która została utworzona w przypadku subskrybowania usługi w chmurze firmy Microsoft, takiej jak Azure, Microsoft Intune lub Office 365.

Twoje konto służbowe obsługuje użytkowników usługi Azure AD i informacje o nich — ich adresy e-mail, hasła, dane profilu, uprawnienia i tak dalej. Konto służbowe zawiera również grupy, aplikacje i inne informacje odnoszące się do firmy i jej zabezpieczeń. 

Służbowy adres e-mail jest częścią dzierżawy usługi Azure Active Directory. Aby móc mieć konto w centrum partnerskim, musisz mieć dzierżawę usługi AAD. Aby uzyskać więcej informacji na Azure Active Directory, przeczytaj artykuł [Tworzenie katalogu w usłudze Azure AD](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

W centrum partnerskim będziesz używać służbowego adresu e-mail, aby zalogować się do konta, a nie do osobistej poczty e-mail.

- Twoje konto służbowe: john@contoso.com
- Twoje konto osobiste: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Co należy zalogować się do Centrum partnerskiego, jeśli masz dzierżawę usługi AAD z firmą Microsoft (na przykład dla pakietu Office 365) i masz dzierżawę dla firmy CSP?

Możesz zalogować się do Centrum partnerskiego przy użyciu konta dostawcy CSP lub konta e-mail MPN Work. Jeśli zdecydujesz się na zalogowanie się przy użyciu służbowego adresu e-mail, po lewej stronie pulpitu nawigacyjnego zostaną wyświetlone informacje o programie MPN i programu CSP. Jeśli zalogujesz się przy użyciu służbowego adresu e-mail MPN usługi Azure AD, zobaczysz tylko informacje o programie MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Jeśli nie chcesz używać istniejącej dzierżawy usługi Azure AD w usłudze Office 365 dla Centrum partnerskiego, możesz utworzyć nową dzierżawę przed migracją z PMC.

Może być wiele powodów, dla których nie chcesz używać istniejącej dzierżawy usługi Azure AD w celu skonfigurowania konta Centrum partnerskiego. Przed rozpoczęciem migracji do Centrum partnerskiego przejdź do [Azure Portal](https://ms.portal.azure.com/#home) , aby utworzyć nową dzierżawę usługi Azure AD. Postępuj zgodnie ze wskazówkami w temacie [Tworzenie nowej dzierżawy w Azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Aby skonfigurować konto Centrum partnerskiego, użyj nowej dzierżawy usługi AAD. Musisz być administratorem globalnym, aby utworzyć dzierżawę. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Role użytkowników, w tym role użytkowników gościa w centrum partnerskim

Centrum partnerskie ma różne typy ról w zależności od typów pracy wymaganej do wykonania. Istnieją takie role, jak Administratorzy globalni, którzy są rolami usługi Azure AD. Niektóre role są specyficzne dla programów, takich jak program dostawcy usług w chmurze czy zachęty, a istnieją role, które są specyficzne dla MPN. Aby dowiedzieć się, jakie są wszystkie role Centrum partnerskiego, przeczytaj temat [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md).

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Co się stanie z rolami użytkowników, gdy przechodzą z PMC do Centrum partnerskiego?

Z wyjątkiem sytuacji, w której administrator globalny MPN lub kontakt z programem podstawowym przeprowadzi migrację, wszyscy użytkownicy w PMC przestaną swoje role administratora. Osoba, która ukończy proces migracji, będzie musiała przypisać role w centrum partnerskim. Role w centrum partnerskim różnią się od ról w obszarze PMC. Przeczytaj [Przypisywanie ról i uprawnień użytkowników] (uprawnienia-overview.md i [przechodzenie z programu PMC do Centrum partnerskiego](move-pmc-pc-map.md#user-roles) , aby uzyskać więcej informacji na temat ról użytkowników w centrum partnerskim.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Jaka jest różnica między profilem firmy a moim profilem biznesowym?

Profil firmy to informacje o firmie, które obejmują adres, lokalizacje, podstawowe informacje kontaktowe, Bank i podatek.

Twój profil biznesowy zawiera informacje o sposobie prezentowania klientów i jest stroną marketingową, w której wyświetlane jest logo, szczegóły dotyczące Twojego zainteresowania firmy, wiedzę fachową itp.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Co oznacza konsolidację kont dla mojego konta?

Jeśli używasz tej samej dzierżawy usługi Azure AD do migracji wielu kont MPN do Centrum partnerskiego, system automatycznie wykryje to i poprosił o skonsolidowanie kont. Jest to prawdziwe, nawet jeśli istnieje wiele domen skojarzonych z tą samą dzierżawą usługi Azure AD. 

Można nadal zdecydować się na migrację do Centrum partnerskiego przy użyciu osobnych dzierżawców usługi AAD, ale zwróć uwagę na to, że wykorzystasz wydzieloną ocenę swoich kompetencji i dodatkowych kosztów zakupu. Aby uzyskać więcej informacji na temat konsolidacji kont, przeczytaj artykuł [konsolidowanie kont firmowych](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Jeśli mam wiele dzierżawców usługi AAD i jedno konto MPN, czy można je połączyć w centrum partnerskim?

Tak, w centrum partnerskim można połączyć wiele dzierżawców usługi Azure AD z jednym kontem Centrum partnerskiego.
Aby uzyskać więcej informacji na temat konsolidacji kont, przeczytaj artykuł [konsolidowanie kont firmowych](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Czy istnieją ograniczenia dotyczące dodawania wielu dzierżawców usługi Azure AD do jednego konta Centrum partnerskiego?

Jeśli dzierżawa usługi Azure AD jest już skojarzona z istniejącym kontem Centrum partnerskiego, nie można jej skojarzyć z nowymi kontami Centrum partnerskiego przy użyciu funkcji wielodostępności. Innym sposobem na to sądzimy, że dzierżawa usługi Azure AD może być skojarzona tylko z jednym kontem Centrum partnerskiego, ale z kontem Centrum partnerskiego może być skojarzonych wiele dzierżawców.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migracja członkostwa w Microsoft Partner Network (MPN) 

Poniżej znajdują się odpowiedzi na często zadawane pytania dotyczące migracji członkostwa MPN.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Kto może przeprowadzić przeniesienie z PMC do Centrum partnerskiego?

Administrator globalny MPN firmy lub kontakt z programem głównym (te dwie role są często przechowywane przez tę samą osobę) mogą inicjować i przełączać.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Czy osoba, która przeprowadzi migrację, stanie się główną osobą kontaktową w ramach firmowego profilu w centrum partnerskim?

Niemniej jednak główny kontakt musi być osobą, która ma autoryzację do podpisywania umów.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Czy firma Microsoft może migrować moje członkowstwa MPN?

Nie. Firma Microsoft nie może pomóc w przenoszeniu konta członkostwa do Centrum partnerskiego. Musisz przenieść konto, logując się do niego przy użyciu konta służbowego (poświadczenia logowania), aby rozpocząć proces migracji. Po wykonaniu kroków związanych z przenoszeniem konta możesz rozpocząć zarządzanie członkostwem oraz przypisać role i uprawnienia użytkowników do zespołu, aby mogli uzyskać dostęp do korzyści i zarządzać członkostwem. 

Firma Microsoft automatycznie przeprowadzi migrację bieżących kompetencji, korzyści, informacji o lokalizacji, informacji o banku/podatkach dla zachęt i MCPych, w tym z dostępem z uczelnią partnerów.

### <a name="how-will-the-renewal-policy-change"></a>Jak zmienią się zasady odnawiania?

W centrum partnerskim okno odnowienia przypada od daty rocznicy do 30 dni.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Czy nasze kompetencje pozostaną bez zmian po przejściu do Centrum partnerskiego?

Tak, nie wpłynie to na kompetencje przenoszone do Centrum partnerskiego. Jeśli zauważysz rozbieżności, skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/support).

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Czy moje korzyści (w tym korzyści z chmury, pomoc techniczna, korzyści z oprogramowania, program Visual Studio) zmieniły się po przeniesieniu?

Kwalifikujące się korzyści nie zmienią się. Jeśli zauważysz rozbieżności, skontaktuj się z [pomocą techniczną](https://partner.microsoft.com/support).

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Czy nasze konta Microsoft z pakietami korzyści dla programu Visual Studio będą honorowane?

Tak. Korzyści wynikające z programu Visual Studio przydzielono do kont MSA i zachowywane. Zostaną one również zachowane po odnowieniu w centrum partnerskim. Jeśli jednak usuniesz alokację MSA po migracji w centrum partnerskim, nie będzie można jej dodać z powrotem do Centrum partnerskiego.

W centrum partnerskim partner może dodawać konta służbowe i konta użytkowników-Gości, które są kontem MSA z tej samej dzierżawy, w której partner jest MPN administratorem w dzierżawie usługi Azure AD. Jeśli partner jest administratorem globalnym w wielu dzierżawach usługi Azure AD, a wszystkie te dzierżawy są skojarzone z tym samym kontem Centrum partnerskiego, partner może dodawać użytkowników we wszystkich dzierżawach do korzyści z programu Visual Studio i alokacji opartych na platformie Azure.

Użytkownicy-Goście mogą mieć przypisane subskrypcje programu Visual Studio oparte na użyciu przez administratora MPN lub administratora globalnego, ale użytkownicy-Goście nie mogą zalogować się do Centrum partnerskiego za pomocą swojego konta MSA. Użytkownicy-Goście mogą jednak zalogować się do platformy Azure i programu Visual Studio, aby sprawdzić poprawność i korzystać z przypisanych im korzyści.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Jak mamy zarządzać naszymi MCPmi i naszym partnerem z University partner?

Brak zmian w skojarzeniach MCP, które przechodzą z PMC. Jednak wszyscy nowi pracownicy po przejściu do Centrum partnerskiego będą musieli zostać powiązani w centrum partnerskim. Wszystkie Twoje uprawnienia University do partnerów dla istniejących użytkowników będą nadal dostępne, ale wszyscy nowi pracownicy powinni przejść do [centrum szkoleniowego,](https://partner.microsoft.com/training) Aby uzyskać informacje na temat sposobu uzyskania dostępu do uczelni partnerskiej.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Jak mogę wyświetlić informacje MCP po przeniesieniu do Centrum partnerskiego?

Wybierz pozycję **kompetencje** z lewej strony na pulpicie nawigacyjnym. Na stronie **kompetencje** można pobrać raport umiejętności. Raport umiejętności zawiera listę użytkowników, którzy uzyskali odpowiednie umiejętności dotyczące kompetencji i programów w centrum partnerskim. Jeśli użytkownicy uzyskali umiejętności, ale te umiejętności nie mają znaczenia dla kompetencji, do których prowadzisz pracę, nie będą wyświetlane w raporcie.

### <a name="are-customer-references-used-in-partner-center"></a>Czy odwołania klientów są używane w centrum partnerskim?

Nie, nie potrzebujesz odwołań klienta, aby spełnić wymagania dotyczące kompetencji w centrum partnerskim.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Czy partner rekordów zostanie przeniesiony do Centrum partnerskiego?

Tak, nie można zmienić partnera rekordu. Dowiedz się więcej [na temat łączenia Twojego identyfikatora partnera z klientami](/azure/billing/billing-partner-admin-link-started).

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Czy ma to wpływ na zachęty ze względu na przechodzenie do Centrum partnerskiego?

Nie, nie ma wpływu na zachęty, jeśli Twoje konto zostało przeniesione bez konsolidacji lokalizacji. Jeśli firma ma wiele kont w kryterium PMC i, po przejściu do Centrum partnerskiego zdecydujesz się na konsolidację na konto globalne, nastąpi utrata zachęty, ale może wystąpić opóźnienie wypłaty. 

Jeśli nie przeniesiesz wszystkich kont PMC, które zostały uwzględnione w programach zachęty, możesz zrezygnować z bodźców, które są powiązane z tymi kontami.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Jakie są role zachęt w centrum partnerskim?

Role zachęt w centrum partnerskim są oparte na lokalizacji i obejmują użytkowników, którzy są administratorami i bodźcami. Aby uzyskać więcej informacji na temat tych ról, zobacz [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Czy można zachęcić administratorów do przypisywania na poziomie globalnym i lokalizacji?

Tak. Administrator zachęty można przypisać administratorom zachęty dla wszystkich lokalizacji lub w każdej lokalizacji.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Czy zachęty mogą być płatne na poziomie globalnym czy w lokalizacji?

Zachęty są wypłacane tylko na poziomie lokalizacji.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Jakie są informacje dotyczące odwołań, jak wiele profilów firmy można utworzyć?

Firma może utworzyć dowolną liczbę profilów firmowych, aby w pełni przedstawić interesy firmy. W każdym profilu biznesowym można wyświetlić maksymalnie pięć lokalizacji, jedną lokalizację na kraj. Każdy profil biznesowy może odbierać odwołania dla każdej z jej lokalizacji.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Jak będą przypisywane odwołania, jakie zmiany mogą oczekiwać? Na przykład jeśli mam firmę globalną na jednym rynku i lokalizacji na innych rynkach, w jaki sposób będą przypisywane odwołania?

Odwołania są przypisywane na podstawie parametrów wyszukiwania, które definiuje klient. Bez względu na to, czy masz jedną lokalizację, czy wiele, jeśli klienci określają pożądaną lokalizację i masz już firmę, która spełnia inne parametry, wówczas odwołanie przejdzie do tej lokalizacji.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Migrujem do Centrum partnerskiego z poziomu Rosji. Otrzymuję komunikat o błędzie dotyczący bezpośredniej sieci Web. Jak mogę kontynuować migrację?

Jeśli zostanie wyświetlony komunikat o błędzie, ponieważ bierzesz udział w programie Internet Direct, wykonaj następujące czynności:

1. Zaloguj się do portalu. Azure.com i Utwórz nową dzierżawę usługi Azure AD. Aby uzyskać więcej informacji [, zobacz Tworzenie nowej dzierżawy usługi Azure AD](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant).

2. Po utworzeniu nowej dzierżawy usługi Azure AD Użyj jej do przeprowadzenia migracji z Centrum partnerskiego partnera do Centrum partnerskiego lub zarejestrowania się w usłudze net New w centrum partnerskim.