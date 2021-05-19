---
title: Dodawanie dzierżaw do konta Partner Center dzierżawy
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak dodawać i konsolidować wiele dzierżaw usługi Azure AD Partner Center konta usługi Azure AD oraz jak nimi zarządzać, i dowiedz się, dlaczego warto to zrobić.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151206"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Dodawanie wielu dzierżaw na koncie usługi Partner Center zarządzanie nimi


**Odpowiednie role:** Administrator globalny | Administrator konta

W tym artykule omówiono sposób konsolidowania wielu dzierżaw usługi Azure Active Directory (Azure AD) dla firmy, a następnie dodawania ich i zarządzania nimi na koncie Partner Center dzierżawy. Istnieje wiele powodów, aby to zrobić. Na przykład:

- Załóżmy, że Twoja firma, Contoso, nabyła inną firmę, Fabrikam. Chcesz, aby obie firmy pozostały oddzielone, ale chcesz, aby nowi pracownicy mogli korzystać z Partner Center. W takim przypadku skojarzysz dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA). To skojarzenie umożliwia użytkownikom w obu firmach pracę w Partner Center.

- Jeśli firma działa z więcej niż jedną dzierżawą (na przykład *contoso.com*, *contoso.uk* i *contoso.in*), można użyć wielodostępności, aby zgrupować je na tym samym koncie komputera.

- Jeśli wytyczne dotyczące koncentracji i pozyskiwania wymagają współpracy z dzierżawami  obu firm, należy użyć zarówno constoso.com, *jak i fabrikam.com* dzierżawców.

- Użytkownicy dowolnej dzierżawy muszą mieć możliwość:
    * Dostęp Partner Center do szkoleń, pobierania cyfrowego lub skojarzenia Microsoft Certified Professional (MCP).
    * Mieć przypisane Partner Center, takie jak Microsoft Partner Network (MPN) lub administrator zachęt.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Dodawanie dzierżawy usługi Azure AD do konta

1. Zaloguj się jako administrator globalny w aplikacji [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. W prawym górnym rogu wybierz pozycję **Ustawienia,** wybierz **pozycję Ustawienia konta,** a następnie wybierz **pozycję Dzierżawy.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Zrzut ekranu przedstawiający przycisk Skojarz w okienku Profil usługi Azure AD."::: 

1. Wybierz **pozycję Skojarz,** a następnie wskaż dzierżawę, którą chcesz skojarzyć.

1. Po wyświetleniu monitu zaloguj się jako administrator globalny do dzierżawy, którą chcesz skojarzyć, a następnie wybierz pozycję **Potwierdź.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zrzut ekranu przedstawiający przycisk Potwierdź w okienku Potwierdzanie nowego skojarzenia usługi Azure AD."::: 

   Po potwierdzeniu skojarzenia zostanie wyświetlony **komunikat Wszystkie** zestawy. Aby wyświetlić nowo dodaną dzierżawę, wybierz pozycję **Powrót do zarządzania dzierżawą.** 
 
>[!NOTE]
>Nie można skojarzyć dzierżawy z kontem, jeśli jest ona już skojarzona z innym Partner Center kontem.


## <a name="remove-a-tenant-from-your-account"></a>Usuwanie dzierżawy z konta
 
1. Zaloguj się jako administrator globalny w aplikacji [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. W prawym górnym rogu wybierz **ikonę Ustawienia,** a następnie wybierz **pozycję Ustawienia konta.**

1. W okienku po lewej stronie wybierz **pozycję Dzierżawy.** W **obszarze Zarządzanie dzierżawami usługi Azure AD** wybierz **kartę Partner.**
 
1. Wybierz **pozycję Usuń** obok dzierżawy, której skojarzenie chcesz usunąć.

   :::image type="content" source="images/disassociate.png" alt-text="Zrzut ekranu przedstawiający bieżące skojarzenia dzierżawy i ich linki Usuń.":::

   Jak pokazano na poprzednim  zrzucie ekranu, linki Usuń są włączone dla wszystkich skojarzonych dzierżaw, z wyjątkiem dzierżawy podstawowej i dzierżawy, do których aktualnie się zalogowano. 

   > [!NOTE]   
   > Po usunięciu dzierżawy użytkownicy w tej dzierżawie nie mają już dostępu do konta usługi Partner Center, a usunięcie może mieć wpływ na Twoje kompetencje. 

## <a name="next-steps"></a>Następne kroki

- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)






