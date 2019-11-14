---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
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
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzenia za pomocą funkcji AutoPilot w Microsoft 365 Business. Profil można przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320263"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="ad042-104">Tworzenie i edytowanie urządzeń rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ad042-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="ad042-105">Przekazywanie listy urządzeń</span><span class="sxs-lookup"><span data-stu-id="ad042-105">Upload a list of devices</span></span>

<span data-ttu-id="ad042-106">Możesz użyć [przewodnika krok po kroku](add-autopilot-devices-and-profile.md) , aby przesłać urządzenia, ale możesz również przesyłać urządzenia na karcie **urządzenia** .</span><span class="sxs-lookup"><span data-stu-id="ad042-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="ad042-107">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="ad042-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="ad042-108">Windows 10, wersja 1703 lub nowsza</span><span class="sxs-lookup"><span data-stu-id="ad042-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="ad042-109">Nowe urządzenia, które nie zostały przez Windows out-of-Box doświadczenie</span><span class="sxs-lookup"><span data-stu-id="ad042-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="ad042-110">W centrum administracyjnym Microsoft 365 dla firm wybierz opcję **urządzenia** \> **autopilot**.</span><span class="sxs-lookup"><span data-stu-id="ad042-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="ad042-111">Na stronie **autopilot** wybierz kartę \> **urządzenia** , a następnie **Dodaj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="ad042-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="ad042-113">W panelu **Dodaj urządzenia** przejdź do [pliku CSV z listą urządzeń](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , który został przygotowany \> , **Zapisz** \> **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="ad042-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="ad042-114">Można uzyskać te informacje od dostawcy sprzętu lub można użyć [skryptu Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) do generowania pliku CSV.</span><span class="sxs-lookup"><span data-stu-id="ad042-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="ad042-115">Przypisywanie profilu do urządzenia lub grupy urządzeń</span><span class="sxs-lookup"><span data-stu-id="ad042-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="ad042-116">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **urządzenia** i zaznacz pole wyboru obok jednego lub kilku urządzeń.</span><span class="sxs-lookup"><span data-stu-id="ad042-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="ad042-117">W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**.</span><span class="sxs-lookup"><span data-stu-id="ad042-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="ad042-118">Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="ad042-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
