---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązywać problemy, które mogą wystąpić podczas pracy z plikami urządzeń rozwiązania AutoPilot w programie Microsoft 365 Business Premium.
ms.openlocfilehash: b74c57acbaa5682f6db97e7d8a090e6e28a40dcc3246f00cacc7984cb52cc758
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809185"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot

## <a name="device-file-error-messages"></a>Komunikaty o błędach pliku urządzenia

Oto informacje dotyczące niektórych błędów, które mogą wystąpić podczas pracy z plikami urządzeń rozwiązania AutoPilot w programie Microsoft 365 Business Premium. 
  
|**Kod błędu**|**Poprawka do wypróbowania**|
|:-----|:-----|
|Nieprawidłowa treść żądania  <br/> |Ten błąd powinien wystąpić rzadko, jeśli jest wyświetlany ten błąd, spróbuj ponownie wykonać operację.  <br/> |
|Wartość skrótu sprzętu dla urządzenia jest poprawna.  <br/> |Jeśli zostanie wyświetlony ten błąd, oznacza to, że wartość podany w pliku CSV skrótu sprzętowego jednego urządzenia jest poprawna. Najpierw sprawdź, czy wartość została wpisowana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś dostawcę sprzętu o pomoc.  <br/> |
|Urządzenie przypisane do innej dzierżawy  <br/> |Jeśli zostanie wyświetlony ten błąd, oznacza to, że wartość podaną w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub większej liczby urządzeń jest poprawna. Najpierw sprawdź, czy wartość została wpisowana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś dostawcę sprzętu o pomoc.  <br/> |
|Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu  <br/> |Jeśli zostanie wyświetlony ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację. Aby naprawić ten błąd, poproś dostawcę sprzętu o pomoc.  <br/> |
|To urządzenie nie jest obsługiwane w konfiguracji za pomocą rozwiązania AutoPilot  <br/> | Ten błąd oznacza, że urządzenie nie spełnia wymagań wdrożeniowych rozwiązania AutoPilot. Urządzenia muszą spełniać następujące wymagania:  <br/>  System Windows 10 w wersji 1703 lub nowszej.  <br/>  Nowe urządzenia, które nie zostały Windows w nowym stanie obsługi.  <br/> |
|Nie znaleziono urządzenia  <br/> |Ten błąd oznacza, że co najmniej jedno urządzenie w pliku CSV nie jest zarejestrowane w Twojej organizacji. Aby rozwiązać ten problem, poproś dostawcę sprzętu o pomoc.  <br/> |
