---
title: Przenoszenie subskrypcji platformy Azure do innego partnera
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak Dostawca rozwiązań w chmurze programu partnerskiego skojarzonego z subskrypcjami platformy Azure klienta.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856070"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Dowiedz się, jak przenieść subskrypcje platformy Azure klienta do innego partnera

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny

W tym artykule opisano, jak klient może przełączać swoje usługi Microsoft Azure między Dostawca rozwiązań w chmurze (CSP).

Aby przełączyć usługi lub subskrypcje platformy Azure klienta na innego partnera, wykonaj te kroki ręczne. Zarówno partner, jak i klient muszą wykonać te kroki.

>[!Note]  
>Obecnie tylko bezpośredni lub pośredni dostawcy mogą przenosić subskrypcje.
>Nie można zmieniać partnerów dla subskrypcji Dostawca rozwiązań w chmurze platformy Azure, usługi Office 365, pakietu Enterprise Mobility Suite ani subskrypcji usługi Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Przełączanie partnerów na subskrypcje platformy Azure

1. Aby przenieść subskrypcję platformy Azure do nowego partnera, klient musi rozpocząć proces i skontaktować się ze swoim bieżącym partnerem z rekordem w zapisie.

   >[!Note]
   > Bieżący partner odpowiada za utworzenie biletu usługi, który inicjuje proces transferu. Firma Microsoft nie może interweniować w imieniu klienta lub nowego partnera. Klient powinien zaplanować ścisłą współpracę z bieżącym partnerem, aby przejście przebiegało bezproblemowo.

2. Partner subskrypcji musi wykonać następujące zadania:

   Utwórz bilet usługi platformy Azure z Partner Center, aby zażądać przeniesienia subskrypcji:

   1. Z Partner Center wybierz pozycję **Klienci,** wybierz klienta z listy, a następnie wybierz pozycję **Zarządzanie usługami.**

   2. W sekcji **Bilety pomocy** technicznej wybierz menu **rozwijane Nowy** bilet, a następnie wybierz pozycję **Microsoft Azure**.
   
   3. Na stronie [Azure Portal](https://portal.azure.com)pozycję **Nowy wniosek o pomoc techniczną.**
   
   4. W kroku 1  wybierz pozycję Zarządzanie subskrypcjami jako typ problemu, określ identyfikator subskrypcji, którą chcesz przenieść, a następnie wybierz Dostawca rozwiązań w chmurze **jako** plan pomocy technicznej.
   
   5. W kroku 2 wybierz **pozycję C-Minimalny wpływ** i wybierz typ problemu **Inne** pytania ogólne.
   
   6. Pobierz formularz [przeniesienia subskrypcji CSP.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. Partner subskrypcji: wypełnij formularz Przeniesienia subskrypcji programu [CSP,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)podpisz go, a następnie wyślij do klienta. 

   Do wypełnienia formularza potrzebne są następujące informacje:

   - Informacje kontaktowe bieżącego partnera i identyfikator Microsoft ID. W menu Partner Center wybierz pozycję **Ustawienia** konta Profil organizacji, a następnie użyj podanych w tym menu &gt;  **identyfikatorów,** nazw organizacji **i** adresów. 

   - Identyfikator Microsoft klienta. W Partner Center wybierz pozycję **Klienci,** a następnie rozwiń listę klientów, aby wyświetlić jego **identyfikator Microsoft**.

   - Identyfikator subskrypcji do przeniesienia. Na rozwiniętej liście klientów wybierz pozycję **Wyświetl subskrypcje,** a następnie rozwiń wybraną subskrypcję, aby wyświetlić **identyfikator subskrypcji**.

   >[!Note]
   >Przeniesienie subskrypcji powoduje wyświetlanie dwóch identyfikatorów subskrypcji na  stronie Edytowanie subskrypcji przeniesionej subskrypcji: **1**— identyfikator subskrypcji Partner Center jest używany do celów rozliczeniowych. **2**— Oryginalny identyfikator subskrypcji platformy Azure jest zachowywany i będzie wyświetlany w Partner Center, a także w portalu zarządzania Azure. Ten identyfikator pojawi się w pliku rekonescji.  **Podczas rejestrowania biletów pomocy technicznej należy użyć obu identyfikatorów.**

4. Klient i nowy partner subskrypcji:

   Przejrzyj formularz, wypełnij informacje o nowym partnerze i podpisz go. Upewnij się, że nowy klient ma podpisaną umowę. Wyślij formularz z powrotem do bieżącego partnera rekordu.

   *Ważne:* Jeśli nowy partner CSP nie ma relacji odsprzedawcy z klientem, musi go ustanowić przed przeniesieniem subskrypcji. [Informacje na temat tego, jak to zrobić, można znaleźć tutaj.](request-a-relationship-with-a-customer.md)

   >[!Note]
   >Nowy partner CSP i dzierżawa klienta muszą znajdować się w tym samym kraju. 

5. Bieżący partner:

   Upewnij się, że formularz zawiera informacje kontaktowe dla obu administratorów partnerów. Pomoc techniczna Microsoft obu administratorów w celu zweryfikowania przeniesienia. Upewnij się, że masz wszystkie trzy podpisy. Następnie użyj opcji **Przekazywanie pliku,** aby dołączyć wypełniony formularz do istniejącego żądania obsługi. Inżynier pomocy technicznej firmy Microsoft wróci do Ciebie w ciągu ośmiu godzin pracy, aby zweryfikować potwierdzenie i ukończenie.

6. Nowy partner:

   Zaktualizuj ustawienia subskrypcji platformy Azure, aby usunąć starego partnera z konta. Aby zobaczyć, które przypisania ról są aprowowane, uruchom dwa polecenia polecenia programu PowerShell.

   - Dodaj nowego partnera jako odsprzedawcę na koncie:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > Identyfikator dzierżawy **klienta jest wyświetlany** w Partner Center jako identyfikator microsoft **klienta**. Aby znaleźć identyfikator Microsoft (identyfikator dzierżawy) dla określonego klienta, zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard) Następnie wybierz **pozycję Klienci** z menu. Znajdź klienta na liście. Wybierz strzałkę w dół, aby rozwinąć ofertę klienta. Zobaczysz informacje o nazwie domeny klienta *i* identyfikatorze **microsoft klienta**. Użyj 16-cyfrowego identyfikatora **Microsoft ID w** poleceniu polecenia programu PowerShell.

   - Wyświetlanie ról na koncie, w tym poprzednich partnerów CSP:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Usuń nieaktualne uprawnienia dostępu:

   - W menu Partner Center wybierz pozycję **Klienci.**
   - Znajdź klienta na liście. Wybierz (kliknij dwukrotnie) nazwę firmy. Ta akcja spowoduje otwarcie strony **Subskrypcje** klienta.
   - W menu szczegółów klienta wybierz pozycję **Zarządzanie usługami.**
   - W **Microsoft Azure** wybierz link, aby przejść do Portal zarządzania Microsoft Azure **.**

## <a name="next-steps"></a>Następne kroki

- Pobierz formularz [przeniesienia subskrypcji CSP.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)

- Dowiedz się więcej [o pomocy technicznej dla wielu partnerów.](multipartner.md)

- [obsługa wielu partnerów.](multipartner.md)
- [obsługa wielu kanałów.](multichannel.md)
- [Przenoszenie subskrypcji platformy Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)