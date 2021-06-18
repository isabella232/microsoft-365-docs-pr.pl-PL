---
title: Zabezpieczanie urządzeń z systemem Windows 10
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Dowiedz się więcej o konfigurowaniu ustawień domyślnych zasad dotyczących urządzeń, które Windows 10 urządzenie otrzyma po zalogowaniu się do swojego konta służbowego.
ms.openlocfilehash: 3f85549e722c9aa4196cf50fc02bee2e89506017
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925244"
---
# <a name="secure-windows-10-devices"></a>Zabezpieczanie urządzeń z systemem Windows 10

Ten artykuł dotyczy Microsoft 365 Business Premium.

Konfigurowane w tym miejscu ustawienia są częścią domyślnych zasad dotyczących urządzeń dla systemu Windows 10. Wszyscy użytkownicy, którzy łączą się z urządzeniem Windows 10, w tym z urządzeniami przenośnymi i komputerami, logując się przy użyciu swojego konta służbowego, automatycznie otrzymają te ustawienia. Zalecane jest zaakceptowanie domyślnych zasad podczas instalacji i dodanie w późniejszym terminie zasad dotyczących konkretnych grup użytkowników.
  
## <a name="settings-to-secure-windows-10-devices"></a>Ustawienia zabezpieczające urządzenia z systemem Windows 10

Domyślnie wszystkie ustawienia są **Włączone**. Dostępne są następujące ustawienia:
  


|Ustawienie  <br/> |Opis  <br/> |
|:-----|:-----|
|Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender  <br/> |Wymaga włączenia programu antywirusowego Windows Defender w celu ochrony komputerów przed zagrożeniami związanymi z połączeniem z Internetem.  <br/> |
|Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge  <br/> |Włącza w programie Microsoft Edge ustawienia ułatwiające ochronę użytkowników przed złośliwymi witrynami i złośliwą zawartością do pobrania.  <br/> |
|Pomóż chronić pliki i foldery na komputerach przed nieautoryzowanym dostępem za pomocą funkcji BitLocker  <br/> |Funkcja BitLocker chroni dane przez zaszyfrowanie dysków twardych komputera i zapewnianie ochrony przed ujawnieniem danych w razie zagubienia lub kradzieży komputera. Aby uzyskać więcej informacji, zobacz [Często zadawane pytania dotyczące funkcji BitLocker.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)  <br/> |
|Wyłącz ekran urządzenia po takim czasie bezczynności  <br/> |Zapewnia bezpieczeństwo danych firmowych podczas bezczynności użytkownika. Jeśli użytkownik pracuje w miejscu publicznym, na przykład kawiarni, i odejdzie na chwilę od urządzenia lub skupi uwagę na czymś innym, przypadkowe osoby mogą obejrzeć zawartość ekranu. To ustawienie pozwala kontrolować czas bezczynności użytkownika, po którym ekran zostanie wyłączony.  <br/> |
|