---
title: Jak odczytać rozliczenie & pliku Rekonesans
ms.topic: article
ms.date: 06/05/2020
description: Dowiedz się więcej na temat faktury & pliki uzgadniania. Na rachunku są naliczane opłaty za centrum partnerskie w ramach programu, produktów i klientów w danym okresie miesięcznym.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215819"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Zapoznaj się z plikiem rachunku i rozliczeniami — Dowiedz się, jak je znaleźć w centrum partnerskim


**Odpowiednie role**

- Administrator globalny
- Administrator rozliczeń
- Agent administracyjny


**Faktura** to **Podsumowanie wszystkich opłat za centrum partnerskie** (w ramach programu, wszystkich produktów i wszystkich klientów). 

## <a name="invoice-types"></a>Typy faktur

Firma Microsoft będzie wydawać jedną fakturę za wszelkie opłaty za licencje (takie jak Office 365) i opłaty za użycie (na przykład platformę Azure) oraz oddzielne faktury za jednorazowe opłaty (takie jak Azure — RI, Marketplace lub Azure plan).

Na przykład  

**Scenariusz 1 [pojedyncza waluta]**: partner ma zakupy dla ofert 145P i licencji usługi O365,  

- Partner otrzyma jedną fakturę PDF i 2 pliki uzgadniania obejmujące opłaty dla usług O365 i Azure (145p).  

**Scenariusz 2 [pojedyncza waluta]**: partner kupił zakupy na platformie Azure, na rynku i/lub na platformie Azure, a także za pomocą 145p zakupów.

- Partner otrzyma jedną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure (145p). 

- Partner otrzyma kolejną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure RI, Marketplace, plan platformy Azure. 

**Scenariusz 3 [wiele walut]**: partner kupił zakupy dla platformy Azure w walucie DKK i plan platformy Azure w EUR i 145p zakupy w euro.

- Partner otrzyma jedną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure RI w DKK. 

- Partner otrzyma jedną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę Azure plan w EUR. 

- Partner otrzyma kolejną fakturę PDF i plik uzgadniania obejmujący opłaty za usługę 145p w EUR (lub w walucie rozliczeniowej partnera). 

## <a name="find-your-bill"></a>Znajdowanie rachunku 

Fakturę można znaleźć na stronie rozliczenia pulpitu nawigacyjnego w centrum partnerskim. Możesz również znaleźć historię rozliczeń, trendy wydatków i pliki uzgadniania na tej stronie. 

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego. 

2. W menu po lewej stronie wybierz pozycję **rozliczenia**. 

3. Na stronie rozliczenia wybierz fakturę, którą chcesz pobrać. 

Możesz znaleźć link do najnowszej faktury w górnej części strony w obszarze saldo konta na podstawie daty ostatniej faktury. 

Poprzednie faktury można znaleźć w sekcji Historia rozliczeń. Wybierz odpowiedni rok, a następnie wybierz strzałkę listy rozwijanej obok odpowiedniego okresu rozliczeniowego. Wybierz łącze obok pozycji faktury (PDF), aby pobrać fakturę tego okresu. 

## <a name="understanding-invoice-pdf"></a>Informacje o dokumencie PDF faktury 

**Faktury za użycie i opłaty oparte na licencji**: faktury za opłaty za usługi, takie jak Office 365 i Azure, będą dostępne w ciągu dwóch (2) dni od wybranej daty rozliczenia [UTC].  

**Faktury za jednorazowej i opłaty cykliczne**: faktury dla usług takich jak Azure RI, Azure plan i Marketplace będą dostępne nie później niż w ciągu każdego miesiąca.  

Poniżej znajdują się niektóre pola klucza w dokumencie PDF faktury —

**Numer faktury**: unikatowy identyfikator dokumentu faktury wygenerowanego dla odpowiedniego okresu rozliczeniowego. 

**Okres rozliczeniowy**: jest to okres, w którym masz użycie i usługi oparte na licencji. 

**Data faktury**: Data rozliczenia lub Data rocznicy, w której jest generowana faktura co miesiąc. 

**Termin płatności**: Data, o którą należy otrzymać płatność. 

**Opłaty**: kwota należna w walucie rozliczeniowej dla odpowiedniego okresu rozliczeniowego. 

**Kredyty**: kredyty (takie jak SLA) lub korekty zmian wprowadzonych w subskrypcjach (na przykład zwiększenie lub zmniejszenie licencji). 

**Instrukcje dotyczące płatności**: Opis sposobu płacenia faktury w zależności od regionu. Zawsze pamiętaj o uwzględnieniu numeru faktury podczas dokonywania płatności. 

Aby uzyskać szczegółowy opis wszystkich pól w pliku faktury (w tym pól dla opłat jednorazowych), zobacz [pola pliku faktury](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Omówienie plików uzgadniania

 Pliki uzgadniania, które udostępniają szczegółowe dane dotyczące szczegółów opłat, są dostępne do pobrania wraz z DOKUMENTem faktury. Pliki uzgadniania obejmują identyfikatory klientów i identyfikatory subskrypcji, których można użyć do tworzenia faktur klienta. Zapoznaj się z  [tematem jak używać plików uzgadniania](use-the-reconciliation-files.md) , aby uzyskać więcej szczegółów na temat plików rekonesans. 

## <a name="next-steps"></a>Następne kroki

- [Jak używać plików uzgadniania](use-the-reconciliation-files.md)