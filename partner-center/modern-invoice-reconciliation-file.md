---
title: Rekonesans pola pliku dla dostawcy CSP jednorazowe zakupy
ms.topic: conceptual
ms.date: 01/29/2021
description: Dowiedz się więcej na temat wszystkich elementów w pliku uzgadniania zakupów jednorazowych w programie CSP w centrum partnerskim, łącznie z przykładowymi wartościami.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: f1606cceaf9dec1f04850fd85b3924ef75bbfda0
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098809"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Pola pliku uzgadniania zakupów jednorazowych dostawcy CSP

## <a name="using-the-recon-file"></a>Korzystanie z pliku Rekonesans
W poniższej tabeli przedstawiono opisy i przykładowe wartości pól w pliku uzgadniania jednorazowych zakupów dla dostawcy usług kryptograficznych.

Aby uzyskać więcej informacji na temat plików uzgadniania, zobacz [Używanie plików uzgadniania](use-the-reconciliation-files.md).

| Kolumna | Opis | Wartość przykładowa |
| ------ | ----------- | ------------ |
| PartnerId | Unikatowy identyfikator w formacie identyfikatora GUID dla określonej jednostki rozliczania. Niewymagane do uzgodnienia. Taka sama we wszystkich wierszach. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Unikatowy identyfikator firmy Microsoft dla klienta w formacie identyfikatora GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nazwa organizacji klienta zgłoszona w centrum partnerskim. Ta kolumna jest ważna w przypadku uzgadniania faktury z informacjami o systemie. | *Johnny nowoczesny DE2* |
| CustomerDomainName | Nazwa domeny klienta. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Kraj, w którym znajduje się Twój klient. Zapoznaj się z pełną [listą krajów](./regional-authorization-overview.md) w Twoim regionie.  | *DE* |
| InvoiceNumber | Numer faktury skojarzony z plikiem uzgodnienia.  | *G002297372* |
| MpnId | Identyfikator MPN partnera dostawcy usług kryptograficznych. Aby uzyskać więcej informacji, zobacz [How to itemize by partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | MPN identyfikator odsprzedawcy rekordu dla subskrypcji. | *6048879* |
| OrderId (Identyfikator zamówienia) | Unikatowy identyfikator zamówienia na platformie rozliczeń firmy Microsoft. Może być przydatne do identyfikowania zamówienia podczas kontaktowania się z pomocą techniczną. Nieużywany do uzgadniania. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate (Data zamówienia) | Data umieszczenia zamówienia. | *10/3/2020* |
| ProductId | Unikatowy identyfikator produktu. | *DZH318Z0BNZ5* |
| Identyfikatora skuId | Unikatowy identyfikator jednostki SKU. | *006G* |
| AvailabilityId | Unikatowy identyfikator dostępności. | *DZH318Z08B80* |
| SkuName | Nazwa jednostki SKU. | *Tabele — LRS* |
| ProductName | Nazwa produktu. | *Tabele* |
| ChargeType | [Typ opłaty](./recon-file-charge-types.md) lub korekty. | *Nowe* |
| UnitPrice | Cena za licencję publikowana w cenniku w momencie zakupu. Upewnij się, że są one zgodne z informacjami przechowywanymi w systemie rozliczeniowym podczas uzgadniania. | *0,045* |
| Liczba | Liczba licencji. Upewnij się, że są one zgodne z informacjami przechowywanymi w systemie rozliczeniowym podczas uzgadniania. | *1* |
| Suma częściowa | Suma przed podatkiem. Suma częściowa powinna być równa ilości rozliczanej pomnożonej przez obowiązującą cenę jednostkową. | *0* |
| TaxTotal | Opłata za podatek. Na podstawie reguł podatkowych i określonych okoliczności na rynku. | *0* |
| Łącznie | Łączna kwota jest równa sumie częściowej powiększonej o kwotę podatku. | *0* |
| Waluta | Rachunek jest generowany w kontekście waluty klienta. Oznacza to, że jeśli jesteś partnerem transakcji z użyciem różnych walut rozliczanych, otrzymasz fakturę dla każdego typu waluty klienta.  | *EUR* |
| PriceAdjustmentDescription | Przyczyny korekty ceny jednostkowej. Są to główne przyczyny, ale nie są ograniczone do określania efektywnej ceny jednostkowej. | *["15,0% w przypadku partnerów uzyskano środki na zarządzanie usługami"]* |
| PublisherName | Wydawca produktu.  | *Microsoft* |
| PublisherId | Unikatowy identyfikator, którego centrum partnerskie używa do identyfikowania wydawcy. | *NA* |
| SubscriptionDescription | Nazwa oferty usługi zakupionej przez klienta zgodnie z definicją w cenniku. Ta kolumna jest tym samym polem, aby Zaoferowaćname. | *Plan platformy Azure* |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeń firmy Microsoft. Nieużywany do uzgadniania. Należy pamiętać, że ten identyfikator nie jest taki sam jak identyfikator subskrypcji w konsoli administracyjnej partnera. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Data Centrum partnerskiego opłaty za subskrypcję. W przypadku zakupu subskrypcji z rocznym okresem rozliczeniowym i comiesięcznym planem rozliczeniowym, a następnie w pierwszym pliku uzgodnienia jest to dzień, w którym zakupiona została subskrypcja. Począwszy od następnego pliku uzgodnienia, zostanie on zwiększony o 30 dni. | *9/1/2020* |
| ChargeEndDate | Dzień końcowy opłat za cykl rozliczeniowy subskrypcji. W przypadku zakupu subskrypcji z rocznym okresem rozliczeniowym i comiesięcznym planem rozliczeniowym, a następnie w pierwszym pliku uzgodnienia jest to 30-dniowy dzień po zakupie subskrypcji. Począwszy od następnego pliku uzgodnienia, zostanie on zwiększony o 30 dni. | *2020-09-30* |
| TermAndBillingCycle | Czas trwania zobowiązania do kontynuowania subskrypcji w momencie zakupu. | *Dane przechowywane (GB/miesiąc)* |
| EffectiveUnitPrice | Cena za jednostkę proporcjonalną do obliczenia kosztu cyklu rozliczeniowego. Rabaty, korekty w dniach rozliczeniowych i inne czynniki określają obowiązującą cenę jednostkową. Aby uzyskać więcej informacji, zobacz [efektywne Obliczanie cen jednostkowych](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Typ jednostki, w której jest naliczany licznik. | *1 GB/miesiąc* |
| AlternateId | Alternatywny identyfikator elementu wiersza zamówienia, do którego się odwoływano. | *6dc5c039750a* |
| BillableQuantity | Łączna liczba rozliczanych opłat.  | *0,005001* |
| BillingFrequency | Plan rozliczeń wybrany w momencie zakupu. | *NA*  |
| PricingCurrency | Waluta w cenniku. | *USD* |
| PCToBCExchangeRate | Kurs wymiany stosowany w przypadku waluty cenowej do faktury rozliczeniowej. | *0,846202666* |
| PCToBCExchangeRateDate | Data ustalenia waluty cenowej waluty rozliczeniowej. | *2020-09-30* |
| MeterDescription | Opis miernika.  | *Tabele — LRS dane przechowywane (GB/miesiąc)* |
| ReservationOrderId | Identyfikator zamówienia rezerwacji. | *E21A6344E398FFC1C4D7...* |

>[!NOTE]
>Możesz uzgodnić użycie platformy Azure w pliku Rekonesans zakupu jednorazowego. W tym celu przejdź do pliku Rekonesans o codziennym użyciu i Wyszukaj swój identyfikator subskrypcji. Spowoduje to wyświetlenie wszystkich kosztów skojarzonych z IDENTYFIKATORem planu platformy Azure. Identyfikator subskrypcji platformy Azure jest pokazywany jako EntitlementID.

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i podatki](billing.md)