---
title: Pliki uzgodnień na podstawie użycia
ms.topic: article
ms.date: 06/08/2020
description: Dowiedz się więcej o wszystkich elementach w pliku uzgodnień opartym na użyciu w Partner Center. Zawiera kilka przykładów.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3048bad7912f101e1c332e54eff981473f0f31d7
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246580"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Informacje o plikach uzgodnień opartych na użyciu i ich określonych polach w Partner Center

**Odpowiednie role:** Administrator konta | Administrator rozliczeń

Aby uzgodnić opłaty z użyciem klienta, porównaj wartości **ResellerID**, **ResellerName** i  **ResellerBillableAccount** z pliku uzgodnień z polami **Nazwa** klienta i Identyfikator subskrypcji z Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Pola w plikach uzgodnień opartych na użyciu

W poniższych polach wyjaśniono, które usługi zostały użyte i jakie są stawki.

| Kolumna | Opis | Przykładowe wartości |
| ------ | ----------- | ------------ |
| PartnerId | Identyfikator partnera w formacie IDENTYFIKATORA GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nazwa partnera. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identyfikator konta partnera. | *1010578050* |
| CustomerCompanyName | Nazwa organizacji klienta zgłoszona w Partner Center. *Jest to bardzo ważne w przypadku uzgadniania faktury z informacjami o systemie.* | *Klient testowy* |
| MpnId | Microsoft Partner Network (MPN) partnera Dostawca rozwiązań w chmurze (CSP). | *4390934* |
| ResellerMpnId | Identyfikator MPN odsprzedawcy rekordu dla subskrypcji.  |
| InvoiceNumber | Numer faktury, na której pojawia się określona transakcja. | *D020001IVK* |
| ChargeStartDate | Data rozpoczęcia cyklu rozliczeniowego, z wyjątkiem dat wcześniej nienaliczanych danych użycia ukrytego (z poprzedniego cyklu rozliczeniowego). Godzina to zawsze początek dnia, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Data zakończenia cyklu rozliczeniowego, z wyjątkiem dat wcześniej niezaliczanych danych użycia ukrytego (z poprzedniego cyklu rozliczeniowego). Czas to zawsze koniec dnia, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeniowej firmy Microsoft. Może być przydatna do zidentyfikowania subskrypcji podczas kontaktowania się z pomocą techniczną. Nie są używane do uzgadniania. *To nie jest to samo co **identyfikator subskrypcji w** konsoli administracyjnej partnera.* | *usCBMgAAAAAAAAIAA* |
| SubscriptionName | Pseudonim oferty usługi. | *Microsoft Azure* |
| SubscriptionDescription | Działalność biznesowa oferty usług. | *Microsoft Azure* |
| OrderID | Unikatowy identyfikator zamówienia na platformie rozliczeniowej firmy Microsoft. Może być przydatna do zidentyfikowania subskrypcji podczas kontaktowania się z pomocą techniczną. Nie są używane do uzgadniania. | *566890604832738111* |
| ServiceName | Nazwa usługi platformy Azure, o których mowa. | *MASZYNY WIRTUALNE* |
| ServiceType | Określony typ usługi platformy Azure. | *Service Bus — indywidualny lub pakiet,* *Usługi SQL Azure database — Business lub Web Edition* |
| ResourceGuid | Określony unikatowy identyfikator dla wszystkich danych usługi i struktury cen. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Nazwa zasobu platformy Azure. | *Transfer danych w (GB),* *transfer danych na zewnątrz (GB)* |
| Region (Region) | Region, do którego ma zastosowanie użycie. Służy głównie do przypisywania stawek do transferów danych, ponieważ stawki różnią się w zależności od regionu. | *Azja i Pacyfik,* *Europa,* *Ameryka Łacińska*, *Ameryka Północna* |
| SKU | Unikatowy identyfikator firmy Microsoft dla oferty. | *7UD-00001* |
| DetailLineItemId | Identyfikator i ilość do podano różne stawki dla usługi lub zasobu w danym okresie rozliczeniowym. W przypadku cen warstwowych platformy Azure może być naliczana jedna stawka dla maksymalnie określonej liczby rozliczanych jednostek, a następnie inna stawka po tej ilości. | *1* |
| ConsumedQuantity | Ilość zużytej usługi (np. godziny lub GB) w okresie raportowania. Obejmuje również wszelkie nienaliowane użycie z poprzednich okresów raportowania. | *11* |
| IncludedQuantity | Jednostki uwzględnione w ramach oferty. Zwykle nie występuje w programie CSP. | *0* |
| OverageQuantity | Jednostki nie są uwzględnione w ramach oferty. Muszą one zostać opłacone przez partnera. Równa wartości **ConsumedQuantity** minus **IncludedQuantity**. | *11* |
| Listprice | Cena oferty obowiązywała w dniu rozpoczęcia subskrypcji. | *0,0808 USD* |
| PretaxCharges | Równa się **wartości ListPrist** pomnożonej **przez wartość OverageQuantity** zaokrągloną do najbliższego centa. | *0,085 USD* |
| TaxAmount | Kwota podatku naliczona. Na podstawie reguł podatkowych obowiązujących na rynku i określonych okoliczności. | *0,08 USD* |
| PostTaxTotal | Suma po opodatkowaniu, gdy podatek ma zastosowanie. | *0,93 USD* |
| Waluta | Typ waluty. Każda jednostka rozliczeniowa ma tylko jedną walutę. Sprawdź, czy jest ona taka jak pierwsza faktura, a następnie po aktualizacji dowolnej ważnej platformy rozliczeniowej. | *EUR* |
| PretaxEffectiveRate | Cena przedtax na jednostkę. Równe **pretaxCharges** podzielone przez **overageQuantity**, zaokrąglone do najbliższego centa. | *0,08 USD* |
| PostTaxEffectiveRate | Po cenie podatku na jednostkę. Równa się **wartości PostTaxTotal** podzielonej **przez wartość OverageQuantity** zaokrągloną do najbliższego centa. Lub równe **PretaxEffectiveRate** plus stawka podatku na kwotę jednostkową, zaokrąglona do najbliższego centa. | *0,08 USD* |
| ChargeType | Typ [opłaty lub](recon-file-charge-types.md) korekty. | Zobacz [typy opłat.](recon-file-charge-types.md) |
| CustomerId | Unikatowy identyfikator microsoft klienta w formacie identyfikatora GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nazwa domeny klienta. To pole może być puste do czasu drugiego cyklu rozliczeniowego. | *example.onmicrosoft.com* |
| BillingCycleType | Częstotliwość rozliczeń czasu.| **Raz na miesiąc**  |
| Jednostka | Jednostka zasobu **Nazwa**. | *GB* lub *GODZINY* |
| CustomerBillableAccount | Unikatowy identyfikator konta na platformie rozliczeniowej firmy Microsoft. | *1280018095* |
| UsageDate | Data wdrożenia usługi. | *2/1/2019 0:00* |
| Region mierzony | Określa lokalizację centrum danych w regionie (dla usług, w których ta wartość ma zastosowanie i jest wypełniana). | *Azja Wschodnia*, *South Azja Wschodnia*, *North Europe*, West *Europe*, North *Central US*, South *Central US* |
| MeteredService | Identyfikuje użycie poszczególnych usług platformy Azure, jeśli nie zostanie ono wyraźnie zidentyfikowane w kolumnie **ServiceName.** Na przykład transfery danych są zgłaszane jako *Microsoft Azure — wszystkie usługi* w kolumnie **ServiceName.** | *AccessControl,* *CDN,* *Compute,* *Database,* *ServiceBus,* *Storage* |
| MeteredServiceType | Pole **MeteredService,** które zawiera dodatkowe wyjaśnienie użycia usługi platformy Azure. | *ZEWNĘTRZNYCH* |
| Project | Zdefiniowana przez klienta nazwa wystąpienia usługi. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Liczba połączeń usługi Azure Service Bus, które zostały zaaprowizowane i wykorzystywane w danym dniu. | *1,000000 połączeń / 30* dni (jeśli masz indywidualnie zaaprowizowane połączenie w ciągu 30-dniowego miesiąca), 25 połączeń / 30 dni — *używane: 1,0000000* (jeśli masz 25 zapakowanych połączeń Service Bus i wykorzystano 1 w tym dniu) |

## <a name="next-steps"></a>Następne kroki

- [Opis pól w plikach uzgodnień Partner Center opartych na licencjach](license-based-recon-files.md)