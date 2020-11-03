---
title: Konfigurowanie urządzeń z systemem Windows dla użytkowników programu Microsoft 365 Business Premium
f1.keywords:
- CSH
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Dowiedz się, jak skonfigurować urządzenia z systemem Windows 10 Pro dla Microsoft 365 Business Premium, włączając scentralizowane mechanizmy zarządzania i zabezpieczeń.
ms.openlocfilehash: c95b9e51c7ec3c440509fe34084d2a030c7f2eec
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841264"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Konfigurowanie urządzeń z systemem Windows dla użytkowników programu Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Wymagania wstępne dotyczące konfigurowania urządzeń z systemem Windows dla programu Microsoft 365 Business Premium

Przed skonfigurowaniem urządzeń z systemem Windows dla programu Microsoft 365 Business Premium upewnij się, że na wszystkich urządzeniach z systemem Windows jest zainstalowany system Windows 10 Pro, wersja 1703 (aktualizacja twórców). System Windows 10 Pro jest warunkiem wstępnym wdrożenia systemu Windows 10 Business, który jest zestawem usług w chmurze i funkcjami zarządzania urządzeniami, które uzupełniają system Windows 10 Pro i umożliwiają scentralizowane mechanizmy kontroli nad zarządzaniem i zabezpieczeniami w witrynie Microsoft 365 Business Premium.
  
Jeśli masz urządzenia z systemem Windows z systemem Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, Twoja subskrypcja usługi Microsoft 365 Business Premium uprawnia do uaktualnienia systemu Windows 10.
  
Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).
  
Zobacz [Weryfikowanie, czy urządzenie jest połączone z usługą Azure AD](#verify-the-device-is-connected-to-azure-ad) , aby sprawdzić, czy masz uaktualnienie, lub aby upewnić się, że uaktualnienie działało.

Obejrzyj krótki klip wideo o łączeniu systemu Windows z systemem Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji

Jeśli wszystkie urządzenia z systemem Windows w organizacji zostały uaktualnione do aktualizacji dla twórców systemu Windows 10 Pro lub są już uruchomione aktualizacje dla twórców systemu Windows 10 Pro, możesz przyłączyć te urządzenia do usługi Azure Active Directory organizacji. Po dołączeniu urządzeń zostaną one automatycznie uaktualnione do systemu Windows 10 Business, który jest częścią abonamentu Microsoft 365 Business Premium.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro

W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.
  
1. Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. W tym miejscu wybierz pozycję **Konfiguracja dla organizacji** , a następnie wprowadź nazwę użytkownika i hasło do usługi Microsoft 365 Business Premium. 
    
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
  
6. Na stronie upewnij się, że to **jest Twoja strona organizacji** , sprawdź, czy informacje są właściwe, a następnie wybierz pozycję **Dołącz**.
  
   **Wszystko gotowe!** Strona **chosse.**
  
   ![Na ekranie upewnij się, że jest to Twoja organizacja, wybierz pozycję Dołącz](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem. Jeśli do migrowania profilu i plików użyto narzędzia innej firmy, zsynchronizuj je również z nowym profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD

Aby zweryfikować stan synchronizacji, na stronie **służbowe lub szkolne** w obszarze **Ustawienia** wybierz pozycję **połączony z** \<organization name\> obszarem _, aby uwidocznić przycisk **informacje** i **Rozłącz**. Wybierz pozycję **informacje** , aby uzyskać stan synchronizacji. 
  
Na stronie **stan synchronizacji** wybierz pozycję **Synchronizuj** , aby uzyskać najnowsze zasady zarządzania urządzeniami przenośnymi na komputerze.
  
Aby rozpocząć korzystanie z konta Microsoft 365 Business Premium, przejdź do przycisku **Start** systemu Windows, kliknij prawym przyciskiem myszy bieżący obraz konta, a następnie **Przełącz konto**. Zaloguj się przy użyciu adresu e-mail i hasła organizacji.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Sprawdzanie, czy komputer jest uaktualniony do wersji Windows 10 Business

Upewnij się, że Twoje urządzenia z systemem Windows 10 dołączone do usługi Azure AD są uaktualnione do systemu Windows 10 Business w ramach abonamentu Microsoft 365 Business Premium.
  
1. Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.
    
2. Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Następne czynności

Aby skonfigurować urządzenia przenośne, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników programu Microsoft 365 Business Premium](set-up-mobile-devices.md), aby ustawić ochronę urządzeń lub zasady ochrony aplikacji, zobacz [zarządzanie systemem Microsoft 365 dla firm](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Aby uzyskać więcej informacji na temat konfigurowania i korzystania z aplikacji Microsoft 365 Business Premium

[Szkolenia wideo dotyczące programu Microsoft 365 dla firm](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
