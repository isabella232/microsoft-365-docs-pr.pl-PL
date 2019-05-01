---
title: Automatyczne instalowanie i odinstalowywanie pakietu Office na urządzeniach z systemem Windows 10
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'Zainstalować lub odinstalować pakiet Office na urządzeniach Windows 10 z Centrum administracyjnego Microsoft 365 Business. '
ms.openlocfilehash: fef4a543aed489202bf05dfb1e8cafbb784ca819
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277296"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="9d2e3-103">Automatyczne instalowanie i odinstalowywanie pakietu Office na urządzeniach z systemem Windows 10</span><span class="sxs-lookup"><span data-stu-id="9d2e3-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="9d2e3-104">Centrum administracyjne usług Microsoft 365 Business pozwala szybko i łatwo zainstalować pakiet Office na komputerach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-104">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="9d2e3-105">Aby dowiedzieć się, jak to działa w przypadku wcześniej zainstalowanych aplikacji pakietu Office, przed rozpoczęciem przeczytaj artykuł na temat [przygotowywania się do instalacji aplikacji klienckich pakietu Office](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="9d2e3-105">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="9d2e3-106">Zarządzanie wdrożeniami pakietu Office</span><span class="sxs-lookup"><span data-stu-id="9d2e3-106">Manage Office deployments</span></span>

1. <span data-ttu-id="9d2e3-107">Zaloguj się do [centrum administracyjnego](https://aka.ms/bcsportal), korzystając z poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-107">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="9d2e3-108">Na karcie **Urządzenia** wybierz pozycję **Zarządzaj wdrożeniem pakietu Office**.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-108">On the **Devices** card, choose **Manage Office Deployment**.</span></span>
      <span data-ttu-id="9d2e3-109">Jeśli nie widzisz karty **działania urządzenia** w strony **głównej** Centrum admin kliknij przycisk **Dodaj** (+), aby dodać je do domu użytkownika admin.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-109">If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="9d2e3-111">W okienku **Zarządzaj wdrożeniem pakietu Office**, które zostanie otwarte, wybierz pozycję **Dodaj grupę**, a następnie wybierz grupy, których chcesz użyć.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-111">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="9d2e3-112">Po dodaniu grup wybierz z listy **Akcja wdrażania** pozycję **Zainstaluj pakiet Office jak najszybciej** lub **Odinstaluj pakiet Office**.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-112">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="9d2e3-114">Choose **Next** \> review the settings and then choose **Confirm**.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-114">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="9d2e3-115">32-bitowy pakiet Office zostanie automatycznie zainstalowany lub odinstalowany na urządzeniach należących do użytkowników określonych przez użyte grupy.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-115">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="9d2e3-116">Aby to sprawdzić, otwórz Menedżera zadań na komputerze wybranym na potrzeby instalacji pakietu Office i znajdź proces Szybka instalacja pakietu Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="9d2e3-116">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  

