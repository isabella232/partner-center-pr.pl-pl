---
title: Zarządzanie listą klientów
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Rekordy klientów są jednymi z najważniejszych zasobów informacyjnych. Dowiedz się, jak wyświetlać, wyszukiwać, aktualizować & eksportować informacje na Partner Center klientów.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: df0f72deb14eac6d75f8579f7099ab3c6b6a2905
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837275"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Zarządzanie listą klientów — wyszukiwanie, aktualizowanie lub eksportowanie klientów w Partner Center

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator | Administrator globalny

Rekordy klientów są jednymi z najważniejszych zasobów informacyjnych w Partner Center. Bazę danych kont klientów można przeszukiwać, eksportować całą bazę danych klienta lub eksportować podzbiór do formatu pliku wartości rozdzielanych przecinkami (Excel zgodny z programem .csv). Możesz również wyeksportować informacje o subskrypcjach klienta do pliku .csv klienta.

Dzienniki aktywności zapewniają również klientom dane dotyczące transakcji i akcji zarządzania, które można eksportować. Aby uzyskać więcej informacji, zobacz [Wyświetlanie dzienników aktywności klientów.](activity-logs.md)

## <a name="search-for-a-customer"></a>Wyszukiwanie klienta

1. Z menu **Partner Center** wybierz pozycję **Klienci.**
2. Aby wyszukać klienta, wprowadź nazwę klienta lub nazwę domeny w polu wyszukiwania.
3. Wybierz strzałkę **w dół** na końcu wiersza klienta, aby wyświetlić jego identyfikator Microsoft oraz skojarzone z nim szybkie linki do subskrypcji i usług.

## <a name="update-a-customers-company-name"></a>Aktualizowanie nazwy firmy klienta

Z menu **Partner Center** wybierz pozycję **Klienci.**
2. Aby wyszukać klienta, wprowadź nazwę klienta lub nazwę domeny w polu wyszukiwania.
3. Wybierz strzałkę **w dół** na końcu wiersza klienta, aby wyświetlić jego identyfikator Microsoft oraz skojarzone z nim szybkie linki do subskrypcji i usług.
4. W obszarze Informacje **o odbiorcy** faktury zaktualizuj nazwę firmy. Po zapisaniu nowej wartości zostanie ona odzwierciedlona na liście klientów. Spowoduje to tylko zmianę nazwy firmy dla odbiorcy faktury i wartości listy klientów. Nie zostanie ona odzwierciedlona w żadnym innym miejscu.

## <a name="export-your-customer-list"></a>Eksportowanie listy klientów

1. Z menu **Partner Center** wybierz pozycję **Klienci.**
2. Wybierz pozycję **Eksportuj klientów.**

   Partner Center konwertuje pełną listę klientów na plik .csv i przekaże go do domyślnego folderu pobierania na komputerze. Można również eksportować podzbiory danych klientów. Kolumny danych są następujące:

   - **Identyfikator firmy Microsoft;**
   - **Nazwa firmy;**
   - **Nazwa domeny podstawowej;**
   - **Relacja**— relacja biznesowa partnera z każdym wymienionym klientem.

    Domyślnie program Partner Center eksportuje całą listę klientów, niezależnie od długości. Możesz również przeszukać listę klientów według nazwy firmy lub domeny i wyeksportować ten podzbiór danych.

3. Jeśli jesteś dostawcą pośrednim, możesz filtrować listę klientów według odsprzedawcy pośredniego. Wybierz **pozycję Filtruj według odsprzedawcy** pośredniego z listy, a następnie wybierz odsprzedawcę.


## <a name="export-customer-subscription-information"></a>Eksportowanie informacji o subskrypcji klienta

1. Z menu **Partner Center** wybierz pozycję **Klienci.**

2. Wybierz **nazwę firmy dla** dowolnego klienta. Zostanie otwarta strona **Subskrypcje** klienta z pełną listą subskrypcji produktów.

3. Wybierz **pozycję Eksportuj subskrypcje.** Partner Center konwertuje dane subskrypcji klienta na plik .csv i przekaże je do domyślnego folderu pobierania na komputerze. Kolumny danych są następujące:
   - **Identyfikator subskrypcji;**
   - **Subskrypcja**— nazwa produktu dla subskrypcji;
   - **Ilość —** liczba zakupionych licencji;
   - **Stan**;
   - **Odsprzedawca**— identyfikator odsprzedawcy, który jest właścicielem subskrypcji i zarządza jej subskrypcją.

> [!NOTE]  
> Aby uzyskać więcej informacji na temat zarządzania subskrypcjami, zobacz [Subskrypcje klientów](customer-subscriptions.md).
