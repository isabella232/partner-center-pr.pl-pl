---
title: Regionalne podatki i opłaty za usługi PSTN
description: Jako partner Office 365, który Microsoft 365 produktów Voice, możesz podlegać regionalnym podatkom, opłatom lub wymogom prawnymi w zakresie usług PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 228534aff70db5c60116d408550361477da7302b784c78ea746cd2ae017c70a0
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691671"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Podatki regionalne, przepisy dotyczące usług publicznej sieci telefonicznej (PTSN)

**Odpowiednie role:** Administrator globalny | Administrator | Agent administracyjny

Usługi publicznej sieci telefonicznej przełączone (PSTN) w niektórych jurysdykcjach mogą podlegać specjalnym wymogom podatkowym i prawnych, które mogą mieć wpływ na zamówienia i fakturowanie partnerów. W tej Stany Zjednoczone, w tym Port Port, usługi PSTN, które obejmują audiokonferencje, plany połączeń i środki komunikacyjne, podlegają specjalnym wymogom podatkowym i prawnych. W witrynie Stany Zjednoczone i PortOryko firma Microsoft ceni usługi PSTN jako nieukońcowe.  Unikatowe podatki i regulacje dotyczące sieci PSTN będą mieć wpływ Office 365 partnerów, którzy Microsoft 365 produkty usługi Voice.  Jeśli partner oznacza cenę usługi Microsoft PSTN, może być odpowiedzialny za obliczanie i remitowanie podatków i opłat PSTN.

## <a name="partner-recommendations"></a>Partner Rekomendacje

Zaangażuj się w przepisy podatkowe i prawne, aby zrozumieć odpowiedzialność organizacji w zakresie regulacji usług PSTN, podatków i opłat oraz innych potencjalnych zobowiązań.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Prezentacja faktury i plik uzgodnień partnera

Dostawca rozwiązań w chmurze (CSP) faktury i pliki uzgodnień programu CSP w usługach Stany Zjednoczone, PortOry i Canada, które obejmują usługi Skype dla firm PSTN i Microsoft 365 Voice, będą dostarczać oddzielne pozycje dla składników PSTN i innych niż PSTN.

Ponadto faktury CSP będą wyświetlać następujący przypis:

* Wyświetlana cena to opłata za audiokonferencje i usługi planu połączeń.  Wszelkie odpowiednie podatki transakcyjne są naliczane wyłącznie za kwotę wyświetlaną z wyjątkiem sprzedaży dokonanej w ramach Stany Zjednoczone.  W Stanach Zjednoczonych wyświetlana cena obejmuje podatek, ponieważ obejmuje opłatę za plan połączeń i usługi audiokonferencji oraz opłaty za podatki i opłaty, które są wymagane do nali należności.  Usługi audiokonferencji i planu połączeń są świadczone przez podmiot powiązany z firmą Microsoft autoryzowany do ich świadczenia.  Zobacz [Licencjonowanie zbiorowe firmy Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247), aby uzyskać więcej szczegółów.

## <a name="reconciliation-file-example"></a>Przykład pliku uzgodnień

Office 365 Enterprise E5 przedstawia plik uzgodnień jako dwa elementy wiersza o identycznych nazwach i identycznych identyfikatorach, ale każdy element wiersza ma unikatową cenę jednostkową (na przykład: 28,40 USD i 2,00 USD). Oddziela to składnik Skype dla firm PSTN w ofercie Office 365, dzięki czemu można prawidłowo stosować podatki.

**Przykład uzgadniania partnera #1 (wybieranie kolumn):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Opłata za cykl   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Opłata za cykl   |2,00   |

**Przykład uzgadniania partnera #2**

Microsoft 365 Business Voice w Kanadzie ma dodatkowe składniki składowe PSTN, które są konsolidowane na fakturze CSP (podobnie jak w przypadku programu Office 365 E5, przedstawiono dwa elementy wiersza, jeden dla składników PSTN i drugi dla składników innych niż PSTN).  Plik uzgodnień programu CSP dla Microsoft 365 Business Voice będzie wyświetlać wszystkie składniki pstn indywidualnie (poszczególne składniki PSTN nie będą konsolidowane w .CSV ani narzędziu interfejsu API).  Suma szczegółów zamówienia i kwot rozlicznych dla klientów znalezionych w pliku uzgodnień będzie odpowiadać fakturze CSP.

## <a name="additional-resources"></a>Dodatkowe zasoby
Aby uzyskać więcej informacji, odwiedź [witrynę Microsoft 365 dla partnerów.](https://www.microsoft.com/microsoft-365/partners/)

