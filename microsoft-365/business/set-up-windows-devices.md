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
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="2623b-103">Konfigurowanie urządzeń z systemem Windows dla użytkowników programu Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="2623b-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="2623b-104">Wymagania wstępne dotyczące konfigurowania urządzeń z systemem Windows dla programu Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="2623b-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="2623b-105">Przed skonfigurowaniem urządzeń z systemem Windows dla programu Microsoft 365 Business Premium upewnij się, że na wszystkich urządzeniach z systemem Windows jest zainstalowany system Windows 10 Pro, wersja 1703 (aktualizacja twórców).</span><span class="sxs-lookup"><span data-stu-id="2623b-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="2623b-106">System Windows 10 Pro jest warunkiem wstępnym wdrożenia systemu Windows 10 Business, który jest zestawem usług w chmurze i funkcjami zarządzania urządzeniami, które uzupełniają system Windows 10 Pro i umożliwiają scentralizowane mechanizmy kontroli nad zarządzaniem i zabezpieczeniami w witrynie Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2623b-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="2623b-107">Jeśli masz urządzenia z systemem Windows z systemem Windows 7 Pro, Windows 8 Pro lub Windows 8,1 Pro, Twoja subskrypcja usługi Microsoft 365 Business Premium uprawnia do uaktualnienia systemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2623b-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="2623b-108">Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="2623b-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="2623b-109">Zobacz [Weryfikowanie, czy urządzenie jest połączone z usługą Azure AD](#verify-the-device-is-connected-to-azure-ad) , aby sprawdzić, czy masz uaktualnienie, lub aby upewnić się, że uaktualnienie działało.</span><span class="sxs-lookup"><span data-stu-id="2623b-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="2623b-110">Obejrzyj krótki klip wideo o łączeniu systemu Windows z systemem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2623b-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="2623b-111">Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="2623b-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="2623b-112">Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji</span><span class="sxs-lookup"><span data-stu-id="2623b-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="2623b-113">Jeśli wszystkie urządzenia z systemem Windows w organizacji zostały uaktualnione do aktualizacji dla twórców systemu Windows 10 Pro lub są już uruchomione aktualizacje dla twórców systemu Windows 10 Pro, możesz przyłączyć te urządzenia do usługi Azure Active Directory organizacji.</span><span class="sxs-lookup"><span data-stu-id="2623b-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="2623b-114">Po dołączeniu urządzeń zostaną one automatycznie uaktualnione do systemu Windows 10 Business, który jest częścią abonamentu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2623b-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="2623b-115">Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="2623b-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="2623b-116">W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="2623b-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="2623b-117">Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**.</span><span class="sxs-lookup"><span data-stu-id="2623b-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="2623b-119">W tym miejscu wybierz pozycję **Konfiguracja dla organizacji** , a następnie wprowadź nazwę użytkownika i hasło do usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2623b-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="2623b-120">Dokończ konfigurację urządzenia z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2623b-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="2623b-p103">Gdy to zrobisz, użytkownik będzie połączony z usługą Azure AD organizacji. Zobacz [Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD](#verify-the-device-is-connected-to-azure-ad), aby się upewnić.</span><span class="sxs-lookup"><span data-stu-id="2623b-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="2623b-123">Urządzenie już skonfigurowane z uruchomionym systemem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="2623b-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="2623b-124">**Połącz użytkowników z usługą Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="2623b-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="2623b-125">Na komputerze PC użytkownika z systemem Windows 10 Pro w wersji 1703 z aktualizacją dla twórców (zobacz [wymagania wstępne](pre-requisites-for-data-protection.md)) kliknij logo systemu Windows i wybierz ikonę Ustawienia.</span><span class="sxs-lookup"><span data-stu-id="2623b-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="2623b-127">W oknie **Ustawienia** wybierz opcję **Konta**.</span><span class="sxs-lookup"><span data-stu-id="2623b-127">In **Settings** , go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="2623b-129">Na stronie **Twoje informacje** kliknij pozycję **Uzyskaj dostęp do miejsca pracy lub nauki** \> **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="2623b-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="2623b-131">W oknie dialogowym **Konfigurowanie konta służbowego** w sekcji **Alternatywne działania** wybierz pozycję **Dołącz to urządzenie do usługi Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="2623b-131">On the **Set up a work or school account** dialog, under **Alternate actions** , choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="2623b-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="2623b-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="2623b-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="2623b-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="2623b-136">Na stronie upewnij się, że to **jest Twoja strona organizacji** , sprawdź, czy informacje są właściwe, a następnie wybierz pozycję **Dołącz**.</span><span class="sxs-lookup"><span data-stu-id="2623b-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="2623b-137">**Wszystko gotowe!**</span><span class="sxs-lookup"><span data-stu-id="2623b-137">On the **You're all set!**</span></span> <span data-ttu-id="2623b-138">Strona **chosse.**</span><span class="sxs-lookup"><span data-stu-id="2623b-138">page, chosse **Done**.</span></span>
  
   ![Na ekranie upewnij się, że jest to Twoja organizacja, wybierz pozycję Dołącz](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="2623b-140">Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem.</span><span class="sxs-lookup"><span data-stu-id="2623b-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="2623b-141">Jeśli do migrowania profilu i plików użyto narzędzia innej firmy, zsynchronizuj je również z nowym profilem.</span><span class="sxs-lookup"><span data-stu-id="2623b-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="2623b-142">Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD</span><span class="sxs-lookup"><span data-stu-id="2623b-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="2623b-143">Aby zweryfikować stan synchronizacji, na stronie **służbowe lub szkolne** w obszarze **Ustawienia** wybierz pozycję **połączony z** \<organization name\> obszarem _, aby uwidocznić przycisk **informacje** i **Rozłącz**.</span><span class="sxs-lookup"><span data-stu-id="2623b-143">To verify your sync status, on the **Access work or school** page in **Settings** , select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="2623b-144">Wybierz pozycję **informacje** , aby uzyskać stan synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="2623b-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="2623b-145">Na stronie **stan synchronizacji** wybierz pozycję **Synchronizuj** , aby uzyskać najnowsze zasady zarządzania urządzeniami przenośnymi na komputerze.</span><span class="sxs-lookup"><span data-stu-id="2623b-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="2623b-146">Aby rozpocząć korzystanie z konta Microsoft 365 Business Premium, przejdź do przycisku **Start** systemu Windows, kliknij prawym przyciskiem myszy bieżący obraz konta, a następnie **Przełącz konto**.</span><span class="sxs-lookup"><span data-stu-id="2623b-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="2623b-147">Zaloguj się przy użyciu adresu e-mail i hasła organizacji.</span><span class="sxs-lookup"><span data-stu-id="2623b-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="2623b-149">Sprawdzanie, czy komputer jest uaktualniony do wersji Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="2623b-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="2623b-150">Upewnij się, że Twoje urządzenia z systemem Windows 10 dołączone do usługi Azure AD są uaktualnione do systemu Windows 10 Business w ramach abonamentu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2623b-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="2623b-151">Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="2623b-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="2623b-152">Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="2623b-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="2623b-154">Następne czynności</span><span class="sxs-lookup"><span data-stu-id="2623b-154">Next steps</span></span>

<span data-ttu-id="2623b-155">Aby skonfigurować urządzenia przenośne, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników programu Microsoft 365 Business Premium](set-up-mobile-devices.md), aby ustawić ochronę urządzeń lub zasady ochrony aplikacji, zobacz [zarządzanie systemem Microsoft 365 dla firm](manage.md).</span><span class="sxs-lookup"><span data-stu-id="2623b-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="2623b-156">Aby uzyskać więcej informacji na temat konfigurowania i korzystania z aplikacji Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="2623b-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="2623b-157">Szkolenia wideo dotyczące programu Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="2623b-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
