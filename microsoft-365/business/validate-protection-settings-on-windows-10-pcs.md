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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Sprawdź poprawność ustawień ochrony aplikacji usługi Microsoft 365 Business na urządzeniach z systemem Windows 10 i sprawdź, czy użytkownicy nie mogą kopiować danych firmy do plików osobistych lub niezarządzanych aplikacji.
ms.openlocfilehash: 5b798e0335188543fc308553f71085bcde8b7752
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560845"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych

Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników. Jeśli włączono **ustawienie Uniemożliwianie** **użytkownikom kopiowania danych firmowych do plików osobistych i wymuszanie zapisywania plików służbowych w** usłudze OneDrive dla Firm dla urządzeń należących do firmy, można to sprawdzić na urządzeniu użytkownika po nawiązaniu połączenia z usługą Azure AD i zalogowaniu się. 
  
 **Sprawdzanie ustawień połączenia**
  
1. Po zalogowaniu się przy użyciu poświadczeń Microsoft 365 Business i połączeniu z usługą Azure AD zgodnie z opisem w artykule [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md) przejdź do obszaru **Ustawienia systemu Windows** \> **Konta** \> **Uzyskaj dostęp do miejsca pracy lub nauki**. Wybierz pozycję **Połączono z usługą Azure AD \<nazwa dzierżawy\>**, a następnie wybierz pozycję **Informacje**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stronie Managed\> by tenant name **(Zarządzane przez** \<nazwę dzierżawy) można wyświetlić informacje o **połączeniu** zawierające **adres serwera zarządzania,** takie jak ten pokazany na poniższej rysunku. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Sprawdź, czy nie można wkleić danych firmy w aplikacji niezarządzanej**
  
1. Otwórz program Outlook 2016 zainstalowany przez usługi Microsoft 365 Business.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony błąd informujący, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych

 **Sprawdzanie ustawień połączenia**
  
1. Na urządzeniu osobistym systemu Windows 10, na którym użytkownik jest zalogowany jako użytkownik lokalny, przejdź do **pozycji Ustawienia systemu Windows**i kliknij lub naciśnij pozycję Dostęp do **kont** \> **służbowych lub szkolnych**.
    
2. W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.
    
3. W oknie dialogowym **Konfigurowanie konta służbowego** \> **Zaloguj się** wprowadź poświadczenia Microsoft 365 Business.
    
4. Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.
    
    ![Kliknij lub naciśnij pozycję Informacje w oknie dialogowym Konto służbowe.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stronie **Praca programu Access lub szkoła** można wyświetlić informacje o **połączeniu** zawierające **adres serwera zarządzania,** takie jak ten pokazany na poniższej rysunku, i zawierają słowa *wip* i *mam* wewnątrz. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Sprawdź, czy nie można wkleić danych firmy w aplikacji niezarządzanej**
  
1. Otwórz program Outlook 2016 i dodaj konto Microsoft 365 Business, jeśli to konieczne, a następnie zaloguj się przy użyciu poświadczeń Microsoft 365 Business.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony błąd informujący, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    

