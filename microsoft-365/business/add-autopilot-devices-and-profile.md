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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak używać programu Windows AutoPilot do konfigurowania nowych urządzeń z systemem Windows 10 dla Twojej firmy.
ms.openlocfilehash: 563c3bbbc9f69996778417b35cfaa64d089770ef
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287600"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku

Za pomocą programu Windows AutoPilot można skonfigurować **nowe** urządzenia z systemem Windows 10 dla firmy, aby były gotowe do użytku produktywnego, gdy tylko podasz je pracownikom.
  
## <a name="device-requirements"></a>Wymagania dotyczące urządzeń

Urządzenia muszą spełniać następujące wymagania:
  
- System Windows 10 w wersji 1703 lub nowszej.
    
- Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji

[![Etykieta, aby poinformować, że centrum admin zmienia się i można znaleźć więcej szczegółów na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Jeśli nie utworzono jeszcze grup urządzeń ani profilów, najlepiej rozpocząć pracę przy użyciu przewodnika krok po kroku. Można jednak [dodać urządzenia](create-and-edit-autopilot-devices.md) i [przypisać do nich profile](create-and-edit-autopilot-profiles.md) bez używania tego przewodnika. 
  
1. Przejdź do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. Na lewej NAV wybierz **urządzenia** \> **autopilot**.

    ![W centrum administracyjnym wybierz urządzenia, a następnie AutoPilot.](media/AutoPilot.png)
  
2. Na stronie **autopilot** kliknij lub naciśnij pozycję **Uruchom przewodnik**.
    
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
    