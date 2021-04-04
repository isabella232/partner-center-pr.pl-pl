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
ms.openlocfilehash: c2f8e4d3351c9905d7066534946b24bd9a8c8cd4
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132268"
---
# <a name="multi-partner-support-for-customers-who-want-to-work-with-more-than-one-partner"></a><span data-ttu-id="e531a-103">Obsługa wielu partnerów dla klientów, którzy chcą korzystać z więcej niż jednego partnera</span><span class="sxs-lookup"><span data-stu-id="e531a-103">Multi-partner support for customers who want to work with more than one partner</span></span>

<span data-ttu-id="e531a-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="e531a-104">**Applies to**</span></span>

- <span data-ttu-id="e531a-105">Centrum partnerskie w chmurze firmy Microsoft dla instytucji rządowych</span><span class="sxs-lookup"><span data-stu-id="e531a-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="e531a-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="e531a-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e531a-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="e531a-107">Global admin</span></span>
- <span data-ttu-id="e531a-108">Administrator zarządzania użytkownikami</span><span class="sxs-lookup"><span data-stu-id="e531a-108">User management admin</span></span>
- <span data-ttu-id="e531a-109">Agent sprzedaży</span><span class="sxs-lookup"><span data-stu-id="e531a-109">Sales agent</span></span>

<span data-ttu-id="e531a-110">Funkcja wielu partnerów w centrum partnerskim obsługuje scenariusze, gdy klient chce współpracować z więcej niż jednym partnerem.</span><span class="sxs-lookup"><span data-stu-id="e531a-110">The Partner Center's multi-partner feature supports scenarios when a customer wants to work with more than one partner.</span></span> <span data-ttu-id="e531a-111">Na przykład klient może chcieć zatrudniać jednego partnera w celu uzyskania ekspertyzy w pakiecie Office 365, ale zatrudniać innego partnera, który jest wyspecjalizowany w Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="e531a-111">For example, a customer may want to hire one partner for their expertise in Office 365, but hire a different partner who specializes in Microsoft Azure.</span></span>

<span data-ttu-id="e531a-112">Dzierżawa CSP platformy Azure może obejmować dodatkową subskrypcję platformy Azure od innego partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="e531a-112">An Azure CSP tenant can include an additional Azure subscription from a different CSP partner.</span></span>

<span data-ttu-id="e531a-113">Aby skorzystać z funkcji wielopartnerskiej w centrum partnerskim, Zaproś klienta o przyznanie uprawnień administracji delegowanej.</span><span class="sxs-lookup"><span data-stu-id="e531a-113">To use the multi-partner feature in the Partner Center, invite the customer to give you delegated administration privileges.</span></span> <span data-ttu-id="e531a-114">Zobacz [żądanie relacji z klientem](request-a-relationship-with-a-customer.md) , aby uzyskać informacje na temat sposobu ustanawiania relacji z klientem, który już pracuje z partnerem.</span><span class="sxs-lookup"><span data-stu-id="e531a-114">See [Request a relationship with a customer](request-a-relationship-with-a-customer.md) for information about how to establish a relationship with a customer who is already working with a partner.</span></span>

<span data-ttu-id="e531a-115">Funkcje wielopartnerskie nie są następujące:</span><span class="sxs-lookup"><span data-stu-id="e531a-115">Multi-partner functionality does not:</span></span>

- <span data-ttu-id="e531a-116">Zmiana wszystkich istniejących subskrypcji klienta</span><span class="sxs-lookup"><span data-stu-id="e531a-116">Change any of the customer's existing subscriptions</span></span>

- <span data-ttu-id="e531a-117">Przeniesienie istniejących subskrypcji lub własności konta klienta</span><span class="sxs-lookup"><span data-stu-id="e531a-117">Transition the customer's existing subscriptions or account ownership</span></span>

- <span data-ttu-id="e531a-118">Zmień warunki lub zobowiązania klienta dla dowolnej z istniejących subskrypcji</span><span class="sxs-lookup"><span data-stu-id="e531a-118">Change the terms or customer's obligations for any of their existing subscriptions</span></span>

- <span data-ttu-id="e531a-119">Zmiana partnera rekordu dla subskrypcji</span><span class="sxs-lookup"><span data-stu-id="e531a-119">Change the partner of record for a subscription</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="e531a-120">Partner w programie CSP nie może obecnie odsprzedać Usługi online innego partnera w programie CSP.</span><span class="sxs-lookup"><span data-stu-id="e531a-120">A partner in the CSP program cannot resell online services to another partner in the CSP program currently.</span></span> <span data-ttu-id="e531a-121">To ograniczenie dotyczy tylko dzierżawcy używanej do przeprowadzania transakcji dostawcy CSP.</span><span class="sxs-lookup"><span data-stu-id="e531a-121">This restriction only applies to the tenant used for conducting CSP transactions.</span></span> <span data-ttu-id="e531a-122">Partnerzy programu CSP korzystający z dzierżawy niebędącej dostawcą usług kryptograficznych do użycia w firmie mogą kupować Usługi online od innego partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="e531a-122">CSP partners who use a non-CSP tenant for their corporate usage can purchase online services from another CSP partner.</span></span> <span data-ttu-id="e531a-123">Firma Microsoft stale przegląda zasady i możliwości wszystkich programów.</span><span class="sxs-lookup"><span data-stu-id="e531a-123">Microsoft continuously reviews the policies and capabilities of all programs.</span></span> <span data-ttu-id="e531a-124">Wszystkie wiadomości dotyczące wersji funkcji lub zmian zasad zostaną ogłoszone za pośrednictwem zwykłych kanałów komunikacji, w tym [anonsów Centrum partnerskiego](announcements/index.md).</span><span class="sxs-lookup"><span data-stu-id="e531a-124">Any news about feature releases or policy changes will be announced through the usual communications channels, including [Partner Center announcements](announcements/index.md).</span></span>
