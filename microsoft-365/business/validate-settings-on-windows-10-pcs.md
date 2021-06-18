---
title: Sprawdzanie poprawności ustawień ochrony aplikacji dla Windows 10 PC
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Dowiedz się, jak sprawdzić Microsoft 365 ustawienia ochrony aplikacji dla firm miały wpływ na ustawienia ochrony aplikacji Windows 10 urządzeniach.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925264"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="e2a0d-103">Sprawdzanie poprawności ustawień ochrony urządzeń dla Windows 10 PC</span><span class="sxs-lookup"><span data-stu-id="e2a0d-103">Validate device protection settings for Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="e2a0d-104">Sprawdzanie, czy Windows 10 urządzenia są ustawione</span><span class="sxs-lookup"><span data-stu-id="e2a0d-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="e2a0d-105">Po [skonfigurowaniu zasad urządzeń](protection-settings-for-windows-10-pcs.md)może upłynieć kilka godzin, aż te zasady zajdą w życie na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="e2a0d-106">Aby potwierdzić, że zasady te obowiązywały, możesz sprawdzić, Windows Ustawienia ekranów na urządzeniach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="e2a0d-107">Ponieważ użytkownicy nie będą mogli modyfikować ustawień aktualizacji Windows i ustawień Program antywirusowy Windows Defender na swoich Windows 10 urządzeniach, wiele opcji zostanie wyszarzeni.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="e2a0d-108">Przejdź do **Ustawienia** Opcje ponownego uruchamiania Windows aktualizacji i upewnij się, że wszystkie ustawienia \> **&amp;** \>  \>  są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Wszystkie opcje Uruchom ponownie są wyszarowane.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="e2a0d-110">Przejdź do **Ustawienia** Opcje aktualizacji Windows Zaawansowane i upewnij się, że wszystkie ustawienia \> **&amp;** \>  \>  są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows Opcje aktualizacji zaawansowanych są wyszarowane.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="e2a0d-112">Przejdź do **Ustawienia** Opcje zaawansowane aktualizacji Windows Opcje aktualizacji Wybierz \> **&amp;** sposób \>  \>  \> **dostarczenia aktualizacji.**</span><span class="sxs-lookup"><span data-stu-id="e2a0d-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="e2a0d-113">Potwierdź, że widzisz komunikat (kolor czerwony), że niektóre ustawienia są ukryte lub zarządzane przez Twoją organizację, a wszystkie opcje są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Strona Wybieranie sposobu dostarczenia aktualizacji wskazuje, że ustawienia są ukryte lub zarządzane przez Organizację.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="e2a0d-115">Aby otworzyć Centrum zabezpieczeń Windows Defender,  przejdź do Ustawienia aktualizacji zabezpieczeń i Windows Defender pozycję Otwórz Windows Defender Ochronę wątku wirusów ustawieniami ochrony przed zagrożeniami \> **&amp;** \>  \>  \> **&amp;** \> **&amp; antywirusowymi.**</span><span class="sxs-lookup"><span data-stu-id="e2a0d-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="e2a0d-116">Sprawdź, czy wszystkie opcje są wyszarowane.</span><span class="sxs-lookup"><span data-stu-id="e2a0d-116">Verify that all options are grayed out.</span></span> 
    
    ![Ustawienia ochrony przed wirusami i zagrożeniami są wyszarowane.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="e2a0d-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="e2a0d-118">Related Topics</span></span>

[<span data-ttu-id="e2a0d-119">Microsoft 365 i zasoby dla firm</span><span class="sxs-lookup"><span data-stu-id="e2a0d-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="e2a0d-120">Wprowadzenie do usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="e2a0d-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="e2a0d-121">Zarządzanie Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="e2a0d-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="e2a0d-122">Konfigurowanie komputerów PC z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="e2a0d-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
