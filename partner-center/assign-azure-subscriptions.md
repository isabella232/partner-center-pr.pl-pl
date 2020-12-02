---
title: Przypisywanie subskrypcji platformy Azure do klientów
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak przypisać subskrypcje platformy Azure klientom w centrum partnerskim i jak umożliwić klientom zarządzanie własnymi subskrypcjami.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473955"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a>Przypisywanie subskrypcji platformy Azure klientom w centrum partnerskim

**Odpowiednie role**

- Administrator globalny
- Agent sprzedaży

## <a name="assign-azure-subscriptions-to-your-customers"></a>Przypisywanie subskrypcji platformy Azure do klientów

1. Wybierz pozycję **klienci** z menu **Centrum partnerskiego** i Znajdź klienta, którym chcesz zarządzać.

2. Wybierz strzałkę w dół na końcu wiersza, aby rozwinąć rekord klienta, a następnie wybierz pozycję **Portal zarządzania Microsoft Azure**. Nastąpi przekierowanie do [Azure Portal](https://portal.azure.com/) , w którym można zarządzać subskrypcjami klienta.

3. W Azure Portal wybierz pozycję **subskrypcje**.

4. Wybierz subskrypcję, którą chcesz przypisać, a następnie wybierz pozycję **Access Control**.

5. Wybierz pozycję **Dodaj** , aby dodać użytkownika do subskrypcji. 

6. Po dodaniu użytkownika do subskrypcji można przypisać użytkownikowi rolę i określone konto, do którego użytkownik będzie miał dostęp.

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a>Umożliwienie klientom zarządzania swoimi subskrypcjami platformy Azure

Po utworzeniu subskrypcji Microsoft Azure dla klienta można umożliwić im Zarządzanie subskrypcją. Aby to zrobić, należy zalogować się do portalu zarządzania Microsoft Azure klienta. 

1. Aby otworzyć Azure Portal klienta, rozwiń listę klientów na liście klientów lub wybierz nazwę klienta, a następnie wybierz pozycję **Portal zarządzania Microsoft Azure**.

   > [!NOTE]  
   > Jeśli zostanie wyświetlony monit o zalogowanie się do Azure Portal, użytkownik nie może mieć delegowanych uprawnień administracyjnych. Wybierz pozycję **Żądaj relacji** , aby zaprosić klienta do identyfikacji użytkownika jako partnera rekordu. Po zaakceptowaniu zaproszenia przez klienta zostaną automatycznie przyznane delegowane uprawnienia administracyjne.

2. W Azure Portal Otwórz listę subskrypcje klienta i wybierz subskrypcję platformy Azure klienta.

3. Przypisz rolę wszystkim użytkownikom klienta, aby mogli tworzyć zasoby w ramach ich subskrypcji i zarządzać nimi.

## <a name="next-steps"></a>Następne kroki

- [Jak partnerzy CSP mogą sprzedawać subskrypcje klientom](customer-subscriptions.md)

- [Jak uzyskać uprawnienia do zarządzania usługą lub subskrypcjami klienta](customers-revoke-admin-privileges.md)
