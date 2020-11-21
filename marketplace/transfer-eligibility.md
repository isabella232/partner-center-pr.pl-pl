---
title: Uprawnienie do transferu — wskazówki dotyczące przenoszenia subskrypcji między kontami rozliczeniowymi, Azure Marketplace
description: Wskazówki dotyczące kontroli komercyjnej przed przeniesieniem subskrypcji między kontami rozliczeń w Azure Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007533"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="5b217-103">Przenoszenie uprawnień do subskrypcji między kontami rozliczeniowymi</span><span class="sxs-lookup"><span data-stu-id="5b217-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="5b217-104">[Subskrypcję można przenieść](/azure/cost-management-billing/understand/subscription-transfer) z jednego konta rozliczeniowego do innego w sekcji Rozliczenia w Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="5b217-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="5b217-105">Przed przeniesieniem subskrypcja jest skanowana pod kątem produktów innych firm.</span><span class="sxs-lookup"><span data-stu-id="5b217-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="5b217-106">Transfer jest dozwolony tylko wtedy, gdy *wszystkie* produkty są wyczyszczone do przeniesienia (patrz poniższe [kryteria](#criteria-for-transfer-approval-or-denial) ).</span><span class="sxs-lookup"><span data-stu-id="5b217-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="5b217-107">System wygeneruje odpowiednie komunikaty o błędach dla aplikacji, które nie zostały wyczyszczone, aby pomóc w ustaleniu następnych kroków.</span><span class="sxs-lookup"><span data-stu-id="5b217-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="5b217-108">Ten artykuł nie dotyczy ofert SaaS, ponieważ zasoby SaaS są dołączone do dzierżawy, a nie do subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="5b217-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="5b217-109">Zasoby SaaS są przenoszone z jednego konta rozliczeniowego do innego, ale jest to wykonywane dla każdego zasobu i pomocy technicznej platformy Azure jako żądania pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="5b217-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="5b217-110">Kryteria zatwierdzania transferu lub odmowy</span><span class="sxs-lookup"><span data-stu-id="5b217-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="5b217-111">Nie można przenieść subskrypcji, Jeśli którakolwiek z jej aplikacji innych firm spełnia następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="5b217-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="5b217-112">Konto docelowe jest komercyjne, a aplikacja jest niedostępna do sprzedaży przez partnerów.</span><span class="sxs-lookup"><span data-stu-id="5b217-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="5b217-113">Aplikacja jest opcjonalna dla wybranych partnerów, a konto docelowe nie znajduje się na liście dozwolonych.</span><span class="sxs-lookup"><span data-stu-id="5b217-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="5b217-114">Oferta była ofertą wersji zapoznawczej w przeszłości dla wybranych subskrypcji lub była ofertą prywatną, a subskrypcja nie znajduje się już na liście dozwolonych.</span><span class="sxs-lookup"><span data-stu-id="5b217-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="5b217-115">Nowe konto rozliczeniowe znajduje się w regionie innym niż miejsce sprzedaży oferty i oferta nie jest sprzedawana w tym regionie.</span><span class="sxs-lookup"><span data-stu-id="5b217-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="5b217-116">Zablokowany transfer nadal obowiązuje do momentu usunięcia zasobu z subskrypcji, po upływie którego można ponowić próbę przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="5b217-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5b217-117">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="5b217-117">Next steps</span></span>

[<span data-ttu-id="5b217-118">Uzyskaj pomoc techniczną dla Microsoft AppSource i witryny Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="5b217-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

