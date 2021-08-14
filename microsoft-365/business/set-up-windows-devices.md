---
title: Konfigurowanie Windows dla Microsoft 365 Business Premium użytkowników
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Skonfiguruj Windows z systemem Windows 10 Pro dla Microsoft 365 Business Premium użytkowników, umożliwiając scentralizowane zarządzanie i mechanizmy kontroli zabezpieczeń.
ms.openlocfilehash: 0a38a244ca997cfadb46c3833c0587e0c4f79fe3d32b90c6d92f08069b352bd3
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837847"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Konfigurowanie Windows dla Microsoft 365 Business Premium użytkowników

## <a name="before-you-begin"></a>Przed rozpoczęciem

Zanim będzie można skonfigurować Windows dla użytkowników Microsoft 365 Business Premium, upewnij się, że na wszystkich Windows działa wersja Windows 10 Pro 1703 (aktualizacja dla twórców). Windows 10 Pro stanowi wymaganie wstępne przy wdrażaniu usługi Windows 10 Business, która jest zestawem usług w chmurze i funkcji zarządzania urządzeniami, który uzupełnia program Windows 10 Pro i włącza mechanizmy scentralizowanego zarządzania i zabezpieczeń Microsoft 365 Business Premium.
  
Jeśli masz Windows z systemem Windows Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja Microsoft 365 Business Premium uprawnia do uaktualnienia Windows 10.
  
Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).
  
Zobacz [Sprawdzanie, czy urządzenie zostało połączone z](#verify-the-device-is-connected-to-azure-ad) usługą Azure AD, aby sprawdzić, czy masz uaktualnienie, lub aby się upewnić, że uaktualnienie się nie posunie.

## <a name="watch-connect-your-pc-to-microsoft-365-business"></a>Obejrzyj: Połączenie komputera do Microsoft 365 Firm

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](../business-video/index.yml).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji

Jeśli wszystkie Windows w organizacji zostały uaktualnione do usługi Windows 10 Pro Creators Update lub są już uruchomione w aktualizacji dla twórców programu Windows 10 Pro, możesz dołączyć te urządzenia do programu Azure Active Directory organizacji. Po dołączeniu urządzeń zostaną one automatycznie uaktualnione do Windows 10 Business, co stanowi część Microsoft 365 Business Premium subskrypcji.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro

W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.
  
1. Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. W tym miejscu **wybierz pozycję Skonfiguruj dla organizacji, a** następnie wprowadź nazwę użytkownika i hasło dla Microsoft 365 Business Premium. 
    
3. Dokończ konfigurację urządzenia z systemem Windows 10.
    
   Gdy to zrobisz, użytkownik będzie połączony z usługą Azure AD organizacji. Zobacz [Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD](#verify-the-device-is-connected-to-azure-ad), aby się upewnić. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Urządzenie już skonfigurowane z uruchomionym systemem Windows 10 Pro

 **Połącz użytkowników z usługą Azure AD:**
  
1. Na komputerze PC użytkownika z systemem Windows 10 Pro w wersji 1703 z aktualizacją dla twórców (zobacz [wymagania wstępne](pre-requisites-for-data-protection.md)) kliknij logo systemu Windows i wybierz ikonę Ustawienia.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. W oknie **Ustawienia** wybierz opcję **Konta**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Na stronie **Twoje informacje** kliknij pozycję **Uzyskaj dostęp do miejsca pracy lub nauki** \> **Połącz**.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. W oknie dialogowym **Konfigurowanie konta służbowego** w sekcji **Alternatywne działania** wybierz pozycję **Dołącz to urządzenie do usługi Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. On the **Let's get you signed in** page, enter your work or school account \> **Next**.
  
   On the **Enter password** page, enter your password \> **Sign in**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Na stronie **Upewnij się, że** to Twoja organizacja sprawdź poprawność informacji i wybierz pozycję **Dołącz**.
  
   Na **ekranie Wszystko jest już ustawione!** strona, chosse **Done .**
  
   ![Na ekranie Upewnij się, że to Twoja organizacja wybierz pozycję Dołącz](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem. Jeśli profil i pliki zostały przeniesione za pomocą narzędzia innej firmy, zsynchronizuj też te dane z nowym profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD

Aby sprawdzić stan synchronizacji,  na stronie Uzyskaj dostęp do pracy  lub nauki w programie **Ustawienia** wybierz obszar Połączono z _ w celu udostępnienia przycisków Informacje i \<organization name\> Rozłącz.   Wybierz **pozycję Informacje,** aby uzyskać stan synchronizacji. 
  
Na stronie **Stan synchronizacji** wybierz pozycję Synchronizuj, aby pobrać na komputer PC najnowsze zasady zarządzania urządzeniami przenośnymi. 
  
Aby rozpocząć korzystanie z konta Microsoft 365 Business Premium, przejdź do przycisku **Start** Windows, kliknij prawym przyciskiem myszy bieżący obraz konta, a następnie wybierz **pozycję Przełącz konto.** Zaloguj się przy użyciu adresu e-mail i hasła organizacji.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Sprawdzanie, czy komputer został uaktualniony do Windows 10 Business

Upewnij się, że urządzenia dołączane do Windows 10 Azure AD są uaktualnione Windows 10 Business w ramach twojej subskrypcji Microsoft 365 Business Premium usługi Azure AD.
  
1. Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.
    
2. Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Następne kroki

Aby skonfigurować urządzenia przenośne, zobacz Konfigurowanie urządzeń przenośnych dla użytkowników usługi [Microsoft 365 Business Premium](set-up-mobile-devices.md). Aby skonfigurować zasady ochrony urządzeń lub ochrony aplikacji, zobacz Zarządzanie usługą [Microsoft 365 dla firm.](manage.md)
  
## <a name="related-content"></a>Zawartość pokrewna

[Microsoft 365 szkoleniowe klipy wideo dla firm](../business-video/index.yml) (strona linku)
