---
title: Regionalne podatki i opłaty za usługę PSTN
description: Jako partner pakietu Office 365, który przetwarza Microsoft 365 produkty głosowe, mogą podlegać regionalne podatki, opłaty lub wymagania prawne dotyczące usług PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 411932923e6bd35732e64521abe567f40f7499e9
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441493"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Podatki regionalne, regulacje dla usług publicznego przełączania sieci telefonicznych (PTSN)

**Odpowiednie role**

- Administrator globalny
- Administrator użytkowników
- Agent administracyjny

Publiczne przełączane usługi telefoniczne (PSTN) w niektórych jurysdykcjach mogą podlegać specjalnym wymaganiom podatkowym i prawnym, które mogą mieć wpływ na kolejność i fakturowanie partnera. W Stany Zjednoczone, w tym Portoryko, usługi PSTN, takie jak konferencje audio, plany wywoływania i kredyty komunikacyjne, podlegają specjalnym wymaganiom podatkowym i obowiązującym w zakresie przepisów. W Stany Zjednoczone i Portoryko, usługi firmy Microsoft cen PSTN jako podatki włącznie.  Unikatowe podatki i regulacje dotyczące sieci PSTN wpłyną na partnerów pakietu Office 365, w których są naliczane Microsoft 365 produkty głosowe.  Jeśli partner oznacza cenę usługi PSTN firmy Microsoft, może być odpowiedzialna za obliczanie i ponowne przeprowadzenie opłat za korzystanie z sieci PSTN.

## <a name="partner-recommendations"></a>Zalecenia dotyczące partnerów

Zapoznaj się z podatkiem i z tytułu prawnego, aby zrozumieć odpowiedzialność organizacji dotyczącą regulacji, podatków i opłat za usługi PSTN oraz inne potencjalne zobowiązania.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Prezentacja faktury i plik uzgadniania partnera

Faktury dostawcy usług kryptograficznych i pliki uzgadniania CSP w Stany Zjednoczone, Portoryko i Kanadzie, które obejmują usługę Skype dla firm PSTN i Microsoft 365 usługi głosowe, będą udostępniać osobne elementy wiersza dla składników PSTN i innych niż PSTN.

Ponadto faktury dostawcy CSP będą wyświetlać następujący przypis dolny:

* Wyświetlana cena to opłata za konferencje audio i wywoływanie usług planu.  Wszelkie stosowane podatki transakcyjne są obciążane wyłącznie ilością pokazaną z wyjątkiem sprzedaży dokonywanej w ramach Stany Zjednoczone.  W Stanach Zjednoczonych wyświetlana cena jest podatkiem włącznie, ponieważ obejmuje ona opłaty za plan wywoływania i usługi konferencji audio oraz opłaty za podatki i opłaty, które są wymagane do naliczania opłat.  Konferencje audio i usługi rozmów telefonicznych są poddane autoryzacji przez stowarzyszone firmy Microsoft w celu ich udostępnienia.  Zobacz [Licencjonowanie zbiorowe firmy Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247), aby uzyskać więcej szczegółów.

## <a name="reconciliation-file-example"></a>Przykład pliku uzgodnienia

Pakiet Office 365 Enterprise E5 przedstawia plik uzgadniania jako dwa elementy wierszy o identycznych nazwach i identycznych identyfikatorach, ale każdy element wiersza ma unikatową cenę jednostkową (przykład: $28,40 i $2,00). Spowoduje to oddzielenie składnika konferencji usługi Skype dla firm w ramach oferty pakietu Office 365, dzięki czemu można prawidłowo zastosować podatki.

**Przykład #1 uzgadniania partnera (Wybierz kolumny):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Opłata za cykl   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Opłata za cykl   |2,00   |

**Przykład uzgadniania partnera #2**

Microsoft 365 Business głosu dostępnego w Kanadzie ma dodatkowe składniki podlegające opodatkowaniu PSTN, które są skonsolidowane na fakturze dostawcy CSP (podobnie jak w przypadku pakietu Office 365 E5, prezentowane są dwa elementy wiersza, jeden dla składników PSTN, a drugi dla składników innych niż PSTN).  Plik uzgadniania CSP dla Microsoft 365 Business głosu będzie wyświetlał wszystkie składniki podlegające opodatkowaniu PSTN osobno (poszczególne składniki PSTN nie będą konsolidowane w programie). Narzędzie CSV lub interfejs API.  Suma informacji o zamówieniu i kwota rozliczana dla klientów znalezionych w pliku uzgadniania będzie zgodna z fakturą dostawcy usług kryptograficznych.

## <a name="additional-resources"></a>Dodatkowe zasoby
Aby uzyskać więcej informacji, odwiedź witrynę [Microsoft 365 dla partnerów](https://www.microsoft.com/microsoft-365/partners/) .

