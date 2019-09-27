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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzenia za pomocą funkcji AutoPilot w Microsoft 365 Business. Profil można przypisać do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 9ae94266f5a41d8d115fc92f0f080a6fdbdc9f15
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288020"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="e8d5c-104">Tworzenie i edytowanie urządzeń rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="e8d5c-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="e8d5c-105">Przekazywanie listy urządzeń</span><span class="sxs-lookup"><span data-stu-id="e8d5c-105">Upload a list of devices</span></span>

<span data-ttu-id="e8d5c-106">Aby przekazać urządzenia, możesz skorzystać z [przewodnika krok po kroku](add-autopilot-devices-and-profile.md), ale możesz to również zrobić przy użyciu karty **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="e8d5c-107">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="e8d5c-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="e8d5c-108">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="e8d5c-109">Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="e8d5c-110">W centrum administracyjnym Microsoft 365 dla firm wybierz opcję **urządzenia** \> **autopilot**.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="e8d5c-111">Na stronie **autopilot** wybierz kartę \> **urządzenia** , a następnie **Dodaj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="e8d5c-113">Na **Dodaj urządzenia** panelu, przejdź do [listy urządzeń CSV-plik](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , który został przygotowany \> **Zapisz** \> **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="e8d5c-114">Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik csv.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="e8d5c-115">Przypisywanie profilu do urządzenia lub grupy urządzeń</span><span class="sxs-lookup"><span data-stu-id="e8d5c-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="e8d5c-116">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pola wyboru obok odpowiednich urządzeń.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="e8d5c-117">W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**.</span><span class="sxs-lookup"><span data-stu-id="e8d5c-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="e8d5c-118">Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="e8d5c-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
