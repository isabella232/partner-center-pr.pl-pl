---
title: Dostęp oparty na rolach usługi Partner Center
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się więcej o określonych rolach wymaganych do wyświetlenia raportów usługi Partner Center Insights. Obejmują one role programu Executive Report Viewer i Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2020
ms.locfileid: "92529669"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Kontrola dostępu oparta na rolach na pulpicie nawigacyjnym usługi Partner Center Insights

Pulpit nawigacyjny usługi Insights używa dwóch nowych ról w centrum partnerskim do zarządzania dostępem pracowników do raportów — programu Executive raportów i raportów.  Użytkownicy w roli programu Executive Report Viewer mają dostęp do wszystkich zestawów danych raportowania, a użytkownicy w roli przeglądarki raportów nie będą mieli dostępu do poufnych zestawów dane, takich jak dochody i dane osobowe dotyczące odbiorców/pracowników.  

Podobnie jak w przypadku innych ról Centrum partnerskiego, Administrator globalny lub administrator konta będzie mógł przypisywać użytkowników do tych ról na stronie Zarządzanie użytkownikami. Role mogą być stosowane w całej firmie lub dla określonych lokalizacji MPN. Role przypisane do określonych lokalizacji MPN ograniczają użytkownika do wyświetlania danych raportowania skojarzonych tylko z wybranymi lokalizacjami MPN. Partner może wybrać jedną lub wiele lokalizacji z poziomu poniższego widoku.

:::image type="content" source="images/pci/roles.png" alt-text="Przedstawia ustawienia ról usługi Partner Center dla konkretnych lokalizacji dla przeglądarki raportów i programu Executive Report Viewer.":::

>[!Note]
> Użytkownicy, którzy są administratorami MPN od dwudziestu 20 stycznia 2020 są automatycznie dodawani do roli programu **Executive Report** w całej firmie dla wszystkich lokalizacji dla tej dzierżawy. Ci użytkownicy mogą w ten sposób uzyskiwać dostęp do raportów w postaci programu Executive Report Viewer bez jawnej akcji wymaganej przez administratora globalnego lub administratora konta. Administratorzy globalni i Administratorzy konta mogą zastąpić automatyczne przypisane role tych użytkowników, aby zwiększyć lub ograniczyć ich możliwości.

## <a name="next-steps"></a>Następne kroki

- Dowiedz się więcej na temat usługi [Partner Center szczegółowe](partner-center-insights.md) informacje i jej różne raporty.
