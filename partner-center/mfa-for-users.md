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
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/16/2020
ms.locfileid: "97579980"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="993a3-103">Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego</span><span class="sxs-lookup"><span data-stu-id="993a3-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="993a3-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="993a3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="993a3-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="993a3-105">Global admin</span></span>

<span data-ttu-id="993a3-106">Lepsze zabezpieczenia i bezpieczeństwo ochrony prywatności znajdują się wśród naszych najważniejszych priorytetów.</span><span class="sxs-lookup"><span data-stu-id="993a3-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="993a3-107">Wiemy, że najlepszą obroną jest zapobieganie i że jest to tylko silne rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="993a3-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="993a3-108">Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie mogli działać i zapewnić odpowiednie zabezpieczenia.</span><span class="sxs-lookup"><span data-stu-id="993a3-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="993a3-109">Zdecydowanie zalecamy, aby wszyscy partnerzy mogli korzystać z uwierzytelniania wieloskładnikowego (MFA) dla swoich użytkowników w dzierżawie partnera.</span><span class="sxs-lookup"><span data-stu-id="993a3-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="993a3-110">Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników</span><span class="sxs-lookup"><span data-stu-id="993a3-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="993a3-111">Aby wykonać to zadanie, musisz być administratorem globalnym Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="993a3-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="993a3-112">Najprostszym rozwiązaniem jest włączenie usługi MFA dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="993a3-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="993a3-113">Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do pozycji **Zarządzanie użytkownikami**.</span><span class="sxs-lookup"><span data-stu-id="993a3-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="993a3-114">Wybierz pozycję **uwierzytelnianie wieloskładnikowe**.</span><span class="sxs-lookup"><span data-stu-id="993a3-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="993a3-115">Wybierz użytkownika, który chcesz włączyć, a następnie wybierz pozycję **Włącz**.</span><span class="sxs-lookup"><span data-stu-id="993a3-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="993a3-116">Spowoduje to włączenie usługi MFA dla tego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="993a3-116">This will enable MFA for this user.</span></span> <span data-ttu-id="993a3-117">Włączona oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji usługi MFA podczas pierwszego logowania.</span><span class="sxs-lookup"><span data-stu-id="993a3-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="993a3-118">Po zalogowaniu zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem wiadomości e-mail lub wiadomości SMS (w zależności od konfiguracji).</span><span class="sxs-lookup"><span data-stu-id="993a3-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Określ sposób weryfikacji":::

>[!NOTE]
><span data-ttu-id="993a3-120">Możesz **wymusić** , aby użytkownicy korzystali z usługi MFA, wykonując te same kroki, jak powyżej, i wybierając pozycję **Wymuszaj**.</span><span class="sxs-lookup"><span data-stu-id="993a3-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="993a3-121">Aby dowiedzieć się więcej, przeczytaj artykuł [Włączanie usługi Azure Multi-Factor Authentication dla poszczególnych użytkowników w celu zabezpieczenia zdarzeń związanych z logowaniem](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="993a3-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="993a3-122">Wszyscy użytkownicy zaczynają **wyłączać**.</span><span class="sxs-lookup"><span data-stu-id="993a3-122">All users start out **Disabled**.</span></span> <span data-ttu-id="993a3-123">Gdy rejestrujesz użytkowników w usłudze Azure Multi-Factor Authentication dla poszczególnych użytkowników, ich stan zmieni się na **włączone**.</span><span class="sxs-lookup"><span data-stu-id="993a3-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="993a3-124">Gdy użytkownicy będą mogli się zalogować i zakończyć proces rejestracji, ich stan zmieni się na **wymuszone**.</span><span class="sxs-lookup"><span data-stu-id="993a3-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="993a3-125">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="993a3-125">Next steps</span></span>

- [<span data-ttu-id="993a3-126">Przypisywanie ról i uprawnień do użytkowników</span><span class="sxs-lookup"><span data-stu-id="993a3-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

