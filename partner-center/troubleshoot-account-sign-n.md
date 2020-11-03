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
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530454"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="40c8b-104">Rozwiązywanie problemów z konfiguracją konta lub MPN odnowienia</span><span class="sxs-lookup"><span data-stu-id="40c8b-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="40c8b-105">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="40c8b-105">**Applies to**</span></span>

- <span data-ttu-id="40c8b-106">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="40c8b-106">Partner Center</span></span>
 
<span data-ttu-id="40c8b-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="40c8b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="40c8b-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="40c8b-108">Global admin</span></span>
- <span data-ttu-id="40c8b-109">Administrator partnerski MPN</span><span class="sxs-lookup"><span data-stu-id="40c8b-109">MPN partner admin</span></span> 
 
<span data-ttu-id="40c8b-110">Poniżej przedstawiono kilka sugestii dotyczących rozwiązywania typowych problemów, które powstają podczas konfigurowania konta Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="40c8b-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="40c8b-111">Co się stanie w przypadku migrowania z Centrum członkostwa w partnerze i nie można edytować żadnych pól informacji o firmie</span><span class="sxs-lookup"><span data-stu-id="40c8b-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="40c8b-112">W przypadkach, w których firma ma już obecność w centrum partnerskim (podyktuj konto CSP) — zostanie wyświetlony ekran tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="40c8b-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="40c8b-113">Na tym ekranie zostaną wyświetlone wszystkie informacje o firmie, które istnieją w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="40c8b-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="40c8b-114">Nie można zmienić szczegółów na tym ekranie.</span><span class="sxs-lookup"><span data-stu-id="40c8b-114">You can't change the details on this screen.</span></span> <span data-ttu-id="40c8b-115">Jest to zgodne z projektem, a nie błędem.</span><span class="sxs-lookup"><span data-stu-id="40c8b-115">This is by design and not an error.</span></span>

<span data-ttu-id="40c8b-116">Wybierz pozycję **Akceptuj** i **Kontynuuj** , aby kontynuować.</span><span class="sxs-lookup"><span data-stu-id="40c8b-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="40c8b-117">Jeśli dział IT wyłączył **Rejestrowanie w centrum partnerskim** .</span><span class="sxs-lookup"><span data-stu-id="40c8b-117">If the IT department has turned off **sign up for Partner Center** .</span></span>

<span data-ttu-id="40c8b-118">Zobaczysz ten komunikat, ponieważ użytkownicy z wirusami są wyłączeni lub że wirusowe rejestrowanie w dzierżawie usługi Azure AD jest wyłączone.</span><span class="sxs-lookup"><span data-stu-id="40c8b-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="40c8b-119">Administrator globalny dla konta usługi Azure AD może włączyć wymagane funkcje, uruchamiając następujące polecenie programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="40c8b-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="40c8b-120">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="40c8b-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="40c8b-121">Aby uzyskać więcej informacji, zapoznaj się z artykułem [rejestracja samoobsługowa](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="40c8b-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="40c8b-122">Nie pamiętasz hasła</span><span class="sxs-lookup"><span data-stu-id="40c8b-122">You forgot your password</span></span>

<span data-ttu-id="40c8b-123">Jeśli zapomniano hasło, wybierz link **nie można uzyskać dostępu do konta?** na stronie logowania.</span><span class="sxs-lookup"><span data-stu-id="40c8b-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="40c8b-124">Ta opcja umożliwia zresetowanie hasła lub poproszenie administratora globalnego o przypisanie nowych poświadczeń.</span><span class="sxs-lookup"><span data-stu-id="40c8b-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="40c8b-125">W Scree "Powiedz nam o swojej firmie" pojawia się błąd "coś poszło źle"</span><span class="sxs-lookup"><span data-stu-id="40c8b-125">On the “Tell us about your company” scree, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="40c8b-126">Ten komunikat o błędzie jest zwykle wyświetlany, jeśli przypadkowo użyto znaków specjalnych, spacji lub kodu kraju w numerze telefonu firmy.</span><span class="sxs-lookup"><span data-stu-id="40c8b-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="40c8b-127">Wartość wprowadzona w polu numer telefonu może zawierać maksymalnie 10 znaków.</span><span class="sxs-lookup"><span data-stu-id="40c8b-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="40c8b-128">Zakup karty kredytowej otrzymuje komunikat o błędzie z informacją o tym, że zamówienie zostało odrzucone.</span><span class="sxs-lookup"><span data-stu-id="40c8b-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="40c8b-129">Sprawdź swoje informacje "</span><span class="sxs-lookup"><span data-stu-id="40c8b-129">Please verify your information”</span></span>


<span data-ttu-id="40c8b-130">Zawsze używaj adresu odpowiadającego karcie kredytowej, a nie podmiotowi prawnemu.</span><span class="sxs-lookup"><span data-stu-id="40c8b-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="40c8b-131">Upewnij się również, że kod pocztowy jest poprawny i odpowiada adresowi, którego używasz.</span><span class="sxs-lookup"><span data-stu-id="40c8b-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="40c8b-132">Chcesz przełączyć się z płatności offline do formy płatności online</span><span class="sxs-lookup"><span data-stu-id="40c8b-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="40c8b-133">Musisz anulować oryginalne zamówienie i ponownie kupić przy użyciu preferowanej metody płatności.</span><span class="sxs-lookup"><span data-stu-id="40c8b-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="40c8b-134">Aby anulować zamówienie:</span><span class="sxs-lookup"><span data-stu-id="40c8b-134">To cancel an order:</span></span>

1. <span data-ttu-id="40c8b-135">Wybierz kartę **oferty członkostwa** na pulpicie nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="40c8b-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="40c8b-136">Wybierz pozycję **Anuluj zamówienie**</span><span class="sxs-lookup"><span data-stu-id="40c8b-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="40c8b-137">Zostanie wyświetlone okno potwierdzenia i musisz potwierdzić, aby anulować kolejność początkową.</span><span class="sxs-lookup"><span data-stu-id="40c8b-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="40c8b-138">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="40c8b-138">Next steps</span></span>

- [<span data-ttu-id="40c8b-139">Zarządzanie kontem w portalu Partner Center</span><span class="sxs-lookup"><span data-stu-id="40c8b-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="40c8b-140">Jak odczytać plik rachunku i Rekonesans</span><span class="sxs-lookup"><span data-stu-id="40c8b-140">How to read your bill and recon file</span></span>](read-your-bill.md)