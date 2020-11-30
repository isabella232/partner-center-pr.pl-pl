---
title: Obsługa wielu partnerów
ms.topic: article
ms.date: 11/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Klient może chcieć współpracować z wieloma partnerami w programie dostawcy rozwiązań w chmurze, który specjalizacje w różnych usługach.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 728a1b7ec4d6b51174f1d3f6fcf21a6385fc4e7a
ms.sourcegitcommit: c79137fba9e70037a2dc0e4a99c7334696c3740a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/30/2020
ms.locfileid: "96322121"
---
# <a name="multi-partner-support-for-customers-who-want-to-work-with-more-than-one-partner"></a><span data-ttu-id="a78b1-103">Obsługa wielu partnerów dla klientów, którzy chcą korzystać z więcej niż jednego partnera</span><span class="sxs-lookup"><span data-stu-id="a78b1-103">Multi-partner support for customers who want to work with more than one partner</span></span>

<span data-ttu-id="a78b1-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="a78b1-104">**Applies to**</span></span>

- <span data-ttu-id="a78b1-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="a78b1-105">Partner Center</span></span>
- <span data-ttu-id="a78b1-106">Centrum partnerskie Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="a78b1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="a78b1-107">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="a78b1-107">**Appropriate roles**</span></span>

- <span data-ttu-id="a78b1-108">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="a78b1-108">Global admin</span></span>
- <span data-ttu-id="a78b1-109">Administrator użytkowników</span><span class="sxs-lookup"><span data-stu-id="a78b1-109">User admin</span></span>
- <span data-ttu-id="a78b1-110">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="a78b1-110">Sales agent</span></span>

<span data-ttu-id="a78b1-111">Funkcja wielu partnerów w centrum partnerskim obsługuje scenariusze, gdy klient chce współpracować z więcej niż jednym partnerem.</span><span class="sxs-lookup"><span data-stu-id="a78b1-111">The Partner Center's multi-partner feature supports scenarios when a customer wants to work with more than one partner.</span></span> <span data-ttu-id="a78b1-112">Na przykład klient może chcieć zatrudniać jednego partnera w celu uzyskania ekspertyzy w pakiecie Office 365, ale zatrudniać innego partnera, który jest wyspecjalizowany w Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="a78b1-112">For example, a customer may want to hire one partner for their expertise in Office 365, but hire a different partner who specializes in Microsoft Azure.</span></span>

<span data-ttu-id="a78b1-113">Dzierżawa CSP platformy Azure może obejmować dodatkową subskrypcję platformy Azure od innego partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="a78b1-113">An Azure CSP tenant can include an additional Azure subscription from a different CSP partner.</span></span>

<span data-ttu-id="a78b1-114">Aby skorzystać z funkcji wielopartnerskiej w centrum partnerskim, Zaproś klienta o przyznanie uprawnień administracji delegowanej.</span><span class="sxs-lookup"><span data-stu-id="a78b1-114">To use the multi-partner feature in the Partner Center, invite the customer to give you delegated administration privileges.</span></span> <span data-ttu-id="a78b1-115">Zobacz [żądanie relacji z klientem](request-a-relationship-with-a-customer.md) , aby uzyskać informacje na temat sposobu ustanawiania relacji z klientem, który już pracuje z partnerem.</span><span class="sxs-lookup"><span data-stu-id="a78b1-115">See [Request a relationship with a customer](request-a-relationship-with-a-customer.md) for information about how to establish a relationship with a customer who is already working with a partner.</span></span>

<span data-ttu-id="a78b1-116">Funkcje wielopartnerskie nie są następujące:</span><span class="sxs-lookup"><span data-stu-id="a78b1-116">Multi-partner functionality does not:</span></span>

- <span data-ttu-id="a78b1-117">Zmiana wszystkich istniejących subskrypcji klienta</span><span class="sxs-lookup"><span data-stu-id="a78b1-117">Change any of the customer's existing subscriptions</span></span>

- <span data-ttu-id="a78b1-118">Przeniesienie istniejących subskrypcji lub własności konta klienta</span><span class="sxs-lookup"><span data-stu-id="a78b1-118">Transition the customer's existing subscriptions or account ownership</span></span>

- <span data-ttu-id="a78b1-119">Zmień warunki lub zobowiązania klienta dla dowolnej z istniejących subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a78b1-119">Change the terms or customer's obligations for any of their existing subscriptions</span></span>

- <span data-ttu-id="a78b1-120">Zmiana partnera rekordu dla subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a78b1-120">Change the partner of record for a subscription</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="a78b1-121">Partner w programie CSP nie może obecnie odsprzedać Usługi online innego partnera w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="a78b1-121">A partner in the CSP program cannot resell online services to another partner in the CSP program currently.</span></span> <span data-ttu-id="a78b1-122">To ograniczenie dotyczy tylko dzierżawcy używanej do przeprowadzania transakcji dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="a78b1-122">This restriction only applies to the tenant used for conducting CSP transactions.</span></span> <span data-ttu-id="a78b1-123">Partnerzy programu CSP korzystający z dzierżawy niebędącej dostawcą usług kryptograficznych do użycia w firmie mogą kupować Usługi online od innego partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="a78b1-123">CSP partners who use a non-CSP tenant for their corporate usage can purchase online services from another CSP partner.</span></span> <span data-ttu-id="a78b1-124">Firma Microsoft stale przegląda zasady i możliwości wszystkich programów.</span><span class="sxs-lookup"><span data-stu-id="a78b1-124">Microsoft continuously reviews the policies and capabilities of all programs.</span></span> <span data-ttu-id="a78b1-125">Wszystkie wiadomości dotyczące wersji funkcji lub zmian zasad zostaną ogłoszone za pośrednictwem zwykłych kanałów komunikacji, w tym [anonsów Centrum partnerskiego](announcements/index.md).</span><span class="sxs-lookup"><span data-stu-id="a78b1-125">Any news about feature releases or policy changes will be announced through the usual communications channels, including [Partner Center announcements](announcements/index.md).</span></span>
