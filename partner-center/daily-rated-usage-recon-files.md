---
title: Pliki uzgodnień użycia ocenianego codziennie
ms.topic: article
ms.date: 06/12/2020
description: Dowiedz się, jak odczytywać pliki uzgodnień dziennego użycia w Partner Center. Zawiera opisy dla określonych pól w pliku rekonescją.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6d3d414aa33991888fcd8b81864e2adee9a46f46
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/03/2021
ms.locfileid: "123457943"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Dowiedz się, jak odczytywać pliki uzgodnień użycia codziennie w u Partner Center

**Dotyczy:** Partner Center | Partner Center dla Microsoft Cloud for US Government

**Odpowiednie role:** Administrator | Administrator rozliczeń | Agent sprzedaży | Agent pomocy technicznej

W tym artykule wyjaśniono, jak odczytywać pliki uzgodnień dziennego użycia.

>[!NOTE]
>Dzienne użycie oceniane zwykle trwa 24 godziny, aby pojawiać się w Partner Center lub uzyskać do niego dostęp za pośrednictwem interfejsu API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Pola w plikach uzgodnień dziennego użycia

| Kolumna | Opis |
| ------ | ----------- |
| PartnerId | Identyfikator partnera w formacie identyfikatora GUID. |
| PartnerName | Nazwa partnera. |
| CustomerId | Unikatowy identyfikator microsoft klienta w formacie identyfikatora GUID. |
| CustomerName | Nazwa organizacji klienta zgłoszona w Partner Center. *Ta kolumna jest ważna w przypadku uzgadniania faktury z informacjami o systemie.* |
| CustomerDomainName | Nazwa domeny klienta. |
| CustomerCountry | Kraj, w którym znajduje się klient. |
| MpnId | Identyfikator MPN partnera CSP. |
| Tier2MpnId | Identyfikator MPN odsprzedawcy rekordu dla subskrypcji. |
| InvoiceNumber | Numer faktury, na której pojawia się określona transakcja. |
| ProductId | Identyfikator produktu. |
| SkuId | Identyfikator określonej jednostki SKU. |
| AvailabilityId | Identyfikator dostępności określonej jednostki SKU. Ta kolumna pokazuje, czy można kupić tę sku w danym kraju, walucie, segmencie branżowym itp. |
| SkuName | Tytuł określonej sku. |
| ProductName | Nazwa produktu. |
| PublisherName | Nazwa wydawcy. |
| PublisherId | Identyfikator wydawcy w formacie identyfikatora GUID. |
| SubscriptionDescription | Nazwa oferty usługi zakupionej przez klienta, zgodnie z definicją w cenniku. (Ta kolumna jest identycznym polem **offername).** |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeniowej firmy Microsoft. Nie służy do uzgadniania. *Ten identyfikator nie jest taki sam jak identyfikator **subskrypcji** w konsoli administracyjnej partnera.* |
| ChargeStartDate | Data rozpoczęcia cyklu rozliczeniowego (z wyjątkiem dat prezentowania wcześniej niezaliczanych danych użycia ukrytego z poprzedniego cyklu rozliczeniowego). Godzina to zawsze początek dnia, 0:00. |
| ChargeEndDate | Data końcowa cyklu rozliczeniowego (z wyjątkiem prezentowania dat wcześniej niezapłacanych danych użycia ukrytego z poprzedniego cyklu rozliczeniowego). Godzina to zawsze koniec dnia, 23:59. |
| UsageDate | Data użycia usługi. |
| Typ miernika | Typ miernika. |
| MeterCategory | Usługa najwyższego poziomu do użycia. |
| MeterId | Identyfikator używanego miernika. |
| MeterSubCategory | Typ usługi platformy Azure, który może mieć wpływ na stawkę. |
| MeterName | Jednostka miary używanego miernika. |
| MeterRegion | Ta kolumna określa lokalizację centrum danych w regionie dla usług, w których region miernika ma zastosowanie i jest wypełniony. |
| Jednostka | Jednostka zasobu **Nazwa**. |
| ResourceLocation | Centrum danych, w którym jest uruchomiony miernik. |
| ConsumedService | Używana usługa platformy Azure. |
| ResourceGroup | Reprezentuje kontener, który zawiera powiązane zasoby dla rozwiązania platformy Azure. |
| ResourceURI | URI używanego zasobu. |
| ChargeType | Typ opłaty lub korekty.  |
| UnitPrice | Cena za licencję opublikowana w cenniku w momencie zakupu. Upewnij się, że ta cena odpowiada informacjom przechowywanym w systemie rozliczeniowym podczas uzgadniania. |
| Liczba | Liczba licencji. Upewnij się, że ta cena odpowiada informacjom przechowywanym w systemie rozliczeniowym podczas uzgadniania. |
| Unittype | Typ jednostki, w przypadku których jest naliczana opłata za miernik.  |
| BillingPreTaxTotal | Łączna kwota rozliczeniowa przed podatkami.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Waluta w regionie geograficznym klienta. |
| PricingPreTaxTotal | Cennik przed dodaniu podatków. |
| PricingCurrency | Waluta w cenniku. |
| ServiceInfo1 | Liczba połączeń Service Bus, które zostały zaaprowizowane i użyte w danym dniu. |
| ServiceInfo2 | Starsze pole, które przechwytuje opcjonalne metadane specyficzne dla usługi. |
| Tagi | Reprezentuje logiczną organizację zasobów platformy Azure ustawioną przez użytkownika. |
| AdditionalInfo | Wszelkie dodatkowe informacje, które nie są zawarte w innych kolumnach. |
| EffectiveUnitPrice | Rzeczywista wartość naliczana za jednostkę, w tym wszelkie rabaty, uzyskane punkty itp. |
| PCToBCExchangeRate | Exchange stosowana dla waluty cennika na walutę rozliczeniową. |
| PCToBCExchangeRateDate | Data, w której jest określana waluta cenowa waluty rozliczeniowej. |
| EntitlementId | Reprezentuje identyfikator subskrypcji platformy Azure. |
| EntitlementDescription | Reprezentuje nazwę identyfikatora subskrypcji platformy Azure. |
| PartnerEarnedCreditPercentage | Wyświetla partnerearnedcredit dla elementu wiersza. Uzyskane punkty to 0 lub 15% |
| CreditPercentage (CreditPercentage) | Wyświetla informacje o środków na korzystanie z platformy Azure. Uzyskane punkty to 0 lub 100 procent. |
| CreditType | Typ środków. Na przykład Zastosowane **środków na korzystanie z platformy Azure.** |

>[!NOTE]
>Dzienne użycie oceniane zwykle trwa 24 godziny, aby pojawiać się w Partner Center lub uzyskać do niego dostęp za pośrednictwem interfejsu API.
