---
title: Łączenie konta służbowego w celu uzyskania dostępu do Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utwórz konto służbowe, które łączy Twoją firmę z Partner Center kontem. Dzięki temu pracownicy w firmie mogą uzyskać dostęp do Partner Center.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 6/17/2021
ms.openlocfilehash: 69aa45de55a4356eaab1bcd4cd309feb14de9f6e
ms.sourcegitcommit: 0410e2a3f91b7e6b592cc47e7af1dfbe468c7881
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112318065"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="1ec82-104">Tworzenie konta służbowego, które łączy twoją firmę z kontem Partner Center konto</span><span class="sxs-lookup"><span data-stu-id="1ec82-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="1ec82-105">**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="1ec82-105">**Appropriate roles**: Global admin | User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="1ec82-106">Dlaczego potrzebujesz konta służbowego</span><span class="sxs-lookup"><span data-stu-id="1ec82-106">Why you need a work account</span></span>

<span data-ttu-id="1ec82-107">Firma Microsoft wymaga połączenia firmowego konta służbowego z nowym Partner Center konta.</span><span class="sxs-lookup"><span data-stu-id="1ec82-107">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="1ec82-108">Link umożliwia użytkownikom konta logowanie się do aplikacji Partner Center przy użyciu nazw użytkowników i haseł kont służbowych.</span><span class="sxs-lookup"><span data-stu-id="1ec82-108">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="1ec82-109">Adres e-mail konta służbowego</span><span class="sxs-lookup"><span data-stu-id="1ec82-109">The work account email address</span></span>

<span data-ttu-id="1ec82-110">Służbowy adres e-mail lub służbowy adres e-mail jest adresem e-mail dostarczonym przez firmę.</span><span class="sxs-lookup"><span data-stu-id="1ec82-110">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="1ec82-111">Adres e-mail konta służbowego ma zazwyczaj format `you@yourcompany.com` .</span><span class="sxs-lookup"><span data-stu-id="1ec82-111">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="1ec82-112">Osobiste adresy e-mail, takie jak Hotmail, Gmail lub Yahoo, nie są służbowym adresem e-mail i nie mogą być używane Partner Center konta.</span><span class="sxs-lookup"><span data-stu-id="1ec82-112">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="1ec82-113">Jeśli masz więcej niż jeden prawidłowy służbowy adres e-mail, użyj tego, który jest skojarzony z siedzibą firmy, a nie z działem regionalnym, na przykład użyj adresu e-mail, a nie `contoso.com` `contoso.uk` adresu.</span><span class="sxs-lookup"><span data-stu-id="1ec82-113">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="1ec82-114">Przed użyciem istniejącego konta służbowego zastanów się, ilu użytkowników na koncie służbowym będzie musiało uzyskać dostęp do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1ec82-114">Before you use an existing work account, think about how many users in the work account will need to access Partner Center.</span></span> <span data-ttu-id="1ec82-115">Jeśli masz użytkowników na koncie służbowym, którzy nie będą potrzebować dostępu do aplikacji Partner Center, rozważ utworzenie nowego konta tylko dla tych użytkowników, którzy będą Partner Center dostępu.</span><span class="sxs-lookup"><span data-stu-id="1ec82-115">If you have users in the work account who won't need access to Partner Center, consider creating a new account for only those users who will need Partner Center access.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="1ec82-116">Nie masz pewności, czy Twoja firma ma już konto służbowe?</span><span class="sxs-lookup"><span data-stu-id="1ec82-116">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="1ec82-117">Jeśli nie masz pewności, czy firma ma konto służbowe, wykonaj następujące kroki, aby to sprawdzić.</span><span class="sxs-lookup"><span data-stu-id="1ec82-117">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="1ec82-118">Jeśli masz aktywną subskrypcję usługi Microsoft Azure lub Office 365, masz już konto służbowe.</span><span class="sxs-lookup"><span data-stu-id="1ec82-118">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="1ec82-119">Zaloguj się w witrynie [Azure Portal](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="1ec82-119">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="1ec82-120">Wybierz Azure Active Directory menu nawigacji, a następnie wybierz **pozycję Custom Domain Nazwy.**</span><span class="sxs-lookup"><span data-stu-id="1ec82-120">Select Azure Active Directory from the navigation menu and select **Custom Domain Names**.</span></span>

3. <span data-ttu-id="1ec82-121">Jeśli masz już konto służbowe, nazwa domeny zostanie wymieniona.</span><span class="sxs-lookup"><span data-stu-id="1ec82-121">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="1ec82-122">Jeśli firma nie ma jeszcze konta służbowego, możesz je utworzyć podczas procesu rejestracji.</span><span class="sxs-lookup"><span data-stu-id="1ec82-122">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="1ec82-123">Na poniższym diagramie przedstawiono kroki dla kilku typowych scenariuszy:</span><span class="sxs-lookup"><span data-stu-id="1ec82-123">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="1ec82-124">określanie, czy masz konto służbowe</span><span class="sxs-lookup"><span data-stu-id="1ec82-124">determine if you have a work account</span></span>
- <span data-ttu-id="1ec82-125">określanie sposobu logowania się do konta służbowego</span><span class="sxs-lookup"><span data-stu-id="1ec82-125">determine how to sign into your work account</span></span>
- <span data-ttu-id="1ec82-126">określanie, czy musisz utworzyć nowe konto służbowe</span><span class="sxs-lookup"><span data-stu-id="1ec82-126">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Czy masz konto służbowe, czy musisz je utworzyć?":::

<span data-ttu-id="1ec82-128">Aby uzyskać więcej informacji na temat dodawania domen w usłudze Azure AD, zobacz [Dodawanie lub kojarzenie domeny w usłudze Azure AD](/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="1ec82-128">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="1ec82-129">Informacje o Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1ec82-129">About Microsoft Azure</span></span>

<span data-ttu-id="1ec82-130">Microsoft Azure to platforma chmury publicznej, której firmy mogą używać do tworzenia i wdrażania aplikacji oraz zarządzania nimi w globalnej sieci centrów danych zarządzanych przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1ec82-130">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="1ec82-131">Firmy używają platformy Azure do tworzenia wirtualnej infrastruktury IT z funkcjami wirtualnymi lub usługami, a nie maszynami fizycznymi.</span><span class="sxs-lookup"><span data-stu-id="1ec82-131">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="1ec82-132">Po zakupie subskrypcji platformy Azure zasadniczo wynajmujesz dedykowane, bezpieczne miejsce w chmurze publicznej Azure, nie różni się zbytnie od wynajmowania podłogi w budynku biurowym w celu przechowywania fizycznej firmy.</span><span class="sxs-lookup"><span data-stu-id="1ec82-132">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="1ec82-133">Właściciel budynku biurowego jest dzierżawcą.</span><span class="sxs-lookup"><span data-stu-id="1ec82-133">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="1ec82-134">Konto służbowe platformy Azure to dedykowana i odizolowana wirtualna reprezentacja firmy w chmurze publicznej platformy Azure utworzona automatycznie podczas subskrybowania usługi w chmurze firmy Microsoft, takiej jak Azure, Microsoft Intune lub Office 365.</span><span class="sxs-lookup"><span data-stu-id="1ec82-134">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="1ec82-135">Twoje konto służbowe hostuje użytkowników usługi Azure AD i informacje o nich — ich hasła, dane profilu, uprawnienia i tak dalej.</span><span class="sxs-lookup"><span data-stu-id="1ec82-135">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="1ec82-136">Konto służbowe zawiera również grupy, aplikacje i inne informacje dotyczące firmy i jej zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="1ec82-136">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1ec82-137">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="1ec82-137">Next steps</span></span>

- [<span data-ttu-id="1ec82-138">Zarządzanie kontem w portalu Partner Center</span><span class="sxs-lookup"><span data-stu-id="1ec82-138">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="1ec82-139">Śledzenie stanu weryfikacji</span><span class="sxs-lookup"><span data-stu-id="1ec82-139">Track verification status</span></span>](verification-responses.md)
