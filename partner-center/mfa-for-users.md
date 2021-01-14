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
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182379"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Konfigurowanie użytkowników przy użyciu uwierzytelniania wieloskładnikowego

**Odpowiednie role**

- Administrator globalny

Lepsze zabezpieczenia i bezpieczeństwo ochrony prywatności znajdują się wśród naszych najważniejszych priorytetów. Wiemy, że najlepszą obroną jest zapobieganie i że jest to tylko silne rozwiązanie. Dlatego potrzebujemy, aby wszyscy w naszym ekosystemie mogli działać i zapewnić odpowiednie zabezpieczenia. Zdecydowanie zalecamy, aby wszyscy partnerzy mogli korzystać z uwierzytelniania wieloskładnikowego (MFA) dla swoich użytkowników w dzierżawie partnera. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Dodawanie uwierzytelniania wieloskładnikowego dla użytkowników

Aby wykonać to zadanie, musisz być administratorem globalnym Twojej firmy.

Najprostszym rozwiązaniem jest włączenie usługi MFA dla użytkowników podczas dodawania ich do dzierżawy usługi Azure AD.

1. Zaloguj się do [Azure Portal](https://portal.azure.com) a następnie przejdź do pozycji **Zarządzanie użytkownikami**.
1. Wybierz pozycję **uwierzytelnianie wieloskładnikowe**.
1. Wybierz użytkownika, który chcesz włączyć, a następnie wybierz pozycję **Włącz**.

Spowoduje to włączenie usługi MFA dla tego użytkownika. Włączona oznacza, że użytkownik zostanie poproszony o skonfigurowanie weryfikacji usługi MFA podczas pierwszego logowania. Po zalogowaniu zostanie wyświetlony monit o podanie kodu wysłanego do nich za pośrednictwem wiadomości e-mail lub wiadomości SMS (w zależności od konfiguracji).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Określ sposób weryfikacji":::

>[!NOTE]
>Możesz **wymusić** , aby użytkownicy korzystali z usługi MFA, wykonując te same kroki, jak powyżej, i wybierając pozycję **Wymuszaj**. Aby dowiedzieć się więcej, przeczytaj artykuł [Włączanie usługi Azure Multi-Factor Authentication dla poszczególnych użytkowników w celu zabezpieczenia zdarzeń związanych z logowaniem](/azure/active-directory/authentication/howto-mfa-userstates). 

Wszyscy użytkownicy zaczynają **wyłączać**. Gdy rejestrujesz użytkowników w usłudze Azure Multi-Factor Authentication dla poszczególnych użytkowników, ich stan zmieni się na **włączone**. Gdy użytkownicy będą mogli się zalogować i zakończyć proces rejestracji, ich stan zmieni się na **wymuszone**. 

## <a name="next-steps"></a>Następne kroki

- [Przypisywanie ról i uprawnień do użytkowników](permissions-overview.md)