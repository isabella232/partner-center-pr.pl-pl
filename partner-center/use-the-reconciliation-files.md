---
title: Korzystanie z plików uzgadniania
ms.topic: article
ms.date: 03/26/2021
description: Dowiedz się więcej na temat plików uzgadniania w centrum partnerskim i interpretacji szczegółowych widoków elementów wierszy opłat dla danego cyklu rozliczeniowego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730090"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Dowiedz się, jak odczytywać elementy wiersza w plikach uzgadniania Centrum partnerskiego

**Odpowiednie role**

- Administrator rozliczeń
- Administrator globalny

Pliki uzgadniania można pobrać z Centrum partnerskiego, aby wyświetlić szczegółowy widok elementu z każdą opłatą w cyklu rozliczeniowym. Szczegóły elementu wiersza obejmują opłaty dla każdej subskrypcji klienta i szczegółowe zdarzenia (na przykład dodatkowe Dodawanie licencji do subskrypcji).

Aby uzyskać informacje na temat sposobu odczytywania **faktury**, zobacz [odczytywanie rachunku](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Informacje o polach plików uzgadniania

- [Pola pliku uzgodnień w oparciu o licencję](license-based-recon-files.md)
- [Pola pliku uzgodnień w oparciu o użycie](usage-based-recon-files.md)
- [Pola pliku uzgodnień dziennego użycia](daily-rated-usage-recon-files.md)
- [Pola pliku uzgadniania jednorazowego zakupu dostawcy usług kryptograficznych](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Informacje o typach opłat w plikach uzgadniania

Aby zrozumieć typy opłat w plikach uzgadniania (kolumna **opłatatype** ), zobacz temat [typy obciążeń plików uzgadniania](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Rozwiązywanie problemów z formatowaniem

Czasami plik uzgadniania może zawierać problemy z formatowaniem. Na przykład ten problem może wystąpić, jeśli ustawienia regionalne en-US nie są używane.

Wykonaj następujące kroki, aby naprawić wszelkie problemy z formatowaniem w plikach uzgadniania:

1. Otwórz plik uzgadniania (w formacie CSV) w programie Microsoft Excel.
2. Wybierz pierwszą kolumnę w pliku.
3. Otwórz **Kreatora konwersji tekstu na kolumny**. Na wstążce wybierz pozycję **dane**, a następnie wybierz pozycję **tekst do kolumn**.
4. W kreatorze wybierz pozycję **rozdzielany typ pliku**. Następnie wybierz pozycję **Dalej**.
5. W polu **ograniczników** wybierz **przecinek**. (Jeśli **karta** jest już zaznaczona, można opuścić tę opcję). Następnie wybierz przycisk **dalej**.
6. W polu **Format danych kolumny** wybierz **datę: MDR**. Następnie wybierz pozycję **Dalej**.
7. W polu **Format danych kolumny** zaznacz opcję **tekst** dla wszystkich kolumn kwoty. Następnie wybierz pozycję **Finish** (Zakończ).

## <a name="download-reconciliation-files-programmatically"></a>Programowe pobieranie plików uzgadniania

Pliki uzgadniania mogą być bardzo duże i czasami trudno je pobrać. Aby programowo pobrać pliki uzgadniania, zobacz [Pobieranie elementów wiersza faktury](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Jeśli rozmiar pliku przekracza limit wierszy w programie Excel

Jeśli możesz pobrać plik uzgadniania, ale nie otworzyć go w programie Microsoft Excel, prawdopodobnie oznacza to, że plik zawiera więcej wierszy niż zezwala program Excel. W takim przypadku można użyć dowolnej z poniższych procedur, aby otworzyć plik.

### <a name="open-a-recon-file-in-power-bi"></a>Otwórz plik rekonesans w Power BI

1. Pobierz plik uzgadniania w zwykły sposób.
2. Pobierz, zainstaluj i Otwórz wystąpienie Power BI.
3. Na karcie **Narzędzia główne** Power BI wybierz pozycję **Pobierz dane**.
4. Na liście **wspólnych źródeł danych** wybierz pozycję **tekst/CSV**.
5. Po wyświetleniu monitu Otwórz plik rekonesans.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Otwórz plik rekonesans w tabeli przestawnej programu Excel

1. Pobierz plik uzgadniania w zwykły sposób.
2. Otwórz nowy plik w programie Microsoft Excel.
3. Na karcie **dane** wybierz pozycję **Pobierz dane**, wybierz pozycję **z pliku**, a następnie wybierz pozycję **tekst/CSV**.
4. Po wyświetleniu monitu Otwórz plik rekonesans. Zostaną wyświetlone Twoje dane.
5. W menu rozwijanym **ładowanie** wybierz pozycję **Załaduj do**, a następnie kliknij przycisk **OK**.
6. W oknie dialogowym **Importowanie danych** wybierz pozycję **raport tabeli przestawnej** , aby otworzyć plik.

## <a name="negative-amount-displayed"></a>Wyświetlana kwota ujemna

W pliku uzgadniania może zostać wyświetlona ujemna kwota. Jest to prawdopodobnie spowodowane jedną z następujących czynności:

- Ostatnio anulowano lub zmniejszono liczbę licencji
- Otrzymałeś środki na umowę licencyjną usługi (SLA) lub użycie platformy Azure

Aby uzyskać więcej informacji na temat tej transakcji, przejrzyj jej atrybut typu opłata w pliku uzgodnienia.

## <a name="map-taxes-or-vat"></a>Podatki mapuje lub VAT

Aby zmapować podatki lub podatek VAT na fakturę:

- Suma wartości kolumny **podatkowej** z pliku opartego na licencji.
- Suma kolumny **TaxAmount** z pliku opartego na użyciu.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemize pliki uzgodnienia według partnera

Partnerzy w **modelu pośrednim** mogą używać tych dodatkowych pól w plikach uzgadniania opartych na licencji i użycia, aby itemize pliki przez odsprzedawcę.

| Identyfikator MPN | Opis |
| ------ | ----------- |
| Identyfikator MPN | Identyfikator Microsoft Partner Network (MPN) partnera dostawcy rozwiązań w chmurze (bezpośredniego lub pośredniego). |
| [IDENTYFIKATOR MPN odsprzedawcy](#reseller-mpn-id) | [Identyfikator MPN odsprzedawcy rekordu dla subskrypcji](#reseller-mpn-id). To pole odnosi się do identyfikatora odsprzedawcy wymienionego dla określonej subskrypcji w centrum partnerskim. Występuje tylko w przypadku plików uzgadniania dla partnerów w modelu pośrednim. |

### <a name="reseller-mpn-id"></a>IDENTYFIKATOR MPN odsprzedawcy

Jeśli partner dostawcy usług kryptograficznych sprzedał subskrypcję bezpośrednio do klienta, jego **identyfikator MPN** zostanie wyświetlony dwukrotnie jako **identyfikator MPN** i **identyfikator MPN odsprzedawcy**.

Jeśli partner CSP ma odsprzedawcę bez **identyfikatora MPN**, ta wartość jest ustawiana na **identyfikator MPN** partnera.

Jeśli partner CSP usunie **identyfikator MPN odsprzedawcy**, ta wartość zostanie ustawiona na *-1*.

Aby wyświetlić lub zaktualizować **identyfikator MPN odsprzedawcy**:

1. Zaloguj się do Centrum partnerskiego.
2. W menu Centrum partnerskiego wybierz pozycję **Customers**.
3. Wybierz klienta z listy.
4. W menu Klient wybierz pozycję **subskrypcje**.
5. Wybierz subskrypcję z listy.
6. Wybierz pozycję **Aktualizuj** , aby zmienić **ODSPRZEDAWCA (identyfikator MPN)**.

## <a name="next-steps"></a>Następne kroki

- [Jak odczytać rozliczenie & pliku Rekonesans](read-your-bill.md) 