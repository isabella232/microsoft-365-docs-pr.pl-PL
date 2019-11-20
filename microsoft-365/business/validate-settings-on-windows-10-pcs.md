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
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak zweryfikować ustawienia ochrony aplikacji biznesowych firmy Microsoft 365 na urządzeniach z systemem Windows 10.
ms.openlocfilehash: b8793ab7f77bbc7f608f237e2455f6fd12c3bb26
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721805"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="fa40c-103">Sprawdzanie poprawności ustawień ochrony urządzenia na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="fa40c-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="fa40c-104">Sprawdź, czy zasady urządzenia systemu Windows 10 są ustawione</span><span class="sxs-lookup"><span data-stu-id="fa40c-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="fa40c-105">Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może potrwać do kilku godzin, aby zasady zostały uwzględnione na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="fa40c-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="fa40c-106">Możesz potwierdzić, że zasady zostały uwzględnione, patrząc na różne ekrany ustawień systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="fa40c-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="fa40c-107">Ponieważ użytkownicy nie będą mogli modyfikować ustawień programu Windows Update i Windows Defender Antivirus na swoich urządzeniach z systemem Windows 10, wiele opcji będzie wyszarzony.</span><span class="sxs-lookup"><span data-stu-id="fa40c-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="fa40c-108">Przejdź do **opcji Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Uruchom ponownie** i Potwierdź, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fa40c-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Wszystkie opcje ponownego uruchomienia są wyszarzone.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="fa40c-110">Przejdź do **Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Zaawansowane opcje** i potwierdzić, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fa40c-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Opcje zaawansowanych aktualizacji systemu Windows są wyszarzone.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="fa40c-112">Przejdź do **Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Zaawansowane opcje** \> **Wybierz sposób dostarczania aktualizacji**.</span><span class="sxs-lookup"><span data-stu-id="fa40c-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="fa40c-113">Potwierdź, że możesz zobaczyć wiadomość (na czerwono), że niektóre ustawienia są ukryte lub zarządzane przez organizację, a wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fa40c-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Wybierz sposób dostarczania aktualizacji strony wskazuje, że ustawienia są ukryte lub zarządzane przez organizację.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="fa40c-115">Aby otworzyć Centrum zabezpieczeń systemu Windows Defender, przejdź do **ustawień** \> **aktualizacji &amp; zabezpieczeń** \> **systemu Windows Defender** \> kliknij przycisk **Otwórz Windows Defender Security Center** \> **Virus &amp; Thread ochrona** \> ochrona **przed wirusami &amp; ochrony przed zagrożeniami**.</span><span class="sxs-lookup"><span data-stu-id="fa40c-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="fa40c-116">Sprawdź, czy wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fa40c-116">Verify that all options are grayed out.</span></span> 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarzone.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="fa40c-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="fa40c-118">Related Topics</span></span>

[<span data-ttu-id="fa40c-119">Dokumentacja i zasoby dotyczące usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fa40c-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="fa40c-120">Rozpoczynanie pracy z usługą Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fa40c-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="fa40c-121">Zarządzanie usługą Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fa40c-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="fa40c-122">Konfigurowanie komputerów PC z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="fa40c-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

