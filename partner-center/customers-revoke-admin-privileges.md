---
title: Uzyskaj uprawnienia administratora klienta
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uzyskaj uprawnienia wymagane do zarządzania usługą lub subskrypcją klienta w ich imieniu. Dowiedz się, w jaki sposób uprawnienia są udzielane, odwoływane i zarządzane.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 6f99c9ed9fb43136bccf0d3024377ba2208ed1a1
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534883"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Uzyskaj uprawnienia do zarządzania usługą lub subskrypcją klienta

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Agent administracyjny
- Agent sprzedaży

Aby zarządzać usługą lub subskrypcją klienta w ich imieniu, klient musi przyznać uprawnienia administratora dla tej usługi. Aby uzyskać uprawnienia administratora od klienta, Wyślij do nich wiadomość e-mail z żądaniem relacji odsprzedawcy. Po zatwierdzeniu żądania przez klienta będzie można zalogować się do portalu administratora usługi i zarządzać usługą w imieniu klienta. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Zaproś klienta o nawiązanie z nim relacji odsprzedawcy

1.  Wybierz pozycję **klienci** , a następnie wybierz pozycję **Żądaj relacji odsprzedawcy**.

2.  Na następnej stronie przejrzyj wersję roboczą wiadomości e-mail. Możesz otworzyć wersję roboczą wiadomości w domyślnej aplikacji poczty e-mail lub skopiować wiadomość do schowka i wkleić do wiadomości e-mail. 

    >[!IMPORTANT]
    >Tekst wiadomości można edytować, ale należy pamiętać o zachowaniu spersonalizowanego linku umożliwiającego bezpośrednie połączenie klienta z Twoim kontem. 
    
3.  Po ukończeniu tego kroku wybierz pozycję **gotowe** .

4.  Wyślij wiadomość e-mail do klienta.

5.  Po zaakceptowaniu zaproszenia klient zostanie wyświetlony na stronie **klientów** i będzie można z niego udostępnić usługę i zarządzać nią.

6.  Aby zarządzać kontem klienta, usługami, użytkownikami i licencjami, rozwiń rekord klienta, wybierając strzałkę w dół obok swojej nazwy, a następnie wybierając Portal administratora dla usługi, którą chcesz zarządzać.

>[!IMPORTANT]  
>Klienci mogą ponownie przypisywać lub usuwać uprawnienia administratora w portalu administracyjnym usługi. Należy jednak poinformować klienta, że usunięcie uprawnień administratora oznacza, że nie będzie już można otworzyć żądania obsługi do firmy Microsoft w ich imieniu. Nie będzie można otwierać tych typów żądań obsługi w imieniu klienta do momentu ponownego negocjowania umowy z klientem.

Klienci mogą dowiedzieć się, którzy z partnerów mają uprawnienia administratora do swojej dzierżawy, z poziomu portalu administracyjnego pakietu Office 365. W tym celu:

1. Klient musi zalogować się do portalu administracyjnego pakietu Office 365 jako Administrator globalny.

2. Wybierz pozycję **Ustawienia**  >  **relacje partnera**.

3. Na stronie **relacje partnera** klient zobaczy listę partnerów, z którymi pracują, oraz tych, którym przyznano uprawnienia administracji delegowanej do swojej dzierżawy.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Klienci mogą zarządzać uprawnieniami administratora delegowanego przez partnera 

Klient może zdecydować o usunięciu z dzierżawy uprawnień administratora delegowanego, ale zachować tę relację w celu odnowienia subskrypcji i licencji. Klienci zarządzają prawami i uprawnieniami do kont Office 365 na stronie **relacje partnerów** w centrum administracyjnym pakietu Office 365. Na tej stronie klienci mogą:

- Sprawdź, z których partnerów mają relację i które partnerzy mają uprawnienia administratora delegowanego

- Usuwanie z dzierżawy uprawnień do administracji delegowanej przez partnera

Aby usunąć uprawnienia administracji delegowanej z partnera:

1. Na stronie **relacje partnera** wybierz partnera zainteresowania.
2. W okienku szczegółów wybierz pozycję **Usuń administratora delegowanego**.
3. W okienku potwierdzenia wybierz pozycję **Usuń**.

>[!IMPORTANT]  
>Przypisania ról usługi Azure AD do partnera są niejawne. Jeśli spróbujesz wyświetlić listę członków ról usługi Azure AD przy użyciu portalu usługi Azure AD/programu PowerShell/Graf, partner nie zostanie zwrócony. Aby dowiedzieć się, czy partnerzy są przypisani do ról usługi Azure AD, należy odwołać się do strony relacje partnerów w portalu administracyjnym pakietu Office 365, aby dowiedzieć się, czy uprawnienie administracji delegowanej zostało przyznane partnerowi.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Uprawnienia administratora delegowanego w usłudze Azure AD 

Istnieją dwie grupy zabezpieczeń, agenci administracyjni i agenci pomocy technicznej w dzierżawie usługi Azure AD partnera, które są używane do administracji delegowanej. Gdy klient przyznaje delegowane uprawnienia administracyjne do partnera:

- Grupa agentów administracyjnych jest przypisana do roli administratora globalnego w dzierżawie usługi Azure AD klienta.

- Grupa agentów pomocy technicznej jest przypisana do roli administratora pomocy technicznej w dzierżawie usługi Azure AD klienta.

W oparciu o przypisane role katalogu członkowie obu grup mogą zalogować się do dzierżawy usługi Azure AD klienta i usług O365 przy użyciu poświadczeń partnera i administratora w imieniu klienta.

Jeśli klient usunie uprawnienia administratora delegowanego, przypisania ról usługi Azure AD zostaną usunięte i nie będzie już można zarządzać dzierżawą usługi Azure AD klienta.

### <a name="azure-subscriptions-and-resource-management"></a>Subskrypcje i zarządzanie zasobami platformy Azure

Każda subskrypcja platformy Azure ma swój własny zestaw ról zarządzania zasobami. Aby partner programu CSP mógł zarządzać subskrypcją platformy Azure klienta, partner musi być przypisany do co najmniej jednej roli w ramach subskrypcji platformy Azure. W szczególności:

- Gdy klient zaakceptuje zaproszenie odsprzedawcy i przyzna delegowane uprawnienia administracyjne partnerowi, partner nie uzyskuje dostępu do istniejących subskrypcji platformy Azure w ramach dzierżawy klienta.

- Gdy Partner CSP Inicjuje nową subskrypcję platformy Azure dla klienta, Grupa agenci administracyjni w ramach dzierżawcy partnera CSP automatycznie przypisze rolę właściciela w ramach subskrypcji. Na podstawie tego przypisania roli członkowie grupy mogą uzyskiwać dostęp do zasobów w ramach subskrypcji i zarządzać nimi.

- Po usunięciu przez klienta uprawnień delegowanych z partnera przy użyciu portalu pakietu Office 365 partner nadal może zarządzać subskrypcją platformy Azure klienta, o ile partner nadal jest przypisany do co najmniej jednej roli w ramach subskrypcji. Aby uniemożliwić partnerowi Zarządzanie subskrypcją platformy Azure, klient musi usunąć przypisanie roli.

## <a name="windows-autopilot"></a>Windows Autopilot

W centrum partnerskim partnerzy CSP mogą zarządzać profilami autopilotażu dla swoich klientów bez uprawnień administratora delegowanego w następujących okolicznościach: 

- Jeśli klient usunie uprawnienia administratora delegowanego, ale zachowuje związek z odsprzedawcą, można nadal zarządzać profilami autopilotażu.

- Można zarządzać urządzeniami klienta, które zostały dodane przez Ciebie lub innego partnera. 

- Nie możesz zarządzać urządzeniami, które zostały dodane przez klienta za pomocą Microsoft Store dla firm, Microsoft Store do edukacji lub portalu Microsoft Intune.

Aby uzyskać więcej informacji na temat autopilotażu, zobacz [uproszczenie konfiguracji urządzenia za pomocą autopilotażu systemu Windows](autopilot.md).

>[!IMPORTANT]  
>Bieżące środowisko zarządzania autopilotażem w centrum partnerskim może nadal ulec zmianie. Po opublikowaniu tego artykułu są brane pod uwagę następujące zmiany:

- Aby partner mógł dodać/zaktualizować/usunąć profile i zastosować/wyeliminować profil z dowolnych urządzeń w dzierżawie klienta, musi mieć przyznane uprawnienia administracyjne delegowane przez klienta.

- Przed usunięciem przez partnera urządzeń dodanych przez partnerów lub klienta w dzierżawie klienta należy przyznać partnerowi uprawnienia administratora delegowanego. W przeciwnym razie partner może usunąć tylko te urządzenia, które zostały dodane wcześniej przez tego samego partnera.
