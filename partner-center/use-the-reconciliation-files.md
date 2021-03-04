---
title: Korzystanie z plików uzgadniania
ms.topic: article
ms.date: 06/08/2020
description: Dowiedz się więcej na temat plików uzgadniania w centrum partnerskim i interpretacji szczegółowych widoków elementów wierszy opłat dla danego cyklu rozliczeniowego.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d927b138c32b3e5f6f5d906db898e17f89a85aae
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755775"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Dowiedz się, jak odczytywać elementy wiersza w plikach uzgadniania Centrum partnerskiego

Dotyczy:

- Centrum partnerskie
- Centrum partnerskie Microsoft Cloud for US Government

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