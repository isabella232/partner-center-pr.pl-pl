---
title: Pliki uzgodnień na podstawie licencji
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Dowiedz się, jak odczytywać pliki uzgodnień oparte na licencjach w Partner Center. W tym artykule wyjaśniono znaczenie każdego pola w pliku rekonescji opartym na licencjach.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ebbd34e8de8db845b06b8d75bc17e88612e8477
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837360"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Opis pól w Partner Center uzgadniania na podstawie licencji

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Administrator rozliczeń | Agent administracyjny

Aby uzgodnić zmiany z zamówieniami klienta, porównaj Syndication_Partner_Subscription_Number z pliku uzgodnień z **identyfikatorem subskrypcji** z Partner Center. 

## <a name="fields-in-license-based-reconciliation-files"></a>Pola w plikach uzgodnień opartych na licencjach

| Kolumna | Opis | Wartość przykładowa |
| ------ | ----------- | ------------ |
| PartnerId | Unikatowy identyfikator w formacie identyfikatora GUID dla określonej jednostki rozliczeniowej. Nie jest wymagane do uzgadniania. Tak samo we wszystkich wierszach. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Unikatowy identyfikator firmy Microsoft dla klienta w formacie identyfikatora GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nazwa organizacji klienta zgłoszona w Partner Center. *Bardzo ważne pole do uzgadniania faktury z informacjami o systemie.* | *Testowanie klienta A* |
| MpnId | Identyfikator MPN partnera CSP. Zobacz, [jak elementować według partnera](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | Identyfikator MPN odsprzedawcy rekordu dla subskrypcji.  |
| OrderId (Identyfikator zamówienia) | Unikatowy identyfikator zamówienia na platformie rozliczeniowej firmy Microsoft. Może być przydatna do zidentyfikowania zamówienia podczas kontaktowania się z pomocą techniczną. Nie są używane do uzgadniania. | *566890604832738111* |
| SubscriptionId | Unikatowy identyfikator subskrypcji na platformie rozliczeniowej firmy Microsoft. Może być przydatna do zidentyfikowania subskrypcji podczas kontaktowania się z pomocą techniczną. Nie są używane do uzgadniania. *Ta wartość nie jest taka sama jak **identyfikator subskrypcji w** konsoli administracyjnej partnera. Zamiast tego **zobacz SyndicationPartnerSubscriptionNumber.*** | *usCBMgAAAAAAAAIAA* |
| SyndykacjaPartnerSubscriptionNumber | Unikatowy identyfikator subskrypcji. Klient może mieć wiele subskrypcji dla tego samego planu. Ta kolumna jest ważna w przypadku analizy pliku uzgodnień. To pole jest mapowe **na identyfikator subskrypcji** w konsoli administracyjnej partnera. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Unikatowy identyfikator oferty. Standardowy identyfikator oferty, zgodnie z definicją w cenniku. *Ta wartość nie jest dopasowana do **identyfikatora oferty** z cennika. Zamiast tego **zobacz DurableOfferID.*** | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Unikatowy trwały identyfikator oferty, zgodnie z definicją w cenniku. *Ta wartość odpowiada **identyfikatorowi oferty** z cennika.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Nazwa oferty usługi zakupionej przez klienta, zgodnie z definicją w cenniku. | *Microsoft Office 365 (plan E3)* |
| SubscriptionStartDate | Data rozpoczęcia subskrypcji w czasie UTC. Godzina to zawsze początek dnia, 0:00. To pole jest ustawione na dzień po przesłaniu zamówienia. Używana z **subskrypcjąEndDate** w celu określenia, czy klient nadal znajduje się w pierwszym roku subskrypcji, czy subskrypcja została odnowiona na następny rok. | *2/1/2019 0:00* |
| SubscriptionEndDate | Data zakończenia subskrypcji w czasie UTC. Godzina to zawsze początek dnia, 0:00. *12 miesięcy plus x **dni*** po dacie rozpoczęcia w celu dostosowania do daty rozliczeniowej partnera lub *12 miesięcy* od daty odnowienia. Po odnowieniu ceny są aktualizowane do bieżącego cennika. Komunikacja z klientem może być wymagana przed automatycznym odnawianiem. | *2/1/2019 0:00* |
| ChargeStartDate | Dzień rozpoczęcia opłat. Godzina to zawsze początek dnia, 0:00. Służy do obliczania opłat dziennych *(proporcjonalnie do opłat),* gdy klient zmienia numery licencji. | *2/1/2019 0:00* |
| ChargeEndDate | Koniec dnia opłat. Czas to zawsze koniec dnia, 23:59. Służy do obliczania opłat dziennych *(proporcjonalnie do opłat),* gdy klient zmienia numery licencji. | *2/28/2019 23:59* |
| ChargeType | Typ [opłaty lub](recon-file-charge-types.md) korekty. | Zobacz [typy opłat.](recon-file-charge-types.md) |
| UnitPrice | Cena za licencję opublikowana w cenniku w momencie zakupu. Upewnij się, że jest to informacja przechowywana w systemie rozliczeniowym podczas uzgadniania. | *6.82* |
| Liczba | Liczba licencji. Upewnij się, że jest to informacja przechowywana w systemie rozliczeniowym podczas uzgadniania. | *2* |
| Kwota | Łączna cena za ilość. Służy do sprawdzania, czy obliczenie kwoty jest takie, jak obliczasz tę wartość dla klientów. | *13.32* |
| TotalOtherDiscount | Kwota rabatu zastosowana do tych opłat. Licencje produktów objęte kompetencją lub MAPS albo nowe subskrypcje kwalifikujące się do zachęty będą również zawierać kwotę rabatu w tej kolumnie. | *2.32* |
| Suma częściowa | Suma przed opodatkowaniem. Sprawdza, czy suma częściowa odpowiada oczekiwanej sumie w przypadku rabatu. | *11* |
| Podatek | Kwota podatku. Na podstawie reguł podatkowych obowiązujących na rynku i określonych okoliczności. | *0* |
| TotalForCustomer | Suma po opodatkowaniu. Sprawdza, czy na fakturze nie są naliczane opłaty podatkowe. | *11* |
| Waluta | Typ waluty. Każda jednostka rozliczeniowa ma tylko jedną walutę. Sprawdź, czy odpowiada pierwszej fakturze. Sprawdź ponownie po każdej istotnej aktualizacji platformy rozliczeniowej. | *EUR* |
| DomainName | Nazwa domeny klienta. To pole może być puste do czasu drugiego cyklu rozliczeniowego. *Nie używaj tego pola jako unikatowego identyfikatora klienta. Klient/partner może zaktualizować domenę vanity lub domyślną za pośrednictwem Office 365 portal.* | *example.onmicrosoft.com* |
| SubscriptionName | Pseudonim subskrypcji. Jeśli pseudonim nie zostanie określony, Partner Center użyje **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Nazwa oferty usług zakupionej przez klienta, zgodnie z definicją w cenniku. (Jest to pole identyczne z **OfferName**). | *PROJECT ONLINE PREMIUM BEZ KLIENTA PROJEKTU* |
| BillingCycleType | Częstotliwość rozliczania godzinowego.| *Raz na miesiąc* |
