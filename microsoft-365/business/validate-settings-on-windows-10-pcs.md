---
title: Sprawdzanie poprawności ustawień ochrony aplikacji dla Windows 10 PC
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić Microsoft 365 ustawienia ochrony aplikacji dla firm miały wpływ na ustawienia ochrony aplikacji Windows 10 urządzeniach.
ms.openlocfilehash: 0b896ae21139adcc425295f31de9232f65380d692a46bd1ef9f81d4516e0e9ec
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861658"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony urządzeń dla Windows 10 PC

## <a name="verify-that-windows-10-device-policies-are-set"></a>Sprawdzanie, czy Windows 10 urządzenia są ustawione

Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może upłynieć kilka godzin, aż te zasady zajdą w życie na urządzeniach użytkowników. Aby potwierdzić, że zasady te obowiązywały, możesz sprawdzić, Windows Ustawienia ekranów na urządzeniach użytkowników. Ponieważ użytkownicy nie będą mogli modyfikować ustawień aktualizacji Windows i ustawień Program antywirusowy Windows Defender na swoich Windows 10 urządzeniach, wiele opcji zostanie wyszarzeni.
  
1. Przejdź do **Ustawienia** Opcje ponownego uruchamiania Windows aktualizacji i upewnij się, że wszystkie ustawienia \> **&amp;** \>  \>  są wyszarowane. 
    
    ![Wszystkie opcje Uruchom ponownie są wyszarowane.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Przejdź do **Ustawienia** Opcje aktualizacji Windows Zaawansowane i upewnij się, że wszystkie ustawienia \> **&amp;** \>  \>  są wyszarowane. 
    
    ![Windows Opcje aktualizacji zaawansowanych są wyszarowane.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Przejdź do **Ustawienia** Opcje zaawansowane aktualizacji Windows Opcje aktualizacji Wybierz \> **&amp;** sposób \>  \>  \> **dostarczenia aktualizacji.**
    
    Potwierdź, że widzisz komunikat (kolor czerwony), że niektóre ustawienia są ukryte lub zarządzane przez Twoją organizację, a wszystkie opcje są wyszarowane.
    
    ![Strona Wybieranie sposobu dostarczenia aktualizacji wskazuje, że ustawienia są ukryte lub zarządzane przez Organizację.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Aby otworzyć Centrum zabezpieczeń Windows Defender,  przejdź do Ustawienia aktualizacji zabezpieczeń i Windows Defender pozycję Otwórz Windows Defender Ochronę wątku wirusów ustawieniami ochrony przed zagrożeniami \> **&amp;** \>  \>  \> **&amp;** \> **&amp; antywirusowymi.** 
    
5. Sprawdź, czy wszystkie opcje są wyszarowane. 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarowane.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tematy pokrewne

[Microsoft 365 i zasoby dla firm](./index.yml)
  
[Wprowadzenie do usługi Microsoft 365 dla firm](microsoft-365-business-overview.md)
  
[Zarządzanie Microsoft 365 dla firm](manage.md)
  
[Konfigurowanie komputerów PC z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
