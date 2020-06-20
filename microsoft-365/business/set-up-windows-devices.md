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
ms.openlocfilehash: 85ac3c964792a132d5699703e543289020e38f57
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785857"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="58908-103">Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="58908-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="58908-104">Wymagania wstępne dotyczące konfigurowania urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="58908-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="58908-105">Zanim będzie można skonfigurować urządzenia z systemem Windows dla użytkowników usługi Microsoft 365 Business Premium, upewnij się, że na wszystkich urządzeniach z systemem Windows są uruchomione systemy Windows 10 Pro w wersji 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="58908-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="58908-106">Windows 10 Pro jest warunkiem wstępnym wdrożenia systemu Windows 10 Business, który jest zestawem usług w chmurze i funkcji zarządzania urządzeniami, które uzupełniają system Windows 10 Pro i umożliwiają scentralizowane zarządzanie i kontrolę bezpieczeństwa usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="58908-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="58908-107">Jeśli masz urządzenia z systemem Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, subskrypcja usługi Microsoft 365 Business Premium uprawnia do uaktualnienia systemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="58908-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="58908-108">Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="58908-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="58908-109">Zobacz [Sprawdź, czy urządzenie jest połączone z usługą Azure AD,](#verify-the-device-is-connected-to-azure-ad) aby sprawdzić, czy masz uaktualnienie lub upewnić się, że uaktualnienie zostało zadziałało.</span><span class="sxs-lookup"><span data-stu-id="58908-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="58908-110">Obejrzyj krótki film o łączeniu systemu Windows z programem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="58908-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="58908-111">Jeśli ten klip wideo okazał się przydatny, poznaj [kompletną serię szkoleń dla małych firm i nowych użytkowników usługi Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="58908-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="58908-112">Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji</span><span class="sxs-lookup"><span data-stu-id="58908-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="58908-113">Gdy wszystkie urządzenia z systemem Windows w organizacji zostały uaktualnione do aktualizacji Windows 10 Pro Creators Update lub są już uruchomione w usłudze Windows 10 Pro Creators Update, można dołączyć do tych urządzeń w usłudze Azure Active Directory twojej organizacji.</span><span class="sxs-lookup"><span data-stu-id="58908-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="58908-114">Po dołączeniu urządzeń zostaną one automatycznie uaktualnione do systemu Windows 10 Business, który jest częścią subskrypcji usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="58908-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="58908-115">Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="58908-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="58908-116">W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="58908-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="58908-117">Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**.</span><span class="sxs-lookup"><span data-stu-id="58908-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="58908-119">W tym miejscu wybierz pozycję **Konfigurowanie dla organizacji,** a następnie wprowadź nazwę użytkownika i hasło dla usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="58908-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="58908-120">Dokończ konfigurację urządzenia z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="58908-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="58908-121">Once you're done, the user will be connected to your organization's Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58908-121">Once you're done, the user will be connected to your organization's Azure AD.</span></span> <span data-ttu-id="58908-122">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span><span class="sxs-lookup"><span data-stu-id="58908-122">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="58908-123">Urządzenie już skonfigurowane z uruchomionym systemem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="58908-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="58908-124">**Połącz użytkowników z usługą Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="58908-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="58908-125">Na komputerze PC użytkownika z systemem Windows 10 Pro w wersji 1703 z aktualizacją dla twórców (zobacz [wymagania wstępne](pre-requisites-for-data-protection.md)) kliknij logo systemu Windows i wybierz ikonę Ustawienia.</span><span class="sxs-lookup"><span data-stu-id="58908-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="58908-127">W oknie **Ustawienia** wybierz opcję **Konta**.</span><span class="sxs-lookup"><span data-stu-id="58908-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="58908-129">Na stronie **Twoje informacje** kliknij pozycję **Uzyskaj dostęp do miejsca pracy lub nauki** \> **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="58908-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="58908-131">W oknie dialogowym **Konfigurowanie konta służbowego** w sekcji **Alternatywne działania** wybierz pozycję **Dołącz to urządzenie do usługi Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="58908-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="58908-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="58908-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="58908-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="58908-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="58908-136">Na stronie **Upewnij się, że jest to twoja organizacja,** sprawdź, czy informacje są poprawne, a następnie kliknij przycisk **Dołącz**.</span><span class="sxs-lookup"><span data-stu-id="58908-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="58908-137">On the **You're all set!**</span><span class="sxs-lookup"><span data-stu-id="58908-137">On the **You're all set!**</span></span> <span data-ttu-id="58908-138">page, click **Done**.</span><span class="sxs-lookup"><span data-stu-id="58908-138">page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="58908-140">Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem.</span><span class="sxs-lookup"><span data-stu-id="58908-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="58908-141">Jeśli do migracji profilu i plików użyto narzędzia innej firmy, należy je również zsynchronizować z nowym profilem.</span><span class="sxs-lookup"><span data-stu-id="58908-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="58908-142">Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD</span><span class="sxs-lookup"><span data-stu-id="58908-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="58908-143">Aby zweryfikować stan synchronizacji, na stronie **Praca lub szkoła programu Access** w obszarze **Ustawienia**kliknij obszar **Podłącz do** _ \<organization name\> _, aby udostępnić przyciski **Informacje** i **Rozłącz**.</span><span class="sxs-lookup"><span data-stu-id="58908-143">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="58908-144">Kliknij przycisk **Informacje**, aby wyświetlić stan synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="58908-144">Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="58908-145">Na stronie Stan synchronizacji kliknij pozycję Synchronizuj, aby pobrać na komputer PC najnowsze zasady zarządzania urządzeniami przenośnymi.</span><span class="sxs-lookup"><span data-stu-id="58908-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="58908-146">Aby rozpocząć korzystanie z konta Microsoft 365 Business Premium, przejdź do przycisku **Start** systemu Windows, kliknij prawym przyciskiem myszy bieżący obraz konta, a następnie **przełącz konto**.</span><span class="sxs-lookup"><span data-stu-id="58908-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="58908-147">Zaloguj się przy użyciu adresu e-mail i hasła organizacji.</span><span class="sxs-lookup"><span data-stu-id="58908-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="58908-149">Sprawdzanie, czy urządzenie zostało uaktualnione do systemu Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="58908-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="58908-150">Sprawdź, czy urządzenia z systemem Windows 10 przyłączone do usługi Azure AD zostały uaktualnione do systemu Windows 10 Business w ramach subskrypcji usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="58908-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="58908-151">Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="58908-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="58908-152">Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="58908-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="58908-154">Następne czynności</span><span class="sxs-lookup"><span data-stu-id="58908-154">Next steps</span></span>

<span data-ttu-id="58908-155">Aby skonfigurować urządzenia przenośne, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business Premium](set-up-mobile-devices.md), Aby ustawić zasady ochrony urządzeń lub ochrony aplikacji, zobacz [Zarządzanie microsoftem 365 dla firm](manage.md).</span><span class="sxs-lookup"><span data-stu-id="58908-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="58908-156">Więcej informacji na temat konfigurowania i korzystania z usługi Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="58908-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="58908-157">Wideo dotyczące szkoleń dotyczących usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="58908-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
