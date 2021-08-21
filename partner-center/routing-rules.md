---
title: Tworzenie reguł routingu dla szans przychodzących i zarządzanie nimi
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Twoja firma może utworzyć reguły, aby zdecydować, w jaki sposób są kierowane przychodzące oferty sprzedaży od sprzedawców firmy Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 42238e2ce36725631f542887c9112593d701ca9c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/20/2021
ms.locfileid: "122621706"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Tworzenie reguł routingu dla szans przychodzących i zarządzanie nimi

**Odpowiednie role:** Administrator poleceń | Użytkownik poleceń

> [!IMPORTANT]
> **Tworzenie reguł routingu jest opcjonalne.** Jest to zalecane tylko w przypadku większych firm, które są obecni na całym świecie, lub jeśli firma ma złożoną hierarchię MPN, w której zarządzanie poleceniami ma być wykonywane na poziomie określonej lokalizacji w oparciu o rynki i rozwiązania klientów.

## <a name="introduction"></a>Wprowadzenie

Funkcja opisana w tym dokumencie pomoże Twojej firmie w skonfigurowaniu reguł, które mogą pomóc w skierowaniu możliwości współs sprzedaży wysyłanych przez sprzedawców firmy Microsoft do wybranej przez Ciebie lokalizacji MPN. Domyślnie polecenia od sprzedawcy firmy Microsoft będą wysyłane do lokalizacji MPN skojarzonej z rozwiązaniem do współpracy sprzedaży uwzględnionym w szansie sprzedaży. Utworzone reguły rozsyłania ułatwiają firmie zastąpienie routingu domyślnego. Tylko [**administrator poleceń**](permissions-overview.md#manage-referrals) z całym zakresem organizacji może tworzyć i edytować reguły routingu. Partnerzy z [**rolą użytkownika poleceń**](permissions-overview.md#manage-referrals) mogą tylko wyświetlać reguły rozsyłania, aby zrozumieć, w jaki sposób skierowania są kierowane w firmie.

Reguły nie będą stosowane retrospektywnie. Wszystkie odwołania utworzone w przeszłości lub ze starszą konfiguracją reguły routingu nie zostaną zaktualizowane. Wszelkie zmiany wprowadzone w zasadach mają zastosowanie natychmiast.

Istnieją trzy główne tabele przestawne dla każdej reguły.

- **Rynek klienta** — rynek, na którym znajduje się firma klienta

- **Rozwiązanie** — rozwiązania opublikowane przez twoją firmę za pośrednictwem portalu OCP GTM lub platformy handlowej

- **Lokalizacja MPN** — lokalizacja MPN, do której ma być kierowane polecenie

Każdą regułę można przeczytać w ten sposób — w przypadku poleceń wysyłanych przez sprzedawców firmy Microsoft z rozwiązaniami z mojej firmy należy skierować je do tej lokalizacji **MPN**

> [!Note]
> Reguły rozsyłania ruchu przychodzącego mają zastosowanie tylko w przypadku możliwości współpracy sprzedaży wysyłanych do Twojej firmy przez sprzedawców firmy Microsoft.

## <a name="navigation"></a>Nawigacja

Reguły rozsyłania można tworzyć na **karcie Polecenia** na **stronie Ustawienia** konta. Aby przejść do strony, wybierz ikonę ustawień obok ikony użytkownika w  prawym górnym rogu, a następnie wybierz kartę Polecenia w panelu nawigacyjnym po lewej stronie.

## <a name="initial-setup"></a>Konfiguracja początkowa

**Konfigurowanie reguł routingu nie jest obowiązkowe.** Jeśli firma zdecyduje się na użycie reguł routingu w celu skorzystania z logiki routingu, możesz rozpocząć od zaimportowania domyślnych reguł, których system zarządzania odwołaniami używa do kierowania poleceń. Bieżąca logika używa identyfikatora MPN skojarzonego z rozwiązaniem, aby skierować wszystkie przychodzące skierowania od sprzedawców firmy Microsoft niezależnie od kraju klienta. Są one dostępne do twojej dyspozycji i **można je zaimportować jednym kliknięciem** jako reguły routingu. Po zakończeniu akcji importowania reguły zostaną zastosowane do wszystkich nowych poleceń wysyłanych przez sprzedawców firmy Microsoft. Firma może edytować lub usuwać istniejące reguły i w razie potrzeby tworzyć nowe reguły. Tylko [**administrator poleceń**](permissions-overview.md#manage-referrals) z zakresem globalnym może importować reguły. To samo uprawnienie jest wymagane w przypadku kolejnych zmian w zasadach routingu.

> [!IMPORTANT]
> **Istnieją zmiany logiki powiadomień e-mail.** Po zaimportowaniu reguł wiadomości e-mail, które zostały  wcześniej wysłane do kontaktów rozwiązania przekazanych na karcie Kolokcja na platformie handlowej, nie będą już wysyłane. **Tylko [administratorzy poleceń](permissions-overview.md#manage-referrals)** z lokalizacji MPN, do której jest wysyłana szansa sprzedaży, zostaną powiadomieni.

## <a name="override-rules"></a>Przesłoń reguły

Można zastąpić dwa typy reguł i zastąpić określony warunek reguły domyślnej. W domyślną regułę można zmienić tylko lokalizację MPN, do której mają być kierowane polecenia. Pozostałe dwa typy reguł, które  można zastąpić, to te z wszystkimi rozwiązaniami i wszystkimi rynkami **jako** warunkami w regułach.

**Przesłonięcie** wszystkich rynków — przy założeniu, że utworzono regułę, która mówi, że dla wszystkich rynków klienta i danego rozwiązania A należy skierować polecenia do lokalizacji MPN M1. Taką regułę można przesłonić za pomocą określonego rynku i tej samej kombinacji rozwiązań. Przykładowe przesłonięcie może być "w przypadku poleceń zawierających klientów z rynku United Kingdom i rozwiązania A, przekieruj je do lokalizacji MPN M2.

**Wszystkie rozwiązania zastępują** — przy założeniu, że utworzono regułę, która mówi, że dla wszystkich rozwiązań i danego rynku MKT1 skierować polecenia do lokalizacji MPN M1. Taką regułę można zastąpić konkretnym rozwiązaniem i taką samą kombinacją rynku. Przykładowe przesłonięcie może być "w przypadku poleceń zawierających klientów z rynku MKT1 i rozwiązania B, przekieruj je do lokalizacji MPN M2.

W poniższej tabeli przedstawiono podsumowanie typów rozwiązań, które można zastąpić

| **Typ** | **Czy można przesłonić ?** |
|-------|-------|
|Domyślne| Nie |
|Wszystkie rynki| Tak|
|Wszystkie rozwiązania| Tak|
|Określone rozwiązania i określone kombinacje rynku| Nie|

> [!Note]
> Lokalizację MPN dla reguły domyślnej można zmienić, mimo że nie można zmienić niczego innego w tej regułie.

## <a name="rules-evaluation"></a>Ocena reguł

Jeśli twoja firma ma wiele reguł, które można zastosować do scenariusza, poniżej użytych kryteriów oceny.

- Pierwszym sprawdzeniem będzie reguła z określonym rozwiązaniem i kombinacją rynku, które znajdują się w szansie sprzedaży dla ruchu przychodzącego. Bezpośrednie dopasowanie do każdej takiej reguły będzie mieć pierwszeństwo przed wszystkimi innymi regułami.
- Jeśli pierwsze sprawdzenie zakończy się niepowodzeniem, sprawdzimy, czy istnieją reguły zawierające rozwiązanie wymienione w poleceniu z warunkiem rynku ustawionym jako wszystkie rynki.
- Jeśli drugie sprawdzenie zakończy się niepowodzeniem, sprawdzimy, czy istnieją reguły, w których wszystkie rozwiązania są wymienione jako kryteria rozwiązania dla określonego rynku.
- Jeśli trzecie sprawdzenie również zakończy się niepowodzeniem, użyjemy reguły domyślnej.

> [!Note]
> Nie można utworzyć reguły, która powoduje konflikt z innymi regułami w określonej lokalizacji i na poziomie rozwiązania. W przypadku próby utworzenia reguły powodującej konflikt interfejs użytkownika zrzuci błąd z nazwą reguły, która jest w konflikcie z konfiguracją.

## <a name="example"></a>Przykład

Reguły routingu dla ruchu przychodzącego zostaną wyjaśnione przy użyciu reguł routingu utworzonych dla firmy Contoso Corporation. Zanim zrozumiemy, jak będą stosowane reguły, poznajmy hierarchię MPN i konfigurowanie użytkowników w firmie Contoso Corporation.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>Hierarchia MPN firmy Contoso Corporation

| **Identyfikator MPN** | **Typ** | **Adres** |
|-------|-------|-------|
|999999| Globalnie| One Contoso way, **Redmond, Stany Zjednoczone of America**|
|555555| Lokalizacja| One Contoso way, **Londyn, Zjednoczone Królestwo**|
|666666| Lokalizacja| One Contoso way, **Singapur, Singapur**|
|777777| Lokalizacja| One Contoso way, **Douru, India**|

#### <a name="sellers-from-contoso-corporation"></a>Sprzedawcy z firmy Contoso Corporation

Poniżej znajdują się sprzedawcy z odpowiednimi rolami poleceń i zakresem w firmie Contoso Corporation.

| **Nazwa** | **Role** | **Zakres** |
|-------|-------|-------|
|Seller One|Administrator poleceń|Cała organizacja|
|Sprzedawca 2|Administrator poleceń|Bengaluru|
|Sprzedawca trzy|Użytkownik poleceń|Londyn|
|Sprzedawca czwarty|Użytkownik poleceń|Singapur|

#### <a name="inbound-routing-rules-for-contoso-corporation"></a>Reguły routingu dla ruchu przychodzącego dla firmy Contoso Corporation

Załóżmy, że poniższy zestaw reguł został utworzony przez sprzedawcę 1 dla firmy Contoso Corporation. Te **reguły mogą tworzyć** tylko sprzedawcy, ponieważ do tworzenia i edytowania reguł wymagany jest administrator poleceń w całym zakresie organizacji. [](permissions-overview.md#manage-referrals)

| **Rynków** | **Rozwiązania** | **Lokalizacja MPN** | **Nazwa reguły routingu** |
|-------|-------|-------|-------|
|Wszystkie rynki|Wszystkie rozwiązania|Redmond|Domyślne|
|Zjednoczone Królestwo|Wszystkie rozwiązania|Londyn|Wszystkie rozwiązania w Zjednoczonym Królestwie|
|Wszystkie rynki|Sol-ABC|Singapur|Sol-ABC — wszystkie rynki|
|Indie|Sol-PQR|Bengaluru|Indie Sol-PQR|

#### <a name="summary-of-routing-for-various-scenarios-based-on-the-rules-for-contoso-corporation"></a>Podsumowanie routingu dla różnych scenariuszy na podstawie reguł dla firmy Contoso Corporation

| **Nie** | **Scenariusz** | **Rynek klientów** | **Dołączone rozwiązania** |**Zastosowana reguła routingu** |**Przypisanie MPN** |**Dostęp do poleceń** |
|-----|----------|-------|-------|-------|-------|-----------|
| 1|Brak dopasowania konkretnego rozwiązania i reguły rynku|Zjednoczone Królestwo|SOL-PQR|Globalnie|999999| Seller One, Seller Two, Seller Three (Sprzedawca trzeci, jeśli został dodany do zespołu), Seller Four (jeśli został dodany do zespołu)|
| 2|Wszystkie rozwiązania i określone reguły rynku są zgodne|Zjednoczone Królestwo|SOL-PQR|Wszystkie rozwiązania w Zjednoczonym Królestwie|555555| Seller One, Seller Three (Sprzedawca trzeci) (jeśli został dodany do zespołu) |
| 3|Określone rozwiązanie i dopasowanie reguły wszystkich rynków|Nigeria|SOL-ABC|SOL-ABC — wszystkie rynki|666666| Seller One, Seller Four (Sprzedawca czwarty) (jeśli został dodany do zespołu) |
| 4|Dopasowanie konkretnego rozwiązania i reguły rynku|Indie|SOL-PQR|Indie Sol-PQR|777777| Seller One, Seller Two|
| 5|Polecenie przychodzące z rozwiązaniem, które nie należy do Twojej firmy|Stany Zjednoczone Ameryki|SOL-XYZ|Globalnie|999999| Seller One, Seller Two, Seller Three (Sprzedawca trzeci, jeśli został dodany do zespołu), Seller Four (jeśli został dodany do zespołu)|

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie możliwościami współpracy sprzedaży](manage-co-sell-opportunities.md)

- [Uzyskiwanie łącznika do współpracy sprzedaży dla usługi Dynamics 365 CRM](connector-dynamics.md)

- [Uzyskiwanie łącznika do współsprzedaży dla rozwiązania Salesforce CRM](connector-salesforce.md)
