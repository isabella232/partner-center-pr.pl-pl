---
title: Dodawanie dzierżaw na koncie w Centrum partnerskim
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Dowiedz się, jak dodawać, konsolidować lub zarządzać wieloma dzierżawami usługi Azure AD na koncie usługi Partner Center, i dowiedz się, dlaczego warto to zrobić.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1e116a6d7aa17cd01a0dfb0342c6f76ad78c448
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073643"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Dodawanie wielu dzierżaw na koncie usługi Partner Center zarządzanie nimi


**Odpowiednie role:** Administrator globalny | Administrator konta

W tym artykule omówiono sposób konsolidowania wielu dzierżaw usługi Azure Active Directory (Azure AD) dla firmy, a następnie dodawania ich i zarządzania nimi na koncie Partner Center dzierżawy. Istnieje wiele powodów, aby to zrobić. Na przykład:

- Załóżmy, że Twoja firma Contoso nabyła inną firmę, Fabrikam. Chcesz, aby obie firmy pozostały oddzielone, ale chcesz, aby nowi pracownicy mogli korzystać z Partner Center. W takim przypadku skojarzysz dzierżawę usługi Azure AD nowej firmy z kontem globalnym partnera (PGA). To skojarzenie umożliwia użytkownikom w obu firmach pracę w Partner Center.

- Jeśli firma działa z więcej niż jedną dzierżawą (na przykład *contoso.com*, *contoso.uk* i *contoso.in*), można użyć wielodostępności, aby zgrupować je na tym samym koncie komputera.

- Jeśli wytyczne dotyczące fuzji i pozyskiwania wymagają współpracy z  dzierżawami obu firm, należy użyć zarówno constoso.com, *jak i fabrikam.com* dzierżawców.

- Użytkownicy dowolnej dzierżawy muszą mieć możliwość:
    * Dostęp Partner Center do szkoleń, pobierania cyfrowego lub skojarzenia z Professional Microsoft Certified MCP).
    * Mieć przypisane Partner Center, takie jak Microsoft Partner Network (MPN) lub administrator zachęt.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Dodawanie dzierżawy usługi Azure AD do konta

1. Zaloguj się do [pulpitu Partner Center jako](https://partner.microsoft.com/dashboard) administrator globalny.

2. Wybierz ikonę Ustawienia koła zębatego, a następnie **pozycję Ustawienia konta,** a następnie wybierz **pozycję Dzierżawy.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Zrzut ekranu przedstawiający przycisk Skojarz w okienku Profil usługi Azure AD.":::

3. Wybierz pozycję Skojarz, a następnie wskaż dzierżawę, którą chcesz skojarzyć. 

4. Po wyświetleniu monitu zaloguj się jako administrator globalny do dzierżawy, którą chcesz skojarzyć, a następnie wybierz pozycję **Potwierdź**.

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Zrzut ekranu przedstawiający przycisk Potwierdź w okienku Potwierdzanie nowego skojarzenia usługi Azure AD.":::

   Po potwierdzeniu skojarzenia zostanie wyświetlony **komunikat Wszystkie** zestawy. Aby wyświetlić nowo dodaną dzierżawę, wybierz pozycję **Powrót do zarządzania dzierżawą.**

> [!NOTE]
> Nie można skojarzyć dzierżawy z kontem, jeśli jest ona już skojarzona z innym Partner Center kontem.

## <a name="remove-a-tenant-from-your-account"></a>Usuwanie dzierżawy z konta

1. Zaloguj się jako administrator globalny w aplikacji [Microsoft Partner Center.](https://partner.microsoft.com/dashboard)

2. Wybierz ikonę Ustawienia koła zębatego, a następnie **pozycję Ustawienia konta,** a następnie wybierz **pozycję Dzierżawy.**

3. Wybierz kartę **Partner**.

4. Wybierz **pozycję Usuń** obok dzierżawy, której skojarzenie chcesz usunąć.

   :::image type="content" source="images/disassociate.png" alt-text="Zrzut ekranu przedstawiający bieżące skojarzenia dzierżawy i ich linki Usuń.":::

   Jak pokazano na poprzednim  zrzucie ekranu, linki Usuń są włączone dla wszystkich skojarzonych dzierżaw, z wyjątkiem dzierżawy podstawowej i dzierżawy, do których aktualnie się zalogowano.

   > [!NOTE]
   > Po usunięciu dzierżawy użytkownicy w tej dzierżawie nie mają już dostępu do konta Partner Center, a usunięcie może mieć wpływ na Twoje kompetencje.

## <a name="next-steps"></a>Następne kroki

- [Tworzenie kont użytkowników](create-user-accounts-and-set-permissions.md)
