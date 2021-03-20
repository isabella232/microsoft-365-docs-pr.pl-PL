---
title: Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
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
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak za pomocą rozwiązania Windows AutoPilot skonfigurować nowe urządzenia z systemem Windows 10 dla swojej firmy, aby były gotowe do użytku przez pracowników.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913507"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku

Korzystając z rozwiązania Windows AutoPilot, możesz skonfigurować nowe urządzenia z systemem **Windows** 10 dla swojej firmy, aby były gotowe do użycia, gdy podasz je pracownikom.
  
## <a name="device-requirements"></a>Wymagania dotyczące urządzeń

Urządzenia muszą spełniać następujące wymagania:
  
- Windows 10 w wersji 1703 lub nowszej
    
- Nowe urządzenia, które nie są już w stanie obsługi klienta systemu Windows
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)

Jeśli jeszcze nie utworzono grup urządzeń ani profilów, najlepiej rozpocząć pracę, korzystając z przewodnika krok po kroku. Możesz również dodawać [urządzenia i przypisywać](create-and-edit-autopilot-devices.md) [do](create-and-edit-autopilot-profiles.md) nich profile bez korzystania z przewodnika. 
  
1. Przejdź do centrum administracyjnego w stronie <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. W lewym okienku nawigacji wybierz pozycję **Devices** \> **AutoPilot (Rozwiązania rozwiązania Devices AutoPilot).**

    ![W centrum administracyjnym wybierz pozycję urządzenia, a następnie pozycję AutoPilot.](../media/AutoPilot.png)
  
2. Na stronie **AutoPilot (Autopilot)** kliknij lub naciśnij pozycję **Uruchom przewodnik**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na **stronie Przekaż plik csv z listą urządzeń** przejdź do lokalizacji, w której się znajdujesz . CSV, a następnie **otwórz** \> **dalej.** Plik musi zawierać trzy nagłówki:
    
    - Kolumna A: Numer seryjny urządzenia
    
    - Kolumna B: Identyfikator produktu systemu Windows
    
    - Kolumna C: Skrót sprzętowy
    
    Możesz uzyskać te informacje od producenta sprzętu lub wygenerować plik CSV za pomocą skryptu programu [PowerShell Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
    Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](../admin/misc/device-list.md). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**. 
    
> [!NOTE]
> Ten skrypt używa usługi WMI do pobierania właściwości potrzebnych klientowi do zarejestrowania urządzenia za pomocą rozwiązania Windows Autopilot. Zwróć uwagę, że w wynikowym pliku CSV normalne jest nieuzyskanie wartości PKID ,ponieważ nie jest to wymagane do zarejestrowania urządzenia, a wartość PKID w wyjściowym pliku CSV jest całkowicie prawidłowa. Zostanie wypełniony tylko numer seryjny i skrót sprzętowy.
    
4. Na **stronie Przypisywanie profilu** możesz wybrać istniejący profil lub utworzyć nowy. Jeśli nie masz jeszcze konta, zostanie wyświetlony monit o jego utworzenie. 
    
    Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.
    
    Funkcje domyślne są wymagane i ustawiane automatycznie. Funkcje domyślne to:
    
    - Pomiń rejestrację Cortany, usługi OneDrive i OEM.
    
    - Tworzenie środowiska logowania z marką Twojej firmy.
    
    - Połącz urządzenia z kontami usługi Azure Active Directory i automatycznie zarejestruj je, aby być zarządzane przez usługę Microsoft 365 Business Premium.
    
    Aby uzyskać więcej informacji, zobacz [Ustawienia profilu rozwiązania AutoPilot — informacje.](autopilot-profile-settings.md) 
    
5. Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**. 
    
    Wybierz przycisk **Dalej**.
    
6. **Wszystko gotowe oznacza,** że utworzony (lub wybrany) profil zostanie zastosowany do grupy urządzeń utworzonej po przesłaniu listy urządzeń. Ustawienia zostaną wprowadzone, gdy użytkownicy urządzenia zalogują się dalej. Wybierz pozycję **Zamknij**.
