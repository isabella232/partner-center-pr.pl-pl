---
title: Nazwa główna usługi Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodać jednostkę usługi do dzierżawy usługi Azure AD. Oznacza to dodanie aplikacji usługi Azure AD (nazwy głównej usługi) w centrum partnerskim.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2020
ms.locfileid: "92529490"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Dodawanie aplikacji usługi Azure AD (nazwy głównej usługi) w centrum partnerskim

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator globalny

W programie komercyjnym Marketplace w centrum partnerskim możesz teraz dodać aplikację usługi Azure AD (nazwę główną usługi) jako użytkownika na koncie Centrum partnerskiego. (Wcześniej można było to zrobić w portal Cloud Partner lub CPP. Teraz, gdy przeprowadzono migrację do Centrum partnerskiego, konto CPP jest tylko do odczytu.
 
>[!Note] 
>Nazwa główna usługi jest równoznaczna z aplikacją usługi Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Dodawanie aplikacji usługi Azure AD (nazwy głównej usługi)

1. Na pulpicie nawigacyjnym Centrum partnerskiego wybierz pozycję **Ustawienia** , a następnie wybierz pozycję **Ustawienia dewelopera**.

2. Wybierz pozycję **Użytkownicy** , a następnie wybierz pozycję **Dodaj aplikacje usługi Azure AD**.

3. Wybierz istniejącą aplikację usługi Azure AD lub Utwórz nową.

4. Jeśli tworzysz nową aplikację usługi Azure AD, uwzględnij następujące informacje:  

   - **Adres URL odpowiedzi**: adres URL, pod którym użytkownicy mogą się logować, aby korzystać z aplikacji usługi Azure AD.

   - **Identyfikator URI aplikacji**: Identyfikator logiczny dla aplikacji usługi Azure AD, który jest prezentowany podczas wysyłania żądania logowania jednokrotnego do usługi Azure AD.

   - **Role zabezpieczeń**: **Menedżer** ról (taki sam jak rola "właściciel" w programie CPP) i **deweloper** (taka sama jak rola "Współautor" w programie CPP) ma zastosowanie do komercyjnego programu Marketplace w centrum partnerskim i można je SKOJARZYĆ z tą aplikacją usługi Azure AD.  

## <a name="next-steps"></a>Następne kroki

- [Omówienie portalu komercyjnego w centrum partnerskim](csp-commercial-marketplace-overview.md)