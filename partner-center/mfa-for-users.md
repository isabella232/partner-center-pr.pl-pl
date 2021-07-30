---
title: Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Dowiedz się, jak skonfigurować pracowników przy użyciu usługi MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ee457193a23de0601b60b2291cdee985aceaaeb8
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114846115"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego

**Odpowiednie role:** Administrator globalny

Naszymi najwyższymi priorytetami są większe zabezpieczenia prywatności i bezpieczeństwo. Wiemy, że najlepszą obroną jest zapobieganie i że jesteśmy tylko tak silni jak nasze słabe łącze. Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie działali i zapewniali odpowiednie zabezpieczenia. Zdecydowanie zalecamy, aby wszyscy partnerzy włączyli uwierzytelnianie wieloskładnikowe (MFA) dla swoich użytkowników w dzierżawie partnera. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników

Aby wykonać to zadanie, musisz być administratorem globalnym w swojej firmie.

Najłatwiej jest włączyć uwierzytelniania wieloskładnikowego dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.

1. Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do **tematu Zarządzanie użytkownikami.**
1. Wybierz **pozycję Uwierzytelnianie wieloskładnikowe.**
1. Wybierz użytkownika, którego chcesz włączyć, a następnie wybierz pozycję **Włącz.**

Spowoduje to włączenie uwierzytelniania wieloskładnikowego dla tego użytkownika. Włączone oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji MFA podczas pierwszego logowania. Następnie podczas logowania zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem poczty e-mail lub wiadomości SMS (w zależności od tego, która konfiguracja została przez nich wysłana).  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Określ sposób weryfikacji.":::

>[!NOTE]
>Możesz **wymusić użycie** uwierzytelniania wieloskładnikowego przez użytkowników, korzystając z powyższych kroków i wybierając pozycję **Wymuszaj.** Aby dowiedzieć się więcej, przeczytaj [włączanie usługi Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-userstates)dla 1 użytkownika w celu zabezpieczenia zdarzeń logowania. 

Wszyscy użytkownicy zaczynają od **wyłączonego .** Po zarejestrowaniu użytkowników w u użytkownikach Azure Active Directory Multi-Factor Authentication ich stan zmieni się na **Włączone.** Po włączeniu logowania użytkowników i ukończeniu procesu rejestracji ich stan zmieni się na **Wymuszone.** 

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień do użytkowników](permissions-overview.md)