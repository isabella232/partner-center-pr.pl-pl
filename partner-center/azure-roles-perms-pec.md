---
title: Role, uprawnienia do środków uzyskane przez partnerów
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Dowiedz się więcej o rolach i uprawnieniach partnerów, aby mogli zdobywać środki uzyskane przez partnerów. Różnią się one od ról, które mają być Partner Center.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957886"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Role i uprawnienia wymagane do zdobywania środków uzyskane przez partnerów

Poniższe role są mapowe na poziomy uprawnień, które określają, czy partner kwalifikuje się do środków uzyskane przez partnera.

>[!Important]
>Te role i uprawnienia nie są takie same jak role i uprawnienia, których użytkownik potrzebuje do pracy w Partner Center.

|**Role**   |**Opis**   |**Kwalifikowanie się do PEC**   |
|-----------------|:------------------|:--------------|
|Właściciel  |Zarządzasz wszystkim, w tym dostępem do zasobów.|Tak|
|Współautor |Zarządzasz wszystkim poza udzielaniem dostępu do zasobów.|Tak|
|Czytelnik|Możesz wyświetlić wszystko, ale nie wprowadzać żadnych zmian|Nie|
|ACRDelete|acr delete|Tak|
|ACRImageSigner|acr image signer|Tak|
|ACRPull|ściąganie acr|Tak|
|AcrPush|acr push|Tak|
|AcrQuarantineReader|Czytnik danych kwarantanny acr|Nie|
|AcrQuarantineWriter| ACR kwarantanny zapisujący danych|Tak|
|API Management współautora usługi|Może zarządzać usługą i interfejsami API|Tak|
|API Management operator usługi|Może zarządzać usługą, ale nie interfejsami API|Tak|
|API Management roli czytelnika usługi|Dostęp tylko do odczytu do usługi i interfejsów API|Nie|
|Współautor Szczegółowe informacje aplikacji|Zarządza składnikami Szczegółowe informacje aplikacji|Tak|
|Aplikacje Szczegółowe informacje Snapshot Debugger|Daje użytkownikowi uprawnienia do wyświetlania i pobierania migawek debugowania zebranych za pomocą usługi Application Szczegółowe informacje Snapshot Debugger. Należy pamiętać, że te uprawnienia nie są uwzględnione w rolach Właściciel ani Współautor.|Tak|
Operator zadania usługi Automation | Tworzenie zadań i zarządzanie nimi przy użyciu automatyzacji runbook. | Tak | 
Operator usługi | Operatorzy automatyzacji mogą uruchamiać, zatrzymywać, wstrzymywać i wznawiać zadania | Tak | 
Automation Runbook Operator | Odczytywanie właściwości runbook — aby móc tworzyć zadania tego typu. | Tak | 
Współautor Avere | Może tworzyć klastry Avere vFXT zarządzać nimi. | Tak | 
Avere, operator | Używany przez klaster Avere vFXT do zarządzania klastrem | Tak | 
Azure Event Hubs właściciela danych | Umożliwia pełny dostęp do Azure Event Hubs zasobów. | Tak | 
Azure Event Hubs Data Receiver | Umożliwia odbieranie dostępu do Azure Event Hubs zasobów. | Tak | 
Azure Event Hubs nadawcy danych | Umożliwia wysyłanie dostępu do Azure Event Hubs zasobów. | Tak | 
Azure Kubernetes Service roli administratora klastra | Lista akcji poświadczeń administratora klastra. | Tak | 
Azure Kubernetes Service roli użytkownika klastra | Lista akcji poświadczeń użytkownika klastra. | Tak | 
Czytnik danych usługi Azure Mapy (wersja zapoznawcza) | Udziela dostępu do odczytu danych związanych z mapą z konta usługi Azure Maps. | Nie | 
Właściciel Service Bus platformy Azure | Umożliwia pełny dostęp do zasobów usługi Azure Service Bus zasobów. | Tak | 
Azure Service Bus Data Receiver | Umożliwia odbieranie dostępu do zasobów usługi Azure Service Bus zasobów. | Tak | 
Azure Service Bus Data Sender | Umożliwia wysyłanie dostępu do zasobów usługi Azure Service Bus zasobów. | Tak | 
Azure Stack właściciela rejestracji | Umożliwia zarządzanie Azure Stack rejestracji. | Tak | 
Współautor kopii zapasowej | Umożliwia zarządzanie usługą tworzenia kopii zapasowych, ale nie pozwala na tworzenie magazynów i zapewnianie dostępu innym osobom | Tak | 
Operator kopii zapasowych | Umożliwia zarządzanie usługami kopii zapasowych z wyjątkiem usuwania kopii zapasowej, tworzenia magazynu i nadawania dostępu innym osobom | Tak | 
Czytelnik kopii zapasowych | Może wyświetlać usługi tworzenia kopii zapasowych, ale nie może wprowadzać zmian | Nie | 
Czytelnik rozliczeń | Zezwala na dostęp do odczytu danych rozliczeń | Nie | 
Współautor BizTalk | Umożliwia zarządzanie usługami BizTalk, ale nie umożliwia dostępu do nich. | Tak | 
Dostęp do węzła członkowskiego łańcucha bloków (wersja zapoznawcza) | Umożliwia dostęp do węzłów członkowskich łańcucha bloków | Tak | 
Współautor strategii | Może zarządzać definicjami strategii, ale nie może ich przypisywać. | Tak | 
Operator strategii | Może przypisywać istniejące opublikowane strategie, ale nie może tworzyć nowych strategii. UWAGA: działa to tylko wtedy, gdy przypisanie jest wykonywane przy użyciu tożsamości zarządzanej przypisanej przez użytkownika. | Tak | 
CDN Współautor punktu końcowego | Może zarządzać CDN końcowymi, ale nie może udzielać dostępu innym użytkownikom. | Tak | 
CDN Czytelnik punktu końcowego | Może wyświetlać CDN końcowe, ale nie może wprowadzać zmian. | Nie | 
CDN Współautor profilu | Może zarządzać CDN i ich punktami końcowymi, ale nie może udzielać dostępu innym użytkownikom. | Tak | 
CDN Czytelnik profilu | Może wyświetlać CDN i ich punkty końcowe, ale nie może wprowadzać zmian. | Nie | 
Współautor klasycznej sieci | Umożliwia zarządzanie sieciami klasycznymi, ale nie umożliwia dostępu do nich. | Tak | 
Współautor Storage klasycznego konta | Umożliwia zarządzanie klasycznymi kontami magazynu, ale nie umożliwia dostępu do nich. | Tak | 
Rola usługi Storage operator klucza konta klasycznego | Operatorzy Storage konta klasycznego mogą wyświetlić listę i ponownie wygenerować klucze na klasycznych kontach Storage kont | Tak | 
Współautor klasycznej maszyny wirtualnej | Umożliwia zarządzanie klasycznymi maszynami wirtualnymi, ale nie dostęp do nich, a nie sieci wirtualnej ani konta magazynu, z które są połączone. | Tak | 
Cognitive Services współautora | Umożliwia tworzenie, odczytywanie, aktualizowanie i usuwanie kluczy usługi Cognitive Services. | Tak | 
Cognitive Services czytnik danych (wersja zapoznawcza) | Umożliwia odczytywanie Cognitive Services danych. | Nie | 
Cognitive Services użytkownika | Umożliwia odczytywanie i wyświetlanie listy kluczy Cognitive Services. | Nie | 
Cosmos Rola czytelnika konta bazy danych | Może odczytywać dane konta usługi Azure Cosmos DB. Aby zarządzać kontami usługi Azure Cosmos DB, zobacz Współautor konta usługi DocumentDB. | Nie | 
Cosmos Operator bazy danych | Umożliwia zarządzanie kontami usługi Azure Cosmos DB, ale nie umożliwia dostępu do danych w nich. Uniemożliwia dostęp do kluczy konta i parametry połączenia. | Tak | 
CosmosBackupOperator | Może przesłać żądanie przywrócenia dla bazy Cosmos DB lub kontenera dla konta | Tak | 
Współautor zarządzania kosztami | Może wyświetlać koszty i zarządzać konfiguracją kosztów (np. budżetami, eksportami) | Tak | 
Cost Management czytelnika | Może wyświetlać dane dotyczące kosztów i konfigurację (np. budżety, eksporty) | Nie | 
urządzenie Data Box współautora | Umożliwia zarządzanie wszystkim w obszarze urządzenie Data Box Service z wyjątkiem dawania dostępu innym osobom. | Tak | 
urządzenie Data Box czytelnika | Umożliwia zarządzanie usługą urządzenie Data Box z wyjątkiem tworzenia zamówienia lub edytowania szczegółów zamówienia i nadawania dostępu innym osobom. | Nie | 
Data Factory współautora | Tworzenie fabryk danych, a także zasobów podrzędnych w tych fabrykach i zarządzanie nimi. | Tak | 
Data Lake Analytics Deweloper | Umożliwia przesyłanie i monitorowanie własnych zadań oraz zarządzanie nimi, ale nie pozwala na tworzenie ani Data Lake Analytics kont. | Tak | 
Przeczyszczania danych | Może przeczyścić dane analityczne | Tak | 
Użytkownik laboratorium DevTest Labs | Umożliwia łączenie, uruchamianie, ponowne uruchamianie i zamykanie maszyn wirtualnych w Azure DevTest Labs. | Tak | 
Współautor strefy DNS | Umożliwia zarządzanie strefami DNS i zestawami rekordów w Azure DNS, ale nie pozwala na kontrolowanie, kto ma do nich dostęp. | Tak | 
Współautor konta bazy danych DocumentDB | Może zarządzać kontami usługi Azure Cosmos DB. Usługa Azure Cosmos DB jest wcześniej znana jako DocumentDB. | Tak | 
EventGrid , współautor subskrypcji zdarzeń | Umożliwia zarządzanie operacjami subskrypcji zdarzeń usługi EventGrid. | Tak | 
EventGrid EventSubscription Reader | Umożliwia odczytywanie subskrypcji zdarzeń usługi EventGrid. | Nie | 
Operator klastra usługi HDInsight | Umożliwia odczytywanie i modyfikowanie konfiguracji klastra usługi HDInsight. | Tak | 
Współautor usług HDInsight Domain Services | Może odczytywać, tworzyć, modyfikować i usuwać operacje związane z usługami Domain Services potrzebne dla pakietu zabezpieczeń Enterprise HDInsight | Tak | 
Współautor konta systemów inteligentnych | Umożliwia zarządzanie kontami systemów inteligentnych, ale nie umożliwia dostępu do nich. | Tak | 
Key Vault współautora | Umożliwia zarządzanie magazynami kluczy, ale nie umożliwia dostępu do nich. | Tak | 
Twórca laboratorium | Umożliwia tworzenie i usuwanie laboratoriów zarządzanych oraz zarządzanie nimi w ramach kont laboratorium platformy Azure. | Tak | 
Współautor usługi Log Analytics | Współautor usługi Log Analytics może odczytywać wszystkie dane monitorowania i edytować ustawienia monitorowania. Edytowanie ustawień monitorowania obejmuje dodawanie rozszerzenia maszyny wirtualnej do maszyn wirtualnych; odczytywanie kluczy konta magazynu w celu skonfigurowania zbierania dzienników z usługi Azure Storage; tworzenie i konfigurowanie kont usługi Automation; dodawanie rozwiązań; i konfigurowanie diagnostyki platformy Azure dla wszystkich zasobów platformy Azure. | Tak | 
Czytelnik usługi Log Analytics | Czytelnik usługi Log Analytics może wyświetlać i przeszukiwać wszystkie dane monitorowania, a także wyświetlać ustawienia monitorowania, w tym wyświetlać konfigurację diagnostyki platformy Azure dla wszystkich zasobów platformy Azure. | Nie | 
Współautor aplikacji logiki | Umożliwia zarządzanie aplikacjami logiki, ale nie zmienia dostępu do nich. | Tak | 
Operator aplikacji logiki | Umożliwia odczytywanie, włączanie i wyłączanie aplikacji logiki, ale nie ich edytowanie ani aktualizowanie. | Tak | 
Rola operatora aplikacji zarządzanej | Umożliwia odczytywanie i wykonywanie akcji w zasobach aplikacji zarządzanej | Tak | 
Czytelnik aplikacji zarządzanych | Umożliwia odczytywanie zasobów w aplikacji zarządzanej i żądanie dostępu JIT. | Nie | 
Współautor tożsamości zarządzanej | Tworzenie, odczytywanie, aktualizowanie i usuwanie tożsamości przypisanej przez użytkownika | Tak | 
Operator tożsamości zarządzanej | Odczytywanie i przypisywanie tożsamości przypisanej przez użytkownika | Tak | 
Współautor grupy zarządzania | Rola współautora grupy zarządzania | Tak | 
Czytelnik grupy zarządzania | Rola czytelnika grupy zarządzania | Nie | 
Współautor monitorowania | Może odczytywać wszystkie dane monitorowania i edytować ustawienia monitorowania. Zobacz też Wprowadzenie do ról, uprawnień i zabezpieczeń z Azure Monitor. | Tak | 
Monitorowanie metryk Publisher | Umożliwia publikowanie metryk dotyczących zasobów platformy Azure | Tak | 
Czytelnik monitorowania | Może odczytywać wszystkie dane monitorowania (metryki, dzienniki itp.). Zobacz też Wprowadzenie do ról, uprawnień i zabezpieczeń z Azure Monitor. | Nie | 
Współautor sieci | Umożliwia zarządzanie sieciami, ale nie zapewnia do nich dostępu. | Tak | 
New Relic współautora konta APM | Umożliwia zarządzanie kontami New Relic Application Performance Management i aplikacjami, ale nie umożliwia dostępu do nich. | Tak | 
Czytelnik i dostęp do danych | Umożliwia wyświetlenie wszystkiego, ale nie pozwala na usunięcie ani utworzenie konta magazynu ani zawartego zasobu. Umożliwi to również dostęp do odczytu/zapisu do wszystkich danych zawartych na koncie magazynu za pośrednictwem dostępu do kluczy konta magazynu. | Tak | 
Redis Cache współautora | Umożliwia zarządzanie pamięciami podręcznmi Redis Cache, ale nie umożliwia dostępu do nich. | Tak | 
Współautor zasad zasobów (wersja zapoznawcza) | (Wersja zapoznawcza) Wypełnianie użytkowników z ea z uprawnieniami do tworzenia/modyfikowania zasad zasobów, tworzenia biletu pomocy technicznej i odczytywania zasobów/hierarchii. | Tak | 
Współautor kolekcji zadań harmonogramu | Umożliwia zarządzanie kolekcjami zadań harmonogramu, ale nie umożliwia dostępu do nich. | Tak | 
Współautor usługi wyszukiwania | Umożliwia zarządzanie usługami wyszukiwania, ale nie umożliwia dostępu do nich. | Tak | 
Administrator zabezpieczeń | Tylko Security Center: może wyświetlać zasady zabezpieczeń, wyświetlać stany zabezpieczeń, edytować zasady zabezpieczeń, wyświetlać alerty i zalecenia, odrzucać alerty i zalecenia | Tak | 
Menedżer zabezpieczeń (starsza wersja) | Jest to starsza rola. Zamiast tego użyj administratora zabezpieczeń | Tak | 
Czytelnik zabezpieczeń | Tylko Security Center: może wyświetlać zalecenia i alerty, wyświetlać zasady zabezpieczeń, wyświetlać stany zabezpieczeń, ale nie może wprowadzać zmian | Nie | 
Współautor usługi Site Recovery | Umożliwia zarządzanie usługą Site Recovery z wyjątkiem tworzenia magazynu i przypisywania ról | Tak | 
Operator usługi Site Recovery | Umożliwia trybu failover i powrotu po awarii, ale nie wykonuje innych Site Recovery zarządzania | Tak | 
Czytelnik usługi Site Recovery | Umożliwia wyświetlanie stanu Site Recovery, ale nie wykonywanie innych operacji zarządzania | Nie | 
Spatial Anchors współautora konta | Umożliwia zarządzanie zakotwiczeniami przestrzenni na koncie, ale nie ich usuwanie | Tak | 
Spatial Anchors właściciela konta | Umożliwia zarządzanie zakotwiczeniami przestrzenni na koncie, w tym ich usuwanie | Tak | 
Spatial Anchors konta | Umożliwia lokalizowanie i odczytywanie właściwości kotwic przestrzennych na koncie | Nie | 
SQL Współautor bazy danych | Umożliwia zarządzanie bazami SQL, ale nie dostęp do nich. Ponadto nie można zarządzać zasadami związanymi z zabezpieczeniami ani ich nadrzędnymi serwerami SQL zabezpieczeń. | Tak | 
SQL Współautor wystąpienia zarządzanego | Umożliwia zarządzanie SQL wystąpieniami zarządzanymi i wymaganą konfiguracją sieci, ale nie może udzielać dostępu innym osobom. | Tak | 
Menedżer zabezpieczeń SQL | Umożliwia zarządzanie zasadami dotyczącymi zabezpieczeń serwerów SQL baz danych, ale nie ma do nich dostępu. | Tak | 
SQL Server Współautorów | Umożliwia zarządzanie serwerami SQL bazami danych, ale nie dostępem do nich, a nie ich zasadami związanymi z zabezpieczeniami. | Tak | 
Współautor konta magazynu | Umożliwia zarządzanie kontami magazynu. Zapewnia dostęp do klucza konta, który może służyć do uzyskiwania dostępu do danych za pośrednictwem autoryzacji klucza wspólnego. | Tak | 
Storage Rola usługi operatora klucza konta | Zezwala na wyświetlanie i ponowne generowanie kluczy dostępu do konta magazynu. | Tak | 
Współautor danych obiektu blob usługi Storage | Odczyt, zapis i usuwanie kontenerów i obiektów blob Storage Azure. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Właściciel danych obiektu blob usługi Storage | Zapewnia pełny dostęp do kontenerów i Storage obiektów blob platformy Azure, w tym do przypisywania kontroli dostępu POSIX. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Czytelnik danych obiektu blob usługi Storage | Odczyt i lista kontenerów Storage Azure i obiektów blob. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Nie | 
Storage Delegat obiektów blob | Pobierz klucz delegowania użytkownika, którego następnie można użyć do utworzenia sygnatury dostępu współdzielonych dla kontenera lub obiektu blob podpisanego przy użyciu poświadczeń usługi Azure AD. Aby uzyskać więcej informacji, zobacz Tworzenie sygnatury dostępu współdzielonego delegowania użytkownika. | Tak | 
Współautor udziału SMB danych w pliku magazynu | Umożliwia dostęp do odczytu, zapisu i usuwania w udziałach plików usługi Azure Storage za pośrednictwem SMB | Tak | 
Współautor udziału SMB danych w pliku magazynu z podwyższonym poziomem uprawnień | Umożliwia odczyt, zapis, usuwanie i modyfikowanie dostępu do uprawnień NTFS w udziałach plików usługi Azure Storage za pośrednictwem SMB | Tak | 
Czytelnik udziału SMB danych w pliku magazynu | Umożliwia dostęp do odczytu do udziału plików platformy Azure za pośrednictwem SMB | Nie | 
Storage Współautor danych kolejki | Odczyt, zapis i usuwanie usługi Azure Storage kolejek i komunikatów w kolejce. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Storage Procesor komunikatów danych kolejki | Podgląd, pobieranie i usuwanie komunikatu z kolejki usługi Azure Storage kolejki. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Storage Nadawca komunikatów o danych w kolejce | Dodawanie komunikatów do kolejki usługi Azure Storage Azure. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Tak | 
Storage Czytnik danych kolejki | Odczyt i lista kolejek i komunikatów Storage Azure. Aby dowiedzieć się, które akcje są wymagane dla danej operacji danych, zobacz Uprawnienia do wywoływania operacji na danych obiektów blob i kolejek. | Nie | 
Współautor żądania pomocy technicznej | Umożliwia tworzenie żądań pomocy technicznej i zarządzanie nimi | Tak | 
Traffic Manager Współautorów | Umożliwia zarządzanie profilami Traffic Manager, ale nie pozwala na kontrolowanie, kto ma do nich dostęp. | Tak | 
Administrator dostępu użytkowników | Umożliwia zarządzanie dostępem użytkowników do zasobów platformy Azure. | Tak | 
Logowanie administratora maszyny wirtualnej | Wyświetlanie Virtual Machines w portalu i logowanie się jako administrator | Tak | 
Współautor maszyny wirtualnej | Umożliwia zarządzanie maszynami wirtualnymi, ale nie dostęp do nich, a nie sieci wirtualnej ani konta magazynu, z które są połączone. | Tak | 
Logowanie użytkownika maszyny wirtualnej | Wyświetl Virtual Machines w portalu i zaloguj się jako zwykły użytkownik. | Tak | 
Współautor planu sieci Web | Umożliwia zarządzanie planami internetowymi witryn internetowych, ale nie umożliwia dostępu do nich. | Tak | 
Współautor witryny internetowej | Umożliwia zarządzanie witrynami internetowymi (nie planami internetowymi), ale nie umożliwia dostępu do nich | Tak |

## <a name="next-steps"></a>Następne kroki

- [Środków uzyskane przez partnerów — omówienie sposobu ich działania w nowym doświadczeniu handlowym w programie CSP](partner-earned-credit.md)
