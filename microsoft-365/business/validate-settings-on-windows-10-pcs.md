---
title: Sprawdzanie poprawności ustawień ochrony aplikacji na komputerach z systemem Windows 10
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Dowiedz się, jak sprawdzić, czy ustawienia ochrony aplikacji usługi Microsoft 365 dla firm zostały zastosowane na urządzeniach z systemem Windows 10 użytkowników.
ms.openlocfilehash: 39aee3bc811cb0090d58f9a282de7a8162c097b3
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403595"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="3f741-103">Sprawdzanie poprawności ustawień ochrony urządzenia na komputerach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="3f741-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="3f741-104">Sprawdzanie, czy ustawiono zasady urządzeń systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="3f741-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="3f741-105">Po [skonfigurowaniu zasad dotyczących urządzeń](protection-settings-for-windows-10-pcs.md)może upłynąć nawet kilka godzin, aby zasady mogły zostać wprowadzone na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3f741-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="3f741-106">Można potwierdzić, że zasady weszły w życie, patrząc na różne ekrany ustawień systemu Windows na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3f741-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="3f741-107">Ponieważ użytkownicy nie będą mogli modyfikować ustawień windows update i windows defender na swoich urządzeniach z systemem Windows 10, wiele opcji będzie wyszarzonych.</span><span class="sxs-lookup"><span data-stu-id="3f741-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="3f741-108">Przejdź do opcji aktualizacji **ustawień** \> \*\* &amp; aktualizacji\*\* \> **systemu Windows Update** Uruchom \> **ponownie** i upewnij się, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="3f741-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Wszystkie opcje ponownego uruchomienia są wyszarzone.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="3f741-110">Przejdź do **opcji Windows** Update zabezpieczeń Windows \> \*\* &amp; \*\* \> **Update** \> **Zaawansowane opcje** i upewnij się, że wszystkie ustawienia są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="3f741-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Opcje aktualizacji zaawansowanych systemu Windows są wyszarzone.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="3f741-112">Przejdź do **pozycji Ustawienia** \> **Aktualizacja &amp; zabezpieczeń** \> **Windows Update** \> **Opcje zaawansowane** \> **Wybierz sposób dostarczania aktualizacji**.</span><span class="sxs-lookup"><span data-stu-id="3f741-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="3f741-113">Upewnij się, że możesz zobaczyć komunikat (na czerwono), że niektóre ustawienia są ukryte lub zarządzane przez organizację, a wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="3f741-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Wybierz sposób dostarczania aktualizacji strona wskazuje ustawienia są ukryte lub zarządzane przez organizację.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="3f741-115">Aby otworzyć Centrum zabezpieczeń usługi Windows Defender, przejdź do **sekcji Ustawienia** \> **aktualizacji &amp; zabezpieczeń** \> **Usługi Windows Defender** \> kliknij pozycję Otwórz usługę Windows Defender Security **Center** \> \*\* &amp; Ochrona wątków\*\* \> **Ustawienia ochrony &amp; przed zagrożeniami przed wirusami**.</span><span class="sxs-lookup"><span data-stu-id="3f741-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="3f741-116">Sprawdź, czy wszystkie opcje są wyszarzone.</span><span class="sxs-lookup"><span data-stu-id="3f741-116">Verify that all options are grayed out.</span></span> 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarzone.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="3f741-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="3f741-118">Related Topics</span></span>

[<span data-ttu-id="3f741-119">Microsoft 365 dla dokumentacji biznesowej i zasobów</span><span class="sxs-lookup"><span data-stu-id="3f741-119">Microsoft 365 for business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="3f741-120">Wprowadzenie do usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="3f741-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="3f741-121">Zarządzanie programem Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="3f741-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="3f741-122">Konfigurowanie komputerów PC z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="3f741-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

