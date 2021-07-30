---
title: Uzyskiwanie uprawnień administratora klienta
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Uzyskaj uprawnienia potrzebne do zarządzania usługą lub subskrypcją klienta w jego imieniu. Dowiedz się, w jaki sposób uprawnienia są udzielane, odwoływały się i zarządzane.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: fafd9e2c13abb1f4b9b12e5839662b27c4852452
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842103"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Uzyskiwanie uprawnień do zarządzania usługą lub subskrypcją klienta

**Odpowiednie role:** Administrator | Agent sprzedaży

Aby zarządzać usługą lub subskrypcją klienta w jego imieniu, klient musi przyznać Ci uprawnienia administratora do tej usługi. Aby uzyskać uprawnienia administratora od klienta, wyślij do klienta wiadomość e-mail z żądaniem relacji odsprzedawcy. Po zatwierdzeniu żądania przez klienta będzie można zalogować się do portalu administracyjnego usługi i zarządzać usługą w imieniu klienta. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Zapraszanie klienta do nawiązania relacji odsprzedawcy

1.  Wybierz **pozycję Customers (Klienci),** a następnie wybierz pozycję Request a reseller **relationship (Zażądaj relacji odsprzedawcy).**

2.  Na następnej stronie przejrzyj wersję roboczą wiadomości e-mail. Możesz otworzyć wersję roboczą wiadomości w domyślnej aplikacji poczty e-mail lub skopiować wiadomość do schowka i wkleić do wiadomości e-mail. 

    >[!IMPORTANT]
    >Tekst wiadomości można edytować, ale należy pamiętać o zachowaniu spersonalizowanego linku umożliwiającego bezpośrednie połączenie klienta z Twoim kontem. 
    
3.  Po **ukończeniu** tego kroku wybierz pozycję Gotowe.

4.  Wyślij wiadomość e-mail do klienta.

5.  Gdy klient zaakceptuje zaproszenie, pojawi się  na stronie Klienci, a ty będziesz w stanie aprowizować usługę dla klienta i zarządzać jej od tej strony.

6.  Aby zarządzać kontem, usługami, użytkownikami i licencjami klienta, rozwiń rekord klienta, wybierając strzałkę w dół obok jego nazwy, a następnie wybierz portal administracyjny dla usługi, którą chcesz zarządzać.

>[!IMPORTANT]  
>Klienci mogą ponownie przypisać lub usuwać uprawnienia administratora w portalu administracyjnym usługi. Należy jednak poinformować klienta, że usunięcie uprawnień administratora oznacza, że nie będzie już można otworzyć żądania obsługi do firmy Microsoft w jego imieniu. Nie będzie można otworzyć tego typu żądań obsługi w imieniu klienta do czasu ponownego negocjowania umowy z klientem.

Twoi klienci mogą dowiedzieć się, którzy partnerzy mają uprawnienia administratora do swojej dzierżawy, z poziomu Office 365 administracyjnego. W tym celu:

1. Klient musi zalogować się do portalu administracyjnego Office 365 jako administrator globalny.

2. Wybierz **pozycję Ustawienia** Relacje z  >  **partnerami.**

3. Na stronie **Relacje z** partnerami klient zobaczy listę partnerów, z którymi pracuje, oraz tych, którym przyznano uprawnienia administratora delegowane do dzierżawy.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Klienci mogą zarządzać delegowanymi uprawnieniami administratora partnera 

Klient może zdecydować się na usunięcie delegowanych uprawnień administratora ze swojej dzierżawy, ale zachować relację z Tobem na potrzeby odnawiania subskrypcji i licencji. Klienci zarządzają prawami i uprawnieniami do swoich kont Office 365 na stronie **Relacje** partnerów w centrum Office 365 administracyjnego. Na tej stronie klienci mogą:

- Zobacz, z którymi partnerami są oni w relacji i którzy partnerzy mają delegowane uprawnienia administratora

- Usuwanie delegowanych uprawnień administracyjnych partnera z dzierżawy

Aby usunąć delegowane uprawnienia administracyjne od partnera:

1. Na stronie **Relacje z** partnerami wybierz odpowiedniego partnera.
2. W okienku szczegółów wybierz pozycję **Usuń administratora delegowanego.**
3. W okienku potwierdzenia wybierz pozycję **Usuń**.

>[!IMPORTANT]  
>Przypisania ról usługi Azure AD do partnera są niejawne. Jeśli spróbujesz wyświetlić listę członków ról usługi Azure AD przy użyciu portalu usługi Azure AD/programu PowerShell/Graph, partner nie zostanie zwrócony. Aby dowiedzieć się, czy partnerzy są przypisani do ról usługi Azure AD, należy zapoznać się ze stroną Relacje partnerów w portalu usługi Office 365 Admin, aby dowiedzieć się, czy partnerowi przyznano delegowane uprawnienia administracyjne, czy nie.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegowane uprawnienia administratora w usłudze Azure AD 

W dzierżawie usługi Azure AD partnera istnieją dwie grupy zabezpieczeń: Agenci administracyjni i Agenci pomocy technicznej, które są używane do administracji delegowanej. Gdy klient przyznaje partnerowi delegowane uprawnienia administracyjne:

- Grupa Agent administratora jest przypisana do roli administratora globalnego w dzierżawie usługi Azure AD klienta.

- Grupa Agent pomocy technicznej jest przypisana do roli administrator pomocy technicznej w dzierżawie usługi Azure AD klienta.

Na podstawie przypisanych ról katalogu członkowie obu grup mogą logować się do dzierżawy usługi Azure AD klienta i usług O365 przy użyciu poświadczeń partnera i administratora w imieniu klienta.

Jeśli klient usunie delegowane uprawnienia administratora, przypisania ról usługi Azure AD zostaną usunięte i nie będzie można już zarządzać dzierżawą usługi Azure AD klienta.

### <a name="azure-subscriptions-and-resource-management"></a>Subskrypcje platformy Azure i zarządzanie zasobami

Każda subskrypcja platformy Azure ma własny zestaw ról zarządzania zasobami. Aby partner CSP może zarządzać subskrypcją platformy Azure klienta, należy przypisać partnera do co najmniej jednej roli w ramach subskrypcji platformy Azure. W szczególności:

- Gdy klient akceptuje zaproszenie odsprzedawcy i przyznaje partnerowi delegowane uprawnienia administracyjne, partner nie uzyskuje automatycznie dostępu do istniejących subskrypcji platformy Azure w ramach dzierżawy klienta.

- Gdy partner programu CSP apowiuje nową subskrypcję platformy Azure dla klienta, do grupy Agenci administracyjni w ramach dzierżawy partnera CSP jest automatycznie przypisywana rola właściciela w ramach subskrypcji. Na podstawie tego przypisania roli członkowie grupy mogą uzyskać dostęp do zasobów i zarządzać nimi w ramach subskrypcji.

- Gdy klient usunie delegowane uprawnienia administracyjne od partnera za pomocą portalu Office 365 Portal, partner może nadal zarządzać subskrypcją platformy Azure klienta, o ile partner jest nadal przypisany do co najmniej jednej roli w ramach subskrypcji. Aby zatrzymać partnera w zarządzaniu subskrypcją platformy Azure, klient musi usunąć przypisanie roli.

## <a name="windows-autopilot"></a>Windows Autopilot

Z Partner Center CSP partnerzy mogą zarządzać profilami rozwiązania Autopilot dla swoich klientów bez delegowanych uprawnień administratora w takich okolicznościach: 

- Jeśli klient usunie delegowane uprawnienia administracyjne, ale zachowa relację odsprzedawcy z Toem, możesz nadal zarządzać profilami rozwiązania Autopilot.

- Możesz zarządzać urządzeniami klientów dodanymi przez Ciebie lub innego partnera. 

- Nie można zarządzać urządzeniami dodanymi przez klienta za pośrednictwem witryny Microsoft Store dla Firm, Microsoft Store dla Instytucji Edukacyjnych lub Microsoft Intune Portal.

Aby uzyskać więcej informacji na temat rozwiązania Autopilot, zobacz Simplify device setup with Windows Autopilot (Upraszczanie konfiguracji [urządzenia za pomocą Windows Autopilot).](autopilot.md)

>[!IMPORTANT]  
>Bieżące środowisko zarządzania rozwiązaniem Autopilot w Partner Center może nadal ulec zmianie. W momencie opublikowania tego artykułu rozważane są następujące zmiany:

- Partner musi uzyskać delegowane uprawnienia administracyjne przez klienta, aby partner może dodawać/aktualizować/usuwać profile i stosować/usuwać profil z dowolnych urządzeń w dzierżawie klienta.

- Partner musi uzyskać delegowane uprawnienia administracyjne przez klienta, aby partner może usunąć urządzenia dodane przez innych partnerów lub przez klienta w dzierżawie klienta. W przeciwnym razie partner może usunąć tylko urządzenia dodane wcześniej przez tego samego partnera.
