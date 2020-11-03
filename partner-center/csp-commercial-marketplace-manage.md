---
title: Zarządzanie produktami z portalu Marketplace & ofertami
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Korzystając z Centrum partnerskiego, Dowiedz się, w jaki sposób dostawcy rozwiązań w chmurze mogą zarządzać dostawcami niezależnych dostawców oprogramowania, które zostały zakupione dla klientów z komercyjnego portalu
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d32f42b2c4bd8e4ec6c659326d1a21385c0642f
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92530003"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Zarządzanie komercyjnymi produktami i ofertami w witrynie Marketplace dla klientów

**Dotyczy**

- Centrum partnerskie
- Partnerzy w programie CSP

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny

Partnerzy w programie Cloud Solution Provider (CSP) mogą używać portalu Centrum partnerskiego do zakupu wielu ofert SaaS oferowanych przez niezależnych dostawców oprogramowania lub subskrypcji dla klientów z komercyjnej witryny Marketplace. Po zakupie oferty masz różne sposoby zarządzania nimi.

## <a name="view-or-edit-a-subscription"></a>Wyświetlanie lub edytowanie subskrypcji

Po zakupieniu subskrypcji od wydawcy niezależnego dostawcy oprogramowania można przejrzeć lub edytować ją w następujący sposób:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego, a następnie wybierz pozycję **klienci** z menu nawigacji po lewej stronie.

2. Wybierz odpowiedniego klienta, a następnie wybierz pozycję **subskrypcje**. Zawiera listę wszystkich subskrypcji opartych na licencji zakupionych dla klienta.

3. W kolumnie **subskrypcja** wybierz subskrypcję, którą chcesz wyświetlić lub edytować. Dzięki temu możesz uzyskać więcej informacji na temat konfigurowania oferty lub jej dostarczania. (Jeśli w ofercie jest wymagana większa akcja, w kolumnie Stan może zostać wyświetlony stan "wymagana akcja"). Może to również towarzyszyć link do witryny wydawcy niezależnego dostawcy oprogramowania.

4. Po wybraniu subskrypcji, którą chcesz wyświetlić lub edytować, Strona szczegółów subskrypcji umożliwia edytowanie subskrypcji i wykonywanie następujących czynności:

    - Zmiana pseudonimu subskrypcji

    - Dodaj/Zmniejsz liczbę licencji w subskrypcji

    - Anuluj subskrypcję

    - Wyłącz automatyczne odnawianie

    - Dodaj pośredni odsprzedawcy identyfikator MPN (jeśli dotyczy)

> [!NOTE]
> Może być konieczne wykonanie pewnych czynności zdefiniowanych przez wydawcę niezależnego dostawcy oprogramowania, aby można było wykonać pewne zmiany w subskrypcji, na przykład anulować subskrypcję.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Przypisywanie licencji i aktywowanie subskrypcji w imieniu klienta

W przypadku zakupienia oferty oprogramowania jako usługi (SaaS) dostarczonej przez wydawcę niezależnego dostawcy oprogramowania w portalu komercyjnym Wydawca programu ISV pomaga zarządzać procesem przypisywania licencji i aktywowania subskrypcji w imieniu klienta.

Wydawca powinien udostępnić spersonalizowany link oraz kod autoryzacji, który identyfikuje określony zakup.

1. Ten spersonalizowany link można znaleźć z poziomu wydawcy niezależnego dostawcy oprogramowania na kilka sposobów:

   - Po zakupieniu oferty SaaS niezależnego dostawcy oprogramowania zobaczysz link na stronie potwierdzenia. Aby znaleźć ten link na stronie, Wyszukaj i wybierz pozycję **Przejdź do witryny wydawcy**.

   - Link można zobaczyć na stronie Subskrypcje określonego klienta. Ten link wydawcy jest wyświetlany w wierszu skojarzonym z ofertą niezależnego dostawcy oprogramowania lub subskrypcją zakupionego dla klienta.

   - Link można [pobrać przy użyciu interfejsów API Centrum partnerskiego](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Aby to zrobić w imieniu klienta, może być konieczne skopiowanie spersonalizowanego linku, wklejenie go do przeglądarki prywatnej, a następnie wprowadzenie poświadczeń klienta.

2. Po nawiązaniu kontaktu z witryną lub systemem wydawcy niezależnego dostawcy oprogramowania będzie wiadomo o wszelkich dodatkowych krokach, które należy wykonać w celu ukończenia procesu instalacji klienta i aprowizacji lub przypisywania licencji.

3. Jako partner programu CSP działającego w imieniu klienta użytkownik jest odpowiedzialny za wykonywanie następujących zadań:

    - Prześlij do wydawcy wszystkie wymagane informacje.

    - Wyślij dowolny wymagany adres URL bezpośrednio do klienta (lub w inny sposób Przekaż szczegółowe informacje o tej subskrypcji klientowi)

4. Po podaniu wymaganych informacji do wydawcy program Publisher zainicjuje obsługę administracyjną i przypisze odpowiednie licencje. Rozliczanie subskrypcji rozpocznie się dopiero po wystąpieniu następujących zdarzeń:

    - Wydawca niezależnego dostawcy oprogramowania pomyślnie przypisał odpowiednie licencje

    - Wydawca niezależnego dostawcy oprogramowania zakończył pracę z firmą Microsoft (za pośrednictwem oddzielnego interfejsu API realizacji SaaS), że Konfiguracja konta została pomyślnie ukończona

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Anulowanie subskrypcji SaaS opartej na licencji od wydawcy niezależnego dostawcy oprogramowania

Gdy subskrybujesz produkt SaaS oparty na licencji oferowany przez wydawcę niezależnego dostawcy oprogramowania, możesz anulować subskrypcję w ramach wyznaczonego okresu anulowania. Ten okres anulowania zmienia się w zależności od tego, czy masz miesięczną, czy roczną subskrypcję. Możesz również wybrać, czy automatycznie odnowić subskrypcję.

Aby uzyskać więcej informacji na temat okresów anulowania, które mają zastosowanie, sposobu anulowania lub autoodnawiania subskrypcji, zobacz:

- [Anulowanie subskrypcji](create-a-new-subscription.md#cancel-a-subscription)

- [Odnawianie komercyjnej subskrypcji portalu Marketplace](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Dodawanie lub usuwanie licencji dla subskrypcji SaaS

W przypadku ofert SaaS komercyjnych Marketplace możesz dodawać lub usuwać licencje użytkowników w ramach subskrypcji klienta.

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard)Centrum partnerskiego, a następnie wybierz pozycję **klienci** z menu nawigacji po lewej stronie.

2. Wybierz odpowiedniego klienta, a następnie wybierz pozycję **subskrypcje**. Zawiera listę wszystkich subskrypcji opartych na licencji zakupionych dla klienta.

3. W kolumnie **subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.

4. Na stronie Szczegóły subskrypcji Znajdź pole **ilość** . Jest to miejsce, w którym można zwiększyć lub zmniejszyć liczbę licencji.

5. Zmień liczbę, a następnie wybierz pozycję **Prześlij**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Zarządzanie subskrypcjami przy użyciu interfejsów API Centrum partnerskiego

Możesz również używać interfejsów API Centrum partnerskiego do zarządzania cyklem życia i zarządzania fakturami dla subskrypcji. Aby uzyskać więcej informacji, zobacz [Tworzenie subskrypcji dla komercyjnych produktów Marketplace](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Następne kroki

- [Kup komercyjne oferty rynkowe](csp-commercial-marketplace-purchase.md)
- [Dowiedz się więcej na temat rozliczeń w portalu komercyjnym](csp-commercial-marketplace-billing.md)