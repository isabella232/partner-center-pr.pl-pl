---
title: Rozwiązywanie problemów z konfigurowaniem konta Centrum partnerskiego lub Rozwiązywanie problemów z odnowieniem MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Rozwiązywanie problemów podczas próby zarejestrowania się w centrum partnerskim. Odpowiedzi na wyzwania związane z metodami płatności, zapomnieniu haseł i nie tylko.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381413"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Rozwiązywanie problemów z konfiguracją konta lub MPN odnowienia

**Dotyczy**

- Centrum partnerskie
 
**Odpowiednie role**

- Administrator globalny
- Administrator partnerski MPN 
 
Poniżej przedstawiono kilka sugestii dotyczących rozwiązywania typowych problemów, które powstają podczas konfigurowania konta Centrum partnerskiego.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Co się stanie w przypadku migrowania z Centrum członkostwa w partnerze i nie można edytować żadnych pól informacji o firmie

W przypadkach, w których firma ma już obecność w centrum partnerskim (podyktuj konto CSP) — zostanie wyświetlony ekran tylko do odczytu. Na tym ekranie zostaną wyświetlone wszystkie informacje o firmie, które istnieją w centrum partnerskim.

Nie można zmienić szczegółów na tym ekranie. Jest to zgodne z projektem, a nie błędem.

Wybierz pozycję **Akceptuj** i **Kontynuuj** , aby kontynuować.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Jeśli dział IT wyłączył **Rejestrowanie w centrum partnerskim**.

Zobaczysz ten komunikat, ponieważ użytkownicy z wirusami są wyłączeni lub że wirusowe rejestrowanie w dzierżawie usługi Azure AD jest wyłączone. Administrator globalny dla konta usługi Azure AD może włączyć wymagane funkcje, uruchamiając następujące polecenie programu PowerShell:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Aby uzyskać więcej informacji, zapoznaj się z artykułem [rejestracja samoobsługowa](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Nie pamiętasz hasła

Jeśli zapomniano hasło, wybierz link **nie można uzyskać dostępu do konta?** na stronie logowania. Ta opcja umożliwia zresetowanie hasła lub poproszenie administratora globalnego o przypisanie nowych poświadczeń.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na ekranie "Powiedz nam o swojej firmie" pojawia się błąd "coś poszło źle"

Ten komunikat o błędzie jest zwykle wyświetlany, jeśli przypadkowo użyto znaków specjalnych, spacji lub kodu kraju w numerze telefonu firmy. Wartość wprowadzona w polu numer telefonu może zawierać maksymalnie 10 znaków.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Zakup karty kredytowej otrzymuje komunikat o błędzie z informacją o tym, że zamówienie zostało odrzucone. Sprawdź swoje informacje "


Zawsze używaj adresu odpowiadającego karcie kredytowej, a nie podmiotowi prawnemu. Upewnij się również, że kod pocztowy jest poprawny i odpowiada adresowi, którego używasz.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Chcesz przełączyć się z płatności offline do formy płatności online 

Musisz anulować oryginalne zamówienie i ponownie kupić przy użyciu preferowanej metody płatności.

Aby anulować zamówienie:

1. Wybierz kartę **oferty członkostwa** na pulpicie nawigacyjnym.

2. Wybierz pozycję **Anuluj zamówienie**

3. Zostanie wyświetlone okno potwierdzenia i musisz potwierdzić, aby anulować kolejność początkową.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
- [Jak odczytać plik rachunku i Rekonesans](read-your-bill.md)
