---
title: Dodawanie wielu użytkowników dla konta klienta
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aby dodać wielu użytkowników do konta klienta, przekaż plik danych do usługi Partner Center format pliku wartości rozdzielanych przecinkami (csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150475"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="aba51-103">Przekazywanie pliku CSV użytkowników na konto klienta</span><span class="sxs-lookup"><span data-stu-id="aba51-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="aba51-104">**Odpowiednie role:** Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="aba51-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="aba51-105">Dodaj wielu użytkowników do konta klienta jednocześnie, przesyłając plik danych w formacie pliku wartości rozdzielanych przecinkami (csv) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="aba51-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="aba51-106">Tworzenie pliku użytkowników klienta i przekazywanie go do konta klienta</span><span class="sxs-lookup"><span data-stu-id="aba51-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="aba51-107">Utwórz plik danych wartości rozdzielanych przecinkami (CSV) z danymi opisanymi powyżej.</span><span class="sxs-lookup"><span data-stu-id="aba51-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="aba51-108">Zapisz plik, aby można było przejść do niego w późniejszym kroku.</span><span class="sxs-lookup"><span data-stu-id="aba51-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="aba51-109">Zobacz [Pola dla pliku CSV, aby zaimportować wielu użytkowników dla konta klienta.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="aba51-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="aba51-110">Zaloguj się do pulpitu Partner Center [nawigacyjnego.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="aba51-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="aba51-111">Z Partner Center wybierz pozycję **Klienci,** a następnie wybierz klienta z listy.</span><span class="sxs-lookup"><span data-stu-id="aba51-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="aba51-112">Wybierz kartę Użytkownicy **i** licencje klienta, a następnie wybierz **pozycję Przekaż użytkowników.**</span><span class="sxs-lookup"><span data-stu-id="aba51-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="aba51-113">W **obszarze Przekaż informacje o użytkowniku** wybierz pozycję **Przeglądaj.**</span><span class="sxs-lookup"><span data-stu-id="aba51-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="aba51-114">W selektorze plików wybierz plik danych, a następnie wybierz pozycję **Otwórz**.</span><span class="sxs-lookup"><span data-stu-id="aba51-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="aba51-115">Wybierz przycisk **Weryfikuj**.</span><span class="sxs-lookup"><span data-stu-id="aba51-115">Select **Validate**.</span></span>

    <span data-ttu-id="aba51-116">**Uwaga**  Większość błędów tworzenia konta jest spowodowanych przez problemy z plikami danych, w tym brakujące informacje, źle sformułowane lub zduplikowane adresy e-mail albo zbyt wiele rekordów w pliku.</span><span class="sxs-lookup"><span data-stu-id="aba51-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="aba51-117">Po Partner Center pliku wybierz lokalizację geograficzną **dla** nowych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="aba51-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="aba51-118">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="aba51-118">Select **Save**.</span></span>
10. <span data-ttu-id="aba51-119">Pobierz tymczasowe informacje o hasłach dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="aba51-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="aba51-120">Pamiętaj, aby teraz pobrać plik z hasłami tymczasowymi, ponieważ nie będzie można tego zrobić później.</span><span class="sxs-lookup"><span data-stu-id="aba51-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="aba51-121">Nowi użytkownicy muszą zalogować się do nowego konta przy użyciu hasła tymczasowego dla nowych kont.</span><span class="sxs-lookup"><span data-stu-id="aba51-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="aba51-122">Nowym użytkownikom są automatycznie przypisywane uprawnienia z listy **Może korzystać z licencji i usług.**</span><span class="sxs-lookup"><span data-stu-id="aba51-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="aba51-123">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="aba51-123">Next steps</span></span>

- [<span data-ttu-id="aba51-124">Nadaj klientom uprawnienia Partner Center do kupowania własnych produktów lub usług</span><span class="sxs-lookup"><span data-stu-id="aba51-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
