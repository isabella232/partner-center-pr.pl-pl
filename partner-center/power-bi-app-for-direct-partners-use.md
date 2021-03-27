---
title: Korzystanie z usługi Partner Center Analytics na potrzeby Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak wyświetlać dane biznesowe za pomocą aplikacji analizy Centrum partnerskiego dla Power BI (dla partnerów bezpośrednich w dostawcy CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633866"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="ce947-103">Wyświetl dane biznesowe za pomocą aplikacji analizy Centrum partnerskiego dla firmy Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="ce947-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="ce947-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="ce947-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ce947-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="ce947-105">Global admin</span></span>
- <span data-ttu-id="ce947-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="ce947-106">User management admin</span></span>
- <span data-ttu-id="ce947-107">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="ce947-107">Sales agent</span></span>
- <span data-ttu-id="ce947-108">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="ce947-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="ce947-109">Wyświetlanie danych firmy</span><span class="sxs-lookup"><span data-stu-id="ce947-109">View your business data</span></span>

<span data-ttu-id="ce947-110">Uzyskaj wizualną reprezentację danych biznesowych za pomocą aplikacji do analizy Centrum partnerskiego dla Power BI, w tym:</span><span class="sxs-lookup"><span data-stu-id="ce947-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="ce947-111">Rozwój bazy klientów, subskrypcji i licencji</span><span class="sxs-lookup"><span data-stu-id="ce947-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="ce947-112">Użycie pakietu Office 365, Microsoft Dynamics i produktów Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ce947-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="ce947-113">Dzienne jednostki zużycia dla każdego zmierzonego zasobu w każdej subskrypcji platformy Azure w ciągu ostatnich 60 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="ce947-114">Szacowany koszt (na podstawie karty z najnowszą stawką)</span><span class="sxs-lookup"><span data-stu-id="ce947-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="ce947-115">Możliwość eksportowania zestawów danych i tworzenia niestandardowych raportów, w tym na klientach.</span><span class="sxs-lookup"><span data-stu-id="ce947-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="ce947-116">Informacje o wersji zapoznawczej aplikacji Centrum partnerskiego</span><span class="sxs-lookup"><span data-stu-id="ce947-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="ce947-117">Ta aplikacja jest tylko dla partnerów bezpośrednich w programie dostawcy rozwiązań w chmurze.</span><span class="sxs-lookup"><span data-stu-id="ce947-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="ce947-118">Inni partnerzy w programie CSP (na przykład pośrednim odsprzedawcy) nie będą mogli się zalogować.</span><span class="sxs-lookup"><span data-stu-id="ce947-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="ce947-119">Wszystkie szacowane koszty to dane dotyczące rozliczeń i fakturowania przed opodatkowaniem i nie są prawnie wiążące.</span><span class="sxs-lookup"><span data-stu-id="ce947-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="ce947-120">Szacowane koszty są przeznaczone do użycia tylko na potrzeby wglądu w dane.</span><span class="sxs-lookup"><span data-stu-id="ce947-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="ce947-121">Informacje o klientach są oparte na subskrypcjach.</span><span class="sxs-lookup"><span data-stu-id="ce947-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="ce947-122">Wszyscy klienci, dla których utworzono ostatnio konta, ale którzy nie mają jeszcze subskrypcji, nie są włączeni do liczenia.</span><span class="sxs-lookup"><span data-stu-id="ce947-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="ce947-123">Szacowany koszt jest oparty na karcie z najnowszą stawką, która jest oparta na cenach dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="ce947-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="ce947-124">Liczba dni to dni kalendarzowe.</span><span class="sxs-lookup"><span data-stu-id="ce947-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="ce947-125">Raport dotyczący usługi Business Insights</span><span class="sxs-lookup"><span data-stu-id="ce947-125">Business Insights report</span></span>

- <span data-ttu-id="ce947-126">**Dzierżawy klientów**: liczba różnych dzierżaw usługi Azure AD klientów, którzy kupili subskrypcje</span><span class="sxs-lookup"><span data-stu-id="ce947-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="ce947-127">**Nowe (ostatnie 30 dni)**: nowi klienci kupują co najmniej jedną subskrypcję w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="ce947-128">Zmiany **(ostatnie 30 dni)**: klienci bez żadnej "aktywne", "z wyprzedzeniem" lub "wyłączone"</span><span class="sxs-lookup"><span data-stu-id="ce947-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="ce947-129">**Nowość (ostatnie 24 godziny)**: nowi klienci kupują co najmniej jedną subskrypcję w ciągu ostatnich 24 godzin</span><span class="sxs-lookup"><span data-stu-id="ce947-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="ce947-130">**Szacowany miesięczny koszt w ciągu ostatnich 12 miesięcy**: trend między miesiącami w przypadku szacowanej kwoty dolara za faktury przed opodatkowaniem, zagregowany miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="ce947-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ce947-131">**Szacowany koszt według produktu w ciągu ostatnich 12 miesięcy**: produkty sprzedane według szacowanej kwoty dolara faktury przed opodatkowaniem zagregowanej w okresie ostatnich 12 miesięcy.</span><span class="sxs-lookup"><span data-stu-id="ce947-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="ce947-132">Ten stan wskazuje na Najpopularniejsze produkty z największą ilością przychodów.</span><span class="sxs-lookup"><span data-stu-id="ce947-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="ce947-133">**Klienci w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych klientów i zmiany klientów zagregowanych miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="ce947-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ce947-134">**Szacowany koszt przez klienta w ciągu ostatnich 12 miesięcy**: klienci posortowani według szacowanej kwoty dolara za faktury przed opodatkowaniem w okresie ostatnich 12 miesięcy.</span><span class="sxs-lookup"><span data-stu-id="ce947-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="ce947-135">Ten stan oznacza, że klienci najczęściej mają najwięcej przychodów.</span><span class="sxs-lookup"><span data-stu-id="ce947-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="ce947-136">**Liczba klientów według produktu**: produkty sprzedawane posortowane przez skojarzonych klientów.</span><span class="sxs-lookup"><span data-stu-id="ce947-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="ce947-137">Ten stan wskazuje Najpopularniejsze produkty sprzedawane większości klientów.</span><span class="sxs-lookup"><span data-stu-id="ce947-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="ce947-138">Raport usługi Subscription Insights</span><span class="sxs-lookup"><span data-stu-id="ce947-138">Subscription Insights report</span></span>

- <span data-ttu-id="ce947-139">**Stan subskrypcji**:</span><span class="sxs-lookup"><span data-stu-id="ce947-139">**Subscription status**:</span></span>

- <span data-ttu-id="ce947-140">Aktywne: subskrypcje należące do "Active" lub "w stanie prolongaty"</span><span class="sxs-lookup"><span data-stu-id="ce947-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="ce947-141">Zawieszone: subskrypcje należące do stanu "wyłączone"</span><span class="sxs-lookup"><span data-stu-id="ce947-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="ce947-142">Cofnięto Inicjowanie obsługi: subskrypcje należące do stanu "de-provisioned" lub "wygasłe"</span><span class="sxs-lookup"><span data-stu-id="ce947-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="ce947-143">**Stan wygaśnięcia**:</span><span class="sxs-lookup"><span data-stu-id="ce947-143">**Expiry status**:</span></span>

  - <span data-ttu-id="ce947-144">Wygasłe: subskrypcje, które już wygasły (Data zakończenia subskrypcji przypada w przeszłości)</span><span class="sxs-lookup"><span data-stu-id="ce947-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="ce947-145">Wygasa po 30 dniach: subskrypcje wygaśnie po upływie 30 dni (w przypadku których data zakończenia subskrypcji będzie późniejsza niż 30 dni)</span><span class="sxs-lookup"><span data-stu-id="ce947-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="ce947-146">Wygasa za 30 dni: subskrypcje wygaśnie w ciągu następnych 30 dni (w przypadku których data zakończenia subskrypcji przypada między dzisiaj a 30 dni)</span><span class="sxs-lookup"><span data-stu-id="ce947-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="ce947-147">**Łączna liczba subskrypcji**: subskrypcje w "aktywny," "w stanie prolongaty" lub "wyłączone"</span><span class="sxs-lookup"><span data-stu-id="ce947-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="ce947-148">**Nowe (ostatnie 30 dni)**: nowe subskrypcje zakupione przez klientów w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="ce947-149">**Nowość (ostatnie 24 godziny)**: nowe subskrypcje zakupione przez klientów w ciągu ostatnich 24 godzin</span><span class="sxs-lookup"><span data-stu-id="ce947-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="ce947-150">**Wygaśnięcie za 30 dni**: subskrypcje wygaśnie w ciągu następnych 30 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="ce947-151">Zmiany **(ostatnie 30 dni)**: subskrypcje, które zostały cofnięte lub zawieszone (wyłączone) w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="ce947-152">**Dystrybucja według typów subskrypcji**:% dystrybucji łącznej liczby subskrypcji według typu subskrypcji opartej na licencji i użycia</span><span class="sxs-lookup"><span data-stu-id="ce947-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="ce947-153">**Liczba aktywnych subskrypcji według produktu**: produkty sprzedane według liczby aktywnych subskrypcji</span><span class="sxs-lookup"><span data-stu-id="ce947-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="ce947-154">**Subskrypcje w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych subskrypcji i subskrypcji zmian zagregowanych miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="ce947-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ce947-155">**Szczegóły subskrypcji klienta**: szczegółowy widok klientów, subskrypcji i ofert</span><span class="sxs-lookup"><span data-stu-id="ce947-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="ce947-156">Raport dotyczący informacji o licencji:</span><span class="sxs-lookup"><span data-stu-id="ce947-156">License Insights report:</span></span>

- <span data-ttu-id="ce947-157">**Łączna liczba licencji**: łączną liczbę licencji agregowanych w ramach wszystkich subskrypcji opartych na licencji</span><span class="sxs-lookup"><span data-stu-id="ce947-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="ce947-158">**Nowe (ostatnie 30 dni)**: Dodanie licencji w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="ce947-159">Zmiany **(ostatnie 30 dni)**: redukcja licencji w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="ce947-160">**Nowość (ostatnie 24 godziny)**: Dodanie licencji w ciągu ostatnich 24 godzin</span><span class="sxs-lookup"><span data-stu-id="ce947-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="ce947-161">**Licencje w ciągu ostatnich 90 dni**: trend w miesiącu, w którym liczba dodatkowych licencji i obniżki są agregowane miesięcznie w okresie ostatnich 90 dni</span><span class="sxs-lookup"><span data-stu-id="ce947-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="ce947-162">**Liczba aktywnych licencji według produktu**: produkty sprzedawane posortowane według liczby aktywnych licencji</span><span class="sxs-lookup"><span data-stu-id="ce947-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="ce947-163">**Liczba aktywnych licencji według klientów**: posortowane według liczby aktywnych licencji</span><span class="sxs-lookup"><span data-stu-id="ce947-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="ce947-164">**Szczegóły zdarzenia licencji klienta w ciągu ostatnich 90 dni**: szczegółowy widok klientów, subskrypcji i zdarzeń subskrypcji, w tym data, nazwa zdarzenia, ilość i zmiana ilości.</span><span class="sxs-lookup"><span data-stu-id="ce947-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="ce947-165">Raport użycia licencji:</span><span class="sxs-lookup"><span data-stu-id="ce947-165">Licenses Usage report:</span></span>

- <span data-ttu-id="ce947-166">**Licencje przypisane przez produkt**: produkty sprzedane według liczby przypisań licencji</span><span class="sxs-lookup"><span data-stu-id="ce947-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="ce947-167">**Licencje używane przez produkt**: produkty sprzedawane posortowane według liczby użycia licencji</span><span class="sxs-lookup"><span data-stu-id="ce947-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="ce947-168">**Dystrybucja przez klienta przypisanych licencji**:% dystrybucji łącznej liczby klientów w przedziałach 20% zakresu przez przypisanie licencji%</span><span class="sxs-lookup"><span data-stu-id="ce947-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="ce947-169">**Dystrybucja przez klienta licencji w użyciu**:% dystrybucji łącznej liczby klientów w przedziale 20% zakresu według użycia licencji%</span><span class="sxs-lookup"><span data-stu-id="ce947-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="ce947-170">**Licencje przypisane przez klienta**: szczegółowy widok licencji sprzedanych i licencji przypisanych przez klientów i produkty</span><span class="sxs-lookup"><span data-stu-id="ce947-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="ce947-171">**Licencje używane przez klienta**: szczegółowy widok sprzedanych licencji i licencji używanych przez klientów i produkty</span><span class="sxs-lookup"><span data-stu-id="ce947-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="ce947-172">Raport usługi Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="ce947-172">Azure Insights report:</span></span>

- <span data-ttu-id="ce947-173">Klienci korzystający z **użycia w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych klientów opartych na użyciu i przetworzonych klientów korzystających z użycia zagregowanych miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="ce947-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ce947-174">**Subskrypcje oparte na użyciu w ciągu ostatnich 12 miesięcy**: trend między miesiącami dla nowych subskrypcji opartych na użyciu i przetworzonych subskrypcji opartych na użyciu zagregowanych miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="ce947-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="ce947-175">**Szacowany koszt użycia przez klienta w ciągu ostatnich 60 dni**: Klienci korzystający z użycia posortowani według szacowanej kwoty dolara za faktury przed opodatkowaniem w okresie ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="ce947-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="ce947-176">Ten stan oznacza, że klienci korzystający z większości klientów korzystający z większości przychodów</span><span class="sxs-lookup"><span data-stu-id="ce947-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="ce947-177">**Szacowany koszt użycia według kategorii w ciągu ostatnich 60 dni**: kategorie mierników subskrypcji opartych na użyciu sortowane według szacowanej kwoty dolara za faktury przed opodatkowaniem w okresie ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="ce947-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="ce947-178">**Szacowany koszt użycia według subskrypcji w ciągu ostatnich 60 dni**: subskrypcje oparte na użyciu przez szacowaną kwotę dolara za faktury przed opodatkowaniem zagregowaną w okresie ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="ce947-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="ce947-179">**Szacowany koszt użycia przez klienta według budżetu wydatków**: klienci posortowani według procentu bieżącego budżetu wydatków użycia przekraczają próg (100%).</span><span class="sxs-lookup"><span data-stu-id="ce947-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="ce947-180">Raport użycia zasobów platformy Azure:</span><span class="sxs-lookup"><span data-stu-id="ce947-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="ce947-181">**Użycie zasobów platformy Azure według dnia w wybranym okresie**: dzienne jednostki zużycia dla każdego zmierzonego zasobu w każdej subskrypcji opartej na użyciu dla wybranego okresu w ciągu ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="ce947-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="ce947-182">**Szacowany koszt użycia zasobów platformy Azure dla wybranego okresu**: szacowany koszt oparty na najnowszej stawce dla każdego zmierzonego zasobu w ramach każdej subskrypcji opartej na użyciu dla wybranego okresu w ciągu ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="ce947-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ce947-183">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="ce947-183">Next steps</span></span>

- [<span data-ttu-id="ce947-184">Omówienie usługi Partner Center Analytics dla Power BI aplikacji</span><span class="sxs-lookup"><span data-stu-id="ce947-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="ce947-185">Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="ce947-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
