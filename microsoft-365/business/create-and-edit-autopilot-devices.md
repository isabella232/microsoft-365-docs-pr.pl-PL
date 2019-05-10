---
title: Tworzenie i edytowanie urządzeń rozwiązania AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Dowiedz się, jak przesyłać urządzeń za pomocą autopilota w Microsoft 365 Business. Można przypisać profil do urządzenia lub grupy urządzeń.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660441"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="adcaa-104">Tworzenie i edytowanie urządzeń rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="adcaa-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="adcaa-105">Przekazywanie listy urządzeń</span><span class="sxs-lookup"><span data-stu-id="adcaa-105">Upload a list of devices</span></span>

<span data-ttu-id="adcaa-106">Aby przekazać urządzenia, możesz skorzystać z [przewodnika krok po kroku](add-autopilot-devices-and-profile.md), ale możesz to również zrobić przy użyciu karty **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="adcaa-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="adcaa-107">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="adcaa-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="adcaa-108">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="adcaa-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="adcaa-109">Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="adcaa-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="adcaa-110">W Centrum administrator firmy Microsoft 365, wybierz **urządzenia** \> **autopilota**.</span><span class="sxs-lookup"><span data-stu-id="adcaa-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="adcaa-111">Na stronie **autopilota** , wybierz kartę **urządzenia** \> **Dodaj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="adcaa-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="adcaa-113">Na panelu **Dodaj urządzenia** , przejdź do [pliku CSV lista urządzeń](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , przygotowanego \> **zapisać** \> **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="adcaa-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="adcaa-114">Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik csv.</span><span class="sxs-lookup"><span data-stu-id="adcaa-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="adcaa-115">Przypisywanie profilu do urządzenia lub grupy urządzeń</span><span class="sxs-lookup"><span data-stu-id="adcaa-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="adcaa-116">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia** i zaznacz pola wyboru obok odpowiednich urządzeń.</span><span class="sxs-lookup"><span data-stu-id="adcaa-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="adcaa-117">W panelu **Urządzenie** wybierz profil z listy rozwijanej **Przypisany profil**.</span><span class="sxs-lookup"><span data-stu-id="adcaa-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="adcaa-118">Jeśli nie masz jeszcze żadnych profilów, odpowiednie instrukcje znajdziesz w temacie [Tworzenie i edytowanie profilów rozwiązania AutoPilot](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="adcaa-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
