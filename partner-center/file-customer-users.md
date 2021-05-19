---
title: Pola dla pliku CSV do importowania wielu użytkowników dla konta klienta
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aby dodać wielu użytkowników do konta klienta, utwórz plik wartości rozdzielanych przecinkami (CSV) z odpowiednimi polami.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150985"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="63f09-103">Dodawanie wielu użytkowników do konta klienta przez utworzenie pliku CSV</span><span class="sxs-lookup"><span data-stu-id="63f09-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="63f09-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="63f09-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="63f09-105">Dodaj wielu użytkowników do konta klienta jednocześnie, przesyłając plik danych w formacie pliku wartości rozdzielanych przecinkami (csv) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="63f09-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="63f09-106">Możesz pobrać przykładowy plik danych z usługi Partner Center następnie edytować go do własnego użytku lub utworzyć nowy plik danych przy użyciu modelu danych zdefiniowanego poniżej.</span><span class="sxs-lookup"><span data-stu-id="63f09-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="63f09-107">Wymagania dotyczące pliku danych</span><span class="sxs-lookup"><span data-stu-id="63f09-107">Data file requirements</span></span>

<span data-ttu-id="63f09-108">Aby dodać wielu użytkowników do konta klienta przy użyciu procesu przekazywania zbiorczego, należy spełnić następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="63f09-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="63f09-109">Musisz mieć uprawnienia administratora globalnego do konta klienta;</span><span class="sxs-lookup"><span data-stu-id="63f09-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="63f09-110">Każdy użytkownik musi mieć unikatowy adres e-mail dołączony do domen poczty e-mail klienta;</span><span class="sxs-lookup"><span data-stu-id="63f09-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="63f09-111">Jednocześnie można przekazać maksymalnie 100 rekordów.</span><span class="sxs-lookup"><span data-stu-id="63f09-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="63f09-112">Jeśli musisz dodać więcej niż 100 użytkowników, utwórz i przekaż dodatkowe pliki danych.</span><span class="sxs-lookup"><span data-stu-id="63f09-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="63f09-113">Wszyscy użytkownicy muszą znajdować się w tej samej lokalizacji **geograficznej.**</span><span class="sxs-lookup"><span data-stu-id="63f09-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="63f09-114">Wprowadź tylko dane opisane poniżej.</span><span class="sxs-lookup"><span data-stu-id="63f09-114">Enter only the data described below.</span></span> <span data-ttu-id="63f09-115">Extraneous data will cause the upload to fail.</span><span class="sxs-lookup"><span data-stu-id="63f09-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="63f09-116">Wprowadź następujące dane w pliku danych:</span><span class="sxs-lookup"><span data-stu-id="63f09-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="63f09-117">**Nazwa kolumny**</span><span class="sxs-lookup"><span data-stu-id="63f09-117">**Column name**</span></span> | <span data-ttu-id="63f09-118">**Opis**</span><span class="sxs-lookup"><span data-stu-id="63f09-118">**Description**</span></span>  | <span data-ttu-id="63f09-119">**Ograniczenie**</span><span class="sxs-lookup"><span data-stu-id="63f09-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="63f09-120">Imię</span><span class="sxs-lookup"><span data-stu-id="63f09-120">First name</span></span>  | <span data-ttu-id="63f09-121">Imię użytkownika (pole opcjonalne)</span><span class="sxs-lookup"><span data-stu-id="63f09-121">User's first name (optional field)</span></span>  | <span data-ttu-id="63f09-122">Limit 50 znaków</span><span class="sxs-lookup"><span data-stu-id="63f09-122">50-character limit</span></span>  |
| <span data-ttu-id="63f09-123">Nazwisko</span><span class="sxs-lookup"><span data-stu-id="63f09-123">Last name</span></span>  | <span data-ttu-id="63f09-124">Nazwisko użytkownika (pole opcjonalne)</span><span class="sxs-lookup"><span data-stu-id="63f09-124">User's last name (optional field)</span></span>  | <span data-ttu-id="63f09-125">Limit 50 znaków</span><span class="sxs-lookup"><span data-stu-id="63f09-125">50-character limit</span></span>  |
| <span data-ttu-id="63f09-126">Nazwa wyświetlana</span><span class="sxs-lookup"><span data-stu-id="63f09-126">Display name</span></span>    | <span data-ttu-id="63f09-127">Nazwa wyświetlana w Partner Center (pole wymagane)</span><span class="sxs-lookup"><span data-stu-id="63f09-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="63f09-128">Limit 50 znaków</span><span class="sxs-lookup"><span data-stu-id="63f09-128">50-character limit</span></span>                         |
| <span data-ttu-id="63f09-129">E-mail</span><span class="sxs-lookup"><span data-stu-id="63f09-129">Email</span></span>   | <span data-ttu-id="63f09-130">Służbowy adres e-mail użytkownika w firmie klienta (pole wymagane)</span><span class="sxs-lookup"><span data-stu-id="63f09-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="63f09-131">Każdy użytkownik musi mieć unikatowy adres e-mail</span><span class="sxs-lookup"><span data-stu-id="63f09-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="63f09-132">Aktualizacja stanu</span><span class="sxs-lookup"><span data-stu-id="63f09-132">Status update</span></span>   | <span data-ttu-id="63f09-133">Służy do wskazywania, czy nowy rekord użytkownika został pomyślnie utworzony</span><span class="sxs-lookup"><span data-stu-id="63f09-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="63f09-134">\*\*Pozostaw puste\*\*</span><span class="sxs-lookup"><span data-stu-id="63f09-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="63f09-135">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="63f09-135">Next steps</span></span>

- [<span data-ttu-id="63f09-136">Jak dodać wielu użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="63f09-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)