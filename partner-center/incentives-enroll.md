---
title: Zachęty rejestracji
ms.topic: how-to
ms.date: 04/15/2021
description: Zarejestruj się w programie zachęt i przypisz role niezbędne do zarządzania użytkownikami. W tym artykule opisano proces rejestracji.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: f3be1b1d267321a4229ba3ea56aa950e14538289
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958593"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a>Rejestracja i zarządzanie użytkownikami w programie zachęt

**Odpowiednie role:** Administrator zachęt

>[!NOTE]
>Aby zarejestrować się w programie zachęt, musisz ukończyć migrację Partner Membership Center Partner Center [programu](./partner-membership-center-retirement-faq.md).

Proces rejestracji składa się z dwóch kroków.

**Krok 1. Zarządzanie użytkownikami:** Ten krok obejmuje ustanowienie administratora zachęt w Partner Center.

**Krok 2. Rejestracja:** firma Microsoft wysyła zaproszenie do zarejestrowania się w programie zachęt.

## <a name="user-management"></a>Zarządzanie użytkownikami

Aby zarejestrować się w programie zachęt Partner Center, administrator administrator globalny lub administrator konta musi skonfigurować użytkowników firmowych jako administratorów zachęt. Aby uzyskać informacje o kontach partnerów, rolach i uprawnieniach, zobacz [Manage your Partner Center account (Zarządzanie kontem partnerskim).](partner-center-account-setup.md) Usługa administrator globalny również skonfigurować użytkowników firmy za pośrednictwem usługi Azure Active Directory (Azure AD).

>[!NOTE]
>Tylko administrator zachęt może zarejestrować się w programach zachęt. Jeśli w Twojej lokalizacji nie ma administratora zachęt, administrator administrator globalny i administrator konta musi go przypisać. Administrator zachęty musi być przypisany do identyfikatorów MPN lokalizacji. Administrator administrator globalny lub administrator konta może być również przypisany jako administrator zachęty. Aby dowiedzieć się więcej o różnych rolach, zobacz [Zarządzanie zachętami.](permissions-overview.md#manage-incentives)

## <a name="enrollment-process"></a>Proces rejestracji

Gdy Organizacja kwalifikuje się do korzystania z zachęt, firma Microsoft wyśle zaproszenie do administratora zachęty kwalifikującego się pliku MPNLocationID, aby rozpocząć proces rejestracji. Ta wiadomość e-mail zostanie wysłana z Partner Center **firmy Microsoft** i będzie mieć temat Zaproszenie do rejestracji **zachęt partnera.** Otwórz zaproszenie i wybierz pozycję **Wprowadzenie**.

Na stronie głównej aplikacji zostanie również Partner Center zaproszenie. Po wybraniu tego komunikatu nie będzie można go wyświetlić ponownie. Administrator zachęty może jednak ukończyć ten proces, logując się  do pulpitu nawigacyjnego Partner Center nawigacyjnym i wybierając pozycję [Przegląd](https://partner.microsoft.com/dashboard/) w obszarze **Zachęty** w lewym okienku nawigacyjnym. Wybierz **pozycję Zarejestruj,** a następnie wypełnij profil wypłaty i profil podatkowy dla programu.

Jeśli masz już domyślną konfigurację profilu bankowego dla lokalizacji MPN i próbujesz zarejestrować się w  tej samej lokalizacji MPN w programie zachęt, po wybraniu pozycji Zarejestruj i zaakceptowaniu zaproszenia zostanie wyświetlony domyślny profil bankowy. Zostanie również pokazany dowolny dostępny profil podatkowy, jeśli został utworzony dla tej lokalizacji MPN. Jeśli firma Microsoft ma wszystkie wymagane szczegóły profilu bankowego i podatkowego, zostanie wyświetlony monit o wybranie opcji **Prześlij** w celu ukończenia rejestracji. Zobacz [Konfigurowanie domyślnego profilu bankowego.](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile)

Możesz również wybrać profil bankowy inny niż domyślny profil bankowy. Jeśli firma Microsoft wymaga dodatkowych szczegółów dotyczących profilów płatności,  profilów podatkowych lub  waluty, zostanie wyświetlony monit Continue (Kontynuuj) i nastąpi przekierowanie do strony profilu płatności i podatku w celu podania brakujących szczegółów. 

Rejestracja jest uznawana za ukończoną tylko wtedy, gdy profil wypłaty i profil podatkowy, który pozyskasz dla rejestracji, są weryfikowane przez firmę Microsoft.

Niektóre programy zachęt nie mają kryteriów kwalifikowalności i są otwarte dla wszystkich partnerów. Administrator zachęt zobaczy zaproszenia dla tych programów na stronie przeglądu zachęt, pod warunkiem, że ma uprawnienia do odpowiedniego programu zachęt i programu MPN. Firma Microsoft nie wysyła wiadomości e-mail z zaproszeniami do tych programów.

Aby uzyskać więcej informacji na temat procesu rejestracji, pobierz przewodnik [po rejestracji zachęt](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (wymagane jest zalogowanie).

## <a name="expiration-and-renewal"></a>Wygaśnięcie i odnowienie

Rejestracja zachęt wygasa na koniec roku obrachunkowego. Jeśli jednak pozostaniesz kwalifikującym się partnerem z aktywną umową, firma Microsoft przekaże rejestrację zachęt do kolejnego roku obrachunkowego. Nie musisz podjąć żadnych działań, o ile informacje o wypłatach i podatku wymagane dla programu zachęt są kompletne zgodnie z regułami programu zachęt.

## <a name="next-steps"></a>Następne kroki

- [Ustalanie uprawnień do programu](incentives-determined-your-program-eligibility.md)
- [Tworzenie profilów wypłat i profilów podatkowych oraz zarządzanie nimi](incentives-create-and-manage-your-payout-and-tax-profiles.md)