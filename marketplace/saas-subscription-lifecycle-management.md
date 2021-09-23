---
title: Zarządzanie cyklem życia subskrypcji oprogramowania jako usługi (SaaS)
description: Zarządzanie cyklem życia subskrypcji oprogramowania jako usługi (SaaS) w Azure Marketplace.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 08/20/2021
ms.author: yonits
author: yonits
ms.openlocfilehash: c5f06fb88a29def9df8d8cc2936f9eea91d8b2b4
ms.sourcegitcommit: eeb81ccb888239a0e8fbe4711de3ce07f3b00358
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/23/2021
ms.locfileid: "128312181"
---
# <a name="saas-subscription-lifecycle-management"></a>Zarządzanie cyklem życia subskrypcji SaaS

W tym artykule opisano sposób odnajdywania zasobu SaaS, różnice między modelami SaaS i SaaS Classic oraz zarządzanie zasobami SaaS w Azure Portal.

## <a name="find-a-saas-resource"></a>Znajdowanie zasobu SaaS

Gdy kupujesz ofertę SaaS od firmy Azure Marketplace, tworzy ona subskrypcję oprogramowania jako usługi (SaaS) w usłudze Azure Portal (aby uzyskać szczegółowe informacje, zobacz Kupowanie oferty SaaS w [usłudze Azure Portal).](purchase-saas-offer-in-azure-portal.md) Aby znaleźć zasób SaaS w portalu:

- **Okno wyszukiwania globalnego** (u góry) — wyszukaj subskrypcję SaaS według nazwy.
- **SaaS** — wyświetla listę wszystkich subskrypcji SaaS. Istnieją dwa typy list SaaS: Zobacz następującą sekcję.
- **Subskrypcje** — wyświetla listę wszystkich subskrypcji platformy Azure, do których masz dostęp w ramach dzierżawy. Aby znaleźć określoną subskrypcję, użyj okna filtru lub wyszukiwania.
- **Wszystkie zasoby** — wyświetla listę wszystkich zasobów utworzonych w ramach wszystkich subskrypcji, do których masz dostęp. Aby znaleźć określoną subskrypcję, użyj filtru (wpisz > SaaS) lub wyszukaj na liście.

## <a name="differences-between-saas-and-saas-classic-lists-of-resources-in-the-azure-portal"></a>Różnice między listami zasobów SaaS i SaaS Classic w Azure Portal

Różnica między tymi dwoma typami polega na tym, że model SaaS Classic umożliwia znalezienie subskrypcji SaaS, które zostały utworzone w ramach dzierżawy, a nie w grupie zasobów.
Jeśli subskrypcja SaaS została zakupiona w 2021 Azure Portal lutym 2021 r., została ona utworzona w ramach dzierżawy i można ją znaleźć w obszarze SaaS Classic. Wszystkie zakupy dokonane w Microsoft AppSource znajdują się na tej liście.

Jeśli przed lutym 2021 r. zakupiono subskrypcję SaaS w ramach usługi Azure Portal i chcesz przenieść ją z dzierżawy do grupy zasobów (zalecane), przejdź do subskrypcji SaaS w sekcji **SaaS Classic** i wybierz pozycję Przenieś do **grupy zasobów.** Subskrypcje można przenosić tylko w stanie **Oczekiwanie** **lub** Aktywne. Po przeniesioniu subskrypcja SaaS jest teraz wyświetlana w widoku **SaaS,** a nie **w modelu SaaS Classic.** Nie można przenieść subskrypcji SaaS do grupy zasobów, jeśli została zakupiona w usłudze AppSource.

To przeniesienie oferuje następujące korzyści:

- Ulepszony dostęp do zasobu SaaS i kontrola nad nim za pomocą dziedziczonych zasad i uprawnień z subskrypcji platformy Azure i grup zasobów (pełna kontrola RBAC)
- Cykl życia usługi SaaS jest powiązany z cyklem życia subskrypcji platformy Azure dla akcji, takich jak przenoszenie i usuwanie
- Łatwiejsze odnajdywanie dzięki zasobom SaaS znalezionym przy użyciu wyszukiwanie globalne
- Korzystanie z Azure Cost Management — monitorowanie wydatków na zasoby SaaS
- Zasoby na poziomie subskrypcji mają zdarzenia zasobów w dzienniku aktywności

## <a name="manage-your-saas-service"></a>Zarządzanie usługą SaaS

Istnieje wiele sposobów zarządzania subskrypcjami SaaS

* W przypadku subskrypcji SaaS zakupionych w Azure Portal zarządzaj nimi w tym miejscu.
* W przypadku subskrypcji SaaS zakupionych w usłudze AppSource zarządzaj nimi w Azure Portal i [centrum Administracja Microsoft 365 usługi](https://admin.microsoft.com/Adminportal/Home?#/subscriptions); Aby uzyskać szczegółowe informacje na temat korzystania z centrum Administracja Microsoft 365, zobacz [Manage third-party app subscriptions for your organization](/microsoft-365/commerce/manage-saas-apps?view=o365-worldwide&preserve-view=true)(Zarządzanie subskrypcjami aplikacji innych firm w organizacji).
* Niektórzy wydawcy umożliwiają zarządzanie subskrypcjami SaaS bezpośrednio na ich platformie. Odwiedź witrynę wydawcy, korzystając z linku na stronie subskrypcji SaaS w Azure Portal.

Istnieje kilka akcji, które można podjąć po zakupie. Niektóre będą wymagać uprawnień właściciela lub współautora:

### <a name="change-plans"></a>Plany zmian

Zmiany wprowadzone w subskrybowanych planach zostaną natychmiast wprowadzone. Rozliczenia będą proporcjonalnie do okresu rozliczeniowego bieżącego planu. Zmiana planów wymaga **uprawnień właściciela** **lub współautora.**

> [!NOTE]
> Wydawca może odmówić zatwierdzenia zmiany, jeśli wybrane zmiany nie są możliwe w ramach usługi. W takim przypadku zmiana nie powiedzie się.

W niektórych przypadkach plan **zmiany może** nie działać:

- Jeśli Twoja subskrypcja jest na poziomie dzierżawy z **uprawnieniami Do** odczytu, nie możesz zmienić planu. W takim przypadku zażądaj uprawnień od osoby, która ma **rolę właściciela** w subskrypcji.
- Jeśli z subskrypcją platformy Azure nie jest skojarzony instrument płatniczy, nie można zmienić planu bezpłatnego na plan płatny. Możesz jednak wybrać inną subskrypcję platformy Azure, a następnie wybrać plan płatny lub dodać pi do wybranej subskrypcji platformy Azure.
- Jeśli wybrany plan ma ograniczenie minimalne/maksymalne liczby użytkowników, które nie obejmuje bieżącej liczby użytkowników, wybierz inny plan z taką samą liczbą użytkowników uwzględnioną w oryginalnym planie, który został zakupiony, lub skontaktuj się z wydawcą.
- Jeśli wydawca nie może zrealizować żądania, skontaktuj się z nim bezpośrednio.

### <a name="change-number-of-users"></a>Zmienianie liczby użytkowników

W przypadku planów opartych na miejscu można dodać lub zmniejszyć liczbę użytkowników zdefiniowanych podczas procesu zakupu. Zmiana liczby subskrybowanych użytkowników rozpocznie się natychmiast, a opłaty będą proporcjonalnie do okresu rozliczeniowego bieżącego planu. Zmiany stanowisk są możliwe tylko w zakresie minimalnej i maksymalnej liczby stanowisk, zgodnie z definicją wydawcy. W niektórych przypadkach trzeba będzie zmienić plan przed zmianą stanowisk i na odwrót.

- Jeśli Twoja subskrypcja znajduje się na poziomie dzierżawy z uprawnieniami do odczytu, nie możesz zmienić liczby użytkowników. Zamiast tego należy zażądać uprawnień współautora od osoby, która ma rolę właściciela w subskrypcji.
- Jeśli wydawca nie może zrealizować żądania, skontaktuj się z nim bezpośrednio.

> [!NOTE]
> Wydawca może odmówić zatwierdzenia zmiany, jeśli nie jest to możliwe w ramach usługi. W takim przypadku zmiana nie powiedzie się.

### <a name="edit-recurring-billing"></a>Edytowanie rozliczeń cyklicznych

Rozliczenia cykliczne umożliwiają zarządzanie odnawianiem subskrypcji SaaS. Gdy rozliczenia cykliczne są wyłączone, subskrypcja i usługa SaaS zakończą się w dniu odnowienia. Opcję odnowienia można zmienić tylko wtedy, gdy subskrypcja jest aktywna. Nie można ponownie aktywować zakończonej i/lub anulowaowej subskrypcji SaaS; W jego miejscu należy utworzyć nową subskrypcję SaaS.

### <a name="view-billing"></a>Wyświetlanie rozliczeń

Wyświetlanie faktur dla subskrypcji platformy Azure i Azure Marketplace zakupionych w ramach tej subskrypcji. W przypadku usługi SaaS zakupionej w portalu zapoznaj się ze  stroną rozliczeń na stronie subskrypcji SaaS w sekcji Rozliczenia, która przekieruje Cię do **Cost Management**.

Cost Management pomaga zrozumieć podział faktur, zarządzać kontem rozliczeniowym i subskrypcjami, monitorować/kontrolować wydatki na platformę Azure i optymalizować użycie zasobów. Umożliwia ona analizowanie kosztów, tworzenie budżetów i zarządzanie nimi i nie tylko. Na przykład umożliwia śledzenie użycia miernika niestandardowego (w przypadku subskrypcji SaaS utworzonych po lutym 2021 r. lub przeniesionych do grupy zasobów). Więcej informacji na temat zarządzania kosztami można znaleźć [Azure Cost Management + Billing dokumentacji.](/azure/cost-management-billing/)

Jeśli zakup został dokonany za pośrednictwem Microsoft AppSource, możesz wyświetlić faktury w Centrum administracyjnym firmy Microsoft w obszarze **& płatności.**

### <a name="cancel-subscription"></a>Anulowanie subskrypcji

Anulowanie powoduje usunięcie twojego dostępu do oprogramowania zakupionego w ramach tej subskrypcji SaaS. Zwroty są przetwarzane zgodnie z zasadami zwrotów; Aby uzyskać szczegółowe informacje, zobacz [Zasady zwrotów Microsoft AppSource i Azure Marketplace](refund-policies.md).

Jeśli Twoja subskrypcja jest na poziomie dzierżawy z **uprawnieniami do** odczytu, nie możesz anulować subskrypcji. Zamiast tego skontaktuj się z osobą z **uprawnieniami właściciela.**

Jeśli masz miesięczną subskrypcję SaaS przez ponad 24 godziny lub roczną lub wieloroczną subskrypcję przez ponad 14 dni, żaden zwrot nie będzie używany dla bieżącego okresu subskrypcji (zobacz zasady anulowania). Rozliczenia oparte na zużyciu po skonfigurowaniu konta SaaS również nie kwalifikują się do zwrotu.

### <a name="delete-subscription"></a>Usuwanie subskrypcji

Ta akcja jest jak anulowanie, z dodatku do usunięcia zasobu SaaS z listy subskrypcji SaaS. Po usunięciu subskrypcji nie będzie można uzyskać do jej dostępu z Azure Portal.

Jeśli Twoja subskrypcja jest na poziomie dzierżawy z **uprawnieniami do** odczytu, nie możesz usunąć subskrypcji. Zamiast tego skontaktuj się z osobą z **uprawnieniami właściciela.**

### <a name="change-azure-subscription-andor-resource-group"></a>Zmienianie subskrypcji platformy Azure i/lub grupy zasobów

Aby zmienić subskrypcję/grupę zasobów skojarzoną z ofertą kupioną w Azure Portal:

1. Przejdź do **sekcji SaaS.**
2. Wybierz subskrypcję do zmiany.
3. W **obszarze Rozliczenia** wybierz pozycję Zmień **rozliczaną subskrypcję.**
4. Wybierz żądaną subskrypcję/grupę zasobów lub utwórz nową grupę zasobów, do których chcesz przenieść zasób SaaS.
5. Wybierz **pozycję Zmień** u dołu, aby ukończyć proces.

W niektórych przypadkach zmiana może nie działać:

- Jeśli Subskrypcja SaaS nie jest w stanie Subskrybowanie, sprawdź stan subskrypcji w sekcji SaaS lub na stronie subskrypcji **SaaS.**
- Jeśli subskrypcja SaaS jest zasobem na poziomie dzierżawy:
    - Musisz mieć uprawnienia *właściciel/współautor w* docelowej subskrypcji platformy Azure.
- Jeśli subskrypcja SaaS jest zasobem na poziomie subskrypcji:
    - Do docelowej *subskrypcji* platformy Azure potrzebne są uprawnienia Odczyt lub *Właściciel/Współautor.*
    - Potrzebujesz uprawnień *właściciela/współautora* dla docelowej grupy zasobów.
    - Jeśli subskrypcja SaaS o tej samej nazwie już istnieje w docelowej grupie zasobów, wybierz inną docelową grupę zasobów.
- Docelowa subskrypcja platformy Azure i subskrypcja zasobów zostaną poddane wszystkim testom wykonywanym podczas zakupu. Aby dowiedzieć się więcej na temat kontroli zakupu, zobacz sekcję Subskrypcja i konfiguracja [SaaS](purchase-saas-offer-in-azure-portal.md#saas-subscription-and-configuration) w te **Azure Portal**.

## <a name="next-steps"></a>Następne kroki

- Jeśli już zakupiono ofertę na platformie handlowej, przejdź do [tematu Rozliczenia i fakturowanie](billing-invoicing.md)
- Dowiedz się więcej o [opcjach planu prywatnego](./private-plans.md)