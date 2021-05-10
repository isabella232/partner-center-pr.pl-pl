---
title: Rozwiązywanie problemów z konfigurowaniem konta Partner Center lub odnawiania MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Rozwiązywanie problemów podczas próby zarejestrowania się w Partner Center. Odpowiada na wyzwania związane z metodami płatności, zapomnianiem haseł i nie tylko.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686266"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="2fbc4-104">Rozwiązywanie problemów z konfiguracją konta lub odnawianiem mpn</span><span class="sxs-lookup"><span data-stu-id="2fbc4-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="2fbc4-105">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="2fbc4-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2fbc4-106">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="2fbc4-106">Global admin</span></span>
- <span data-ttu-id="2fbc4-107">Administrator partnera MPN</span><span class="sxs-lookup"><span data-stu-id="2fbc4-107">MPN partner admin</span></span>
 
<span data-ttu-id="2fbc4-108">Poniżej znajdują się sugestie dotyczące rozwiązywania typowych problemów występujących podczas konfigurowania Partner Center konta.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="2fbc4-109">Co się stanie, jeśli migrujesz z Partner Membership Center i nie możesz edytować żadnych pól informacji o firmie</span><span class="sxs-lookup"><span data-stu-id="2fbc4-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="2fbc4-110">W przypadkach, gdy firma jest już obecna w Partner Center (na przykład na koncie CSP) — zostanie wyświetlone ekran tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="2fbc4-111">Na tym ekranie będą wyświetlane wszystkie informacje o firmie, które istnieją w Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="2fbc4-112">Nie można zmienić szczegółów na tym ekranie.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-112">You can't change the details on this screen.</span></span> <span data-ttu-id="2fbc4-113">Jest to projektowe, a nie błędne.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-113">This is by design and not an error.</span></span>

<span data-ttu-id="2fbc4-114">Wybierz **pozycję Zaakceptuj** i **kontynuuj,** aby kontynuować.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="2fbc4-115">Jeśli dział IT wyłączył logowanie **do Partner Center**</span><span class="sxs-lookup"><span data-stu-id="2fbc4-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="2fbc4-116">Zostanie wyświetlony ten komunikat, ponieważ użytkownicy są wyłączeni lub rejestracja za pomocą oprogramowania marketingowego jest wyłączona w dzierżawie usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="2fbc4-117">Administrator globalny konta usługi Azure AD może włączyć wymagane funkcje, uruchamiając następujące polecenie programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2fbc4-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="2fbc4-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="2fbc4-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="2fbc4-119">Aby uzyskać więcej informacji, zapoznaj [się z tematem Self-service sign up (Rejestracja samoobsługowa).](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="2fbc4-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="2fbc4-120">Nie pamiętasz hasła</span><span class="sxs-lookup"><span data-stu-id="2fbc4-120">You forgot your password</span></span>

<span data-ttu-id="2fbc4-121">Jeśli nie pamiętasz hasła, wybierz link Nie **możesz uzyskać dostępu do konta?** na stronie logowania.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="2fbc4-122">Ta opcja umożliwia zresetowanie hasła lub poproś administratora globalnego o przypisanie Ci nowych poświadczeń.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="2fbc4-123">Na ekranie "Poinformuj nas o swojej firmie" zostanie wyświetlony błąd "Wystąpił problem"</span><span class="sxs-lookup"><span data-stu-id="2fbc4-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="2fbc4-124">Ten komunikat o błędzie jest zwykle wyświetlany, jeśli przypadkowo używasz znaków specjalnych, spacji lub kodu kraju w firmowym numerze telefonu.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="2fbc4-125">Wartość wprowadzona w polu Numer telefonu może zawierać maksymalnie 10 znaków.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="2fbc4-126">Podczas zakupu karty kredytowej jest wyświetlany komunikat o błędzie informujący, że "Twoje zamówienie zostało odrzucone.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="2fbc4-127">Sprawdź swoje informacje"</span><span class="sxs-lookup"><span data-stu-id="2fbc4-127">Please verify your information”</span></span>


<span data-ttu-id="2fbc4-128">Zawsze używaj adresu odpowiadającego karcie kredytowej, a nie jednostki prawnej.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="2fbc4-129">Upewnij się również, że kod pocztowy jest poprawny i odpowiada adresowi, z których korzystasz.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="2fbc4-130">Chcesz przełączyć się z płatności w trybie offline na formę płatności online</span><span class="sxs-lookup"><span data-stu-id="2fbc4-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="2fbc4-131">Musisz anulować oryginalne zamówienie i ponownie je zkupić przy użyciu preferowanej formy płatności.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="2fbc4-132">Aby anulować zamówienie:</span><span class="sxs-lookup"><span data-stu-id="2fbc4-132">To cancel an order:</span></span>

1. <span data-ttu-id="2fbc4-133">Wybierz **kartę Oferty** członkostwa na pulpicie nawigacyjnym.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="2fbc4-134">Wybierz **pozycję Anuluj zamówienie**</span><span class="sxs-lookup"><span data-stu-id="2fbc4-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="2fbc4-135">Zostanie wyświetlone okno potwierdzenia z potwierdzeniem, które należy potwierdzić, aby anulować początkowe zamówienie.</span><span class="sxs-lookup"><span data-stu-id="2fbc4-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2fbc4-136">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="2fbc4-136">Next steps</span></span>

- [<span data-ttu-id="2fbc4-137">Zarządzanie kontem w portalu Partner Center</span><span class="sxs-lookup"><span data-stu-id="2fbc4-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="2fbc4-138">Jak odczytać rachunek i ponownie skonfigurować plik</span><span class="sxs-lookup"><span data-stu-id="2fbc4-138">How to read your bill and recon file</span></span>](read-your-bill.md)
