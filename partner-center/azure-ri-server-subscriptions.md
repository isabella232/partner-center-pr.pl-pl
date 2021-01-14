---
title: Rezerwacje platformy Azure & subskrypcje serwera
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o możliwościach dostawcy rozwiązań w chmurze, aby uzyskać, zainicjować i zarządzać rezerwacjami platformy Azure oraz subskrypcjami serwera dla klientów.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182498"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Pozyskiwanie, Inicjowanie obsługi & Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych platformy Azure (RI) i subskrypcjami serwera dla klientów


**Odpowiednie role**

- Agent administracyjny
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży
- Administrator zarządzania użytkownikami


## <a name="what-are-azure-reservations"></a>Co to jest Azure Reservations?

Azure Reservations pomóc zaoszczędzić pieniądze przez przedpłatę za rok lub trzy lata maszyny wirtualnej, SQL Database pojemność obliczeniowa, Azure Cosmos DB przepływność lub inne zasoby platformy Azure. Funkcja przedpłaty umożliwia uzyskanie rabatu za zasoby, których używasz. Rezerwacje mogą znacząco obniżyć swoją maszynę wirtualną, obliczenia w usłudze SQL Database, Azure Cosmos DB i inne koszty zasobów do 72% w porównaniu z cenami z płatność zgodnie z rzeczywistym użyciem. Rezerwacje umożliwiają skorzystanie z rabatu na rozliczenia i nie mają wpływu na stan środowiska uruchomieniowego Twoich zasobów. Aby uzyskać więcej informacji, zobacz [co to są Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Dlaczego klienci kupują rezerwację?

W przypadku klientów z maszynami wirtualnymi, Azure Cosmos DB lub baz danych SQL, które są uruchamiane przez długi czas, zakup rezerwacji daje im największą opłacalną opcję. Na przykład jeśli klient ciągle uruchamia cztery wystąpienia usługi bez rezerwacji, opłaty są naliczone według stawek płatność zgodnie z rzeczywistym użyciem. Jeśli kupią rezerwację dla tych zasobów, natychmiast uzyskają rabat rezerwacji. Zasoby nie będą już obciążane opłatami według stawek płatności zgodnie z rzeczywistym użyciem.

### <a name="compelling-new-azure-offer-in-csp"></a>Atrakcyjna nowa oferta platformy Azure w programie CSP

Dzięki dołączeniu Azure Reservations i subskrypcji serwera do swojego programu CSP firma Microsoft lepiej umożliwia swoim partnerom rozwiązywanie problemów z coraz większym popytem w celu uzyskania bardziej ekonomicznych rozwiązań do obsługi wysoce przewidywalnych, trwałych obciążeń w chmurze. Program CSP umożliwia partnerom pozyskiwanie, Inicjowanie obsługi i zarządzanie subskrypcjami Azure Reservations i serwera w imieniu klientów komercyjnych za pośrednictwem Centrum partnerskiego firmy Microsoft i Azure Portal.
Oferujemy również partnerów w naszym programie CSP, w których można kupować rezerwacje platformy Azure. Partnerzy programu CSP mogą [kupować rezerwacje platformy Azure w imieniu klienta](azure-reservations-buying.md) lub mogą [zezwolić klientowi na kupowanie własnych rezerwacji](give-customers-permission.md) w ramach wcześniejszej subskrypcji platformy Azure.

Azure Reservations zapewnić klientom elastyczność wirtualizacji dla szerokiego zakresu rozwiązań obliczeniowych, w tym tworzenia i testowania, uruchamiania aplikacji oraz rozszerzania centrum danych.

W [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) na przykład komercyjni klienci mogą teraz zaoszczędzić do 72%, a w przeciwieństwie do cen maszyn wirtualnych z systemem Azure — po prostu przy zakupie lub "obsłużeniu" — w przypadku okresu 1-lub 3-letniego. Klienci korzystający z systemu Windows Server z Korzyść użycia hybrydowego platformy Azure, dostępną w ramach programu Software Assurance, będą mogli zaoszczędzić do 80% w porównaniu z cenami zgodnie z rzeczywistym użyciem.

W przypadku niedopasowanej kombinacji atrakcyjnych cen i niedopasowanej elastyczności wdrożenia klienci będą widzieli najlepszą ogólną wartość, wybierając Azure Reservations.

- Zobacz [zakupy rezerwacji](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) w witrynie Azure Portal.

- Zapoznaj się z **Microsoft Azure** **listą komercyjnych cen dostawcy usług kryptograficznych (CSP) na platformie Azure** na stronie [ceny i oferty](https://partner.microsoft.com/dashboard/sell/pricingandoffers) w centrum partnerskim dla subskrypcji oprogramowania i rocznych subskrypcji systemu Linux.


 
**Subskrypcje roczne niezależnego dostawcy oprogramowania Linux**

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

**Subskrypcje roczne niezależnego dostawcy oprogramowania**

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>Wprowadzenie

Aby zrozumieć, w jaki sposób można określić, Azure Reservations z klientami oraz jak najszybciej rozpocząć pracę, zalecamy następujące podejście do przeglądu materiałów gotowości:

1. Przejrzyj i zapoznaj się z [nowym przewodnikiem obsługi handlu w centrum partnerskim](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).

2. Informacje na temat aktualizacji Azure Reservations i subskrypcji serwera w [interfejsie API Centrum partnerskiego (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).


### <a name="sales-readiness"></a>Gotowość do sprzedaży

- [Licencja dostępu klienta (CAL) Usługi pulpitu zdalnego (RDS) (anons)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [Azure Reserved VM Instances (Azure Portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [Subskrypcje serwera](./csp-software-subscriptions.md)

- [Rezerwacje bazy danych SQL (Azure Portal)](/azure/sql-database/sql-database-reserved-capacity)

- [Azure Cosmos DB (Azure Portal)](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [Wystąpienie zarządzane SQL (Azure Portal)](/azure/sql-database/sql-database-managed-instance)

- [SUSE i Red Hat Enterprise Linux (Azure Portal)](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [Red Hat Linux na platformie Azure](https://azure.com/redhat)

- [SUSE Linux na platformie Azure](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [System Linux na platformie Azure](https://azure.microsoft.com/overview/linux-on-azure/)

- [Przegląd cen platformy Azure](https://azure.microsoft.com/pricing/)

- [Kalkulator cen platformy Azure](https://azure.microsoft.com/pricing/calculator)

- [Azure Databricks rezerwacji jednostek](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a>Szkolenia

Zarejestruj się, aby wyświetlić [seminaria internetowe gotowości do licencjonowania komercyjnego](https://commercial-licensing.eventbuilder.com/FY2019_ALL) oraz zdarzenia na żądanie.
Wcześniej zarejestrowane zdarzenia gotowości licencjonowania obejmują następujące tematy:

- Usługi CSP online, dostawcy CSP Azure i ogólne aktualizacje licencjonowania, w tym Azure (listopad 2018)

- Zarezerwowana pojemność bazy danych SQL & elastyczność rozmiaru wystąpienia (sierpień 2018)

- Subskrypcje serwera w programie CSP (lipiec 2018)

- Przegląd Azure Reservations w programie CSP (2018 maja)

## <a name="operations"></a>Operacje

[Centrum partnerskie — nowy Przewodnik operacji handlowych](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): kompleksowy przewodnik dotyczący najważniejszych zasad i aspektów operacyjnych, takich jak umowy, porządkowanie przez centrum partnerskie, faktury, szczegóły cennika, zachęty, plik uzgadniania, interfejs API/zestaw SDK, piaskownica i udostępnione usługi partnerskie platformy Azure.

## <a name="azure-hybrid-benefit"></a>Korzyść użycia hybrydowego platformy Azure

[Korzyść użycia hybrydowego platformy Azure](https://azure.microsoft.com/pricing/hybrid-benefit) to korzyść cenowa dla klientów korzystających z licencji z programem Software Assurance, która pomaga zmaksymalizować wartość istniejących inwestycji w system Windows Server i/lub SQL Server licencje licencyjne podczas migracji na platformę Azure. Uprawnieni klienci mogą zaoszczędzić do 40% * na platformie Azure Virtual Machines (infrastruktura jako usługa lub IaaS) i zaoszczędzić do 55% na Azure SQL Database (platforma jako usługa lub PaaS) i SQL Server na platformie Azure Virtual Machines (IaaS) z Korzyść użycia hybrydowego platformy Azure, które zwiększają się do 80% w połączeniu z wystąpieniami zarezerwowanymi platformy Azure.

## <a name="next-steps"></a>Następne kroki

- [Często zadawane pytania dotyczące korzyści użycia hybrydowego platformy Azure](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* Rzeczywiste oszczędności mogą różnić się w zależności od regionu, typu wystąpienia lub użycia.