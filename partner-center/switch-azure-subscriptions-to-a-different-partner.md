---
title: Przenoszenie subskrypcji platformy Azure do innego partnera
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak Dostawca rozwiązań w chmurze partner programu skojarzonego z subskrypcjami platformy Azure klienta.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: 28e90ec4a699e2d8830f3695a30151e6b00e8cd1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248129"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-without-converting-them-to-an-azure-plan"></a>Przenoszenie subskrypcji platformy Azure klienta do innego partnera bez konwertowania ich na plan platformy Azure

**Dotyczy:** Partner Center | Partner Center dla Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny

W tym artykule opisano, jak klient może przenieść subskrypcję platformy Azure ze swojego bieżącego Dostawca rozwiązań w chmurze (CSP) do innego CSP.

W pierwszej sekcji, Przenoszenie subskrypcji platformy [Azure](#transferring-azure-subscriptions-to-another-partner)do innego partnera, opisano, jak klient może przenieść subskrypcję Microsoft Azure z jednego Dostawca rozwiązań w chmurze (CSP) do innego.

W następnej sekcji [Transfering a previous Azure offer subscription without converting it to the Azure plan](#transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan)(Przenoszenie poprzedniej subskrypcji oferty platformy Azure bez konwertowania jej na plan platformy Azure) krótko opisano sposób wprowadzania nowego planu platformy Azure. Następnie opisano specjalny przypadek, w którym niektóre subskrypcje poprzedniej oferty platformy Azure można przenieść do innego programu CSP bez konwertowania ich na nowy plan platformy Azure.

Klient, bieżący dostawca usług i nowy dostawca usług mają obowiązki podczas przenoszenia subskrypcji klienta do nowego dostawcy [usług platformy Azure.](#responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider) Klient powinien zaplanować ścisłą współpracę z bieżącym partnerem, aby przejście przebiegało bezproblemowo.

 Informacje wysokiego poziomu, które ułatwiają subskrybentom platformy Azure przenoszenie subskrypcji do i od partnerów CSP, można znaleźć w te tematu [Transfer Azure subscriptions between subscribers and CSPs](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)(Przenoszenie subskrypcji platformy Azure między subskrybentami i partnerami CSP).

Dodatkowe informacje o tym, jak klienci mogą zmieniać swoje subskrypcje platformy Azure z jednego partnera na innego, można znaleźć w tece [Transfer a customer's Azure subscriptions to a different CSP (under an Azure plan) (Przenoszenie](/partner-center/transfer-azure-subscriptions-under-azure-plan) subskrypcji platformy Azure klienta do innego programu CSP (w ramach planu platformy Azure)

## <a name="prerequisites"></a>Wymagania wstępne

- Partner programu CSP musi mieć relację odsprzedawcy z klientem, aby można było przenieść subskrypcję.  Aby uzyskać więcej informacji, [zobacz How to request a reseller relationship from a customer in Partner Center](/partner-center/request-a-relationship-with-a-customer).
- Partner musi być dostawcą bezpośrednim lub pośrednim, aby przenieść subskrypcję.
- Nie można przenieść subskrypcji skojarzonych z następującymi ofertami: plan platformy Azure, Office 365, Enterprise Mobility Suite i Microsoft Dynamics CRM.
- Aby przenieść subskrypcję, klient musi znajdować się w tym samym kraju co partner.
- Partnerzy działający w Microsoft Cloud for US Government microsoft cloud (Niemcy) muszą zażądać uprawnień do zarządzania usługą lub subskrypcją klienta. Aby uzyskać więcej informacji, zobacz [Uzyskiwanie uprawnień do zarządzania usługą](/partner-center/customers-revoke-admin-privileges)lub subskrypcją klienta.

## <a name="transferring-azure-subscriptions-to-another-partner"></a>Przenoszenie subskrypcji platformy Azure do innego partnera

Przenoszenie subskrypcji platformy Azure z jednego partnera CSP do innego jest wieloetapowym procesem, który wymaga działań klienta, bieżącego partnera i nowego partnera na różnych etapach. W poniższej tabeli przedstawiono diagram sekwencji ułatwiający wyjaśnienie, kto i kiedy robi.

### <a name="responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Obowiązki podczas przenoszenia subskrypcji klienta do nowego dostawcy usług platformy Azure

|Krok  |Customer  |Bieżący partner  |Nowy partner  |
|---------|---------|---------|---------|
|1     |[Klient powiadamia firmę Microsoft i bieżącego partnera na pisanie](#step-1-customer-contacts-current-partner-in-writing)         |         |         |
|2     |         |[Tworzenie biletu pomocy technicznej w celu zażądania przeniesienia](#step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer)        |         |
|3     |         |[Wysyłanie wypełnionego formularza przeniesienia do klienta](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)|         |
|4     |         |[Kompletna zmiana Dostawca rozwiązań w chmurze formularza](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)       |         |
|5     |[Przeglądanie, podpisywanie & formularza powrotu](#step-5-the-customer-and-new-partner-review--return-the-form)       |         |[Przeglądanie, podpisywanie & formularza powrotu](#step-5-the-customer-and-new-partner-review--return-the-form)         |
|6     |         |[Formularz przeglądu i dołączanie do żądania obsługi](#step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request)        |         |
|7     |         |         |[Usuwanie starego partnera z konta](#step-7-new-partner-removes-old-partner-from-account)         |
|8     |         |         |[Usuwanie nieaktualnych uprawnień dostępu](#step-8-new-partner-removes-outdated-access-permissions)         |

### <a name="steps-for-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Procedura przenoszenia subskrypcji klienta do nowego dostawcy usług platformy Azure

#### <a name="step-1-customer-contacts-current-partner-in-writing"></a>Krok 1. Klient kontaktuje się na pisanie z bieżącym partnerem

Klient rozpoczyna proces przenoszenia, powiadamiając na pisanie zarówno firmę Microsoft, jak i bieżącego partnera CSP (czyli nie słownie) o żądaniu przeniesienia subskrypcji.

#### <a name="step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer"></a>Krok 2. Bieżący dostawca tworzy bilet pomocy technicznej platformy Azure w celu zażądania przeniesienia

Bieżący partner tworzy bilet pomocy technicznej platformy Azure w celu zażądania przeniesienia subskrypcji.

> [!NOTE]
> Bieżący partner odpowiada za utworzenie biletu pomocy technicznej, który inicjuje proces przenoszenia. Firma Microsoft nie interweniuje w imieniu klienta ani nowego partnera.

**Aby utworzyć bilet pomocy technicznej w celu zażądania przeniesienia:**

1. W menu Partner Center wybierz pozycję **Klienci,** wybierz klienta z listy, a następnie wybierz pozycję **Zarządzanie usługami.**
1. W sekcji **Bilety pomocy technicznej** wybierz pozycję Nowy **bilet,** a następnie wybierz **Microsoft Azure.**
1. W [Azure Portal](https://portal.azure.com/)wybierz pozycję Nowy **wniosek o pomoc techniczną.**
1. W kroku 1 wniosku o  pomoc techniczną wybierz pozycję Zarządzanie subskrypcjami jako typ problemu, określ identyfikator subskrypcji, który chcesz przenieść, a następnie wybierz Dostawca rozwiązań w chmurze jako plan pomocy technicznej. 
1. W kroku 2 wybierz **pozycję C-Minimalny wpływ** i wybierz typ problemu **Inne** pytania ogólne.

#### <a name="step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer"></a>Krok 3. Bieżący partner kończy formularz przeniesienia i wysyła go do klienta

Bieżący partner pobiera i kończy zmianę formularza [Dostawca rozwiązań w chmurze](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), podpisuje go, a następnie wysyła do klienta.

#### <a name="step-4-current-partner-completes-current-partner-fills-in-the-change-of-cloud-solution-provider-form"></a>Krok 4. Bieżący partner wypełnia formularz Zmiana Dostawca rozwiązań w chmurze partnera

Bieżący partner kończy formularz [Zmiany Dostawca rozwiązań w chmurze](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)podpisuje go i wysyła do klienta.

Informacje potrzebne do ukończenia formularza *zmiany Dostawca rozwiązań w chmurze* są:

- **Informacje kontaktowe bieżącego partnera** i identyfikator Microsoft ID (które można znaleźć w menu Partner Center, wybierając pozycję Ustawienia konta **> profilu organizacji).**
- **Identyfikator Microsoft klienta** (który można znaleźć w menu usługi  Partner Center, wybierając pozycję Klienci, a następnie rozwijając listę klientów, aby ujawnić jego identyfikator Microsoft ID).
- Identyfikator **subskrypcji** do przeniesienia (który można znaleźć w menu usługi Partner Center, wybierając pozycję Klienci, a następnie rozwijając listę klientów, wybierając pozycję Wyświetl subskrypcje, a następnie rozwijając wybraną subskrypcję, aby wyświetlić identyfikator subskrypcji.  

#### <a name="step-5-the-customer-and-new-partner-review--return-the-form"></a>Krok 5. Klient i nowy partner & zwrócić formularz

Współpracując z klientem i nowym partnerem:

1. Przejrzyj formularz, wypełnij informacje o nowym partnerze i podpisz go.
1. Upewnij się, że nowy klient ma podpisaną umowę.
1. Wyślij formularz z powrotem do bieżącego partnera.

#### <a name="step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request"></a>Krok 6. Formularz bieżących przeglądów partnerów i dołącza go do żądania obsługi

Gdy bieżący partner otrzyma formularz,:

- Upewnij się, że formularz zawiera informacje kontaktowe dla obu administratorów partnerów. (Pomoc techniczna Microsoft obu administratorów w celu zweryfikowania przeniesienia).
- Sprawdź, czy mają wszystkie trzy podpisy, a następnie użyj opcji **Upload,** aby dołączyć wypełniony formularz do istniejącego żądania obsługi. (Inżynier pomocy technicznej firmy Microsoft kontaktuje się z nimi w ciągu ośmiu godzin w celu zweryfikowania potwierdzenia i ukończenia).

#### <a name="step-7-new-partner-removes-old-partner-from-account"></a>Krok 7. Nowy partner usuwa starego partnera z konta

Nowy partner aktualizuje ustawienia subskrypcji platformy Azure w programie PowerShell, aby usunąć starego partnera z konta.

> [!NOTE]
> Pierwsze polecenie cmdlet programu PowerShell wymaga identyfikatora dzierżawy klienta **,** który jest wyświetlany Partner Center jako identyfikator **Microsoft klienta**. W następującej procedurze opisano, jak znaleźć identyfikator Microsoft klienta (identyfikator dzierżawy) do użycia w poleceniach cmdlet.

Aby znaleźć identyfikator microsoft klienta (identyfikator dzierżawy) do użycia w Połączenie **cmdlet programu PowerShell *Połączenie-AzAccount:***

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)
1. Wybierz **pozycję Klienci** z menu.
1. Znajdź klienta na wyświetlonej liście.
1. Wybierz strzałkę w dół, aby rozwinąć ofertę klienta. Zobaczysz informacje o nazwie domeny  klienta i identyfikatorze **microsoft klienta**.
1. Użyj 16-cyfrowego **identyfikatora Microsoft ID w** poleceniach cmdlet programu PowerShell, które są następujące po tej procedurze.

Pierwsze polecenie cmdlet programu PowerShell dodaje nowego partnera jako odsprzedawcę na koncie:

```powershell
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

Drugie polecenie cmdlet wyświetla role na koncie, w tym poprzednich partnerów CSP:

```powershell
Get-AzRoleAssignment
```

#### <a name="step-8-new-partner-removes-outdated-access-permissions"></a>Krok 8. Nowy partner usuwa nieaktualne uprawnienia dostępu

   **Aby usunąć nieaktualne uprawnienia dostępu:**

   1. W menu Partner Center wybierz pozycję **Klienci.**
   1. Znajdź klienta na liście klientów.
   1. Kliknij dwukrotnie nazwę firmy klienta. Zostanie **wyświetlona strona Subskrypcje** klienta.
   1. W menu szczegółów klienta wybierz pozycję **Zarządzanie usługami.**
   1. W **Microsoft Azure** wybierz pozycję **Microsoft Azure portal zarządzania**.

## <a name="transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan"></a>Przenoszenie poprzedniej subskrypcji oferty platformy Azure bez konwertowania jej na plan platformy Azure

W tej sekcji krótko opisano sposób wprowadzania nowego planu platformy Azure. Następnie opisano specjalny przypadek, w którym niektóre subskrypcje poprzedniej oferty platformy Azure można przenieść do innego programu CSP bez konwertowania ich na nowy plan platformy Azure.

> [!NOTE]
> Aby przenieść subskrypcje platformy Azure klienta zakupione w ramach poprzedniej oferty platformy Azure do nowego programu CSP i przekonwertować je na plan platformy *Azure*( jest to akcja domyślna), zobacz poprzednią sekcję Przenoszenie subskrypcji platformy [*Azure*](#transferring-azure-subscriptions-to-another-partner)do innego partnera i artykuł Przenoszenie subskrypcji platformy Azure klienta do innego programu [*CSP (w*](/partner-center/transfer-azure-subscriptions-under-azure-plan)ramach planu platformy Azure).

### <a name="the-azure-plan-and-the-previous-azure-offer"></a>Plan platformy Azure i poprzednia oferta platformy Azure

Firma Microsoft wprowadziła nowe środowisko handlowe, [plan platformy Azure,](/partner-center/azure-plan-lp)w lipcu 2021 r. Aby dać partnerom czas na dołączanie nowych funkcji do swoich usług i przejście klientów z poprzedniej oferty platformy Azure (MS-AZR-0145p) do planu platformy Azure, poprzednia oferta platformy Azure będzie nadal dostępna przez ograniczony czas.

Przejście z poprzedniej oferty platformy Azure do planu platformy Azure obejmuje trzy fazy:

**Faza 1:** od momentu wprowadzenia planu platformy Azure w lipcu 2021 r. wszyscy nowi klienci programu Azure CSP zostały umieszczeni w planie platformy Azure. Partnerzy mogą nadal korzystać z poprzedniej oferty platformy Azure u klientów, którzy już ją kupili.

**Faza 2:** 1 lutego 2022 r. zachęty i możliwość marży partnera zostaną usunięte z poprzedniej oferty platformy Azure.

**Faza 3:** W chwili, gdy nie zostanie jeszcze określona poprzednia oferta platformy Azure zostanie wycofana, a klienci nadal korzystający z poprzedniej oferty platformy Azure zostaną zmigrowani do planu platformy Azure. (Partnerzy zostaną powiadomieni o dacie wycofania z sześciu miesięcy z wyprzedzeniem).

### <a name="transferring-subscriptions-without-conversion"></a>Przenoszenie subskrypcji bez konwersji

W tej sekcji opisano specjalny przypadek przenoszenia subskrypcji zakupionej w ramach poprzedniej oferty platformy Azure do nowego dostawcy CSP bez konwertowania jej na *plan platformy Azure.*

Subskrypcję klienta dla poprzedniej oferty platformy Azure można przenieść do nowego partnera CSP bez konwersji na plan platformy Azure, korzystając z kroków z poprzedniej sekcji Przenoszenie subskrypcji platformy [Azure](#transferring-azure-subscriptions-to-another-partner)do innego partnera, jeśli:

- Poprzednia oferta platformy Azure jest nadal dostępna.
- Zarówno bieżący partner, jak i nowy partner mają klienta z subskrypcją poprzedniej oferty platformy Azure.

Jeśli tylko bieżący partner ma klienta z subskrypcją poprzedniej oferty platformy Azure, bieżący partner może użyć narzędzia przejścia, aby przenieść subskrypcję klienta do nowego partnera, jednocześnie konwertując ją na nowy plan platformy Azure.

> [!NOTE]
> Tylko partnerzy, którzy mają bezpośrednią relację rozliczeń z firmą Microsoft, mogą uzyskać dostęp do narzędzia przejściowego. Odsprzedawcy pośredni muszą współpracować ze swoimi dostawcami pośrednimi, aby korzystać z narzędzia przejściowego.

## <a name="next-steps"></a>Następne kroki

- [Przenoszenie subskrypcji platformy Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure](transfer-azure-subscriptions-under-azure-plan.md)
- Pobieranie formularza [przeniesienia subskrypcji CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Dowiedz się więcej [o pomocy technicznej dla wielu partnerów](multipartner.md)
- Dowiedz się więcej [na temat obsługi wielu kanałów](multichannel.md)
