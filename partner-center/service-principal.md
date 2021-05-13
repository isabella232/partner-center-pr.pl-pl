---
title: Jednostkę usługi Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodać jednostkę usługi do dzierżawy usługi Azure AD. Oznacza to dodanie aplikacji usługi Azure AD (jednostki usługi) w Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854931"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Dodawanie aplikacji usługi Azure AD (jednostki usługi) w usłudze Partner Center

**Odpowiednie role:** Administrator globalny

W programie komercyjnej platformy handlowej w Partner Center możesz teraz dodać aplikację usługi Azure AD (jednostkę usługi) jako użytkownika na Partner Center konta. (Wcześniej można było to zrobić na koncie Cloud Partner Portal lub CPP. Teraz, po migracji do Partner Center, konto CPP jest tylko do odczytu).
 
>[!Note] 
>Jednostkę usługi należy do aplikacji usługi Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Dodawanie aplikacji usługi Azure AD (jednostki usługi)

1. Na pulpicie Partner Center nawigacyjnym wybierz pozycję **Ustawienia,** a następnie pozycję **Ustawienia dewelopera.**

2. Wybierz **pozycję Użytkownicy,** a następnie **wybierz pozycję Dodaj aplikacje usługi Azure AD.**

3. Wybierz istniejącą aplikację usługi Azure AD lub utwórz nową.

4. Jeśli tworzysz nową aplikację usługi Azure AD, dołącz następujące informacje:  

   - **Adres URL odpowiedzi:** adres URL, pod którym użytkownicy mogą logować się w celu korzystania z aplikacji usługi Azure AD.

   - **Identyfikator URI identyfikatora aplikacji:** identyfikator logiczny aplikacji usługi Azure AD, który jest prezentowany podczas wysyłanie żądania logowania pojedynczego do usługi Azure AD.

   - Role **zabezpieczeń:** role Menedżer **(taki** sam jak rola "Właściciel" w programie CPP) i Deweloper **(takie** same jak rola "Współautor" w programie CPP) mają zastosowanie do programu komercyjnej platformy handlowej w programie Partner Center i mogą być skojarzone z tą aplikacją usługi Azure AD.  

## <a name="next-steps"></a>Następne kroki

- [Omówienie platformy handlowej w Partner Center](csp-commercial-marketplace-overview.md)