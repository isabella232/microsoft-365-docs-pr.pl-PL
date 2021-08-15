---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Sprawdź Microsoft 365 Business Premium ustawień ochrony aplikacji na Windows 10 urządzeniach i upewnij się, że użytkownicy nie mogą kopiować danych firmowych do plików osobistych ani do aplikacji nieza zarządzanych.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861760"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych

Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników. Jeśli zostało  włączone ustawienie Uniemożliwiaj użytkownikom kopiowanie danych firmowych do plików osobistych i wymusz na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm dla urządzeń należących do firmy, możesz **to** sprawdzić na urządzeniu użytkownika po połączeniu się przez tego użytkownika z usługą Azure AD i zalogowaniu. 
  
 **Sprawdzanie ustawień połączenia**
  
1. Po zalogowaniu się przy użyciu poświadczeń usługi Microsoft 365 Business Premium i nawiązyniu połączenia z usługą Azure AD zgodnie z opisem w tece Konfigurowanie urządzeń z usługą Windows dla użytkowników [usługi Microsoft 365 Business Premium](set-up-windows-devices.md)przejdź do witryny **Windows Ustawienia** Konta Uzyskaj dostęp do pracy lub \>  \> **nauki.** Wybierz **pozycję Połączono z \<tenant name\> usługą Azure AD,** a następnie wybierz **pozycję Informacje.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stronie **Zarządzane przez** możesz zobaczyć informacje o połączeniu, które zawierają adres serwera zarządzania, jak pokazano na \<tenant name\> poniższym rysunku.   
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Sprawdzanie, czy nie można wkleić danych firmowych w aplikacji nieza zarządzanych**
  
1. Otwórz Outlook 2016 zainstalowany przez aplikację Microsoft 365 Business Premium.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie z komunikatem, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych

 **Sprawdzanie ustawień połączenia**
  
1. Na twoim Windows 10 osobistym, na którym zalogowano Cię jako użytkownik lokalny, przejdź do aplikacji **Windows Ustawienia** i kliknij lub naciśnij **pozycję** Konta Uzyskaj dostęp do miejsca pracy lub \> **nauki.**
    
2. W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.
    
3. Wprowadź poświadczenia Microsoft 365 Business Premium w **oknie dialogowym** Konfigurowanie konta służbowego Lub szkolnego \> **Zaloguj się.**
    
4. Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.
    
    ![Kliknij lub naciśnij pozycję Informacje w oknie dialogowym Konto służbowe.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stronie Uzyskaj **dostęp** do pracy  lub nauki widoczne  są informacje o połączeniu, które zawierają adres serwera zarządzania, taki jak przedstawiony na poniższej ilustracji, oraz *wyrazy wip* i *mam* w obrębie. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Sprawdzanie, czy nie można wkleić danych firmowych w aplikacji nieza zarządzanych**
  
1. Otwórz Outlook 2016 konto i w razie Microsoft 365 Business Premium dodaj konto, a następnie zaloguj się przy użyciu Microsoft 365 Business Premium konta.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie z komunikatem Aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    

