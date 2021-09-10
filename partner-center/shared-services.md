---
title: Dodawanie Azure Partner Shared Services
description: Użyj Azure Partner Shared Services, aby kupić subskrypcje platformy Azure na własny użytek i uzyskać ujednoliconą metodę zakupu, śledzenia i zarządzania platformą Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 35c5d378f66071f3c97abdf74eec27e78a8ac778
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123958870"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Dodaj Azure Partner Shared Services, aby partnerzy mogą kupować subskrypcje platformy Azure na własny użytek

**Odpowiednie role:** Administrator globalny | Agent administracyjny | Agent sprzedaży

Azure Partner Shared Services (APSS) to nowy typ oferty dla partnerów w programie Dostawca rozwiązań w chmurze (CSP), który umożliwia partnerom kupowanie subskrypcji platformy Azure na własny użytek.Daje partnerom możliwość korzystania z jednolitej metody zakupów, śledzenia i zarządzania platformą Azure, a także możliwości skonsolidowania umów licencjonowania platformy Azure i odsprzedawczych z firmą Microsoft. Dzięki usłudze APSS partnerzy mają teraz taką samą elastyczność korzystania z subskrypcji platformy Azure w programie CSP, jak w programach Microsoft Enterprise Agreement i Web Direct, otwierając scenariusze, takie jak: tworzenie środowisk deweloperskich i testowych, wdrażanie obciążeń wewnętrznych oraz hostowania usług udostępnionych lub aplikacji wielodostępnych.  

## <a name="create-the-shared-services-tenant"></a>Tworzenie dzierżawy usług udostępnionych

1. Przejdź do **Ustawienia**  >  **konta Usługi**  >  **udostępnione.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Ustawienia konta > usług udostępnionych":::

2. Jeśli nie masz jeszcze dzierżawy usług udostępnionych, wybierz pozycję **Utwórz usługi udostępnione.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Tworzenie usług udostępnionych.":::

3. Powoduje to utworzenie dzierżawy usług udostępnionych i zakup Azure CSP usług udostępnionych, która będzie używana dla zasobów udostępnionych i obciążeń wewnętrznych.

   :::image type="content" source="images/sharedservices5.png" alt-text="Utwórz dzierżawę i kup subskrypcję.":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informacje o Azure — usługi wewnętrzne/udostępnione oferty

- Subskrypcja Azure — usługi wewnętrzne/udostępnione to nowy typ oferty platformy Azure w programie CSP dostępnym za pośrednictwem Partner Center, który partnerzy mogą uzyskać na własny użytek z platformy Azure.

- Azure Partner Shared Services są uprawnione i mogą być używane do zakupu interfejsów API.

- Ofertę Azure — usługi wewnętrzne/udostępnione można zastosować tylko do dzierżawy usług udostępnionych.

- Podstawowym zastosowaniem subskrypcji Azure — usługi wewnętrzne/udostępnione jest użycie platformy Azure do własnych celów programistyczych. Udostępnionej dzierżawy używanej do aprowiwizować tej oferty nie można używać w przypadku innych usług, takich jak Office 365 licencji usługi Dynamics.

- Możesz anulować subskrypcję, tak jak każdą inną subskrypcję. Przejdź do ustawień  >  **ustawień Wyświetl wszystko usługi**  >  **udostępnione.** Wybierz subskrypcję Azure — usługi wewnętrzne/udostępnione i anuluj ją.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Uzyskiwanie dostępu do Azure Partner Shared Services szczegółów użycia

Zużycie platformy Azure znajdziesz na fakturze za program CSP i pliku uzgodnień. Zostanie ona uwzględniona jako część Microsoft Azure na fakturze. Szczegółowe informacje o zużyciu będą dostępne w pliku uzgodnień zarejestrowanym dla dzierżawy utworzonej dla tej oferty.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services cen

Aby wyświetlić nowy plik cennika usługi APSS, przejdź do sekcji **Sell** Pricing and offers (Sprzedawaj ceny i oferty) i wybierz cennik  >   z bieżącego miesiąca. W najbliższych tygodniach zostanie również wydany interfejs API karty z określoną szybkością.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Oferty i Azure Partner Shared Services Marketplace

Od 1 marca 2019 r. platforma APSS nie obsługuje już ofert w witrynie Marketplace.

|**Obsługa witryny Marketplace**   |**APSS obsługiwane przed 1 marca 2019 r.**|**Po 1 marca 2019 r.**|
|---------------------------|:----------------------------|:-------------------|
|Bring your own license (BYOL) i bezpłatne usługi   | Tak   | Nie|
|Inne oferty na platformie handlowej innych firm   | Nie   |Nie|

Nie będzie to miało wpływu na partnerów, którzy mają usługę BYOL lub bezpłatne usługi wdrożone przy użyciu usługi APSS; jednak po 1 marca 2019 r. nie będą mogli zakupić nowych usług BYOL ani bezpłatnych.

Aby skorzystać z pełnego katalogu dostępnych ofert witryny Marketplace (nie tylko BYOL i bezpłatnych usług), zalecamy partnerom programu CSP wdrażanie usług udostępnionych przy użyciu bezpośrednich subskrypcji internetowych platformy Azure.  Partnerzy programu CSP, którzy wcześniej wdrożyli zasoby usług innych firm i bezpłatnych usług z witryny Marketplace oraz chcą nadal z nich korzystać i wdrażać więcej ofert innych firm, są zachęcani do migrowania subskrypcji APSS do bezpośredniej migracji istniejącej subskrypcji platformy [Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)w sieci Web.

Partnerzy, którzy planują dalsze korzystanie z subskrypcji APSS po 1 marca 2019 r. i chcą wdrożyć nowe usługi [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) innych firm lub bezpłatne usługi, mogą postępować zgodnie z instrukcjami od isvs, aby wdrożyć je w swoich subskrypcjach APSS.

## <a name="next-steps"></a>Następne kroki

- [Sprzedaż subskrypcji oprogramowania za pośrednictwem dostawcy rozwiązań w chmurze (CSP)](csp-software-subscriptions.md)