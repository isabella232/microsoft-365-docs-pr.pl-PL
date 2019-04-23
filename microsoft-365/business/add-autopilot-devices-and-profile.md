---
title: Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak autopilota systemu Windows służy do definiowania nowych urządzeń Windows 10 dla Twojej firmy.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277147"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku

Rozwiązanie Windows AutoPilot pozwala skonfigurować nowe firmowe urządzenia z systemem Windows 10, tak aby były gotowe do użycia w środowisku produkcyjnym od razu po przekazaniu ich pracownikom.
  
## <a name="device-requirements"></a>Wymagania dotyczące urządzeń

Urządzenia muszą spełniać następujące wymagania:
  
- System Windows 10 w wersji 1703 lub nowszej.
    
- Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji

Jeśli nie utworzono jeszcze grup urządzeń ani profilów, najlepiej rozpocząć pracę przy użyciu przewodnika krok po kroku. Można jednak [dodać urządzenia](create-and-edit-autopilot-devices.md) i [przypisać do nich profile](create-and-edit-autopilot-profiles.md) bez używania tego przewodnika. 
  
1. W centrum administracyjnym usługi Microsoft 365 Business przejdź do karty **Akcje urządzenia** i wybierz pozycję **Wdróż system Windows za pomocą rozwiązania Autopilot**.
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. Na stronie **Przygotowywanie systemu Windows** kliknij lub naciśnij pozycję **Uruchom przewodnik**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na stronie **Przekazywanie pliku csv z listą urządzeń** przejdź do lokalizacji, w której znajduje się przygotowany plik CSV, a następnie wybierz pozycję **Otwórz** \> **Dalej**. Plik powinien zawierać trzy nagłówki:
    
  - Kolumna A: Numer seryjny urządzenia
    
  - Kolumna B: Identyfikator produktu systemu Windows
    
  - Kolumna C: Skrót sprzętowy
    
    Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik CSV. 
    
    Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**. 
    
4. Na stronie **Przypisywanie profilu** możesz utworzyć nowy lub wybrać istniejący profil. Jeśli nie masz jeszcze profilu, zostanie wyświetlony monit o jego utworzenie. 
    
    Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.
    
    Funkcje domyślne są wymagane i zostaną ustawione automatycznie. Funkcje domyślne to:
    
  - Rejestracja Cortany, usługi OneDrive i producenta OEM jest pomijana.
    
  - Tworzenie środowiska logowania z marką Twojej firmy.
    
  - Urządzenia zostaną połączone z kontami usługi Azure Active Directory i automatycznie zarejestrowane na potrzeby zarządzania przez usługę Microsoft 365 Business.
    
    Aby uzyskać więcej informacji, zobacz
    
    [Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md) . 
    
5. Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**. 
    
    Wybierz przycisk **Dalej**.
    
6. Wyświetlenie strony **Gotowe** oznacza, że utworzony (lub wybrany) profil zostanie zastosowany do grupy urządzeń utworzonej po przekazaniu listy urządzeń. Ustawienia te zostaną zastosowane przy następnym logowaniu się użytkowników tych urządzeń. Wybierz pozycję **Zamknij**.
    