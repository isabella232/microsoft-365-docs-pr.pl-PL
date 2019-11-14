---
title: Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak używać programu Windows AutoPilot do konfigurowania nowych urządzeń z systemem Windows 10 dla Twojej firmy.
ms.openlocfilehash: 5f40dac57285b83da57d4506bac58e562475522c
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323100"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku

Za pomocą programu Windows AutoPilot można skonfigurować **nowe** urządzenia z systemem Windows 10 dla firmy, aby były gotowe do użycia w przypadku nadania ich pracownikom.
  
## <a name="device-requirements"></a>Wymagania dotyczące urządzeń

Urządzenia muszą spełniać następujące wymagania:
  
- Windows 10, wersja 1703 lub nowsza
    
- Nowe urządzenia, które nie zostały przez Windows out-of-Box doświadczenie
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Jeśli nie utworzono jeszcze grup urządzeń lub profilów, najlepszym sposobem na rozpoczęcie korzystania z tej funkcji jest przewodnik krok po kroku. Można również [dodawać urządzenia](create-and-edit-autopilot-devices.md) i [przypisywać profile](create-and-edit-autopilot-profiles.md) do nich bez korzystania z przewodnika. 
  
1. Przejdź do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. W okienku nawigacyjnym z lewej strony wybierz **urządzenia** \> **autopilot**.

    ![W centrum administracyjnym wybierz urządzenia, a następnie AutoPilot.](media/AutoPilot.png)
  
2. Na stronie **autopilot** kliknij lub naciśnij pozycję **Uruchom przewodnik**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na stronie **Prześlij plik. CSV z listą urządzeń** przejdź do lokalizacji, w której masz przygotowane. Plik CSV, a następnie **Otwórz** \> **Następny**. Plik musi mieć trzy nagłówki:
    
    - Kolumna A: Numer seryjny urządzenia
    
    - Kolumna B: Identyfikator produktu systemu Windows
    
    - Kolumna C: Skrót sprzętowy
    
    Można uzyskać te informacje od dostawcy sprzętu lub można użyć [skryptu Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) do generowania pliku CSV. 
    
    Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**. 
    
4. Na stronie **Przypisywanie profilu** można wybrać istniejący profil lub utworzyć nowy. Jeśli jeszcze go nie masz, zostaniesz poproszony o jego utworzenie. 
    
    Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.
    
    Domyślne funkcje są wymagane i są ustawiane automatycznie. Funkcje domyślne to:
    
    - Pomiń rejestrację Cortany, OneDrive i OEM.
    
    - Tworzenie środowiska logowania z marką Twojej firmy.
    
    - Połącz swoje urządzenia z kontami usługi Azure Active Directory i automatycznie zarejestruj je, aby były zarządzane przez firmę Microsoft 365 Business.
    
    Aby uzyskać więcej informacji, zobacz informacje [o ustawieniach profilu AutoPilot](autopilot-profile-settings.md). 
    
5. Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**. 
    
    Wybierz przycisk **Dalej**.
    
6. **Skończysz wskazuje,** że profil utworzony (lub wybrany) zostanie zastosowany do utworzonej grupy urządzeń przez przesłanie listy urządzeń. Ustawienia będą obowiązywać, gdy użytkownicy urządzenia zalogują się dalej. Wybierz pozycję **Zamknij**.
    