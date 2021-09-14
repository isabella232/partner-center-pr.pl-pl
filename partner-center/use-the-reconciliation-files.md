---
title: Korzystanie z plików uzgodnień
ms.topic: article
ms.date: 03/26/2021
description: Dowiedz się więcej o plikach uzgodnień w Partner Center i interpretowaniu szczegółowych widoków elementów wiersza opłat dla danego cyklu rozliczeniowego.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5fae4c9b9b40c8a71b56c46d0d1be629f832842
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246574"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Dowiedz się, jak odczytywać elementy wiersza w plikach Partner Center uzgodnień

**Odpowiednie role:** Administrator rozliczeń | Administrator globalny

Pliki uzgodnień można pobrać ze strony Partner Center, aby uzyskać szczegółowy widok elementów wiersza każdej opłaty w cyklu rozliczeniowym. Szczegóły elementu wiersza obejmują opłaty za subskrypcje poszczególnych klientów i szczegółowe zdarzenia (takie jak krótkoterminowe dodawanie licencji do subskrypcji).

Aby uzyskać informacje na temat odczytywania **faktury,** zobacz [Odczytywanie rachunku](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Opis pól pliku uzgodnień

- [Pola pliku uzgodnień w oparciu o licencję](license-based-recon-files.md)
- [Pola pliku uzgodnień w oparciu o użycie](usage-based-recon-files.md)
- [Pola pliku uzgodnień dziennego użycia](daily-rated-usage-recon-files.md)
- [Pola pliku uzgodnień programu CSP z zakupem czasowym](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Opis typów opłat w plikach uzgodnień

Aby poznać typy opłat w plikach uzgodnień (kolumna **ChargeType),** zobacz Typy opłat [pliku uzgodnień](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Rozwiązywanie problemów z formatowaniem

Czasami plik uzgodnień może zawierać problemy z formatowaniem. Na przykład ten problem może wystąpić, jeśli nie są używane lokalne en-US.

Wykonaj następujące kroki, aby rozwiązać wszelkie problemy z formatowaniem w plikach uzgodnień:

1. Otwórz plik uzgodnień (w formacie .csv) w Microsoft Excel.
2. Wybierz pierwszą kolumnę w pliku.
3. Otwórz Kreatora **konwertowania tekstu na kolumny.** Na wstążce wybierz pozycję **Dane,** a następnie wybierz **pozycję Tekst na kolumny.**
4. W kreatorze wybierz typ **pliku rozdzielanego**. Następnie wybierz pozycję **Dalej**.
5. W polu **Ograniczniki** wybierz pozycję **Przecinek**. (Jeśli **karta** jest już zaznaczona, możesz pozostawić tę opcję zaznaczoną). Następnie wybierz pozycję **Dalej.**
6. W polu **Format danych kolumny** wybierz pozycję **Date:MDY.** Następnie wybierz pozycję **Dalej**.
7. W polu **Format danych kolumny** wybierz pozycję **Tekst** dla wszystkich kolumn ilości. Następnie wybierz pozycję **Finish** (Zakończ).

## <a name="download-reconciliation-files-programmatically"></a>Programowe pobieranie plików uzgodnień

Pliki uzgodnień mogą być bardzo duże i czasami trudno je pobrać. Aby pobrać pliki uzgodnień programowo, zobacz [Pobieranie elementów wiersza faktury.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Jeśli plik przekracza limit wierszy w Excel

Jeśli możesz pobrać plik uzgodnień, ale nie otworzysz go w Microsoft Excel, prawdopodobnie oznacza to, że plik zawiera więcej wierszy niż Excel będzie zezwalać. W takim przypadku możesz otworzyć plik za pomocą jednej z poniższych procedur.

### <a name="open-a-recon-file-in-power-bi"></a>Otwórz plik rekonesji w Power BI

1. Pobierz plik uzgodnień w zwykły sposób.
2. Pobierz, zainstaluj i otwórz wystąpienie programu Microsoft Power BI.
3. Na karcie Power BI **Narzędzia** główne wybierz pozycję **Pobierz dane.**
4. Na liście **wspólnych źródeł danych wybierz** pozycję **Tekst/CSV.**
5. Po wyświetleniu monitu otwórz plik rekonescji.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Otwieranie pliku rekonescji w Excel tabeli przestawnej

1. Pobierz plik uzgodnień w zwykły sposób.
2. Otwórz nowy plik w Microsoft Excel.
3. Na karcie **Dane** wybierz pozycję **Pobierz dane,** wybierz pozycję **Z pliku**, a następnie wybierz **pozycję Tekst/CSV.**
4. Po wyświetleniu monitu otwórz plik rekonescji. Zostaną wyświetlone dane.
5. W menu **rozwijaym** Załaduj wybierz pozycję **Załaduj do**, a następnie wybierz przycisk **OK.**
6. W **oknie dialogowym Import danych** wybierz pozycję **Raport tabeli przestawnej,** aby otworzyć plik.

## <a name="negative-amount-displayed"></a>Wyświetlana kwota ujemna

W pliku uzgodnień może być widać kwotę ujemną. Jest to prawdopodobnie spowodowane przez jedną z następujących przyczyn:

- Ostatnio anulowano lub ograniczono liczbę licencji
- Otrzymano kredyt na umowę licencyjną usługi (SLA) lub na korzystanie z platformy Azure

Aby uzyskać więcej informacji na temat tej transakcji, sprawdź jej atrybut typu opłaty w pliku uzgodnienia.

## <a name="map-taxes-or-vat"></a>Mapowanie podatków lub podatku VAT

Aby zamapować podatki lub podatek od wartości dodanej (VAT) na fakturę:

- **Zsuń kolumnę** Tax (Podatek) z pliku opartego na licencjach.
- **Zsuń kolumnę TaxAmount** z pliku opartego na użyciu.

## <a name="itemize-reconciliation-files-by-partner"></a>Elementowanie plików uzgodnień według partnera

Partnerzy w modelu **pośrednim mogą** używać tych dodatkowych pól zarówno w plikach uzgodnień opartych na licencjach, jak i opartych na użyciu, aby określić te pliki według odsprzedawcy.

| Identyfikator MPN | Opis |
| ------ | ----------- |
| Identyfikator MPN | Identyfikator Microsoft Partner Network (MPN) partnera Dostawca rozwiązań w chmurze (CSP) (bezpośredniego lub pośredniego). |
| [Identyfikator MPN odsprzedawcy](#reseller-mpn-id) | Identyfikator [MPN odsprzedawcy rekordu dla subskrypcji](#reseller-mpn-id). To pole odpowiada identyfikatorowi odsprzedawcy wymienionemu dla określonej subskrypcji w Partner Center. Pojawia się tylko w plikach uzgodnień dla partnerów w modelu pośrednim. |

### <a name="reseller-mpn-id"></a>Identyfikator MPN odsprzedawcy

Jeśli partner CSP sprzedał subskrypcję bezpośrednio klientowi, jego identyfikator **MPN** jest dwukrotnie wymieniony jako identyfikator **MPN** i identyfikator **MPN odsprzedawcy.**

Jeśli partner programu CSP ma odsprzedawcę bez identyfikatora **MPN,** ta wartość jest ustawiana na identyfikator **MPN** partnera.

Jeśli partner CSP usunie identyfikator **MPN odsprzedawcy,** ta wartość zostanie ustawiona *na -1.*

Aby wyświetlić lub zaktualizować identyfikator **MPN odsprzedawcy:**

1. Zaloguj się do Centrum partnerskiego.
2. W menu Partner Center wybierz pozycję **Klienci.**
3. Wybierz klienta z listy.
4. W menu klienta wybierz pozycję **Subskrypcje.**
5. Wybierz subskrypcję z listy.
6. Wybierz **pozycję aktualizuj,** aby zmienić **odsprzedawcę (identyfikator MPN).**

## <a name="next-steps"></a>Następne kroki

- [Jak odczytać rachunek & pliku rekonescji](read-your-bill.md) 