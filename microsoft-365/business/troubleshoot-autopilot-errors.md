---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązać problemy z błędami pliku urządzenia autopilota.
ms.openlocfilehash: 9b8d8ab424dd3189ff5c228dab8f5c513ff5dafc
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982747"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot

## <a name="device-file-error-messages"></a>Komunikaty o błędach pliku urządzenia

Oto informacje na niektóre błędy mogą pojawić się podczas pracy z plikami urządzenia autopilota w Microsoft 365 Business. 
  
|**Kod błędu**|**Aby spróbować naprawić**|
|:-----|:-----|
|Nieprawidłowe żądanie ciała  <br/> |Ten błąd powinno mieć miejsce rzadko, jeśli widzisz ten błąd, spróbuj ponowić operację.  <br/> |
|Wartość mieszania sprzętu dla urządzenia nie są poprawne.  <br/> |Wystąpienie tego błędu oznacza, że wartości podane w pliku CSV dla hash hardwaru jednym z urządzeń nie jest prawidłowe. Najpierw upewnij się, że wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale nadal dzieje się ten błąd, należy poprosić o pomoc z dostawcą sprzętu.  <br/> |
|Urządzenia przypisane do innego lokatora  <br/> |Wystąpienie tego błędu oznacza, że wartości podane w pliku CSV dla numeru seryjnego lub klucz produktu dla jednego lub więcej urządzeń nie jest prawidłowe. Najpierw upewnij się, że wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale nadal dzieje się ten błąd, należy poprosić o pomoc z dostawcą sprzętu.  <br/> |
|Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu  <br/> |Wystąpienie tego błędu oznacza, że urządzenie, które są podczas rejestracji jest już zarejestrowana przez innych organizacji. Aby rozwiązać ten problem, poproś o pomoc z dostawcą sprzętu.  <br/> |
|To urządzenie nie jest obsługiwana dla instalacji za pomocą autopilota  <br/> | Ten błąd oznacza, że urządzenie nie spełnia wymagania dotyczące wdrażania autopilota. Urządzenia muszą spełniać następujące wymagania:  <br/>  System Windows 10 w wersji 1703 lub nowszej.  <br/>  Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.  <br/> |
|Nie znaleziono urządzenia  <br/> |Ten błąd oznacza, że jedno lub więcej urządzeń w pliku CSV nie jest zarejestrowany dla danej organizacji. Aby rozwiązać ten problem, poproś o pomoc z dostawcą sprzętu.  <br/> |
   
