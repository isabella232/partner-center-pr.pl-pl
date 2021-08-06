---
title: Przenoszenie subskrypcji platformy Azure do innego partnera
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Dowiedz się, jak Dostawca rozwiązań w chmurze partnera programu skojarzonego z subskrypcjami platformy Azure klienta.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: cac2d1443fd47f45a70729bf034e65f33861e73698633938ae196e274f4a382b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681386"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Dowiedz się, jak przenieść subskrypcje platformy Azure klienta do innego partnera

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny

W tym artykule opisano, jak klient może przełączyć swoje usługi Microsoft Azure z jednego Dostawca rozwiązań w chmurze (CSP) na inny po zakupie poprzedniej oferty platformy Azure w programie CSP.

Po fazie 1 zmian wprowadzonych w poprzedniej ofercie platformy Azure w programie [CSP](https://go.microsoft.com/fwlink/p/?linkid=2164140)dla wszystkich istniejących relacji odsprzedawcy między partnerami i klientami w programie CSP partner może kontynuować transakcję poprzedniej oferty platformy Azure (MS-AZR-0145p), jeśli klient już ją kupił. W przypadku wszystkich istniejących relacji odsprzedawcy między partnerami i klientami, jeśli klient nie zakupił wcześniej poprzedniej oferty platformy Azure, partner może tylko transakcyjnie korzystać z nowej oferty platformy Azure.

- Jeśli bieżący i przyszły partner mają aktywne poprzednie subskrypcje ofert platformy **Azure** z klientem, poprzednie oferty platformy Azure (MS-AZR-0145p) opisane w tym dokumencie między bieżącym i przyszłym partnerem będą nadal dostępne po fazie 1, o ile obydwaj partnerzy zachowają aktywne poprzednie subskrypcje ofert platformy Azure. Ta możliwość przeniesienia zakończy się, gdy przyszły partner nie ma już aktywnych poprzednich subskrypcji ofert platformy Azure lub gdy poprzednia oferta platformy Azure (MS-AZR-0145p) w programie CSP zostanie trwale wycofana w fazie 3.

   > [!NOTE]
   > W tym scenariuszu nie ma dostępnych zautomatyzowanych narzędzi i należy skorzystać z poniższego procesu.

- Jeśli tylko bieżący partner ma klienta z aktywną poprzednią subskrypcją platformy **Azure (MS-AZR-0145p), a** przyszły partner jej nie ma, przeniesienie poprzedniej oferty platformy Azure między partnerami nie będzie już możliwe po fazie 1. Ponieważ przyszły partner nie może utworzyć poprzedniej subskrypcji oferty platformy Azure (MS-AZR-0145p) dla klienta, ten transfer nie zostanie włączony. W takim przypadku to narzędzie przejściowe może służyć do przenoszenia subskrypcji platformy Azure klienta między partnerami w programie CSP, jednocześnie konwertując ją na nową subskrypcję oferty platformy Azure.

Aby przełączyć usługi lub subskrypcje platformy Azure klienta na innego partnera z poprzednią ofertą platformy Azure (MS-AZR-0145p), wykonaj następujące kroki ręczne. Zarówno partner, jak i klient muszą wykonać te kroki.

> [!NOTE]  
> Obecnie tylko bezpośredni lub pośredni dostawcy mogą przenosić subskrypcje.
> Nie można zmienić partnerów dla subskrypcji Dostawca rozwiązań w chmurze platformy Azure skojarzonych z planem platformy Azure, Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM subskrypcjami.

## <a name="transfer-azure-subscriptions-to-another-partner-with-the-previous-azure-offer"></a>Przenoszenie subskrypcji platformy Azure do innego partnera z poprzednią ofertą platformy Azure

1. Aby przenieść subskrypcję platformy Azure do nowego partnera z poprzednią ofertą platformy Azure, klient musi rozpocząć proces i skontaktować się ze swoim bieżącym partnerem rekordu w formie zapisu.

   > [!NOTE]
   > Bieżący partner odpowiada za utworzenie biletu usługi, który inicjuje proces transferu. Firma Microsoft nie może interweniować w imieniu klienta lub nowego partnera. Klient powinien zaplanować ścisłą współpracę z bieżącym partnerem, aby przejście przebiegało bezproblemowo.

2. Partner subskrypcji musi wykonać następujące zadania:

   Utwórz bilet usługi platformy Azure z Partner Center, aby zażądać przeniesienia subskrypcji:

   1. Z Partner Center wybierz pozycję **Klienci,** wybierz klienta z listy, a następnie wybierz pozycję **Zarządzanie usługami.**
   2. W sekcji **Bilety pomocy technicznej** wybierz menu rozwijane **Nowy** bilet, a następnie wybierz **pozycję Microsoft Azure**.
   3. Na stronie [Azure Portal](https://portal.azure.com)pozycję **Nowy wniosek o pomoc techniczną.**
   4. W kroku 1  wybierz pozycję **Zarządzanie** subskrypcjami jako typ problemu, określ identyfikator subskrypcji, którą chcesz przenieść, a następnie wybierz Dostawca rozwiązań w chmurze jako plan pomocy technicznej.
   5. W kroku 2 wybierz **pozycję C-Minimalny wpływ** i wybierz typ problemu Inne pytania ogólne. 
   6. Pobierz formularz [przeniesienia subskrypcji CSP.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. Partner subskrypcji: wypełnij formularz Przeniesienia subskrypcji programu [CSP,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)podpisz go, a następnie wyślij do klienta. 

   Do ukończenia formularza potrzebne są następujące informacje:

   - Informacje kontaktowe bieżącego partnera i identyfikator Microsoft ID. W menu Partner Center wybierz pozycję **Ustawienia** konta Profil organizacji, a następnie użyj wymienionych w nich pozycji &gt; Identyfikator **firmy Microsoft,** Nazwa organizacji **i** Adres.
   - Identyfikator Microsoft klienta. W menu Partner Center wybierz pozycję **Klienci,** a następnie rozwiń listę klientów, aby wyświetlić jego **identyfikator Microsoft.**
   - Identyfikator subskrypcji do przeniesienia. Na rozwiniętej liście klientów wybierz pozycję **Wyświetl subskrypcje,** a następnie rozwiń wybraną subskrypcję, aby wyświetlić **identyfikator subskrypcji**.

   > [!NOTE]
   > Przeniesienie subskrypcji powoduje, że zostaną wyświetlony dwa identyfikatory subskrypcji na stronie Edytowanie subskrypcji przeniesionej subskrypcji: **1**— identyfikator subskrypcji usługi Partner Center jest używany na potrzeby rozliczeń.  **2**— Oryginalny identyfikator subskrypcji platformy Azure jest zachowywany i będzie wyświetlany w Partner Center, a także w portalu zarządzania azure. Ten identyfikator pojawi się w pliku rekonescji.  **Podczas rejestrowania biletów pomocy technicznej należy użyć obu identyfikatorów.**

4. Klient i nowy partner subskrypcji:

   Przejrzyj formularz, wypełnij informacje o nowym partnerze i podpisz go. Upewnij się, że nowy klient ma podpisaną umowę. Wyślij formularz z powrotem do bieżącego partnera rekordów.

   *Ważne:* Jeśli nowy partner CSP nie ma relacji odsprzedawcy z klientem, musi ustanowić go przed przeniesieniem subskrypcji. [Informacje na temat tego, jak to zrobić, można znaleźć tutaj.](request-a-relationship-with-a-customer.md)

   > [!NOTE]
   > Nowy partner CSP i dzierżawa klienta muszą znajdować się w tym samym kraju. 

5. Bieżący partner:

   Upewnij się, że formularz zawiera informacje kontaktowe dla obu administratorów partnerów. Pomoc techniczna Microsoft obu administratorów w celu zweryfikowania przeniesienia. Upewnij się, że masz wszystkie trzy podpisy. Następnie użyj opcji **Upload,** aby dołączyć wypełniony formularz do istniejącego żądania obsługi. Inżynier pomocy technicznej firmy Microsoft wróci do Ciebie w ciągu ośmiu godzin pracy, aby zweryfikować potwierdzenie i ukończenie.

6. Nowy partner:

   Zaktualizuj ustawienia subskrypcji platformy Azure, aby usunąć starego partnera z konta. Aby zobaczyć, które przypisania ról są aprowowane, uruchom dwa polecenia polecenia programu PowerShell.

   - Dodaj nowego partnera jako odsprzedawcę na koncie:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     > [!NOTE]
     > Identyfikator dzierżawy **klienta jest wyświetlany** w Partner Center jako identyfikator microsoft **klienta**. Aby znaleźć identyfikator Microsoft (identyfikator dzierżawy) dla określonego klienta, zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard) Następnie wybierz **pozycję Klienci** z menu. Znajdź klienta na liście. Wybierz strzałkę w dół, aby rozwinąć ofertę klienta. Zobaczysz informacje o nazwie domeny klienta *i* identyfikatorze **microsoft klienta**. Użyj 16-cyfrowego identyfikatora **Microsoft ID w** poleceniu polecenia programu PowerShell.

   - Wyświetlanie ról na koncie, w tym poprzednich partnerów CSP:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Usuń nieaktualne uprawnienia dostępu:

   1. W menu Partner Center wybierz pozycję **Klienci.**
   1. Znajdź klienta na liście. Wybierz (kliknij dwukrotnie) nazwę firmy. Ta akcja spowoduje otwarcie **strony Subskrypcje** klienta.
   1. W menu szczegółów klienta wybierz pozycję **Zarządzanie usługami.**
   1. W **Microsoft Azure** wybierz link **Microsoft Azure portal zarządzania** link.

## <a name="next-steps"></a>Następne kroki

- [Przenoszenie subskrypcji platformy Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Przenoszenie subskrypcji platformy Azure w ramach planu platformy Azure](transfer-azure-subscriptions-under-azure-plan.md)
- Pobieranie formularza [przeniesienia subskrypcji CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Dowiedz się więcej [o pomocy technicznej dla wielu partnerów](multipartner.md)
- Dowiedz się więcej [na temat obsługi wielu kanałów](multichannel.md)
