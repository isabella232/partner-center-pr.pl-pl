---
title: Nie można zalogować się do Centrum partnerskiego
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Rozwiązywanie możliwych przyczyn i informacje o rozwiązaniach, dla których nie można zalogować się do Centrum partnerskiego — Dowiedz się więcej na temat resetowania haseł, sprawdzania ról i sprawdzania poświadczeń.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266575"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Rozwiązywanie problemów z logowaniem w centrum partnerskim

**Odpowiednie role**

- Wszyscy partnerzy zainteresowani Centrum partnerskiego

Ten artykuł zawiera rozwiązania typowych problemów z logowaniem w centrum partnerskim.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Hasło do Centrum partnerskiego zostało zapomniane

Jeśli hasło nie zostanie zapomniane i nie można się zalogować do Centrum partnerskiego, skontaktuj się z pomocą techniczną. Znajdź odpowiedni kontakt w [obsłudze produktów firmowych](/microsoft-365/admin/contact-support-for-business-products).

Jeśli jesteś partnerem usługi MPN, poprosimy o utworzenie nowego hasła przez administratora globalnego. Jeśli jesteś pośrednim odsprzedawcą dostawcy usług kryptograficznych, poprosimy o utworzenie nowego administratora globalnego dla Ciebie w dzierżawie usługi Azure AD lub utworzenie nowego hasła przy użyciu delegowanych uprawnień administratora.

Aby dowiedzieć się więcej na temat sposobu resetowania hasła i odzyskania dostępu do konta służbowego, przeczytaj temat [Resetowanie hasła służbowego przy użyciu informacji zabezpieczających](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Nie można wyświetlić oczekiwanych stron ani możliwości ani zarządzać nimi w centrum partnerskim

Dostęp do stron w centrum partnerskim jest kontrolowany przez przypisane role. Aby sprawdzić, które role są przypisane, w centrum partnerskim wybierz ikonę Ustawienia, wybierz pozycję **Ustawienia konta**, a następnie w obszarze Ustawienia konta wybierz pozycję **Zarządzanie użytkownikami**. W polu wyszukiwania wpisz swoją nazwę, a następnie Wyświetl wyniki.

Jeśli nie masz możliwości wyświetlania kompetencji, klientów, bodźców lub użytkowników, których oczekujesz, wypróbuj następujące rozwiązania:

- Aby uzyskać dostęp do możliwości MPN, dostawcy usług kryptograficznych i odwołań, skontaktuj się z administratorem globalnym lub administratorem konta. Aby dowiedzieć się więcej o rolach i zadaniach, które są włączane w centrum partnerskim, zobacz [Przypisywanie ról & uprawnień użytkownikom](permissions-overview.md).
- Aby uzyskać dostęp do możliwości komercyjnej witryny Marketplace oraz programów Windows & Xbox, Office Store, Microsoft Edge i Developer, skontaktuj się z osobą w roli właściciela lub Menedżera w organizacji. Aby dowiedzieć się więcej o rolach i uprawnieniach, zobacz [jak zarządzać komercyjnym kontem witryny Marketplace w centrum partnerskim firmy Microsoft](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Twoja oferta lub korzyści nie są widoczne w centrum partnerskim

Upewnij się, że używasz poprawnych poświadczeń do zalogowania się. Na przykład Twoje konta służbowe i osobiste mogą wyglądać tak samo (np abc@contoso.com .), ale mogą to być konto osobiste, które zostało utworzone, a inne mogą być kontem biznesowym skonfigurowanym w Twoim imieniu. W takim przypadku, jeśli użytkownik jest zalogowany, ale nie może wyświetlić oczekiwanych możliwości związanych z MPN, CSP i komercyjnym rynkiem, spróbuj wybrać konto służbowe.

## <a name="next-steps"></a>Następne kroki

- [Weryfikowanie informacji o koncie](verification-responses.md)
- [Resetowanie hasła](reset-my-pasword.md)
- [Resetowanie hasła użytkownika](reset-a-user-password.md)