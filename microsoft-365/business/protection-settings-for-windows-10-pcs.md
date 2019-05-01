---
title: Konfigurowanie ustawień ochrony urządzeń dla komputerów z systemem Windows 10
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
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Dowiedz się więcej o domyślnych i innych ustawień, które są dostępne w Microsoft Business 365 do zabezpieczenia urządzeń Windows 10.
ms.openlocfilehash: f9e890cde7a8290a9a8e81720d32a6a2889c312f
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32285930"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="ee71e-103">Konfigurowanie ustawień ochrony urządzeń dla komputerów z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="ee71e-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="ee71e-104">Zabezpieczanie urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="ee71e-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="ee71e-105">Obejrzyj klip wideo na temat zabezpieczania urządzeń z systemem Windows 10 za pomocą usługi Microsoft 365 Business:</span><span class="sxs-lookup"><span data-stu-id="ee71e-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="ee71e-106">Zaloguj się do [Centrum administracyjnego](https://go.microsoft.com/fwlink/p/?linkid=837890) z poświadczeniami administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="ee71e-106">Sign in to [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="ee71e-107">Na nawigacji z lewej strony wybierz **urządzenia** \> **zasady** \> **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="ee71e-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="ee71e-108">W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad.</span><span class="sxs-lookup"><span data-stu-id="ee71e-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="ee71e-109">W sekcji **Typ zasad** wybierz opcję **Konfiguracja urządzeń z systemem Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="ee71e-109">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="ee71e-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span><span class="sxs-lookup"><span data-stu-id="ee71e-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span></span> 
    
    <span data-ttu-id="ee71e-112">Aby zresetować ustawienia do wartości domyślnych, w dowolnej chwili możesz użyć linku **Resetuj ustawienia domyślne**.</span><span class="sxs-lookup"><span data-stu-id="ee71e-112">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="ee71e-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="ee71e-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="ee71e-116">Na koniec wybierz przycisk **Gotowe**, aby zapisać zasady i zastosować je na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="ee71e-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="ee71e-117">Dostępne ustawienia</span><span class="sxs-lookup"><span data-stu-id="ee71e-117">Available settings</span></span>

<span data-ttu-id="ee71e-p103">Domyślnie wszystkie ustawienia są **Włączone**. Dostępne są następujące ustawienia.</span><span class="sxs-lookup"><span data-stu-id="ee71e-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="ee71e-120">Aby uzyskać więcej informacji, zobacz [Jaka jest zależność między funkcjami ochrony w usłudze Microsoft 365 Business i ustawieniami usługi Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="ee71e-120">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="ee71e-121">Ustawienie</span><span class="sxs-lookup"><span data-stu-id="ee71e-121">Setting</span></span>  <br/> |<span data-ttu-id="ee71e-122">Opis</span><span class="sxs-lookup"><span data-stu-id="ee71e-122">Description</span></span>  <br/> |
|<span data-ttu-id="ee71e-123">Chroń komputery przed wirusami i innymi zagrożeniami za pomocą ochrony antywirusowej programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="ee71e-123">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="ee71e-124">Wymaga włączenia programu antywirusowego Windows Defender w celu ochrony komputerów przed zagrożeniami związanymi z połączeniem z Internetem.</span><span class="sxs-lookup"><span data-stu-id="ee71e-124">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="ee71e-125">Chroń komputery przed zagrożeniami internetowymi w programie Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ee71e-125">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="ee71e-126">Włącza w programie Microsoft Edge ustawienia ułatwiające ochronę użytkowników przed złośliwymi witrynami i złośliwą zawartością do pobrania.</span><span class="sxs-lookup"><span data-stu-id="ee71e-126">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="ee71e-127">Użyj reguł, które zmniejszają obszar ataków na urządzenia</span><span class="sxs-lookup"><span data-stu-id="ee71e-127">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="ee71e-p104">Gdy zmniejszanie obszaru ataków jest włączone, pomaga blokować akcje i aplikacje zwykle używane przez złośliwe oprogramowanie do infekowania urządzeń. To ustawienie jest dostępne tylko wtedy, gdy jest włączona ochrona antywirusowa programu Windows Defender. Zobacz [Zmniejszanie obszarów ataków](https://go.microsoft.com/fwlink/?linkid=870417), aby dowiedzieć się więcej.  </span><span class="sxs-lookup"><span data-stu-id="ee71e-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="ee71e-131">Chroń foldery przed zagrożeniami, takimi jak oprogramowanie wymuszające okup</span><span class="sxs-lookup"><span data-stu-id="ee71e-131">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="ee71e-p105">To ustawienie używa kontrolowanego dostępu do folderów w celu ochrony danych firmy przed modyfikacją przez podejrzane lub złośliwe aplikacje, takie jak oprogramowanie wymuszające okup. Tego typu aplikacje mają zablokowaną możliwość wprowadzania zmian w chronionych folderach. To ustawienie jest dostępne tylko wtedy, gdy jest włączona ochrona antywirusowa programu Windows Defender. Zobacz [Chronienie folderów za pomocą kontrolowanego dostępu do folderów](https://go.microsoft.com/fwlink/?linkid=870418), aby dowiedzieć się więcej.  </span><span class="sxs-lookup"><span data-stu-id="ee71e-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="ee71e-136">Blokuj dostęp sieciowy do potencjalnie złośliwej zawartości w Internecie</span><span class="sxs-lookup"><span data-stu-id="ee71e-136">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="ee71e-p106">To ustawienie umożliwia blokowanie połączeń wychodzących użytkownika do lokalizacji internetowych o niskiej reputacji, które mogą wiązać się z wyłudzaniem informacji, oszustwami i złośliwą zawartością. To ustawienie jest dostępne tylko wtedy, gdy jest włączona ochrona antywirusowa programu Windows Defender. Zobacz [Chronienie sieci](https://go.microsoft.com/fwlink/?linkid=870419), aby uzyskać więcej informacji.  </span><span class="sxs-lookup"><span data-stu-id="ee71e-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="ee71e-140">Pomóż chronić pliki i foldery na komputerach przed nieautoryzowanym dostępem za pomocą funkcji BitLocker</span><span class="sxs-lookup"><span data-stu-id="ee71e-140">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="ee71e-p107">Funkcja BitLocker chroni dane przez zaszyfrowanie dysków twardych komputera i zapewnianie ochrony przed ujawnieniem danych w razie zagubienia lub kradzieży komputera. Zobacz [Często zadawane pytania dotyczące funkcji BitLocker](https://go.microsoft.com/fwlink/?linkid=871000), aby uzyskać więcej informacji.  </span><span class="sxs-lookup"><span data-stu-id="ee71e-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="ee71e-143">Zezwalaj użytkownikom na pobieranie aplikacji z witryny Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="ee71e-143">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="ee71e-p108">Pozwala użytkownikom pobierać i instalować aplikacje z witryny Microsoft Store. Do aplikacji tych należą zarówno gry, jak i narzędzia biurowe, więc zostawiamy to ustawienie **włączone**, ale możesz je wyłączyć w celu dodatkowego zwiększenia bezpieczeństwa.  </span><span class="sxs-lookup"><span data-stu-id="ee71e-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="ee71e-146">Zezwalaj użytkownikom na korzystanie z Cortany</span><span class="sxs-lookup"><span data-stu-id="ee71e-146">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="ee71e-p109">Cortana może być bardzo pomocna. Może włączać lub wyłączać ustawienia, udzielać wskazówek i przypominać o spotkaniach, więc to ustawienie domyślnie jest **włączone**.  </span><span class="sxs-lookup"><span data-stu-id="ee71e-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="ee71e-149">Zezwalaj użytkownikom na otrzymywanie porad i reklam dotyczących systemu Windows od firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="ee71e-149">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="ee71e-150">Porady dotyczące systemu Windows mogą być przydatne i ułatwiać użytkownikom zapoznawanie się nowymi funkcjami.</span><span class="sxs-lookup"><span data-stu-id="ee71e-150">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="ee71e-151">Automatycznie aktualizuj urządzenia z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="ee71e-151">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="ee71e-152">Zapewnia, że urządzenia z systemem Windows 10 automatycznie otrzymują najnowsze aktualizacje.</span><span class="sxs-lookup"><span data-stu-id="ee71e-152">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="ee71e-153">Wyłącz ekran urządzenia po takim czasie bezczynności</span><span class="sxs-lookup"><span data-stu-id="ee71e-153">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="ee71e-p110">Zapewnia bezpieczeństwo danych firmowych podczas bezczynności użytkownika. Jeśli użytkownik pracuje w miejscu publicznym, na przykład kawiarni, i odejdzie na chwilę od urządzenia lub skupi uwagę na czymś innym, przypadkowe osoby mogą obejrzeć zawartość ekranu. To ustawienie pozwala kontrolować czas bezczynności użytkownika, po którym ekran zostanie wyłączony.</span><span class="sxs-lookup"><span data-stu-id="ee71e-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  
