---
title: Jak odczytać swój rachunek & pliku rekonescji
ms.topic: article
ms.date: 06/05/2020
description: Dowiedz się więcej o plikach uzgodnień & faktur. Na rachunku są Partner Center opłaty za program, produkty i klientów w tym miesięcznym okresie.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf75d847320e901638890bef8077a1656399d2ffc5aaaf984af329784d1de030
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115678241"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Opis pliku rachunku i uzgodnień — dowiedz się, jak znaleźć je w Partner Center


**Odpowiednie role:** Administrator globalny | Administrator rozliczeń | Agent administracyjny


Faktura jest **podsumowaniem wszystkich opłat Partner Center** (w ramach programu, wszystkich produktów i wszystkich klientów).  

## <a name="find-your-bill-and-reconciliation-file"></a>Znajdowanie pliku rachunku i uzgodnień 

Fakturę można znaleźć na stronie Rozliczenia pulpitu nawigacyjnego w Partner Center. Na tej stronie można również znaleźć historię rozliczeń, trendy wydatków i pliki uzgodnień. 

1. Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard/home) 

2. W menu po lewej stronie wybierz pozycję **Rozliczenia.** 

3. Na stronie stanu rozliczeń wybierz plik faktury lub uzgodnienia, aby wyświetlić bardziej szczegółowe informacje. 

Link do najnowszej faktury można znaleźć w górnej części strony w obszarze Saldo konta od daty ostatniej faktury. 

Poprzednie faktury można znaleźć w sekcji Historia rozliczeń. Wybierz odpowiedni rok, a następnie wybierz strzałkę listy rozwijanej obok odpowiedniego okresu rozliczeniowego. Wybierz link obok opcji Faktury (.pdf), aby pobrać fakturę z tego okresu. 

## <a name="invoice-types"></a>Typy faktur

Firma Microsoft wystawi jedną fakturę dla wszelkich opłat opartych na licencjach (takich jak Office 365) i opłat opartych na użyciu (takich jak platforma Azure) oraz oddzielnej faktury za opłaty godzinowe (takie jak RI platformy Azure, witryna Marketplace lub plan platformy Azure).

Na przykład  

**Scenariusz 1 [jedna waluta]**: Partner ma zakupy dla oferty 145P i Office 365 licencji  

- Partner otrzyma jeden plik PDF faktury i dwa pliki uzgodnień obejmujące opłaty za Office 365 i platformę Azure (145p).  

**Scenariusz 2 [jedna waluta]**: Partner ma zakupy dla planu usługi Azure RI, witryny Marketplace i/lub platformy Azure wraz z zakupami 145p.

- Partner otrzyma jeden plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za platformę Azure (145p). 

- Partner otrzyma kolejny plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za wystąpienie zarezerwowane platformy Azure, platformę Marketplace i plan platformy Azure. 

**Scenariusz 3 [Multi-Currency]**: Partner ma zakupy dla usługi Azure RI w systemie DKK i planu platformy Azure w EUR wraz z zakupami w wysokości 145p w EUR.

- Partner otrzyma jeden plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za RI platformy Azure w systemie DKK. 

- Partner otrzyma jeden plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za plan platformy Azure w eur. 

- Partner otrzyma kolejny plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za ofertę 145p w walucie EUR (lub walucie rozliczeniowej partnera). 


## <a name="understanding-invoice-pdf"></a>Omówienie pliku PDF faktury 

**Faktury** za użycie i opłaty na podstawie licencji: Faktury za opłaty za usługi takie jak Office 365 i Azure będą dostępne w ciągu dwóch (2) dni od wybranej daty rozliczeniowej [UTC].  

**Faktury za jednorazową** i cykliczną opłatę: faktury za opłaty za usługi, takie jak azure RI, plan platformy Azure, portal Marketplace, będą dostępne nie później niż ósmego dnia każdego miesiąca.  

Poniżej przedstawiono niektóre z kluczowych pól w dokumencie PDF faktury —

**Numer faktury:** unikatowy identyfikator dokumentu faktury wygenerowanego dla odpowiedniego okresu rozliczeniowego. 

**Okres rozliczeniowy:** jest to okres, w którym masz użycie i usługi oparte na licencjach. 

**Data faktury:** data rozliczeniowa lub data rocznicy, w której faktura jest generowana w każdym miesiącu. 

**Termin płatności:** data, do której należy odebrać płatność. 

**Opłaty:** kwota należności w walucie rozliczeniowej dla odpowiedniego okresu rozliczeniowego. 

**Środki:** środki (takie jak umowa sla)) lub korekty zmian wprowadzonych w subskrypcjach (na przykład zwiększenie lub zmniejszenie liczby licencji). 

**Instrukcje** dotyczące płatności: Opis sposobu płacenia za fakturę w zależności od regionu. Zawsze pamiętaj, aby podczas dokonywania płatności dołączyć numer faktury. 

Aby uzyskać szczegółowy opis wszystkich pól w pliku faktury (w tym pól opłat godzinowych), zobacz [Pola pliku faktury](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Opis plików uzgodnień

 Pliki uzgodnień, które zawierają szczegółowe/szczegółowe informacje o opłatach, są dostępne do pobrania wraz z dokumentem PDF faktury. Pliki uzgodnień obejmują identyfikatory klientów i identyfikatory subskrypcji, których można użyć do tworzenia faktur klientów. Aby uzyskać więcej informacji na temat plików uzgodnień, [zobacz Jak używać plików uzgodnień](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Następne kroki

- [Jak używać plików uzgodnień](use-the-reconciliation-files.md)