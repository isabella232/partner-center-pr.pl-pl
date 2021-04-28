---
title: Recon file fields for CSP one-time purchases (Ponowne pola plików dla zakupów jednego programu CSP)
ms.topic: conceptual
ms.date: 01/29/2021
description: Dowiedz się więcej na temat wszystkich elementów w pliku uzgodnień dotyczących zakupów Partner Center CSP, w tym przykładowych wartości.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 7ff320124230ec8e0b3505b1c1dbbb7c811cb67f
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120720"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Pola pliku uzgodnień zakupu terminowego programu CSP

**Odpowiednie role**

- Administrator konta
- Agent rozliczeń

## <a name="using-the-recon-file"></a>Korzystanie z pliku rekonescji
W poniższej tabeli przedstawiono opisy i przykładowe wartości pól w pliku uzgodnień dla zakupów tylko raz w programie CSP.

Aby uzyskać więcej informacji na temat plików uzgodnień, zobacz [Używanie plików uzgodnień](use-the-reconciliation-files.md).

| Kolumna | Opis | Wartość przykładowa |
| ------ | ----------- | ------------ |
| PartnerId | Unikatowy identyfikator w formacie identyfikatora GUID dla określonej jednostki rozliczeniowej. Nie jest wymagane do uzgadniania. Tak samo we wszystkich wierszach. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Unikatowy identyfikator firmy Microsoft dla klienta w formacie identyfikatora GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nazwa organizacji klienta zgłoszona w Partner Center. Ta kolumna jest ważna w przypadku uzgadniania faktury z informacjami o systemie. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Nazwa domeny klienta. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Kraj, w którym znajduje się Klient. Zobacz pełną [listę krajów dla](./regional-authorization-overview.md) Twojego regionu.  | *DE* |
| InvoiceNumber | Numer faktury skojarzony z plikiem uzgodnień.  | *G002297372* |
| MpnId | Identyfikator MPN partnera CSP. Aby uzyskać więcej informacji, [zobacz, jak elementować według partnera](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identyfikator MPN odsprzedawcy rekordu dla subskrypcji. | *6048879* |
| OrderId (Identyfikator zamówienia) | Unikatowy identyfikator zamówienia na platformie rozliczeniowej firmy Microsoft. Może być przydatna do zidentyfikowania zamówienia podczas kontaktowania się z pomocą techniczną. Nie służy do uzgadniania. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate (Data zamówienia) | Data zamówienia. | *10/3/2020* |
| ProductId | Unikatowy identyfikator produktu. | *DZH318Z0BNZ5* |
| SkuId | Unikatowy identyfikator jednostki SKU. | *006G* |
| AvailabilityId | Unikatowy identyfikator dostępności. | *DZH318Z08B80* |
| SkuName | Nazwa SKU. | *Tabele — LRS* |
| ProductName | Nazwa produktu. | *Tabele* |
| ChargeType | Typ [opłaty lub](./recon-file-charge-types.md) korekty. | *Nowe* |
| UnitPrice | Cena za licencję opublikowana w cenniku w momencie zakupu. Upewnij się, że jest to informacja przechowywana w systemie rozliczeniowym podczas uzgadniania. | *0.045* |
| Liczba | Liczba licencji. Upewnij się, że jest to informacja przechowywana w systemie rozliczeniowym podczas uzgadniania. | *1* |
| Suma częściowa | Suma przed opodatkowaniem. Suma częściowa powinna być równa rozliczanej ilości pomnożonej przez efektywną cenę jednostkową. | *0* |
| TaxTotal | Kwota podatku. Na podstawie reguł podatkowych obowiązujących na rynku i określonych okoliczności. | *0* |
| Łącznie | Łączna kwota jest równa sumie częściowej plus kwota podatku. | *0* |
| Waluta | Rachunek jest generowany w kontekście waluty klienta. Oznacza to, że jeśli jesteś partnerem w transakcji z klientami z różnych rozliczanych walut, otrzymasz fakturę dla każdego typu waluty klienta.  | *EUR* |
| PriceAdjustmentDescription | Przyczyny korekt ceny jednostkowej. Są to główne przyczyny, ale nie tylko ustalanie efektywnej ceny jednostkowej. | *["15,0% środków uzyskane przez partnerów dla usług zarządzanych"]* |
| PublisherName | Wydawca produktu.  | *Microsoft* |
| PublisherId | Unikatowy identyfikator używany Partner Center do identyfikowania wydawcy. | *NA* |
| SubscriptionDescription | Nazwa oferty usługi zakupionej przez klienta, zgodnie z definicją w cenniku. Ta kolumna jest identycznym polem co OfferName. | *Plan platformy Azure* |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeniowej firmy Microsoft. Nie służy do uzgadniania. Należy pamiętać, że ten identyfikator nie jest taki sam jak identyfikator subskrypcji w konsoli administracyjnej partnera. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Data rozpoczęcia okresu rozliczeniowego subskrypcji. | *9/1/2020* |
| ChargeEndDate | Data zakończenia okresu rozliczeniowego subskrypcji. | *2020-09-30* |
| TermAndBillingCycle | Zobowiązanie czasu trwania w celu kontynuowania subskrypcji w momencie zakupu. | *Dane przechowywane (GB/miesiąc)* |
| EffectiveUnitPrice | Proporcjonalna cena jednostkowa do obliczenia kosztu dla cyklu rozliczeniowego. Rabaty, korekty w dniach rozliczeniowych i inne czynniki określają efektywną cenę jednostkową. Aby uzyskać więcej informacji, zobacz [Obliczanie efektywnej ceny jednostkowej](./effective-unit-price-calculation.md).  | *0.03825* |
| Unittype | Typ jednostki, w której jest naliczany miernik. | *1 GB/miesiąc* |
| AlternateId | Alternatywny identyfikator elementu wiersza zamówienia, do których się odwołujesz. | *6dc5c039750a* |
| Ilość rozliczana | Łączna ilość rozliczana.  | *0.005001* |
| BillingFrequency | Plan rozliczeniowy wybrany w momencie zakupu. | *NA*  |
| PricingCurrency | Waluta w cenniku. | *USD* |
| PCToBCExchangeRate | Kurs wymiany stosowany dla waluty cennika na walutę rozliczeniową. | *0.846202666* |
| PCToBCExchangeRateDate | Data, w której jest określana waluta cenowa na walutę rozliczeniową. | *2020-09-30* |
| MeterDescription (Opis miernika) | Opis miernika.  | *Tabele — dane LRS przechowywane (GB/miesiąc)* |
| ReservationOrderId | Identyfikator zamówienia rezerwacji. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Opis środków. | *Środków na korzystanie z platformy Azure* |

>[!NOTE]
>Możesz uzgodnić zużycie platformy Azure w pliku ponownego zakupu w ramach jednego zakupu. W tym celu przejdź do pliku z rekonescją dziennego użycia i wyszukaj swój subscriptionID. Spowoduje to wyświetlenie wszystkich kosztów skojarzonych z identyfikatorem planu platformy Azure. Twoja subskrypcja platformy Azure jest wyświetlana jako entitlementID.

## <a name="next-steps"></a>Następne kroki

- [Rozliczenia i podatki](billing.md)
