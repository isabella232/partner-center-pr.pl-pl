---
title: Regionalne podatki i opłaty za usługi PSTN
description: Jako partner usługi Office 365, który Microsoft 365 produkty voice, możesz podlegać regionalnym podatkom, opłatom lub wymogom prawnymi w zakresie usług PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854727"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Podatki regionalne, przepisy dotyczące usług publicznej sieci telefonicznej (PTSN)

**Odpowiednie role:** Administrator globalny | Administrator | Agent administracyjny

Usługi publicznej sieci telefonicznej przełączone (PSTN) w niektórych jurysdykcjach mogą podlegać specjalnym wymogom podatkowym i prawnych, które mogą mieć wpływ na zamówienia i fakturowanie partnerów. W tej Stany Zjednoczone, w tym Port Port, usługi PSTN, które obejmują audiokonferencje, plany połączeń i środki komunikacyjne, podlegają specjalnym wymogom podatkowym i prawnych. W witrynie Stany Zjednoczone i PortOryko firma Microsoft ceni usługi PSTN jako nieukońcowe.  Unikatowe podatki i regulacje dotyczące sieci PSTN będą mieć wpływ na partnerów usługi Office 365, którzy Microsoft 365 usługi Voice.  Jeśli partner oznacza cenę usługi Microsoft PSTN, może być odpowiedzialny za obliczanie i remitowanie podatków i opłat PSTN.

## <a name="partner-recommendations"></a>Zalecenia partnerów

Zaangażuj się w przepisy podatkowe i prawne, aby zrozumieć odpowiedzialność organizacji w zakresie regulacji usług PSTN, podatków i opłat oraz innych potencjalnych zobowiązań.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Prezentacja faktury i plik uzgodnień partnera

Faktury CSP i pliki uzgodnień programu CSP w Stany Zjednoczone, Portoryko i Kanadzie, które obejmują usługi Skype dla firm PSTN i Microsoft 365 Voice, będą dostarczać oddzielne pozycje dla składników PSTN i innych niż PSTN.

Ponadto faktury CSP będą wyświetlać następujący przypis:

* Wyświetlana cena to opłata za audiokonferencje i usługi planu połączeń.  Wszelkie odpowiednie podatki transakcyjne są naliczane wyłącznie za kwotę wyświetlaną z wyjątkiem sprzedaży dokonanej w ramach Stany Zjednoczone.  W Stanach Zjednoczonych wyświetlana cena obejmuje podatek, ponieważ obejmuje opłatę za plan połączeń i usługi audiokonferencji oraz opłaty za podatki i opłaty, które są wymagane do nali należności.  Usługi audiokonferencji i planu połączeń są świadczone przez podmiot powiązany z firmą Microsoft autoryzowany do ich świadczenia.  Zobacz [Licencjonowanie zbiorowe firmy Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247), aby uzyskać więcej szczegółów.

## <a name="reconciliation-file-example"></a>Przykład pliku uzgodnień

Usługa Office 365 Enterprise E5 jest przedstawiana w pliku uzgodnień jako dwa elementy wiersza o identycznych nazwach i identycznych identyfikatorach, ale każdy element wiersza ma unikatową cenę jednostkową (na przykład: 28,40 USD i 2,00 USD). Oddzieli to składnik Skype dla firm z konferencji PSTN w ofercie usługi Office 365, dzięki czemu można prawidłowo stosować podatki.

**Przykład uzgadniania partnera #1 (wybieranie kolumn):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Opłata za cykl   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Opłata za cykl   |2,00   |

**Przykład uzgadniania partnera #2**

Usługa Microsoft 365 Business Voice dostępna w Kanadzie ma dodatkowe składniki składowe PSTN, które są konsolidowane na fakturze CSP (podobnie jak w przypadku usługi Office 365 E5, prezentowane są dwa elementy wiersza, jeden dla składników PSTN, a drugi dla składników spoza sieci PSTN).  Plik uzgodnień programu CSP dla usługi Microsoft 365 Business Voice będzie wyświetlać osobno wszystkie składniki pstn (poszczególne składniki PSTN nie zostaną skonsolidowane w programie . Narzędzie CSV lub API).  Suma szczegółów zamówienia i kwot rozlicznych dla klientów znalezionych w pliku uzgodnień będzie odpowiadać fakturze CSP.

## <a name="additional-resources"></a>Dodatkowe zasoby
Aby uzyskać więcej informacji, odwiedź [witrynę Microsoft 365 dla partnerów.](https://www.microsoft.com/microsoft-365/partners/)

