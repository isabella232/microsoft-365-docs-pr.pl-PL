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
description: Dowiedz się, jak rozwiązywać problemy, które mogą wystąpić podczas pracy z plikami urządzeń rozwiązania AutoPilot w uwitrynie Microsoft 365 Business Premium.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578092"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot

## <a name="device-file-error-messages"></a>Komunikaty o błędach pliku urządzenia

Oto informacje na temat niektórych błędów, które mogą wystąpić podczas pracy z plikami urządzeń rozwiązania AutoPilot w uwitrynie Microsoft 365 Business Premium. 
  
|**Kod błędu**|**Poprawka do wypróbowania**|
|:-----|:-----|
|Nieprawidłowa treść żądania  <br/> |Ten błąd powinien wystąpić rzadko, jeśli jest wyświetlany ten błąd, spróbuj ponownie wykonać operację.  <br/> |
|Wartość skrótu sprzętu dla urządzenia jest poprawna.  <br/> |Jeśli zostanie wyświetlony ten błąd, oznacza to, że wartość podany w pliku CSV skrótu sprzętowego jednego urządzenia jest poprawna. Najpierw sprawdź, czy wartość została wpisowana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś dostawcę sprzętu o pomoc.  <br/> |
|Urządzenie przypisane do innej dzierżawy  <br/> |Jeśli zostanie wyświetlony ten błąd, oznacza to, że wartość podaną w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub większej liczby urządzeń jest poprawna. Najpierw sprawdź, czy wartość została wpisowana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś dostawcę sprzętu o pomoc.  <br/> |
|Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu  <br/> |Jeśli zostanie wyświetlony ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację. Aby naprawić ten błąd, poproś dostawcę sprzętu o pomoc.  <br/> |
|To urządzenie nie jest obsługiwane w konfiguracji za pomocą rozwiązania AutoPilot  <br/> | Ten błąd oznacza, że urządzenie nie spełnia wymagań wdrożeniowych rozwiązania AutoPilot. Urządzenia muszą spełniać następujące wymagania:  <br/>  System Windows 10 w wersji 1703 lub nowszej.  <br/>  Nowe urządzenia, które nie zostały przez system Windows w wersji "od 1 do 3".  <br/> |
|Nie znaleziono urządzenia  <br/> |Ten błąd oznacza, że co najmniej jedno urządzenie w pliku CSV nie jest zarejestrowane w Twojej organizacji. Aby rozwiązać ten problem, poproś dostawcę sprzętu o pomoc.  <br/> |
