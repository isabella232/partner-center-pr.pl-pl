---
title: Dodawanie udostępnionych usług partnerskich platformy Azure
description: Korzystając z udostępnionych usług partnerskich platformy Azure, można kupować subskrypcje platformy Azure do własnych potrzeb i korzystać z jednolitych metod kupowania, śledzenia i zarządzania platformą Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: a59cf0b271a0ccf5fd5a1d8e3e85ff43818a3801
ms.sourcegitcommit: fe867be44de3479607be3309940b904d7ea9fc6e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2021
ms.locfileid: "102247700"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Dodaj udostępnione usługi partnerskie platformy Azure, aby partnerzy mogli kupować subskrypcje platformy Azure pod kątem własnych potrzeb

 
**Odpowiednie role**

- Administrator globalny
- Agent administracyjny
- Agent sprzedaży

Usługi udostępnione partnerskiej platformy Azure to nowy typ oferty dla partnerów w programie CSP, który umożliwia partnerom kupowanie subskrypcji platformy Azure do własnych potrzeb.Umożliwia ona partnerom używanie jednolitej metody do kupowania, śledzenia i zarządzania platformą Azure, a także do konsolidacji licencji na korzystanie z platformy Azure i odsprzedaży umów z firmą Microsoft. Dzięki udostępnionym usługom partnerskim platformy Azure partnerzy mają teraz taką samą elastyczność jak korzystanie z subskrypcji platformy Azure w programie CSP, jak w przypadku programów Microsoft Enterprise Agreement i Web Direct, otwieranie scenariuszy, takich jak tworzenie środowisk deweloperskich i testowych, wdrażanie obciążeń wewnętrznych i hostowanie usług udostępnionych lub aplikacji wielodostępnych.  

## <a name="create-the-shared-services-tenant"></a>Tworzenie dzierżawy usług udostępnionych

1. Przejdź do pozycji **Ustawienia**  >  **konta ustawienia**  >  **usługi udostępnione**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Ustawienia konta > usług udostępnionych":::

2. Jeśli nie masz jeszcze dzierżawy usług udostępnionych, kliknij przycisk **Utwórz usługi udostępnione**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Tworzenie usług udostępnionych":::

3. Spowoduje to utworzenie dzierżawy usług udostępnionych i zakupienie subskrypcji usług udostępnionych CSP platformy Azure, która będzie używana na potrzeby udostępnionych zasobów i obciążenia wewnętrznego.

   :::image type="content" source="images/sharedservices5.png" alt-text="Tworzenie dzierżawy i kupowanie subskrypcji":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informacje o ofercie Azure — usługi wewnętrzne/udostępnione

- Subskrypcja Azure — usługi wewnętrzne/udostępnione jest nowym typem oferty platformy Azure w programie CSP dostępnym za pomocą Centrum partnerskiego, które partnerzy uzyskają w celu korzystania z platformy Azure.

- Subskrypcje udostępnionych usług partnerskich platformy Azure są uprawnione i mogą być używane do kupowania usług RIs.

- Oferta Azure — usługi wewnętrzne/udostępnione może być stosowana tylko do dzierżawy usług udostępnionych.

- Głównym zastosowaniem subskrypcji Azure — usługi wewnętrzne/udostępnione jest użycie platformy Azure do własnych celów deweloperskich. Dzierżawy udostępnionej używanej do aprowizacji tej oferty nie można używać w przypadku innych usług, takich jak Office 365 lub Dynamics.

- Subskrypcję można anulować, podobnie jak w przypadku każdej innej subskrypcji. Przejdź do pozycji **Ustawienia**  >  **Wyświetl wszystkie ustawienia**  >  **udostępnione usługi**. Wybierz subskrypcję Azure — usługi wewnętrzne/udostępnione i Anuluj ją.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Dostęp do szczegółów użycia udostępnionych usług partnerskich platformy Azure

Możesz znaleźć użycie platformy Azure na fakturze dostawcy CSP i pliku uzgodnienia. Zostanie ona uwzględniona jako część elementu wiersza Microsoft Azure w fakturze. Szczegółowe informacje dotyczące użycia będą dostępne w pliku uzgadniania zarejestrowanym dla dzierżawy, która została utworzona dla tej oferty.

## <a name="azure-partner-shared-services-pricing"></a>Cennik usług udostępnionych partnerów platformy Azure

Aby wyświetlić nowy plik cen dla usług udostępnionych partnera platformy Azure, przejdź do pozycji **Sprzedaj**  >  **Cennik i oferty** i wybierz Cennik bieżącego miesiąca. W najbliższych tygodniach zostanie również wydanych określony interfejs API karty rate.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Oferty w witrynie Marketplace i udostępnione usługi partnerskie platformy Azure

Od 1 marca 2019, usługi udostępnione partner Azure (APSS) nie obsługują już ofert z witryny Marketplace.

|**Pomoc techniczna Marketplace**   |**APSS jest obsługiwany przed 1 marca 2019**|**Po 1 marca 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring your own license (BYOL) i bezpłatne usługi   | Tak   | Nie|
|Inne oferty rynkowe innych firm   | Nie   |Nie|

Nie wpłynie to na partnerów, którzy mają BYOLe lub bezpłatne usługi wdrożone przy użyciu APSS. Jednak po 1 marca 2019 nie będzie możliwe zakupienie nowych BYOL lub bezpłatnych usług.

Aby skorzystać z pełnego wykazu dostępnych ofert w portalu Marketplace (nie tylko BYOL i bezpłatnych usług), zalecamy, aby partnerzy CSP wdrażali usługi udostępnione przy użyciu bezpośrednich subskrypcji platformy Azure w sieci Web.  Partnerzy dostawcy usług kryptograficznych, którzy wdrożyły zasoby BYOL i bezpłatnych usług innych firm z rynku Marketplace i chcą nadal korzystać z nich i wdrażają więcej ofert innych firm, zachęcamy do migrowania subskrypcji APSS do sieci Web bezpośrednie [Migrowanie istniejących subskrypcji platformy Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Partnerzy, którzy chcą nadal korzystać z subskrypcji usługi APSS po 1 marca 2019 i chcą wdrożyć nowe [usługi BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) lub bezpłatne usługi innych firm, mogą wykonać instrukcje od niezależnych dostawców oprogramowania, aby wdrożyć je w swoich subskrypcjach APSS.

## <a name="next-steps"></a>Następne kroki

- [Sprzedaż subskrypcji oprogramowania za pośrednictwem dostawcy rozwiązań w chmurze (CSP)](csp-software-subscriptions.md)