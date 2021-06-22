---
title: Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Dowiedz się, jak skonfigurować pracowników przy użyciu usługi MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450811"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="ea382-103">Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego</span><span class="sxs-lookup"><span data-stu-id="ea382-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="ea382-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="ea382-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="ea382-105">Naszymi najwyższymi priorytetami są większe zabezpieczenia i ochrona prywatności.</span><span class="sxs-lookup"><span data-stu-id="ea382-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="ea382-106">Wiemy, że najlepszą obroną jest zapobieganie i że jesteśmy tylko tak silni, jak nasze słabe łącze.</span><span class="sxs-lookup"><span data-stu-id="ea382-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="ea382-107">Dlatego potrzebujemy wszystkich w naszym ekosystemie, aby działać i zapewnić odpowiednie zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="ea382-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="ea382-108">Zdecydowanie zalecamy, aby wszyscy partnerzy włączyli uwierzytelnianie wieloskładnikowe (MFA) dla swoich użytkowników w dzierżawie partnera.</span><span class="sxs-lookup"><span data-stu-id="ea382-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="ea382-109">Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="ea382-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="ea382-110">Aby wykonać to zadanie, musisz być administratorem globalnym w swojej firmie.</span><span class="sxs-lookup"><span data-stu-id="ea382-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="ea382-111">Najłatwiej jest włączyć usługę MFA dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ea382-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="ea382-112">Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do **tematu User management (Zarządzanie użytkownikami).**</span><span class="sxs-lookup"><span data-stu-id="ea382-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="ea382-113">Wybierz **pozycję Uwierzytelnianie wieloskładnikowe.**</span><span class="sxs-lookup"><span data-stu-id="ea382-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="ea382-114">Wybierz użytkownika, którego chcesz włączyć, a następnie wybierz pozycję **Włącz.**</span><span class="sxs-lookup"><span data-stu-id="ea382-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="ea382-115">Spowoduje to włączenie uwierzytelniania wieloskładnikowego dla tego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="ea382-115">This will enable MFA for this user.</span></span> <span data-ttu-id="ea382-116">Włączone oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji MFA podczas pierwszego logowania.</span><span class="sxs-lookup"><span data-stu-id="ea382-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="ea382-117">Później podczas logowania zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem poczty e-mail lub wiadomości SMS (w zależności od tego, która konfiguracja została przez nich wysłana).</span><span class="sxs-lookup"><span data-stu-id="ea382-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Określ sposób weryfikacji.":::

>[!NOTE]
><span data-ttu-id="ea382-119">Możesz **wymusić użycie** usługi MFA przez użytkowników, korzystając z powyższych kroków i wybierając pozycję **Wymuszaj.**</span><span class="sxs-lookup"><span data-stu-id="ea382-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="ea382-120">Aby dowiedzieć się więcej, przeczytaj włączanie usługi [Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-userstates)dla uwierzytelniania na użytkownika w celu zabezpieczenia zdarzeń logowania.</span><span class="sxs-lookup"><span data-stu-id="ea382-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="ea382-121">Wszyscy użytkownicy zaczynają od **wyłączonej .**</span><span class="sxs-lookup"><span data-stu-id="ea382-121">All users start out **Disabled**.</span></span> <span data-ttu-id="ea382-122">W przypadku rejestrowania użytkowników w usługach Azure Active Directory Multi-Factor Authentication ich stan zmienia się na **Włączone.**</span><span class="sxs-lookup"><span data-stu-id="ea382-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="ea382-123">Po włączeniu logowania użytkowników i ukończeniu procesu rejestracji ich stan zmienia się na **Wymuszone.**</span><span class="sxs-lookup"><span data-stu-id="ea382-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ea382-124">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="ea382-124">Next steps</span></span>

- [<span data-ttu-id="ea382-125">Przypisywanie ról i uprawnień do użytkowników</span><span class="sxs-lookup"><span data-stu-id="ea382-125">Assign roles and permissions to users</span></span>](permissions-overview.md)