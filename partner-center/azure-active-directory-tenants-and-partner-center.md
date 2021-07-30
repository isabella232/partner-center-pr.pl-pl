---
title: Łączenie konta służbowego w celu uzyskania dostępu do Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Utwórz konto służbowe, które łączy Twoją firmę z Partner Center kontem. Dzięki temu pracownicy w firmie mogą uzyskać dostęp do Partner Center.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 6/17/2021
ms.openlocfilehash: 04624db5201b3a0e57b74b43678f6f2cd134c5c9
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841695"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Tworzenie konta służbowego, które łączy twoją firmę z kontem Partner Center konto

**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami

## <a name="why-you-need-a-work-account"></a>Dlaczego potrzebujesz konta służbowego

Firma Microsoft wymaga połączenia firmowego konta służbowego z nowym Partner Center konta. Link umożliwia użytkownikom konta logowanie się do aplikacji Partner Center przy użyciu nazw użytkowników i haseł kont służbowych.

## <a name="the-work-account-email-address"></a>Adres e-mail konta służbowego

Służbowy adres e-mail lub służbowy adres e-mail jest adresem e-mail dostarczonym przez firmę. Adres e-mail konta służbowego ma zazwyczaj format `you@yourcompany.com` . Osobiste adresy e-mail, takie jak Hotmail, Gmail lub Yahoo, nie są służbowym adresem e-mail i nie mogą być używane Partner Center konta.

Jeśli masz więcej niż jeden prawidłowy służbowy adres e-mail, użyj tego, który jest skojarzony z siedzibą firmy, a nie z działem regionalnym, na przykład użyj adresu e-mail, a nie `contoso.com` `contoso.uk` adresu.

> [!NOTE]  
> Przed użyciem istniejącego konta służbowego zastanów się, ilu użytkowników na koncie służbowym będzie musiało uzyskać dostęp do Partner Center. Jeśli masz użytkowników na koncie służbowym, którzy nie będą potrzebować dostępu do aplikacji Partner Center, rozważ utworzenie nowego konta tylko dla tych użytkowników, którzy będą Partner Center dostępu.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nie masz pewności, czy Twoja firma ma już konto służbowe?

Jeśli nie masz pewności, czy firma ma konto służbowe, wykonaj następujące kroki, aby to sprawdzić. Jeśli masz aktywną subskrypcję usługi Microsoft Azure lub Office 365, masz już konto służbowe.

1. Zaloguj się w witrynie [Azure Portal](https://portal.azure.com).

2. Wybierz Azure Active Directory menu nawigacji, a następnie wybierz pozycję **Custom Domain Nazwy.**

3. Jeśli masz już konto służbowe, nazwa domeny zostanie wymieniona.

Jeśli firma nie ma jeszcze konta służbowego, możesz je utworzyć podczas procesu rejestracji.

Na poniższym diagramie przedstawiono kroki dla kilku typowych scenariuszy:

- określanie, czy masz konto służbowe
- określanie sposobu logowania się do konta służbowego
- określanie, czy musisz utworzyć nowe konto służbowe

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Czy masz konto służbowe, czy musisz je utworzyć?":::

Aby uzyskać więcej informacji na temat dodawania domen w usłudze Azure AD, zobacz [Dodawanie lub kojarzenie domeny w usłudze Azure AD](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Informacje o Microsoft Azure

Microsoft Azure to platforma chmury publicznej, której firmy mogą używać do tworzenia i wdrażania aplikacji oraz zarządzania nimi w globalnej sieci centrów danych zarządzanych przez firmę Microsoft. Firmy używają platformy Azure do tworzenia wirtualnej infrastruktury IT z funkcjami wirtualnymi lub usługami, a nie maszynami fizycznymi.

Po zakupie subskrypcji platformy Azure zasadniczo wynajmujesz dedykowane, bezpieczne miejsce w chmurze publicznej Azure, nie różni się zbytnie od wynajmowania podłogi w budynku biurowym w celu przechowywania fizycznej firmy. Właściciel budynku biurowego jest dzierżawcą.

Konto służbowe platformy Azure to dedykowana i odizolowana wirtualna reprezentacja firmy w chmurze publicznej Platformy Azure, utworzona automatycznie podczas subskrybowania usługi w chmurze firmy Microsoft, takiej jak Azure, Microsoft Intune lub Office 365.

Twoje konto służbowe hostuje użytkowników usługi Azure AD i informacje o nich — ich hasła, dane profilu, uprawnienia i tak dalej. Konto służbowe zawiera również grupy, aplikacje i inne informacje dotyczące firmy i jej zabezpieczeń.

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie kontem w portalu Partner Center](partner-center-account-setup.md)
- [Śledzenie stanu weryfikacji](verification-responses.md)
