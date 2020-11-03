---
title: Pliki uzgadniania użycia codziennie
ms.topic: article
ms.date: 06/12/2020
description: Informacje na temat odczytywania codziennych plików uzgadniania użycia w centrum partnerskim. Zawiera opisy dla konkretnych pól w pliku rekonesans.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8b45ef4767e4bde28befd35c5294ed19149bf034
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530394"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Informacje na temat odczytywania codziennych plików uzgadniania użycia w centrum partnerskim

**Dotyczy**

- Centrum partnerskie
- Centrum partnerskie dla Microsoft Cloud dla instytucji rządowych USA

**Odpowiednie role**

- Agent administracyjny
- Administrator rozliczeń
- Agent sprzedaży
- Agent pomocy technicznej

W tym artykule wyjaśniono, jak czytać pliki uzgadniania użycia codziennie.

>[!NOTE]
>Dzienne użycie zwykle trwa 24 godziny w centrum partnerskim lub dostęp do niego za pomocą interfejsu API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Pola w plikach uzgadnianych codziennych użycia

| Kolumna | Opis |
| ------ | ----------- |
| PartnerId | Identyfikator partnera w formacie identyfikatora GUID. |
| PartnerName | Nazwa partnera. |
| CustomerId | Unikatowy identyfikator firmy Microsoft dla klienta w formacie identyfikatora GUID. |
| CustomerName | Nazwa organizacji klienta zgłoszona w centrum partnerskim. *Ta kolumna jest ważna w przypadku uzgadniania faktury z informacjami o systemie.* |
| CustomerDomainName | Nazwa domeny klienta. |
| CustomerCountry | Kraj, w którym znajduje się klient. |
| MpnId | Identyfikator MPN partnera dostawcy usług kryptograficznych. |
| Tier2MpnId | MPN identyfikator odsprzedawcy rekordu dla subskrypcji. |
| InvoiceNumber | Numer faktury, w której zostanie wyświetlona określona transakcja. |
| ProductId | Identyfikator produktu. |
| Identyfikatora skuId | Identyfikator określonej jednostki SKU. |
| AvailabilityId | Identyfikator dla dostępności określonej jednostki SKU. Ta kolumna wskazuje, czy jednostka SKU jest dostępna do zakupu w danym kraju, walucie, segmencie branżowym itd. |
| SkuName | Tytuł określonej jednostki SKU. |
| ProductName | Nazwa produktu. |
| PublisherName | Nazwa wydawcy. |
| PublisherId | Identyfikator wydawcy w formacie identyfikatora GUID. |
| SubscriptionDescription | Nazwa oferty usługi zakupionej przez klienta zgodnie z definicją w cenniku. (Ta kolumna jest tym samym polem, aby **zaoferowaćname** ). |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeń firmy Microsoft. Nieużywany do uzgadniania. *Ten identyfikator nie jest taki sam jak **Identyfikator subskrypcji** w konsoli administracyjnej partnera.* |
| ChargeStartDate | Data rozpoczęcia cyklu rozliczeniowego (z wyjątkiem przedstawiania dat wcześniej nieobciążona ukrytymi danymi użycia z poprzedniego okresu rozliczeniowego). Godzina to zawsze początek dnia, 0:00. |
| ChargeEndDate | Data zakończenia cyklu rozliczeniowego (z wyjątkiem przedstawiania dat wcześniej nieodpłatnych danych użycia z poprzedniego okresu rozliczeniowego). Czas jest zawsze koniec dnia, 23:59. |
| UsageDate | Data użycia usługi. |
| Licznik mierników | Typ miernika. |
| MeterCategory | Usługa najwyższego poziomu do użycia. |
| MeterId | Identyfikator używanego licznika. |
| MeterSubCategory | Typ usługi platformy Azure, który może mieć wpływ na stawkę. |
| MeterName | Jednostka miary zużytego licznika. |
| MeterRegion | Ta kolumna określa lokalizację centrum danych w regionie dla usług, gdzie MeterRegion ma zastosowanie i jest wypełniona. |
| Jednostka | Jednostka **nazwy** zasobu. |
| ResourceLocation | Centrum danych, w którym jest uruchomiony licznik. |
| ConsumedService | Użyta usługa platformy Azure. |
| ResourceGroup | Reprezentuje kontener, który zawiera powiązane zasoby dla rozwiązania platformy Azure. |
| ResourceURI | Identyfikator URI używanego zasobu. |
| ChargeType | Typ opłaty lub korekty.  |
| Cena jednostkowa | Cena za licencję publikowana w cenniku w momencie zakupu. Zadbaj o to, aby cena była zgodna z informacjami przechowywanymi w systemie rozliczeniowym podczas uzgadniania. |
| Liczba | Liczba licencji. Zadbaj o to, aby cena była zgodna z informacjami przechowywanymi w systemie rozliczeniowym podczas uzgadniania. |
| UnitType | Typ jednostki, w której jest naliczany pomiar.  |
| BillingPreTaxTotal | Łączna kwota rozliczeń przed opodatkowaniem.<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ] *[ @Quantity ]* [ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Waluta w regionie geograficznym klienta. |
| PricingPreTaxTotal | Ceny przed dodaniem podatków. |
| PricingCurrency | Waluta w cenniku. |
| ServiceInfo1 | Liczba połączeń Service Bus, które zostały zainicjowane i wykorzystane w danym dniu. |
| ServiceInfo2 | Starsze pole, które przechwytuje opcjonalne metadane specyficzne dla usługi. |
| Tagi | Reprezentuje logiczną organizację zasobów platformy Azure ustawionych przez użytkownika. |
| AdditionalInfo | Wszelkie dodatkowe informacje, które nie są zawarte w innych kolumnach. |
| EffectiveUnitPrice | Rzeczywista wartość naliczana na jednostkę, w tym rabaty, kredyty i tak dalej. |
| PCToBCExchangeRate | Kurs wymiany stosowany w przypadku waluty cenowej do faktury rozliczeniowej. |
| PCToBCExchangeRateDate | Data ustalenia waluty cenowej waluty rozliczeniowej. |
| EntitlementId | Reprezentuje identyfikator subskrypcji platformy Azure. |
| EntitlementDescription | Reprezentuje nazwę identyfikatora subskrypcji platformy Azure. |
| PartnerEarnedCreditPercentage | Wyświetla PartnerEarnedCredit dla elementu wiersza. Kwota uzyskanych środków wynosi 0 lub 15% |

>[!NOTE]
>Dzienne użycie zwykle trwa 24 godziny w centrum partnerskim lub dostęp do niego przy użyciu interfejsu API.


