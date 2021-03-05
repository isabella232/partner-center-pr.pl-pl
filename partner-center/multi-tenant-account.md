---
title: Dodawanie dzierżawców do konta Centrum partnerskiego
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżawców usługi Azure AD na koncie Centrum partnerskiego oraz zarządzać nimi, a także dowiedzieć się, dlaczego warto to zrobić.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124809"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Dodawanie wielu dzierżawców i zarządzanie nimi na koncie Centrum partnerskiego


**Odpowiednie role**

- Administrator globalny
- Administrator konta

W tym artykule omówiono sposób konsolidowania wielu dzierżaw Azure Active Directory (Azure AD) dla Twojej firmy, a następnie dodawania ich i zarządzania nimi na koncie Centrum partnerskiego. Istnieje wiele powodów, dla których należy to zrobić. Na przykład:

- Załóżmy, że firma Contoso uzyska kolejną firmę, firmę fabrikam. Chcesz, aby dwie firmy pozostały do oddzielenia, ale chcesz, aby nowi pracownicy mogli korzystać z Centrum partnerskiego. W takim przypadku należy skojarzyć dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA). To skojarzenie umożliwia użytkownikom w obu firmach działanie w centrum partnerskim.

- Jeśli uruchamiasz swoją firmę z więcej niż jedną dzierżawą (na przykład *contoso.com*, *contoso.uk* i *contoso.in*), możesz użyć wielodostępności, aby ZGRUPOWAĆ je na tym samym koncie komputera.

- Jeśli fuzje i wskazówki dotyczące pozyskiwania wymagają pracy z dzierżawcami obu firm, należy użyć zarówno dzierżaw *constoso.com* , jak i *fabrikam.com* .

- Użytkownicy dowolnych dzierżawców muszą mieć możliwość:
    * Centrum partnerskie dostępu do szkoleń, plików cyfrowych i skojarzeń Microsoft Certified Professional (MCP).
    * Należy przypisać role Centrum partnerskiego, takie jak administrator Microsoft Partner Network (MPN) lub administrator zachęt.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Dodawanie dzierżawy usługi Azure AD do konta

1. Zaloguj się jako Administrator globalny do [Centrum partnerskiego firmy Microsoft](https://partner.microsoft.com/dashboard).

1. W prawym górnym rogu wybierz pozycję **Ustawienia**, wybierz pozycję **Ustawienia konta**, a następnie wybierz pozycję **dzierżawy**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Zrzut ekranu przedstawiający przycisk Skojarz w okienku profil usługi Azure AD."::: 

1. Wybierz pozycję **Skojarz**, a następnie wskaż dzierżawcę, który chcesz skojarzyć.

1. W wierszu polecenia Zaloguj się jako Administrator globalny do dzierżawy, którą chcesz skojarzyć, a następnie wybierz pozycję **Potwierdź**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zrzut ekranu przedstawiający przycisk Potwierdź w okienku Potwierdź nowe skojarzenie usługi Azure AD."::: 

   Po potwierdzeniu skojarzenia zostanie wyświetlony komunikat **cała grupa** . Aby wyświetlić nowo dodaną dzierżawę, wybierz pozycję **Wróć do zarządzania dzierżawcą**. 
 
>[!NOTE]
>Nie można skojarzyć dzierżawy z kontem, jeśli jest ono już skojarzone z innym kontem Centrum partnerskiego.


## <a name="remove-a-tenant-from-your-account"></a>Usuwanie dzierżawy z konta
 
1. Zaloguj się jako Administrator globalny do [Centrum partnerskiego firmy Microsoft](https://partner.microsoft.com/dashboard).

1. W prawym górnym rogu wybierz ikonę **Ustawienia** , a następnie wybierz pozycję **Ustawienia konta**.

1. W okienku po lewej stronie wybierz pozycję **dzierżawy**. W obszarze **Zarządzanie dzierżawami usługi Azure AD** wybierz kartę **partner** .
 
1. Wybierz pozycję **Usuń** obok dzierżawy, której skojarzenie chcesz usunąć.

   :::image type="content" source="images/disassociate.png" alt-text="Zrzut ekranu przedstawiający bieżące skojarzenia dzierżawców i ich linki do usunięcia.":::

   Jak pokazano na poprzednim zrzucie ekranu, łącza **Usuń** są włączone dla wszystkich skojarzonych dzierżawców, z wyjątkiem głównej dzierżawy i dzierżawy, do której użytkownik jest aktualnie zalogowany. 

   > [!NOTE]   
   > Po usunięciu dzierżawy użytkownicy tej dzierżawy nie mają już dostępu do konta Centrum partnerskiego, a usunięcie może mieć wpływ na swoje kompetencje. 

## <a name="next-steps"></a>Następne kroki

- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)






