---
title: Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium
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
description: Dowiedz się, jak skonfigurować urządzenia z systemem Windows 10 Pro dla użytkowników usługi Microsoft 365 Business Premium, umożliwiając scentralizowane zarządzanie i kontrolę zabezpieczeń.
ms.openlocfilehash: ecd9f5aa348d29d34e77061657619c015b09c41a
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402963"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Wymagania wstępne dotyczące konfigurowania urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium

Zanim będzie można skonfigurować urządzenia z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium, upewnij się, że na wszystkich urządzeniach z systemem Windows są uruchomione systemy Windows 10 Pro w wersji 1703 (Creators Update). Windows 10 Pro jest warunkiem wstępnym wdrożenia systemu Windows 10 Business, który jest zestawem usług w chmurze i funkcji zarządzania urządzeniami, które uzupełniają system Windows 10 Pro i umożliwiają scentralizowane zarządzanie i kontrolę bezpieczeństwa usługi Microsoft 365 Business Premium.
  
Jeśli masz urządzenia z systemem Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja usługi Microsoft 365 Business Premium uprawnia do uaktualnienia systemu Windows 10.
  
Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).
  
Zobacz [Sprawdź, czy urządzenie jest połączone z usługą Azure AD,](#verify-the-device-is-connected-to-azure-ad) aby sprawdzić, czy masz uaktualnienie lub upewnić się, że uaktualnienie zostało zadziałało.

Obejrzyj krótki film o łączeniu systemu Windows z programem Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji

Gdy wszystkie urządzenia z systemem Windows w organizacji zostały uaktualnione do aktualizacji Windows 10 Pro Creators Update lub są już uruchomione w usłudze Windows 10 Pro Creators Update, można dołączyć do tych urządzeń w usłudze Azure Active Directory twojej organizacji. Po dołączeniu urządzeń zostaną one automatycznie uaktualnione do systemu Windows 10 Business, który jest częścią subskrypcji usługi Microsoft 365 Business Premium.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro

W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.
  
1. Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. W tym miejscu wybierz pozycję **Konfigurowanie dla organizacji,** a następnie wprowadź nazwę użytkownika i hasło dla usługi Microsoft 365 Business Premium. 
    
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
  
6. Na stronie **Upewnij się, że jest to twoja organizacja,** sprawdź, czy informacje są poprawne, a następnie kliknij przycisk **Dołącz**.
  
   Na stronie **Wszystko gotowe** kliknij przycisk **Gotowe**.
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem. Jeśli do migracji profilu i plików użyto narzędzia innej firmy, należy je również zsynchronizować z nowym profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD

Aby zweryfikować stan synchronizacji, na stronie **Praca lub szkoła programu Access** w obszarze **Ustawienia**kliknij obszar **Podłącz do** _ \<organization name\> _, aby udostępnić przyciski **Informacje** i **Rozłącz**. Kliknij przycisk **Informacje**, aby wyświetlić stan synchronizacji. 
  
Na stronie Stan synchronizacji kliknij pozycję Synchronizuj, aby pobrać na komputer PC najnowsze zasady zarządzania urządzeniami przenośnymi.
  
Aby rozpocząć korzystanie z konta Microsoft 365 Business Premium, przejdź do przycisku **Start** systemu Windows, kliknij prawym przyciskiem myszy bieżący obraz konta, a następnie **przełącz konto**. Zaloguj się przy użyciu adresu e-mail i hasła organizacji.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Sprawdzanie, czy urządzenie zostało uaktualnione do systemu Windows 10 Business

Sprawdź, czy urządzenia z systemem Windows 10 przyłączone do usługi Azure AD zostały uaktualnione do systemu Windows 10 Business w ramach subskrypcji usługi Microsoft 365 Business Premium.
  
1. Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.
    
2. Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Następne czynności

Aby skonfigurować urządzenia przenośne, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business Premium](set-up-mobile-devices.md), Aby ustawić zasady ochrony urządzeń lub ochrony aplikacji, zobacz [Zarządzanie microsoftem 365 dla firm](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Więcej informacji na temat konfigurowania i korzystania z usługi Microsoft 365 Business Premium

[Wideo dotyczące szkoleń dotyczących usługi Microsoft 365 dla firm](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
