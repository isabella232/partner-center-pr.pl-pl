---
title: Łączenie konta służbowego w celu uzyskania dostępu do Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Utwórz konto służbowe, które łączy Twoją firmę z twoim Partner Center kontem. Dzięki temu pracownicy w firmie mogą uzyskać dostęp do Partner Center.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 6/17/2021
ms.openlocfilehash: c1f74e2977b110befd38c741259e84dd8bc9acb6
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115100055"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Tworzenie konta służbowego, które łączy twoją firmę z kontem Partner Center konta

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami

## <a name="why-you-need-a-work-account"></a>Dlaczego potrzebujesz konta służbowego

Firma Microsoft wymaga połączenia firmowego konta z nowym kontem Partner Center konta. Ten link umożliwia użytkownikom konta logowanie się w Partner Center przy użyciu nazw użytkowników i haseł kont służbowych.

## <a name="the-work-account-email-address"></a>Adres e-mail konta służbowego

Konto służbowe lub służbowy adres e-mail to adres e-mail dostarczony przez twoją firmę. Adres e-mail konta służbowego ma zazwyczaj format `you@yourcompany.com` . Osobiste adresy e-mail, takie jak Hotmail, Gmail lub Yahoo, nie są służbowym adresem e-mail i nie mogą być używane Partner Center konta.

Jeśli masz więcej niż jeden prawidłowy służbowy adres e-mail, użyj tego, który jest skojarzony z siedzibą firmy, a nie z działem regionalnym, na przykład użyj adresu e-mail, a nie `contoso.com` `contoso.uk` adresu.

> [!NOTE]  
> Przed użyciem istniejącego konta służbowego zastanów się, ilu użytkowników na koncie służbowym będzie musiało uzyskać dostęp do Partner Center. Jeśli masz użytkowników na koncie służbowym, którzy nie będą potrzebować dostępu do Partner Center, rozważ utworzenie nowego konta tylko dla tych użytkowników, którzy będą Partner Center dostępu.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nie masz pewności, czy Firma ma już konto służbowe?

Jeśli nie masz pewności, czy firma ma konto służbowe, wykonaj następujące kroki, aby to sprawdzić. Jeśli masz aktywną subskrypcję usługi Microsoft Azure lub Office 365, masz już konto służbowe.

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com).

2. Wybierz Azure Active Directory z menu nawigacji, a następnie wybierz pozycję **Custom Domain Nazwy.**

3. Jeśli masz już konto służbowe, nazwa domeny zostanie wymieniona.

Jeśli firma nie ma jeszcze konta służbowego, możesz je utworzyć podczas procesu rejestracji.

Na poniższym diagramie przedstawiono kilka typowych scenariuszy:

- określanie, czy masz konto służbowe
- określanie sposobu logowania się do konta służbowego
- określanie, czy musisz utworzyć nowe konto służbowe

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Czy masz konto służbowe, czy musisz je utworzyć?":::

Aby uzyskać więcej informacji na temat dodawania domen w usłudze Azure AD, zobacz [Dodawanie lub kojarzenie domeny w usłudze Azure AD](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Informacje o Microsoft Azure

Microsoft Azure to platforma chmury publicznej, której firmy mogą używać do tworzenia i wdrażania aplikacji oraz zarządzania nimi w globalnej sieci centrów danych zarządzanych przez firmę Microsoft. Firmy używają platformy Azure do tworzenia wirtualnej infrastruktury IT z funkcjami wirtualnymi lub usługami zamiast maszyn fizycznych.

Po zakupie subskrypcji platformy Azure zasadniczo wynajmujesz dedykowane, bezpieczne miejsce w chmurze publicznej Azure, nie różni się zbytnie od wynajmowania podłogi w budynku biurowym w celu przechowywania fizycznej firmy. Właściciel budynku biurowego jest dzierżawcą.

Konto służbowe platformy Azure to dedykowana i odizolowana wirtualna reprezentacja firmy w chmurze publicznej Platformy Azure, utworzona automatycznie podczas subskrybowania usługi w chmurze firmy Microsoft, takiej jak Azure, Microsoft Intune lub Office 365.

Konto służbowe hostuje użytkowników usługi Azure AD oraz informacje o nich — ich hasła, dane profilu, uprawnienia i tak dalej. Konto służbowe zawiera również grupy, aplikacje i inne informacje dotyczące firmy i jej zabezpieczeń.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
- [Śledzenie stanu weryfikacji](verification-responses.md)
