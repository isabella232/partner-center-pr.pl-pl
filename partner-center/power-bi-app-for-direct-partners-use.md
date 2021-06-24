---
title: Używanie Partner Center Analytics na Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak wyświetlać dane biznesowe przy użyciu aplikacja statystyczna Centrum partnerskiego dla usługi Power BI (dla bezpośrednich partnerów w programie Dostawca rozwiązań w chmurze (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564985"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="c2eb2-103">Wyświetlanie danych biznesowych za pomocą aplikacji Partner Center Analytics dla firmy Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="c2eb2-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="c2eb2-104">**Odpowiednie role:** Administrator globalny | Administrator zarządzania użytkownikami | Agent sprzedaży | Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="c2eb2-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="c2eb2-105">Wyświetlanie danych biznesowych</span><span class="sxs-lookup"><span data-stu-id="c2eb2-105">View your business data</span></span>

<span data-ttu-id="c2eb2-106">Pobierz wizualną reprezentację danych biznesowych za pomocą aplikacji Partner Center Analytics dla usługi Microsoft Power BI, w tym:</span><span class="sxs-lookup"><span data-stu-id="c2eb2-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="c2eb2-107">Rozwój bazy klientów, subskrypcji i licencji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="c2eb2-108">Użycie usług Office 365, Microsoft Dynamics i Microsoft Azure produktów</span><span class="sxs-lookup"><span data-stu-id="c2eb2-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="c2eb2-109">Jednostki dziennego zużycia dla każdego zasobu taryfowego w każdej subskrypcji platformy Azure w ciągu ostatnich 60 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="c2eb2-110">Szacowany koszt (na podstawie najnowszej karty stawki)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="c2eb2-111">Możliwość eksportowania zestawów danych i tworzenia raportów niestandardowych, w tym niestandardowych dla niestandardowych klientów.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="c2eb2-112">Informacje o wersji zapoznawczej Partner Center Analytics</span><span class="sxs-lookup"><span data-stu-id="c2eb2-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="c2eb2-113">Ta aplikacja jest dostępna tylko dla bezpośrednich partnerów Dostawca rozwiązań w chmurze (CSP).</span><span class="sxs-lookup"><span data-stu-id="c2eb2-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="c2eb2-114">Inni partnerzy w programie CSP (na przykład odsprzedawcy pośredni) nie będą mogli się zalogować.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="c2eb2-115">Wszelkie szacowane koszty są danymi rozliczeń przed opodatkowaniem/fakturami i nie są prawnie związane.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="c2eb2-116">Szacowane koszty są przeznaczone tylko do wglądu w dane.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="c2eb2-117">Informacje o kliencie są oparte na subskrypcjach.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="c2eb2-118">Klienci, dla których ostatnio utworzono konta, ale którzy nie mają jeszcze subskrypcji, nie są uwzględniani w liczbach.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="c2eb2-119">Szacowany koszt jest oparty na najnowszej karcie stawki, która jest oparta na cenach CSP.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="c2eb2-120">Dni to dni kalendarzowe.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="c2eb2-121">Raport Business Insights</span><span class="sxs-lookup"><span data-stu-id="c2eb2-121">Business Insights report</span></span>

- <span data-ttu-id="c2eb2-122">**Dzierżawy klientów:** liczba różnych dzierżaw Azure Active Directory (Azure AD) klientów, którzy kupili subskrypcje</span><span class="sxs-lookup"><span data-stu-id="c2eb2-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="c2eb2-123">**Nowość (ostatnie 30 dni):** nowi klienci, którzy kupią co najmniej jedną subskrypcję w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="c2eb2-124">**Rezygnacja (ostatnie 30 dni)**: klienci bez żadnych subskrypcji "aktywnych", "w prolongacie" lub "wyłączonych"</span><span class="sxs-lookup"><span data-stu-id="c2eb2-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="c2eb2-125">**Nowość (ostatnie 24 godziny):** nowi klienci, którzy kupują co najmniej jedną subskrypcję w ciągu ostatnich 24 godzin</span><span class="sxs-lookup"><span data-stu-id="c2eb2-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="c2eb2-126">**Szacowany koszt miesięczny w** ciągu ostatnich 12 miesięcy: trend miesiąc do miesiąca szacowanej kwoty faktury przed opodatkowaniem zagregowanej miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="c2eb2-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c2eb2-127">**Szacowany koszt według produktu** w ciągu ostatnich 12 miesięcy: produkty sprzedawane posortowane według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w okresie ostatnich 12 miesięcy.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="c2eb2-128">Ten stan wskazuje, że najważniejsze produkty przynoszą największe przychody.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="c2eb2-129">**Klienci w ciągu ostatnich 12 miesięcy:** trend miesiąc do miesiąca nowych klientów i klientów z rezygnacjami agregowany miesięcznie w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="c2eb2-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c2eb2-130">**Szacowany koszt według klienta** w ciągu ostatnich 12 miesięcy: klienci posortowani według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w okresie ostatnich 12 miesięcy.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="c2eb2-131">Ten stan wskazuje, że najpowszechniejsi klienci przynoszą najwięcej przychodów.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="c2eb2-132">**Liczba klientów według produktu:** produkty sprzedane posortowane według skojarzonych klientów.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="c2eb2-133">Ten stan wskazuje najważniejsze produkty sprzedane większości klientów.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="c2eb2-134">Raport Szczegółowe informacje o subskrypcji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-134">Subscription Insights report</span></span>

- <span data-ttu-id="c2eb2-135">**Stan subskrypcji:**</span><span class="sxs-lookup"><span data-stu-id="c2eb2-135">**Subscription status**:</span></span>

- <span data-ttu-id="c2eb2-136">Aktywne: subskrypcje należące do stanu "aktywne" lub "w prolongacie"</span><span class="sxs-lookup"><span data-stu-id="c2eb2-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="c2eb2-137">Wstrzymane: subskrypcje należące do stanu "wyłączone"</span><span class="sxs-lookup"><span data-stu-id="c2eb2-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="c2eb2-138">Coprowizowane: subskrypcje należące do stanu "coprowizowana" lub "wygasła"</span><span class="sxs-lookup"><span data-stu-id="c2eb2-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="c2eb2-139">**Stan wygaśnięcia:**</span><span class="sxs-lookup"><span data-stu-id="c2eb2-139">**Expiry status**:</span></span>

  - <span data-ttu-id="c2eb2-140">Wygasłe: subskrypcje, które już wygasły (gdzie data zakończenia subskrypcji jest w przeszłości)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="c2eb2-141">Wygasanie po 30 dniach: subskrypcje, które wygasną po 30 dniach (gdzie data zakończenia subskrypcji to po następnych 30 dniach)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="c2eb2-142">Wygasanie w ciągu 30 dni: subskrypcje, które wygasną w ciągu następnych 30 dni (gdzie data zakończenia subskrypcji to od dnia dzisiejszego do następnych 30 dni)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="c2eb2-143">**Łączna liczba subskrypcji:** subskrypcje w stanie "aktywne", "w prolongacie" lub "wyłączone"</span><span class="sxs-lookup"><span data-stu-id="c2eb2-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="c2eb2-144">**Nowość (ostatnie 30 dni):** nowe subskrypcje zakupione przez klientów w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="c2eb2-145">**Nowość (ostatnie 24 godziny):** nowe subskrypcje zakupione przez klientów w ciągu ostatnich 24 godzin</span><span class="sxs-lookup"><span data-stu-id="c2eb2-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="c2eb2-146">**Wygasanie w ciągu 30 dni:** subskrypcje, które wygasną w ciągu następnych 30 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="c2eb2-147">**Rezygnacja (ostatnie 30 dni):** subskrypcje, które zostały anulowane lub wstrzymane (wyłączone) w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="c2eb2-148">**Dystrybucja według typów subskrypcji:** procent dystrybucji łącznej liczby subskrypcji według typu subskrypcji na podstawie licencji i na podstawie użycia</span><span class="sxs-lookup"><span data-stu-id="c2eb2-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="c2eb2-149">**Liczba aktywnych subskrypcji według produktu:** sprzedane produkty posortowane według liczby aktywnych subskrypcji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="c2eb2-150">**Subskrypcje w ciągu ostatnich 12** miesięcy: trend miesiąc do miesiąca nowych subskrypcji i subskrypcji rezygnacji zagregowanych co miesiąc w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="c2eb2-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c2eb2-151">**Szczegóły subskrypcji klienta:** szczegółowy widok klientów, subskrypcji i ofert</span><span class="sxs-lookup"><span data-stu-id="c2eb2-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="c2eb2-152">Raport License Insights:</span><span class="sxs-lookup"><span data-stu-id="c2eb2-152">License Insights report:</span></span>

- <span data-ttu-id="c2eb2-153">**Łączna liczba licencji:** łączna liczba licencji zagregowana we wszystkich subskrypcjach opartych na licencjach</span><span class="sxs-lookup"><span data-stu-id="c2eb2-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="c2eb2-154">**Nowość (ostatnie 30 dni):** dodawanie licencji w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="c2eb2-155">**Rezygnacja (ostatnie 30 dni):** zmniejszenie liczby licencji w ciągu ostatnich 30 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="c2eb2-156">**Nowość (ostatnie 24 godziny):** dodawanie licencji w ciągu ostatnich 24 godzin</span><span class="sxs-lookup"><span data-stu-id="c2eb2-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="c2eb2-157">**Licencje w ciągu ostatnich 90 dni:** trend dodatku i redukcji licencji z miesiąca na miesiąc zagregowany co miesiąc w okresie ostatnich 90 dni</span><span class="sxs-lookup"><span data-stu-id="c2eb2-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="c2eb2-158">**Liczba aktywnych licencji według produktu:** sprzedane produkty posortowane według liczby aktywnych licencji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="c2eb2-159">**Liczba aktywnych licencji według klienta:** klienci posortowani według liczby aktywnych licencji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="c2eb2-160">Szczegóły zdarzeń licencji klienta z ostatnich **90** dni: szczegółowy widok klientów, subskrypcji i zdarzeń subskrypcji, w tym daty zdarzenia, nazwy zdarzenia, ilości i zmiany ilości.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="c2eb2-161">Raport użycia licencji:</span><span class="sxs-lookup"><span data-stu-id="c2eb2-161">Licenses Usage report:</span></span>

- <span data-ttu-id="c2eb2-162">**Licencje przypisane według produktu:** produkty sprzedane posortowane według liczby przypisań licencji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="c2eb2-163">**Licencje w użyciu według produktu:** produkty sprzedane posortowane według liczby użycia licencji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="c2eb2-164">**Rozkład przypisanych licencji** przez klientów: procent rozkładu całkowitej liczby klientów uszkodzonych w zasobnikach o zakresie 20% według przypisania licencji %</span><span class="sxs-lookup"><span data-stu-id="c2eb2-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="c2eb2-165">**Rozkład klientów licencji w** użyciu: procent rozkładu całkowitej liczby klientów uszkodzonych w zasobnikach o zakresie 20% według % użycia licencji</span><span class="sxs-lookup"><span data-stu-id="c2eb2-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="c2eb2-166">**Licencje przypisane przez klienta:** szczegółowy widok sprzedanych licencji i licencji przypisanych przez klientów i produkty</span><span class="sxs-lookup"><span data-stu-id="c2eb2-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="c2eb2-167">**Licencje w użyciu przez klienta:** szczegółowy widok sprzedanych licencji i licencji w użyciu przez klientów i produkty</span><span class="sxs-lookup"><span data-stu-id="c2eb2-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="c2eb2-168">Raport usługi Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="c2eb2-168">Azure Insights report:</span></span>

- <span data-ttu-id="c2eb2-169">Klienci na podstawie użycia w ciągu ostatnich **12** miesięcy: trend z miesiąca na miesiąc nowych klientów opartych na użyciu i klientów opartych na użyciu z rezygnacjami zagregowanych co miesiąc w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="c2eb2-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c2eb2-170">**Subskrypcje oparte na** użyciu w ciągu ostatnich 12 miesięcy: trend miesiąc po miesiącu nowych subskrypcji opartych na użyciu i subskrypcji opartych na użyciu, które są agregowane co miesiąc w okresie ostatnich 12 miesięcy</span><span class="sxs-lookup"><span data-stu-id="c2eb2-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c2eb2-171">Szacowany koszt użycia według klienta w ciągu ostatnich **60** dni: Klienci na podstawie użycia posortowani według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w ciągu ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="c2eb2-172">Ten stan wskazuje, że najpowszechniejsi klienci na podstawie użycia przynoszą najwięcej przychodów</span><span class="sxs-lookup"><span data-stu-id="c2eb2-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="c2eb2-173">Szacowany koszt użycia według kategorii w ciągu ostatnich **60** dni: kategorie mierników subskrypcji opartych na użyciu posortowane według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w okresie ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="c2eb2-174">**Szacowany koszt użycia** według subskrypcji w ciągu ostatnich 60 dni: subskrypcje oparte na użyciu według szacowanej kwoty faktury przed opodatkowaniem zagregowanej w ciągu ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="c2eb2-175">**Szacowany koszt użycia przez klienta według budżetu wydatków:** Klienci posortowani według wartości procentowej bieżącego budżetu wydatków na użycie przekraczającego próg (100%).</span><span class="sxs-lookup"><span data-stu-id="c2eb2-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="c2eb2-176">Raport Użycia zasobów platformy Azure:</span><span class="sxs-lookup"><span data-stu-id="c2eb2-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="c2eb2-177">**Użycie zasobów platformy Azure według dnia dla** wybranego okresu: dzienne jednostki zużycia dla każdego mierzonego zasobu w każdej subskrypcji opartej na użyciu dla wybranego okresu w ciągu ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="c2eb2-178">**Szacowany koszt** użycia zasobów platformy Azure dla wybranego okresu: Szacowany koszt na podstawie najnowszej stawki karty dla każdego mierzonego zasobu w każdej subskrypcji opartej na użyciu dla wybranego okresu w ciągu ostatnich 60 dni.</span><span class="sxs-lookup"><span data-stu-id="c2eb2-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c2eb2-179">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="c2eb2-179">Next steps</span></span>

- [<span data-ttu-id="c2eb2-180">Partner Center Analytics for Power BI app overview (Omówienie usługi Partner Center Analytics for Power BI app)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="c2eb2-181">Instalowanie i wyświetlanie podglądu aplikacji statystycznej Centrum partnerskiego dla usługi Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="c2eb2-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
