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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Dowiedz się, jak za pomocą rozwiązania Windows AutoPilot skonfigurować nowe urządzenia z systemem Windows 10 dla swojej firmy, aby były gotowe do użytku przez pracowników.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913507"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="14159-103">Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku</span><span class="sxs-lookup"><span data-stu-id="14159-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="14159-104">Korzystając z rozwiązania Windows AutoPilot, możesz skonfigurować nowe urządzenia z systemem **Windows** 10 dla swojej firmy, aby były gotowe do użycia, gdy podasz je pracownikom.</span><span class="sxs-lookup"><span data-stu-id="14159-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="14159-105">Wymagania dotyczące urządzeń</span><span class="sxs-lookup"><span data-stu-id="14159-105">Device requirements</span></span>

<span data-ttu-id="14159-106">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="14159-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="14159-107">Windows 10 w wersji 1703 lub nowszej</span><span class="sxs-lookup"><span data-stu-id="14159-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="14159-108">Nowe urządzenia, które nie są już w stanie obsługi klienta systemu Windows</span><span class="sxs-lookup"><span data-stu-id="14159-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="14159-109">Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji</span><span class="sxs-lookup"><span data-stu-id="14159-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="14159-110">[![Etykieta informująca, że centrum administracyjne zmienia się, a więcej informacji na ten temat możesz znaleźć w witrynie aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="14159-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="14159-111">Jeśli jeszcze nie utworzono grup urządzeń ani profilów, najlepiej rozpocząć pracę, korzystając z przewodnika krok po kroku.</span><span class="sxs-lookup"><span data-stu-id="14159-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="14159-112">Możesz również dodawać [urządzenia i przypisywać](create-and-edit-autopilot-devices.md) [do](create-and-edit-autopilot-profiles.md) nich profile bez korzystania z przewodnika.</span><span class="sxs-lookup"><span data-stu-id="14159-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="14159-113">Przejdź do centrum administracyjnego w stronie <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="14159-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="14159-114">W lewym okienku nawigacji wybierz pozycję **Devices** \> **AutoPilot (Rozwiązania rozwiązania Devices AutoPilot).**</span><span class="sxs-lookup"><span data-stu-id="14159-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![W centrum administracyjnym wybierz pozycję urządzenia, a następnie pozycję AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="14159-116">Na stronie **AutoPilot (Autopilot)** kliknij lub naciśnij pozycję **Uruchom przewodnik**.</span><span class="sxs-lookup"><span data-stu-id="14159-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="14159-118">Na **stronie Przekaż plik csv z listą urządzeń** przejdź do lokalizacji, w której się znajdujesz . CSV, a następnie **otwórz** \> **dalej.**</span><span class="sxs-lookup"><span data-stu-id="14159-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="14159-119">Plik musi zawierać trzy nagłówki:</span><span class="sxs-lookup"><span data-stu-id="14159-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="14159-120">Kolumna A: Numer seryjny urządzenia</span><span class="sxs-lookup"><span data-stu-id="14159-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="14159-121">Kolumna B: Identyfikator produktu systemu Windows</span><span class="sxs-lookup"><span data-stu-id="14159-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="14159-122">Kolumna C: Skrót sprzętowy</span><span class="sxs-lookup"><span data-stu-id="14159-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="14159-123">Możesz uzyskać te informacje od producenta sprzętu lub wygenerować plik CSV za pomocą skryptu programu [PowerShell Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo)</span><span class="sxs-lookup"><span data-stu-id="14159-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="14159-p103">Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](../admin/misc/device-list.md). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="14159-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="14159-126">Ten skrypt używa usługi WMI do pobierania właściwości potrzebnych klientowi do zarejestrowania urządzenia za pomocą rozwiązania Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="14159-126">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="14159-127">Zwróć uwagę, że w wynikowym pliku CSV normalne jest nieuzyskanie wartości PKID ,ponieważ nie jest to wymagane do zarejestrowania urządzenia, a wartość PKID w wyjściowym pliku CSV jest całkowicie prawidłowa.</span><span class="sxs-lookup"><span data-stu-id="14159-127">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="14159-128">Zostanie wypełniony tylko numer seryjny i skrót sprzętowy.</span><span class="sxs-lookup"><span data-stu-id="14159-128">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="14159-129">Na **stronie Przypisywanie profilu** możesz wybrać istniejący profil lub utworzyć nowy.</span><span class="sxs-lookup"><span data-stu-id="14159-129">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="14159-130">Jeśli nie masz jeszcze konta, zostanie wyświetlony monit o jego utworzenie.</span><span class="sxs-lookup"><span data-stu-id="14159-130">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="14159-131">Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="14159-131">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="14159-132">Funkcje domyślne są wymagane i ustawiane automatycznie.</span><span class="sxs-lookup"><span data-stu-id="14159-132">The default features are required and are set automatically.</span></span> <span data-ttu-id="14159-133">Funkcje domyślne to:</span><span class="sxs-lookup"><span data-stu-id="14159-133">The default features are:</span></span>
    
    - <span data-ttu-id="14159-134">Pomiń rejestrację Cortany, usługi OneDrive i OEM.</span><span class="sxs-lookup"><span data-stu-id="14159-134">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="14159-135">Tworzenie środowiska logowania z marką Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="14159-135">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="14159-136">Połącz urządzenia z kontami usługi Azure Active Directory i automatycznie zarejestruj je, aby być zarządzane przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="14159-136">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="14159-137">Aby uzyskać więcej informacji, zobacz [Ustawienia profilu rozwiązania AutoPilot — informacje.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="14159-137">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="14159-138">Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="14159-138">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="14159-139">Wybierz przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="14159-139">Choose **Next**.</span></span>
    
6. <span data-ttu-id="14159-140">**Wszystko gotowe oznacza,** że utworzony (lub wybrany) profil zostanie zastosowany do grupy urządzeń utworzonej po przesłaniu listy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="14159-140">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="14159-141">Ustawienia zostaną wprowadzone, gdy użytkownicy urządzenia zalogują się dalej.</span><span class="sxs-lookup"><span data-stu-id="14159-141">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="14159-142">Wybierz pozycję **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="14159-142">Choose **Close**.</span></span>
