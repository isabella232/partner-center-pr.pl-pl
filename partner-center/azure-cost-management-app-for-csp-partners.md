---
title: Usługa Azure Cost Management firmy Cloudyn dla dostawców CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak zarejestrować aplikację sieci Web Cloudyn i użyć klucza tajnego w centrum partnerskim, aby można było używać aplikacji do śledzenia użycia i kosztów platformy Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534996"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Śledzenie użycia i kosztów platformy Azure za pomocą aplikacji Azure Cost Management dla partnerów CSP  

**Odpowiednie role**

- Administrator globalny
- Agent administracyjny

[Uzyskaj więcej informacji na temat Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Przed rozpoczęciem
Przed rozpoczęciem korzystania z Azure Cost Management upewnij się, że spełniasz następujące wymagania:

- Jesteś partnerem w programie dostawcy rozwiązań w chmurze.
- Można utworzyć aplikację internetową interfejsu API Centrum partnerskiego.

## <a name="overview"></a>Omówienie

Cloudyn to aplikacja internetowa, która umożliwia śledzenie i zarządzanie ilością klientów korzystających z platformy Azure oraz kosztami tego użycia. Jest on używany za pomocą interfejsu API Centrum partnerskiego.

## <a name="register-your-web-app-in-the-partner-center"></a>Zarejestruj swoją aplikację sieci Web w centrum partnerskim
Po zarejestrowaniu aplikacji internetowej Azure Active Directory w centrum partnerskim zostanie włączony dostęp do interfejsu API Centrum partnerskiego. 
1.  Zaloguj się do [Centrum partnerskiego](https://partnercenter.microsoft.com/pcv/dashboard/overview) przy użyciu [konta administratora globalnego lub agenta administratora](create-user-accounts-and-set-permissions.md).
2.  W **centrum partnerskim** wybierz pozycję **Ustawienia konta** &gt; **[Zarządzanie aplikacjami](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
3.  W sekcji **aplikacja sieci Web** kliknij pozycję **Dodaj nową aplikację sieci Web**.
<br> **Uwaga**: Jeśli wcześniej utworzono aplikację sieci Web, możesz pominąć krok 3.
4.  Skopiuj i Zapisz identyfikator GUID **identyfikatora** i **Identyfikator aplikacji** dla aplikacji sieci Web. Do korzystania z 30-dniowej bezpłatnej wersji próbnej aplikacji Azure Cost Management wymagane są oba identyfikatory.

## <a name="add-a-secret-key-to-your-app"></a>Dodawanie klucza tajnego do aplikacji
1. Na liście rozwijanej obok przycisku **Dodaj klucz** wybierz czas trwania wynoszący 1 lub 2 lata.
2. Kliknij przycisk **Dodaj klucz**. 
3. Skopiuj i Zapisz wartość klucza tajnego. Będzie to konieczne w przypadku 30-dniowej bezpłatnej wersji próbnej.<br>
   > [!NOTE]  
   > Klucze tajne aplikacji są podobne do haseł z dłuższymi datami ważności. Zapisz wartość klucza w bezpiecznej lokalizacji do użycia w przyszłości.

## <a name="next-steps"></a>Następne kroki
Rozpocznij [30-dniową bezpłatną wersję próbną](https://go.microsoft.com/fwlink/?linkid=857895).
Aby rozpocząć okres próbny, potrzebne są następujące szczegóły:
- Poświadczenia logowania do Centrum partnerskiego
- Identyfikator GUID identyfikatora Commerce
- Identyfikator GUID identyfikatora aplikacji
- Wartość klucza tajnego aplikacji
