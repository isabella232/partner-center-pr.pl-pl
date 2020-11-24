---
title: Zarządzanie lokalizacjami na koncie partnerskim
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak dodać nową lokalizację i jak używać identyfikatora MPN Location w programach zachęty, biznesie CSP, subskrypcjach i innych transakcjach.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514806"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Zarządzanie lokalizacjami kont MPN i Dodawanie nowej lokalizacji

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator globalny
- Administrator konta

IDENTYFIKATOR MPN lokalizacji identyfikuje każdą konkretną lokalizację firmy. IDENTYFIKATOR MPN Location służy do rejestrowania w programach zachęty, do firmowego dostawcy rozwiązań w chmurze (CSP) i innych transakcji roboczych. Globalny identyfikator MPN jest używany dla działań nietransakcyjnych, takich jak żądania pomocy technicznej.

## <a name="the-following-is-a-typical-scenario"></a>Poniżej przedstawiono typowy scenariusz:

Firma Contoso ma swoje konto globalne partnera (PGA) w Wielkiej Brytanii. Jest to zarejestrowana firma prawna, a jej globalny identyfikator MPN jest używany do zarządzania wszystkimi nietransakcyjnymi biznesowymi. Firma Contoso ma także równorzędne konta firmowe lub działy w innej lokalizacji w Wielkiej Brytanii, Francji i w USA. W strukturze konta MPN te PLAs są reprezentowane jako unikatowe lokalizacje MPN identyfikatory. PLAs są używane dla transakcji transakcyjnych, takich jak CSP lub programy zachęt. Wypłaty są powiązane z określonymi lokalizacjami. 

>[!NOTE]
>Istnieje relacja 1-1 między dzierżawą dostawcy usług kryptograficznych i IDENTYFIKATORem lokalizacji MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura lokalizacji MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Wymagania wstępne w celu dodania nowej lokalizacji dla firmy dostawcy CSP

Aby dodać nową lokalizację biznesową programu CSP, istnieje kilka wymagań wstępnych:

1. W kraju, w którym chcesz przeprowadzić działalność biznesową, musisz mieć identyfikator MPN lokalizacji.

1. Potrzebna jest nowa dzierżawa usługi Azure AD w [regionie firmy](regional-authorization-overview.md) , która nie została już zarejestrowana w dostawcy usług kryptograficznych. Utwórz to po zarejestrowaniu w dostawcy usług kryptograficznych.
 
3. Użyj nowej dzierżawy usługi AAD, aby zarejestrować się w programie CSP w regionie.
Dostarczenie szczegółowych informacji o firmie, takich jak imię i nazwisko, adres, podstawowe informacje kontaktowe firmy. To konto zostanie poddane weryfikacji, dlatego należy dodać prawidłowe informacje.

>[!NOTE] 
 >Pamiętaj, aby zalogować się przy użyciu **nowych** poświadczeń dla **nowej** dzierżawy usługi Azure AD. Nie używaj istniejących poświadczeń, ponieważ centrum partnerskie sprawdzi, czy masz już konto.

4. Zaakceptuj umowę partnera firmy Microsoft i aktywuj konto.

## <a name="add-an-mpn-location"></a>Dodaj lokalizację MPN

1. Zaloguj się przy użyciu konta MPN w centrum partnerskim. Konto MPN powinno mieć uprawnienia administratora globalnego lub administratora konta. 

1. Na **ikonie ustawienia** wybierz **Ustawienia organizacji**.

2. Wybierz pozycję **Legal** , a następnie wybierz pozycję **lokalizacje.**

3. Wybierz pozycję **Dodaj lokalizację** i Wstaw szczegóły adresu lokalizacji, która ma zostać dodana do firmy, a także główną osobę kontaktową dla tej lokalizacji.

> [!NOTE]
> Po dodaniu lokalizacji w centrum partnerskim nie można jej usunąć. Aby zalogować się, zobaczysz **MPN** w menu po lewej stronie Centrum partnerskiego.

## <a name="change-global-partner-account-location"></a>Zmień lokalizację globalnego konta partnera

1. W obszarze **[lokalizacje biznesowe](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** Sprawdź listę lokalizacji, aby upewnić się, że na liście znajduje się lokalizacja potrzebna jako jednostka prawna. Jeśli nie, Dodaj ją.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Zrzut ekranu przedstawiający stronę lokalizacje konta Centrum partnerskiego z listą wszystkich bieżących lokalizacji.":::

2. Wybierz pozycję **Legal** , a następnie wybierz pozycję **zaktualizuj służbowy profil prawny**
  
3. Wybierz region i jednostkę prawną i **Prześlij** ją.

  
## <a name="next-steps"></a>Następne kroki

- Dowiedz się więcej na temat [procesu weryfikacji](verification-responses.md).
