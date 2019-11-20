---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązywać problemy z błędami plików urządzenia AutoPilot.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718704"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot

## <a name="device-file-error-messages"></a>Komunikaty o błędach pliku urządzenia

Oto informacje na temat niektórych błędów, które mogą być widoczne podczas pracy z plikami urządzeń AutoPilot w Microsoft 365 Business. 
  
|**Kod błędu**|**Napraw, aby spróbować**|
|:-----|:-----|
|Nieprawidłowa treść żądania  <br/> |Ten błąd powinien się zdarzyć rzadko, jeśli widzisz ten błąd, spróbuj ponownie wykonać operację.  <br/> |
|Wartość skrótu sprzętowego urządzenia nie jest poprawna.  <br/> |Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla skrótu sprzętowego jednego urządzenia nie jest poprawna. Najpierw sprawdź, czy wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal się dzieje, Poproś dostawcę sprzętu o pomoc.  <br/> |
|Urządzenie przypisane do innego dzierżawcy  <br/> |Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub większej liczby urządzeń nie jest poprawna. Najpierw sprawdź, czy wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal się dzieje, Poproś dostawcę sprzętu o pomoc.  <br/> |
|Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu  <br/> |Jeśli widzisz ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację. Aby naprawić ten błąd, Poproś dostawcę sprzętu o pomoc.  <br/> |
|To urządzenie nie jest obsługiwane w przypadku instalacji przy użyciu funkcji AutoPilot  <br/> | Ten błąd oznacza, że urządzenie nie spełnia wymagań dotyczących wdrażania AutoPilot. Urządzenia muszą spełniać następujące wymagania:  <br/>  System Windows 10 w wersji 1703 lub nowszej.  <br/>  Nowe urządzenia, które nie zostały przez Windows out-of-Box doświadczenia.  <br/> |
|Nie znaleziono urządzenia  <br/> |Ten błąd oznacza, że jeden lub więcej urządzeń w pliku CSV nie jest zarejestrowany w organizacji. Aby rozwiązać ten problem, Poproś dostawcę sprzętu o pomoc.  <br/> |
