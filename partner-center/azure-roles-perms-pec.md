---
title: Role, uprawnienia dla partnerów, które uzyskały środki
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej na temat ról i uprawnień dla partnerów, aby mieć możliwość uzyskania kredytów uzyskanych przez partnerów (PEC). Różnią się one od ról do pracy w centrum partnerskim.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/11/2020
ms.locfileid: "92529690"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Role i uprawnienia kwalifikujące się do zdobycia środków uzyskanych przez partnera

Poniższe role mapują do poziomów uprawnień, które określają, czy partner jest uprawniony do korzystania z kredytów uzyskanych przez partnerów.

>[!Important]
>Te role i uprawnienia nie są takie same, jak role i uprawnienia, które użytkownik musi pracować w centrum partnerskim.

|**Role**   |**Opis**   |**Prawo dla PEC**   |
|-----------------|:------------------|:--------------|
|Właściciel  |Wszystko jest zarządzane, w tym dostęp do zasobów.|Tak|
|Współautor |Możesz zarządzać wszystkimi elementami z wyjątkiem udzielania dostępu do zasobów.|Tak|
|Czytelnik|Możesz wyświetlić wszystko, ale nie wprowadzać żadnych zmian|Nie|
|ACRDelete|ACR Usuń|Tak|
|ACRImageSigner|ACR podpisującego obraz|Tak|
|ACRPull|ACR ściągaj|Tak|
|AcrPush|ACR wypychania|Tak|
|AcrQuarantineReader|czytnik danych kwarantanny ACR|Nie|
|AcrQuarantineWriter| składnik zapisywania danych kwarantanny ACR|Tak|
|Współautor usługi API Management|Może zarządzać usługą i interfejsami API|Tak|
|Rola operatora usługi API Management|Może zarządzać usługą, ale nie z interfejsów API|Tak|
|Rola czytnika usługi API Management|Dostęp tylko do odczytu do usługi i interfejsów API|Nie|
|Współautor składnika Application Insights|Zarządza składnikami Application Insights|Tak|
|Application Insights Snapshot Debugger|Daje użytkownikowi uprawnienia do wyświetlania i pobierania migawek debugowania zebranych za pomocą Snapshot Debugger Application Insights. Należy zauważyć, że te uprawnienia nie są uwzględnione w rolach właściciel lub współautor.|Tak|
Operator zadania automatyzacji | Twórz zadania i zarządzaj nimi za pomocą elementów Runbook usługi Automation. | Tak | 
Operator usługi | Operatory automatyzacji mogą uruchamiać, zatrzymywać, wstrzymywać i wznawiać zadania | Tak | 
Operator elementu Runbook usługi Automation | Odczytywanie właściwości elementu Runbook — aby można było tworzyć zadania elementu Runbook. | Tak | 
Współautor avere | Można utworzyć klaster avere vFXT i zarządzać nim. | Tak | 
Operator avere | Używane przez klaster avere vFXT do zarządzania klastrem | Tak | 
Właściciel danych Event Hubs platformy Azure | Umożliwia pełny dostęp do zasobów usługi Azure Event Hubs. | Tak | 
Usługa Azure Event Hubs Data Receiver | Zezwala na odbieranie dostępu do zasobów usługi Azure Event Hubs. | Tak | 
Nadawca danych Event Hubs platformy Azure | Zezwala na wysyłanie dostępu do zasobów Event Hubs platformy Azure. | Tak | 
Rola administratora klastra usługi Kubernetes platformy Azure | Wyświetl listę akcji poświadczeń administratora klastra. | Tak | 
Rola użytkownika klastra usługi Azure Kubernetes Service | Wyświetl listę akcji poświadczeń użytkownika klastra. | Tak | 
Czytnik danych Azure Maps (wersja zapoznawcza) | Przyznaje dostęp do odczytu danych związanych z mapowaniem z konta usługi Azure Maps. | Nie | 
Właściciel danych Azure Service Bus | Umożliwia pełny dostęp do zasobów Azure Service Bus. | Tak | 
Azure Service Bus odbiorca danych | Umożliwia uzyskanie dostępu do zasobów Azure Service Bus. | Tak | 
Nadawca danych Azure Service Bus | Zezwala na dostęp do Azure Service Bus zasobów. | Tak | 
Właściciel rejestracji Azure Stack | Umożliwia zarządzanie rejestracjami Azure Stack. | Tak | 
Współautor kopii zapasowej | Umożliwia zarządzanie usługą kopii zapasowych, ale nie może tworzyć magazynów i zapewniać dostępu innym osobom | Tak | 
Operator kopii zapasowych | Umożliwia zarządzanie usługami kopii zapasowych, z wyjątkiem usuwania kopii zapasowych, tworzenia magazynu i udzielania dostępu innym osobom | Tak | 
Czytnik kopii zapasowych | Może wyświetlać usługi kopii zapasowej, ale nie może wprowadzać zmian | Nie | 
Czytelnik rozliczeń | Zezwala na dostęp do odczytu do danych rozliczeniowych | Nie | 
Współautor BizTalk | Umożliwia zarządzanie usługami BizTalk Services, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Dostęp do węzła elementu członkowskiego łańcucha bloków (wersja zapoznawcza) | Zezwala na dostęp do węzłów składowych łańcucha bloków | Tak | 
Współautor planu | Może zarządzać definicjami planu, ale nie należy ich przypisywać. | Tak | 
Operator planu | Może przypisywać istniejące opublikowane plany, ale nie może tworzyć nowych planów. Uwaga: to działanie działa tylko wtedy, gdy przypisanie zostało wykonane przy użyciu tożsamości zarządzanej przypisanej przez użytkownika. | Tak | 
Współautor punktu końcowego usługi CDN | Może zarządzać punktami końcowymi usługi CDN, ale nie może udzielić dostępu innym użytkownikom. | Tak | 
Czytnik punktu końcowego usługi CDN | Może wyświetlać punkty końcowe usługi CDN, ale nie może wprowadzać zmian. | Nie | 
Współautor profilu CDN | Może zarządzać profilami sieci CDN i ich punktami końcowymi, ale nie może udzielać dostępu innym użytkownikom. | Tak | 
Czytnik profilu CDN | Może wyświetlać profile usługi CDN i ich punkty końcowe, ale nie może wprowadzać zmian. | Nie | 
Współautor klasycznej sieci | Umożliwia zarządzanie sieciami klasycznymi, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Współautor klasycznego konta magazynu | Umożliwia zarządzanie klasycznymi kontami magazynu, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Rola usługi operatora kluczy klasycznego konta magazynu | Operatorzy kluczy klasycznego konta magazynu mogą wyświetlać i ponownie generować klucze na klasycznych kontach magazynu | Tak | 
Współautor klasycznej maszyny wirtualnej | Umożliwia zarządzanie klasycznymi maszynami wirtualnymi, ale nie umożliwia uzyskiwania do nich dostępu, a nie do sieci wirtualnej ani konta magazynu, z którymi są połączone. | Tak | 
Współautor Cognitive Services | Umożliwia tworzenie, odczytywanie, aktualizowanie, usuwanie i zarządzanie kluczami Cognitive Services. | Tak | 
Czytnik danych Cognitive Services (wersja zapoznawcza) | Umożliwia odczytywanie danych Cognitive Services. | Nie | 
Cognitive Services użytkownika | Umożliwia odczytywanie i wyświetlanie listy kluczy Cognitive Services. | Nie | 
Rola czytnika konta Cosmos DB | Może odczytywać Azure Cosmos DB dane konta. Aby zarządzać kontami Azure Cosmos DB, zobacz współautor konta usługi DocumentDB. | Nie | 
Operator Cosmos DB | Umożliwia zarządzanie kontami Azure Cosmos DB, ale nie dostęp do danych w nich. Uniemożliwia dostęp do kluczy konta i parametrów połączenia. | Tak | 
CosmosBackupOperator | Może przesłać żądanie przywracania dla bazy danych Cosmos DB lub kontenera dla konta | Tak | 
Współautor Cost Management | Umożliwia wyświetlanie kosztów i zarządzanie konfiguracją kosztów (np. budżetów, eksportów) | Tak | 
Cost Management czytelnik | Może wyświetlać dane i konfigurację kosztów (np. budżetów, eksportów) | Nie | 
Współautor urządzenie Data Box | Umożliwia zarządzanie wszystko w obszarze usługi urządzenie Data Box z wyjątkiem udzielenia dostępu innym osobom. | Tak | 
urządzenie Data Box czytelnik | Umożliwia zarządzanie usługą urządzenie Data Box, z wyjątkiem tworzenia kolejności lub edytowania szczegółów kolejności i udzielania dostępu innym osobom. | Nie | 
Współautor Data Factory | Twórz fabryki danych i zarządzaj nimi, a także zasobami podrzędnymi. | Tak | 
Data Lake Analytics deweloper | Umożliwia przesyłanie własnych zadań, monitorowanie ich i zarządzanie nimi, ale nie tworzenie ani usuwanie kont Data Lake Analytics. | Tak | 
Przeczyszczanie danych | Można przeczyścić dane analityczne | Tak | 
Użytkownik DevTest Labs | Umożliwia łączenie, uruchamianie, ponowne uruchamianie i zamykanie maszyn wirtualnych w Azure DevTest Labs. | Tak | 
Współautor strefy DNS | Umożliwia zarządzanie strefami i zestawami rekordów DNS w Azure DNS, ale nie pozwala na kontrolowanie dostępu do nich. | Tak | 
Współautor konta DocumentDB | Może zarządzać kontami Azure Cosmos DB. Azure Cosmos DB jest dawniej znany jako DocumentDB. | Tak | 
Współautor EventGrid EventSubscription | Umożliwia zarządzanie operacjami subskrypcji zdarzeń EventGrid. | Tak | 
EventGrid EventSubscription | Umożliwia odczytanie subskrypcji zdarzeń EventGrid. | Nie | 
Operator klastra usługi HDInsight | Umożliwia odczytywanie i modyfikowanie konfiguracji klastrów usługi HDInsight. | Tak | 
Współautor usług domenowych w usłudze HDInsight | Może odczytywać, tworzyć, modyfikować i usuwać operacje związane z usługami domenowymi, które są potrzebne pakiet Enterprise Security usługi HDInsight | Tak | 
Współautor konta systemów inteligentnych | Umożliwia zarządzanie kontami inteligentnych systemów, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Współautor Key Vault | Umożliwia Zarządzanie magazynami kluczy, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Twórca laboratorium | Umożliwia tworzenie i usuwanie zarządzanych laboratoriów z kont laboratorium platformy Azure oraz zarządzanie nimi. | Tak | 
Współautor usługi Log Analytics | Współautor Log Analytics może odczytywać wszystkie dane monitorowania i edytować ustawienia monitorowania. Edytowanie ustawień monitorowania obejmuje dodanie rozszerzenia maszyny wirtualnej do maszyn wirtualnych; Odczytywanie kluczy konta magazynu w celu skonfigurowania kolekcji dzienników z usługi Azure Storage; Tworzenie i Konfigurowanie kont usługi Automation; Dodawanie rozwiązań; i Konfigurowanie diagnostyki platformy Azure dla wszystkich zasobów platformy Azure. | Tak | 
Czytelnik usługi Log Analytics | Log Analytics Reader może wyświetlać i przeszukiwać wszystkie dane monitorowania, a także wyświetlać ustawienia monitorowania, w tym Wyświetlanie konfiguracji diagnostyki platformy Azure na wszystkich zasobach platformy Azure. | Nie | 
Współautor aplikacji logiki | Umożliwia zarządzanie aplikacjami logiki, ale nie umożliwia zmiany dostępu do nich. | Tak | 
Operator aplikacji logiki | Umożliwia odczytywanie, Włączanie i wyłączanie aplikacji logiki, ale nie ich edytowanie ani aktualizowanie. | Tak | 
Rola operatora aplikacji zarządzanej | Umożliwia odczytywanie i wykonywanie akcji dotyczących zasobów aplikacji zarządzanej | Tak | 
Czytnik aplikacji zarządzanych | Umożliwia odczytanie zasobów w zarządzanej aplikacji i zażądanie dostępu JIT. | Nie | 
Współautor tożsamości zarządzanej | Tworzenie, odczytywanie, aktualizowanie i usuwanie tożsamości przypisanej przez użytkownika | Tak | 
Operator tożsamości zarządzanej | Odczytaj i przypisz tożsamość przypisaną przez użytkownika | Tak | 
Współautor grupy zarządzania | Rola współautora grupy zarządzania | Tak | 
Czytelnik grupy zarządzania | Rola czytelnika grupy zarządzania | Nie | 
Współautor monitorowania | Może odczytywać wszystkie dane monitorowania i edytować ustawienia monitorowania. Zobacz też Rozpoczynanie pracy z rolami, uprawnieniami i zabezpieczeniami przy użyciu Azure Monitor. | Tak | 
Wydawca metryk monitorowania | Włącza publikowanie metryk dla zasobów platformy Azure | Tak | 
Czytnik monitorowania | Może odczytywać wszystkie dane monitorowania (metryki, dzienniki itp.). Zobacz też Rozpoczynanie pracy z rolami, uprawnieniami i zabezpieczeniami przy użyciu Azure Monitor. | Nie | 
Współautor sieci | Umożliwia zarządzanie sieciami, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Nowe współautor konta APM Relic | Umożliwia zarządzanie kontami i aplikacjami New Relic Application Performance Management, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Czytnik i dostęp do danych | Umożliwia wyświetlenie wszystkiego, ale nie pozwala na usunięcie ani utworzenie konta magazynu ani zawartego zasobu. Zezwoli również na dostęp do odczytu i zapisu do wszystkich danych znajdujących się na koncie magazynu za pośrednictwem dostępu do kluczy konta magazynu. | Tak | 
Współautor Redis Cache | Umożliwia zarządzanie pamięciami podręcznymi Redis, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Współautor zasad zasobów (wersja zapoznawcza) | Przeglądania Wypełnianie użytkowników z umowy EA z prawami do tworzenia/modyfikowania zasad zasobów, tworzenia biletów pomocy technicznej i odczytywania zasobów/hierarchii. | Tak | 
Współautor kolekcji zadań usługi Scheduler | Umożliwia zarządzanie kolekcjami zadań harmonogramu, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Współautor Search Service | Umożliwia zarządzanie usługami wyszukiwania, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Administrator zabezpieczeń | Tylko w Security Center: mogą wyświetlać zasady zabezpieczeń, wyświetlać Stany zabezpieczeń, edytować zasady zabezpieczeń, wyświetlać alerty i zalecenia, odrzucać alerty i zalecenia | Tak | 
Security Manager (starsza wersja) | Jest to Starsza rola. Zamiast tego użyj administratora zabezpieczeń | Tak | 
Czytelnik zabezpieczeń | Tylko w Security Center: mogą wyświetlać rekomendacje i alerty, wyświetlać zasady zabezpieczeń, wyświetlać Stany zabezpieczeń, ale nie mogą wprowadzać zmian | Nie | 
Współautor Site Recovery | Umożliwia zarządzanie usługą Site Recovery z wyjątkiem tworzenia magazynu i przypisywania ról | Tak | 
Operator Site Recovery | Umożliwia przełączenie w tryb failover i powrót po awarii, ale nie wykonywanie innych operacji zarządzania Site Recovery | Tak | 
Site Recovery czytelnik | Umożliwia wyświetlanie stanu Site Recovery, ale nie wykonywanie innych operacji zarządzania | Nie | 
Współautor konta kotwic przestrzennych | Umożliwia zarządzanie zakotwiczeniami przestrzennymi na Twoim koncie, ale nie ich usuwanie | Tak | 
Właściciel konta zakotwiczeń przestrzennych | Umożliwia zarządzanie zakotwiczeniami przestrzennymi na Twoim koncie, w tym ich usuwanie | Tak | 
Czytnik konta zakotwiczeń przestrzennych | Umożliwia lokalizowanie i odczytywanie właściwości kotwic przestrzennych na Twoim koncie | Nie | 
Współautor bazy danych SQL | Umożliwia zarządzanie bazami danych SQL, ale nie umożliwia uzyskiwania do nich dostępu. Nie można również zarządzać zasadami związanymi z zabezpieczeniami ani ich nadrzędnymi serwerami SQL. | Tak | 
Współautor wystąpienia zarządzanego SQL | Umożliwia zarządzanie wystąpieniami zarządzanymi SQL i wymaganą konfiguracją sieci, ale nie zapewnia dostępu innym osobom. | Tak | 
Menedżer zabezpieczeń SQL | Umożliwia zarządzanie zasadami związanymi z zabezpieczeniami serwerów SQL i baz danych, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Współautor SQL Server | Umożliwia zarządzanie serwerami i bazami danych SQL, ale nie umożliwia uzyskiwania do nich dostępu ani zasad związanych z zabezpieczeniami. | Tak | 
Współautor konta magazynu | Umożliwia zarządzanie kontami magazynu. Zapewnia dostęp do klucza konta, który może służyć do uzyskiwania dostępu do danych za pośrednictwem autoryzacji klucza współużytkowanego. | Tak | 
Rola usługi operatora kluczy konta magazynu | Zezwala na wyświetlanie i ponowne generowanie kluczy dostępu do konta magazynu. | Tak | 
Współautor danych obiektu blob usługi Storage | Odczytuj, zapisuj i usuwaj kontenery i obiekty blob usługi Azure Storage. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Właściciel danych obiektu blob usługi Storage | Zapewnia pełen dostęp do kontenerów obiektów blob i danych usługi Azure Storage, w tym do przypisywania kontroli dostępu POSIX. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Czytelnik danych obiektu blob usługi Storage | Odczytuj i wyświetlaj kontenery usługi Azure Storage oraz obiekty blob. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Nie | 
Delegat obiektów blob magazynu | Pobierz klucz delegowania użytkownika, którego można następnie użyć do utworzenia sygnatury dostępu współdzielonego dla kontenera lub obiektu BLOB podpisanego przy użyciu poświadczeń usługi Azure AD. Aby uzyskać więcej informacji, zobacz Tworzenie skojarzeń zabezpieczeń dla delegowania użytkowników. | Tak | 
Współautor udziału SMB danych w pliku magazynu | Zezwala na dostęp do odczytu, zapisu i usuwania w udziałach plików usługi Azure Storage za pośrednictwem protokołu SMB | Tak | 
Współautor udziału SMB danych w pliku magazynu z podwyższonym poziomem uprawnień | Zezwala na dostęp do odczytu, zapisu, usuwania i modyfikowania uprawnień NTFS w udziałach plików usługi Azure Storage za pośrednictwem protokołu SMB | Tak | 
Czytelnik udziału SMB danych w pliku magazynu | Zezwala na dostęp do odczytu do udziału plików platformy Azure za pośrednictwem protokołu SMB | Nie | 
Współautor danych kolejki magazynu | Odczytuj, zapisuj i usuwaj kolejki usługi Azure Storage oraz wiadomości w kolejce. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Procesor komunikatów danych kolejki magazynu | Wgląd, pobieranie i usuwanie wiadomości z kolejki usługi Azure Storage. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Nadawca komunikatu o danych kolejki magazynu | Dodawanie komunikatów do kolejki usługi Azure Storage. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Czytnik danych kolejki magazynu | Odczytuj i wyświetlaj kolejki usługi Azure Storage oraz wiadomości w kolejce. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Nie | 
Współautor żądania pomocy technicznej | Pozwala tworzyć żądania pomocy technicznej i zarządzać nimi | Tak | 
Współautor Traffic Manager | Umożliwia zarządzanie profilami Traffic Manager, ale nie pozwala na kontrolowanie użytkowników, którzy mają do nich dostęp. | Tak | 
Administrator dostępu użytkowników | Umożliwia zarządzanie dostępem użytkowników do zasobów platformy Azure. | Tak | 
Logowanie administratora maszyny wirtualnej | Wyświetl Virtual Machines w portalu i zaloguj się jako administrator | Tak | 
Współautor maszyny wirtualnej | Umożliwia zarządzanie maszynami wirtualnymi, ale nie dostęp do nich, a nie do sieci wirtualnej ani konta magazynu, z którymi są połączone. | Tak | 
Logowanie użytkownika maszyny wirtualnej | Wyświetl Virtual Machines w portalu i zaloguj się jako zwykły użytkownik. | Tak | 
Współautor planu sieci Web | Umożliwia zarządzanie planami sieci Web dla witryn internetowych, ale nie umożliwia uzyskiwania do nich dostępu. | Tak | 
Współautor witryny sieci Web | Pozwala zarządzać witrynami sieci Web (a nie planami internetowymi), ale nie uzyskiwać do nich dostępu | Tak |
