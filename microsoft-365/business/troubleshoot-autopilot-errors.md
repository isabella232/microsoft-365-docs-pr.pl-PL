---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
f1.keywords:
- NOCSH
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
ms.openlocfilehash: 8390f695a3e11386ae2617da4061bed1d8214375
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594213"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot

## <a name="device-file-error-messages"></a>Komunikaty o błędach plików urządzenia

Oto informacje na temat niektórych błędów, które mogą pojawić się podczas pracy z plikami urządzeń AutoPilot w usłudze Microsoft 365 Business. 
  
|**Kod błędu**|**Napraw, aby spróbować**|
|:-----|:-----|
|Nieprawidłowy organ żądania  <br/> |Ten błąd powinien wystąpić rzadko, jeśli widzisz ten błąd, spróbuj ponownie wykonać operację.  <br/> |
|Wartość skrótu sprzętowego dla urządzenia jest niepoprawna.  <br/> |Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla skrótu sprzętowego jednego urządzenia jest poprawna. Najpierw sprawdź, czy wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś o pomoc dostawcę sprzętu.  <br/> |
|Urządzenie przypisane do innej dzierżawy  <br/> |Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub więcej urządzeń jest niepoprawna. Najpierw sprawdź, czy wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś o pomoc dostawcę sprzętu.  <br/> |
|Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu  <br/> |Jeśli widzisz ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację. Aby naprawić ten błąd, poproś o pomoc dostawcę sprzętu.  <br/> |
|To urządzenie nie jest obsługiwane do konfiguracji przy użyciu programu AutoPilot  <br/> | Ten błąd oznacza, że urządzenie nie spełnia wymagań wdrażania programu AutoPilot. Urządzenia muszą spełniać następujące wymagania:  <br/>  System Windows 10 w wersji 1703 lub nowszej.  <br/>  Nowe urządzenia, które nie przeszły przez system Windows out-of-box środowiska.  <br/> |
|Nie znaleziono urządzenia  <br/> |Ten błąd oznacza, że co najmniej jedno urządzenie w pliku CSV nie jest zarejestrowane w organizacji. Aby rozwiązać ten problem, poproś o pomoc dostawcę sprzętu.  <br/> |
