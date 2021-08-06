---
title: Dodaj Azure Partner Shared Services
description: Użyj Azure Partner Shared Services, aby kupić subskrypcje platformy Azure na własny użytek oraz uzyskać ujednoliconą metodę zakupu i śledzenia platformy Azure oraz zarządzania nimi.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: d160a63969c66736afca7221a78c4448e7fe117ccbb7882846ed7bad22002df5
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115678104"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Dodaj Azure Partner Shared Services, aby partnerzy mogą kupować subskrypcje platformy Azure na własny użytek

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Agent sprzedaży

Azure Partner Shared Services (APSS) to nowy typ oferty dla partnerów w programie Dostawca rozwiązań w chmurze (CSP), który umożliwia partnerom kupowanie subskrypcji platformy Azure na własny użytek.Daje to partnerom możliwość korzystania z jednolitej metody zakupu, śledzenia i zarządzania platformą Azure, a także możliwości skonsolidowania umów licencjonowania platformy Azure i sprzedaży z firmą Microsoft. Dzięki usłudze APSS partnerzy mają teraz taką samą elastyczność korzystania z subskrypcji platformy Azure w programie CSP, jak w programach Microsoft Enterprise Agreement i Web Direct, otwierając scenariusze, takie jak: tworzenie środowisk deweloperskich i testowych, wdrażanie obciążeń wewnętrznych oraz hostowania usług udostępnionych lub aplikacji wielodostępnych.  

## <a name="create-the-shared-services-tenant"></a>Tworzenie dzierżawy usług udostępnionych

1. Przejdź do **Ustawienia**  >  **Ustawienia konta Usługi**  >  **udostępnione.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Ustawienia konta > usług udostępnionych":::

2. Jeśli nie masz jeszcze dzierżawy usług udostępnionych, wybierz pozycję **Utwórz usługi udostępnione.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Tworzenie usług udostępnionych.":::

3. Powoduje to utworzenie dzierżawy usług udostępnionych i zakup Azure CSP usług udostępnionych na potrzeby zasobów udostępnionych i obciążenia wewnętrznego.

   :::image type="content" source="images/sharedservices5.png" alt-text="Utwórz dzierżawę i kup subskrypcję.":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informacje o Azure — usługi wewnętrzne/udostępnione usługi

- Subskrypcja Azure — usługi wewnętrzne/udostępnione to nowy typ oferty platformy Azure w programie CSP dostępnym za pośrednictwem usługi Partner Center, który partnerzy mogą uzyskać na własny użytek z platformy Azure.

- Azure Partner Shared Services kwalifikują się i mogą być używane do zakupu interfejsów API.

- Ofertę Azure — usługi wewnętrzne/udostępnione można zastosować tylko do dzierżawy usług udostępnionych.

- Podstawowym zastosowaniem subskrypcji Azure — usługi wewnętrzne/udostępnione jest to, że platformy Azure można używać do własnych celów programistych. Udostępnionej dzierżawy używanej do aprowizować tej oferty nie można używać w przypadku innych usług, takich jak Office 365 licencji usługi Dynamics.

- Możesz anulować subskrypcję, tak jak każdą inną subskrypcję. Przejdź do ustawień **usługi**  >  **Wyświetl wszystko usługi**  >  **udostępnione.** Wybierz subskrypcję Azure — usługi wewnętrzne/udostępnione i anuluj ją.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Uzyskiwanie dostępu do Azure Partner Shared Services szczegółów użycia

Zużycie platformy Azure znajdziesz na fakturze za program CSP i w pliku uzgodnień. Zostanie ona uwzględniona jako część Microsoft Azure na fakturze. Szczegółowe informacje o zużyciu będą dostępne w pliku uzgodnień zarejestrowanym dla dzierżawy utworzonej dla tej oferty.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services cenowe

Aby wyświetlić nowy plik cennika usługi APSS, przejdź do sekcji **Sell** Pricing and offers (Sprzedawaj ceny i oferty) i wybierz  >   cennik bieżącego miesiąca. W najbliższych tygodniach zostanie również wydany interfejs API karty z określoną szybkością.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Oferty i oferty w witrynie Marketplace Azure Partner Shared Services

Od 1 marca 2019 r. platforma APSS nie obsługuje już ofert w witrynie Marketplace.

|**Pomoc techniczna w witrynie Marketplace**   |**APSS obsługiwane przed 1 marca 2019 r.**|**Po 1 marca 2019 r.**|
|---------------------------|:----------------------------|:-------------------|
|Bring your own license (BYOL) i bezpłatne usługi   | Tak   | Nie|
|Inne oferty na platformie handlowej innych firm   | Nie   |Nie|

Nie będzie to miało wpływu na partnerów, którzy mają usługę BYOL lub bezpłatne usługi wdrożone przy użyciu usługi APSS; jednak po 1 marca 2019 r. nie będą mogli kupować nowych usług BYOL ani bezpłatnych usług.

Aby skorzystać z pełnego katalogu dostępnych ofert witryny Marketplace (nie tylko byol i bezpłatnych usług), zalecamy partnerom programu CSP wdrażanie usług udostępnionych przy użyciu bezpośrednich subskrypcji internetowych platformy Azure.  Partnerzy programu CSP, którzy wcześniej wdrożyli zasoby usług bezpłatnych i byOL innych firm z witryny Marketplace i chcą nadal z nich korzystać oraz wdrażać więcej ofert innych firm, są zachęcani do migrowania subskrypcji APSS do bezpośredniej migracji w sieci Web istniejących subskrypcji platformy [Azure.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

Partnerzy, którzy planują dalsze korzystanie z subskrypcji APSS po 1 marca 2019 r. i chcą wdrożyć nowe usługi [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) innych firm lub bezpłatne usługi, mogą wykonać instrukcje od isvs, aby wdrożyć je w swoich subskrypcjach APSS.

## <a name="next-steps"></a>Następne kroki

- [Sprzedaż subskrypcji oprogramowania za pośrednictwem dostawcy rozwiązań w chmurze (CSP)](csp-software-subscriptions.md)