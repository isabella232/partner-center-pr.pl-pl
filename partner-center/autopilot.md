---
title: Dostosowywanie out-of-box experience urządzenia
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Przed dostarczeniem nowego urządzenia klienta możesz użyć profilów rozwiązania Windows Autopilot, aby dostosować lub wstępnie skonfigurować środowisko out-of-box experience (OOBE) urządzenia.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 95a201c53fc2eaf230d08bb4cfdd03a5747b5c05
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838482"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Używanie profilów rozwiązania Windows Autopilot na nowych urządzeniach w celu dostosowania środowiska gotowego do użycia dla klienta

**Odpowiednie role:** Agent administracyjny | Administrator globalny | Agent sprzedaży | Administrator zarządzania użytkownikami

Jeśli zarządzasz urządzeniami klienta, może być konieczne dostosowanie out-of-box experience (OOBE) dla użytkowników klienta. Nowe urządzenia można wstępnie skonfigurować przy użyciu profilów rozwiązania Windows Autopilot przed dostarczeniem urządzeń do klientów i zastosować nowe profile do już zakupionych urządzeń. 

Należy pamiętać, że od producentów OEM rozpoczęto zawieranie etykiety wysyłkowej poza polem urządzenia rozwiązania Autopilot, które zawiera identyfikator klucza produktu **(PKID) urządzenia.**  Ten 1-wymiarowy, czytelny kod kreskowy umożliwia partnerom niższego szczebla rejestrowanie urządzeń w programie Autopilot bez konieczności rozpakowania urządzeń i zbierania identyfikatorów urządzeń w alternatywny sposób.

W tym artykule wyjaśniono, jak tworzyć i stosować profile rozwiązania Autopilot do urządzeń w Partner Center.

Jeśli nie znasz jeszcze rozwiązania Autopilot, zapoznaj się z informacjami w tych artykułach:

- [Omówienie rozwiązania Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Podręcznik wdrażania rozwiązania Autopilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Omówienie

Dzięki funkcji Windows Autopilot w Partner Center można tworzyć profile niestandardowe do zastosowania na urządzeniach klientów. W momencie opublikowania tego artykułu były dostępne następujące ustawienia profilu:

- Pomiń ustawienia prywatności. To opcjonalne ustawienie profilu rozwiązania Autopilot pozwala organizacjom nie pytać o ustawienia prywatności podczas procesu OOBE.

- Wyłącz tworzenie konta administratora lokalnego na urządzeniu. Organizacje mogą zdecydować, czy użytkownik konfiguracji urządzenia powinien mieć dostęp administratora po zakończeniu procesu.

- Automatycznie skonfiguruj urządzenie do pracy lub nauki. Wszystkie urządzenia zarejestrowane przy użyciu rozwiązania Autopilot będą automatycznie traktowane jako urządzenia służbowe, więc to pytanie nie zostanie zadane podczas procesu OOBE.

- Pomiń Cortana, OneDrive i rejestracji OEM. Wszystkie urządzenia zarejestrowane przy użyciu rozwiązania Autopilot będą automatycznie pomijać te strony podczas procesu OOBE (out-of-box experience).

- Pomiń umowę licencyjną użytkownika oprogramowania (EULA). Począwszy od Windows 10 wersji 1709, organizacje mogą zdecydować się pominąć stronę eula przedstawioną podczas procesu OOBE. Aby uzyskać Windows ominięcia strony eula rozwiązania Autopilot podczas instalacji, zobacz Windows rozwiązania [Autopilot.](#windows-autopilot-eula-dismissal)

Mają zastosowanie następujące uprawnienia i ograniczenia dotyczące zarządzania profilami i urządzeniami:

- Partnerzy programu CSP mogą nadal zarządzać profilami rozwiązania Autopilot dla istniejących klientów, z którymi mają relacje odsprzedawcy, nawet jeśli klienci usunęli uprawnienia administracji delegowanej dla partnerów.

- Możesz zarządzać istniejącymi urządzeniami dla dodanych przez Ciebie klientów.

- Nie możesz zarządzać urządzeniami przekazanymi przez Twojego klienta do sklepu Microsoft Store dla firm lub portalu usługi Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Tworzenie profilów rozwiązania Autopilot i zarządzanie nimi w Partner Center

W Partner Center można tworzyć profile wdrażania Windows rozwiązania Autopilot i stosować je do urządzeń.

>[!NOTE]
>Tylko agenci administracyjni mogą tworzyć i stosować profile.

### <a name="create-a-new-autopilot-profile"></a>Tworzenie nowego profilu rozwiązania Autopilot

1. Wybierz **pozycję** Klienci Partner Center menu, a następnie wybierz klienta, dla których tworzysz profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **Windows profile rozwiązania Autopilot wybierz** pozycję Dodaj nowy **profil.**

4. Wprowadź nazwę i opis profilu, a następnie skonfiguruj ustawienia OOBE. Wybierz spośród opcji:  

   - Pomijanie ustawień prywatności podczas instalacji

   - Wyłączanie konta administratora lokalnego w instalatorze
  
   - Automatyczne pomijanie stron w konfiguracji<br>
        (Obejmuje *opcje Automatycznie wybieraj konfigurację* dla konta służbowego i *Pomiń Cortana, OneDrive i Strony konfiguracji rejestracji OEM)*
  
   - Pomijanie umowy licencyjnej użytkownika oprogramowania (EULA)<br> 
       >[!IMPORTANT] 
       >Aby uzyskać Windows ominięcia strony eula rozwiązania Autopilot podczas instalacji, zobacz Windows rozwiązania [Autopilot.](#windows-autopilot-eula-dismissal)

5. Po **zakończeniu wybierz** pozycję Prześlij.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Stosowanie profilu rozwiązania Autopilot do urządzeń klientów

>[!NOTE]
>W poniższych instrukcjach przyjęto założenie, że urządzenia klienta zostały już dodane do aplikacji Partner Center i że możesz uzyskać dostęp do ich listy urządzeń. Jeśli urządzenia klienta nie zostały jeszcze dodane, postępuj zgodnie z instrukcjami w artykule Dodawanie urządzeń do konta klienta, [a](#add-devices-to-a-customers-account) następnie wykonaj poniższe kroki.

Po utworzeniu profilu rozwiązania Autopilot dla klienta można go zastosować do urządzeń klienta.

1. Wybierz **pozycję** Customers (Klienci) Partner Center menu aplikacji, a następnie wybierz klienta, dla których utworzono profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **obszarze Zastosuj profile do urządzeń** wybierz urządzenia lub grupy urządzeń, do których chcesz dodać profile, a następnie wybierz pozycję Zastosuj **profil.** Właśnie zastosowany profil zostanie wyświetlony w **kolumnie** Profil.

4. Wykonaj poniższe kroki, aby sprawdzić, czy profil zostanie pomyślnie zastosowany do urządzenia.

    a.  Połączenie urządzenie do sieci i włącz je.

    b.  Sprawdź, czy są wyświetlane odpowiednie ekrany OOBE (jeśli są).

    c.  Po zatrzymaniu procesu OOBE zresetuj urządzenie do domyślnych ustawień fabrycznych, aby przygotować je dla nowego użytkownika.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Usuwanie profilu rozwiązania Autopilot z urządzenia klienta

1. Wybierz **pozycję** Customers (Klienci) Partner Center menu aplikacji, a następnie wybierz klienta, dla których utworzono profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **obszarze Zastosuj profile do urządzeń** wybierz urządzenia, z których chcesz usunąć profil, a następnie wybierz pozycję Usuń **profil.**

   >[!NOTE]
   >Usunięcie profilu z urządzenia nie powoduje usunięcia profilu z listy. Jeśli chcesz usunąć profil, postępuj zgodnie z instrukcjami w sekcji [Aktualizowanie lub usuwanie profilu rozwiązania Autopilot.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualizowanie lub usuwanie profilu rozwiązania Autopilot

Jeśli klient chce zmienić środowisko out-of-box po wysłaniu do nich urządzeń, możesz zmienić profil w Partner Center.

Gdy urządzenie klienta połączy się z Internetem, podczas procesu OOBE zostanie pobrana najnowsza wersja profilu. Ponadto za każdym razem, gdy klient przywróci urządzenie do domyślnych ustawień fabrycznych, urządzenie ponownie pobierze najnowszą wersję profilu podczas procesu OOBE.

1. Wybierz **pozycję** Klienci Partner Center menu, a następnie wybierz klienta, który chce zmienić profil rozwiązania Autopilot.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **Windows profile rozwiązania Autopilot** wybierz profil, który chcesz zaktualizować. Określ wymagane zmiany, a następnie wybierz pozycję **Prześlij.**

Aby usunąć ten profil, wybierz **pozycję Usuń profil** w prawym górnym rogu strony.

### <a name="add-devices-to-a-customers-account"></a>Dodawanie urządzeń do konta klienta

>[!NOTE]
>Agenci sprzedaży i agenci administracyjni mogą dodawać urządzenia do konta klienta.

Aby można było zastosować niestandardowe profile rozwiązania Autopilot do urządzeń klientów, musisz mieć dostęp do listy urządzeń klienta.

Jeśli planujesz używać nazwy OEM, numeru seryjnego i kombinacji modelu, należy pamiętać o tych ograniczeniach:

- Ta krotka działa tylko w przypadku urządzeń nowszej (np. skrótów 4k) i nie jest obsługiwana w przypadku skrótów 128b (RS2 i poprzednich urządzeń).

- W rejestracji krotki jest zróżnicowa wielkość liter, dlatego  dane w pliku muszą być zgodne z nazwami modelu i producenta dokładnie tak, jak podano w przypadku dostawcy OEM (dostawcy sprzętu).

Postępuj zgodnie z poniższymi instrukcjami, aby dodać urządzenia do konta klienta w Partner Center.

1. Wybierz **pozycję** Klienci z Partner Center, a następnie wybierz klienta, którego urządzeniami chcesz zarządzać.

2. Na stronie szczegółów klienta wybierz pozycję **Urządzenia.**

3. W **obszarze Zastosuj profile do urządzeń wybierz** pozycję Dodaj **urządzenia.**

4. Wprowadź nazwę listy urządzeń, a  następnie wybierz pozycję Przeglądaj, aby przekazać listę klientów (w formacie .csv) do Partner Center.

    >[!NOTE]
    >Ten plik powinien zostać .csv z zakupem urządzenia. Jeśli nie otrzymasz pliku .csv, możesz utworzyć go samodzielnie, korzystając z procedury opisanej w tece Dodawanie urządzeń do rozwiązania [Windows Autopilot.](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)  

5. Upload plik .csv a następnie wybierz pozycję **Zapisz.**

Jeśli podczas próby przekazania pliku CSV zostanie wyświetlony komunikat o błędzie, sprawdź format pliku. Możesz użyć samego skrótu sprzętu lub nazwy producenta OEM, numeru seryjnego i modelu (w tej kolejności kolumn) lub identyfikatora produktu systemu Windows. Możesz również użyć przykładowego pliku .csv linku obok przycisku **Dodaj urządzenia,** aby utworzyć listę urządzeń.

Plik .csv powinien wyglądać podobnie do tego:

> **Numer seryjny urządzenia,Windows identyfikator produktu,skrót sprzętu,nazwa producenta,model urządzenia**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> W polach "Nazwa producenta" i "Model urządzenia" jest wielkość liter.

Jeśli nie wiesz, jaką wartość należy umieścić w polach Nazwa producenta i Model urządzenia, możesz uruchomić to na urządzeniu, aby zebrać poprawne wartości:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Odrzucanie z programu Autopilot (eula)

### <a name="important-information"></a>WAŻNE INFORMACJE

Windows Funkcja Autopilot umożliwia skonfigurowanie dostosowanych instalacji Windows na urządzeniach, które zarządzasz dla klientów. Jeśli klient ma takie uprawnienia, można pominąć lub ukryć niektóre ekrany konfiguracji, które są zwykle prezentowane użytkownikom podczas konfigurowania aplikacji Windows, w tym ekran akceptacji umowy licencyjnej użytkownika oprogramowania (EULA).

Korzystając z tej funkcji, zgadzasz się, że pomijanie lub ukrywanie ekranów, które mają na celu powiadomienie lub zaakceptowanie warunków przez użytkowników, oznacza, że użytkownik uzyskał wystarczającą zgodę i autoryzację od klienta, aby ukryć warunki, oraz że w imieniu klienta (w zależności od tego, czy jest to organizacja, czy indywidualny użytkownik) , wyrażać zgodę na wszelkie powiadomienia i akceptować wszelkie postanowienia, które mają zastosowanie do klienta. Obejmuje to umowę z warunkami i postanowieniami licencji lub powiadomienie, które zostaną przedstawione użytkownikowi, jeśli użytkownik nie pominął ani nie ukrywał jej za pomocą tego narzędzia. Klient nie może korzystać z oprogramowania Windows tych urządzeniach, jeśli klient nie uzyskał w prawidłowy sposób licencji na oprogramowanie od firmy Microsoft lub licencjonowanych dystrybutorów.