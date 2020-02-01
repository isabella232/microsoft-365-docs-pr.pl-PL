---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić poprawność ustawień ochrony aplikacji usługi Microsoft 365 Business na urządzeniach z systemem Windows 10.
ms.openlocfilehash: e3cd0a1927e0b81c9a97d26196603086b9ea2293
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594960"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony urządzeń na komputerach z systemem Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Sprawdzanie, czy zasady urządzeń z systemem Windows 10 są ustawione

Po [skonfigurowaniu zasad dotyczących urządzeń](protection-settings-for-windows-10-pcs.md)może uchylić zasady na urządzeniach użytkowników nawet kilka godzin. Możesz potwierdzić, że zasady weszły w życie, patrząc na różne ekrany ustawień systemu Windows na urządzeniach użytkowników. Ponieważ użytkownicy nie będą mogli modyfikować ustawień windows update i Windows Defender Antivirus na swoich urządzeniach z systemem Windows 10, wiele opcji zostanie wyszarzonych.
  
1. Przejdź do **opcji Ustawienia** \> **Aktualizuj &amp; zabezpieczenia** \> **Windows Update** \> **Restart** i upewnij się, że wszystkie ustawienia są wyszarzone. 
    
    ![Wszystkie opcje ponownego uruchamiania są wyszarzone.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Przejdź do **ustawienia** \> **Aktualizuj &amp; zabezpieczenia** \> **Windows Update** \> Zaawansowane **opcje** i upewnij się, że wszystkie ustawienia są wyszarzone. 
    
    ![Opcje aktualizacji zaawansowanych systemu Windows są wyszarzone.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Przejdź do **ustawienia** \> **Aktualizuj &amp; zabezpieczenia** \> **Windows Update** \> **Opcje** \> zaawansowane **Wybierz sposób dostarczania aktualizacji**.
    
    Upewnij się, że widzisz komunikat (na czerwono), że niektóre ustawienia są ukryte lub zarządzane przez organizację, a wszystkie opcje są wyszarzone.
    
    ![Wybierz sposób dostarczania aktualizacji strona wskazuje, że ustawienia są ukryte lub zarządzane przez organizację.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Aby otworzyć Centrum zabezpieczeń usługi Windows Defender, przejdź do **pozycji Ustawienia** \> **Aktualizuj &amp; zabezpieczenia usługi Windows** \> **Defender** \> kliknij pozycję Otwórz zabezpieczenia programu **Windows Defender Security Center** \> **Virus &amp; Virus** \> **protection Virus &amp; threat protection settings**. 
    
5. Sprawdź, czy wszystkie opcje są wyszarzone. 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarzone.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tematy pokrewne

[Dokumentacja i zasoby dotyczące usługi Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Rozpoczynanie pracy z usługą Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Zarządzanie usługą Microsoft 365 Business](manage.md)
  
[Konfigurowanie komputerów PC z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
  

