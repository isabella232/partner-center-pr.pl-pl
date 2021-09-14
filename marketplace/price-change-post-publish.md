---
title: Zmiany cen produktów w witrynie Marketplace po opublikowaniu
description: W tym artykule opisano typowe pytania dotyczące zmiany cen planów po opublikowaniu.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: bfb99986483d0aaaa5d685c266c8118c1345517c
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247017"
---
# <a name="price-changes-to-marketplace-products"></a>Zmiany cen produktów w witrynie Marketplace

Niezależni dostawcy oprogramowania (ISV) sprzedaje swoje produkty za pośrednictwem Azure Marketplace mogą aktualizować ceny planu (lub jednostki SKU) od czasu do czasu. Nowa cena SKU może być wyższa lub niższa niż poprzednia cena. Zmiana ceny jest aktualizowana na poziomie produktu/SKU/rynku. W związku z tym mogą być dostępne aktualizacje cen, które są istotne dla niektórych rynków, ale nie dla wszystkich.

W niektórych przypadkach (zobacz poniżej) zmiana ceny może mieć wpływ na produkty zakupione w przeszłości, a klient zobaczy zmianę ceny na fakturze miesięcznej. Azure Marketplace powiadomi klientów korzystających z tych produktów co najmniej 90 dni przed zastosowaniem nowej ceny.

## <a name="which-offer-types-can-be-affected-from-price-change"></a>Na jakie typy ofert może mieć wpływ zmiana ceny?

Wszystkie produkty do sprzedaży za pośrednictwem usług Azure Marketplace i AppSource, na przykład produkty, które mają co najmniej jeden plan.

## <a name="can-a-free-sku-turn-one-day-into-a-paid-one"></a>Czy bezpłatna sku może przekształcić jeden dzień w płatną?

Nie. IsV cannot turn a free SKU into a paid SKU(IsV isV cannot turn a free SKU into a paid SKU) (IsV isV cannot turn a free SKU into a paid SKU) An ISV who wants to make a product billable will need to publish a new paid SKU.

## <a name="price-increase-awareness-in-the-marketplace-product-pages"></a>Zwiększanie świadomości cen na stronach produktów w witrynie Marketplace

Jak wspomniano, isvs who want to publish a price increase must give at co najmniej 90 days warning before the new price takes effect. Ma to na celu powiadomienie klientów planujących zakup produktu. Strony produktów w witrynie Marketplace są aktualizowane z wyprzedzeniem co najmniej 90 dni w przypadku nadchodzącej zmiany. Strony są aktualizowane przy użyciu komunikatu ze szczegółami nadchodzącej daty zmiany ceny i nowej stawki

:::image type="content" source="media/price-change/plan-pricing.png" alt-text="Ilustruje stronę cennika planu":::

> [!NOTE]
> Cennik na powyższej ilustracji jest tylko do celów przykładowych. Rzeczywiste ceny mogą się różnić.

Takie powiadomienie będzie wyświetlane tylko wtedy, gdy cena podniesie się, a nie wtedy, gdy cena spada.

## <a name="when-is-the-new-price-taking-effect"></a>Kiedy nowa cena dzieje się owacyjnie?

 Data wejścia w życie nowej ceny będzie zawsze rozpoczynać się od miesiąca kalendarzowego. W okresie powiadomienia z 90-dniowym okresem typowa oś czasu aktualizacji ceny będzie wyglądać tak:

15 stycznia — isV update a future price update to a SKU in the catalog

16-18 stycznia — strona produktu zostanie zaktualizowana o komunikat ostrzegawczy o nadchodzącym zwiększeniu ceny, który będzie miał miejsce od 1 maja (koniec stycznia + 90 dni).

1 maja — nowa cena jest obowiązywać

## <a name="customers-affected-from-a-price-change-post-purchase"></a>Klienci, których dotyczy zmiana ceny (po zakupie)

Zakup produktu przed datą wejścia w życie zwiększenia ceny nie *gwarantuje* ceny zakupu w okresie istnienia wdrożenia produktu. Różne typy ofert, których dotyczy problem:

- Produkty oparte na zużyciu (na przykład maszyny wirtualne rozliczane według godziny lub ceny mierzonego użycia usługi SaaS lub oferty aplikacji zarządzanych), gdy nowa cena będzie efektywna, ich koszt jednostkowy zużycia zwiększy się. W przypadku klientów, którzy są rozliczani w połowie miesiąca, w miesięcznym raporcie użycia będą dostępne dwa wiersze: jeden dla użycia do daty wejścia w życie nowej ceny (w powyższym przykładzie: 1 maja) i jeden dla daty wejścia w życie zużycia
- Wpływ na produkty oparte na zużyciu z miesięczną opłatą (taką jak SaaS z miernikami niestandardowymi) będzie mieć wpływ na cenę jednostek zużycia, ponieważ nowa cena zostanie wpłynęła na platformę handlowa. Opłata miesięczna pozostanie niezmieniona do końca okresu uprawnień.
- Produkty oparte na stanowiskach (takie jak usługi SaaS oparte na licencjach), jeśli data wejścia w życie zmiany ceny nastąpi po zakupie, cena zakupu jest gwarantowana do następnej daty odnowienia , czy to miesięcznego odnowienia, czy rocznej daty odnowienia.
    - Dodawanie lub usuwanie stanowisk po zmianie ceny po dacie wejścia w życie, ale przed datą odnowienia umowy, będzie utrzymywana przy oryginalnej cenie zakupu. Po odnowieniu nowa cena rozpocznie obowiązywać.
    - Zmiana SKU, zmiana SKU po zmianie ceny data wejścia w życie będzie traktowana jako nowy zakup i będzie podlegać nowej cenie. Ta zmiana dotyczy również scenariuszy, w których zmiana liczby stanowisk wymaga zmiany wersji SKU klienta. Na przykład przeniesienie z 400 stanowisk na 500 stanowisk, co może wymagać od klienta zakupu nowej warstwy/SKU produktu.

## <a name="customer-notifications"></a>Powiadomienia klientów

Klienci, którzy już korzystali z produktu/SKU na rynku, na który ma wpływ nadchodzący wzrost cen, zostaną powiadomieni pocztą e-mail o nadchodzącej zmianie. Dzięki temu będą oni w stanie podjąć działania w tej sprawie, jeśli wybiorą taką możliwość. Powiadomienie e-mail zostanie wysłane 90 dni przed rozpoczęciem stosowania nowej ceny, a druga wiadomość zostanie wysłana 30 dni przed datą wejścia w życie zmiany ceny. Komunikat zostanie wysłany do właściciela sekcji faktury (projektu), właścicieli grupy rozliczeniowej i właścicieli konta rozliczeniowego subskrypcji.

## <a name="next-steps"></a>Następne kroki

- [Co to jest Azure Marketplace?](azure-marketplace-overview.md)
- [Azure Marketplace zakupu](azure-purchasing-invoicing.md)