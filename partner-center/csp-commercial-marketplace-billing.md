---
title: Rozliczenia dla komercyjnych produktów Marketplace
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dowiedz się, jak działa rozliczenia dla niezależnych dostawców oprogramowania SaaS produkty lub subskrypcje kupione dla klientów z portalu komercyjnego w centrum partnerskim.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10592c7f8a3b1f075bc726161603859552b29961
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979536"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Rozliczanie za komercyjne produkty i subskrypcje w witrynie Marketplace w centrum partnerskim


**Odpowiednie role**

- Administrator globalny
- Administrator rozliczeń

Jako partner w programie CSP możesz użyć Centrum partnerskiego, aby kupić produkty SaaS oparte na licencjach od wydawców niezależnych dostawców oprogramowania w portalu komercyjnym. Po wykonaniu tej czynności możesz uzyskać dostęp do rachunku za te typy zakupów. Okres rozliczeniowy zaczyna się pierwszego dnia miesiąca kalendarzowego i zostaje zakończony ostatni dzień miesiąca kalendarzowego. Faktury są udostępniane w dniu ósmego dnia następnego miesiąca.

Możesz uzyskiwać dostęp do faktur z poziomu [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego lub [interfejsów API Centrum partnerskiego](/partner-center/develop/).

W przypadku partnerów w programie CSP są naliczane opłaty za komercyjne rozwiązania w portalu Marketplace, które zostały nabyte dla klienta, gdy kupują te produkty z poziomu Centrum partnerskiego lub z Azure Portal (przy użyciu wcześniejszej, zakupionej przez dostawcę CSP dzierżawy platformy Azure).

>[!NOTE]
>Jeśli klienci korzystają z własnej dzierżawy usługi Azure AD (nie zakupionej od partnera w programie CSP), klienci mogą również zakupić własne rozwiązanie SaaS niezależnego dostawcy oprogramowania ([Microsoft AppSource](https://appsource.microsoft.com/) lub [Azure Marketplace](https://azuremarketplace.microsoft.com/)). W takim przypadku otrzymają własny rachunek bezpośrednio od firmy Microsoft. Podobnie, jeśli Partner w programie CSP sprzedaje subskrypcję platformy Azure lub nowy plan platformy Azure dla klienta i przyzna klientowi (lub pośredniemu odsprzedawcy) [dostęp](/azure/role-based-access-control/built-in-roles) do tej dzierżawy (przypisując rolę do klienta oprócz **czytnika**), ten klient (lub pośredni odsprzedawca) może także zakupić komercyjne oferty rynkowe bez wcześniejszego zatwierdzenia lub powiadomienia do partnera CSP. W takich przypadkach firma Microsoft nie będzie bezpośrednio powiadamiać partnerów w programie CSP o zakupach dokonywanych przez ich klientów. Firma Microsoft oferuje jednak opcjonalny mechanizm [Azure monitor](/azure/azure-monitor/platform/alerts-activity-log) , którego można użyć do ustawiania alertów lub powiadomień dotyczących aktywności w ramach subskrypcji platformy Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Dostęp do informacji dotyczących rozliczeń dla komercyjnych produktów Marketplace

Administrator globalny lub administrator rozliczeń dla Twojej firmy otrzyma wiadomość e-mail, gdy faktura będzie gotowa do wyświetlenia. Aby uzyskać dostęp do najnowszej faktury i pliku uzgadniania dla komercyjnych zakupów produktów Marketplace:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/)Centrum partnerskiego.

2. W menu Centrum partnerskiego wybierz pozycję **rozliczenia**. 

    Zobaczysz dwie karty w górnej części strony rozliczenia: **cykliczne** i **cykliczne oraz jednorazowe zakupy**. Każda karta umożliwia dostęp do plików fakturowania i uzgadniania (Rekonesans) dla różnych produktów Marketplace:

    - Karta **cykliczna** : zawiera pliki faktury i uzgodnienia dla subskrypcji związanych z pakietem Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro i Microsoft Azure.

    - Karta **cykliczne i jednorazowe zakupy** : pokazuje pliki faktury i uzgodnienia dla usługi Azure plan, rezerwacje platformy Azure, oprogramowanie i komercyjne produkty Marketplace.
  
3. Wybierz kartę **cykliczne i jednorazowe zakupy** . W przypadku zakupu subskrypcji dla klienta w innej walucie zostanie wyświetlona karta dla każdej waluty. Na tej stronie można wykonać kilka czynności:

    - Aby wyświetlić najnowsze faktury i plik uzgadniania, wybierz pozycję **Faktura** lub **plik uzgadniania**. (Jeśli chcesz, możesz również uzyskać dostęp do najnowszych danych z faktury i pliku Rekonesans przy użyciu [interfejsów API Centrum partnerskiego](/partner-center/develop/).

    - Aby wyświetlić wcześniejsze faktury i pliki Rekonesans, rozwiń wiersz **historia rozliczeń** poniżej.

    - Aby sprawdzić szacowane saldo konta lub rozliczanie w dowolnym momencie na podstawie ostatniego działania konta, wybierz link poniżej nagłówka **oszacowań** .  

    >[!NOTE]
    > Po wystawieniu rachunku na ósmy dzień miesiąca będzie uwzględniać podatki oraz inne stosowne opłaty i kredyty. Oznacza to, że ostateczna kwota może różnić się od tego, co widzisz w okresie rozliczeniowym.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Więcej informacji na temat faktur i plików Rekonesans dla komercyjnych produktów Marketplace

Ta sekcja zawiera więcej informacji na temat faktur i plików uzgadniania dla komercyjnych subskrypcji SaaS w portalu Marketplace zakupionych dla klientów od niezależnych dostawców oprogramowania.

Po wybraniu opcji **cykliczne i jednorazowe zakupy** w obszarze **rozliczenia** w menu Centrum partnerskiego uzyskasz dostęp do faktur i plików uzgadniania pod kątem opłat związanych z zakupami firmy Microsoft (pierwszej firmy) i niezależnego dostawcy oprogramowania (innych firm). Te zakupy można kojarzyć z:

- SaaS subskrypcje (od wydawców firmy Microsoft lub niezależnych dostawców oprogramowania)

- Plan platformy Azure

- Rezerwacje platformy Azure

- Inne oprogramowanie oparte na subskrypcji (od wydawców firmy Microsoft lub niezależnego dostawcy oprogramowania)

Przykłady tych zakupów mogą obejmować oprogramowanie SUSE Linux (subskrypcję oprogramowania) lub subskrypcję produktu Azure ISV SaaS.

>[!NOTE]
> Aby uzyskać więcej informacji o sposobie odczytywania plików faktur i Rekonesans, zobacz też [Omówienie rozliczeń](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Porady dotyczące odczytywania faktury

W przypadku zakupu produktu SaaS opartego na licencji od wydawcy niezależnego dostawcy oprogramowania będą wyświetlane opłaty za licencję na fakturę. Jest to prawdziwe nawet wtedy, gdy produkt SaaS (lub zużywa) podstawowe zasoby infrastruktury platformy Azure. Wynika to z faktu, że opłaty za użycie infrastruktury platformy Azure klienta dla produktu SaaS niezależnego dostawcy oprogramowania są naliczane bezpośrednio do niezależnego dostawcy oprogramowania. (Niezależni dostawcy oprogramowania będą widzieli powiązane opłaty za użycie platformy Azure we własnym pliku uzgadniania faktur dziennych za korzystanie z platformy Azure).

Faktura będzie zawierać kilka stron:

- **Strona 1 faktury:** Zawiera podsumowanie podsumowania szczegółów rozliczeń partnera programu CSP. Obejmuje to podsumowanie opłat za okres rozliczeniowy, numer faktury, warunki płatności (NET 60 dni), a także formy płatności według sieci lub kontroli.

- **Strona 2 (i wszystkie kolejne strony) faktury:** Szczegóły dotyczące zakupów firmy Microsoft i zakupu niezależnych dostawców oprogramowania (opartych na licencjach) z komercyjnej witryny Marketplace. Możesz zidentyfikować zakupy na podstawie licencji niezależnego dostawcy oprogramowania w wierszu **wydawcy** poniżej każdej nazwy produktu. Skojarzony plik uzgadniania oferuje więcej szczegółów dotyczących rozliczeń dla określonych opłat za faktury.

- **Końcowa Strona faktury:** W przypadku naliczania opłat za produkty Marketplace oparte na licencji od niezależnego dostawcy oprogramowania zostanie wyświetlona więcej szczegółowych informacji o nazwie i adresie wydawcy niezależnego dostawcy oprogramowania.

### <a name="tips-on-reading-your-reconciliation-file"></a>Porady dotyczące odczytywania pliku uzgodnienia

Plik uzgodnienia **cykliczne i jednorazowe zakupy** zawiera kilka kolumn z dodatkowymi szczegółami, które mapują opłaty na fakturę. Kolumna **wydawcaname** wskazuje, czy zakup pochodzi od firmy Microsoft, czy wydawcy niezależnego dostawcy oprogramowania.

Niektóre opłaty w pliku uzgadniania mogą pojawić się z kosztem $0. Może to być spowodowane ofertą oferowaną przez niezależnego dostawcę oprogramowania (zwykle 30 lub 60 dni) lub z ofertą dołączenia do własnej licencji.

W przypadku bezpłatnej wersji próbnej niezależnych dostawców oprogramowania:

- Bezpłatny okres próbny obejmuje koszt produktu SaaS opartego na licencji niezależnego dostawcy oprogramowania. Nie będzie też naliczana opłata za skojarzone użycie infrastruktury platformy Azure przez ten produkt SaaS.  Jeśli używasz oferty niezależnego dostawcy oprogramowania, bezpłatna wersja próbna nie obejmuje kosztu użycia infrastruktury platformy Azure. W takim przypadku opłaty za użycie infrastruktury platformy Azure będą wyświetlane w osobnym pliku uzgodnienia platformy Azure.

- W przypadku zakupu i wdrożenia bezpłatnego produktu uprawniającego do korzystania z wersji próbnej niezależnego dostawcy oprogramowania klient zostanie automatycznie zarejestrowany w bezpłatnej wersji próbnej przez wydawcę niezależnego dostawcy oprogramowania. Bezpłatny okres próbny kończy się automatycznie po okresie zdefiniowanym przez wydawcę niezależnego dostawcy oprogramowania. Po zakończeniu okresu klient będzie obciążany opłatą. Oznacza to, że plik uzgadniania może przedstawiać dwa wiersze dla produktu uprawniającego do wersji próbnej: taki, który śledzi okres próbny i taki, który śledzi płatną ofertę (co spowoduje wyświetlenie kosztu $0 do momentu zakończenia okresu próbnego). Po zakończeniu okresu próbnego wiersz pokazujący płatną ofertę zacznie zawierać opłaty. 

Aby uzyskać więcej informacji o tym, co reprezentuje każda kolumna, zobacz [Używanie plików uzgadniania](use-the-reconciliation-files.md). Zobacz również [typy rozliczeń w centrum partnerskim](billing-different-types.md)

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie komercyjnymi produktami Marketplace dla klientów](csp-commercial-marketplace-manage.md)
- [Dowiedz się więcej na temat pomocy technicznej dla komercyjnych produktów Marketplace](csp-commercial-marketplace-support.md)