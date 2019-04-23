---
title: Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Dowiedz się, jak skonfigurować urządzeniach z systemem Windows 10 Pro dla użytkowników biznesowych 365 firmy Microsoft. '
ms.openlocfilehash: f93257bd9a68385fca4f178a2e09c5c11506ee2c
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32284401"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="1f9b4-103">Konfigurowanie urządzeń z systemem Windows dla użytkowników usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="1f9b4-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f9b4-104">Wymagania wstępne</span><span class="sxs-lookup"><span data-stu-id="1f9b4-104">Prerequisites</span></span>

<span data-ttu-id="1f9b4-p101">Zanim będzie można skonfigurować urządzenia z systemem Windows dla użytkowników usługi Microsoft 365 Business należy się upewnić, że na wszystkich tych urządzeniach jest zainstalowany system Windows 10 Pro w wersji 1703 (aktualizacja dla twórców). System Windows 10 Pro stanowi wymaganie wstępne w przypadku wdrażania systemu Windows 10 Business  zestawu usług w chmurze i funkcji zarządzania urządzeniami  który uzupełnia system Windows 10 Pro i udostępnia mechanizmy scentralizowanego zarządzania i zabezpieczeń usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="1f9b4-107">Jeśli na urządzeniach z systemem Windows działa system Windows 7 Pro, Windows 8 Pro lub Windows 8.1 Pro, to subskrypcja usługi Microsoft 365 Business uprawnia do uaktualnienia do systemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="1f9b4-108">Aby uzyskać więcej informacji na temat uaktualniania urządzeń z systemem Windows do systemu Windows 10 Pro (aktualizacja dla twórców), wykonaj czynności opisane w tym temacie: [Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="1f9b4-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="1f9b4-109">Zobacz, [Sprawdź urządzenie jest podłączone do Azure AD](#verify-the-device-is-connected-to-azure-ad) , sprawdź, czy masz uaktualnienia lub upewnić się, że uaktualnienie pracował.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span> 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="1f9b4-110">Dołączanie urządzeń z systemem Windows 10 do usługi Azure AD organizacji</span><span class="sxs-lookup"><span data-stu-id="1f9b4-110">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="1f9b4-p102">Kiedy wszystkie urządzenia z systemem Windows w organizacji zostaną uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców) lub jeśli mają już zainstalowany system Windows 10 Pro (aktualizacja dla twórców), możesz dołączyć te urządzenia do usługi Azure Active Directory Twojej organizacji. Gdy urządzenia zostaną dołączone, zostaną automatycznie uaktualnione do systemu Windows 10 Business  jest to część subskrypcji usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p102">Once all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory. Once the devices are joined, they will automatically be upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="1f9b4-113">Całkowicie nowe lub nowo uaktualnione urządzenie z systemem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="1f9b4-113">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="1f9b4-114">W przypadku całkowicie nowego urządzenia z systemem Windows 10 Pro (aktualizacja dla twórców) lub w przypadku urządzenia, które zostało uaktualnione do systemu Windows 10 Pro (aktualizacja dla twórców), ale nie przeszło konfiguracji urządzenia z systemem Windows 10, wykonaj poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-114">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="1f9b4-115">Postępuj zgodnie z instrukcjami konfiguracji urządzenia z systemem Windows 10 do momentu przejścia do strony **Jak chcesz skonfigurować?**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-115">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="1f9b4-117">Na tej stronie wybierz opcję **Konfiguruj dla organizacji**, a następnie wprowadź nazwę użytkownika i hasło dla usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-117">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="1f9b4-118">Dokończ konfigurację urządzenia z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-118">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="1f9b4-p103">Gdy to zrobisz, użytkownik będzie połączony z usługą Azure AD organizacji. Zobacz [Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD](#verify-the-device-is-connected-to-azure-ad), aby się upewnić.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="1f9b4-121">Urządzenie już skonfigurowane z uruchomionym systemem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="1f9b4-121">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="1f9b4-122">**Połącz użytkowników z usługą Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="1f9b4-122">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="1f9b4-123">Na komputerze PC użytkownika z systemem Windows 10 Pro w wersji 1703 z aktualizacją dla twórców (zobacz [wymagania wstępne](pre-requisites-for-data-protection.md)) kliknij logo systemu Windows i wybierz ikonę Ustawienia.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-123">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="1f9b4-125">W oknie **Ustawienia** wybierz opcję **Konta**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-125">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="1f9b4-127">Na stronie **Twoje informacje** kliknij pozycję **Uzyskaj dostęp do miejsca pracy lub nauki** \> **Połącz**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-127">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="1f9b4-129">W oknie dialogowym **Konfigurowanie konta służbowego** w sekcji **Alternatywne działania** wybierz pozycję **Dołącz to urządzenie do usługi Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-129">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="1f9b4-131">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-131">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="1f9b4-132">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-132">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="1f9b4-134">Na stronie **Sprawdź, czy jest to organizacja** Sprawdź, czy informacje są poprawne i kliknij przycisk **Dołącz**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-134">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="1f9b4-p104">Na stronie **Wszystko gotowe** kliknij przycisk **Gotowe**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="1f9b4-p105">Jeśli masz pliki przesłane do usługi OneDrive dla Firm, zsynchronizuj je z powrotem. Jeśli profil i pliki zostały przeniesione przy użyciu narzędzi innej firmy, zsynchronizuj też te dane z nowym profilem.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p105">If you uploaded files to OneDrive for Business, sync them back down. If you used a third party tool to migrate profile and files, sync those also to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="1f9b4-140">Sprawdzanie, czy urządzenie zostało połączone z usługą Azure AD</span><span class="sxs-lookup"><span data-stu-id="1f9b4-140">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="1f9b4-p106">Aby sprawdzić stan synchronizacji, na stronie **Uzyskaj dostęp do miejsca pracy lub nauki** w sekcji **Ustawienia** kliknij obszar **Połączono z** _ \<organization name\> _ w celu pokazania przycisków **Informacje** i **Rozłącz**. Kliknij przycisk **Informacje**, aby wyświetlić stan synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="1f9b4-143">Na stronie Stan synchronizacji kliknij pozycję Synchronizuj, aby pobrać na komputer PC najnowsze zasady zarządzania urządzeniami przenośnymi.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-143">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="1f9b4-p107">Aby rozpocząć korzystanie z konta usługi Microsoft 365 Business, otwórz menu **Start** systemu Windows, kliknij bieżący obraz profilu prawym przyciskiem myszy i wybierz polecenie **Przełącz konto**. Zaloguj się przy użyciu adresu e-mail i hasła organizacji.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-p107">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture and then **Switch account**. Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="1f9b4-147">Sprawdzanie, czy urządzenie zostało uaktualnione do systemu Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="1f9b4-147">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="1f9b4-148">Sprawdź, czy urządzenia z systemem Windows 10 dołączone do usługi Azure AD zostały uaktualnione do systemu Windows 10 Business w ramach subskrypcji usługi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-148">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="1f9b4-149">Wybierz pozycję **Ustawienia** \> **System** \> **Informacje**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-149">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="1f9b4-150">Potwierdź, że w polu **Wersja** jest wskazywany system **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="1f9b4-150">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="1f9b4-152">Następne czynności</span><span class="sxs-lookup"><span data-stu-id="1f9b4-152">Next steps</span></span>

<span data-ttu-id="1f9b4-153">Aby skonfigurować urządzenia przenośne, zobacz [Konfigurowanie urządzeń przenośnych dla użytkowników usługi Microsoft 365 Business](set-up-mobile-devices.md). Aby ustawić zasady ochrony aplikacji lub ochrony urządzeń, zobacz [Zarządzanie usługą Microsoft 365 Business](manage.md).</span><span class="sxs-lookup"><span data-stu-id="1f9b4-153">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  
