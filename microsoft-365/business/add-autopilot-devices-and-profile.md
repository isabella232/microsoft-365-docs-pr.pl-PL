---
title: Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku
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
description: Dowiedz się, jak używać programu Windows AutoPilot do konfigurowania nowych urządzeń z systemem Windows 10 dla Twojej firmy.
ms.openlocfilehash: d028ea3e902965d55c445dc3b3a02aa315201b25
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574793"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="97d85-103">Dodawanie urządzeń i profilu rozwiązania Autopilot przy użyciu przewodnika krok po kroku</span><span class="sxs-lookup"><span data-stu-id="97d85-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="97d85-104">Za pomocą programu Windows AutoPilot można skonfigurować **nowe** urządzenia z systemem Windows 10 dla firmy, aby były gotowe do użytku produktywnego, gdy tylko podasz je pracownikom.</span><span class="sxs-lookup"><span data-stu-id="97d85-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="97d85-105">Wymagania dotyczące urządzeń</span><span class="sxs-lookup"><span data-stu-id="97d85-105">Device requirements</span></span>

<span data-ttu-id="97d85-106">Urządzenia muszą spełniać następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="97d85-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="97d85-107">System Windows 10 w wersji 1703 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="97d85-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="97d85-108">Nowe urządzenia, które nie są składnikami gotowych rozwiązań z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="97d85-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="97d85-109">Tworzenie urządzeń i profilów za pomocą przewodnika konfiguracji</span><span class="sxs-lookup"><span data-stu-id="97d85-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="97d85-110">[![Etykieta, aby poinformować, że centrum admin zmienia się i można znaleźć więcej szczegółów na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="97d85-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="97d85-111">Jeśli nie utworzono jeszcze grup urządzeń ani profilów, najlepiej rozpocząć pracę przy użyciu przewodnika krok po kroku. Można jednak [dodać urządzenia](create-and-edit-autopilot-devices.md) i [przypisać do nich profile](create-and-edit-autopilot-profiles.md) bez używania tego przewodnika.</span><span class="sxs-lookup"><span data-stu-id="97d85-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="97d85-112">Przejdź do centrum administracyjnego w <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="97d85-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="97d85-113">Na lewej NAV wybierz **urządzenia** \> **autopilot**.</span><span class="sxs-lookup"><span data-stu-id="97d85-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![W centrum administracyjnym wybierz urządzenia, a następnie AutoPilot.](media/AutoPilot.png)
  
2. <span data-ttu-id="97d85-115">Na stronie **autopilot** kliknij lub naciśnij pozycję **Uruchom przewodnik**.</span><span class="sxs-lookup"><span data-stu-id="97d85-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="97d85-p101">Na stronie **Przekazywanie pliku csv z listą urządzeń** przejdź do lokalizacji, w której znajduje się przygotowany plik CSV, a następnie wybierz pozycję **Otwórz** \> **Dalej**. Plik powinien zawierać trzy nagłówki:</span><span class="sxs-lookup"><span data-stu-id="97d85-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="97d85-119">Kolumna A: Numer seryjny urządzenia</span><span class="sxs-lookup"><span data-stu-id="97d85-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="97d85-120">Kolumna B: Identyfikator produktu systemu Windows</span><span class="sxs-lookup"><span data-stu-id="97d85-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="97d85-121">Kolumna C: Skrót sprzętowy</span><span class="sxs-lookup"><span data-stu-id="97d85-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="97d85-122">Możesz uzyskać te informacje od producenta komputera lub użyć [skryptu programu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), który wygeneruje plik CSV.</span><span class="sxs-lookup"><span data-stu-id="97d85-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="97d85-p102">Aby uzyskać więcej informacji, zobacz [Lista urządzeń w pliku CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Możesz również pobrać przykładowy plik na stronie **Przekazywanie pliku csv z listą urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="97d85-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="97d85-p103">Na stronie **Przypisywanie profilu** możesz utworzyć nowy lub wybrać istniejący profil. Jeśli nie masz jeszcze profilu, zostanie wyświetlony monit o jego utworzenie.</span><span class="sxs-lookup"><span data-stu-id="97d85-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="97d85-127">Profil to kolekcja ustawień, które można zastosować do jednego urządzenia lub do grupy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="97d85-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="97d85-p104">Funkcje domyślne są wymagane i zostaną ustawione automatycznie. Funkcje domyślne to:</span><span class="sxs-lookup"><span data-stu-id="97d85-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="97d85-130">Rejestracja Cortany, usługi OneDrive i producenta OEM jest pomijana.</span><span class="sxs-lookup"><span data-stu-id="97d85-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="97d85-131">Tworzenie środowiska logowania z marką Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="97d85-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="97d85-132">Urządzenia zostaną połączone z kontami usługi Azure Active Directory i automatycznie zarejestrowane na potrzeby zarządzania przez usługę Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="97d85-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="97d85-133">Aby uzyskać więcej informacji, zobacz</span><span class="sxs-lookup"><span data-stu-id="97d85-133">For more information, see</span></span>
    
    <span data-ttu-id="97d85-134">[Ustawienia profilu rozwiązania AutoPilot  informacje](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="97d85-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="97d85-135">Pozostałe ustawienia to **Pomiń ustawienia prywatności** i **Nie zezwalaj użytkownikowi na zostanie administratorem lokalnym**. Oba są domyślnie **wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="97d85-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="97d85-136">Wybierz przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="97d85-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="97d85-p105">Wyświetlenie strony **Gotowe** oznacza, że utworzony (lub wybrany) profil zostanie zastosowany do grupy urządzeń utworzonej po przekazaniu listy urządzeń. Ustawienia te zostaną zastosowane przy następnym logowaniu się użytkowników tych urządzeń. Wybierz pozycję **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="97d85-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    