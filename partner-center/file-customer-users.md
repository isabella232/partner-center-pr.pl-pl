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
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/03/2020
ms.locfileid: "92529433"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="ca3df-103">Dodawanie wielu użytkowników do konta klienta przez utworzenie pliku CSV</span><span class="sxs-lookup"><span data-stu-id="ca3df-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="ca3df-104">**Dotyczy**</span><span class="sxs-lookup"><span data-stu-id="ca3df-104">**Applies to**</span></span>

- <span data-ttu-id="ca3df-105">Centrum partnerskie</span><span class="sxs-lookup"><span data-stu-id="ca3df-105">Partner Center</span></span>

<span data-ttu-id="ca3df-106">**Odpowiednie role**</span><span class="sxs-lookup"><span data-stu-id="ca3df-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ca3df-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="ca3df-107">Global admin</span></span>

<span data-ttu-id="ca3df-108">Jednocześnie Dodaj wielu użytkowników do konta klienta, przekazując plik danych w formacie pliku wartości rozdzielanych przecinkami (CSV) do Centrum partnerskiego.</span><span class="sxs-lookup"><span data-stu-id="ca3df-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="ca3df-109">Możesz pobrać przykładowy plik danych z Centrum partnerskiego, a następnie edytować go w celu użycia lub utworzyć nowy plik danych przy użyciu modelu danych zdefiniowanego poniżej.</span><span class="sxs-lookup"><span data-stu-id="ca3df-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="ca3df-110">Wymagania dotyczące pliku danych</span><span class="sxs-lookup"><span data-stu-id="ca3df-110">Data file requirements</span></span>

<span data-ttu-id="ca3df-111">Aby dodać wielu użytkowników do konta klienta przy użyciu procesu przekazywania zbiorczego, należy spełnić następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="ca3df-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="ca3df-112">Użytkownik musi mieć uprawnienia administratora globalnego do konta klienta.</span><span class="sxs-lookup"><span data-stu-id="ca3df-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="ca3df-113">Każdy użytkownik musi mieć unikatowy adres e-mail dołączony do domen poczty e-mail klienta;</span><span class="sxs-lookup"><span data-stu-id="ca3df-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="ca3df-114">Jednocześnie można przekazać do 100 rekordów.</span><span class="sxs-lookup"><span data-stu-id="ca3df-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="ca3df-115">Jeśli musisz dodać więcej niż 100 użytkowników, Utwórz i przekaż dodatkowe pliki danych.</span><span class="sxs-lookup"><span data-stu-id="ca3df-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="ca3df-116">Wszyscy użytkownicy muszą znajdować się w tej samej **lokalizacji** geograficznej.</span><span class="sxs-lookup"><span data-stu-id="ca3df-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="ca3df-117">Wprowadź tylko dane opisane poniżej.</span><span class="sxs-lookup"><span data-stu-id="ca3df-117">Enter only the data described below.</span></span> <span data-ttu-id="ca3df-118">Dane nadmiarowe spowodują, że przekazywanie zakończy się niepowodzeniem.</span><span class="sxs-lookup"><span data-stu-id="ca3df-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="ca3df-119">Wprowadź następujące dane w pliku danych:</span><span class="sxs-lookup"><span data-stu-id="ca3df-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="ca3df-120">**Nazwa kolumny**</span><span class="sxs-lookup"><span data-stu-id="ca3df-120">**Column name**</span></span> | <span data-ttu-id="ca3df-121">**Opis**</span><span class="sxs-lookup"><span data-stu-id="ca3df-121">**Description**</span></span>  | <span data-ttu-id="ca3df-122">**Ograniczenie**</span><span class="sxs-lookup"><span data-stu-id="ca3df-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="ca3df-123">Imię</span><span class="sxs-lookup"><span data-stu-id="ca3df-123">First name</span></span>  | <span data-ttu-id="ca3df-124">Imię użytkownika (pole opcjonalne)</span><span class="sxs-lookup"><span data-stu-id="ca3df-124">User's first name (optional field)</span></span>  | <span data-ttu-id="ca3df-125">50 — limit znaków</span><span class="sxs-lookup"><span data-stu-id="ca3df-125">50-character limit</span></span>  |
| <span data-ttu-id="ca3df-126">Nazwisko</span><span class="sxs-lookup"><span data-stu-id="ca3df-126">Last name</span></span>  | <span data-ttu-id="ca3df-127">Nazwisko użytkownika (pole opcjonalne)</span><span class="sxs-lookup"><span data-stu-id="ca3df-127">User's last name (optional field)</span></span>  | <span data-ttu-id="ca3df-128">50 — limit znaków</span><span class="sxs-lookup"><span data-stu-id="ca3df-128">50-character limit</span></span>  |
| <span data-ttu-id="ca3df-129">Nazwa wyświetlana</span><span class="sxs-lookup"><span data-stu-id="ca3df-129">Display name</span></span>    | <span data-ttu-id="ca3df-130">Nazwa wyświetlana w centrum partnerskim (pole wymagane)</span><span class="sxs-lookup"><span data-stu-id="ca3df-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="ca3df-131">50 — limit znaków</span><span class="sxs-lookup"><span data-stu-id="ca3df-131">50-character limit</span></span>                         |
| <span data-ttu-id="ca3df-132">E-mail</span><span class="sxs-lookup"><span data-stu-id="ca3df-132">Email</span></span>   | <span data-ttu-id="ca3df-133">Służbowy adres e-mail użytkownika w firmie klienta (wymagane pole)</span><span class="sxs-lookup"><span data-stu-id="ca3df-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="ca3df-134">Każdy użytkownik musi mieć unikatowy adres e-mail</span><span class="sxs-lookup"><span data-stu-id="ca3df-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="ca3df-135">Aktualizacja stanu</span><span class="sxs-lookup"><span data-stu-id="ca3df-135">Status update</span></span>   | <span data-ttu-id="ca3df-136">Służy do wskazania, czy nowy rekord użytkownika został pomyślnie utworzony</span><span class="sxs-lookup"><span data-stu-id="ca3df-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="ca3df-137">\*\*Pozostaw puste\*\*</span><span class="sxs-lookup"><span data-stu-id="ca3df-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="ca3df-138">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="ca3df-138">Next steps</span></span>

- [<span data-ttu-id="ca3df-139">Jak dodać wielu użytkowników dla klienta</span><span class="sxs-lookup"><span data-stu-id="ca3df-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)