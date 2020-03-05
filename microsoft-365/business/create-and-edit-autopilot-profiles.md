---
title: Tworzenie i edytowanie profilów rozwiązania AutoPilot
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Dowiedz się, jak utworzyć profil AutoPilota i zastosować go do urządzenia, a także edytować lub usunąć profil lub usunąć profil z urządzenia.
ms.openlocfilehash: 6a8057969242d839ebbb4cbef8d26dd3f1858c59
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417341"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="9899a-103">Tworzenie i edytowanie profilów rozwiązania AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9899a-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="9899a-104">Tworzenie profilu</span><span class="sxs-lookup"><span data-stu-id="9899a-104">Create a profile</span></span>

<span data-ttu-id="9899a-105">Profil dotyczy urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="9899a-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="9899a-106">W centrum administracyjnym programu Microsoft 365 Business wybierz pozycję **Autopilot** **urządzeń** \> .</span><span class="sxs-lookup"><span data-stu-id="9899a-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="9899a-107">Na stronie **Autopilot** wybierz kartę **Profile** \> **stwórz profil**.</span><span class="sxs-lookup"><span data-stu-id="9899a-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="9899a-108">Na stronie **Tworzenie profilu** wprowadź nazwę profilu, który pomaga go zidentyfikować, na przykład Marketing.</span><span class="sxs-lookup"><span data-stu-id="9899a-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="9899a-109">Włącz żądane ustawienie, a następnie wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9899a-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="9899a-110">Aby uzyskać więcej informacji na temat ustawień profilu AutoPilot, zobacz [Ustawienia profilu AutoPilota](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="9899a-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="9899a-112">Stosowanie profilu do urządzenia</span><span class="sxs-lookup"><span data-stu-id="9899a-112">Apply profile to a device</span></span>

<span data-ttu-id="9899a-113">Po utworzeniu profilu można go zastosować do urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="9899a-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="9899a-114">Możesz wybrać istniejący profil w [przewodniku krok po kroku](add-autopilot-devices-and-profile.md) i zastosować go do nowych urządzeń lub zastąpić istniejący profil dla urządzenia lub grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="9899a-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="9899a-115">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="9899a-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9899a-116">Zaznacz pole wyboru obok nazwy urządzenia, a następnie w panelu **Urządzenie** wybierz profil \> z listy rozwijanej **Przypisany profil** **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9899a-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="9899a-118">Edytowanie, usuwanie lub czyszczenie profilu</span><span class="sxs-lookup"><span data-stu-id="9899a-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="9899a-p103">Profil przypisany do urządzenia można zaktualizować, nawet jeśli już przekazano urządzenie użytkownikowi. Gdy urządzenie łączy się z Internetem, pobiera najnowszą wersję profilu w procesie konfiguracji. Jeśli użytkownik przywróci domyślne ustawienia fabryczne na urządzeniu, ponownie pobierze ono najnowsze aktualizacje profilu.</span><span class="sxs-lookup"><span data-stu-id="9899a-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="9899a-122">Edytowanie profilu</span><span class="sxs-lookup"><span data-stu-id="9899a-122">Edit a profile</span></span>

1. <span data-ttu-id="9899a-123">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**.</span><span class="sxs-lookup"><span data-stu-id="9899a-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9899a-124">Zaznacz pole wyboru obok nazwy urządzenia, \*\*\*\* a następnie w panelu \> Profil zaktualizuj dowolne z dostępnych ustawień **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9899a-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="9899a-125">Jeśli zrobisz to, zanim urządzenie użytkownika połączy się z Internetem, profil zostanie zastosowany w procesie konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="9899a-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="9899a-126">Usuwanie profilu</span><span class="sxs-lookup"><span data-stu-id="9899a-126">Delete a profile</span></span>

1. <span data-ttu-id="9899a-127">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Profile**.</span><span class="sxs-lookup"><span data-stu-id="9899a-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9899a-128">Zaznacz pole wyboru obok nazwy urządzenia, a następnie w panelu **Profil** wybierz polecenie **Usuń zapisywanie** **profilu** \> .</span><span class="sxs-lookup"><span data-stu-id="9899a-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="9899a-129">Usunięty profil zostaje odłączony od urządzenia lub grupy urządzeń, do których go przypisano.</span><span class="sxs-lookup"><span data-stu-id="9899a-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="9899a-130">Czyszczenie profilu</span><span class="sxs-lookup"><span data-stu-id="9899a-130">Remove a profile</span></span>

1. <span data-ttu-id="9899a-131">Na stronie **Przygotowywanie systemu Windows** wybierz kartę **Urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="9899a-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9899a-132">Zaznacz pole wyboru obok nazwy urządzenia, a następnie w panelu **Urządzenie** wybierz pozycję \> **Brak** z listy rozwijanej **Przypisany profil** **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9899a-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
