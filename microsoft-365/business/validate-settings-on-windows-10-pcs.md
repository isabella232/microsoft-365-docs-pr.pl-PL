---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić poprawność ustawień ochrony aplikacji Microsoft 365 Business w urządzeniach 10 systemu Windows.
ms.openlocfilehash: db05c86bd75cc30e22e025034a3dab478d0f5365
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982707"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Sprawdź poprawność ustawień ochrony urządzenia na komputerach z systemem Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Sprawdź, czy są ustawione zasady dotyczące urządzeń Windows 10

Po [Ustawianie zasad urządzeń](protection-settings-for-windows-10-pcs.md)może potrwać do kilku godzin dla zasady obowiązywały na urządzeniach użytkowników. Możesz potwierdzić, że zasady weszło w życie patrząc na różnych ekranach ustawienia systemu Windows na urządzeniach użytkowników. Ponieważ użytkownicy nie będą mogli modyfikować ustawień usługi Windows Update i Windows Defender Antivirus na swoich urządzeniach Windows 10, wiele z tych opcji będzie wyszarzona.
  
1. Przejdź do **opcji ustawienia** \> **Aktualizacja &amp; zabezpieczenia** \> **Windows Update** \> **Opcje ponownego uruchamiania** i Potwierdź, że wszystkie ustawienia są wyszarzone. 
    
    ![Wszystkie opcje ponownego uruchomienia są wyszarzone.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Przejdź do **opcji ustawienia** \> **Aktualizacja &amp; zabezpieczenia** \> **Witryny Windows Update** \> **Opcje zaawansowane** i Potwierdź, że wszystkie ustawienia są wyszarzone. 
    
    ![Opcje zaawansowane systemu Windows aktualizacje są wyszarzone.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Przejdź do **opcji ustawienia** \> **Aktualizacja &amp; zabezpieczenia** \> **Windows Update** \> **Opcje zaawansowane** \> **Wybierz, w jaki sposób aktualizacje są pobierane**.
    
    Upewnij się, czy widzisz komunikat (na czerwono), niektóre ustawienia są ukryte lub zarządzanych przez własną organizację, a wszystkie opcje są wyszarzone.
    
    ![Wybierz sposób dostarczane są aktualizacje strony wskazuje ustawienia są ukryte lub zarządzanych przez własną organizację.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Aby otworzyć Centrum zabezpieczeń systemu Windows Defender, przejdź do **ustawień** \> **Aktualizacja &amp; zabezpieczenia** \> **Programu Windows Defender** \> kliknij **Otwórz Windows Defender Centrum zabezpieczeń** \> **wirus &amp; wątku Ochrona** \> **wirus &amp; zagrożenie ustawienia ochrony**. 
    
5. Sprawdź, czy wszystkie opcje są wyszarzone. 
    
    ![Ustawienia ochrony wirusów i zagrożeń są wyszarzone.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tematy pokrewne

[Dokumentacja i zasoby dotyczące usługi Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Rozpoczynanie pracy z usługą Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Zarządzanie usługą Microsoft 365 Business](manage.md)
  
[Konfigurowanie komputerów PC z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
  

