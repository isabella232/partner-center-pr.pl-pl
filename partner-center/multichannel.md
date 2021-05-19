---
title: Obsługa wielu kanałów dla klientów
description: W niektórych przypadkach klienci mogą chcieć zatrudnić Cię do aprowizować i obsługiwać subskrypcję kupioną w innym miejscu.
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bd0bb946c2f59f50c27aff58569d497bc21bf30b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146412"
---
# <a name="multi-channel-support---using-other-partners-to-support-customer-subscriptions-purchased-elsewhere"></a><span data-ttu-id="f339d-103">Obsługa wielu kanałów — używanie innych partnerów do obsługi subskrypcji klientów zakupionych w innym miejscu</span><span class="sxs-lookup"><span data-stu-id="f339d-103">Multi-channel support - using other partners to support customer subscriptions purchased elsewhere</span></span>

<span data-ttu-id="f339d-104">**Dotyczy:** Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f339d-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f339d-105">**Odpowiednie role:** Administrator globalny | Administrator zarządzający użytkownikami | Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="f339d-105">**Appropriate roles**: Global admin | User management admin | Sales agent</span></span>

<span data-ttu-id="f339d-106">Funkcja Partner Center obsługuje scenariusze, w których klient chce zatrudnić partnera do zarządzania subskrypcją kupioną w innym miejscu i obsługiwać ją.</span><span class="sxs-lookup"><span data-stu-id="f339d-106">The Partner Center's multi-channel feature supports scenarios when a customer wants to hire a partner to manage and support a subscription they purchased elsewhere.</span></span> <span data-ttu-id="f339d-107">Obsługa wielu kanałów ma zastosowanie, gdy klient:</span><span class="sxs-lookup"><span data-stu-id="f339d-107">Multi-channel support applies when the customer:</span></span>

- <span data-ttu-id="f339d-108">Już zakupione subskrypcje bezpośrednio od firmy Microsoft lub za pośrednictwem programów Advisor, Open lub EA.</span><span class="sxs-lookup"><span data-stu-id="f339d-108">Already purchased subscriptions directly from Microsoft or through the Advisor, Open, or EA programs.</span></span>

- <span data-ttu-id="f339d-109">Zakupiono subskrypcje od innej firmy, która nie jest Dostawca rozwiązań w chmurze programem firmy Microsoft lub nie jest partnerem syndykacji firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f339d-109">Purchased the subscriptions from a third party not in the Cloud Solution Provider program or not a Microsoft Syndication Partner.</span></span> <span data-ttu-id="f339d-110">Klienci nie mogą przełączyć istniejących subskrypcji opartych na licencjach na innego partnera w programie Dostawca rozwiązań w chmurze — muszą poczekać do końca okresu subskrypcji lub anulować przed przeniesieniem.</span><span class="sxs-lookup"><span data-stu-id="f339d-110">Customers can't switch existing license-based subscriptions to a different partner in the Cloud Solution Provider program-they must wait until the end of their subscription period or cancel before moving.</span></span>

|<span data-ttu-id="f339d-111">Aby obsługiwać te usługi</span><span class="sxs-lookup"><span data-stu-id="f339d-111">To support these services</span></span>  | <span data-ttu-id="f339d-112">W tym celu:</span><span class="sxs-lookup"><span data-stu-id="f339d-112">Do this:</span></span> |
|:---------|:---------|
|<span data-ttu-id="f339d-113">Usługi oparte na licencjach</span><span class="sxs-lookup"><span data-stu-id="f339d-113">License-based services</span></span>    | <span data-ttu-id="f339d-114">Aby zapewnić obsługę kont wielokanałowych, musisz poprosić klienta o uprawnienia do zarządzania subskrypcjami.</span><span class="sxs-lookup"><span data-stu-id="f339d-114">To provide support for multi-channel accounts, you must request permissions from the customer to manage their subscriptions.</span></span> <span data-ttu-id="f339d-115">Aby uzyskać więcej informacji, zobacz [Request a reseller relationship with a customer (Żądanie relacji odsprzedawcy z klientem).](request-a-relationship-with-a-customer.md)</span><span class="sxs-lookup"><span data-stu-id="f339d-115">For more information, see [Request a reseller relationship with a customer](request-a-relationship-with-a-customer.md).</span></span>   |
|<span data-ttu-id="f339d-116">Usługi oparte na użyciu</span><span class="sxs-lookup"><span data-stu-id="f339d-116">Usage-based services</span></span>     |  <span data-ttu-id="f339d-117">W przypadku klienta, który ma już subskrypcję usługi Microsoft Azure z innego kanału, takiego jak Advisor, Open lub EA, musisz utworzyć nową subskrypcję platformy Azure w usłudze Partner Center, ręcznie wprowadzić szczegóły subskrypcji, a następnie anulować poszczególne usługi lub całą subskrypcję.</span><span class="sxs-lookup"><span data-stu-id="f339d-117">For a customer who already has a subscription to Microsoft Azure from another channel, such as Advisor, Open, or EA, you'll need to create a new Azure subscription in Partner Center, manually enter the subscription details, and then cancel the individual services or the entire subscription.</span></span> <span data-ttu-id="f339d-118">Azure CSP współistnieć z różnymi kanałami.</span><span class="sxs-lookup"><span data-stu-id="f339d-118">Azure CSP can coexist with different channels.</span></span><br/><br/> <span data-ttu-id="f339d-119">Na przykład w przypadku klienta, który ma już subskrypcję usługi Microsoft Azure innego partnera, możesz przełączyć usługi platformy Azure na innego partnera.</span><span class="sxs-lookup"><span data-stu-id="f339d-119">For a customer who already has a subscription to Microsoft Azure from another partner, for example, you can switch Azure services to the other partner.</span></span>  <span data-ttu-id="f339d-120">Aby uzyskać więcej informacji, zobacz [Przełączanie subskrypcji platformy Azure na innego partnera.](switch-azure-subscriptions-to-a-different-partner.md)</span><span class="sxs-lookup"><span data-stu-id="f339d-120">For more information, see [Switch Azure subscriptions to a different partner](switch-azure-subscriptions-to-a-different-partner.md).</span></span> |

> [!IMPORTANT]  
> <span data-ttu-id="f339d-121">Partner CSP nie może obecnie odsprzedawać Usługi online partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="f339d-121">A CSP partner cannot resell online services to another CSP partner currently.</span></span> <span data-ttu-id="f339d-122">Firma Microsoft stale przegląda zasady i możliwości wszystkich programów.</span><span class="sxs-lookup"><span data-stu-id="f339d-122">Microsoft continuously reviews policies and capabilities of all programs.</span></span> <span data-ttu-id="f339d-123">Wszelkie ogłoszenia o wydaniach funkcji będą ogłaszane za pośrednictwem zwykłych kanałów komunikacyjnych, w tym Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f339d-123">Any announcements about feature releases will be announced through the usual communication channels, including the Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f339d-124">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="f339d-124">Next steps</span></span>

[<span data-ttu-id="f339d-125">Praca z innymi partnerami</span><span class="sxs-lookup"><span data-stu-id="f339d-125">Work with other partners</span></span>](work-with-other-partners.md)

- <span data-ttu-id="f339d-126">Jeśli jesteś odsprzedawcą pośrednim, zobacz [partner z dostawcami pośrednimi](indirect-reseller-tasks-in-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="f339d-126">If you're an indirect reseller, see [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md).</span></span>

- <span data-ttu-id="f339d-127">Jeśli jesteś dostawcą pośrednim, zobacz [Partner with indirect resellers (Partner z odsprzedawcami pośrednimi).](indirect-provider-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="f339d-127">If you're an indirect provider, see [Partner with indirect resellers](indirect-provider-tasks-in-partner-center.md).</span></span>
