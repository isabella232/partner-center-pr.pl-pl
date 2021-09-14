---
title: Dodawanie dzierżaw na koncie w Centrum partnerskim
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Dowiedz się, jak dodawać, konsolidować lub zarządzać wieloma dzierżawami usługi Azure AD na koncie usługi Partner Center, i dowiedz się, dlaczego warto to zrobić.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2bb4507fd7e5f60584c8fca99256c964a7521dc8
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247486"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Dodawanie wielu dzierżaw na koncie usługi Partner Center zarządzanie nimi


**Odpowiednie role:** Administrator globalny | Administrator konta

W tym artykule omówiono sposób konsolidowania wielu dzierżaw usługi Azure Active Directory (Azure AD) dla firmy, a następnie dodawania ich i zarządzania nimi na koncie Partner Center dzierżawy. Istnieje wiele powodów, aby to zrobić. Na przykład:

- Załóżmy, że Twoja firma, Contoso, nabyła inną firmę, Fabrikam. Chcesz, aby te dwie firmy pozostały oddzielone, ale chcesz, aby nowi pracownicy mogli korzystać z Partner Center. W takim przypadku należy skojarzyć dzierżawę usługi Azure AD nowej firmy z globalnym kontem partnera (PGA). To skojarzenie umożliwia użytkownikom w obu firmach pracę w Partner Center.

- W przypadku prowadzenia firmy z więcej niż jedną dzierżawą (na przykład *contoso.com*, *contoso.uk* i *contoso.in)* można użyć wielodostępności do grupowania ich na tym samym koncie komputera.

- Jeśli wytyczne dotyczące fuzjów i pozyskiwania wymagają współpracy z  dzierżawami obu firm, należy użyć zarówno constoso.com, jak *i fabrikam.com* dzierżawców.

- Użytkownicy dowolnej dzierżawy muszą mieć możliwość:
    * Dostęp Partner Center do szkoleń, pobierania cyfrowego lub skojarzenia Professional Microsoft Certified Professional (MCP).
    * Mieć przypisane Partner Center, takie jak Microsoft Partner Network (MPN) lub administrator zachęt.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Dodawanie dzierżawy usługi Azure AD do konta

1. Zaloguj się jako administrator globalny do usługi [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. W prawym górnym rogu wybierz pozycję **Ustawienia** pozycję **Ustawienia konta,** a następnie pozycję **Dzierżawy.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Zrzut ekranu przedstawiający przycisk Skojarz w okienku Profil usługi Azure AD."::: 

1. Wybierz **pozycję Skojarz,** a następnie wskaż dzierżawę, którą chcesz skojarzyć.

1. Po wyświetleniu monitu zaloguj się jako administrator globalny do dzierżawy, którą chcesz skojarzyć, a następnie wybierz pozycję **Potwierdź.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zrzut ekranu przedstawiający przycisk Potwierdź w okienku Potwierdzanie nowego skojarzenia usługi Azure AD."::: 

   Po potwierdzeniu skojarzenia zostanie **wyświetlony komunikat Wszystkie** zestawy. Aby wyświetlić nowo dodaną dzierżawę, wybierz pozycję **Powrót do zarządzania dzierżawą.** 
 
>[!NOTE]
>Nie można skojarzyć dzierżawy z kontem, jeśli jest ona już skojarzona z innym Partner Center kontem.


## <a name="remove-a-tenant-from-your-account"></a>Usuwanie dzierżawy z konta
 
1. Zaloguj się jako administrator globalny do usługi [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. W prawym górnym rogu wybierz **ikonę Ustawienia,** a następnie wybierz **pozycję Ustawienia konta.**

1. W okienku po lewej stronie wybierz **pozycję Dzierżawy.** W **obszarze Zarządzanie dzierżawami usługi Azure AD** wybierz **kartę Partner.**
 
1. Wybierz **pozycję Usuń** obok dzierżawy, której skojarzenie chcesz usunąć.

   :::image type="content" source="images/disassociate.png" alt-text="Zrzut ekranu przedstawiający bieżące skojarzenia dzierżawy i ich linki Usuń.":::

   Jak pokazano na poprzednim  zrzucie ekranu, linki Usuń są włączone dla wszystkich skojarzonych dzierżaw, z wyjątkiem dzierżawy podstawowej i dzierżawy, do których użytkownik jest aktualnie zalogowany. 

   > [!NOTE]   
   > Po usunięciu dzierżawy użytkownicy w tej dzierżawie nie mają już dostępu do konta usługi Partner Center, a usunięcie może mieć wpływ na Twoje kompetencje. 

## <a name="next-steps"></a>Następne kroki

- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)






