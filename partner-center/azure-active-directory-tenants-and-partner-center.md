---
title: Połącz konto służbowe, aby uzyskać dostęp do Centrum partnerskiego
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utwórz konto służbowe łączące firmę z kontem Centrum partnerskiego. Dzięki temu pracownicy w firmie mogą uzyskiwać dostęp do Centrum partnerskiego.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: 2cc30c3681f0310f738ed937c15e0142b20cdc4c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529833"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Utwórz konto służbowe łączące firmę z kontem Centrum partnerskiego

**Dotyczy**

- Centrum partnerskie

**Odpowiednie role**

- Administrator globalny
- Administrator zarządzania użytkownikami

## <a name="why-you-need-a-work-account"></a>Dlaczego potrzebujesz konta służbowego

Firma Microsoft wymaga połączenia konta służbowego firmy z nowym kontem Centrum partnerskiego. Link umożliwia użytkownikom konta logowanie się do Centrum partnerskiego przy użyciu nazw użytkowników i haseł konta służbowego.

## <a name="the-work-account-email-address"></a>Adres e-mail konta służbowego

Twoje konto służbowe lub służbowe wiadomości e-mail to adres e-mail podany przez firmę. Adres e-mail konta służbowego jest zwykle w formacie `you@yourcompany.com` . Osobiste adresy e-mail, takie jak Hotmail, Gmail lub Yahoo, nie będą działać i nie mogą być używane w ramach konta Centrum partnerskiego.

Jeśli masz więcej niż jeden prawidłowy służbowy adres e-mail, użyj tego, który jest skojarzony z centralną siedzibą firmy, a nie z działem regionalnym, na przykład użyj adresu `contoso.com` e-mail, a nie `contoso.uk` adres.

> [!NOTE]  
> Przed podjęciem decyzji o użyciu istniejącego konta służbowego należy wziąć pod uwagę liczbę użytkowników, którzy będą musieli współpracować w centrum partnerskim. Jeśli masz użytkowników na koncie, które nie muszą współpracować w centrum partnerskim, rozważ utworzenie nowego konta tylko dla tych użytkowników, którzy będą musieli korzystać z Centrum partnerskiego.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nie masz pewności, czy Twoja firma ma już konto służbowe?

Jeśli nie masz pewności, czy firma ma konto służbowe, wykonaj następujące kroki, aby je sprawdzić. Jeśli masz aktywną subskrypcję do Microsoft Azure lub pakietu Office 365, masz już konto służbowe.

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com).

2. Wybierz Azure Active Directory z menu, a następnie wybierz pozycję nazwy domen.

3. Jeśli masz już konto służbowe, nazwa domeny zostanie wyświetlona.

Jeśli firma nie ma jeszcze konta służbowego, można ją utworzyć podczas procesu rejestracji.

Na poniższym diagramie przedstawiono kroki dla kilku typowych scenariuszy:

- Określanie, czy masz konto służbowe
- Określanie sposobu logowania się do konta służbowego
- Określanie, czy konieczne jest utworzenie nowego konta służbowego

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Czy masz konto służbowe lub musisz je utworzyć?":::

Aby uzyskać więcej informacji na temat dodawania domen w usłudze Azure AD, zobacz [Dodawanie lub kojarzenie domeny w usłudze Azure AD](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Informacje o Microsoft Azure

Microsoft Azure to platforma chmury publicznej, za pomocą której firmy mogą tworzyć i wdrażać aplikacje oraz zarządzać nimi w globalnej sieci zarządzanych przez firmę Microsoft centrów danych. Firmy używają platformy Azure do kompilowania wirtualnej infrastruktury IT za pomocą funkcji wirtualnych lub usług, a nie maszyn fizycznych.

Gdy kupisz subskrypcję platformy Azure, jesteś w istocie dzierżawionym dedykowanym, bezpiecznym miejscem w chmurze publicznej platformy Azure, ale nie różni się zbyt od wynajmu piętra w ramach budynku biurowego w celu zapewnienia fizycznej firmy. Dla właściciela budynku biurowego firma jest dzierżawcą.

Konto służbowe platformy Azure to dedykowana i izolowana wirtualna reprezentacja firmy w chmurze publicznej platformy Azure, która została utworzona w przypadku subskrybowania usługi w chmurze firmy Microsoft, takiej jak Azure, Microsoft Intune lub Office 365.

Twoje konto służbowe obsługuje użytkowników usługi Azure AD i informacje o nich — hasła, dane profilu, uprawnienia i tak dalej. Konto służbowe zawiera również grupy, aplikacje i inne informacje odnoszące się do firmy i jej zabezpieczeń.