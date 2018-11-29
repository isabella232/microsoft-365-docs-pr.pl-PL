---
title: Tworzenie i edytowanie profilów rozwiązania AutoPilot
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Dowiedz się, tworzenie, edytowanie, usuwanie lub Usuń profile autopilota. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983137"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="7870c-103">Tworzenie i edytowanie profilów rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="7870c-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="7870c-104">Tworzenie profilu</span><span class="sxs-lookup"><span data-stu-id="7870c-104">Create a profile</span></span>

<span data-ttu-id="7870c-105">Profil dotyczy urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="7870c-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="7870c-106">W centrum administracyjnym usług Microsoft 365 Business wybierz pozycję **Wdróż system Windows za pomocą rozwiązania Autopilot** na karcie **Akcje urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="7870c-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="7870c-108">Na stronie **Przygotowanie systemu Windows** wybierz kartę **Profile** \> **Utwórz profil**.</span><span class="sxs-lookup"><span data-stu-id="7870c-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="7870c-109">Na stronie **Tworzenie profilu** wprowadź opisową nazwę profilu, na przykład Marketing, włącz odpowiednie ustawienia (więcej informacji można znaleźć w temacie [Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md)) i wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="7870c-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="7870c-111">Stosowanie profilu do urządzenia</span><span class="sxs-lookup"><span data-stu-id="7870c-111">Apply profile to a device</span></span>

<span data-ttu-id="7870c-p101">Utworzony profil można zastosować do urządzenia lub grupy urządzeń. W [przewodniku krok po kroku](add-autopilot-devices-and-profile.md) można wybrać istniejący profil i zastosować go do nowych urządzeń lub zamienić istniejący profil dla urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="7870c-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="7870c-114">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="7870c-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="7870c-115">Kliknij pole wyboru obok nazwy urządzenia, jak i w panelu **urządzenia** , wybierz profil z listy rozwijanej **przypisany profil** \> **zapisać**.</span><span class="sxs-lookup"><span data-stu-id="7870c-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="7870c-117">Edytowanie, usuwanie lub czyszczenie profilu</span><span class="sxs-lookup"><span data-stu-id="7870c-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="7870c-p102">Profil przypisany do urządzenia można zaktualizować, nawet jeśli już przekazano urządzenie użytkownikowi. Gdy urządzenie łączy się z Internetem, pobiera najnowszą wersję profilu w procesie konfiguracji. Jeśli użytkownik przywróci domyślne ustawienia fabryczne na urządzeniu, ponownie pobierze ono najnowsze aktualizacje profilu.</span><span class="sxs-lookup"><span data-stu-id="7870c-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="7870c-121">Edytowanie profilu</span><span class="sxs-lookup"><span data-stu-id="7870c-121">Edit a profile</span></span>

1. <span data-ttu-id="7870c-122">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**.</span><span class="sxs-lookup"><span data-stu-id="7870c-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="7870c-123">Kliknij pole wyboru obok nazwy urządzenia i w **profilu** panelu zaktualizować dowolne dostępne ustawienia \> **zapisać**.</span><span class="sxs-lookup"><span data-stu-id="7870c-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="7870c-124">Jeśli zrobisz to, zanim urządzenie użytkownika połączy się z Internetem, profil zostanie zastosowany w procesie konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="7870c-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="7870c-125">Usuwanie profilu</span><span class="sxs-lookup"><span data-stu-id="7870c-125">Delete a profile</span></span>

1. <span data-ttu-id="7870c-126">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**.</span><span class="sxs-lookup"><span data-stu-id="7870c-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="7870c-127">Kliknij pole wyboru obok nazwy urządzenia, a w panelu **profilu** kliknij przycisk **Usuń profil** \> **zapisać**.</span><span class="sxs-lookup"><span data-stu-id="7870c-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="7870c-128">Usunięty profil zostaje odłączony od urządzenia lub grupy urządzeń, do których go przypisano.</span><span class="sxs-lookup"><span data-stu-id="7870c-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="7870c-129">Czyszczenie profilu</span><span class="sxs-lookup"><span data-stu-id="7870c-129">Remove a profile</span></span>

1. <span data-ttu-id="7870c-130">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="7870c-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="7870c-131">Kliknij pole wyboru obok nazwy urządzenia, jak i w panelu **urządzenia** , wybierz opcję **Brak** z listy rozwijanej **przypisany profil** \> **zapisać**.</span><span class="sxs-lookup"><span data-stu-id="7870c-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
