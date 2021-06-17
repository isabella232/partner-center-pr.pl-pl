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
ms.openlocfilehash: 37373c032dc34315c0e3274987805d7518d0b595
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276607"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego

**Odpowiednie role:** Administrator globalny

Naszymi najwyższymi priorytetami są większe zabezpieczenia i ochrona prywatności. Wiemy, że najlepszą obroną jest zapobieganie i że jesteśmy tylko tak silni, jak nasze słabe łącze. Dlatego potrzebujemy wszystkich w naszym ekosystemie, aby działać i zapewnić odpowiednie zabezpieczenia. Zdecydowanie zalecamy, aby wszyscy partnerzy włączyli uwierzytelnianie wieloskładnikowe (MFA) dla swoich użytkowników w dzierżawie partnera. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników

Aby wykonać to zadanie, musisz być administratorem globalnym w swojej firmie.

Najłatwiej jest włączyć usługę MFA dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.

1. Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do **tematu User management (Zarządzanie użytkownikami).**
1. Wybierz **pozycję Uwierzytelnianie wieloskładnikowe.**
1. Wybierz użytkownika, którego chcesz włączyć, a następnie wybierz pozycję **Włącz.**

Spowoduje to włączenie uwierzytelniania wieloskładnikowego dla tego użytkownika. Włączone oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji MFA podczas pierwszego logowania. Później podczas logowania zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem poczty e-mail lub wiadomości SMS (w zależności od tego, która konfiguracja została przez nich wysłana).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Określ sposób weryfikacji.":::

>[!NOTE]
>Możesz **wymusić użycie** usługi MFA przez użytkowników, korzystając z powyższych kroków i wybierając pozycję **Wymuszaj.** Aby dowiedzieć się więcej, przeczytaj włączanie usługi [Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-userstates)dla uwierzytelniania na użytkownika w celu zabezpieczenia zdarzeń logowania. 

Wszyscy użytkownicy zaczynają od **wyłączonej .** W przypadku rejestrowania użytkowników w usługach Azure Active Directory Multi-Factor Authentication ich stan zmienia się na **Włączone.** Po włączeniu logowania użytkowników i ukończeniu procesu rejestracji ich stan zmienia się na **Wymuszone.** 

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień do użytkowników](permissions-overview.md)