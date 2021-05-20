---
title: Dostosowywanie out-of-box experience urządzenia
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Przed dostarczeniem nowego urządzenia klienta można użyć profilów usługi Windows Autopilot w celu dostosowania lub wstępnego skonfigurowania out-of-box experience (OOBE) urządzenia.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149829"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Używanie profilów rozwiązania Windows Autopilot na nowych urządzeniach w celu dostosowania środowiska gotowego do użycia dla klienta

**Odpowiednie role:** Administrator | Administrator globalny | Agent sprzedaży | Administrator zarządzania użytkownikami

Jeśli zarządzasz urządzeniami klienta, może być konieczne dostosowanie out-of-box experience (OOBE) dla użytkowników klienta. Nowe urządzenia można wstępnie skonfigurować przy użyciu profilów Windows Autopilot przed dostarczeniem urządzeń do klientów i zastosować nowe profile do już zakupionych urządzeń. 

Należy pamiętać, że od producentów OEM rozpoczęto zawieranie etykiety wysyłkowej poza polem urządzenia rozwiązania Autopilot, które zawiera identyfikator klucza produktu **(PKID) urządzenia.**  Ten 1-wymiarowy, czytelny kod kreskowy zapewnia partnerom niższego szczebla możliwość rejestrowania urządzeń w programie Autopilot bez konieczności rozpakowania urządzeń i zbierania identyfikatorów urządzeń w alternatywny sposób.

W tym artykule wyjaśniono, jak tworzyć i stosować profile rozwiązania Autopilot do urządzeń w Partner Center.

Jeśli nie znasz jeszcze rozwiązania Autopilot, zapoznaj się z informacjami w tych artykułach:

- [Omówienie rozwiązania Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Podręcznik wdrażania rozwiązania Autopilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Omówienie

Dzięki funkcji Windows Autopilot na Partner Center można tworzyć profile niestandardowe do zastosowania na urządzeniach klientów. W momencie opublikowania tego artykułu były dostępne następujące ustawienia profilu:

- Pomiń ustawienia prywatności. To opcjonalne ustawienie profilu rozwiązania Autopilot pozwala organizacjom nie pytać o ustawienia prywatności podczas procesu OOBE.

- Wyłącz tworzenie konta administratora lokalnego na urządzeniu. Organizacje mogą zdecydować, czy po zakończeniu procesu użytkownik konfiguracji urządzenia powinien mieć dostęp administratora.

- Automatycznie skonfiguruj urządzenie do pracy lub nauki. Wszystkie urządzenia zarejestrowane przy użyciu rozwiązania Autopilot zostaną automatycznie uznane za urządzenia służbowe, więc to pytanie nie zostanie zadane podczas procesu OOBE.

- Pomiń strony konfiguracji cortany, usługi OneDrive i rejestracji OEM. Wszystkie urządzenia zarejestrowane przy użyciu rozwiązania Autopilot będą automatycznie pomijać te strony podczas procesu OOBE (out-of-box experience).

- Pomiń umowę licencyjną użytkownika oprogramowania (EULA). Począwszy od Windows 10 wersji 1709, organizacje mogą zdecydować się pominąć stronę eula przedstawioną podczas procesu OOBE. Zobacz [Windows Autopilot poniżej,](#windows-autopilot-eula-dismissal) aby uzyskać ważne informacje dotyczące pomijania strony eula podczas instalacji systemu Windows.

Mają zastosowanie następujące uprawnienia i ograniczenia dotyczące zarządzania profilami i urządzeniami:

- Partnerzy programu CSP mogą nadal zarządzać profilami rozwiązania Autopilot dla istniejących klientów, z którymi mają relacje odsprzedawcy, nawet jeśli klienci usunęli uprawnienia administracji delegowanej dla partnerów.

- Możesz zarządzać istniejącymi urządzeniami dla dodanych przez Ciebie klientów.

- Nie możesz zarządzać urządzeniami przekazanymi przez Twojego klienta do sklepu Microsoft Store dla firm lub portalu usługi Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Tworzenie profilów rozwiązania Autopilot i zarządzanie nimi w Partner Center

W Partner Center można tworzyć Windows Autopilot wdrażania i stosować je do urządzeń.

>[!NOTE]
>Tylko agenci administracyjni mogą tworzyć i stosować profile.

### <a name="create-a-new-autopilot-profile"></a>Tworzenie nowego profilu rozwiązania Autopilot

1. Wybierz **pozycję** Klienci Partner Center menu, a następnie wybierz klienta, dla których tworzysz profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia**.

3. W **Windows Autopilot profilów wybierz** pozycję Dodaj nowy **profil.**

4. Wprowadź nazwę i opis profilu, a następnie skonfiguruj ustawienia OOBE. Wybierz spośród opcji:  

   - Pomijanie ustawień prywatności w konfiguracji

   - Wyłączanie konta administratora lokalnego w instalatorze
  
   - Automatyczne pomijanie stron w konfiguracji<br>
        (Obejmuje *automatyczne wybieranie ustawień dla służbowych* i *pomijanie cortany, usługi OneDrive* i stron konfiguracji rejestracji OEM)
  
   - Pomiń umowę licencyjną użytkownika końcowego (EULA)<br> 
       >[!IMPORTANT] 
       >Zobacz [Windows Autopilot poniżej,](#windows-autopilot-eula-dismissal) aby uzyskać ważne informacje dotyczące pomijania strony eula podczas instalacji systemu Windows.

5. Po **zakończeniu wybierz** pozycję Prześlij.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Stosowanie profilu rozwiązania Autopilot do urządzeń klientów

>[!NOTE]
>W poniższych instrukcjach przyjęto założenie, że urządzenia klienta zostały już dodane do Partner Center i że możesz uzyskać dostęp do jego listy urządzeń. Jeśli urządzenia klienta nie zostały jeszcze dodane, postępuj zgodnie z instrukcjami w artykule Dodawanie urządzeń do konta klienta, [a](#add-devices-to-a-customers-account) następnie wykonaj poniższe kroki.

Po utworzeniu profilu rozwiązania Autopilot dla klienta można go zastosować do urządzeń klienta.

1. Wybierz **pozycję** Customers (Klienci) Partner Center menu aplikacji, a następnie wybierz klienta, dla których utworzono profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia**.

3. W **obszarze Zastosuj profile do urządzeń** wybierz urządzenia lub grupy urządzeń, do których chcesz dodać profile, a następnie wybierz pozycję Zastosuj **profil.** Właśnie zastosowany profil zostanie wyświetlony w **kolumnie** Profil.

4. Wykonaj poniższe kroki, aby sprawdzić, czy profil zostanie pomyślnie zastosowany do urządzenia.

    a.  Podłącz urządzenie do sieci i włącz je.

    b.  Sprawdź, czy są wyświetlane odpowiednie ekrany OOBE (jeśli występują).

    c.  Po zatrzymaniu procesu OOBE przywróć domyślne ustawienia fabryczne urządzenia, aby przygotować je dla nowego użytkownika.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Usuwanie profilu rozwiązania Autopilot z urządzenia klienta

1. Wybierz **pozycję** Customers (Klienci) Partner Center menu aplikacji, a następnie wybierz klienta, dla których utworzono profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia**.

3. W **obszarze Zastosuj profile do urządzeń** wybierz urządzenia, z których chcesz usunąć profil, a następnie wybierz pozycję Usuń **profil.**

   >[!NOTE]
   >Usunięcie profilu z urządzenia nie powoduje usunięcia profilu z listy. Jeśli chcesz usunąć profil, postępuj zgodnie z instrukcjami w sekcji [Aktualizowanie lub usuwanie profilu rozwiązania Autopilot.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualizowanie lub usuwanie profilu rozwiązania Autopilot

Jeśli klient chce zmienić środowisko out-of-box po wysłaniu do nich urządzeń, możesz zmienić profil w Partner Center.

Gdy urządzenie klienta połączy się z Internetem, pobierze najnowszą wersję profilu podczas procesu OOBE. Ponadto za każdym razem, gdy klient przywróci urządzenie do domyślnych ustawień fabrycznych, urządzenie ponownie pobierze najnowszą wersję profilu podczas procesu OOBE.

1. Wybierz **pozycję** Klienci z Partner Center, a następnie wybierz klienta, który chce, aby zmienić profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **Windows Autopilot profilów** wybierz profil, który chcesz zaktualizować. Określ wymagane zmiany, a następnie wybierz pozycję **Prześlij.**

Aby usunąć ten profil, wybierz **pozycję Usuń profil** w prawym górnym rogu strony.

### <a name="add-devices-to-a-customers-account"></a>Dodawanie urządzeń do konta klienta

>[!NOTE]
>Agenci sprzedaży i agenci administracyjni mogą dodawać urządzenia do konta klienta.

Aby można było zastosować niestandardowe profile rozwiązania Autopilot do urządzeń klientów, musisz mieć dostęp do listy urządzeń klienta.

Jeśli planujesz używać nazwy OEM, numeru seryjnego i kombinacji modelu, należy pamiętać o tych ograniczeniach:

- Ta krotka działa tylko w przypadku urządzeń nowszej (na przykład 4k skrótów) i nie jest obsługiwana w przypadku skrótów 128b (RS2 i poprzednich urządzeń).

- W rejestracji krotki jest wielkość liter, dlatego dane w pliku  muszą być zgodne z nazwami modelu i producenta dokładnie tak, jak podano w przypadku dostawcy OEM (dostawcy sprzętu).

Postępuj zgodnie z poniższymi instrukcjami, aby dodać urządzenia do konta klienta w Partner Center.

1. Wybierz **pozycję** Klienci z Partner Center, a następnie wybierz klienta, którego urządzeniami chcesz zarządzać.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **obszarze Zastosuj profile do urządzeń wybierz** pozycję Dodaj **urządzenia.**

4. Wprowadź nazwę listy urządzeń, a  następnie wybierz pozycję Przeglądaj, aby przekazać listę klientów (w formacie pliku CSV) do Partner Center.

    >[!NOTE]
    >Ten plik CSV powinien zostać odebrany wraz z zakupem urządzenia. Jeśli nie otrzymasz pliku CSV, możesz go utworzyć samodzielnie, korzystając z procedury opisanej w temacie [Dodawanie](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)urządzeń do Windows Autopilot .  

5. Przekaż plik CSV, a następnie wybierz pozycję **Zapisz.**

Jeśli podczas próby przekazania pliku CSV zostanie wyświetlony komunikat o błędzie, sprawdź format pliku. Możesz użyć samego skrótu sprzętu lub nazwy producenta OEM, numeru seryjnego i modelu (w tej kolejności kolumn) lub identyfikatora produktu systemu Windows. Możesz również użyć przykładowego pliku CSV dostarczonego za pomocą linku obok **przycisku Dodaj urządzenia,** aby utworzyć listę urządzeń.

Plik CSV powinien wyglądać podobnie do tego:

> **Numer seryjny urządzenia,Identyfikator produktu systemu Windows,Skrót sprzętu,Nazwa producenta,Model urządzenia**

> **{serialNumber},,,Microsoft Corporation, Surface Laptop**

>[!NOTE]
> W polach "Nazwa producenta" i "Model urządzenia" jest wielkość liter.

Jeśli nie wiesz, jaką wartość należy umieścić dla pól Nazwa producenta i Model urządzenia, możesz uruchomić tę wartość na urządzeniu, aby zebrać poprawne wartości:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot odrzuć eula

### <a name="important-information"></a>WAŻNE INFORMACJE

Windows Autopilot umożliwia skonfigurowanie dostosowanych instalacji systemu Windows na urządzeniach, które są zarządzane dla klientów. W przypadku autoryzacji klienta można pominąć lub ukryć niektóre ekrany konfiguracji, które są zwykle prezentowane użytkownikom podczas konfigurowania systemu Windows, w tym ekran akceptacji umowy licencyjnej użytkownika oprogramowania (EULA).

Korzystając z tej funkcji, użytkownik zgadza się, że pomijanie lub ukrywanie ekranów, które mają na celu powiadomienie lub akceptację warunków, oznacza, że klient uzyskał wystarczającą zgodę i autoryzację, aby ukryć warunki, oraz że w imieniu klienta (w zależności od przypadku organizacji lub użytkownika indywidualnego) wyraża zgodę na wszelkie powiadomienia i akceptuje wszelkie postanowienia dotyczące klienta. Obejmuje to umowę z warunkami i postanowieniami licencji lub powiadomienie, które zostaną przedstawione użytkownikowi, jeśli użytkownik nie pominął ani nie ukrywał jej za pomocą tego narzędzia. Klient nie może korzystać z oprogramowania systemu Windows na tych urządzeniach, jeśli klient nie uzyskał w prawidłowy sposób licencji na oprogramowanie od firmy Microsoft lub licencjonowanych dystrybutorów.