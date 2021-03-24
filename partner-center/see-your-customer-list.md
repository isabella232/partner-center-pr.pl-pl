---
title: Zarządzanie listą klientów
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Rekordy klientów są wśród najważniejszych zasobów informacji. Dowiedz się, jak wyświetlać, przeszukiwać, aktualizować i & eksportować informacje na liście klientów w centrum partnerskim.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ab5b3ef871aa8a969e8da48e2cb6f4cfebf4c6
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028336"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Zarządzanie listą klientów — wyszukiwanie, aktualizowanie i eksportowanie klientów w centrum partnerskim

**Dotyczy**

- Centrum partnerskie w chmurze firmy Microsoft dla instytucji rządowych

Rekordy klientów znajdują się wśród najważniejszych zasobów informacji w centrum partnerskim. Bazę danych kont klientów można wyszukać, wyeksportować całą bazę danych klienta lub wyeksportować podzestaw do formatu pliku wartości rozdzielanych przecinkami (CSV) zgodnego z programem Excel. Możesz również wyeksportować informacje o subskrypcjach klienta do pliku CSV.

Dzienniki aktywności udostępniają również dane możliwe do eksportu w przypadku transakcji i akcji zarządzania dla klientów. Aby uzyskać więcej informacji, zobacz [Wyświetlanie dzienników aktywności klienta](activity-logs.md).

## <a name="search-for-a-customer"></a>Wyszukaj klienta

1. W menu **Centrum partnerskiego** wybierz pozycję **Customers**.
2. Aby wyszukać klienta, wprowadź nazwę klienta lub nazwę domeny w polu wyszukiwania.
3. Wybierz **strzałkę w dół** znajdującą się na końcu wiersza klienta, aby wyświetlić identyfikator firmy Microsoft i powiązane z nimi subskrypcje i usługi.

## <a name="update-a-customers-company-name"></a>Aktualizowanie nazwy firmy klienta

W menu **Centrum partnerskiego** wybierz pozycję **Customers**.
2. Aby wyszukać klienta, wprowadź nazwę klienta lub nazwę domeny w polu wyszukiwania.
3. Wybierz **strzałkę w dół** znajdującą się na końcu wiersza klienta, aby wyświetlić identyfikator firmy Microsoft i powiązane z nimi subskrypcje i usługi.
4. W obszarze informacje o **rozliczaniu** klienta należy zaktualizować nazwę firmy. Po zapisaniu nowej wartości będzie ona widoczna na liście Customer (klient). Spowoduje to zmianę nazwy firmy dla rachunku i wartości z listy klientów. Nie będzie on widoczny w żadnym miejscu.

## <a name="export-your-customer-list"></a>Eksportowanie listy klientów

1. W menu **Centrum partnerskiego** wybierz pozycję **Customers**.
2. Wybierz pozycję **Eksportuj klientów**.

   Centrum partnerskie konwertuje kompletną listę klientów na plik CSV i przekazuje ją do domyślnego folderu pobierania na komputerze. Można również eksportować podzbiory danych klienta. Kolumny danych obejmują następujące elementy:

   - **Identyfikator firmy Microsoft**;
   - **Nazwa firmy**;
   - **Nazwa domeny podstawowej**;
   - **Relacja**— relacja biznesowa partnera z poszczególnymi klientami.

    Domyślnie centrum partnerskie eksportuje całą listę klientów, niezależnie od długości. Możesz również przeszukać listę klientów według nazwy firmy lub domeny i wyeksportować ten podzbiór danych.

3. Jeśli jesteś dostawcą pośrednim, możesz odfiltrować listę klientów przez pośredniego odsprzedawcy. Wybierz pozycję **Filtruj według pośredniego odsprzedawcy** z listy, a następnie wybierz odsprzedawcę.


## <a name="export-customer-subscription-information"></a>Eksportowanie informacji o subskrypcji klienta

1. W menu **Centrum partnerskiego** wybierz pozycję **Customers**.

2. Wybierz **nazwę firmy** dla każdego klienta. Zostanie otwarta strona **subskrypcje** klienta zawierająca kompletną listę subskrypcji produktów.

3. Wybierz pozycję **Eksportuj subskrypcje**. Centrum partnerskie konwertuje dane subskrypcji klienta do pliku CSV i przekazuje je do domyślnego folderu pobierania na komputerze. Kolumny danych obejmują następujące elementy:
   - **Identyfikator subskrypcji**;
   - **Subskrypcja**— Nazwa produktu dla subskrypcji;
   - **Ilość**— liczba zakupionych licencji;
   - **Stan**;
   - **Odsprzedawca**— identyfikator odsprzedawcy, który jest właścicielem i zarządza subskrypcją.

> [!NOTE]  
> Aby uzyskać więcej informacji na temat zarządzania subskrypcjami, zobacz [subskrypcje klientów](customer-subscriptions.md).
