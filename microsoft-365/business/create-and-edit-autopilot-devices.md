---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzenia za pomocą programu AutoPilot w usłudze Microsoft 365 Business Premium. Profil można przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 83c027cfe019e037518c4ca13eb331e5300fc2c1
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165866"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="450a0-104">Tworzenie i edytowanie urządzeń rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="450a0-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="450a0-105">Przekazywanie listy urządzeń</span><span class="sxs-lookup"><span data-stu-id="450a0-105">Upload a list of devices</span></span>

<span data-ttu-id="450a0-106">Możesz użyć [przewodnika krok po kroku,](add-autopilot-devices-and-profile.md) aby przekazać urządzenia, ale możesz też przekazywać urządzenia na karcie **Urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="450a0-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="450a0-107">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="450a0-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="450a0-108">Windows 10, wersja 1703 lub nowsza</span><span class="sxs-lookup"><span data-stu-id="450a0-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="450a0-109">Nowe urządzenia, które nie zostały przez windows out-of-box experience</span><span class="sxs-lookup"><span data-stu-id="450a0-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="450a0-110">W centrum administracyjnym usługi Microsoft 365 wybierz pozycję **Urządzenia** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="450a0-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="450a0-111">Na stronie **Autopilot** wybierz **Devices** kartę \> Urządzenia **Dodawanie urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="450a0-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="450a0-113">Na panelu **Dodawanie urządzeń** przejdź do [przygotowanego pliku CSV listy urządzeń](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) , który został przygotowany \> **Zapisz** \> **zamknij**.</span><span class="sxs-lookup"><span data-stu-id="450a0-113">On the **Add devices** panel, browse to a [Device list CSV file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="450a0-114">Informacje te można uzyskać od dostawcy sprzętu lub użyć [skryptu Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) do wygenerowania pliku CSV.</span><span class="sxs-lookup"><span data-stu-id="450a0-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="450a0-115">Przypisywanie profilu do urządzenia lub grupy urządzeń</span><span class="sxs-lookup"><span data-stu-id="450a0-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="450a0-116">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pole wyboru obok jednego lub większej liczby urządzeń.</span><span class="sxs-lookup"><span data-stu-id="450a0-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="450a0-117">W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**.</span><span class="sxs-lookup"><span data-stu-id="450a0-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="450a0-118">Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="450a0-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
