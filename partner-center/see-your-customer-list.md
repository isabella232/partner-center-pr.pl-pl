---
title: Zarządzanie listą klientów
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Rekordy klientów należą do najważniejszych zasobów informacyjnych. Dowiedz się, jak wyświetlać, wyszukiwać, aktualizować & eksportować informacje na Partner Center klientów.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854506"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Zarządzanie listą klientów — wyszukiwanie, aktualizowanie lub eksportowanie klientów w Partner Center

**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government

**Odpowiednie role:** Administrator | Administrator globalny

Rekordy klientów są jednymi z najważniejszych zasobów informacyjnych w Partner Center. Możesz przeszukać bazę danych kont klientów, wyeksportować całą bazę danych klienta lub wyeksportować podzbiór do formatu pliku wartości rozdzielanych przecinkami (CSV) zgodnego z programem Excel. Możesz również wyeksportować informacje o subskrypcjach klienta do pliku CSV.

Dzienniki aktywności zapewniają również klientom dane dotyczące transakcji i akcji zarządzania, które można eksportować. Aby uzyskać więcej informacji, zobacz [Wyświetlanie dzienników aktywności klientów.](activity-logs.md)

## <a name="search-for-a-customer"></a>Wyszukiwanie klienta

1. Z menu **Partner Center** wybierz pozycję **Klienci.**
2. Aby wyszukać klienta, wprowadź nazwę klienta lub nazwę domeny w polu wyszukiwania.
3. Wybierz strzałkę **w dół** na końcu wiersza klienta, aby wyświetlić jego identyfikator Microsoft oraz skojarzone z nim szybkie linki do subskrypcji i usług.

## <a name="update-a-customers-company-name"></a>Aktualizowanie nazwy firmy klienta

Z menu **Partner Center** wybierz pozycję **Klienci.**
2. Aby wyszukać klienta, wprowadź nazwę klienta lub nazwę domeny w polu wyszukiwania.
3. Wybierz strzałkę **w dół** na końcu wiersza klienta, aby wyświetlić jego identyfikator Microsoft oraz skojarzone z nim szybkie linki do subskrypcji i usług.
4. W obszarze informacje **o odbiorcy** faktury zaktualizuj nazwę firmy. Po zapisaniu nowej wartości zostanie ona odzwierciedlona na liście klientów. Spowoduje to tylko zmianę nazwy firmy dla odbiorcy faktury i wartości listy klientów. Nie zostaną one odzwierciedlone w żadnym innym miejscu.

## <a name="export-your-customer-list"></a>Eksportowanie listy klientów

1. Z menu **Partner Center** wybierz pozycję **Klienci.**
2. Wybierz pozycję **Eksportuj klientów.**

   Partner Center konwertuje pełną listę klientów na plik CSV i przekaże ją do domyślnego folderu pobierania na komputerze. Można również eksportować podzbiory danych klientów. Kolumny danych obejmują następujące elementy:

   - **Identyfikator Microsoft;**
   - **Nazwa firmy;**
   - **Nazwa domeny podstawowej;**
   - **Relacja**— relacja biznesowa partnera z każdym klientem na liście.

    Domyślnie program Partner Center eksportuje całą listę klientów, niezależnie od długości. Możesz również przeszukać listę klientów według nazwy firmy lub domeny i wyeksportować ten podzbiór danych.

3. Jeśli jesteś dostawcą pośrednim, możesz filtrować listę klientów według odsprzedawcy pośredniego. Wybierz **pozycję Filtruj według odsprzedawcy** pośredniego z listy, a następnie wybierz odsprzedawcę.


## <a name="export-customer-subscription-information"></a>Eksportowanie informacji o subskrypcji klienta

1. Z menu **Partner Center** wybierz pozycję **Klienci.**

2. Wybierz nazwę **firmy dla** dowolnego klienta. Zostanie otwarta strona **Subskrypcje** klienta z pełną listą subskrypcji produktów.

3. Wybierz **pozycję Eksportuj subskrypcje.** Partner Center dane subskrypcji klienta na plik CSV i przekazanie ich do domyślnego folderu pobierania na komputerze. Kolumny danych są następujące:
   - **Identyfikator subskrypcji;**
   - **Subskrypcja**— nazwa produktu dla subskrypcji;
   - **Ilość —** liczba zakupionych licencji;
   - **Stan**;
   - **Odsprzedawca**— identyfikator odsprzedawcy, który jest właścicielem subskrypcji i zarządza jej subskrypcją.

> [!NOTE]  
> Aby uzyskać więcej informacji na temat zarządzania subskrypcjami, zobacz [Subskrypcje klientów](customer-subscriptions.md).
