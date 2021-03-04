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
ms.openlocfilehash: 9622f02039360e8ab39f459c9a2fe082ec70c854
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756743"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="56ec9-104">Rozwiązywanie problemów z konfiguracją konta lub MPN odnowienia</span><span class="sxs-lookup"><span data-stu-id="56ec9-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="56ec9-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="56ec9-105">**Appropriate roles**</span></span>

- <span data-ttu-id="56ec9-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="56ec9-106">Global admin</span></span>
- <span data-ttu-id="56ec9-107">Administrator partnerski MPN</span><span class="sxs-lookup"><span data-stu-id="56ec9-107">MPN partner admin</span></span> 
 
<span data-ttu-id="56ec9-108">Poniżej przedstawiono kilka sugestii dotyczących rozwiązywania typowych problemów, które powstają podczas konfigurowania konta Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="56ec9-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="56ec9-109">Co się stanie w przypadku migrowania z Centrum członkostwa w partnerze i nie można edytować żadnych pól informacji o firmie</span><span class="sxs-lookup"><span data-stu-id="56ec9-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="56ec9-110">W przypadkach, w których firma ma już obecność w centrum partnerskim (podyktuj konto CSP) — zostanie wyświetlony ekran tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="56ec9-110">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="56ec9-111">Na tym ekranie zostaną wyświetlone wszystkie informacje o firmie, które istnieją w centrum partnerskim.</span><span class="sxs-lookup"><span data-stu-id="56ec9-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="56ec9-112">Nie można zmienić szczegółów na tym ekranie.</span><span class="sxs-lookup"><span data-stu-id="56ec9-112">You can't change the details on this screen.</span></span> <span data-ttu-id="56ec9-113">Jest to zgodne z projektem, a nie błędem.</span><span class="sxs-lookup"><span data-stu-id="56ec9-113">This is by design and not an error.</span></span>

<span data-ttu-id="56ec9-114">Wybierz pozycję **Akceptuj** i **Kontynuuj** , aby kontynuować.</span><span class="sxs-lookup"><span data-stu-id="56ec9-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="56ec9-115">Jeśli dział IT wyłączył **Rejestrowanie w centrum partnerskim**.</span><span class="sxs-lookup"><span data-stu-id="56ec9-115">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="56ec9-116">Zobaczysz ten komunikat, ponieważ użytkownicy z wirusami są wyłączeni lub że wirusowe rejestrowanie w dzierżawie usługi Azure AD jest wyłączone.</span><span class="sxs-lookup"><span data-stu-id="56ec9-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="56ec9-117">Administrator globalny dla konta usługi Azure AD może włączyć wymagane funkcje, uruchamiając następujące polecenie programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="56ec9-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="56ec9-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="56ec9-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="56ec9-119">Aby uzyskać więcej informacji, zapoznaj się z artykułem [rejestracja samoobsługowa](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="56ec9-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="56ec9-120">Nie pamiętasz hasła</span><span class="sxs-lookup"><span data-stu-id="56ec9-120">You forgot your password</span></span>

<span data-ttu-id="56ec9-121">Jeśli zapomniano hasło, wybierz link **nie można uzyskać dostępu do konta?** na stronie logowania.</span><span class="sxs-lookup"><span data-stu-id="56ec9-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="56ec9-122">Ta opcja umożliwia zresetowanie hasła lub poproszenie administratora globalnego o przypisanie nowych poświadczeń.</span><span class="sxs-lookup"><span data-stu-id="56ec9-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="56ec9-123">Na ekranie "Powiedz nam o swojej firmie" pojawia się błąd "coś poszło źle"</span><span class="sxs-lookup"><span data-stu-id="56ec9-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="56ec9-124">Ten komunikat o błędzie jest zwykle wyświetlany, jeśli przypadkowo użyto znaków specjalnych, spacji lub kodu kraju w numerze telefonu firmy.</span><span class="sxs-lookup"><span data-stu-id="56ec9-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="56ec9-125">Wartość wprowadzona w polu numer telefonu może zawierać maksymalnie 10 znaków.</span><span class="sxs-lookup"><span data-stu-id="56ec9-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="56ec9-126">Zakup karty kredytowej otrzymuje komunikat o błędzie z informacją o tym, że zamówienie zostało odrzucone.</span><span class="sxs-lookup"><span data-stu-id="56ec9-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="56ec9-127">Sprawdź swoje informacje "</span><span class="sxs-lookup"><span data-stu-id="56ec9-127">Please verify your information”</span></span>


<span data-ttu-id="56ec9-128">Zawsze używaj adresu odpowiadającego karcie kredytowej, a nie podmiotowi prawnemu.</span><span class="sxs-lookup"><span data-stu-id="56ec9-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="56ec9-129">Upewnij się również, że kod pocztowy jest poprawny i odpowiada adresowi, którego używasz.</span><span class="sxs-lookup"><span data-stu-id="56ec9-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="56ec9-130">Chcesz przełączyć się z płatności offline do formy płatności online</span><span class="sxs-lookup"><span data-stu-id="56ec9-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="56ec9-131">Musisz anulować oryginalne zamówienie i ponownie kupić przy użyciu preferowanej metody płatności.</span><span class="sxs-lookup"><span data-stu-id="56ec9-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="56ec9-132">Aby anulować zamówienie:</span><span class="sxs-lookup"><span data-stu-id="56ec9-132">To cancel an order:</span></span>

1. <span data-ttu-id="56ec9-133">Wybierz kartę **oferty członkostwa** na pulpicie nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="56ec9-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="56ec9-134">Wybierz pozycję **Anuluj zamówienie**</span><span class="sxs-lookup"><span data-stu-id="56ec9-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="56ec9-135">Zostanie wyświetlone okno potwierdzenia i musisz potwierdzić, aby anulować kolejność początkową.</span><span class="sxs-lookup"><span data-stu-id="56ec9-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="56ec9-136">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="56ec9-136">Next steps</span></span>

- [<span data-ttu-id="56ec9-137">Zarządzanie kontem w portalu Partner Center</span><span class="sxs-lookup"><span data-stu-id="56ec9-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="56ec9-138">Jak odczytać plik rachunku i Rekonesans</span><span class="sxs-lookup"><span data-stu-id="56ec9-138">How to read your bill and recon file</span></span>](read-your-bill.md)
