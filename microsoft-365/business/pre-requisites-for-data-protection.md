---
title: Wymagania wstępne dotyczące ochrony danych na urządzeniach za pomocą usługi Microsoft 365 dla firm
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
ms.assetid: 7770e280-3a6c-436f-a157-b008a2744f51
description: Dowiedz się więcej o wymaganiach dotyczących konfigurowania organizacji za pomocą usługi Microsoft 365 dla firm i ochrony danych służbowych na urządzeniach użytkowników.
ms.openlocfilehash: 237825d2c2683bb6e71ae2fd31f8a25b1aa85ff7
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785897"
---
# <a name="prerequisites-for-protecting-data-on-devices-with-microsoft-365-for-business"></a><span data-ttu-id="09f5a-103">Wymagania wstępne dotyczące ochrony danych na urządzeniach za pomocą usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="09f5a-103">Prerequisites for protecting data on devices with Microsoft 365 for business</span></span>

<span data-ttu-id="09f5a-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="09f5a-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="09f5a-105">Pierwszym krokiem w konfigurowaniu organizacji za pomocą usługi Microsoft 365 dla firm jest upewnienie się, że można spełnić wymagania wstępne.</span><span class="sxs-lookup"><span data-stu-id="09f5a-105">The first step in setting up your organization with Microsoft 365 for business is to make sure you can meet the prerequisites.</span></span>
  
## <a name="requirements-for-setting-up-your-organization-with-microsoft-365-for-business"></a><span data-ttu-id="09f5a-106">Wymagania dotyczące konfigurowania organizacji za pomocą usługi Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="09f5a-106">Requirements for setting up your organization with Microsoft 365 for business</span></span>

- <span data-ttu-id="09f5a-107">Urządzenia z systemem Windows muszą korzystać z wersji Windows 7 Professional, Windows 8 Pro lub Windows 8.1 Pro.</span><span class="sxs-lookup"><span data-stu-id="09f5a-107">Windows devices must be running Windows 7 Professional, Windows 8 Pro, or Windows 8.1 Pro.</span></span>
    
    [<span data-ttu-id="09f5a-108">Uaktualnianie urządzeń z systemem Windows do systemu Windows Pro (aktualizacja dla twórców)</span><span class="sxs-lookup"><span data-stu-id="09f5a-108">Upgrade Windows devices to Windows Pro Creators Update</span></span>](upgrade-to-windows-pro-creators-update.md)
    
    <span data-ttu-id="09f5a-109">Jeśli korzystasz z systemu Windows 10 Home, musisz **kupić system** Windows 10 Pro.</span><span class="sxs-lookup"><span data-stu-id="09f5a-109">If you're running Windows 10 Home, then you must **purchase** Windows  10 Pro.</span></span> <span data-ttu-id="09f5a-110">Aby uzyskać instrukcje, zobacz [uaktualnianie systemu Windows 10 Home do systemu Windows 10 Pro.](https://support.microsoft.com/office/0aee10c1-4d34-43ee-a325-579c6c2df90e)</span><span class="sxs-lookup"><span data-stu-id="09f5a-110">See [upgrade Windows 10 Home to Windows 10 Pro](https://support.microsoft.com/office/0aee10c1-4d34-43ee-a325-579c6c2df90e) for instructions.</span></span> 
    
- <span data-ttu-id="09f5a-111">Usuń urządzenia z rozwiązań do zarządzania urządzeniami mobilnymi (Mobile Iron, AirWatch i tak dalej).</span><span class="sxs-lookup"><span data-stu-id="09f5a-111">Remove devices from mobile management solutions (Mobile Iron, AirWatch, and so on).</span></span> <span data-ttu-id="09f5a-112">W usłudze Microsoft 365 dla firm mobilnych zarządzania zostanie zarejestrowana wszystkie osoby w organizacji.</span><span class="sxs-lookup"><span data-stu-id="09f5a-112">You'll enroll all the people in your organization in Microsoft 365 for business mobile management.</span></span>
    
- <span data-ttu-id="09f5a-113">System Apple iOS 8.0 lub nowszy.</span><span class="sxs-lookup"><span data-stu-id="09f5a-113">Apple iOS 8.0 and later.</span></span>
    
    <span data-ttu-id="09f5a-114">System Google Android 4.0 lub nowszy (z uwzględnieniem wersji Samsung KNOX Standard 4.0 lub nowszej).</span><span class="sxs-lookup"><span data-stu-id="09f5a-114">Google Android 4.0 and later (including Samsung KNOX Standard 4.0 and higher).</span></span> <span data-ttu-id="09f5a-115">Aby uzyskać więcej informacji, zobacz [Obsługiwane urządzenia usługi Intune](https://go.microsoft.com/fwlink/p/?linkid=852307).</span><span class="sxs-lookup"><span data-stu-id="09f5a-115">For more information, see [Intune supported devices](https://go.microsoft.com/fwlink/p/?linkid=852307).</span></span>
    
- <span data-ttu-id="09f5a-116">Jeśli masz istniejące aplikacje pakietu Office na komputerach użytkowników, przeczytaj instrukcje przygotowania do [instalacji klienta pakietu Office,](prepare-for-office-client-deployment.md) aby zapoznać się z krokami, które mogą być konieczne przed skonfigurowaniem usługi Microsoft 365 dla firm w celu zainstalowania pakietu Office 2016 na komputerach użytkowników.</span><span class="sxs-lookup"><span data-stu-id="09f5a-116">If you have existing Office applications on user computers, read [prepare for Office client installation](prepare-for-office-client-deployment.md) to understand steps you might need to take before you can set up Microsoft 365 for business to install Office 2016 on user computers.</span></span> 
