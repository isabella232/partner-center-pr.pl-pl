---
title: Jednostkę usługi Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Dowiedz się, jak dodać jednostkę usługi do dzierżawy usługi Azure AD. Oznacza to dodanie aplikacji usługi Azure AD (jednostki usługi) w Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a7851d270ad51a5a06ebc7d7725a2ae5c803419b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842834"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Dodawanie aplikacji usługi Azure AD (jednostki usługi) w Partner Center

**Odpowiednie role:** Administrator globalny

W programie komercyjnej platformy handlowej w usłudze Partner Center możesz teraz dodać aplikację usługi Microsoft Azure Active Directory (Azure AD) (jednostkę usługi) jako użytkownika na Partner Center konta. (Wcześniej można było to zrobić na koncie Cloud Partner Portal (CPP). Teraz, po migracji do Partner Center, konto CPP jest tylko do odczytu).
 
>[!Note] 
>Jednostki usługi to synonimy aplikacji usługi Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Dodawanie aplikacji usługi Azure AD (jednostki usługi)

1. Na pulpicie Partner Center nawigacyjnym wybierz pozycję **Ustawienia** a następnie wybierz pozycję **Ustawienia dewelopera.**

2. Wybierz **pozycję Użytkownicy,** a następnie **wybierz pozycję Dodaj aplikacje usługi Azure AD.**

3. Wybierz istniejącą aplikację usługi Azure AD lub utwórz nową.

4. Jeśli tworzysz nową aplikację usługi Azure AD, dołącz następujące informacje:  

   - **Adres URL odpowiedzi:** adres URL, pod którym użytkownicy mogą się logować w celu korzystania z aplikacji usługi Azure AD.

   - **Identyfikator URI identyfikatora** aplikacji: identyfikator logiczny aplikacji usługi Azure AD, który jest prezentowany podczas wysyłanie żądania logowania pojedynczego do usługi Azure AD.

   - **Role zabezpieczeń:** Role Menedżer **(takie** same jak rola "Właściciel" w CPP) i Deweloper **(takie** same jak rola "Współautor" w CPP) mają zastosowanie do programu komercyjnej platformy handlowej w programie Partner Center i mogą być skojarzone z tą aplikacją usługi Azure AD.  

## <a name="next-steps"></a>Następne kroki

- [Omówienie platformy handlowej w Partner Center](csp-commercial-marketplace-overview.md)