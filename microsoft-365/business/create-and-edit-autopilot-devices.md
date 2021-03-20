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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przekazywać urządzenia za pomocą rozwiązania AutoPilot w uwitrynie Microsoft 365 Business Premium. Profil możesz przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 910abb98b94b749177b04cd12c766f82d348e379
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913403"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="e4ebc-104">Tworzenie i edytowanie urządzeń rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="e4ebc-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="e4ebc-105">Przekazywanie listy urządzeń</span><span class="sxs-lookup"><span data-stu-id="e4ebc-105">Upload a list of devices</span></span>

<span data-ttu-id="e4ebc-106">Aby przekazać [urządzenia,](add-autopilot-devices-and-profile.md) możesz skorzystać z przewodnika krok po kroku, ale możesz również przekazać urządzenia na **karcie** Urządzenia.</span><span class="sxs-lookup"><span data-stu-id="e4ebc-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="e4ebc-107">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="e4ebc-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="e4ebc-108">Windows 10 w wersji 1703 lub nowszej</span><span class="sxs-lookup"><span data-stu-id="e4ebc-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="e4ebc-109">Nowe urządzenia, które nie są już w stanie obsługi klienta systemu Windows</span><span class="sxs-lookup"><span data-stu-id="e4ebc-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="e4ebc-110">W centrum administracyjnym platformy Microsoft 365 wybierz pozycję **Devices** \> **AutoPilot (Rozwiązania rozwiązania Devices AutoPilot).**</span><span class="sxs-lookup"><span data-stu-id="e4ebc-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="e4ebc-111">Na stronie **AutoPilot** wybierz kartę **Urządzenia** Dodaj \> **urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="e4ebc-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="e4ebc-113">W **panelu Dodaj urządzenia** przejdź do przygotowanego przez Ciebie pliku [CSV](../admin/misc/device-list.md) z listą urządzeń i zapisz \>  \> **zamknij.**</span><span class="sxs-lookup"><span data-stu-id="e4ebc-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="e4ebc-114">Możesz uzyskać te informacje od producenta sprzętu lub wygenerować plik CSV za pomocą skryptu programu [PowerShell Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo)</span><span class="sxs-lookup"><span data-stu-id="e4ebc-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="e4ebc-115">Przypisywanie profilu do urządzenia lub grupy urządzeń</span><span class="sxs-lookup"><span data-stu-id="e4ebc-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="e4ebc-116">Na stronie **Przygotowywanie systemu Windows** wybierz **kartę** Urządzenia, a następnie zaznacz pole wyboru obok jednego lub większej liczby urządzeń.</span><span class="sxs-lookup"><span data-stu-id="e4ebc-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="e4ebc-117">W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**.</span><span class="sxs-lookup"><span data-stu-id="e4ebc-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="e4ebc-118">Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="e4ebc-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
