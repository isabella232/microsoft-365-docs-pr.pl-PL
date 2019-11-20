---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
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
description: Dowiedz się, jak zweryfikować ustawienia ochrony aplikacji biznesowych firmy Microsoft 365 na urządzeniach z systemem Windows 10.
ms.openlocfilehash: b8793ab7f77bbc7f608f237e2455f6fd12c3bb26
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721805"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony urządzenia na komputerach z systemem Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Sprawdź, czy zasady urządzenia systemu Windows 10 są ustawione

Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może potrwać do kilku godzin, aby zasady zostały uwzględnione na urządzeniach użytkowników. Możesz potwierdzić, że zasady zostały uwzględnione, patrząc na różne ekrany ustawień systemu Windows na urządzeniach użytkowników. Ponieważ użytkownicy nie będą mogli modyfikować ustawień programu Windows Update i Windows Defender Antivirus na swoich urządzeniach z systemem Windows 10, wiele opcji będzie wyszarzony.
  
1. Przejdź do **opcji Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Uruchom ponownie** i Potwierdź, że wszystkie ustawienia są wyszarzone. 
    
    ![Wszystkie opcje ponownego uruchomienia są wyszarzone.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Przejdź do **Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Zaawansowane opcje** i potwierdzić, że wszystkie ustawienia są wyszarzone. 
    
    ![Opcje zaawansowanych aktualizacji systemu Windows są wyszarzone.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Przejdź do **Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Zaawansowane opcje** \> **Wybierz sposób dostarczania aktualizacji**.
    
    Potwierdź, że możesz zobaczyć wiadomość (na czerwono), że niektóre ustawienia są ukryte lub zarządzane przez organizację, a wszystkie opcje są wyszarzone.
    
    ![Wybierz sposób dostarczania aktualizacji strony wskazuje, że ustawienia są ukryte lub zarządzane przez organizację.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Aby otworzyć Centrum zabezpieczeń systemu Windows Defender, przejdź do **ustawień** \> **aktualizacji &amp; zabezpieczeń** \> **systemu Windows Defender** \> kliknij przycisk **Otwórz Windows Defender Security Center** \> **Virus &amp; Thread ochrona** \> ochrona **przed wirusami &amp; ochrony przed zagrożeniami**. 
    
5. Sprawdź, czy wszystkie opcje są wyszarzone. 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarzone.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tematy pokrewne

[Dokumentacja i zasoby dotyczące usługi Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Rozpoczynanie pracy z usługą Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Zarządzanie usługą Microsoft 365 Business](manage.md)
  
[Konfigurowanie komputerów PC z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
  

