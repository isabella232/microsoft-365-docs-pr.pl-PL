---
title: Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Dowiedz się, jak tworzyć zasady zarządzania aplikacjami i chronić pliki służbowe na osobistych urządzeniach z systemem Windows 10 użytkowników.
ms.openlocfilehash: ce389980ceb8bd889214404b0c48769380044bcf
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550212"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="a453b-103">Konfigurowanie ustawień ochrony aplikacji dla urządzeń z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="a453b-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="a453b-104">Tworzenie zasad zarządzania aplikacjami dla systemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="a453b-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="a453b-105">Jeśli użytkownicy mają urządzenia osobiste z systemem Windows 10, na których wykonują zadania służbowe, możesz również chronić dane na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="a453b-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="a453b-106">Przejdź do centrum <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>administracyjnego pod adresem .</span><span class="sxs-lookup"><span data-stu-id="a453b-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="a453b-107">Na lewym urządzeniu nawigacyjnym wybierz pozycję Dodaj **zasady** \> **urządzeń** \> **.**</span><span class="sxs-lookup"><span data-stu-id="a453b-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="a453b-108">W okienku **Dodawanie zasad** wprowadź unikatową nazwę dla zasad.</span><span class="sxs-lookup"><span data-stu-id="a453b-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="a453b-109">W sekcji **Typ zasad** wybierz pozycję **Zarządzanie aplikacjami dla systemu Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="a453b-109">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="a453b-110">W **obszarze Typ urządzenia**wybierz opcję **Osobiste** lub Należące **do firmy**.</span><span class="sxs-lookup"><span data-stu-id="a453b-110">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="a453b-111">Opcja **Szyfruj pliki służbowe** zostanie włączona automatycznie.</span><span class="sxs-lookup"><span data-stu-id="a453b-111">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="a453b-112">Jeśli nie chcesz, aby użytkownicy mogli zapisywać pliki służbowe na swoich komputerach, **włącz** ustawienie **Uniemożliw użytkownikom kopiowanie danych firmy do plików osobistych i wymuś na nich zapisywanie plików służbowych w usłudze OneDrive dla Firm**.</span><span class="sxs-lookup"><span data-stu-id="a453b-112">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="a453b-113">Rozwiń **odzyskiwanie danych na urządzeniach z systemem Windows**.</span><span class="sxs-lookup"><span data-stu-id="a453b-113">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="a453b-114">Zalecamy włączenie **go**.</span><span class="sxs-lookup"><span data-stu-id="a453b-114">We recommend that you turn it **On**.</span></span>
    
    <span data-ttu-id="a453b-115">Aby móc przejść do lokalizacji certyfikatu agenta odzyskiwania danych, musisz najpierw go utworzyć.</span><span class="sxs-lookup"><span data-stu-id="a453b-115">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="a453b-116">Aby uzyskać instrukcje, zobacz [Tworzenie i weryfikowanie certyfikatu agenta odzyskiwania danych (EFS) systemu szyfrowania plików (EFS).](https://go.microsoft.com/fwlink/p/?linkid=853700)</span><span class="sxs-lookup"><span data-stu-id="a453b-116">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="a453b-117">Domyślnie pliki robocze są szyfrowane przy użyciu klucza tajnego, który jest przechowywany na urządzeniu i skojarzony z profilem użytkownika.</span><span class="sxs-lookup"><span data-stu-id="a453b-117">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="a453b-118">Tylko użytkownik może otwierać i odszyfrowywać plik.</span><span class="sxs-lookup"><span data-stu-id="a453b-118">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="a453b-119">Jednak w razie utraty urządzenia lub usunięcia użytkownika plik może utknąć w stanie zaszyfrowania.</span><span class="sxs-lookup"><span data-stu-id="a453b-119">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="a453b-120">Administrator może odszyfrować plik za pomocą certyfikatu agenta odzyskiwania danych (DRA).</span><span class="sxs-lookup"><span data-stu-id="a453b-120">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="a453b-122">Rozwiń **Chroń dodatkowe lokalizacje sieci i chmury,** jeśli chcesz dodać dodatkowe domeny lub lokalizacje usługi SharePoint Online, aby upewnić się, że pliki we wszystkich wymienionych aplikacjach są chronione.</span><span class="sxs-lookup"><span data-stu-id="a453b-122">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="a453b-123">Jeśli chcesz wprowadzić więcej niż jeden element dla jednego pola, użyj średnika (;) między elementami.</span><span class="sxs-lookup"><span data-stu-id="a453b-123">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="a453b-p105">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="a453b-p105">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="a453b-127">Na koniec wybierz przycisk **Dodaj**, aby zapisać zasady i zastosować je na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="a453b-127">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
