---
title: Pola pliku CSV do importowania wielu użytkowników dla konta klienta
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aby dodać wielu użytkowników do konta klienta, Utwórz plik z wartościami rozdzielanymi przecinkami (CSV) z odpowiednimi polami.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441425"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="cb3f1-103">Dodawanie wielu użytkowników do konta klienta przez utworzenie pliku CSV</span><span class="sxs-lookup"><span data-stu-id="cb3f1-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="cb3f1-104">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="cb3f1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="cb3f1-105">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="cb3f1-105">Global admin</span></span>

<span data-ttu-id="cb3f1-106">Jednocześnie Dodaj wielu użytkowników do konta klienta, przekazując plik danych w formacie pliku wartości rozdzielanych przecinkami (CSV) do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="cb3f1-107">Możesz pobrać przykładowy plik danych z Centrum partnerskiego, a następnie edytować go w celu użycia lub utworzyć nowy plik danych przy użyciu modelu danych zdefiniowanego poniżej.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="cb3f1-108">Wymagania dotyczące pliku danych</span><span class="sxs-lookup"><span data-stu-id="cb3f1-108">Data file requirements</span></span>

<span data-ttu-id="cb3f1-109">Aby dodać wielu użytkowników do konta klienta przy użyciu procesu przekazywania zbiorczego, należy spełnić następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="cb3f1-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="cb3f1-110">Użytkownik musi mieć uprawnienia administratora globalnego do konta klienta.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="cb3f1-111">Każdy użytkownik musi mieć unikatowy adres e-mail dołączony do domen poczty e-mail klienta;</span><span class="sxs-lookup"><span data-stu-id="cb3f1-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="cb3f1-112">Jednocześnie można przekazać do 100 rekordów.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="cb3f1-113">Jeśli musisz dodać więcej niż 100 użytkowników, Utwórz i przekaż dodatkowe pliki danych.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="cb3f1-114">Wszyscy użytkownicy muszą znajdować się w tej samej **lokalizacji** geograficznej.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="cb3f1-115">Wprowadź tylko dane opisane poniżej.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-115">Enter only the data described below.</span></span> <span data-ttu-id="cb3f1-116">Dane nadmiarowe spowodują, że przekazywanie zakończy się niepowodzeniem.</span><span class="sxs-lookup"><span data-stu-id="cb3f1-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="cb3f1-117">Wprowadź następujące dane w pliku danych:</span><span class="sxs-lookup"><span data-stu-id="cb3f1-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="cb3f1-118">**Nazwa kolumny**</span><span class="sxs-lookup"><span data-stu-id="cb3f1-118">**Column name**</span></span> | <span data-ttu-id="cb3f1-119">**Opis**</span><span class="sxs-lookup"><span data-stu-id="cb3f1-119">**Description**</span></span>  | <span data-ttu-id="cb3f1-120">**Ograniczenie**</span><span class="sxs-lookup"><span data-stu-id="cb3f1-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="cb3f1-121">Imię</span><span class="sxs-lookup"><span data-stu-id="cb3f1-121">First name</span></span>  | <span data-ttu-id="cb3f1-122">Imię użytkownika (pole opcjonalne)</span><span class="sxs-lookup"><span data-stu-id="cb3f1-122">User's first name (optional field)</span></span>  | <span data-ttu-id="cb3f1-123">50 — limit znaków</span><span class="sxs-lookup"><span data-stu-id="cb3f1-123">50-character limit</span></span>  |
| <span data-ttu-id="cb3f1-124">Nazwisko</span><span class="sxs-lookup"><span data-stu-id="cb3f1-124">Last name</span></span>  | <span data-ttu-id="cb3f1-125">Nazwisko użytkownika (pole opcjonalne)</span><span class="sxs-lookup"><span data-stu-id="cb3f1-125">User's last name (optional field)</span></span>  | <span data-ttu-id="cb3f1-126">50 — limit znaków</span><span class="sxs-lookup"><span data-stu-id="cb3f1-126">50-character limit</span></span>  |
| <span data-ttu-id="cb3f1-127">Nazwa wyświetlana</span><span class="sxs-lookup"><span data-stu-id="cb3f1-127">Display name</span></span>    | <span data-ttu-id="cb3f1-128">Nazwa wyświetlana w centrum partnerskim (pole wymagane)</span><span class="sxs-lookup"><span data-stu-id="cb3f1-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="cb3f1-129">50 — limit znaków</span><span class="sxs-lookup"><span data-stu-id="cb3f1-129">50-character limit</span></span>                         |
| <span data-ttu-id="cb3f1-130">E-mail</span><span class="sxs-lookup"><span data-stu-id="cb3f1-130">Email</span></span>   | <span data-ttu-id="cb3f1-131">Służbowy adres e-mail użytkownika w firmie klienta (wymagane pole)</span><span class="sxs-lookup"><span data-stu-id="cb3f1-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="cb3f1-132">Każdy użytkownik musi mieć unikatowy adres e-mail</span><span class="sxs-lookup"><span data-stu-id="cb3f1-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="cb3f1-133">Aktualizacja stanu</span><span class="sxs-lookup"><span data-stu-id="cb3f1-133">Status update</span></span>   | <span data-ttu-id="cb3f1-134">Służy do wskazywania, czy nowy rekord użytkownika został pomyślnie utworzony</span><span class="sxs-lookup"><span data-stu-id="cb3f1-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="cb3f1-135">\*\*Pozostaw puste\*\*</span><span class="sxs-lookup"><span data-stu-id="cb3f1-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="cb3f1-136">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="cb3f1-136">Next steps</span></span>

- [<span data-ttu-id="cb3f1-137">Jak dodać wielu użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="cb3f1-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)