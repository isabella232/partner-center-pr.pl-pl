---
title: Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych
description: Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376668"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="07b60-103">Wymagania wstępne dotyczące programowego uzyskiwania dostępu do danych analitycznych</span><span class="sxs-lookup"><span data-stu-id="07b60-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="07b60-104">**Odpowiednie role:** Administrator globalny | Administrator programu MPN</span><span class="sxs-lookup"><span data-stu-id="07b60-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="07b60-105">Aby programowo uzyskać dostęp do danych analitycznych szczegółowych informacji dla partnerów, należy spełnić następujące wymagania.</span><span class="sxs-lookup"><span data-stu-id="07b60-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="07b60-106">Rejestracja w programie MPN</span><span class="sxs-lookup"><span data-stu-id="07b60-106">MPN Program enrollment</span></span>

<span data-ttu-id="07b60-107">Aby programowo uzyskać dostęp do danych analizy szczegółowych informacji partnera, musisz być zarejestrowany w programie MPN i mieć Partner Center konto.</span><span class="sxs-lookup"><span data-stu-id="07b60-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="07b60-108">Aby dowiedzieć się, jak to zrobić, [zobacz Tworzenie konta MPN w Partner Center](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="07b60-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="07b60-109">Tworzenie Azure Active Directory (AAD)</span><span class="sxs-lookup"><span data-stu-id="07b60-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="07b60-110">Zwykłych poświadczeń użytkownika nie można używać do programowego dostępu do danych usługi Partner Szczegółowe informacje Analytics.</span><span class="sxs-lookup"><span data-stu-id="07b60-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="07b60-111">Aby Azure Active Directory programowych interfejsów API dostępu, należy utworzyć aplikację Azure Active Directory (AAD) wraz z kluczem tajnym (aplikacja i dostęp użytkowników).</span><span class="sxs-lookup"><span data-stu-id="07b60-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="07b60-112">Aby dowiedzieć się, jak utworzyć aplikację i klucz tajny WAD, zobacz Szybki start: rejestrowanie aplikacji za pomocą [Platforma tożsamości Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Aby uzyskać dostęp do usługi Microsoft interfejs API Partner, wymagane jest uprawnienie.</span><span class="sxs-lookup"><span data-stu-id="07b60-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="07b60-113">Aby dowiedzieć się, jak dodać uprawnienie, zobacz [interfejs API Partner — Partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="07b60-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="07b60-114">Przypisywanie użytkownikowi roli Executive Report Viewer (ERV)</span><span class="sxs-lookup"><span data-stu-id="07b60-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="07b60-115">Aby programowo uzyskać dostęp do danych analizy szczegółowych informacji partnerów, musisz mieć programowego podglądu raportów kadry kierowniczej (ERV).</span><span class="sxs-lookup"><span data-stu-id="07b60-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="07b60-116">Aby dowiedzieć się, jak przypisać użytkownikowi rolę ERV, zobacz [Partner Center Szczegółowe informacje dostęp oparty na](insights-roles.md) rolach — Partner Center</span><span class="sxs-lookup"><span data-stu-id="07b60-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="07b60-117">Generowanie tokenu usługi AAD</span><span class="sxs-lookup"><span data-stu-id="07b60-117">Generate an AAD token</span></span>

<span data-ttu-id="07b60-118">Token usługi AAD należy wygenerować przy użyciu identyfikatora aplikacji (klienta), hasła klienta, identyfikatora użytkownika i hasła.   [Sprawdź tutaj,](insights-programmatic-first-api-call.md#token-generation) aby uzyskać instrukcje generowania tokenu usługi AAD.</span><span class="sxs-lookup"><span data-stu-id="07b60-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="07b60-119">Token jest ważny przez jedną godzinę.</span><span class="sxs-lookup"><span data-stu-id="07b60-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="07b60-120">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="07b60-120">Next steps</span></span>
[<span data-ttu-id="07b60-121">Paradygmat dostępu programowego</span><span class="sxs-lookup"><span data-stu-id="07b60-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)