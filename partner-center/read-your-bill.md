---
title: Opis pliku rachunku i uzgodnień
ms.topic: article
ms.date: 09/27/2021
description: Dowiedz się więcej o plikach uzgodnień & faktur. Na rachunku są Partner Center opłaty za program, produkty i klientów w tym miesięcznym okresie.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2004734a250a23be3037342ecc01f5e6bf7b51b0
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070194"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Opis pliku rachunku i uzgodnień — dowiedz się, jak znaleźć je w Partner Center

**Odpowiednie role:** Administrator globalny | Administrator rozliczeń | Agent administracyjny

Faktura jest podsumowaniem wszystkich opłat Partner Center w ramach programu, wszystkich produktów i wszystkich klientów.

## <a name="find-your-bill-and-reconciliation-file"></a>Znajdowanie pliku rachunku i uzgodnień

Fakturę można znaleźć na stronie Rozliczenia pulpitu nawigacyjnego w Partner Center. Na tej stronie można również znaleźć historię rozliczeń, trendy wydatków i pliki uzgodnień.

> [!NOTE]
> Interfejs Partner Center wersji zapoznawczej zapewnia bardziej wydajne i wydajne środowisko użytkownika za pośrednictwem logicznie pogrupowanych obszarów roboczych. Aby dowiedzieć się więcej na temat interfejsu obszarów roboczych i sposobu jego włączanie, zobacz Getting around Partner Center (Poruszanie [się po Partner Center).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Widok obszarów roboczych](#tab/workspaces-view)

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego.

2. Wybierz **kafelek Rozliczenia.**

3. Wybierz fakturę lub plik uzgodnień, aby wyświetlić bardziej szczegółowe informacje.

Link do najnowszej faktury można znaleźć w górnej części strony w obszarze Saldo konta od daty ostatniej faktury.

Poprzednie faktury można znaleźć w sekcji Historia rozliczeń. Wybierz odpowiedni rok, a następnie wybierz strzałkę listy rozwijanej obok odpowiedniego okresu rozliczeniowego. Wybierz link obok opcji Faktury (.pdf), aby pobrać fakturę dla tego okresu.

#### <a name="current-view"></a>[Bieżący widok](#tab/current-view)

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/home) Centrum partnerskiego.

2. W menu po lewej stronie wybierz pozycję **Rozliczenia.**

3. Na stronie stanu rozliczeń wybierz plik faktury lub uzgodnienia, aby wyświetlić bardziej szczegółowe informacje.

Link do najnowszej faktury można znaleźć w górnej części strony w obszarze Saldo konta od daty ostatniej faktury.

Poprzednie faktury można znaleźć w sekcji Historia rozliczeń. Wybierz odpowiedni rok, a następnie wybierz strzałkę listy rozwijanej obok odpowiedniego okresu rozliczeniowego. Wybierz link obok opcji Faktury (.pdf), aby pobrać fakturę dla tego okresu.

* * *

## <a name="invoice-types"></a>Typy faktur

Firma Microsoft wystawi jedną fakturę dla wszelkich opłat opartych na licencjach (takich jak Office 365) i opłat opartych na użyciu (takich jak platforma Azure) oraz oddzielnej faktury za opłaty godzinowe (takie jak RI platformy Azure, witryna Marketplace lub plan platformy Azure).

Na przykład  

**Scenariusz 1 [jedna waluta]**: Partner ma zakupy dla oferty 145P i Office 365 licencji  

- Partner otrzyma jeden plik PDF faktury i dwa pliki uzgodnień obejmujące opłaty za Office 365 platformy Azure (145p).  

**Scenariusz 2 [jedna waluta]**: Partner ma zakupy dla planu usługi Azure RI, witryny Marketplace i/lub platformy Azure wraz z zakupami w wysokości 145p.

- Partner otrzyma jeden plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za platformę Azure (145p). 

- Partner otrzyma kolejny plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za wystąpienie zarezerwowane platformy Azure, platformę Marketplace i plan platformy Azure. 

**Scenariusz 3 [wiele walut]:** Partner ma zakupy dla usługi Azure RI w systemie DKK i planu platformy Azure w EUR wraz z zakupami w wysokości 145p w EUR.

- Partner otrzyma jeden plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za RI platformy Azure w systemie DKK. 

- Partner otrzyma jeden plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za plan platformy Azure w eur. 

- Partner otrzyma kolejny plik PDF faktury i jeden plik uzgodnień obejmujący opłaty za ofertę 145p w eur (lub walucie rozliczeniowej partnera). 

## <a name="understanding-invoice-pdf"></a>Omówienie pliku PDF faktury 

**Faktury za** użycie i opłaty na podstawie licencji: faktury za opłaty za usługi takie jak Office 365 i Azure będą dostępne w ciągu dwóch (2) dni od wybranej daty rozliczeniowej [UTC].  

**Faktury za jednorazową** i cykliczną opłatę: faktury za opłaty za usługi, takie jak azure RI, plan platformy Azure i portal Marketplace, będą dostępne nie później niż ósmą część każdego miesiąca.  

Poniżej przedstawiono niektóre z kluczowych pól w dokumencie PDF faktury —

**Numer faktury:** unikatowy identyfikator dokumentu faktury wygenerowanego dla odpowiedniego okresu rozliczeniowego. 

**Okres rozliczeniowy:** jest to okres, w którym masz użycie i usługi oparte na licencjach. 

**Data faktury:** data rozliczeniowa lub data rocznicy, w której faktura jest generowana co miesiąc. 

**Termin płatności:** data, do której należy odebrać płatność. 

**Opłaty:** kwota należności w walucie rozliczeniowej dla odpowiedniego okresu rozliczeniowego. 

**Środki:** środki (takie jak umowa sla)) lub korekty zmian wprowadzonych w subskrypcjach (na przykład zwiększenie lub zmniejszenie liczby licencji). 

**Instrukcje** dotyczące płatności: Opis sposobu płacenia za fakturę w zależności od regionu. Zawsze pamiętaj, aby podczas dokonywania płatności dołączyć numer faktury. 

Aby uzyskać szczegółowy opis wszystkich pól w pliku faktury (w tym pól opłat godzinowych), zobacz [Pola pliku faktury](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Opis plików uzgodnień

 Pliki uzgodnień, które zawierają szczegółowe/szczegółowe informacje o opłatach, są dostępne do pobrania wraz z dokumentem PDF faktury. Pliki uzgodnień obejmują identyfikatory klientów i identyfikatory subskrypcji, których można użyć do tworzenia faktur klientów. Aby uzyskać więcej informacji na temat plików uzgodnień, [zobacz Jak używać plików uzgodnień](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Następne kroki

- [Jak używać plików uzgodnień](use-the-reconciliation-files.md)