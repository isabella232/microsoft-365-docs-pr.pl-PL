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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić poprawność ustawień ochrony aplikacji Microsoft 365 Business w urządzeniach 10 systemu Windows.
ms.openlocfilehash: 15c2d54c6281369875d15985c9d4ed16f0114176
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072241"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="554f3-103">Sprawdź poprawność ustawień ochrony urządzenia na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="554f3-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="554f3-104">Sprawdź, czy są ustawione zasady dotyczące urządzeń Windows 10</span><span class="sxs-lookup"><span data-stu-id="554f3-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="554f3-105">Po [Ustawianie zasad urządzeń](protection-settings-for-windows-10-pcs.md)może potrwać do kilku godzin dla zasady obowiązywały na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="554f3-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="554f3-106">Możesz potwierdzić, że zasady weszło w życie patrząc na różnych ekranach ustawienia systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="554f3-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="554f3-107">Ponieważ użytkownicy nie będą mogli modyfikować ustawień usługi Windows Update i Windows Defender Antivirus na swoich urządzeniach Windows 10, wiele z tych opcji będzie wyszarzona.</span><span class="sxs-lookup"><span data-stu-id="554f3-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="554f3-108">Przejdź do **opcji ustawienia** \> **Aktualizacja &amp; zabezpieczenia** \> **Windows Update** \> **Opcje ponownego uruchamiania** i Potwierdź, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="554f3-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Wszystkie opcje ponownego uruchomienia są wyszarzone.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="554f3-110">Przejdź do **opcji ustawienia** \> **Aktualizacja &amp; zabezpieczenia** \> **Witryny Windows Update** \> **Opcje zaawansowane** i Potwierdź, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="554f3-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Opcje zaawansowane systemu Windows aktualizacje są wyszarzone.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="554f3-112">Przejdź do **opcji ustawienia** \> **Aktualizacja &amp; zabezpieczenia** \> **Windows Update** \> **Opcje zaawansowane** \> **Wybierz, w jaki sposób aktualizacje są pobierane**.</span><span class="sxs-lookup"><span data-stu-id="554f3-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="554f3-113">Upewnij się, czy widzisz komunikat (na czerwono), niektóre ustawienia są ukryte lub zarządzanych przez własną organizację, a wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="554f3-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Wybierz sposób dostarczane są aktualizacje strony wskazuje ustawienia są ukryte lub zarządzanych przez własną organizację.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="554f3-115">Aby otworzyć Centrum zabezpieczeń systemu Windows Defender, przejdź do **ustawień** \> **Aktualizacja &amp; zabezpieczenia** \> **Programu Windows Defender** \> kliknij **Otwórz Windows Defender Centrum zabezpieczeń** \> **wirus &amp; wątku Ochrona** \> **wirus &amp; zagrożenie ustawienia ochrony**.</span><span class="sxs-lookup"><span data-stu-id="554f3-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="554f3-116">Sprawdź, czy wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="554f3-116">Verify that all options are greyed out.</span></span> 
    
    ![Ustawienia ochrony wirusów i zagrożeń są wyszarzone.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="554f3-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="554f3-118">Related Topics</span></span>

[<span data-ttu-id="554f3-119">Dokumentacja i zasoby dotyczące usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="554f3-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="554f3-120">Rozpoczynanie pracy z usługą Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="554f3-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="554f3-121">Zarządzanie usługą Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="554f3-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="554f3-122">Konfigurowanie komputerów PC z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="554f3-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

