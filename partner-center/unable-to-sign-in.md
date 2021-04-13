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
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="c852c-103">Rozwiązywanie problemów z logowaniem w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="c852c-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="c852c-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="c852c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c852c-105">Wszyscy partnerzy zainteresowani Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="c852c-105">All partners interested in Partner Center</span></span>

<span data-ttu-id="c852c-106">Ten artykuł zawiera rozwiązania typowych problemów z logowaniem w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="c852c-106">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="c852c-107">Hasło do Centrum partnerskiego zostało zapomniane</span><span class="sxs-lookup"><span data-stu-id="c852c-107">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="c852c-108">Jeśli hasło nie zostanie zapomniane i nie można się zalogować do Centrum partnerskiego, skontaktuj się z pomocą techniczną.</span><span class="sxs-lookup"><span data-stu-id="c852c-108">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="c852c-109">Znajdź odpowiedni kontakt w [obsłudze produktów firmowych](/microsoft-365/admin/contact-support-for-business-products).</span><span class="sxs-lookup"><span data-stu-id="c852c-109">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="c852c-110">Jeśli jesteś partnerem usługi MPN, poprosimy o utworzenie nowego hasła przez administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="c852c-110">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="c852c-111">Jeśli jesteś pośrednim odsprzedawcą dostawcy usług kryptograficznych, poprosimy o utworzenie nowego administratora globalnego dla Ciebie w dzierżawie usługi Azure AD lub utworzenie nowego hasła przy użyciu delegowanych uprawnień administratora.</span><span class="sxs-lookup"><span data-stu-id="c852c-111">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="c852c-112">Aby dowiedzieć się więcej na temat sposobu resetowania hasła i odzyskania dostępu do konta służbowego, przeczytaj temat [Resetowanie hasła służbowego przy użyciu informacji zabezpieczających](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="c852c-112">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="c852c-113">Nie można wyświetlić oczekiwanych stron ani możliwości ani zarządzać nimi w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="c852c-113">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="c852c-114">Dostęp do stron w centrum partnerskim jest kontrolowany przez przypisane role.</span><span class="sxs-lookup"><span data-stu-id="c852c-114">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="c852c-115">Aby sprawdzić, które role są przypisane, w centrum partnerskim wybierz ikonę Ustawienia, wybierz pozycję **Ustawienia konta**, a następnie w obszarze Ustawienia konta wybierz pozycję **Zarządzanie użytkownikami**.</span><span class="sxs-lookup"><span data-stu-id="c852c-115">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="c852c-116">W polu wyszukiwania wpisz swoją nazwę, a następnie Wyświetl wyniki.</span><span class="sxs-lookup"><span data-stu-id="c852c-116">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="c852c-117">Jeśli nie masz możliwości wyświetlania kompetencji, klientów, bodźców lub użytkowników, których oczekujesz, wypróbuj następujące rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="c852c-117">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="c852c-118">Aby uzyskać dostęp do możliwości MPN, dostawcy usług kryptograficznych i odwołań, skontaktuj się z administratorem globalnym lub administratorem konta. Aby dowiedzieć się więcej o rolach i zadaniach, które są włączane w centrum partnerskim, zobacz [Przypisywanie ról & uprawnień użytkownikom](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c852c-118">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="c852c-119">Aby uzyskać dostęp do możliwości komercyjnej witryny Marketplace oraz programów Windows & Xbox, Office Store, Microsoft Edge i Developer, skontaktuj się z osobą w roli właściciela lub Menedżera w organizacji.</span><span class="sxs-lookup"><span data-stu-id="c852c-119">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="c852c-120">Aby dowiedzieć się więcej o rolach i uprawnieniach, zobacz [jak zarządzać komercyjnym kontem witryny Marketplace w centrum partnerskim firmy Microsoft](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span><span class="sxs-lookup"><span data-stu-id="c852c-120">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="c852c-121">Twoja oferta lub korzyści nie są widoczne w centrum partnerskim</span><span class="sxs-lookup"><span data-stu-id="c852c-121">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="c852c-122">Upewnij się, że używasz poprawnych poświadczeń do zalogowania się.</span><span class="sxs-lookup"><span data-stu-id="c852c-122">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="c852c-123">Na przykład Twoje konta służbowe i osobiste mogą wyglądać tak samo (np abc@contoso.com .), ale mogą to być konto osobiste, które zostało utworzone, a inne mogą być kontem biznesowym skonfigurowanym w Twoim imieniu.</span><span class="sxs-lookup"><span data-stu-id="c852c-123">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="c852c-124">W takim przypadku, jeśli użytkownik jest zalogowany, ale nie może wyświetlić oczekiwanych możliwości związanych z MPN, CSP i komercyjnym rynkiem, spróbuj wybrać konto służbowe.</span><span class="sxs-lookup"><span data-stu-id="c852c-124">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c852c-125">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="c852c-125">Next steps</span></span>

- [<span data-ttu-id="c852c-126">Weryfikowanie informacji o koncie</span><span class="sxs-lookup"><span data-stu-id="c852c-126">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="c852c-127">Resetowanie hasła</span><span class="sxs-lookup"><span data-stu-id="c852c-127">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="c852c-128">Resetowanie hasła użytkownika</span><span class="sxs-lookup"><span data-stu-id="c852c-128">Reset a user password</span></span>](reset-a-user-password.md)