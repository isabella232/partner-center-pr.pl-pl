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
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151631"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="bc94e-103">Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego</span><span class="sxs-lookup"><span data-stu-id="bc94e-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="bc94e-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="bc94e-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="bc94e-105">Naszymi najwyższymi priorytetami są większe zabezpieczenia prywatności i bezpieczeństwo.</span><span class="sxs-lookup"><span data-stu-id="bc94e-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="bc94e-106">Wiemy, że najlepszą obroną jest zapobieganie i że jesteśmy tylko tak silni jak nasze słabe łącze.</span><span class="sxs-lookup"><span data-stu-id="bc94e-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="bc94e-107">Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie działali i zapewniali odpowiednie zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="bc94e-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="bc94e-108">Zdecydowanie zalecamy, aby wszyscy partnerzy włączyli uwierzytelnianie wieloskładnikowe (MFA) dla swoich użytkowników w dzierżawie partnera.</span><span class="sxs-lookup"><span data-stu-id="bc94e-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="bc94e-109">Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="bc94e-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="bc94e-110">Aby wykonać to zadanie, musisz być administratorem globalnym w swojej firmie.</span><span class="sxs-lookup"><span data-stu-id="bc94e-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="bc94e-111">Najłatwiej jest włączyć usługę MFA dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bc94e-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="bc94e-112">Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do **tematu Zarządzanie użytkownikami.**</span><span class="sxs-lookup"><span data-stu-id="bc94e-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="bc94e-113">Wybierz **pozycję Uwierzytelnianie wieloskładnikowe.**</span><span class="sxs-lookup"><span data-stu-id="bc94e-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="bc94e-114">Wybierz użytkownika, którego chcesz włączyć, a następnie wybierz pozycję **Włącz.**</span><span class="sxs-lookup"><span data-stu-id="bc94e-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="bc94e-115">Spowoduje to włączenie uwierzytelniania wieloskładnikowego dla tego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="bc94e-115">This will enable MFA for this user.</span></span> <span data-ttu-id="bc94e-116">Wartość Włączone oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji MFA podczas pierwszego logowania.</span><span class="sxs-lookup"><span data-stu-id="bc94e-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="bc94e-117">Następnie podczas logowania zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem poczty e-mail lub wiadomości SMS (w zależności od tego, która konfiguracja została przez nich wysłana).</span><span class="sxs-lookup"><span data-stu-id="bc94e-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Określanie sposobu weryfikacji":::

>[!NOTE]
><span data-ttu-id="bc94e-119">Możesz **wymusić użycie** uwierzytelniania wieloskładnikowego przez użytkowników, korzystając z powyższych kroków i wybierając pozycję **Wymuszaj.**</span><span class="sxs-lookup"><span data-stu-id="bc94e-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="bc94e-120">Aby dowiedzieć się więcej, przeczytaj [włączanie usługi Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-userstates)dla 1 użytkownika w celu zabezpieczenia zdarzeń logowania.</span><span class="sxs-lookup"><span data-stu-id="bc94e-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="bc94e-121">Wszyscy użytkownicy zaczynają od **wyłączonego .**</span><span class="sxs-lookup"><span data-stu-id="bc94e-121">All users start out **Disabled**.</span></span> <span data-ttu-id="bc94e-122">W przypadku rejestrowania użytkowników w usługach Azure Active Directory Multi-Factor Authentication ich stan zmieni się na **Włączone.**</span><span class="sxs-lookup"><span data-stu-id="bc94e-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="bc94e-123">Po włączeniu logowania użytkowników i ukończeniu procesu rejestracji ich stan zmieni się na **Wymuszone.**</span><span class="sxs-lookup"><span data-stu-id="bc94e-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bc94e-124">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="bc94e-124">Next steps</span></span>

- [<span data-ttu-id="bc94e-125">Przypisywanie ról i uprawnień do użytkowników</span><span class="sxs-lookup"><span data-stu-id="bc94e-125">Assign roles and permissions to users</span></span>](permissions-overview.md)