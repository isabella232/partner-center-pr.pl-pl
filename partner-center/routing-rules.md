---
title: Tworzenie reguł routingu dla szans przychodzących i zarządzanie nimi
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Twoja firma może utworzyć reguły, aby zdecydować, jak są kierowane przychodzące możliwości sprzedaży od sprzedawców firmy Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959766"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Tworzenie reguł routingu dla szans przychodzących i zarządzanie nimi

**Odpowiednie role:** Administrator poleceń | Użytkownik poleceń

> [!IMPORTANT]
> **Tworzenie reguł routingu jest opcjonalne.** Jest to zalecane tylko w przypadku większych firm, które są obecni na całym świecie, lub jeśli firma ma złożoną hierarchię MPN, w której zarządzanie poleceniami ma być wykonywane na poziomie określonej lokalizacji w zależności od rynku i rozwiązań klientów.

## <a name="introduction"></a>Wprowadzenie

Funkcja opisana w tym dokumencie pomoże Twojej firmie w skonfigurowaniu reguł, które mogą pomóc w skierowaniu możliwości sprzedaży wysyłanych przez sprzedawców firmy Microsoft do wybranej lokalizacji MPN. Domyślnie polecenia od sprzedawcy firmy Microsoft są wysyłane do lokalizacji MPN skojarzonej z rozwiązaniem do współpracy sprzedaży uwzględnionym w szansie sprzedaży. Utworzone reguły rozsyłania ułatwiają firmie zastąpienie routingu domyślnego. Tylko [**administrator poleceń z**](permissions-overview.md#manage-referrals) całym zakresem organizacji może tworzyć i edytować reguły rozsyłania. Partnerzy z [**rolą użytkownika poleceń**](permissions-overview.md#manage-referrals) mogą tylko wyświetlać reguły rozsyłania, aby zrozumieć, jak polecenia są kierowane w firmie.

Reguły nie będą stosowane retrospektywnie. Wszystkie odwołania utworzone w przeszłości lub ze starszą konfiguracją reguły rozsyłania nie zostaną zaktualizowane. Wszelkie zmiany wprowadzone w zasadach są stosowane natychmiast.

Istnieją trzy główne pivoty dla każdej reguły.

- **Rynek klienta** — rynek, na którym znajduje się firma klienta

- **Rozwiązanie** — rozwiązania opublikowane przez Twoją firmę za pośrednictwem portalu OCP GTM lub platformy handlowej

- **Lokalizacja MPN** — lokalizacja MPN, do której ma być kierowane polecenie

Każdą regułę można przeczytać w ten sposób — w przypadku poleceń wysyłanych przez sprzedawców firmy Microsoft wraz z rozwiązaniami z mojej firmy przekieruj je do **tej lokalizacji MPN**

> [!Note]
> Reguły rozsyłania ruchu przychodzącego mają zastosowanie tylko w przypadku możliwości współpracy sprzedaży wysyłanych do Twojej firmy przez sprzedawców firmy Microsoft.

## <a name="navigation"></a>Nawigacja

Reguły rozsyłania można utworzyć na **karcie Polecenia** na **stronie Ustawienia** konta. Aby przejść do strony, wybierz ikonę ustawień obok ikony użytkownika w  prawym górnym rogu, a następnie wybierz kartę Polecenia w lewym panelu nawigacyjnym.

## <a name="initial-setup"></a>Konfiguracja początkowa

**Konfigurowanie reguł routingu nie jest obowiązkowe.** Jeśli firma zdecyduje się na użycie reguł rozsyłania w celu skorzystania z logiki routingu, możesz rozpocząć od zaimportowania domyślnych reguł, których system zarządzania odwołaniami używa do kierowania poleceń. Bieżąca logika używa identyfikatora MPN skojarzonego z rozwiązaniem do kierowania wszystkich przychodzących poleceń od sprzedawców firmy Microsoft niezależnie od kraju klienta. Są one dostępne do twojej dyspozycji i **można je zaimportować jednym kliknięciem** jako regułą rozsyłania. Po zakończeniu akcji importowania reguły będą stosowane do wszystkich nowych poleceń wysyłanych przez sprzedawców firmy Microsoft. Firma może edytować lub usuwać istniejące reguły i w razie potrzeby tworzyć nowe reguły. Reguły [**mogą importować**](permissions-overview.md#manage-referrals) tylko administratorzy poleceń z zakresem globalnym. To samo uprawnienie jest wymagane dla wszystkich kolejnych zmian w zasadach rozsyłania.

> [!IMPORTANT]
> **Istnieją zmiany w logice powiadomień e-mail.** Po zaimportowaniu reguł wiadomości e-mail, które zostały  wcześniej wysłane do kontaktów rozwiązania przekazanych na karcie Współpraca na platformie handlowej, nie będą już wysyłane. **Powiadomienia [będą dotyczyć](permissions-overview.md#manage-referrals)** tylko administratorów poleceń w lokalizacji MPN, do której jest wysyłana szansa sprzedaży.

## <a name="override-rules"></a>Przesłanianie reguł

Można zastąpić dwa typy reguł i zastąpić określony warunek reguły domyślnej. W domyślną regułę można zmienić tylko lokalizację MPN, do której mają być kierowane polecenia. Pozostałe dwa typy reguł, które można zastąpić, to te, które mają w regułach warunki **Wszystkie rozwiązania** i Wszystkie rynki. 

**Przesłonięcie** wszystkich rynków — przy założeniu, że utworzono regułę dla wszystkich rynków klientów i danego rozwiązania A, należy skierować polecenia do lokalizacji MPN M1. Taką regułę można zastąpić kombinacją określonego rynku i tego samego rozwiązania. Przykładowe przesłonięcie może być "w przypadku poleceń zawierających klientów z rynku Zjednoczone Królestwo i rozwiązania A, które należy skierować do lokalizacji MPN M2.

**Wszystkie rozwiązania zastępują** — przy założeniu, że utworzono regułę, która mówi dla wszystkich rozwiązań i danego rynku MKT1, przekieruj polecenia do lokalizacji MPN M1. Tę regułę można przesłonić za pomocą określonego rozwiązania i tej samej kombinacji rynku. Przykładowe przesłonięcie może być "dla poleceń zawierających klientów z rynku MKT1 i rozwiązania B, przekieruj je do lokalizacji MPN M2.

W poniższej tabeli przedstawiono podsumowanie typów rozwiązań, które można zastąpić

| **Typ** | **Czy można przesłonić ?** |
|-------|-------|
|Domyślne| Nie |
|Wszystkie rynki| Tak|
|Wszystkie rozwiązania| Tak|
|Określone rozwiązania i kombinacja określonych rynków| Nie|

> [!Note]
> Lokalizację MPN dla reguły domyślnej można zmienić, mimo że nie można zmienić niczego innego w tej regułie.

## <a name="rules-evaluation"></a>Ocena reguł

Jeśli firma ma wiele reguł, które można zastosować do scenariusza, poniżej kryteriów oceny.

- Pierwszym sprawdzeniem będzie reguła z określonym rozwiązaniem i kombinacją rynku, które znajdują się w szansie sprzedaży dla ruchu przychodzącego. Bezpośrednie dopasowanie do każdej takiej reguły będzie mieć pierwszeństwo przed wszystkimi innymi regułami.
- Jeśli pierwsze sprawdzenie zakończy się niepowodzeniem, sprawdzimy, czy istnieją reguły, które zawierają rozwiązanie wymienione w poleceniu z warunkiem rynku ustawionym jako wszystkie rynki.
- Jeśli drugie sprawdzenie zakończy się niepowodzeniem, sprawdzimy, czy istnieją reguły, w których wszystkie rozwiązania są wymienione jako kryteria rozwiązania dla określonego rynku.
- Jeśli trzecie sprawdzenie również zakończy się niepowodzeniem, użyjemy reguły domyślnej.

> [!Note]
> Nie można utworzyć reguły, która powoduje konflikt z innymi regułami w określonej lokalizacji i na poziomie rozwiązania. W przypadku próby utworzenia reguły powodującej konflikt interfejs użytkownika zwęci nazwę reguły, która jest w konflikcie z konfiguracją.

## <a name="example"></a>Przykład

Reguły routingu dla ruchu przychodzącego zostaną wyjaśnione za pomocą reguł rozsyłania utworzonych dla firmy Contoso Corporation. Przed zrozumieniem sposobu stosowania reguł należy poznać hierarchię MPN i konfigurowanie użytkowników w firmie Contoso Corporation.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>Hierarchia MPN firmy Contoso Corporation

| **Identyfikator MPN** | **Typ** | **Adres** |
|-------|-------|-------|
|999999| Globalnie| One Contoso way, **Redmond, Stany Zjednoczone of America**|
|555555| Lokalizacja| One Contoso way, **Londyn, Zjednoczone Królestwo**|
|666666| Lokalizacja| One Contoso way, **Singapur, Singapur**|
|777777| Lokalizacja| One Contoso way, **Douru, Indie**|

#### <a name="sellers-from-contoso-corporation"></a>Sprzedawcy z firmy Contoso Corporation

Poniżej znajdują się sprzedawcy z odpowiednimi rolami poleceń i zakresem w firmie Contoso Corporation.

| **Nazwa** | **Role** | **Zakres** |
|-------|-------|-------|
|Seller One|Administrator poleceń|Cała organizacja|
|Sprzedawca dwa|Administrator poleceń|Bengaluru|
|Sprzedawca trzeci|Użytkownik poleceń|Londyn|
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
