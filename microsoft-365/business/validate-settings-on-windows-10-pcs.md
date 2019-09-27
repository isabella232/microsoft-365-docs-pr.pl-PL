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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak zweryfikować ustawienia ochrony aplikacji biznesowych firmy Microsoft 365 w urządzeniach z systemem Windows 10.
ms.openlocfilehash: 66e83df19e44419b37bcc1c5678ab13317162dbc
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288600"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="fe9f0-103">Sprawdzanie poprawności ustawień ochrony urządzenia na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="fe9f0-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="fe9f0-104">Sprawdź, czy zasady urządzenia systemu Windows 10 są ustawione</span><span class="sxs-lookup"><span data-stu-id="fe9f0-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="fe9f0-105">Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może potrwać do kilku godzin, aby zasady zostały uwzględnione na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="fe9f0-106">Możesz potwierdzić, że zasady zostały uwzględnione, patrząc na różne ekrany ustawień systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="fe9f0-107">Ponieważ użytkownicy nie będą mogli modyfikować ustawień programu Windows Update i Windows Defender Antivirus na swoich urządzeniach z systemem Windows 10, wiele z tych opcji będzie wyszarzony.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="fe9f0-108">Przejdź do **opcji Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Uruchom ponownie** i Potwierdź, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Wszystkie opcje ponownego uruchomienia są wyszarzone.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="fe9f0-110">Przejdź do **Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Zaawansowane opcje** i potwierdzić, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Opcje aktualizacji zaawansowanych systemu Windows są wszystkie wyszarzone.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="fe9f0-112">Przejdź do **Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Update** \> **Zaawansowane opcje** \> **Wybierz sposób dostarczania aktualizacji**.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="fe9f0-113">Potwierdź, że możesz zobaczyć wiadomość (na czerwono), że niektóre ustawienia są ukryte lub zarządzane przez organizację, a wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Wybierz sposób dostarczania aktualizacji strony wskazuje, że ustawienia są ukryte lub zarządzane przez organizację.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="fe9f0-115">Aby otworzyć Centrum zabezpieczeń systemu Windows Defender, przejdź do **ustawień** \> **aktualizacji &amp; zabezpieczeń** \> **Windows Defender** \> kliknij **Otwórz Windows Defender Security Center** \> **wątku &amp; wirusa Ustawienia ochrony przed** **zagrożeniami wirusami &amp; .** \></span><span class="sxs-lookup"><span data-stu-id="fe9f0-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="fe9f0-116">Sprawdź, czy wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-116">Verify that all options are greyed out.</span></span> 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarzone.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="fe9f0-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="fe9f0-118">Related Topics</span></span>

[<span data-ttu-id="fe9f0-119">Dokumentacja i zasoby dotyczące usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fe9f0-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="fe9f0-120">Rozpoczynanie pracy z usługą Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fe9f0-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="fe9f0-121">Zarządzanie usługą Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fe9f0-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="fe9f0-122">Konfigurowanie komputerów PC z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="fe9f0-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

