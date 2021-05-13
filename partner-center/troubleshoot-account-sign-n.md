---
title: Rozwiązywanie problemów z konfigurowaniem konta Partner Center lub odnawianiem MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Rozwiązywanie problemów podczas próby zarejestrowania się w Partner Center. Odpowiada na wyzwania związane z metodami płatności, zapomnia hasłami i nie tylko.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854693"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Rozwiązywanie problemów z konfiguracją konta lub odnawianiem mpn

**Odpowiednie role:** Administrator globalny | Administrator partnera MPN
 
Poniżej znajdują się sugestie dotyczące rozwiązywania typowych problemów występujących podczas konfigurowania Partner Center konta.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Co się stanie, jeśli migrujesz z Partner Membership Center i nie możesz edytować żadnych pól informacji o firmie

W przypadkach, gdy firma jest już obecna w Partner Center (na przykład na koncie CSP) — zostanie wyświetlone ekran tylko do odczytu. Na tym ekranie będą wyświetlane wszystkie informacje o firmie, które istnieją w Partner Center.

Nie można zmienić szczegółów na tym ekranie. Jest to projektowe, a nie błędne.

Wybierz **pozycję Zaakceptuj** i **kontynuuj,** aby kontynuować.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Jeśli dział IT wyłączył opcji Zarejestruj **się w Partner Center**

Zostanie wyświetlony ten komunikat, ponieważ użytkownicy marketingowi są wyłączeni lub w dzierżawie usługi Azure AD jest wyłączona rejestracja wirusowa. Administrator globalny konta usługi Azure AD może włączyć wymagane funkcje, uruchamiając następujące polecenie programu PowerShell:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Aby uzyskać więcej informacji, zapoznaj [się z tematem Self-service sign up (Rejestracja samoobsługowa).](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Nie pamiętasz hasła

Jeśli nie pamiętasz hasła, wybierz link Nie możesz uzyskać dostępu do **konta?** na stronie logowania. Ta opcja umożliwia zresetowanie hasła lub poproś administratora globalnego o przypisanie Ci nowych poświadczeń.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na ekranie "Poinformuj nas o swojej firmie" zostanie wyświetlony komunikat o błędzie "Wystąpił problem"

Ten komunikat o błędzie jest zwykle wyświetlany, jeśli przypadkowo używasz znaków specjalnych, spacji lub kodu kraju w numerze telefonu firmy. Wartość wprowadzona w polu Numer telefonu może zawierać maksymalnie 10 znaków.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Podczas zakupu karty kredytowej jest wyświetlany komunikat o błędzie informujący o tym, że zamówienie zostało odrzucone. Sprawdź swoje informacje"


Zawsze używaj adresu odpowiadającego karcie kredytowej, a nie jednostki prawnej. Upewnij się również, że kod pocztowy jest poprawny i odpowiada adresowi, z których korzystasz.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Chcesz przełączyć się z płatności offline na formę płatności online 

Musisz anulować oryginalne zamówienie i ponownie wykup przy użyciu preferowanej formy płatności.

Aby anulować zamówienie:

1. Wybierz **kartę Oferty** członkostwa na pulpicie nawigacyjnym.

2. Wybierz **pozycję Anuluj zamówienie**

3. Zostanie wyświetlone okno potwierdzenia z potwierdzeniem, które należy potwierdzić, aby anulować początkowe zamówienie.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
- [Jak odczytać rachunek i ponownie złożyć plik](read-your-bill.md)
