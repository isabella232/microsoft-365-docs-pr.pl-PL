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
description: Sprawdź poprawność ustawień ochrony aplikacji usługi Microsoft 365 Business Premium na urządzeniach z systemem Windows 10 i upewnij się, że użytkownicy nie mogą kopiować danych firmowych do plików osobistych ani do aplikacji nieza zarządzanych.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579867"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych

Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników. Jeśli zostało  włączone ustawienie Uniemożliwiaj użytkownikom kopiowanie danych firmowych do plików osobistych i wymusz na nich zapisywanie plików służbowych w usłudze **OneDrive** dla Firm dla urządzeń należących do firmy, możesz to sprawdzić na urządzeniu użytkownika po połączeniu się przez tego użytkownika z usługą Azure AD i zalogowaniu. 
  
 **Sprawdzanie ustawień połączenia**
  
1. Po zalogowaniu się przy użyciu poświadczeń usługi Microsoft 365 Business Premium i nawiązyniu połączenia z usługą Azure AD zgodnie z opisem w tece Konfigurowanie urządzeń z systemem Windows dla użytkowników [usługi Microsoft 365 Business Premium](set-up-windows-devices.md)przejdź do strony Ustawienia systemu **Windows** Konta Dostępu do pracy lub \>  \> **nauki.** Wybierz **pozycję Połączono z \<tenant name\> usługą Azure AD,** a następnie wybierz **pozycję Informacje.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stronie **Zarządzane przez** możesz zobaczyć informacje o połączeniu, które zawierają adres serwera zarządzania, jak pokazano na \<tenant name\> poniższym rysunku.   
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Sprawdzanie, czy nie można wkleić danych firmowych w aplikacji nieza zarządzanych**
  
1. Otwórz program Outlook 2016 zainstalowany przez usługę Microsoft 365 Business Premium.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie z komunikatem, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych

 **Sprawdzanie ustawień połączenia**
  
1. Na urządzeniu osobistym z systemem Windows 10, na którym zalogowano się jako użytkownik lokalny, przejdź do ustawień systemu **Windows** i kliknij lub naciśnij **pozycję** Konta Uzyskaj dostęp do miejsca pracy \> **lub nauki.**
    
2. W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.
    
3. Wprowadź poświadczenia usługi Microsoft 365 Business Premium w oknie dialogowym Konfigurowanie **konta służbowego Zaloguj** \> **się.**
    
4. Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.
    
    ![Kliknij lub naciśnij pozycję Informacje w oknie dialogowym Konto służbowe.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stronie Uzyskaj **dostęp** do pracy  lub nauki widoczne  są informacje o połączeniu, które zawierają adres serwera zarządzania, taki jak przedstawiony na poniższej ilustracji, oraz *wyrazy wip* i *mam* w obrębie. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Sprawdzanie, czy nie można wkleić danych firmowych w aplikacji nieza zarządzanych**
  
1. Otwórz program Outlook 2016 i w razie potrzeby dodaj konto Microsoft 365 Business Premium i zaloguj się przy użyciu poświadczeń platformy Microsoft 365 Business Premium.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie z komunikatem Aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    

