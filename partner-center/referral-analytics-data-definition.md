---
title: Definicje danych analizy poleceń
ms.topic: article
ms.date: 08/10/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Dokument zawiera listę różnych raportów i ich definicji danych, które można pobrać ze stron analizy poleceń.
author: v-sausharma
ms.author: v-sausharma
ms.localizationpriority: medium
ms.openlocfilehash: e2409dcbfd2a9de677ef4ec79bf8749072859325
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959779"
---
# <a name="referral-analytics-export--data-definitions"></a>Eksportowanie analizy poleceń — definicje danych

**Odpowiednie role:** Administrator poleceń

## <a name="introduction"></a>Wprowadzenie

Za pomocą przycisku Eksportuj na stronie analizy potencjalnych klienta i współzasyłania można wyeksportować nieprzetworzone zestawy danych.

Różne raporty, które można pobrać wraz z ich definicjami danych, są wymienione w następujących tabelach:

## <a name="leads-export"></a>Eksportowanie potencjalnych klientów

|   Nazwa kolumny |   Opis danych    |
|----|----|
|   Identyfikator polecenia |   Unikatowy identyfikator polecenia  |
|   Kraj klienta    |   Kraj klienta |
|   Nazwa klienta   |   Nazwa klienta    |
|   Data utworzenia polecenia  |   Data utworzenia polecenia   |
|   Źródło polecenia |   Źródło polecenia: Kwalifikowane, Marketplace  |
|   Typ polecenia   |   Typ potencjalnego klienta    |
|   Kierunek potencjalnego klienta  |   Kierunek potencjalnego klienta   |
|   Waluta potencjalnych klienta   |   Waluta potencjalnego klienta    |
|   Wartość potencjalnego klienta  |   Szacowana wartość potencjalnego klienta dostarczana przez partnera    |
|   Wartość potencjalnego klienta (USD)    |   Szacowana wartość potencjalnego klienta dostarczana przez partnera w USD |
|   Stan      |   Najnowszy stan polecenia   |
|   Przyczyna stanu   |   Uwagi lub przyczyna stanu    |
|       |       |


## <a name="co-sell-export"></a>Eksportowanie do współpracy

|   Nazwa kolumny |   Opis danych    |
|    ----    |    ----    |
|   Identyfikator polecenia |   Unikatowy identyfikator polecenia  |
|   Kraj klienta    |   Kraj klienta |
|   Customer City   |   Miasto klienta    |
|   Nazwa klienta   |   Nazwa klienta    |
|   Data utworzenia polecenia  |   Data utworzenia polecenia   |
|   Typ transakcji   |   Typ transakcji: współsieć, prowadzone przez partnera, prywatne |
|   Kierunek transakcji  |   Kierunek transakcji: przychodzący i wychodzący    |
|   Waluta transakcji   |   Waluta transakcji    |
|   Szacowana wartość transakcji    |   Szacowana wartość transakcji dostarczana przez partnera    |
|   Szacowana wartość transakcji (USD)  |   Szacowana wartość transakcji dostarczana przez partnera w USD |
|   Identyfikator rozwiązania     |   Lista identyfikatorów rozwiązań |
|   Nazwa rozwiązania   |   Lista nazw rozwiązań  |
|   Identyfikator MPN  |   Identyfikator sieci partnera firmy Microsoft partnera |
|   Nazwa partnera    |   Nazwa partnera |
|   Identyfikator transakcji |   Identyfikator transakcji  |
|   Identyfikator zaangażowania   |   Unikatowy identyfikator zaangażowania    |
|   Identyfikator MICROSOFT MSX    |   IDENTYFIKATOR TRANSAKCJI MSX  |
|   Data utworzenia polecenia firmy Microsoft    |   Data utworzenia odwołania od firmy Microsoft |
|   Imię zarejestrowanego kontaktu   |   Imię i nazwisko kontaktu z partnerem podane podczas rejestracji transakcji |
|   Nazwisko zarejestrowanego kontaktu    |   Nazwisko kontaktu z partnerem podanego podczas rejestracji transakcji  |
|   Zarejestrowana kontaktowa wiadomość e-mail    |   Wiadomość e-mail kontaktu z partnerem podaną podczas rejestracji transakcji  |
|   Zarejestrowany numer telefonu kontaktowego |   Telefon kontaktu z partnerem podanego podczas rejestracji transakcji   |
|   Waluta kontraktu   |   Waluta kontraktu dostarczonego podczas rejestracji transakcji  |
|   Wartość kontraktu  |   Łączna wartość kontraktu zapewniana podczas rejestracji transakcji. Obejmuje to opłaty za oprogramowanie i usługę, ale nie koszty sprzętu  |
|   Wartość kontraktu (USD)    |   Łączna wartość kontraktu w USD podana podczas rejestracji transakcji   |
|   Data rozpoczęcia kontraktu |   Data rozpoczęcia umowy podanej podczas rejestracji transakcji    |
|   Data zakończenia kontraktu   |   Data zakończenia umowy podanej podczas rejestracji transakcji  |
|   Data podpisania kontraktu  |   Podpisz datę umowy podaną podczas rejestracji transakcji |
|   Typ kontraktu   |   Typ kontraktu    |
|   Identyfikator zarejestrowanego rozwiązania do transakcji |   Identyfikator rozwiązania do rejestracji transakcji    |
|   Nazwa zarejestrowanego rozwiązania do transakcji   |   Nazwa rozwiązania do rejestracji transakcji  |
|   Waluta zarejestrowanego rozwiązania transakcji   |   Waluta dla rozwiązania udostępnianego podczas rejestracji transakcji |
|   Wartość zarejestrowanego rozwiązania transakcji  |   Wartość rozwiązania zapewniana podczas rejestracji transakcji. Ogólnie rzecz biorąc, jest to łączna wartość kontraktu mniejsza niż wszystkie cykliczne opłaty za implementację.   |
|   Wartość zarejestrowanego rozwiązania transakcji (USD)    |   Wartość rozwiązania w USD zapewniana podczas rejestracji transakcji |
|   Wdrożono w dniu |   Wskazuje, czy rozwiązanie zostało wdrożone na platformie Azure, czy na innych platformach    |
|   Wdrożenie podstawowe w dniu   |   Wskazuje, czy rozwiązanie zostało wdrożone w dzierżawie klienta lub dzierżawie partnera  |
|   Data utworzenia transakcji  |   Data utworzenia rejestracji transakcji  |
|   Data przesłanej transakcji     |   Data przesłanej rejestracji transakcji |
|   Data zatwierdzenia/odrzucenia transakcji     |   Data zatwierdzenia/odrzucenia transakcji. Jest to mapowane na kolumnę stanu. |
|   Umowa federalna USA |   Wskazuje, czy jest to umowa federalna USA    |
|   Is Marketplace Transacted Deal  |   Wskazuje, czy jest to transakcja z transakcją w witrynie Marketplace    |
|   Data transakcji w witrynie Marketplace    |   Data transakcji w witrynie Marketplace, jeśli transakcja jest transakcyjna na platformie handlowej|
|   Stan      |   Najnowszy stan polecenia   |
|   Przyczyna stanu   |   Uwagi lub przyczyna stanu    |
|       |       |
