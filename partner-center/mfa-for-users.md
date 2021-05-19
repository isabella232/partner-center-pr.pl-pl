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
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego

**Odpowiednie role:** Administrator globalny

Naszymi najwyższymi priorytetami są większe zabezpieczenia prywatności i bezpieczeństwo. Wiemy, że najlepszą obroną jest zapobieganie i że jesteśmy tylko tak silni jak nasze słabe łącze. Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie działali i zapewniali odpowiednie zabezpieczenia. Zdecydowanie zalecamy, aby wszyscy partnerzy włączyli uwierzytelnianie wieloskładnikowe (MFA) dla swoich użytkowników w dzierżawie partnera. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników

Aby wykonać to zadanie, musisz być administratorem globalnym w swojej firmie.

Najłatwiej jest włączyć usługę MFA dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.

1. Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do **tematu Zarządzanie użytkownikami.**
1. Wybierz **pozycję Uwierzytelnianie wieloskładnikowe.**
1. Wybierz użytkownika, którego chcesz włączyć, a następnie wybierz pozycję **Włącz.**

Spowoduje to włączenie uwierzytelniania wieloskładnikowego dla tego użytkownika. Wartość Włączone oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji MFA podczas pierwszego logowania. Następnie podczas logowania zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem poczty e-mail lub wiadomości SMS (w zależności od tego, która konfiguracja została przez nich wysłana).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Określanie sposobu weryfikacji":::

>[!NOTE]
>Możesz **wymusić użycie** uwierzytelniania wieloskładnikowego przez użytkowników, korzystając z powyższych kroków i wybierając pozycję **Wymuszaj.** Aby dowiedzieć się więcej, przeczytaj [włączanie usługi Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-userstates)dla 1 użytkownika w celu zabezpieczenia zdarzeń logowania. 

Wszyscy użytkownicy zaczynają od **wyłączonego .** W przypadku rejestrowania użytkowników w usługach Azure Active Directory Multi-Factor Authentication ich stan zmieni się na **Włączone.** Po włączeniu logowania użytkowników i ukończeniu procesu rejestracji ich stan zmieni się na **Wymuszone.** 

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień do użytkowników](permissions-overview.md)