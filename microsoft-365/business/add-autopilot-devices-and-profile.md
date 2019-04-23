---
title: Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak autopilota systemu Windows służy do definiowania nowych urządzeń Windows 10 dla Twojej firmy.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277147"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="7d6f6-103">Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku</span><span class="sxs-lookup"><span data-stu-id="7d6f6-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="7d6f6-104">Rozwiązanie Windows AutoPilot pozwala skonfigurować nowe firmowe urządzenia z systemem Windows 10, tak aby były gotowe do użycia w środowisku produkcyjnym od razu po przekazaniu ich pracownikom.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-104">You can use Windows AutoPilot to set up new Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="7d6f6-105">Wymagania dotyczące urządzeń</span><span class="sxs-lookup"><span data-stu-id="7d6f6-105">Device requirements</span></span>

<span data-ttu-id="7d6f6-106">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="7d6f6-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="7d6f6-107">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="7d6f6-108">Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="7d6f6-109">Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji</span><span class="sxs-lookup"><span data-stu-id="7d6f6-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="7d6f6-110">Jeśli nie utworzono jeszcze grup urządzeń ani profilów, najlepiej rozpocząć pracę przy użyciu przewodnika krok po kroku. Można jednak [dodać urządzenia](create-and-edit-autopilot-devices.md) i [przypisać do nich profile](create-and-edit-autopilot-profiles.md) bez używania tego przewodnika.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-110">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="7d6f6-111">W centrum administracyjnym usługi Microsoft 365 Business przejdź do karty **Akcje urządzenia** i wybierz pozycję **Wdróż system Windows za pomocą rozwiązania Autopilot**.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-111">In the Microsoft 365 Business admin center, locate the **Device actions** card, and choose **Deploy Windows with Autopilot**.</span></span>
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="7d6f6-113">Na stronie **Przygotowywanie systemu Windows** kliknij lub naciśnij pozycję **Uruchom przewodnik**.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-113">On the **Prepare Windows** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="7d6f6-p101">Na stronie **Przekazywanie pliku csv z listą urządzeń** przejdź do lokalizacji, w której znajduje się przygotowany plik CSV, a następnie wybierz pozycję **Otwórz** \> **Dalej**. Plik powinien zawierać trzy nagłówki:</span><span class="sxs-lookup"><span data-stu-id="7d6f6-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="7d6f6-117">Kolumna A: Numer seryjny urządzenia</span><span class="sxs-lookup"><span data-stu-id="7d6f6-117">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="7d6f6-118">Kolumna B: Identyfikator produktu systemu Windows</span><span class="sxs-lookup"><span data-stu-id="7d6f6-118">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="7d6f6-119">Kolumna C: Skrót sprzętowy</span><span class="sxs-lookup"><span data-stu-id="7d6f6-119">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="7d6f6-120">Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik CSV.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-120">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="7d6f6-p102">Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="7d6f6-p103">Na stronie **Przypisywanie profilu** możesz utworzyć nowy lub wybrać istniejący profil. Jeśli nie masz jeszcze profilu, zostanie wyświetlony monit o jego utworzenie.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="7d6f6-125">Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-125">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="7d6f6-p104">Funkcje domyślne są wymagane i zostaną ustawione automatycznie. Funkcje domyślne to:</span><span class="sxs-lookup"><span data-stu-id="7d6f6-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="7d6f6-128">Rejestracja Cortany, usługi OneDrive i producenta OEM jest pomijana.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-128">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="7d6f6-129">Tworzenie środowiska logowania z marką Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-129">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="7d6f6-130">Urządzenia zostaną połączone z kontami usługi Azure Active Directory i automatycznie zarejestrowane na potrzeby zarządzania przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-130">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="7d6f6-131">Aby uzyskać więcej informacji, zobacz</span><span class="sxs-lookup"><span data-stu-id="7d6f6-131">For more information, see</span></span>
    
    <span data-ttu-id="7d6f6-132">[Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="7d6f6-132">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="7d6f6-133">Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-133">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="7d6f6-134">Wybierz przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-134">Choose **Next**.</span></span>
    
6. <span data-ttu-id="7d6f6-p105">Wyświetlenie strony **Gotowe** oznacza, że utworzony (lub wybrany) profil zostanie zastosowany do grupy urządzeń utworzonej po przekazaniu listy urządzeń. Ustawienia te zostaną zastosowane przy następnym logowaniu się użytkowników tych urządzeń. Wybierz pozycję **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="7d6f6-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    