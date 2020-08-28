---
title: Edytowanie lub Ustawianie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Dowiedz się, jak tworzyć lub edytować zasady zarządzania aplikacjami oraz chronić pliki służbowe na osobistych urządzeniach użytkowników z systemem Windows 10.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289204"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="fccf6-103">Ustawianie lub edytowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="fccf6-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="fccf6-104">Ten artykuł dotyczy programu Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fccf6-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="fccf6-105">Edytowanie zasad zarządzania aplikacjami dla systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="fccf6-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="fccf6-106">Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="fccf6-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="fccf6-107">Na lewym pasku nawigacyjnym wybierz pozycję Zasady dotyczące **urządzeń** \> **Policies** .</span><span class="sxs-lookup"><span data-stu-id="fccf6-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="fccf6-108">Wybierz istniejące zasady aplikacji systemu Windows, a następnie pozycję **Edytuj**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="fccf6-109">Wybierz pozycję **Edytuj** obok ustawienia, które chcesz zmienić, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="fccf6-110">Tworzenie zasad zarządzania aplikacjami dla systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="fccf6-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="fccf6-111">Jeśli użytkownicy mają urządzenia osobiste z systemem Windows 10, na których wykonują zadania służbowe, możesz również chronić dane na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="fccf6-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="fccf6-112">Przejdź do centrum administracyjnego <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="fccf6-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="fccf6-113">Na lewym pasku nawigacyjnym wybierz pozycję Zasady dotyczące **urządzeń** , \> **Policies** \> **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="fccf6-114">W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad.</span><span class="sxs-lookup"><span data-stu-id="fccf6-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="fccf6-115">W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="fccf6-116">W obszarze **Typ urządzenia**wybierz pozycję **osobisty** lub **firmowy własność**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="fccf6-117">Opcja **Szyfruj pliki służbowe** zostanie włączona automatycznie.</span><span class="sxs-lookup"><span data-stu-id="fccf6-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="fccf6-118">Jeśli nie chcesz, aby użytkownicy mogli zapisywać pliki służbowe na swoich komputerach, **włącz** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="fccf6-119">Rozwiń pozycję **Odzyskaj dane na urządzeniach z systemem Windows**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="fccf6-120">Zalecamy **włączenie tej opcji.**</span><span class="sxs-lookup"><span data-stu-id="fccf6-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="fccf6-121">Aby móc przejść do lokalizacji certyfikatu agenta odzyskiwania danych, musisz najpierw go utworzyć.</span><span class="sxs-lookup"><span data-stu-id="fccf6-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="fccf6-122">Aby uzyskać instrukcje, zobacz [Tworzenie i weryfikowanie certyfikatu agenta odzyskiwania danych (dra) na system szyfrowania plików (EFS)](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="fccf6-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="fccf6-123">Domyślnie pliki robocze są szyfrowane przy użyciu klucza tajnego, który jest przechowywany na urządzeniu i skojarzony z profilem użytkownika.</span><span class="sxs-lookup"><span data-stu-id="fccf6-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="fccf6-124">Tylko użytkownik może otwierać i odszyfrowywać plik.</span><span class="sxs-lookup"><span data-stu-id="fccf6-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="fccf6-125">Jednak w razie utraty urządzenia lub usunięcia użytkownika plik może utknąć w stanie zaszyfrowania.</span><span class="sxs-lookup"><span data-stu-id="fccf6-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="fccf6-126">Administrator może odszyfrować plik za pomocą certyfikatu agenta odzyskiwania danych (DRA).</span><span class="sxs-lookup"><span data-stu-id="fccf6-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="fccf6-128">Rozwiń pozycję **Chroń dodatkowe lokalizacje sieciowe i chmury** , jeśli chcesz dodać dodatkowe domeny lub lokalizacje usługi SharePoint Online, aby upewnić się, że pliki we wszystkich wymienionych aplikacjach są chronione.</span><span class="sxs-lookup"><span data-stu-id="fccf6-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="fccf6-129">Jeśli musisz wprowadzić więcej niż jeden element dla każdego pola, użyj średnika (;) między elementami.</span><span class="sxs-lookup"><span data-stu-id="fccf6-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="fccf6-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="fccf6-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="fccf6-133">Na koniec wybierz przycisk **Dodaj**, aby zapisać zasady i zastosować je na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="fccf6-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
