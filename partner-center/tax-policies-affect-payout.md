---
title: Jak zasady podatkowe wpływają na wypłatę w portalu Azure Marketplace
description: Dowiedz się, jak zasady podatkowe wpływają na wypłatę w portalu Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768826"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="10e9a-103">Jak zasady podatkowe wpływają na wypłatę w portalu Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="10e9a-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="10e9a-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="10e9a-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="10e9a-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="10e9a-105">Global admin</span></span>
-    <span data-ttu-id="10e9a-106">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="10e9a-106">User management admin</span></span>
-    <span data-ttu-id="10e9a-107">Agent administracyjny</span><span class="sxs-lookup"><span data-stu-id="10e9a-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="10e9a-108">Wprowadzenie</span><span class="sxs-lookup"><span data-stu-id="10e9a-108">Introduction</span></span>

<span data-ttu-id="10e9a-109">Komercyjny Portal firmy Microsoft ma globalne zasięg.</span><span class="sxs-lookup"><span data-stu-id="10e9a-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="10e9a-110">Transakcje odbywają się w różnych granicach i w zależności od tego, gdzie znajdują się niezależnego dostawcy oprogramowania i klienta, implikacje podatkowe mogą się różnić.</span><span class="sxs-lookup"><span data-stu-id="10e9a-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="10e9a-111">Microsoft AppSource i Portal Azure Marketplace używają informacji o profilu podatkowym Centrum partnerskiego, aby określić kraj niezależnego dostawcy oprogramowania.</span><span class="sxs-lookup"><span data-stu-id="10e9a-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="10e9a-112">Aby określić kraj klienta, użyj informacji rozliczeniowych klienta lub, jeśli klient znajduje się w Unii Europejskiej, korzystamy z dwóch różnych informacji.</span><span class="sxs-lookup"><span data-stu-id="10e9a-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="10e9a-113">Aby lepiej zrozumieć poniższe scenariusze, zapoznaj się z tabelą [szczegóły podatku](tax-details-marketplace.md) , która pokazuje, czy firma Microsoft zbiera i płaci podatki w imieniu wydawcy, czy też odpowiedzialność należy do wydawcy.</span><span class="sxs-lookup"><span data-stu-id="10e9a-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="10e9a-114">Wszystkie przykłady wartości sprzedaży i procenty podatku w tym temacie są przeznaczone tylko do celów informacyjnych.</span><span class="sxs-lookup"><span data-stu-id="10e9a-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="10e9a-115">Transakcje transakcyjne wydawcy w kraju podatków zarządzanym przez firmę Microsoft</span><span class="sxs-lookup"><span data-stu-id="10e9a-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="10e9a-116">**Scenariusz A** — transakcje, które odbywają się między wydawcą a klientem w [kraju podatków zarządzanym przez firmę Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="10e9a-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="10e9a-117">W tych transakcjach w momencie sprzedaży zostanie dodany podatek, a firma Microsoft wyśle ten podatek do odpowiedniego kraju.</span><span class="sxs-lookup"><span data-stu-id="10e9a-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="10e9a-118">Nie są potrącane żadne podatki z tytułu wypłaty i opłaty za wypłaty są na wyłączność.</span><span class="sxs-lookup"><span data-stu-id="10e9a-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="10e9a-119">Zapoznaj się z [scenariuszem D](#foreign-publisher-transacts-with-us-customer) w przypadku transakcji między wydawcy spoza USA a klientem USA.</span><span class="sxs-lookup"><span data-stu-id="10e9a-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Pokazuje przepływ pracy dla scenariusza procesu wypłaty A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="10e9a-121">Operacje transakcyjne wydawcy w kraju podatków zarządzanym przez firmę Microsoft, w którym opłata za witrynę Marketplace to usługa opodatkowana</span><span class="sxs-lookup"><span data-stu-id="10e9a-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="10e9a-122">**Scenariusz B** — transakcje, które odbywają się między wydawcą w Stanach Zjednoczonych (zgodnie z informacjami o profilu podatkowym Centrum partnerskiego) do klienta w kraju podatków zarządzanym przez firmę Microsoft, w którym kraj nakłada podatek od opłaty witryny Marketplace (usługa podlegająca opodatkowaniu).</span><span class="sxs-lookup"><span data-stu-id="10e9a-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="10e9a-123">W tym scenariuszu opłata za usługę magazynu jest odejmowana od wypłaty wydawcy.</span><span class="sxs-lookup"><span data-stu-id="10e9a-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="10e9a-125">Operacje transakcyjne wydawcy w kraju podatków zarządzanym przez program Publisher</span><span class="sxs-lookup"><span data-stu-id="10e9a-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="10e9a-126">**Scenariusz C** — transakcje, które odbywają się między wydawcą a klientem w kraju podatków zarządzanym przez wydawcę, które nie nakładają potrąconej zaliczki na podatek dla klientów.</span><span class="sxs-lookup"><span data-stu-id="10e9a-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="10e9a-127">Klienci nie będą obciążani podatkiem w momencie sprzedaży i są zobowiązani przez wydawcę, aby uregulować wszystkie stosowne podatki.</span><span class="sxs-lookup"><span data-stu-id="10e9a-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="10e9a-128">Aby uzyskać więcej informacji na temat cen specyficznych dla kraju (na przykład w celu przesunięcia nadchodzącego opodatkowania) [, zobacz plany i cenniki dla ofert komercyjnych w portalu Marketplace](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="10e9a-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="10e9a-130">Obce transakcje wydawcy z klientem USA</span><span class="sxs-lookup"><span data-stu-id="10e9a-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="10e9a-131">**Scenariusz D** — wszyscy wydawcy zagraniczni (zgodnie z informacjami o profilu podatkowym w centrum partnerskim) w krajach bez Traktatu USA (patrz [scenariusz E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) w celu sprzedaży do klienta opartego na USA (zgodnie z definicją adresu konta klienta).</span><span class="sxs-lookup"><span data-stu-id="10e9a-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="10e9a-132">Rząd USA wymaga od firmy Microsoft potrącenia w imieniu wydawcy.</span><span class="sxs-lookup"><span data-stu-id="10e9a-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="10e9a-133">Podatek potrącony od wypłaty do wydawcy jest obliczany na podstawie ceny oferty.</span><span class="sxs-lookup"><span data-stu-id="10e9a-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="10e9a-135">Wydawca obcy z postanowieniami umowy Transacting z klientem USA</span><span class="sxs-lookup"><span data-stu-id="10e9a-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="10e9a-136">**Scenariusz E** — wszyscy wydawcy zagraniczni (zgodnie z informacjami o profilu podatkowym w centrum partnerskim) w krajach z Traktatem Stanów Zjednoczonych, którzy wprowadzają sprzedaż do klienta opartego na USA (zgodnie z definicją adresu konta klienta).</span><span class="sxs-lookup"><span data-stu-id="10e9a-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="10e9a-137">Administracja USA nie wymaga od firmy Microsoft powstrzymania podatku w imieniu wydawcy.</span><span class="sxs-lookup"><span data-stu-id="10e9a-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="10e9a-139">Wydawca obcy jest sprzedawany do klienta zarejestrowanego w Unii VAT w kraju zarządzanym przez firmę Microsoft (poza Irlandią)</span><span class="sxs-lookup"><span data-stu-id="10e9a-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="10e9a-140">**Scenariusz F** — wszystkie transakcje między wydawcami obcymi i klientami zarejestrowanymi w Unii VAT (poza Irlandią) w Microsoft-Managed kraju.</span><span class="sxs-lookup"><span data-stu-id="10e9a-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="10e9a-141">Klient nie uiszcza podatku od sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="10e9a-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="10e9a-143">Wydawca obcy jest sprzedawany do klienta zarejestrowanego w Unii VAT w kraju zarządzanym przez firmę Microsoft (w Irlandii)</span><span class="sxs-lookup"><span data-stu-id="10e9a-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="10e9a-144">**Scenariusz G** — wszystkie transakcje między wydawcami obcymi i klientami zarejestrowanymi w Unii VAT (w Irlandii) w Microsoft-Managed kraju.</span><span class="sxs-lookup"><span data-stu-id="10e9a-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="10e9a-145">Klient płaci irlandzki podatek VAT, a firma Microsoft płaci ten podatek dla Irlandii rządowego.</span><span class="sxs-lookup"><span data-stu-id="10e9a-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Pokazuje przepływ pracy dotyczący scenariusza procesu wypłaty G.":::

## <a name="next-steps"></a><span data-ttu-id="10e9a-147">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="10e9a-147">Next steps</span></span>

- [<span data-ttu-id="10e9a-148">Często zadawane pytania dotyczące programu Publisher</span><span class="sxs-lookup"><span data-stu-id="10e9a-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="10e9a-149">Instrukcje dotyczące tworzenia profilów płatności i podatków</span><span class="sxs-lookup"><span data-stu-id="10e9a-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)