---
title: Dostosowywanie wbudowanego środowiska urządzenia
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Przed dostarczeniem nowego urządzenia klienta można użyć profilów autopilotażu systemu Windows do dostosowania lub wstępnego skonfigurowania gotowego do użycia środowiska (OOBE) urządzenia.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534997"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Używanie profilów rozwiązania Windows Autopilot na nowych urządzeniach w celu dostosowania środowiska gotowego do użycia dla klienta

**Odpowiednie role**

- Agent administracyjny
- Administrator globalny
- Agent sprzedaży
- Administrator zarządzania użytkownikami

Jeśli zarządzasz urządzeniami klienta, może być konieczne dostosowanie środowiska OOBE (out-of-Box Experience) dla użytkowników klienta. Można wstępnie skonfigurować nowe urządzenia z profilami autopilotażu systemu Windows przed dostarczeniem urządzeń do klientów i zastosować nowe profile do urządzeń, które zostały już zakupione. 

Należy pamiętać, że producenci OEM, którzy uruchomili etykietę wysyłkową na zewnątrz pola urządzenie pilotażowe, pokazujący **Identyfikator klucza produktu (PKID)** urządzenia.  Ten 1-wymiarowy, czytelny kod kreskowy zapewnia partnerom podrzędnym możliwość rejestrowania urządzeń dla autopilotażu bez konieczności Unbox urządzeń i zbierania identyfikatorów urządzeń przy użyciu alternatywnych metod.

W tym artykule wyjaśniono, jak utworzyć i zastosować profile autopilotażu na urządzeniach w centrum partnerskim.

Jeśli nie znasz już programu pilotażowego, zapoznaj się z informacjami w poniższych artykułach:

- [Omówienie rozwiązania Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Przewodnik dotyczący wdrażania w programie autopilotaż](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Omówienie

Dzięki funkcji autopilotażu systemu Windows w centrum partnerskim można tworzyć niestandardowe profile, które mają zastosowanie do urządzeń klienckich. Następujące ustawienia profilu były dostępne po opublikowaniu tego artykułu:

- Pomiń ustawienia prywatności. To opcjonalne ustawienie profilu autopilotażu pozwala organizacjom nie żądać ustawień prywatności podczas procesu OOBE.

- Wyłącz tworzenie konta administratora lokalnego na urządzeniu. Organizacje mogą zdecydować, czy użytkownik konfigurujący urządzenie powinien mieć dostęp administratora po zakończeniu procesu.

- Automatycznie Skonfiguruj urządzenie pod kątem pracy lub szkoły. Wszystkie urządzenia zarejestrowane za pomocą autopilotażu będą automatycznie uznawane za urządzenia służbowe, więc nie będzie to konieczne w trakcie procesu OOBE.

- Pomiń strony konfiguracji Cortany, OneDrive i rejestracji OEM. Wszystkie urządzenia zarejestrowane za pomocą autopilotażu automatycznie pomijają te strony podczas procesu OOBE (out-of-Box Experience).

- Pomiń umowę licencyjną użytkownika oprogramowania (EULA). Począwszy od systemu Windows 10 w wersji 1709, organizacje mogą zdecydować o pominięciu strony umów EULA przedstawionych podczas procesu OOBE. Aby zapoznać się z ważnymi informacjami na temat pomijania strony umów EULA podczas instalacji systemu Windows, zobacz sekcję dotyczącą [umowy EULA systemu Windows](#windows-autopilot-eula-dismissal) .

Mają zastosowanie następujące uprawnienia i ograniczenia dotyczące zarządzania profilami i urządzeniami:

- Partnerzy programu CSP mogą nadal zarządzać profilami rozwiązania Autopilot dla istniejących klientów, z którymi mają relacje odsprzedawcy, nawet jeśli klienci usunęli uprawnienia administracji delegowanej dla partnerów.

- Możesz zarządzać istniejącymi urządzeniami dla dodanych przez Ciebie klientów.

- Nie możesz zarządzać urządzeniami przekazanymi przez Twojego klienta do sklepu Microsoft Store dla firm lub portalu usługi Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Tworzenie profilów autopilotażu i zarządzanie nimi w centrum partnerskim

W centrum partnerskim można utworzyć profile wdrażania systemu Windows i zastosować je do urządzeń.

>[!NOTE]
>Tylko agenci administracyjni mogą tworzyć i stosować profile.

### <a name="create-a-new-autopilot-profile"></a>Utwórz nowy profil autopilotażu

1. Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego tworzysz profil autopilotażu.

2. Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.

3. W obszarze **Profile autopilotaż systemu Windows** wybierz pozycję **Dodaj nowy profil**.

4. Wprowadź nazwę i opis profilu, a następnie skonfiguruj ustawienia OOBE. Wybierz spośród opcji:  

   - Pomiń ustawienia prywatności w instalatorze

   - Wyłącz konto administratora lokalnego w instalatorze
  
   - Automatycznie Pomijaj strony w instalatorze<br>
        (Obejmuje *Automatyczne wybieranie ustawień dotyczących pracy lub szkoły* oraz *pomijanie stron ustawień rejestracji Cortany, OneDrive i OEM*)
  
   - Pomiń umowę licencyjną użytkownika oprogramowania (EULA)<br> 
       >[!IMPORTANT] 
       >Aby zapoznać się z ważnymi informacjami na temat pomijania strony umów EULA podczas instalacji systemu Windows, zobacz sekcję dotyczącą [umowy EULA systemu Windows](#windows-autopilot-eula-dismissal) .

5. Po zakończeniu wybierz pozycję **Prześlij** .

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Stosowanie profilu autopilotażu do urządzeń klienckich

>[!NOTE]
>W poniższych instrukcjach przyjęto założenie, że urządzenia klienta zostały już dodane do Centrum partnerskiego i że można uzyskać dostęp do listy urządzeń. Jeśli urządzenia klienta nie zostały jeszcze dodane, postępuj zgodnie z instrukcjami w temacie [Dodawanie urządzeń do konta klienta](#add-devices-to-a-customers-account) , a następnie wykonaj poniższe kroki.

Po utworzeniu profilu programu pilotażowego dla klienta można go zastosować na urządzeniach klienta.

1. Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego został utworzony profil autopilotażu.

2. Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.

3. W obszarze **Zastosuj profile do urządzeń** wybierz urządzenia lub grupy urządzeń, do których chcesz dodać profile, a następnie wybierz pozycję **Zastosuj profil**. Właśnie stosowany profil zostanie wyświetlony w kolumnie **profil** .

4. Wykonaj poniższe kroki, aby sprawdzić, czy profil zostanie pomyślnie zastosowany do urządzenia.

    a.  Podłącz urządzenie do sieci i włącz je.

    b.  Sprawdź, czy są wyświetlane odpowiednie ekrany OOBE (jeśli istnieją).

    c.  Po zatrzymaniu procesu OOBE Zresetuj urządzenie do domyślnych ustawień fabrycznych, aby przygotować je do nowego użytkownika.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Usuwanie profilu autopilotażu z urządzenia klienta

1. Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, dla którego został utworzony profil autopilotażu.

2. Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.

3. W obszarze **Zastosuj profile do urządzeń** wybierz urządzenia, z których chcesz usunąć profil, a następnie wybierz pozycję **Usuń profil**.

   >[!NOTE]
   >Usunięcie profilu z urządzenia nie powoduje usunięcia go z listy. Jeśli chcesz usunąć profil, postępuj zgodnie z instrukcjami w temacie [Aktualizowanie lub usuwanie profilu autopilotażu](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualizowanie lub usuwanie profilu autopilotażu

Jeśli klient chce zmienić wbudowane środowisko po wysłaniu do nich urządzeń, można zmienić profil w centrum partnerskim.

Gdy urządzenie klienta nawiązuje połączenie z Internetem, pobiera najnowsze wersje profilu podczas procesu OOBE. Ponadto w przypadku gdy klient przywraca domyślne ustawienia fabryczne urządzenia, urządzenie powróci do najnowszej wersji profilu podczas procesu OOBE.

1. Wybierz pozycję **klienci** z menu Centrum partnerskiego, a następnie wybierz klienta, który chce zmienić profil autopilotażu.

2. Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.

3. W obszarze **Profile autopilotaż systemu Windows** wybierz profil, który ma zostać zaktualizowany. Wprowadź wymagane zmiany, a następnie wybierz pozycję **Prześlij**.

Aby usunąć ten profil, wybierz pozycję **Usuń profil** w prawym górnym rogu strony.

### <a name="add-devices-to-a-customers-account"></a>Dodawanie urządzeń do konta klienta

>[!NOTE]
>Agenci sprzedaży i agenci administracyjni mogą dodawać urządzenia do konta klienta.

Aby można było zastosować niestandardowe profile autopilotażu na urządzeniach klienckich, musisz mieć dostęp do listy urządzeń klienta.

Jeśli planujesz użycie nazwy producenta OEM, numeru seryjnego i kombinacji modelu, należy pamiętać o następujących ograniczeniach:

- Ta krotka działa tylko w przypadku nowszych urządzeń (na przykład skrótów 4K) i nie jest obsługiwana w przypadku skrótów 128B (RS2 i starszych urządzeń).

- Rejestracja spójnej kolekcji uwzględnia wielkość liter, dlatego dane w pliku muszą być zgodne z nazwą modelu i producenta **_dokładnie_* znakiem dostarczonym przez dostawcę OEM (dostawca sprzętu).

Postępuj zgodnie z poniższymi instrukcjami, aby dodać urządzenia do konta klienta w centrum partnerskim.

1. Wybierz _ *Customers** z menu Centrum partnerskiego, a następnie wybierz klienta, którego urządzenia chcesz zarządzać.

2. Na stronie Szczegóły klienta wybierz pozycję **urządzenia**.

3. W obszarze **Zastosuj profile do urządzeń** wybierz pozycję **Dodaj urządzenia**.

4. Wprowadź nazwę listy urządzeń, a następnie wybierz pozycję **Przeglądaj** , aby przekazać listę klientów (w formacie pliku CSV) do Centrum partnerskiego.

    >[!NOTE]
    >Plik CSV powinien zostać odebrany przy użyciu zakupu urządzenia. Jeśli plik CSV nie został odebrany, możesz go utworzyć, wykonując czynności opisane w temacie [Dodawanie urządzeń do systemu Windows autopilotaż](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Przekaż plik CSV, a następnie wybierz pozycję **Zapisz**.

Jeśli podczas próby przekazania pliku CSV zostanie wyświetlony komunikat o błędzie, sprawdź format pliku. Możesz użyć samego skrótu sprzętu lub nazwy producenta OEM, numeru seryjnego i modelu (w tej kolejności kolumn) lub identyfikatora produktu systemu Windows. Możesz również użyć pliku CSV z linkiem obok pozycji **Dodaj urządzenia** , aby utworzyć listę urządzeń.

Plik CSV powinien wyglądać następująco:

> **Numer seryjny urządzenia, identyfikator produktu systemu Windows, skrót sprzętu, nazwa producenta, model urządzenia**

> **{numer_seryjny},,, Microsoft Corporation, Surface laptop**

>[!NOTE]
> "Nazwa producenta" i "model urządzenia" są rozróżniana wielkość liter.

Jeśli nie wiesz, jakie wartości należy umieścić w polu Nazwa producenta i model urządzenia, możesz uruchomić to urządzenie, aby zebrać poprawne wartości:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Odrzucanie umowy EULA systemu Windows

### <a name="important-information"></a>WAŻNE INFORMACJE

Program Windows automatycznie pilotaż umożliwia skonfigurowanie dostosowanych instalacji systemu Windows na urządzeniach zarządzanych przez klientów. Jeśli klient zezwoli na to w tym celu, można pominąć lub ukryć niektóre ekrany skonfigurowane, które są zwykle prezentowane użytkownikom podczas konfigurowania systemu Windows, w tym na ekranie akceptacji umowy licencyjnej użytkownika oprogramowania.

Za pomocą tej funkcji, użytkownik wyraża zgodę na pominięcie lub ukrycie wszelkich ekranów, które zostały zaprojektowane w celu udostępnienia użytkownikom informacji lub akceptacji warunków oznacza, że uzyskano wystarczającą zgodę i autoryzację od klienta, aby ukryć warunki i w imieniu klienta (czy organizacja lub indywidualny użytkownik może mieć możliwość), wyrazić zgodę na wszelkie powiadomienia i zaakceptować warunki, które są odpowiednie dla klienta. Obejmuje to umowę dotyczącą warunków i postanowień licencyjnych lub informacji, które byłyby widoczne dla użytkownika, jeśli nie została pominięta lub ukryta przy użyciu tego narzędzia. Klient nie może używać oprogramowania systemu Windows na tych urządzeniach, jeśli klient nie uzyskał ważnej licencji na oprogramowanie firmy Microsoft lub jej licencjonowanych dystrybutorów.