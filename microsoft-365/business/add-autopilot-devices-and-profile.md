---
title: Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak skonfigurować nowe urządzenia z systemem Windows 10 dla firmy za pomocą programu AutoPilot systemu Windows 10.
ms.openlocfilehash: 1fd0abb76d16b79dd11ef27b6b27a87894d89ef9
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593278"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="98f7c-103">Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku</span><span class="sxs-lookup"><span data-stu-id="98f7c-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="98f7c-104">Za pomocą programu AutoPilot systemu Windows można skonfigurować **nowe** urządzenia z systemem Windows 10 dla Twojej firmy, aby były gotowe do użycia, gdy dasz je pracownikom.</span><span class="sxs-lookup"><span data-stu-id="98f7c-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="98f7c-105">Wymagania dotyczące urządzeń</span><span class="sxs-lookup"><span data-stu-id="98f7c-105">Device requirements</span></span>

<span data-ttu-id="98f7c-106">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="98f7c-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="98f7c-107">Windows 10, wersja 1703 lub nowsza</span><span class="sxs-lookup"><span data-stu-id="98f7c-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="98f7c-108">Nowe urządzenia, które nie przeszły przez system Windows gotowe do obsługi</span><span class="sxs-lookup"><span data-stu-id="98f7c-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="98f7c-109">Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji</span><span class="sxs-lookup"><span data-stu-id="98f7c-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="98f7c-110">[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="98f7c-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="98f7c-111">Jeśli nie utworzono jeszcze grup urządzeń ani profilów, najlepszym sposobem na rozpoczęcie pracy jest użycie przewodnika krok po kroku.</span><span class="sxs-lookup"><span data-stu-id="98f7c-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="98f7c-112">Można również [dodawać do](create-and-edit-autopilot-devices.md) nich urządzenia i [przypisywać do](create-and-edit-autopilot-profiles.md) nich profile bez użycia przewodnika.</span><span class="sxs-lookup"><span data-stu-id="98f7c-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="98f7c-113">Przejdź do centrum <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administracyjnego pod adresem .</span><span class="sxs-lookup"><span data-stu-id="98f7c-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="98f7c-114">W lewym okienku nawigacji wybierz pozycję **Urządzenia** \> **Autopilot**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![W centrum administracyjnym wybierz urządzenia, a następnie Autopilota.](media/AutoPilot.png)
  
2. <span data-ttu-id="98f7c-116">Na stronie **Autopilot** kliknij lub naciśnij **pozycję Przewodnik startowy**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="98f7c-118">Na **stronie Prześlij plik csv z listą urządzeń** przejdź do lokalizacji, w której masz przygotowane . CSV, a następnie **otwórz** \> **dalej**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="98f7c-119">Plik musi mieć trzy nagłówki:</span><span class="sxs-lookup"><span data-stu-id="98f7c-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="98f7c-120">Kolumna A: Numer seryjny urządzenia</span><span class="sxs-lookup"><span data-stu-id="98f7c-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="98f7c-121">Kolumna B: Identyfikator produktu systemu Windows</span><span class="sxs-lookup"><span data-stu-id="98f7c-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="98f7c-122">Kolumna C: Skrót sprzętowy</span><span class="sxs-lookup"><span data-stu-id="98f7c-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="98f7c-123">Te informacje można uzyskać od dostawcy sprzętu lub użyć [skryptu Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) do wygenerowania pliku CSV.</span><span class="sxs-lookup"><span data-stu-id="98f7c-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="98f7c-p103">Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-p103">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="98f7c-126">Na stronie **Przypisywanie profilu** można wybrać istniejący profil lub utworzyć nowy.</span><span class="sxs-lookup"><span data-stu-id="98f7c-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="98f7c-127">Jeśli jeszcze go nie masz, zostanie wyświetlony monit o jego utworzenie.</span><span class="sxs-lookup"><span data-stu-id="98f7c-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="98f7c-128">Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="98f7c-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="98f7c-129">Funkcje domyślne są wymagane i są ustawiane automatycznie.</span><span class="sxs-lookup"><span data-stu-id="98f7c-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="98f7c-130">Funkcje domyślne to:</span><span class="sxs-lookup"><span data-stu-id="98f7c-130">The default features are:</span></span>
    
    - <span data-ttu-id="98f7c-131">Pomiń cortanę, onedrive i rejestrację OEM.</span><span class="sxs-lookup"><span data-stu-id="98f7c-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="98f7c-132">Tworzenie środowiska logowania z marką Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="98f7c-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="98f7c-133">Połącz urządzenia z kontami usługi Azure Active Directory i automatycznie rejestruj je, aby były zarządzane przez firmę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="98f7c-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="98f7c-134">Aby uzyskać więcej informacji, zobacz [Ustawienia profilu autopilota](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="98f7c-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="98f7c-135">Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="98f7c-136">Wybierz przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="98f7c-137">**Gotowe zdjęcie** wskazuje, że utworzony (lub wybrany) profil zostanie zastosowany do utworzonej grupy urządzeń, przesyłając listę urządzeń.</span><span class="sxs-lookup"><span data-stu-id="98f7c-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="98f7c-138">Ustawienia będą obowiązywać, gdy użytkownicy urządzenia zalogują się w następnej kolejności.</span><span class="sxs-lookup"><span data-stu-id="98f7c-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="98f7c-139">Wybierz pozycję **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="98f7c-139">Choose **Close**.</span></span>
    