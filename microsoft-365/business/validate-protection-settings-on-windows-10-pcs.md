---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak zweryfikować ustawienia ochrony aplikacji biznesowych firmy Microsoft 365 w urządzeniach z systemem Windows 10.
ms.openlocfilehash: c54b053c1f6efbca8fd02431c416793a044c6821
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721865"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach firmowych

Po [skonfigurowaniu zasad ochrony aplikacji](protection-settings-for-windows-10-devices.md) może upłynąć kilka godzin, zanim te zasady zaczną obowiązywać na urządzeniach użytkowników. Jeśli **włączono** **uniemożliwić użytkownikom kopiowanie danych firmowych do plików osobistych i wymusić ich zapisać pliki robocze do OneDrive dla firmy** ustawienie dla urządzeń należących do firmy, można to sprawdzić na urządzeniu użytkownika po nawiązaniu połączenia z usługą Azure AD i zalogowany. 
  
 **Sprawdzanie ustawień połączenia**
  
1. Po zalogowaniu się przy użyciu poświadczeń Microsoft 365 Business i połączeniu z usługą Azure AD zgodnie z opisem w artykule [Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business](set-up-windows-devices.md) przejdź do obszaru **Ustawienia systemu Windows** \> **Konta** \> **Uzyskaj dostęp do miejsca pracy lub nauki**. Wybierz pozycję **Połączono z usługą Azure AD \<nazwa dzierżawy\>**, a następnie wybierz pozycję **Informacje**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na **zarządzanych przez** \<nazwę\> dzierżawcy strony, możesz zobaczyć informacje o **połączeniu** , który zawiera **adres serwera zarządzania** , jak pokazano na poniższej ilustracji. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Sprawdź, czy nie można wkleić danych firmowych w aplikacji niezarządzanej**
  
1. Otwórz program Outlook 2016 zainstalowany przez usługi Microsoft 365 Business.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Zostanie wyświetlony komunikat o błędzie informujący, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Potwierdzanie, że użytkownicy nie mogą skopiować danych firmowych do plików osobistych na urządzeniach osobistych

 **Sprawdzanie ustawień połączenia**
  
1. Na urządzeniu osobistym z systemem Windows 10, w którym użytkownik jest zalogowany jako użytkownik lokalny, przejdź do pozycji **Ustawienia systemu Windows**i kliknij **** \> lub naciśnij pozycję **dostęp do kont w pracy lub szkole**.
    
2. W obszarze **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Połącz**.
    
3. W oknie dialogowym **Konfigurowanie konta służbowego** \> **Zaloguj się** wprowadź poświadczenia Microsoft 365 Business.
    
4. Na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** wybierz pozycję **Konto służbowe**, a następnie pozycję **Informacje**.
    
    ![Kliknij lub naciśnij pozycję informacje w oknie dialogowym konto służbowe lub szkolne.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stronie **dostęp do pracy lub szkoły** możesz zobaczyć **Informacje o połączeniu** , które zawierają **adres serwera zarządzania** , taki jak pokazany na poniższym rysunku, i zawiera słowa *PWT* i *mam* w. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Sprawdź, czy nie można wkleić danych firmowych w aplikacji niezarządzanej**
  
1. Otwórz program Outlook 2016 i dodaj konto Microsoft 365 Business, jeśli to konieczne, a następnie zaloguj się przy użyciu poświadczeń Microsoft 365 Business.
    
2. Otwórz wiadomość e-mail, a następnie skopiuj z niej jakąś zawartość.
    
    Otwórz Notatnik i spróbuj wkleić w nim tę zawartość.
    
    Otrzymasz komunikat o błędzie informujący, że aplikacja nie może uzyskać dostępu do zawartości.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Można jednak wkleić tę zawartość w programie Word 2016.
    

