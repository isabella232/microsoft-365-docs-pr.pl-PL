---
title: Tworzenie i edytowanie profilów rozwiązania AutoPilot
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Dowiedz się, tworzenie, edytowanie, usuwanie lub Usuń profile autopilota. '
ms.openlocfilehash: 85fc897b2f428afae8d55feeb577021adaa30f72
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277154"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="cb0e1-103">Tworzenie i edytowanie profilów rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="cb0e1-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="cb0e1-104">Tworzenie profilu</span><span class="sxs-lookup"><span data-stu-id="cb0e1-104">Create a profile</span></span>

<span data-ttu-id="cb0e1-105">Profil dotyczy urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="cb0e1-106">W Centrum administrator firmy Microsoft 365, wybierz **urządzenia** \> **autopilota**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="cb0e1-107">Na stronie **autopilota** , wybierz kartę **Profile** \> **Utwórz profil**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="cb0e1-108">Na stronie **Tworzenie profilu** wprowadź opisową nazwę profilu, na przykład Marketing, włącz odpowiednie ustawienia (więcej informacji można znaleźć w temacie [Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md)) i wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="cb0e1-110">Stosowanie profilu do urządzenia</span><span class="sxs-lookup"><span data-stu-id="cb0e1-110">Apply profile to a device</span></span>

<span data-ttu-id="cb0e1-p101">Utworzony profil można zastosować do urządzenia lub grupy urządzeń. W [przewodniku krok po kroku](add-autopilot-devices-and-profile.md) można wybrać istniejący profil i zastosować go do nowych urządzeń lub zamienić istniejący profil dla urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="cb0e1-113">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="cb0e1-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="cb0e1-116">Edytowanie, usuwanie lub czyszczenie profilu</span><span class="sxs-lookup"><span data-stu-id="cb0e1-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="cb0e1-p102">Profil przypisany do urządzenia można zaktualizować, nawet jeśli już przekazano urządzenie użytkownikowi. Gdy urządzenie łączy się z Internetem, pobiera najnowszą wersję profilu w procesie konfiguracji. Jeśli użytkownik przywróci domyślne ustawienia fabryczne na urządzeniu, ponownie pobierze ono najnowsze aktualizacje profilu.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="cb0e1-120">Edytowanie profilu</span><span class="sxs-lookup"><span data-stu-id="cb0e1-120">Edit a profile</span></span>

1. <span data-ttu-id="cb0e1-121">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="cb0e1-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="cb0e1-123">Jeśli zrobisz to, zanim urządzenie użytkownika połączy się z Internetem, profil zostanie zastosowany w procesie konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="cb0e1-124">Usuwanie profilu</span><span class="sxs-lookup"><span data-stu-id="cb0e1-124">Delete a profile</span></span>

1. <span data-ttu-id="cb0e1-125">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="cb0e1-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="cb0e1-127">Usunięty profil zostaje odłączony od urządzenia lub grupy urządzeń, do których go przypisano.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="cb0e1-128">Czyszczenie profilu</span><span class="sxs-lookup"><span data-stu-id="cb0e1-128">Remove a profile</span></span>

1. <span data-ttu-id="cb0e1-129">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="cb0e1-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="cb0e1-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    