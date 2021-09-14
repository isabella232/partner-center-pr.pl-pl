---
title: Rozwiązywanie problemów z konfigurowaniem konta Partner Center lub odnawianiem MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Rozwiązywanie problemów podczas próby zarejestrowania się w Partner Center. Odpowiada na wyzwania związane z metodami płatności, zapomnia hasłami i nie tylko.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 08672379e300eccf18a0a1f0cfc1e41b4b7dbc91
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247281"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Rozwiązywanie problemów z konfiguracją konta lub odnawianiem MPN

**Odpowiednie role:** Administrator globalny | Administrator partnera MPN
 
Poniżej znajdują się sugestie dotyczące rozwiązywania typowych problemów występujących podczas konfigurowania Partner Center konta.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Co się stanie, jeśli migrujesz z Partner Membership Center i nie możesz edytować żadnych pól informacji o firmie

W przypadkach, gdy firma jest już obecna w Partner Center (na przykład na koncie Dostawca rozwiązań w chmurze (CSP) — zostanie wyświetlone ekran tylko do odczytu. Na tym ekranie zostaną wyświetlane wszystkie informacje o firmie, które istnieją w Partner Center.

Nie można zmienić szczegółów na tym ekranie. Jest to projektowe, a nie błędne.

Aby kontynuować, wybierz **pozycję Zaakceptuj,** a następnie wybierz pozycję **Kontynuuj.**


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Jeśli dział IT wyłączył opcji Zarejestruj **się w celu Partner Center**

Ten komunikat jest wyświetlany, ponieważ użytkownicy marketingowi są wyłączeni lub w dzierżawie usługi Azure Active Directory (AD). Administrator globalny konta usługi Azure AD może włączyć wymagane funkcje, uruchamiając następujące polecenie programu PowerShell:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Aby uzyskać więcej informacji, zapoznaj [się z tematem Self-service sign up (Rejestracja samoobsługowa).](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Nie pamiętasz hasła

Jeśli nie pamiętasz hasła, na stronie logowania wybierz pozycję Nie **możesz uzyskać dostępu do konta?**. Ta opcja umożliwia zresetowanie hasła lub poproś administratora globalnego o przypisanie Ci nowych poświadczeń.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na ekranie "Poinformuj nas o swojej firmie" zostanie wyświetlony błąd "Wystąpił problem"

Ten komunikat o błędzie jest zwykle wyświetlany, jeśli przypadkowo używasz znaków specjalnych, spacji lub kodu kraju w firmowym numerze telefonu. Wartość wprowadzona w polu Telefon Number może zawierać maksymalnie 10 znaków.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Podczas zakupu karty kredytowej jest wyświetlany komunikat o błędzie z informacją, że "Twoje zamówienie zostało odrzucone. Sprawdź swoje informacje"


Zawsze używaj adresu odpowiadającego karcie kredytowej, a nie jednostki prawnej. Upewnij się również, że kod pocztowy jest poprawny i odpowiada adresowi, z których korzystasz.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Chcesz przełączyć się z płatności w trybie offline na formę płatności online 

Musisz anulować oryginalne zamówienie i ponownie je zkupić przy użyciu preferowanej formy płatności.

Aby anulować zamówienie:

1. Na pulpicie Partner Center nawigacyjnym wybierz **kartę Oferty** członkostwa.

2. Wybierz **pozycję Anuluj zamówienie**

3. Zostanie wyświetlone okno potwierdzenia z potwierdzeniem, które należy potwierdzić, aby anulować początkowe zamówienie.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
- [Jak odczytać rachunek i ponownie skonfigurować plik](read-your-bill.md)
