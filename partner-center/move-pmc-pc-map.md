---
title: Przenoszenie z witryny PMC do Centrum partnerskiego
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zapoznaj się z różnicami między programem PMC i centrum partnerskim w zakresie odnowień, struktury konta, logowania, ról użytkowników, kompetencji i innych.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dae147c45aca27657f1e88b6943279f9771313d6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132999"
---
# <a name="moving-from-partner-membership-center-pmc-to-partner-center"></a>Przeniesienie z Centrum członkostwa partnerów (PMC) do Centrum partnerskiego

**Odpowiednie role**

- Administrator globalny

Ułatwiamy współpracę z firmą Microsoft, wprowadzając pojedynczą witrynę sieci Web (centrum partnerskie), która służy jako centralny punkt zaangażowania. Wszystko, co zostało wykonane w centrum członkostwa partnerów (PMC), można uzyskać z pulpitu nawigacyjnego w centrum partnerskim. 

Możesz również wykonywać wiele innych zadań bez opuszczania jednej witryny sieci Web. Niektóre Terminologia i funkcje mogą wyglądać inaczej. Aby dowiedzieć się, gdzie wykonywać pewne zadania i jakie funkcje są dostępne, należy zapoznać się z informacjami o witrynie na pulpicie nawigacyjnym.

W tej tabeli przedstawiono niektóre różnice między pakietem PMC i centrum partnerskim.

## <a name="renewing-your-microsoft-partner-network--membership"></a>Odnawianie członkostwa Microsoft Partner Network

|**KRYTERIÓW PMC**   |**Centrum partnerskie**|
|----------------------|:-----------------------------|
|Rozpoczęte odnowienia 90 przed rocznicą i muszą zostać ukończone w dniu rocznicy| Partnerzy mogą odnowić dzień po rocznicie i maksymalnie 30 dni po rocznicie.|

## <a name="account-structure"></a>Struktura konta

|**KRYTERIÓW PMC**   |**Centrum partnerskie**|
|----------------------|:-----------------------------|
|Lokalizacja główna i lokalizacje — każdy oceniono osobno. Ocena kompetencji została wykonana na poziomie lokalnym|Jedna firma globalna, konto globalne partnera (PGA), w tym lokalizacje, oceniane jako całość; dane dotyczące wydajności i umiejętności agregowane na poziomie PGA; zawiera kilka widoków profilów dla programów, takich jak Profil partnera i profil biznesowy dla odwołań i marketingu, aby uzyskać więcej informacji Odczytaj [strukturę konta w centrum partnerskim](account-structure.md).|

## <a name="sign-in"></a>Zaloguj

|**KRYTERIÓW PMC**   |**Centrum partnerskie**|
|----------------------|:-----------------------------|
|Może korzystać z poświadczeń konta użytkownika konto Microsoft (MSA) lub osobistych joe@outlook.com|Musisz użyć poświadczeń konta służbowego (na przykład joe@joescompany.com ). Aby uzyskać więcej informacji, Przeczytaj [firmowe konto służbowe i centrum partnerskie](azure-active-directory-tenants-and-partner-center.md).|

## <a name="user-roles"></a>Role użytkownika

|**KRYTERIÓW PMC**   |**Centrum partnerskie**|
|----------------------|:-----------------------------|
|Wiele ról w funkcji PMC nie jest używanych w centrum partnerskim|Administrator, który wykonuje przeniesienie do Centrum partnerskiego, jest automatycznie przypisywany do ról administratorów MPN, administrator konta i odwołania. Następnie mogą przypisywać innych użytkowników do ról użytkownika.|
|Użytkownicy byli zarządzani na poziomie lokalizacji|Użytkownicy są zarządzani na poziomie firmy (PGA), a nie na poziomie lokalizacji. Wyjątkiem jest administrator zachęt, który działa na poziomie lokalizacji.|
|   |Centrum partnerskie ma dwa szerokie zbiory ról: role zarządzające dzierżawą usługi Azure AD oraz role zarządzające firmą firmy. Organizuj role w sposób, który ma sens dla Twojej firmy. Jedna osoba może robić wszystko lub wiele osób może mieć przypisane osobne role i uprawnienia. Aby uzyskać więcej informacji, przeczytaj temat [Przypisywanie ról i uprawnień użytkowników](permissions-overview.md). 

## <a name="how-competencies-and-benefits-are-accounted-for"></a>Jak są uwzględniane kompetencje i korzyści

|**KRYTERIÓW PMC**   |**Centrum partnerskie**|
|----------------------|:-----------------------------|
|Naliczone na lokalizację i zarządzane na lokalizację|Korzyści są przeznaczone dla całej firmy, w tym do administrowania korzyściami, ale możesz zarządzać korzyściami w sposób najlepiej pasujący do Twojej firmy |
|Mogą mieć dodatkowe zalety — zestawy narzędzi (ABTKs), dopóki nie zostaną wycofane w październiku 2018.|Brak ABTKs; jedno mapowanie na firmę; jedno kompetencje Silver na firmę; jedna kwalifikacja złota na firmę|
||Dopóki nie masz jeszcze map, możesz je zakupić. Prawa własności do map nie są powiązane z kompetencjami.  
|Uzyskano dostęp do korzyści z cyfrowego pobrania partnera (PDD) |Dostęp do wszystkich korzyści można uzyskać w centrum partnerskim|
|Kompetencje i korzyści rozdzielone i podzielone między wiele lokalizacji|Twoje kompetencje i korzyści ze wszystkich Twoich lokalizacji są konsolidowane na poziomie firmy (PGA) i będą przechowywane do daty rocznicy. W takim przypadku konieczne będzie zakupienie lub odnowienie na poziomie firmy. Wydajność, umiejętności i kompetencje są agregowane globalnie|
|Oświadczenia dotyczące załączników w ramach programu Software Assurance są wykonywane w narzędziu Walidacja załącznika i wykup (VVR).|Teraz możesz uzyskiwać dostęp do (SATV) i/lub wdrożonych usług planowania (DPS) w centrum partnerskim i zarządzać nimi.  Starsza wersja narzędzia VVR zostanie zlikwidowana 1 października 2019.  |

## <a name="associating-mcp-ids-to-partner-center"></a>Kojarzenie identyfikatorów MCP z centrum partnerskim

|**KRYTERIÓW PMC**   |**Centrum partnerskie**   |
|-------------------------|:-------------------|
|Ten sam identyfikator MCP można skojarzyć z wieloma firmami.| Tylko jeden identyfikator MCP może być skojarzony z jednym kontem Centrum partnerskiego. Należy ręcznie utworzyć skojarzenie. Na pulpicie nawigacyjnym Centrum partnerskiego wybierz ikonę **konta** w prawym rogu pulpitu nawigacyjnego, a następnie wybierz pozycję **mój profil**. W ramach **uczenia** będziesz mieć możliwość skojarzenia Twojego konta Microsoft Learning, a także łączenia konto Microsoft z firmą partnerskią.

## <a name="visual-studio-benefits-and-msa"></a>Zalety programu Visual Studio i MSA

|**KRYTERIÓW PMC**   |**Centrum partnerskie**   |
|-----------------|:-----------------|
|Alokacja korzyści dla programu Visual Studio do MSA|Korzyści wynikające z programu Visual Studio przydzielono do kont MSA i zachowywane.|
||Alokacje MSA programu Visual Studio zostaną zachowane po odnowieniu w centrum partnerskim.|
||W centrum partnerskim partner może dodawać konta służbowe i konta użytkowników-Gości z tej samej dzierżawy, w której partner jest MPN administratorem w dzierżawie usługi Azure AD. Jeśli partner jest administratorem globalnym w wielu dzierżawach usługi Azure AD, a wszystkie te dzierżawy są skojarzone z tym samym kontem Centrum partnerskiego, partner może dodawać użytkowników we wszystkich dzierżawach do korzyści z programu Visual Studio i alokacji opartych na platformie Azure. Użytkownicy-Goście mogą mieć przypisane subskrypcje programu Visual Studio oparte na użyciu przez administratora MPN lub administratora globalnego, ale użytkownicy-Goście nie mogą zalogować się do Centrum partnerskiego za pomocą swojego konta MSA. Użytkownicy-Goście mogą jednak zalogować się do platformy Azure i programu Visual Studio, aby sprawdzić poprawność i korzystać z przypisanych im korzyści. |

## <a name="programs-now-located-and-managed-in-partner-center"></a>Programy zlokalizowane teraz i zarządzane w centrum partnerskim 

|**KRYTERIÓW PMC**   |**Centrum partnerskie**|
|----------------------|:-----------------------------|
|PDD  |Korzyści|
|MIKROUKŁAD, ICP, KOŁOWY | Zachęty|
||Polecenia|
|Szczegółowe informacje o partnerze| Analiza|
|Walidacja załącznika i narzędzie do wykupu| Walidacja załącznika i narzędzie do wykupu|
|           |Programy dostawcy rozwiązań w chmurze|

Korzyści wynikające z programu Visual Studio przydzielono do kont MSA i zachowywane. Zostaną one również zachowane po odnowieniu w centrum partnerskim. Jeśli jednak usuniesz alokację MSA po migracji w centrum partnerskim, nie będzie można jej dodać z powrotem do Centrum partnerskiego.

W centrum partnerskim partner może dodawać konta służbowe i konta użytkowników-Gości z tej samej dzierżawy, w której partner jest MPN administratora w dzierżawie usługi Azure AD. Jeśli partner jest administratorem globalnym w wielu dzierżawach usługi Azure AD, a wszystkie te dzierżawy są skojarzone z tym samym kontem Centrum partnerskiego, partner może dodawać użytkowników we wszystkich dzierżawach do korzyści z programu Visual Studio i alokacji opartych na platformie Azure.

Użytkownicy-Goście mogą mieć przypisane subskrypcje programu Visual Studio oparte na użyciu przez administratora MPN lub administratora globalnego, ale użytkownicy-Goście nie mogą zalogować się do Centrum partnerskiego za pomocą swojego konta MSA. Użytkownicy-Goście mogą jednak zalogować się do platformy Azure i programu Visual Studio, aby sprawdzić poprawność i korzystać z przypisanych im korzyści.
