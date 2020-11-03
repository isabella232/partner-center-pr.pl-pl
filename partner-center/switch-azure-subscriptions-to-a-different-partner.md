---
title: Przenoszenie subskrypcji platformy Azure do innego partnera
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak zmienić partnera programu Cloud Solution Provider skojarzonego z subskrypcjami platformy Azure klienta.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/29/2020
ms.openlocfilehash: 992dd7f9901efd0176395fb626e4048d5229e82b
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530237"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Dowiedz się, jak przenieść subskrypcje platformy Azure klienta do innego partnera

**Dotyczy**

- Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA
- Centrum partnerskie dla chmury globalnej firmy Microsoft
- Partnerzy w programie dostawcy rozwiązań w chmurze (CSP)

W tym artykule opisano, jak klient może przełączać Microsoft Azure usług z jednego dostawcy rozwiązań w chmurze (CSP) na inny.

Aby przełączyć usługi platformy Azure lub subskrypcje klienta na innego partnera, wykonaj te kroki ręcznie. Zarówno partner, jak i klient muszą wykonać te czynności.

>[!Note]  
>Obecnie tylko dostawcy bezpośredni lub pośredni mogą przenosić subskrypcje.
>Nie można zmienić partnerów dla subskrypcji dostawcy rozwiązań w chmurze skojarzonych z planem Azure, pakietem Office 365, pakietem Enterprise Mobility Suite ani subskrypcjami programu Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Przełączanie partnerów dla subskrypcji platformy Azure

1. Aby przetransferować subskrypcję platformy Azure do nowego partnera, klient musi rozpocząć proces i skontaktować się z jego bieżącym partnerem.

   >[!Note]
   > Jest to odpowiedzialność bieżącego partnera o utworzenie biletu usługi, który inicjuje proces transferu. Firma Microsoft nie może interweniować w imieniu klienta lub nowego partnera. Klient powinien zaplanować ścisłą pracę z bieżącym partnerem, aby zapewnić płynność przejścia.

2. Partner subskrypcji musi wykonać następujące zadania:

   Utwórz bilet usługi platformy Azure z Centrum partnerskiego, aby zażądać przeniesienia subskrypcji:

   1. W menu Centrum partnerskiego wybierz pozycję **klienci** , wybierz z listy pozycję Klient, a następnie wybierz pozycję **Zarządzanie usługami** . 

   2. W sekcji **bilety pomocy technicznej** wybierz listę rozwijaną **nowy bilet** i wybierz pozycję **Microsoft Azure** .
   
   3. W [Azure Portal](https://portal.azure.com)wybierz pozycję **nowe żądanie obsługi** .
   
   4. W kroku 1 Wybierz pozycję **Zarządzanie subskrypcją** jako typ problemu, określ identyfikator subskrypcji, który chcesz przenieść, a następnie wybierz pozycję **dostawca rozwiązań w chmurze** jako plan pomocy technicznej.
   
   5. W kroku 2 Wybierz pozycję **C-minimalny wpływ** i wybierz **inne pytania ogólne** jako typ problemu.
   
   6. Pobierz [formularz transferu subskrypcji dostawcy usług kryptograficznych](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

3. Partner subskrypcji: Wypełnij [formularz transfer subskrypcji dostawcy usług kryptograficznych](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA), podpisz, a następnie wyślij go do klienta. 

   Aby wypełnić formularz, potrzebne są następujące informacje:

   - Informacje kontaktowe bieżącego partnera i identyfikator firmy Microsoft. W menu Centrum partnerskiego wybierz pozycję **Ustawienia konta** &gt; **profil organizacji** , a następnie użyj **identyfikatora Microsoft** , **nazwy organizacji** i **adresu** znajdującego się w tym miejscu.

   - Identyfikator firmy Microsoft dla klienta. W menu Centrum partnerskiego wybierz pozycję **klienci** , a następnie rozwiń listę klientów, aby zobaczyć ich **Identyfikator Microsoft** .

   - Identyfikator subskrypcji do przeniesienia. W rozwiniętej liście klientów wybierz pozycję **Wyświetl subskrypcje** , a następnie rozwiń wybraną subskrypcję, aby wyświetlić **Identyfikator subskrypcji** .

   >[!Note]
   >Transfer subskrypcji powoduje użycie dwóch identyfikatorów subskrypcji, które będą widoczne na stronie **Edytuj subskrypcję** przesłanej subskrypcji: **1** — Identyfikator subskrypcji Centrum partnerskiego jest używany na potrzeby rozliczeń. **2** — oryginalny identyfikator subskrypcji platformy Azure jest zachowywany i będzie widoczny w centrum partnerskim, a także w portalu zarządzania Azure. Ten identyfikator pojawi się w pliku rekonesans.  **Podczas rejestrowania biletów pomocy technicznej należy używać obu identyfikatorów.**

4. Klient i nowy partner dla subskrypcji:

   Przejrzyj formularz, Wypełnij informacje o nowym partnerze i podpisz go. Potwierdź, że nowy klient ma umowę umowną na miejscu. Wyślij formularz z powrotem do bieżącego partnera rekordu.

   *Ważne* : Jeśli nowy partner CSP nie ma relacji odsprzedawcy z klientem, musi ustanowić ten element przed przekazaniem subskrypcji. [Informacje o tym, jak to zrobić](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Nowy partner CSP i dzierżawca klienta muszą znajdować się w tym samym kraju. 

5. Bieżący Partner:

   Upewnij się, że formularz zawiera informacje kontaktowe dla obu administratorów partnerskich. Pomoc techniczna firmy Microsoft skontaktować się z obydwoma administratorami w celu zweryfikowania transferu. Upewnij się, że masz wszystkie trzy podpisy. Następnie użyj opcji **przekazywania plików** , aby dołączyć ukończony formularz do istniejącego żądania usługi. Specjalista pomocy technicznej firmy Microsoft powróci do Ciebie w ciągu ośmiu godzin roboczych w celu zweryfikowania odbioru i zakończenia.

6. Nowy partner:

   Zaktualizuj ustawienia subskrypcji platformy Azure, aby usunąć starego partnera z konta. Aby sprawdzić, które przypisania ról są obsługiwane, Uruchom dwa polecenia cmdlet programu PowerShell.

   - Dodaj nowego partnera jako odsprzedawcę na koncie:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > **Identyfikator dzierżawy** klienta jest wyświetlany w centrum partnerskim jako **Identyfikator firmy Microsoft** dla klienta. Aby znaleźć identyfikator Microsoft (identyfikator dzierżawy) dla określonego klienta, zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego. Następnie wybierz pozycję **klienci** z menu. Znajdź klienta na liście. Wybierz strzałkę w dół, aby rozwinąć listę klientów. Zobaczysz informacje o *nazwie domeny* klienta i **identyfikatorze firmy Microsoft** dla klienta. Użyj 16-cyfrowego **identyfikatora firmy Microsoft** w programie PowerShell polecenia cmdlet.

   - Wyświetlanie ról na koncie, w tym poprzednich partnerów programu CSP:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Usuń nieaktualne uprawnienia dostępu

   - W menu Centrum partnerskiego wybierz pozycję **Customers** .
   - Znajdź klienta na liście. Wybierz (kliknij dwukrotnie) nazwę swojej firmy. Spowoduje to otwarcie strony **subskrypcje** klientów.
   - W menu Szczegóły klienta wybierz pozycję **Zarządzanie usługami** .
   - W obszarze **Microsoft Azure** kliknij link, aby przejść do **Portal zarządzania Microsoft Azure** .

## <a name="next-steps"></a>Następne kroki

- Pobierz [formularz transferu subskrypcji dostawcy usług kryptograficznych](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Dowiedz się więcej o [pomocy technicznej dla partnerów](multipartner.md).

- [Obsługa wielopartnerskich](multipartner.md).
- [Obsługa wielokanałowa](multichannel.md).
- [Przenoszenie subskrypcji platformy Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)