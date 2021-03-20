---
title: Ustawianie budżetu wydatków na platformę Azure dla klientów
ms.topic: how-to
ms.date: 03/17/2021
description: Dowiedz się, jak ustawiać lub usuwać miesięczne budżety wydatków platformy Azure dla klientów, a także wyświetlać dane wydatków platformy Azure i ustawiać powiadomienia związane z budżetem.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712753"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Ustaw, sprawdzaj lub usuwaj miesięczne budżety wydatków platformy Azure dla klientów w centrum partnerskim

**Odpowiednie role**

- Agent administracyjny

Możesz [ustawić miesięczny budżet wydatków platformy Azure dla klientów](#set-azure-spending-budget) w centrum partnerskim. Dzięki temu klienci mogą zarządzać wydatkami na platformę Azure. Ta opcja umożliwia porównanie wydatków platformy Azure dla klientów z budżetem w danym miesiącu. Ułatwia ona również klientom budżetowanie wydatków na platformę Azure, dzięki czemu miesięczne rozliczenie nie jest wyższe niż przewidywane.

> [!NOTE]  
> Ta funkcja jest niedostępna w piaskownicy lub testowaniu na kontach w środowisku produkcyjnym.

Po [ustawieniu budżetu wydatków na platformę Azure dla swoich klientów](#set-azure-spending-budget)można również przejrzeć użycie klienta w następujący sposób. Te opcje mogą pomóc w określeniu błędnie skonfigurowanych usług lub nietypowych trendów, które mogą sugerować oszustwo. Następnie możesz współpracować z klientami, aby identyfikować główną przyczynę i zarządzać kosztami. W razie potrzeby można także [zmienić budżet klienta](#set-azure-spending-budget) na wyższą kwotę.

- [Sprawdź bieżące wydatki na platformę Azure](#check-current-azure-spending)

- [Włącz powiadomienia e-mail, gdy wydatki klienta zbliżają się do limitu budżetu](#notifications-for-budget-limits)

- [Wyświetlanie wyszczególnionych kosztów według usługi dla subskrypcji opartych na użyciu](#itemized-costs-by-service)

W dowolnym momencie możesz również [usunąć budżet wydatków platformy Azure](#remove-azure-spending-budget) dla klientów.

## <a name="azure-spending-data"></a>Dane wydatków platformy Azure

Dane wydatków platformy Azure to *oszacowanie* , a *rzeczywiste kwoty rozliczeń mogą się różnić*. Wartość danych *nie odzwierciedla* podatków, kredytów, korekt lub innych opłat, które mogą być stosowane.

Dane wydatków są *odświeżane raz* dziennie. Klienci mogą nadal korzystać z usług i zasobów platformy Azure (i być obciążani nimi), chyba że zmienisz ustawienia konta w Azure Portal.

## <a name="set-azure-spending-budget"></a>Ustaw budżet wydatków na platformę Azure

Możesz *ustawić miesięczny budżet wydatków platformy Azure* dla wielu klientów w centrum partnerskim:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **wydatki na platformę Azure**.

3. Na stronie **wydatków platformy Azure** w obszarze **klienci z subskrypcjami Microsoft Azure** wybierz klientów, dla których chcesz ustawić budżet.

4. Wprowadź wartość dla **miesięcznego budżetu**.

5. Wybierz pozycję **Zastosuj** , aby zapisać zmiany.

Możesz również *ustawić budżet dla pojedynczego klienta* w ustawieniach subskrypcji:

1. Zaloguj się do pulpitu nawigacyjnego Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **klienci**.

3. Na stronie **klienci** wybierz **nazwę firmy** klienta.

4. Na stronie **subskrypcje** klienta w obszarze **subskrypcja oparta na użyciu** wybierz pozycję **Zmień budżet**.

5. Wprowadź wartość budżetu.

6. Wybierz pozycję **Zastosuj** , aby zapisać zmiany.

## <a name="remove-azure-spending-budget"></a>Usuń budżet wydatków platformy Azure

Możesz *usunąć miesięczny budżet wydatków platformy Azure* dla klientów w centrum partnerskim:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **wydatki na platformę Azure**.

3. Na stronie **wydatków platformy Azure** w obszarze **klienci z subskrypcjami Microsoft Azure** wybierz klientów, których budżet chcesz usunąć.

4. Wybierz pozycję **Usuń budżet**.

## <a name="check-current-azure-spending"></a>Sprawdź bieżące wydatki na platformę Azure

W dowolnym momencie możesz *śledzić bieżące wydatki na korzystanie z platformy Azure i budżety miesięczne klientów* :

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **wydatki na platformę Azure**.

3. Na stronie **wydatków na platformę Azure** w obszarze **klienci z subskrypcjami Microsoft Azure** można zobaczyć przegląd budżetów miesięcznych klientów, bieżące oszacowania wydatków i procent użycia budżetu.

## <a name="notifications-for-budget-limits"></a>Powiadomienia dotyczące limitów budżetu

*Powiadomienia e-mail można włączyć* , gdy miesięczne wydatki klienta zbliżają się do limitu budżetu. Po włączeniu tej opcji użytkownik zostanie powiadomiony, że klienci będą korzystać z co najmniej 80% czasu miesięcznego budżetu. Ta opcja pomaga zachować oczami na rachunku na korzystanie z platformy Azure. Aby skonfigurować powiadomienia e-mail:

1. Zaloguj się do Centrum partnerskiego.

2. Przejdź do obszaru **Settings** (Ustawienia).

3. Wybierz pozycję **moje preferencje**.

4. Jeśli nie, skonfiguruj preferowany adres e-mail.

5. Skonfiguruj preferowany język dla powiadomienia.

6. Wybierz kartę **dostawca CSP** w sekcji **Preferencje powiadomień** .

7. Zaznacz opcję Poczta E-mail dla powiadomienia **wydatków platformy Azure** i **Zapisz**.


## <a name="itemized-costs-by-service"></a>Wyszczególnione koszty według usługi

Można *wyświetlić wyszczególnione koszty (i szacowane użycie) według usługi dla subskrypcji opartych na użyciu*:

1. Zaloguj się do Centrum partnerskiego.

2. W menu po lewej stronie w obszarze **CSP** wybierz pozycję **klienci**.

3. Na stronie **klienci** wybierz **nazwę firmy** klienta.

4. Na stronie **subskrypcje** klienta w obszarze **subskrypcje na podstawie użycia** wybierz nazwę **subskrypcji**.

5. Na stronie subskrypcja można przejrzeć **koszty wyszczególnione** według usługi i **szacowane użycie** w bieżącym miesiącu.


## <a name="next-steps"></a>Następne kroki

- [Nowe środowisko handlowe w programie CSP — rozliczenia platformy Azure](azure-plan-billing.md)
