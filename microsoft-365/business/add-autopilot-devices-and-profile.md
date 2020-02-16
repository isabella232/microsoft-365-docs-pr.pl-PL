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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak skonfigurować nowe urządzenia z systemem Windows 10 dla firmy za pomocą programu AutoPilot systemu Windows 10.
ms.openlocfilehash: e5774b1e2079a5249e0f6e9e7142de19268253b5
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42068552"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku

Za pomocą programu AutoPilot systemu Windows można skonfigurować **nowe** urządzenia z systemem Windows 10 dla Twojej firmy, aby były gotowe do użycia, gdy dasz je pracownikom.
  
## <a name="device-requirements"></a>Wymagania dotyczące urządzeń

Urządzenia muszą spełniać następujące wymagania:
  
- Windows 10, wersja 1703 lub nowsza
    
- Nowe urządzenia, które nie przeszły przez system Windows gotowe do obsługi
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji

[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Jeśli nie utworzono jeszcze grup urządzeń ani profilów, najlepszym sposobem na rozpoczęcie pracy jest użycie przewodnika krok po kroku. Można również [dodawać do](create-and-edit-autopilot-devices.md) nich urządzenia i [przypisywać do](create-and-edit-autopilot-profiles.md) nich profile bez użycia przewodnika. 
  
1. Przejdź do centrum <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administracyjnego pod adresem .

2. W lewym okienku nawigacji wybierz pozycję **Urządzenia** \> **Autopilot**.

    ![W centrum administracyjnym wybierz urządzenia, a następnie Autopilota.](../media/AutoPilot.png)
  
2. Na stronie **Autopilot** kliknij lub naciśnij **pozycję Przewodnik startowy**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na **stronie Prześlij plik csv z listą urządzeń** przejdź do lokalizacji, w której masz przygotowane . CSV, a następnie **otwórz** \> **dalej**. Plik musi mieć trzy nagłówki:
    
    - Kolumna A: Numer seryjny urządzenia
    
    - Kolumna B: Identyfikator produktu systemu Windows
    
    - Kolumna C: Skrót sprzętowy
    
    Te informacje można uzyskać od dostawcy sprzętu lub użyć [skryptu Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) do wygenerowania pliku CSV. 
    
    Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**. 
    
4. Na stronie **Przypisywanie profilu** można wybrać istniejący profil lub utworzyć nowy. Jeśli jeszcze go nie masz, zostanie wyświetlony monit o jego utworzenie. 
    
    Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.
    
    Funkcje domyślne są wymagane i są ustawiane automatycznie. Funkcje domyślne to:
    
    - Pomiń cortanę, onedrive i rejestrację OEM.
    
    - Tworzenie środowiska logowania z marką Twojej firmy.
    
    - Połącz urządzenia z kontami usługi Azure Active Directory i automatycznie rejestruj je, aby były zarządzane przez firmę Microsoft 365 Business.
    
    Aby uzyskać więcej informacji, zobacz [Ustawienia profilu autopilota](autopilot-profile-settings.md). 
    
5. Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**. 
    
    Wybierz przycisk **Dalej**.
    
6. **Gotowe zdjęcie** wskazuje, że utworzony (lub wybrany) profil zostanie zastosowany do utworzonej grupy urządzeń, przesyłając listę urządzeń. Ustawienia będą obowiązywać, gdy użytkownicy urządzenia zalogują się w następnej kolejności. Wybierz pozycję **Zamknij**.
    
