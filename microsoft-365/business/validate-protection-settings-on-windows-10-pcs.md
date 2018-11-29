---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić poprawność ustawień ochrony aplikacji Microsoft 365 Business w urządzeniach 10 systemu Windows.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983297"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych

Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników. Jeśli zostało **włączone** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm** dla urządzeń należących do firmy, można to sprawdzić na urządzeniu użytkownika po połączeniu się przez niego z usługą Azure AD i zalogowaniu. 
  
 **Sprawdzanie ustawień połączenia**
  
1. Po zalogowaniu się przy użyciu poświadczeń Microsoft 365 Business i połączeniu z usługą Azure AD zgodnie z opisem w artykule [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md) przejdź do obszaru **Ustawienia systemu Windows** \> **Konta** \> **Uzyskaj dostęp do miejsca pracy lub nauki**. Wybierz pozycję **Połączono z usługą Azure AD \<nazwa dzierżawy\>**, a następnie wybierz pozycję **Informacje**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stronie **Zarządzane przez** \<nazwa dzierżawy\> wyświetlana jest sekcja **Informacje o połączeniu** zawierająca pozycję **Adres serwera zarządzania**, jak na przykład ta przedstawiona na poniższej ilustracji. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Potwierdzanie, że nie można skopiować danych firmowych do aplikacji niezarządzanej**
  
1. Otwórz program Outlook 2016 zainstalowany przez usługi Microsoft 365 Business.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie z informacją, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych

 **Sprawdzanie ustawień połączenia**
  
1. Na urządzeniu osobistym z systemem Windows 10, na którym zalogowano się jako użytkownik lokalny, przejdź do obszaru **Ustawienia systemu Windows**, a następnie kliknij lub naciśnij pozycję **Konta** \> **Uzyskaj dostęp do miejsca pracy lub nauki**.
    
2. W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.
    
3. W oknie dialogowym **Konfigurowanie konta służbowego** \> **Zaloguj się** wprowadź poświadczenia Microsoft 365 Business.
    
4. Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wyświetlana jest sekcja **Informacje o połączeniu** zawierająca pozycję **Adres serwera zarządzania**, jak na przykład ta przedstawiona na poniższej ilustracji, wraz z wyrazami  *wip*  i  *mam*  . 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Potwierdzanie, że nie można skopiować danych firmowych do aplikacji niezarządzanej**
  
1. Otwórz program Outlook 2016 i dodaj konto Microsoft 365 Business, jeśli to konieczne, a następnie zaloguj się przy użyciu poświadczeń Microsoft 365 Business.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie z informacją, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    

