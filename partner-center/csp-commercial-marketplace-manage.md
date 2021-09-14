---
title: Zarządzanie produktami na platformie handlowej & ofert
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Korzystając Partner Center, dowiedz się, jak dostawcy rozwiązań w chmurze mogą zarządzać ofertami dostawców oprogramowania innych firm zakupionymi dla klientów na platformie handlowej.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14901b47b7363b2d87861be43a7071d9f23545cc
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247227"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Zarządzanie produktami i ofertami na platformie handlowej dla klientów


**Odpowiednie role:** Administrator globalny | Agent administracyjny

Partnerzy w programie Dostawca rozwiązań w chmurze (CSP) mogą za pomocą portalu Partner Center zakupić wiele ofert lub subskrypcji SaaS isv SaaS dla swoich klientów na platformie handlowej. Po zakupie oferty masz różne sposoby zarządzania jej.

## <a name="view-or-edit-a-subscription"></a>Wyświetlanie lub edytowanie subskrypcji

Po zakupie subskrypcji od zewnętrznego wydawcy isv publisher możesz przejrzeć lub edytować ją w następujący sposób:

1. Zaloguj się do Partner Center [nawigacyjnego,](https://partner.microsoft.com/dashboard)a następnie wybierz **pozycję Klienci** z menu nawigacji po lewej stronie.

2. Wybierz odpowiedniego klienta, a następnie wybierz **pozycję Subskrypcje.** Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.

3. W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz wyświetlić lub edytować. Dzięki temu możesz uzyskać więcej informacji na temat skonfigurowania lub aprowizować ofertę. (Jeśli w ofercie jest potrzebnych więcej akcji, w kolumnie Stan może być również wyświetlany stan "Potrzebna akcja". Może temu również towarzyszyć link do witryny wydawcy ISV).

4. Po wybraniu subskrypcji, którą chcesz wyświetlić lub edytować, na stronie szczegółów subskrypcji możesz edytować subskrypcję i wykonać takie czynności jak:

    - Zmienianie pseudonimu subskrypcji

    - Dodawanie/zmniejszanie liczby licencji w subskrypcji

    - Anulowanie subskrypcji

    - Wyłącz automatyczne odnawianie

    - Dodaj identyfikator MPN odsprzedawcy pośredniego, jeśli ma to zastosowanie

> [!NOTE]
> Może być konieczne wykonanie pewnych kroków zdefiniowanych przez wydawcę isv przed wykonaniem pewnych zmian w subskrypcji, takich jak anulowanie subskrypcji.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Przypisywanie licencji i aktywowanie subskrypcji w imieniu klienta

W przypadku zakupu oferty oprogramowania jako usługi (SaaS) dostarczonej przez wydawcę niezależnego dostawcy oprogramowania na platformie handlowej wydawca isv pomaga zarządzać procesem przypisywania licencji i aktywowania subskrypcji w imieniu klienta.

Wydawca powinien dostarczyć spersonalizowany link i kod autoryzacji, który identyfikuje określony zakup.

1. Możesz znaleźć ten spersonalizowany link od wydawcy isv na kilka sposobów:

   - Link jest widoczny na stronie potwierdzenia, która jest wyświetlana po zakupie oferty SaaS dostawcy oprogramowania isv. Aby znaleźć ten link na stronie, poszukaj i wybierz **pozycję Przejdź do witryny wydawcy.**

   - Link jest wyświetlony na stronie Subskrypcje określonego klienta. Ten link wydawcy jest wyświetlany w wierszu skojarzonym z ofertą lub subskrypcją zakupioną dla klienta przez isvv.

   - Link możesz [pobrać przy użyciu interfejsów API Partner Center .](/partner-center/develop/get-activation-link-by-order-line-item)

   > [!NOTE]
   > Aby to zrobić w imieniu klienta, może być konieczne skopiowanie spersonalizowanego linku, wklejenie go w prywatnej przeglądarce i wprowadzenie poświadczeń klienta.

2. Po dojściu do witryny lub systemu wydawcy ISV wydawca będzie wiedzieć o wszelkich dodatkowych krokach, które należy wykonać, aby ukończyć proces konfiguracji klienta i aprowizować lub przypisywać licencje.

3. Jako partner w programie CSP pracującym w imieniu klienta ponosisz odpowiedzialność za wykonywanie następujących zadań:

    - Prześlij wszelkie wymagane informacje do wydawcy.

    - Wyślij dowolny wymagany adres URL bezpośrednio do klienta (lub w inny sposób bezpośrednio przekaż szczegóły dotyczące tej subskrypcji do klienta)

4. Po podaniem wymaganych informacji wydawca aprowizuje i przypisuje odpowiednie licencje. Rozliczanie subskrypcji rozpocznie się dopiero po wystąpienia następujących zdarzeń:

    - Wydawca isv pomyślnie przypisał odpowiednie licencje

    - Wydawca ISV potwierdza firmie Microsoft (za pośrednictwem oddzielnego interfejsu API realizacji SaaS), że konfiguracja konta została pomyślnie ukończona

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Anulowanie subskrypcji SaaS opartej na licencji od wydawcy isv publisher

W przypadku subskrybowania opartego na licencji produktu SaaS oferowanego przez wydawcę ISV na platformie handlowej można anulować subskrypcję w wyznaczonym okresie anulowania. Ten okres anulowania zmienia się w zależności od tego, czy masz subskrypcję miesięczną, czy roczną. Możesz również wybrać, czy subskrypcja ma być odnawiana automatycznie.

Aby uzyskać więcej informacji na temat okresów anulowania, które mają zastosowanie, sposobu anulowania lub automatycznego odnawiania subskrypcji, zobacz [Anulowanie subskrypcji](create-a-new-subscription.md#cancel-a-subscription).

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Dodawanie lub usuwanie licencji dla subskrypcji SaaS

W przypadku ofert platformy handlowej SaaS można dodawać lub usuwać licencje użytkowników dla subskrypcji klienta.

1. Zaloguj się do Partner Center [nawigacyjnego,](https://partner.microsoft.com/dashboard)a następnie wybierz **pozycję Klienci** z menu nawigacji po lewej stronie.

2. Wybierz odpowiedniego klienta, a następnie wybierz **pozycję Subskrypcje.** Zawiera listę wszystkich subskrypcji opartych na licencjach zakupionych dla klienta.

3. W kolumnie **Subskrypcja** wybierz subskrypcję, którą chcesz zmodyfikować.

4. Na stronie szczegółów subskrypcji znajdź **pole Quantity (Ilość).** W tym miejscu można zwiększyć lub zmniejszyć liczbę licencji.

5. Zmień ilość, a następnie wybierz pozycję **Prześlij**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Zarządzanie subskrypcjami przy użyciu Partner Center API

Za pomocą interfejsów API Partner Center do zarządzania cyklem życia i zarządzania fakturami dla subskrypcji. Aby uzyskać więcej informacji, [zobacz Tworzenie subskrypcji dla produktów platformy handlowej](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Następne kroki

- [Kupowanie ofert komercyjnej platformy handlowej](csp-commercial-marketplace-purchase.md)
- [Dowiedz się więcej o rozliczeniach na platformie handlowej](csp-commercial-marketplace-billing.md)
