---
title: Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Dowiedz się, jak rozwiązywać problemy z błędami, które mogą być widoczne podczas pracy z plikami urządzeń AutoPilot w usłudze Microsoft 365 Business Premium.
ms.openlocfilehash: 0c0742e5bf17c85cedfb421cabfd87c0e2184ba5
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635049"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Rozwiązywanie problemów z urządzeniami rozwiązania AutoPilot

## <a name="device-file-error-messages"></a>Komunikaty o błędach pliku urządzenia

Oto informacje na temat niektórych błędów, które mogą pojawić się podczas pracy z plikami urządzeń AutoPilot w usłudze Microsoft 365 Business Premium. 
  
|**Kod błędu**|**Poprawka, aby spróbować**|
|:-----|:-----|
|Nieprawidłowa treść żądania  <br/> |Ten błąd powinien się zdarzyć rzadko, jeśli widzisz ten błąd, spróbuj ponownie wykonać operację.  <br/> |
|Wartość skrótu sprzętowego urządzenia nie jest poprawna.  <br/> |Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla skrótu sprzętowego jednego urządzenia jest nieprawidłowa. Najpierw sprawdź, czy wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś dostawcę sprzętu o pomoc.  <br/> |
|Urządzenie przypisane do innej dzierżawy  <br/> |Jeśli widzisz ten błąd, oznacza to, że wartość podana w pliku CSV dla numeru seryjnego lub klucza produktu jednego lub większej liczby urządzeń jest nieprawidłowa. Najpierw sprawdź, czy wartość została wpisana poprawnie. Jeśli uważasz, że wartość jest poprawna, ale ten błąd nadal występuje, poproś dostawcę sprzętu o pomoc.  <br/> |
|Plik CSV zawiera nieprawidłowy numer seryjny lub klucz produktu  <br/> |Jeśli widzisz ten błąd, oznacza to, że urządzenie, które próbujesz zarejestrować, jest już zarejestrowane przez inną organizację. Aby naprawić ten błąd, poproś dostawcę sprzętu o pomoc.  <br/> |
|To urządzenie nie jest obsługiwane do konfiguracji przy użyciu programu AutoPilot  <br/> | Ten błąd oznacza, że urządzenie nie spełnia wymagań dotyczących wdrażania programu AutoPilot. Urządzenia muszą spełniać następujące wymagania:  <br/>  System Windows 10 w wersji 1703 lub nowszej.  <br/>  Nowe urządzenia, które nie zostały za pośrednictwem systemu Windows out-of-box środowiska.  <br/> |
|Nie znaleziono urządzenia  <br/> |Ten błąd oznacza, że co najmniej jedno urządzenie w pliku CSV nie jest zarejestrowane w organizacji. Aby rozwiązać ten problem, poproś dostawcę sprzętu o pomoc.  <br/> |
