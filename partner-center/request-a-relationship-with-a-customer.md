---
title: Poproś o nawiązanie relacji odsprzedawca-klient
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zażądaj relacji z klientem w scenariuszach wielokanałowych dla wielu partnerów lub jeśli musisz przywrócić delegowane uprawnienia administratora dla klienta.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 83f615e69a9285365e68305fa909104e0da52992
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551643"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Jak zażądać relacji odsprzedawcy od klienta w Centrum partnerskim

**Odpowiednie role:** Administrator | Administrator globalny

Jeśli chcesz zarządzać usługą lub subskrypcją klienta w jego imieniu, klient musi przyznać Ci uprawnienia administratora do tej usługi lub subskrypcji i podpisać Umowa z Klientem Microsoft.

Jeśli chcesz ustanowić relację odsprzedawcy z klientem i zarządzać tylko subskrypcjami platformy Azure, które aprowizujesz, nie musisz uzyskiwać uprawnień administratora.

>[!NOTE] 
>Opcja nieuzysłania żądania uprawnień nie jest dostępna dla partnerów działających w Microsoft Cloud for US Government lub Microsoft Cloud w Niemczech. Aby dowiedzieć się więcej, zobacz [Klienci delegowanie uprawnień administracyjnych do partnerów.](customers-revoke-admin-privileges.md)

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Zapraszanie klienta do nawiązania relacji odsprzedawcy

Możesz zażądać relacji odsprzedawcy z klientem z danego kraju lub tego samego regionu.

1. Wybierz **pozycję Customers** (Klienci) **Partner Center** menu aplikacji, a następnie wybierz pozycję Request a reseller relationship **(Zażądaj relacji odsprzedawcy).**

2. Aby zażądać uprawnień administratora od tego klienta, wybierz pozycję Uwzględnij delegowane uprawnienia administracyjne dla Azure Active Directory **i Office 365.** Aby ustanowić relację bez żądania uprawnień administratora, usuń zaznaczenie tej opcji.

3. Na następnej stronie przejrzyj wersję roboczą wiadomości e-mail. Możesz otworzyć wersję roboczą wiadomości w domyślnej aplikacji poczty e-mail lub skopiować wiadomość do schowka i wkleić do wiadomości e-mail.

   Tekst wiadomości można edytować, ale należy pamiętać o zachowaniu spersonalizowanego linku umożliwiającego bezpośrednie połączenie klienta z Twoim kontem. Po **ukończeniu** tego kroku wybierz pozycję Gotowe.

4. Wyślij wiadomość e-mail do klienta.

5. Gdy klient zaakceptuje Zaproszenie, pojawi się  na stronie Klienci i będzie mógł aprowizować usługę dla klienta i zarządzać jej od tej strony.

   > [!NOTE]
   > Jeśli klient nie zaakceptował jeszcze Umowa z Klientem Microsoft, po zaakceptowaniu zaproszenia zostanie wyświetlony monit o jej zaakceptowanie. Klient musi być administratorem globalnym, aby zaakceptować zaproszenie.

6. Aby zarządzać kontem, usługami, użytkownikami i licencjami klienta, rozwiń rekord klienta, wybierając strzałkę w dół obok jego nazwy.

> [!IMPORTANT]  
> Klienci mogą ponownie przypisać lub usuwać uprawnienia administratora w portalu administracyjnym usługi. Jednak dopóki nie zostanie ponownie wynegocjowana umowa z klientem, użytkownik nadal będzie odpowiedzialny za świadczenie pomocy technicznej dla klientów i korzystanie z warunków umowy Microsoft Partner Agreement nawet po ponownej przypisania lub usunięciu przez klienta uprawnień administratora. W takiej sytuacji, jeśli klient wymaga pomocy, możesz zadzwoń do działu pomocy technicznej firmy Microsoft, aby otworzyć żądanie obsługi w imieniu klienta.

## <a name="changes-to-the-customer-invitation-experience"></a>Zmiany w obsługi zapraszania klientów

Środowisko klienta dotyczące akceptowania zaproszenia do relacji odsprzedawcy od partnera Dostawca rozwiązań w chmurze (CSP) jest hostowane przez różne portale dla klientów. Lokalizacja portalu zależy od tego, czy klient znajduje się w chmurze publicznej firmy Microsoft, czy w chmurze krajowej:

|Typy klientów chmury  | Gdzie klient akceptuje zaproszenie do relacji odsprzedawcy? |
|---------|---------
| Klienci w chmurze publicznej | Microsoft 365 Administracyjne |
| Klienci w witrynie Partner Center for Microsoft Cloud (Niemcy) | Microsoft Office Admin Portal |
| Klienci w Partner Center for Microsoft Cloud for US Government | Microsoft Office Admin Portal |
|

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie kontaktów pomocy technicznej](assign-support-contacts.md)

- [Usuwanie relacji z klientem](remove-a-relationship.md)
