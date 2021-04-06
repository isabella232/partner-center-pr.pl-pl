---
title: Pliki uzgodnień na podstawie licencji
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informacje o sposobie odczytywania plików uzgadniania opartych na licencjach w centrum partnerskim. W tym artykule opisano znaczenie każdego pola w pliku Rekonesans opartego na licencji.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4c311de4a504785e15cefc7a93f1ee3da396ea7d
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441289"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Informacje o polach w plikach uzgodnień opartych na licencji Centrum partnerskiego

**Dotyczy**

- Centrum partnerskie Microsoft Cloud for US Government

**Odpowiednie role**

- Administrator globalny
- Administrator zarządzania użytkownikami
- Administrator rozliczeń
- Agent administracyjny

Aby uzgodnić zmiany z zamówieniami klienta, porównaj **Syndication_Partner_Subscription_Number** z pliku uzgadniania z **identyfikatorem subskrypcji** z Centrum partnerskiego.

## <a name="fields-in-license-based-reconciliation-files"></a>Pola w plikach uzgodnień opartych na licencji

| Kolumna | Opis | Wartość przykładowa |
| ------ | ----------- | ------------ |
| PartnerId | Unikatowy identyfikator w formacie identyfikatora GUID dla określonej jednostki rozliczania. Niewymagane do uzgodnienia. Taka sama we wszystkich wierszach. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Unikatowy identyfikator firmy Microsoft dla klienta w formacie identyfikatora GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nazwa organizacji klienta zgłoszona w centrum partnerskim. *Bardzo ważne pole umożliwiające uzgodnienie faktury z informacjami o systemie.* | *Testowanie klienta A* |
| MpnId | Identyfikator MPN partnera dostawcy usług kryptograficznych. Zobacz [, jak itemize według partnera](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | MPN identyfikator odsprzedawcy rekordu dla subskrypcji.  |
| OrderId (Identyfikator zamówienia) | Unikatowy identyfikator zamówienia na platformie rozliczeń firmy Microsoft. Może być przydatne do identyfikowania zamówienia podczas kontaktowania się z pomocą techniczną. Nieużywany do uzgadniania. | *566890604832738111* |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeń firmy Microsoft. Może być przydatne do identyfikowania subskrypcji podczas kontaktowania się z pomocą techniczną. Nieużywany do uzgadniania. *Ta wartość nie jest taka sama jak **Identyfikator subskrypcji** w konsoli administracyjnej partnera. Zamiast tego zobacz **SyndicationPartnerSubscriptionNumber** .* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Unikatowy identyfikator dla subskrypcji. Klient może mieć wiele subskrypcji dla tego samego planu. Ta kolumna jest ważna w przypadku analizy plików uzgadniania. To pole jest mapowane na **Identyfikator subskrypcji** w konsoli administracyjnej partnera. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Unikatowy identyfikator oferty. Identyfikator oferty standardowej, zgodnie z definicją w cenniku. *Ta wartość nie jest zgodna z **identyfikatorem oferty** z cennika. Zamiast tego zobacz **DurableOfferID** .* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Unikatowy identyfikator oferty trwałej, zgodnie z definicją w cenniku. *Ta wartość jest zgodna z **identyfikatorem oferty** z cennika.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Nazwa oferty usługi zakupionej przez klienta zgodnie z definicją w cenniku. | *Microsoft Office 365 (plan E3)* |
| SubscriptionStartDate | Data rozpoczęcia subskrypcji. Godzina to zawsze początek dnia, 0:00. To pole jest ustawione na dzień po przesłaniu zamówienia. Używany z **SubscriptionEndDate** do określenia: Jeśli klient nadal znajduje się w pierwszym roku subskrypcji lub odnowieniu subskrypcji przez następny rok. | *2/1/2019 0:00* |
| SubscriptionEndDate | Data zakończenia subskrypcji. Godzina to zawsze początek dnia, 0:00. *12 miesięcy i **x** dni po dacie rozpoczęcia* do dopasowania do daty rozliczenia partnera lub *12 miesięcy od daty odnowienia*. Po odnowieniu ceny są aktualizowane na bieżącą listę cenową. Przed automatycznym odnowieniem może być wymagana komunikacja z klientem. | *2/1/2019 0:00* |
| ChargeStartDate | Początkowy dzień opłat. Godzina to zawsze początek dnia, 0:00. Służy do obliczania opłat dziennych (opłaty *pro rata* ), gdy klient zmieni numery licencji. | *2/1/2019 0:00* |
| ChargeEndDate | Dzień końcowy opłat. Czas jest zawsze koniec dnia, 23:59. Służy do obliczania opłat dziennych (opłaty *pro rata* ), gdy klient zmieni numery licencji. | *2/28/2019 23:59* |
| ChargeType | [Typ opłaty](recon-file-charge-types.md) lub korekty. | Zobacz [typy opłat](recon-file-charge-types.md). |
| UnitPrice | Cena za licencję publikowana w cenniku w momencie zakupu. Upewnij się, że są one zgodne z informacjami przechowywanymi w systemie rozliczeniowym podczas uzgadniania. | *6,82* |
| Liczba | Liczba licencji. Upewnij się, że są one zgodne z informacjami przechowywanymi w systemie rozliczeniowym podczas uzgadniania. | *2* |
| Kwota | Łączna cena za ilość. Służy do sprawdzania, czy Obliczanie kwoty jest zgodne z sposobem obliczania tej wartości dla klientów. | *13,32* |
| TotalOtherDiscount | Kwota rabatu zastosowana do tych opłat. Licencje na produkty dołączone do kompetencji lub map lub nowe subskrypcje kwalifikujące się do bodźca będą również zawierać kwotę rabatu w tej kolumnie. | *2,32* |
| Suma częściowa | Suma przed podatkiem. Sprawdza, czy Suma częściowa jest zgodna z oczekiwaną sumą w przypadku rabatu. | *11* |
| Podatek | Opłata za podatek. Na podstawie reguł podatkowych i określonych okoliczności na rynku. | *0* |
| TotalForCustomer | Suma po opodatkowaniu. Sprawdza, czy opłaty są naliczane na podstawie faktury. | *11* |
| Waluta | Typ waluty. Każda jednostka rozliczeniowa ma tylko jedną walutę. Sprawdź, czy pasuje do pierwszej faktury. Sprawdź ponownie po aktualizacji wszystkich głównych platform rozliczeń. | *EUR* |
| DomainName | Nazwa domeny klienta. To pole może pojawić się puste do momentu drugiego okresu rozliczeniowego. *Nie używaj tego pola jako unikatowego identyfikatora klienta. Klient/partner może zaktualizować znaczącym lub domenę domyślną za pomocą portalu pakietu Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Pseudonim subskrypcji. Jeśli nie określono pseudonimu, centrum partnerskie będzie korzystać z **oferty**. | *PROJECT ONLINE* |
| SubscriptionDescription | Nazwa oferty usługi zakupionej przez klienta zgodnie z definicją w cenniku. (To jest identyczne pole, aby **zaoferowaćname**). | *PROJECT ONLINE PREMIUM BEZ PROGRAMU PROJECT CLIENT* |
| BillingCycleType | Częstotliwość jednorazowego rozliczania.| *Raz na miesiąc* |