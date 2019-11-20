---
title: Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Dowiedz się, jak skonfigurować urządzenia z systemem Windows 10 Pro dla użytkowników Microsoft 365 Business. '
ms.openlocfilehash: f929c64b00e4ebf24e9f82fcfea433119abf2f1c
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718884"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business

## <a name="prerequisites"></a>Wymagania wstępne

Zanim będzie można skonfigurować urządzenia z systemem Windows dla użytkowników usługi Microsoft 365 Business należy się upewnić, że na wszystkich tych urządzeniach jest zainstalowany system Windows 10 Pro w wersji 1703 (aktualizacja dla twórców). System Windows 10 Pro stanowi wymaganie wstępne w przypadku wdrażania systemu Windows 10 Business  zestawu usług w chmurze i funkcji zarządzania urządzeniami  który uzupełnia system Windows 10 Pro i udostępnia mechanizmy scentralizowanego zarządzania i zabezpieczeń usługi Microsoft 365 Business.
  
Jeśli na urządzeniach z systemem Windows działa system Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, to subskrypcja usługi Microsoft 365 Business uprawnia do uaktualnienia do systemu Windows 10.
  
Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).
  
Zobacz [Sprawdź, czy urządzenie jest podłączone do usługi Azure AD](#verify-the-device-is-connected-to-azure-ad) , aby zweryfikować, że masz uaktualnienie, lub upewnij się, że uaktualnienie działało. 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji

Gdy wszystkie urządzenia z systemem Windows w organizacji zostały uaktualnione do systemu Windows 10 Pro twórcy aktualizacji lub są już uruchomione Windows 10 Pro twórcy aktualizacji, można przyłączyć te urządzenia do usługi Azure Active Directory w organizacji. Po przyłączeniu urządzeń zostaną one automatycznie uaktualnione do systemu Windows 10 Business, który jest częścią subskrypcji Microsoft 365 Business.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro

W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.
  
1. Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Na tej stronie wybierz opcję **Konfiguruj dla organizacji**, a następnie wprowadź nazwę użytkownika i hasło dla usługi Microsoft 365 Business. 
    
3. Dokończ konfigurację urządzenia z systemem Windows 10.
    
   Gdy to zrobisz, użytkownik będzie połączony z usługą Azure AD organizacji. Zobacz [Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD](#verify-the-device-is-connected-to-azure-ad), aby się upewnić. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Urządzenie już skonfigurowane z uruchomionym systemem Windows 10 Pro

 **Połącz użytkowników z usługą Azure AD:**
  
1. Na komputerze PC użytkownika z systemem Windows 10 Pro w wersji 1703 z aktualizacją dla twórców (zobacz [wymagania wstępne](pre-requisites-for-data-protection.md)) kliknij logo systemu Windows i wybierz ikonę Ustawienia.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. W oknie **Ustawienia** wybierz opcję **Konta**.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Na stronie **Twoje informacje** kliknij pozycję **Uzyskaj dostęp do miejsca pracy lub nauki** \> **Połącz**.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. W oknie dialogowym **Konfigurowanie konta służbowego** w sekcji **Alternatywne działania** wybierz pozycję **Dołącz to urządzenie do usługi Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. On the **Let's get you signed in** page, enter your work or school account \> **Next**.
  
   On the **Enter password** page, enter your password \> **Sign in**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Na upewnij się, że **jest to strona organizacji** , sprawdź, czy informacje są poprawne i kliknij przycisk **Dołącz**.
  
   Na stronie **Wszystko gotowe** kliknij przycisk **Gotowe**.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem. Jeśli do migracji profilu i plików użyto narzędzia innej firmy, zsynchronizuj je również z nowym profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD

Aby sprawdzić stan synchronizacji, na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** w sekcji **Ustawienia** kliknij obszar **Połączono z** _ \<organization name\> _ w celu pokazania przycisków **Informacje** i **Rozłącz**. Kliknij przycisk **Informacje**, aby wyświetlić stan synchronizacji. 
  
Na stronie Stan synchronizacji kliknij pozycję Synchronizuj, aby pobrać na komputer PC najnowsze zasady zarządzania urządzeniami przenośnymi.
  
Aby rozpocząć korzystanie z konta Microsoft 365 Business, przejdź do przycisku **Start** systemu Windows, kliknij prawym przyciskiem myszy bieżący obraz konta, a następnie **Przełącz konto**. Zaloguj się przy użyciu adresu e-mail i hasła organizacji.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Sprawdzanie, czy urządzenie zostało uaktualnione do systemu Windows 10 Business

Sprawdź, czy urządzenia z systemem Windows 10 dołączone do usługi Azure AD zostały uaktualnione do systemu Windows 10 Business w ramach subskrypcji usługi Microsoft 365 Business.
  
1. Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.
    
2. Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Następne czynności

Aby skonfigurować urządzenia przenośne, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business](set-up-mobile-devices.md). Aby ustawić zasady ochrony aplikacji lub ochrony urządzeń, zobacz [Zarządzanie usługą Microsoft 365 Business](manage.md).
  
