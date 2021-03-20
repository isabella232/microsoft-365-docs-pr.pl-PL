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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić, czy ustawienia ochrony aplikacji platformy Microsoft 365 dla firm obowiązywały na urządzeniach użytkowników z systemem Windows 10.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912419"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony urządzeń na komputerach z systemem Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Sprawdzanie, czy ustawiono zasady dotyczące urządzeń z systemem Windows 10

Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może upłynieć kilka godzin, aż te zasady zajdą w życie na urządzeniach użytkowników. Aby potwierdzić, że zasady te obowiązywały, możesz zobaczyć różne ekrany ustawień systemu Windows na urządzeniach użytkowników. Ponieważ użytkownicy nie będą mogli modyfikować ustawień oprogramowania antywirusowego Windows Update i Windows Defender na urządzeniach z systemem Windows 10, wiele opcji zostanie wyszarowanych.
  
1. Przejdź do opcji **Ustawienia** \> **Aktualizacja &amp; zabezpieczeń** \> **Uruchom ponownie usługę Windows Update** i upewnij się, że wszystkie ustawienia są \>  wyszarowane. 
    
    ![Wszystkie opcje Uruchom ponownie są wyszarowane.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Przejdź do opcji **Ustawienia** Zaktualizuj zabezpieczenia Windows Update Zaawansowane i upewnij się, że wszystkie ustawienia \> **&amp;** \>  \>  są wyszarowane. 
    
    ![Opcje aktualizacji zaawansowanych systemu Windows są wyszarowane.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Przejdź  do ustawień \> **Aktualizacja &amp; zabezpieczeń Opcje** \> **zaawansowane usługi Windows Update** Wybierz sposób dostarczenia \>  \> **aktualizacji.**
    
    Potwierdź, że widzisz komunikat (kolor czerwony), że niektóre ustawienia są ukryte lub zarządzane przez Twoją organizację, a wszystkie opcje są wyszarowane.
    
    ![Strona Wybieranie sposobu dostarczenia aktualizacji wskazuje, że ustawienia są ukryte lub zarządzane przez Organizację.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Aby otworzyć usługę Windows Defender Security Center, przejdź do **ustawienia** Zaktualizuj zabezpieczenia Programu Windows Defender, kliknij pozycję Otwórz ochronę wątku wirusów programu \> **&amp;** \>  \> Windows  \> **Defender: &amp;** \> **ustawienia ochrony przed zagrożeniami w &amp; programie Windows Defender.** 
    
5. Sprawdź, czy wszystkie opcje są wyszarowane. 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarowane.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Tematy pokrewne

[Dokumentacja i zasoby dotyczące platformy Microsoft 365 dla firm](./index.yml)
  
[Wprowadzenie do platformy Microsoft 365 dla firm](microsoft-365-business-overview.md)
  
[Zarządzanie usługą Microsoft 365 dla firm](manage.md)
  
[Konfigurowanie komputerów PC z systemem Windows 10](protection-settings-for-windows-10-pcs.md)
