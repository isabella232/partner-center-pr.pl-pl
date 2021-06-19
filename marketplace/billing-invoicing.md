---
title: Rozliczenia i fakturowanie dla Azure Marketplace klientów
description: W tym artykule opisano typowe pytania dotyczące rozliczeń i fakturowania dla Azure Marketplace klientów.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: d45d301abfea03e06a8fc67e759012d4275d7dec
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373460"
---
# <a name="azure-marketplace-billing-and-invoicing"></a>Azure Marketplace rozliczeń i fakturowania

W tym artykule omówiono informacje dotyczące rozliczeń i fakturowania dla Azure Marketplace klientów.

## <a name="microsoft-supports-multiple-currencies"></a>Firma Microsoft obsługuje wiele walut

Azure Marketplace oferty są wycenione i rozliczane w tych 17 walutach:

- Dolar australijski (AUD)
- Real Brazylia (BRL)
- Funt brytyjskie (GB))
- Dolar kanada (CAD)
- Chiński (CNY)
- Krona duńska (DKK)
- Euro (EUR)
- Rupia indyjska (INR)
- Jen japoński (JPY)
- Won koreański (KRW)
- Dolar nowozelandzki (NZD)
- Krona norweska (NOK)
- Rosyjski łańcowia (RUB)
- Krona szwedzki (SEK)
- Dobowe (CHF)
- Dolar tajwański (TWD)
- Dolar amerykański (USD)

## <a name="billing"></a>Rozliczenia

Opłaty będą naliczane za cykliczne zakupy w okresie, w którym zostały zakupione. Te opłaty będą widoczne na fakturze za odpowiedni miesiąc kalendarzowy. Będą one nadal autoryzować w następnym okresie tego samego dnia pierwotnego zakupu.

[![Przykładowy harmonogram rozliczania cyklicznych zakupów miesięcznych i cyklicznych w roku.](media/billing/billing-charges-recurring.png)](media/billing/billing-charges-recurring.png#lightbox)

>[!NOTE]
> Okres świadczenia usługi to okres, za który zapłacono za korzystanie z usługi. Zostanie ona automatycznie odnowiona w godzinach i okresu świadczenia usługi, chyba że użytkownik anuluje je wcześniej.

> [!NOTE]
> Dostosowujemy się do ostatniego dnia miesiąca rozliczeniowego, jeśli data miesiąca odnowienia nie może być równa dacie miesiąca zakupu. Oznacza to, że jeśli jeden z nich ma subskrybować datę 1/31, datą zakończenia rozliczeń dla lutego będzie 2/27, a nowy okres rozliczeniowy zaczyna się 2.02.28 (2.02.28 i 2/29, jeśli zaczyna się w roku przestępniowym).

## <a name="invoices"></a>Faktury

Otrzymasz wiadomość e-mail na początku każdego miesiąca kalendarzowego, gdy faktura będzie dostępna w Azure Portal. Na fakturze będą wyświetlane wszystkie bezpłatne i płatne oferty zakupione i/lub zużyte w miesiącu kalendarzowym. Jeśli masz tylko bezpłatne oferty, zobaczysz tylko pozycje 0 USD i nie trzeba będzie podjąć żadnych działań płatniczych. **Enterprise Agreement klienci otrzymają** łącznie fakturę przedstawiającą opłaty za platformę Azure i Azure Marketplace (z wyłączeniem klientów w Australii, Japonii i Singapurze). **Klienci, którzy kupują bezpośrednio Azure Marketplace,** otrzymają rachunek tylko za Azure Marketplace zakupów. Aby uzyskać szczegółowe informacje, [zobacz Invoices for MOSP accounts (Faktury dla kont moSP).](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)

Po otrzymaniu faktury mogą być różne:

- Jeśli instrument płatniczy jest kartą kredytową, faktura zostanie wystawowana natychmiast po zakupie rezerwacji. Ta faktura będzie oddzielona od faktury miesięcznej.
- Jeśli instrument płatniczy to czek/przelew, ten zakup zostanie uwzględniony na miesięcznej fakturze za platformę Marketplace.

Faktury są tworzone dla kont rozliczeniowych programu Microsoft Online Service Program (MOSP), Umowy z Klientem Microsoft (MCA) i umowy Microsoft Partner Agreement (MPA). Faktury są generowane na podstawie typu konta rozliczeniowego. Azure Marketplace rozliczeniowe są naliczane kilka dni po zakończeniu okresu rozliczeniowego. Faktura dla maszyn Azure Marketplace, rezerwacji i maszyn wirtualnych punktowych jest generowana około dziewiątego dnia [miesiąca.](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts) Pokazuje odpowiednie opłaty z poprzedniego miesiąca. Jeśli na przykład użytkownik zakupił rezerwację 1 marca, a inna rezerwacja 30 marca, jedna faktura w kwietniu obejmuje obie rezerwacje.

Aby uzyskać więcej informacji na temat faktur, zobacz Understand your Azure external service charges (Informacje [o opłatach za usługi zewnętrzne platformy Azure).](/azure/cost-management-billing/understand/understand-azure-marketplace-charges)

## <a name="next-steps"></a>Następne kroki

- [Co to jest Azure Marketplace?](azure-marketplace-overview.md)
- [Azure Marketplace zakupu](azure-purchasing-invoicing.md)
