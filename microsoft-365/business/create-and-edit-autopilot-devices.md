---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzeń za pomocą autopilota w Microsoft 365 Business. Można przypisać profil do urządzenia lub grupy urządzeń.
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982937"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="61e5e-104">Tworzenie i edytowanie urządzeń rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="61e5e-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="61e5e-105">Przekazywanie listy urządzeń</span><span class="sxs-lookup"><span data-stu-id="61e5e-105">Upload a list of devices</span></span>

<span data-ttu-id="61e5e-106">Aby przekazać urządzenia, możesz skorzystać z [przewodnika krok po kroku](add-autopilot-devices-and-profile.md), ale możesz to również zrobić przy użyciu karty **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="61e5e-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="61e5e-107">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="61e5e-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="61e5e-108">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="61e5e-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="61e5e-109">Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="61e5e-109">New devices that have not been through Windows out-of-box experience.</span></span>
    
1. <span data-ttu-id="61e5e-110">W centrum administracyjnym usług Microsoft 365 Business wybierz pozycję **Wdróż system Windows za pomocą rozwiązania Autopilot** na karcie **Akcje urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="61e5e-110">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="61e5e-112">Na stronie **Przygotowanie systemu Windows** wybierz kartę **urządzenia** \> **Dodaj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="61e5e-112">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="61e5e-114">Na panelu **Dodaj urządzenia** , przejdź do [pliku CSV lista urządzeń](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , przygotowanego \> **zapisać** \> **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="61e5e-114">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="61e5e-115">Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik csv.</span><span class="sxs-lookup"><span data-stu-id="61e5e-115">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="61e5e-116">Przypisywanie profilu do urządzenia lub grupy urządzeń</span><span class="sxs-lookup"><span data-stu-id="61e5e-116">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="61e5e-117">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pola wyboru obok odpowiednich urządzeń.</span><span class="sxs-lookup"><span data-stu-id="61e5e-117">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="61e5e-118">W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**.</span><span class="sxs-lookup"><span data-stu-id="61e5e-118">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="61e5e-119">Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="61e5e-119">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
