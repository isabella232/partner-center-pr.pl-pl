---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925037"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Zarządzanie lokalizacjami kont MPN i Dodawanie nowej lokalizacji


**Odpowiednie role**

- Administrator globalny
- Administrator konta

IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy. IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych. Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.

## <a name="the-following-is-a-typical-scenario"></a>Poniżej przedstawiono typowy scenariusz:

Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii. Jest to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi. Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA. W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory. PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt. Wypłaty są powiązane z określonymi lokalizacjami. 

>[!NOTE]
>Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Wymagania wstępne w celu dodania nowego konta dla firmy dostawcy CSP

Aby dodać nowe konto biznesowe dostawcy usług kryptograficznych, Zacznij od upewnienia się, że spełniono wymagania wstępne.

1. W kraju, w którym ma być prowadzone biznesowe Oprogramowanie CSP, musi znajdować się identyfikator MPN. Aby utworzyć nową lokalizację MPN, przeczytaj sekcję "Dodawanie lokalizacji MPN" poniżej.
  
1. Aby utworzyć nową dostawcę CSP pośredniego rejestracji odsprzedawcy, przeczytaj artykuł [współpraca z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowego** konta dostawcy usług kryptograficznych. Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.

2. Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.

## <a name="add-an-mpn-location"></a>Dodaj lokalizację MPN

1. Zaloguj się przy użyciu konta MPN w centrum partnerskim. (Poświadczenia MPN mogą się różnić od poświadczeń programu CSP). Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

1. Na **ikonie ustawień** wybierz **Ustawienia konta** , a następnie wybierz pozycję **profil organizacji**.

2. Wybierz pozycję **Legal** , a następnie na karcie **partner** wybierz pozycję **lokalizacje biznesowe,** a następnie kliknij pozycję **Dodaj lokalizację.**

3. Podaj wymagane szczegóły, takie jak nazwa firmy, adres i kontakt, dla lokalizacji, która ma zostać dodana do firmy.
 
1. Kliknij pozycję **Dodaj lokalizację**. Spowoduje to utworzenie nowego identyfikatora MPN dla nowej lokalizacji, z której można korzystać w przypadku transakcji i zachęt dostawcy usług kryptograficznych.

:::image type="content" source="images/legal-biz.png" alt-text="Dodaj nową firmę prawną":::

> [!NOTE]
> Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć. Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.

## <a name="change-country-of-partner-global-account"></a>Zmień kraj konta partnera globalnego 

1. Zaloguj się przy użyciu konta MPN w centrum partnerskim. (Poświadczenia MPN mogą się różnić od poświadczeń programu CSP). Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

2. Na karcie **partner** przejdź do **lokalizacji biznesowej** i sprawdź listę lokalizacji, aby upewnić się, że lokalizacja, która ma się pojawić jako podmiot prawny, jest wyświetlana. 
 
1. Aby dodać lokalizację, kliknij pozycję **Dodaj lokalizację**, a następnie w polu wylot wprowadź wymagane szczegóły, takie jak nazwa firmy, adres i kontakt podstawowy dla lokalizacji, która ma zostać dodana do firmy. 
 
1. Wybierz pozycję **Zmień kraj** obok listy rozwijanej **kraj/region** i postępuj zgodnie z instrukcjami. 

:::image type="content" source="images/lbp.png" alt-text="Brak danych profilu biznesowego firmy":::

5. Kliknij pozycję **Zapisz**.

6. Globalny kraj konta MPN zostanie zmieniony na nowy kraj prawny.
  
## <a name="next-steps"></a>Następne kroki

- Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).
