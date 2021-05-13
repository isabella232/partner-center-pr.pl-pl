---
title: Ustawianie budżetu wydatków na platformę Azure dla klientów
ms.topic: how-to
ms.date: 03/17/2021
description: Dowiedz się, jak ustawiać lub usuwać miesięczne budżety wydatków na platformę Azure dla klientów, a także jak wyświetlać dane wydatków na platformie Azure i ustawiać powiadomienia dotyczące budżetu.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855356"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Ustawianie, sprawdzanie lub usuwanie miesięcznych budżetów wydatków na platformę Azure dla klientów w Partner Center

**Odpowiednie role:** Agent administracyjny

Możesz ustawić [miesięczny budżet wydatków na platformę Azure dla klientów w](#set-azure-spending-budget) Partner Center. Ułatwia to klientom zarządzanie wydatkami na platformę Azure. Ta opcja umożliwia porównanie wydatków klientów na platformę Azure z budżetem w ciągu miesiąca. Ułatwia to również klientom budżetowanie wydatków na platformę Azure, dzięki czemu ich miesięczne rachunki nie są wyższe niż przewidujesz.

> [!NOTE]  
> Ta funkcja nie jest dostępna w piaskownicy ani na kontach Test w środowisku produkcyjnym (TIP).

Po [skonfigurowaniu budżetu wydatków na platformę Azure](#set-azure-spending-budget)dla klientów możesz również przejrzeć użycie klientów w następujący sposób. Te opcje mogą pomóc w wykrywaniu błędnie skonfigurowanych usług lub nietypowych trendów, które mogą sugerować oszustwo. Następnie możesz współpracować z klientami, aby zidentyfikować główną przyczynę i zarządzać kosztami. W razie potrzeby można również zmienić budżet klienta [na](#set-azure-spending-budget) wyższą kwotę.

- [Sprawdzanie bieżących wydatków na platformę Azure](#check-current-azure-spending)

- [Włącz powiadomienia e-mail, gdy wydatki klienta zbliża się do limitu budżetu](#notifications-for-budget-limits)

- [Wyświetlanie kosztów pozycji według usługi dla subskrypcji opartych na użyciu](#itemized-costs-by-service)

W dowolnym momencie [możesz również usunąć budżet](#remove-azure-spending-budget) wydatków na platformę Azure dla klientów.

## <a name="azure-spending-data"></a>Dane wydatków na platformę Azure

Dane wydatków na platformę Azure są *szacowane,* a *rzeczywiste kwoty rozliczeń mogą się różnić.* Wartość danych nie odzwierciedla *podatków,* środków, korekt ani innych opłat, które mogą być naliczane.

Dane wydatków są *odświeżane raz dziennie.* Klienci mogą nadal korzystać z usług i zasobów platformy Azure (za które są naliczane opłaty), chyba że zmienisz ustawienia konta w Azure Portal.

## <a name="set-azure-spending-budget"></a>Ustawianie budżetu wydatków na platformę Azure

Możesz ustawić *miesięczny budżet wydatków na platformę Azure dla* wielu klientów w Partner Center:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Wydatki na platformę Azure.**

3. Na stronie **wydatków na** platformę Azure w obszarze **Klienci Microsoft Azure subskrypcjami** wybierz klientów, dla których chcesz ustawić budżet.

4. Wprowadź wartość dla budżetu **miesięcznego.**

5. Wybierz **pozycję Zastosuj,** aby zapisać zmiany.

Możesz również *ustawić budżet dla pojedynczego klienta w* ustawieniach subskrypcji:

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Klienci**.

3. Na **stronie Klienci** wybierz nazwę firmy **klienta**.

4. Na stronie Subskrypcje klienta w **obszarze** Subskrypcja oparta **na użyciu** wybierz pozycję **Zmień budżet.**

5. Wprowadź wartość budżetu.

6. Wybierz **pozycję Zastosuj,** aby zapisać zmiany.

## <a name="remove-azure-spending-budget"></a>Usuwanie budżetu wydatków na platformę Azure

Możesz usunąć *miesięczny budżet wydatków na* platformę Azure dla klientów w Partner Center:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Wydatki na platformę Azure.**

3. Na stronie **wydatków na** platformę Azure w obszarze **Klienci Microsoft Azure subskrypcjami** wybierz klientów, których budżet chcesz usunąć.

4. Wybierz **pozycję Usuń budżet.**

## <a name="check-current-azure-spending"></a>Sprawdzanie bieżących wydatków na platformę Azure

Bieżące wydatki *na platformę Azure* i budżety miesięczne klientów można śledzić w dowolnym momencie:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Wydatki na platformę Azure.**

3. Na stronie **wydatków na** platformę Azure w obszarze Klienci z subskrypcjami **Microsoft Azure** można zobaczyć omówienie miesięcznych budżetów klientów, bieżących szacunkowych wydatków i procentowego użytego budżetu.

## <a name="notifications-for-budget-limits"></a>Powiadomienia dotyczące limitów budżetu

Możesz *włączyć powiadomienia e-mail,* gdy miesięczne wydatki klienta zbliżają się do limitu budżetu. Po włączeniu tej opcji będziesz powiadamiany, gdy klienci będą korzystać z co najmniej 80% miesięcznego budżetu. Ta opcja pomaga śledzić rachunek za korzystanie z platformy Azure. Aby skonfigurować powiadomienia e-mail:

1. Zaloguj się do Centrum partnerskiego.

2. Przejdź do obszaru **Settings** (Ustawienia).

3. Wybierz **pozycję Moje preferencje.**

4. Skonfiguruj preferowany adres e-mail, jeśli nie został jeszcze skonfigurowany.

5. Skonfiguruj preferowany język powiadomienia.

6. Wybierz **kartę CSP** w **sekcji Preferencje** powiadomień.

7. Zaznacz opcję Email (Adres e-mail) dla **powiadomienia Azure Spending (Wydatki na** platformę Azure) i save **(Zapisz).**


## <a name="itemized-costs-by-service"></a>Koszty z elementami według usługi

Możesz wyświetlić *koszty z pozycjami (i szacowane użycie) według usługi dla subskrypcji opartych na użyciu:*

1. Zaloguj się do Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **Klienci.**

3. Na stronie **Klienci** wybierz nazwę firmy **klienta**.

4. Na stronie **Subskrypcje klienta** w obszarze **Subskrypcje** oparte na użyciu wybierz nazwę **subskrypcji**.

5. Na stronie subskrypcji możesz przejrzeć  koszty ujmowane według usługi i Szacowane użycie **dla** bieżącego miesiąca.


## <a name="next-steps"></a>Następne kroki

- [Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure](azure-plan-billing.md)
