---
title: Rezerwacje platformy Azure & subskrypcje serwera
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o możliwościach dostawcy rozwiązań w chmurze, aby uzyskać, zainicjować i zarządzać rezerwacjami platformy Azure oraz subskrypcjami serwera dla klientów.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529908"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Pozyskiwanie, Inicjowanie obsługi & Zarządzanie wystąpieniami zarezerwowanych maszyn wirtualnych platformy Azure (RI) i subskrypcjami serwera dla klientów

Dotyczy:

- Centrum partnerskie

**Odpowiednie role**

- Agent administracyjny
- Administrator globalny
- Agent pomocy technicznej
- Agent sprzedaży
- Administrator zarządzania użytkownikami

> [!NOTE]
> Ten artykuł ma zastosowanie tylko do partnerów w programie Cloud Solution Provider (CSP). Klienci korzystający z innych rodzajów subskrypcji (na przykład płatność zgodnie z rzeczywistym użyciem, osoby, umowę klienta firmy Microsoft lub subskrypcje Umowa Enterprise) powinni przeczytać [dokumentację dotyczącą zastrzeżeń platformy Azure](/azure/cost-management-billing/reservations).


## <a name="what-are-azure-reservations"></a>Co to jest Azure Reservations?

Azure Reservations pomóc zaoszczędzić pieniądze przez przedpłatę za rok lub trzy lata maszyny wirtualnej, SQL Database pojemność obliczeniowa, Azure Cosmos DB przepływność lub inne zasoby platformy Azure. Funkcja przedpłaty umożliwia uzyskanie rabatu za zasoby, których używasz. Rezerwacje mogą znacząco obniżyć swoją maszynę wirtualną, obliczenia w usłudze SQL Database, Azure Cosmos DB i inne koszty zasobów do 72% w porównaniu z cenami z płatność zgodnie z rzeczywistym użyciem. Rezerwacje umożliwiają skorzystanie z rabatu na rozliczenia i nie mają wpływu na stan środowiska uruchomieniowego Twoich zasobów. Aby uzyskać więcej informacji, zobacz [co to są Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Dlaczego klienci kupują rezerwację?

W przypadku klientów z maszynami wirtualnymi, Azure Cosmos DB lub baz danych SQL, które są uruchamiane przez długi czas, zakup rezerwacji daje im największą opłacalną opcję. Na przykład jeśli klient ciągle uruchamia cztery wystąpienia usługi bez rezerwacji, opłaty są naliczone według stawek płatność zgodnie z rzeczywistym użyciem. Jeśli kupią rezerwację dla tych zasobów, natychmiast uzyskają rabat rezerwacji. Zasoby nie będą już obciążane opłatami według stawek płatności zgodnie z rzeczywistym użyciem.

### <a name="compelling-new-azure-offer-in-csp"></a>Atrakcyjna nowa oferta platformy Azure w programie CSP

Dzięki dołączeniu Azure Reservations i subskrypcji serwera do swojego programu CSP firma Microsoft lepiej umożliwia swoim partnerom rozwiązywanie problemów z coraz większym popytem w celu uzyskania bardziej ekonomicznych rozwiązań do obsługi wysoce przewidywalnych, trwałych obciążeń w chmurze. Program CSP umożliwia partnerom pozyskiwanie, Inicjowanie obsługi i zarządzanie subskrypcjami Azure Reservations i serwera w imieniu klientów komercyjnych za pośrednictwem Centrum partnerskiego firmy Microsoft i Azure Portal.

Oferujemy również partnerów w naszym programie CSP, w których można kupować rezerwacje platformy Azure. Partnerzy programu CSP mogą [kupować rezerwacje platformy Azure w imieniu klienta](azure-reservations-buying.md) lub mogą [zezwolić klientowi na kupowanie własnych rezerwacji](give-customers-permission.md) w ramach wcześniejszej subskrypcji platformy Azure.

Azure Reservations zapewnić klientom elastyczność wirtualizacji dla szerokiego zakresu rozwiązań obliczeniowych, w tym tworzenia i testowania, uruchamiania aplikacji oraz rozszerzania centrum danych.

W [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) na przykład komercyjni klienci mogą teraz zaoszczędzić do 72%, a w przeciwieństwie do cen maszyn wirtualnych z systemem Azure — po prostu przy zakupie lub "obsłużeniu" — w przypadku okresu 1-lub 3-letniego. Klienci korzystający z systemu Windows Server z Korzyść użycia hybrydowego platformy Azure, dostępną w ramach programu Software Assurance, będą mogli zaoszczędzić do 80% w porównaniu z cenami zgodnie z rzeczywistym użyciem.

W przypadku niedopasowanej kombinacji atrakcyjnych cen i niedopasowanej elastyczności wdrożenia klienci będą widzieli najlepszą ogólną wartość, wybierając Azure Reservations:

#### <a name="azure-reservations"></a>Rezerwacje platformy Azure

- Azure Reserved VM Instances
- Rezerwacje bazy danych SQL
- Wystąpienie zarządzane SQL
- Azure Cosmos DB
- Azure SQL Data Warehouse
- App Services
- Azure Databricks rezerwacji jednostek
- Dysk zarządzany
- Blokowy obiekt blob
- MySQL
- Eksplorator danych platformy Azure
- MariaDB
- PostgreSQL

#### <a name="server-subscriptions"></a>Subskrypcje serwera

- Windows Server
- Licencje CAL na Usługi pulpitu zdalnego (RDS)
- SQL Server

#### <a name="linux-isv-annual-subscriptions"></a>Subskrypcje roczne niezależnego dostawcy oprogramowania Linux

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

#### <a name="isv-annual-subscriptions"></a>Subskrypcje roczne niezależnego dostawcy oprogramowania

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>Wprowadzenie

Aby zrozumieć, w jaki sposób można określić, Azure Reservations z klientami oraz jak najszybciej rozpocząć pracę, zalecamy następujące podejście do przeglądu materiałów gotowości:

1. Przejrzyj prezentacje przeglądowe i powiązane seminaria internetowe na potrzeby pozycji i pozycjonowania wartości klienta
2. Przejrzyj i zapoznaj się z współczesnym przewodnikiem operacyjnym handlu
3. Zapoznaj się z tematem często zadawanych subskrypcji na platformę Azure
4. Informacje o aktualizacjach dla Azure Reservations i subskrypcji serwera w [interfejsie API Centrum partnerskiego (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)

## <a name="resources"></a>Zasoby

Poniżej znajduje się kompleksowa Lista zasobów, które ułatwiają szybkie dołączanie do Azure Reservations transakcyjnych w centrum partnerskim:

### <a name="sales-readiness"></a>Gotowość do sprzedaży

- [Azure Reservations i subskrypcje serwera z omówieniem Korzyść użycia hybrydowego platformy Azure](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [Arkusz sprzedaży](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [Często zadawane pytania dla partnerów Azure Reservations](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [Często zadawane pytania dla partnerów dotyczące Azure Reservations i bazy danych SQL](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [Licencja dostępu klienta (CAL) Usługi pulpitu zdalnego (RDS) (anons)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [Azure Reserved VM Instances (Azure Portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [Subskrypcje serwera](csp-software-subscriptions.md)
- [Baza danych SQL na platformie Azure — omówienie](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
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
- Cennik dostawcy usług kryptograficznych **Microsoft Azure: listy zarezerwowanych wystąpień** i cennika usługi **subskrypcje oprogramowania** są dostępne na stronie [& oferty](https://partner.microsoft.com/pcv/sales) Centrum partnerskiego.

### <a name="training"></a>Szkolenia

Zarejestruj się, aby wyświetlić [seminaria internetowe gotowości do licencjonowania komercyjnego](https://commercial-licensing.eventbuilder.com/FY2019_ALL) oraz zdarzenia na żądanie.

Zdarzenia gotowości do licencjonowania na żądanie obejmują tematy takie jak:

- Usługi CSP online, dostawcy CSP Azure i ogólne aktualizacje licencjonowania, w tym Azure (listopad 2018)
- Zarezerwowana pojemność bazy danych SQL & elastyczność rozmiaru wystąpienia (sierpień 2018)
- Subskrypcje serwera w programie CSP (lipiec 2018)
- Przegląd Azure Reservations w programie CSP (2018 maja)

Inne przydatne szkolenia obejmują [moduł licencjonowania platformy Azure na Uniwersytecie dla partnerów](https://aka.ms/azure_partner_licensing).

### <a name="operations"></a>Operacje

- [Współczesny Przewodnik dotyczący operacji handlowych](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (zaktualizowany): kompleksowy przewodnik dotyczący najważniejszych zasad i aspektów operacyjnych, takich jak umowy, porządkowanie przez centrum partnerskie, faktury, szczegóły cennika, zachęty, plik uzgodnienia, interfejs API/zestaw SDK, piaskownica i udostępnione usługi partnera platformy Azure.
- [Współczesne oferty dotyczące dostępności kraju i waluty klienta](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [Sprzedaj Microsoft Azure wystąpienia zarezerwowane](azure-reservations.md)
- [Kup rezerwacje Microsoft Azure w imieniu klientów](azure-reservations-buying.md)
- [Zarządzanie rezerwacjami platformy Azure w imieniu klientów](azure-reservations-manage.md)
- [Rozliczenia dla rezerwacji platformy Azure](azure-plan-billing.md)
- [Rozmiar maszyny wirtualnej dla maksymalnego użycia zastrzeżenia](azure-usage.md)
- [Interfejs API Centrum partnerskiego (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [Usługi pulpitu zdalnego](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a>Korzyść użycia hybrydowego platformy Azure

[Korzyść użycia hybrydowego platformy Azure](https://azure.microsoft.com/pricing/hybrid-benefit) pomaga uzyskać więcej wartości z licencji systemu Windows Server i zaoszczędzić do * 47 procent na maszynach wirtualnych. Możesz korzystać z korzyści z licencji systemu Windows Server Datacenter i Standard Edition, które są objęte programem Software Assurance. W zależności od wersji można przekonwertować licencje lub użyć ich ponownie w celu uruchomienia maszyn wirtualnych z systemem Windows Server na platformie Azure i zaliczyć niższą podstawową stawkę obliczeniową (stawki za maszyny wirtualne z systemem Linux).

Zobacz również [korzyść użycia hybrydowego platformy Azure często zadawane pytania](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* Rzeczywiste oszczędności mogą różnić się w zależności od regionu, typu wystąpienia lub użycia.
