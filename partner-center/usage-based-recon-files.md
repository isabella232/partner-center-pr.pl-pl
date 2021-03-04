---
title: Pliki uzgadniania oparte na użyciu
ms.topic: article
ms.date: 06/08/2020
description: Dowiedz się więcej na temat wszystkich elementów w pliku uzgodnień opartych na użyciu w centrum partnerskim. Zawiera kilka przykładów.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d3941d09d6ec808f3d188521c4f0c51c9a6d0222
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755759"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Omówienie plików uzgadniania opartych na użyciu i ich określonych pól w centrum partnerskim

Dotyczy:

- Centrum partnerskie
- Centrum partnerskie Microsoft Cloud for US Government

**Odpowiednie role**

- Administrator konta
- Administrator rozliczeń

Aby uzgodnić opłaty za użycie klienta, porównaj **ResellerID**, **resprzedawcaname** i **ResellerBillableAccount** z pliku UZGADNIAnia z **nazwą klienta** i **identyfikatorem subskrypcji** z Centrum partnerskiego.

## <a name="fields-in-usage-based-reconciliation-files"></a>Pola w plikach uzgadniania opartego na użyciu

Poniższe pola wyjaśniają, które usługi zostały użyte i stawka.

| Kolumna | Opis | Przykładowe wartości |
| ------ | ----------- | ------------ |
| PartnerId | Identyfikator partnera w formacie identyfikatora GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nazwa partnera. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identyfikator konta partnera. | *1010578050* |
| CustomerCompanyName | Nazwa organizacji klienta zgłoszona w centrum partnerskim. *Bardzo ważne jest, aby uzgodnić fakturę z informacjami o systemie.* | *Klient testowy* |
| MpnId | Identyfikator MPN partnera dostawcy usług kryptograficznych. | *4390934* |
| ResellerMpnId | MPN identyfikator odsprzedawcy rekordu dla subskrypcji.  |
| InvoiceNumber | Numer faktury, w której zostanie wyświetlona określona transakcja. | *D020001IVK* |
| ChargeStartDate | Data rozpoczęcia cyklu rozliczeniowego, z wyjątkiem czasu prezentowania dat wcześniej nieodpłatnych danych użycia (z poprzedniego cyklu rozliczeniowego). Godzina to zawsze początek dnia, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Data zakończenia cyklu rozliczeniowego, z wyjątkiem momentu prezentowania dat wcześniej nieodpłatnych danych użycia (z poprzedniego cyklu rozliczeniowego). Czas jest zawsze koniec dnia, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeń firmy Microsoft. Może być przydatne do identyfikowania subskrypcji podczas kontaktowania się z pomocą techniczną. Nieużywany do uzgadniania. *Nie jest to ten sam **Identyfikator subskrypcji** w konsoli administracyjnej partnera.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Pseudonim do oferty usługi. | *Microsoft Azure* |
| SubscriptionDescription | Biznes oferty usługi. | *Microsoft Azure* |
| OrderID | Unikatowy identyfikator zamówienia na platformie rozliczeń firmy Microsoft. Może być przydatne do identyfikowania subskrypcji podczas kontaktowania się z pomocą techniczną. Nieużywany do uzgadniania. | *566890604832738111* |
| ServiceName | Nazwa usługi platformy Azure. | *MASZYNY WIRTUALNE* |
| ServiceType | Konkretny typ usługi platformy Azure. | *Service Bus — poszczególne lub dodatki*, *SQL Azure Database — Business lub Web Edition* |
| ResourceGuid | Konkretny unikatowy identyfikator dla wszystkich danych usługi i struktury cenowej. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Nazwa zasobu platformy Azure. | *Transfer danych (GB)*, *transfer danych wychodzących (GB)* |
| Region (Region) | Region, którego dotyczy użycie. Używane przede wszystkim do przypisywania stawek do transferów danych, ponieważ stawki różnią się w zależności od regionu. | *Azja i Pacyfik*, *Europa*, *Ameryka Łacińska*, *Ameryka Północna* |
| SKU | Unikatowy identyfikator firmy Microsoft dla oferty. | *7UD — 00001* |
| DetailLineItemId | Identyfikator i ilość itemize różne stawki za usługę lub zasób w danym okresie rozliczeniowym. W przypadku cen warstwowych platformy Azure może istnieć jedna stawka za określoną liczbę jednostek rozliczanych, a następnie inna stawka po tej ilości. | *1* |
| ConsumedQuantity | Ilość zużytej usługi (na przykład godziny lub GB) w okresie raportowania. Obejmuje również wszelkie rozliczane użycie z poprzednich okresów raportowania. | *11* |
| IncludedQuantity | Jednostki wchodzące w skład oferty. Zwykle nieobecny w dostawcy CSP. | *0* |
| OverageQuantity | Jednostki, które nie należą do oferty. Muszą one być płatne przez partnera. Równa się **ConsumedQuantity** minus **IncludedQuantity**. | *11* |
| ListPrice | Cena oferty obowiązuje w dniu rozpoczęcia subskrypcji. | *$0,0808* |
| PretaxCharges | Równe **ListPrist** pomnożone przez **OverageQuantity**, zaokrąglone do najbliższej wartości procentowej. | *$0,085* |
| TaxAmount | Kwota podatku naliczana. Na podstawie reguł podatkowych i określonych okoliczności na rynku. | *$0,08* |
| PostTaxTotal | Suma po opodatkowaniu, gdy jest stosowany podatek. | *$0,93* |
| Waluta | Typ waluty. Każda jednostka rozliczeniowa ma tylko jedną walutę. Sprawdź, czy pasuje do pierwszej faktury, a następnie po każdej ważnej aktualizacji platformy rozliczeniowej. | *EUR* |
| PretaxEffectiveRate | Cena pretax na jednostkę. Równe **PretaxCharges** podzielone przez **OverageQuantity**, zaokrąglone do najbliższej wartości procentowej. | *$0,08* |
| PostTaxEffectiveRate | Opłata skarbowa na jednostkę. Równe **PostTaxTotal** podzielone przez **OverageQuantity**, zaokrąglone do najbliższej wartości procentowej. Lub równa **PretaxEffectiveRate** Plus stawka podatkowa za jednostkę, zaokrąglona do najbliższej wartości procentowej. | *$0,08* |
| ChargeType | [Typ opłaty](recon-file-charge-types.md) lub korekty. | Zobacz [typy opłat](recon-file-charge-types.md). |
| CustomerId | Unikatowy identyfikator firmy Microsoft dla klienta w formacie GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nazwa domeny klienta. To pole może pojawić się puste do momentu drugiego okresu rozliczeniowego. | *example.onmicrosoft.com* |
| BillingCycleType | Częstotliwość rozliczania czasu.| **Raz na miesiąc**  |
| Jednostka | Jednostka **nazwy** zasobu. | *GB* lub *godz* . |
| CustomerBillableAccount | Unikatowy identyfikator konta na platformie rozliczeń firmy Microsoft. | *1280018095* |
| UsageDate | Data wdrożenia usługi. | *2/1/2019 0:00* |
| MeteredRegion | Określa lokalizację centrum danych w regionie (dla usług, w których ta wartość jest stosowana i wypełniana). | *Azja Wschodnia*, *Południowe Azja Wschodnia*, *Europa Północna*, *Europa Zachodnia*, *Północno-środkowe stany USA*, *Południowo-środkowe stany USA* |
| MeteredService | Identyfikuje indywidualne użycie usługi platformy Azure, jeśli nie jest ona wyraźnie określona w kolumnie **ServiceName** . Na przykład transfery danych są raportowane jako *Microsoft Azure — wszystkie usługi* w kolumnie **ServiceName** . | *AccessControl*, *CDN*, *COMPUTE*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Podnagłówek dla pola **MeteredService** , które zapewnia dodatkowe wyjaśnienie użycia usługi platformy Azure. | *ZEWNĘTRZNYCH* |
| Project | Zdefiniowana przez klienta nazwa wystąpienia usługi. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Liczba połączeń Azure Service Bus, które zostały zainicjowane i wykorzystane w danym dniu. | *1,000000 połączeń/30 dni* (Jeśli w ciągu 30-dniowego miesiąca zarejestrowano się indywidualnie), *25 połączeń/30 dni — używane: 1,000000* (Jeśli korzystasz z 25 pakietów Service Bus połączenia z zainicjowaną obsługą 1 w tym dniu) |

## <a name="next-steps"></a>Następne kroki

- [Informacje o polach w plikach uzgodnień opartych na licencji Centrum partnerskiego](license-based-recon-files.md)