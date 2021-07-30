---
title: Rozliczenia za produkty platformy handlowej
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Dowiedz się, jak działa rozliczanie dla produktów SaaS isv lub subskrypcji zakupionych dla klientów na platformie handlowej w Partner Center.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 102f13530ece08cd813412a44897ece0186e7cbb
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837955"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Rozliczenia za produkty i subskrypcje platformy handlowej w Partner Center


**Odpowiednie role:** Administrator globalny | Administrator rozliczeń

Jako partner w programie CSP możesz używać usługi Partner Center do kupowania opartych na licencjach produktów SaaS od wydawców ISV na platformie handlowej. Po tym możesz uzyskać dostęp do rachunku za tego typu zakupy. Okres rozliczeniowy rozpoczyna się pierwszego dnia miesiąca kalendarzowego i kończy się ostatniego dnia miesiąca kalendarzowego. Faktury są udostępniane 8 dnia następnego miesiąca.

Dostęp do faktur można uzyskać z pulpitu nawigacyjnego Partner Center [lub](https://partner.microsoft.com/dashboard/) przy użyciu [Partner Center API.](/partner-center/develop/)

Partnerzy w programie CSP są rozliczani za rozwiązania platformy handlowej dla isV zakupione dla klienta w przypadku zakupu tych produktów w usłudze Partner Center lub u firmy Azure Portal (przy użyciu wcześniej zakupionej dzierżawy platformy Azure przez klienta CSP).

>[!NOTE]
>Jeśli klienci korzystają z własnej dzierżawy usługi Azure AD (nie tej zakupionej od partnera w programie CSP), klienci mogą również zakupić własne rozwiązanie SaaS dla isv bezpośrednio w witrynie ([Microsoft AppSource](https://appsource.microsoft.com/) [lub Azure Marketplace](https://azuremarketplace.microsoft.com/)). Jeśli to zrobi, otrzyma własny rachunek bezpośrednio od firmy Microsoft. Podobnie jeśli partner w programie CSP sprzedaje klientowi subskrypcję platformy Azure lub nowy plan [](/azure/role-based-access-control/built-in-roles) platformy Azure i udziela klientowi (lub odsprzedawcy pośredniego) dostępu opartego na rolach do tej dzierżawy (przypisując mu dowolną rolę oprócz **Czytelnika),** ten klient (lub odsprzedawca pośredni) może również zakupić oferty platformy handlowej bez wcześniejszego zatwierdzenia lub powiadomienia partnera CSP. W takich przypadkach firma Microsoft nie będzie bezpośrednio powiadamiać partnerów w programie CSP o zakupach dokonanych przez ich klientów. Firma Microsoft oferuje jednak opcjonalny mechanizm [Azure Monitor,](/azure/azure-monitor/platform/alerts-activity-log) który umożliwia ustawianie alertów lub powiadomień dotyczących aktywności w subskrypcji platformy Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Uzyskiwanie dostępu do informacji rozliczeniowych dotyczących produktów na platformie handlowej

Gdy faktura będzie gotowa do wyświetlenia, administrator globalny lub administrator rozliczeń w firmie otrzyma wiadomość e-mail. Aby uzyskać dostęp do najnowszej faktury i pliku uzgodnień dla zakupów produktów na platformie handlowej:

1. Zaloguj się do [pulpitu nawigacyjnego](https://partner.microsoft.com/dashboard/) Centrum partnerskiego.

2. Z menu Partner Center wybierz pozycję **Rozliczenia.** 

    W górnej części strony Rozliczenia zostaną wyświetlonych dwie **karty:** Cykliczne i Cykliczne oraz Zakupy **jednorazowe.** Każda karta umożliwia dostęp do plików faktur i uzgodnień (uzgodnień) dla różnych produktów z platformy handlowej:

    - **Karta** Cykliczne: wyświetla pliki faktur i uzgodnień dla subskrypcji związanych z usługami Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro i Microsoft Azure.

    - **Karta Zakupów cyklicznych i jednorazowych:** pokazuje pliki faktur i uzgodnień dla planu platformy Azure, rezerwacji platformy Azure, oprogramowania i produktów platformy handlowej.
  
3. Wybierz **kartę Cykliczne i zakupy jednorazowe.** Jeśli zakupiono subskrypcje dla klienta w innej walucie, zobaczysz kartę dla każdej waluty. Na tej stronie możesz wykonać kilka czynności:

    - Aby wyświetlić najnowszą fakturę i plik uzgodnień, wybierz **pozycję Plik** faktury **lub uzgodnień.** (Jeśli chcesz, możesz również uzyskać dostęp do najnowszej faktury i ponownie utworzyć plik danych przy [użyciu Partner Center API.](/partner-center/develop/)

    - Aby wyświetlić wcześniejsze faktury i ponownie skonfigurować pliki, rozwiń wiersz **Historia rozliczeń** poniżej.

    - Aby sprawdzić szacowane saldo konta lub rachunek w dowolnym momencie na podstawie najnowszej aktywności konta, wybierz link w obszarze **nagłówka Oszacowania.**  

    >[!NOTE]
    > Gdy opublikujemy Twój rachunek 8 dnia miesiąca, będzie on obejmować podatki oraz wszelkie inne obowiązujące opłaty i środki. Oznacza to, że końcowa należna kwota może różnić się od kwoty, która będzie się różnić w okresie rozliczeniowym.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Więcej informacji o fakturach i plikach wymiany dla produktów platformy handlowej

Ta sekcja zawiera więcej informacji na temat plików faktur i uzgodnień dla subskrypcji SaaS komercyjnej platformy handlowej zakupionych dla klientów od zewnętrznych wydawców isV.

Po wybraniu  pozycji Zakupy cykliczne i  jednorazowe z opcji Rozliczenia w menu usługi Partner Center uzyskasz dostęp do faktur i plików uzgodnień dla opłat związanych zarówno z zakupami firmy Microsoft (firmy Microsoft), jak i z zakupami dostawcy oprogramowania (innych firm). Te zakupy mogą być skojarzone z:

- Subskrypcje SaaS (od wydawców firmy Microsoft lub isV)

- Plan platformy Azure

- Rezerwacje platformy Azure

- Inne oprogramowanie oparte na subskrypcji (od firmy Microsoft lub od wydawców ISV)

Przykładami takich zakupów mogą być oprogramowanie SUSE Linux (subskrypcja oprogramowania) lub subskrypcja produktu SaaS dostawcy oprogramowania platformy Azure.

>[!NOTE]
> Aby uzyskać więcej informacji na temat odczytywania faktur i plików ponownego rozliczania, zobacz również [Omówienie rozliczeń](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Wskazówki na odczytywaniu faktury

W przypadku zakupu opartego na licencji produktu SaaS od zewnętrznego wydawcy isv publisher zobaczysz tylko opłaty za licencję na fakturze. Dzieje się tak nawet wtedy, gdy produkt SaaS dostawcy oprogramowania isv korzysta z podstawowych zasobów infrastruktury platformy Azure. Wynika to z tego, że opłaty za użycie infrastruktury platformy Azure klienta dla produktu SaaS dostawcy oprogramowania są rozliczane bezpośrednio u dostawcy oprogramowania. (Dostawcy oprogramowania zobaczą skojarzone opłaty za użycie platformy Azure we własnym pliku uzgodnień faktur z dziennego użycia platformy Azure).

Faktura będzie zawierać kilka stron:

- **Strona 1 faktury:** Zawiera podsumowanie szczegółów rozliczeń partnera programu CSP. Obejmuje to podsumowanie opłat za okres rozliczeniowy, numer faktury, warunki płatności (60 dni netto) i formy płatności rozliczeń do zapłacenia za pomocą przelewu lub czeku.

- **Strona 2 (i wszystkie kolejne strony) faktury:** Szczegóły opłat za zakupy firmy Microsoft i zakupy innych firm (na podstawie licencji) z platformy handlowej. Zakupy oparte na licencjach isv można zidentyfikować przy **Publisher** pod każdą nazwą produktu. Skojarzony plik uzgodnień zawiera więcej szczegółów rozliczeń dla konkretnych opłat na fakturze.

- **Ostatnia strona faktury:** Jeśli za produkty z platformy handlowej opartej na licencjach zostały naliczone opłaty od isV, na ostatniej stronie zostanie podanych więcej szczegółów dotyczących nazwy i adresu wydawcy isv.

### <a name="tips-on-reading-your-reconciliation-file"></a>Wskazówki odczytywania pliku uzgodnień

Plik **uzgodnień cyklicznych i jednorazowych** zakupów zawiera kilka kolumn z dodatkowymi szczegółami, które są mapowane na opłaty na fakturze. Kolumna **PublisherName** pokazuje, czy zakup pochodzi od firmy Microsoft, czy od zewnętrznego wydawcy isv publisher.

Niektóre opłaty w pliku uzgodnień mogą być wyświetlane z kosztem 0 USD. Może to być spowodowane ofertą "bezpłatnej wersji próbnej" (zazwyczaj 30 lub 60 dni) lub ofertą bring your own license dla isV.

W przypadku ofert bezpłatnej wersji próbnej isv:

- W tym okresie bezpłatny okres próbny obejmuje koszt produktu SaaS opartego na licencjach dostawcy oprogramowania. Nie zostaną również naliczone opłaty za skojarzone użycie infrastruktury platformy Azure przez ten produkt SaaS.  Jeśli jednak korzystasz z oferty wirtualnego oprogramowania opartego na użyciu, bezpłatna wersja próbna nie obejmuje kosztu bazowego użycia infrastruktury platformy Azure. W takim przypadku opłaty za użycie infrastruktury platformy Azure będą wyświetlane w oddzielnym pliku uzgodnień platformy Azure.

- Po zakupie i wdrożeniu bezpłatnej wersji próbnej kwalifikującej się produktu dla klienta przez isV klient jest automatycznie zarejestrowany w bezpłatnej wersji próbnej przez wydawcę isv. Bezpłatny okres próbny kończy się automatycznie po okresie zdefiniowanym przez wydawcę isv. Po zakończeniu okresu klient zostanie obciążony. Oznacza to, że w pliku uzgodnień mogą być wyświetlane dwa wiersze dla produktu kwalifikującego się do korzystania z wersji próbnej: jeden, który śledzi okres próbny, i jeden, który śledzi płatną ofertę (co spowoduje wyświetlenie kosztu w wysokości 0 USD do momentu zakończenia okresu próbnego). Po zakończeniu okresu próbnego zaczną być wyświetlane opłaty w wierszu przedstawiającym płatną ofertę. 

Aby uzyskać więcej informacji o tym, co reprezentuje każda kolumna, zobacz [Używanie plików uzgodnień](use-the-reconciliation-files.md). Zobacz też [Typy rozliczeń w Partner Center](./billing-basics.md)

## <a name="next-steps"></a>Następne kroki

- [Zarządzanie produktami platformy handlowej dla klientów](csp-commercial-marketplace-manage.md)
- [Dowiedz się więcej o pomocy technicznej dla produktów platformy handlowej](csp-commercial-marketplace-support.md)