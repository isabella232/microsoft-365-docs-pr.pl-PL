---
title: Przygotowanie do wdrożenia klienta pakietu Office przez usługę Microsoft 365 dla firm
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Dowiedz się, jak automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i aktualizować je.
ms.openlocfilehash: 6f3a80be9729a3818607c0f42e2cc7ece66a07ee
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401327"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="eae9b-103">Przygotowanie do wdrożenia klienta pakietu Office przez usługę Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="eae9b-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="eae9b-104">Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich</span><span class="sxs-lookup"><span data-stu-id="eae9b-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="eae9b-105">Za pomocą usługi Microsoft 365 dla firm można automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i utrzymywać je na bieżąco z aktualizacjami.</span><span class="sxs-lookup"><span data-stu-id="eae9b-105">You can use Microsoft 365 for business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="eae9b-106">Automatyczna instalacja działa najlepiej, jeśli komputer użytkownika końcowego jest w systemie Windows 10 Business i:</span><span class="sxs-lookup"><span data-stu-id="eae9b-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="eae9b-107">nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).</span><span class="sxs-lookup"><span data-stu-id="eae9b-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="eae9b-108">lub</span><span class="sxs-lookup"><span data-stu-id="eae9b-108">or</span></span>
    
- <span data-ttu-id="eae9b-109">jest zainstalowana wersja Szybka instalacja pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="eae9b-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="eae9b-110">Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook).</span><span class="sxs-lookup"><span data-stu-id="eae9b-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="eae9b-111">Jeśli widzisz **aktualizacje pakietu Office,** jak pokazano na poniższym rysunku, instalacja została wykonana przy użyciu funkcji Szybka instalacja.</span><span class="sxs-lookup"><span data-stu-id="eae9b-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="eae9b-113">**Kto korzysta z posiadania tej funkcji**</span><span class="sxs-lookup"><span data-stu-id="eae9b-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="eae9b-114">Użytkownik końcowy, którego komputer spełnia następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="eae9b-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="eae9b-115">**Ma** licencję użytkownika systemu Windows 10 Business, aktywną licencję microsoft 365 dla firm, windows 10 Creators Update i jest przyłączony do usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eae9b-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="eae9b-116">**Nie ma** 64-bitowych aplikacji pakietu Office (np.</span><span class="sxs-lookup"><span data-stu-id="eae9b-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="eae9b-117">Jeśli wymagane są 64-bitowe aplikacje pakietu Office, ta funkcja nie jest dobrym rozwiązaniem, ponieważ nie ma obsługi wyzwalania 64-bitowej wersji pakietu Office typu Szybka, aby uruchomić pakiet Office z konsoli administracyjnej usługi Microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="eae9b-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="eae9b-118">**Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project).</span><span class="sxs-lookup"><span data-stu-id="eae9b-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="eae9b-119">Usługa Microsoft 365 dla firm uaktualnia pakiet Office do wersji szybka obsługa pakietu Office 2016 i nie działa z autonomicznymi aplikacjami MSI pakietu Office 2016.</span><span class="sxs-lookup"><span data-stu-id="eae9b-119">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="eae9b-120">W poniższej tabeli przedstawiono, jakie działania użytkownicy końcowi/administratorzy mogą wymagać, w zależności od stanu początkowego, aby mieć pomyślną 32-bitową wersję szybka wdrożenia pakietu Office z konsoli administracyjnej usługi Microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="eae9b-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="eae9b-121">**Stan początkowy instalacji pakietu Office**</span><span class="sxs-lookup"><span data-stu-id="eae9b-121">**Starting Office install status**</span></span>|<span data-ttu-id="eae9b-122">**Działania, które należy podjąć przed zainstalowaniem pakietu Microsoft 365 dla firm Office**</span><span class="sxs-lookup"><span data-stu-id="eae9b-122">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="eae9b-123">**Stan końcowy**</span><span class="sxs-lookup"><span data-stu-id="eae9b-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="eae9b-124">Brak zainstalowanego pakietu Office</span><span class="sxs-lookup"><span data-stu-id="eae9b-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="eae9b-125">Brak</span><span class="sxs-lookup"><span data-stu-id="eae9b-125">None</span></span>  <br/> |<span data-ttu-id="eae9b-126">32-bitowy pakiet Office 2016 jest instalowany przy użyciu funkcji Szybka instalacja</span><span class="sxs-lookup"><span data-stu-id="eae9b-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="eae9b-127">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych</span><span class="sxs-lookup"><span data-stu-id="eae9b-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="eae9b-128">Brak</span><span class="sxs-lookup"><span data-stu-id="eae9b-128">None</span></span>  <br/> |<span data-ttu-id="eae9b-129">Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\***</span><span class="sxs-lookup"><span data-stu-id="eae9b-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="eae9b-130">Istniejąca 32-bitowa wersja pakietu Click-to-Run pakietu Office i 32-bitowe lub 64-bitowe autonomiczne aplikacje pakietu Office (na przykład Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="eae9b-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="eae9b-131">Brak</span><span class="sxs-lookup"><span data-stu-id="eae9b-131">None</span></span>  <br/> |<span data-ttu-id="eae9b-132">Nie ma to wpływu na aplikacje autonomiczne.</span><span class="sxs-lookup"><span data-stu-id="eae9b-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="eae9b-133">Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="eae9b-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="eae9b-134">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)</span><span class="sxs-lookup"><span data-stu-id="eae9b-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="eae9b-135">Brak</span><span class="sxs-lookup"><span data-stu-id="eae9b-135">None</span></span>  <br/> |<span data-ttu-id="eae9b-136">Nie ma to wpływu na aplikacje autonomiczne.</span><span class="sxs-lookup"><span data-stu-id="eae9b-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="eae9b-137">Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="eae9b-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="eae9b-138">Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office</span><span class="sxs-lookup"><span data-stu-id="eae9b-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="eae9b-139">Odinstalowywanie 64-bitowych aplikacji pakietu Office, jeśli można je zastąpić 32-bitowymi aplikacjami pakietu Office</span><span class="sxs-lookup"><span data-stu-id="eae9b-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="eae9b-140">Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="eae9b-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="eae9b-141">Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich</span><span class="sxs-lookup"><span data-stu-id="eae9b-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="eae9b-142">Odinstalowanie pakietu Office 2016 w wersji MSI.</span><span class="sxs-lookup"><span data-stu-id="eae9b-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="eae9b-p106">Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych</span><span class="sxs-lookup"><span data-stu-id="eae9b-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="eae9b-145">Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office</span><span class="sxs-lookup"><span data-stu-id="eae9b-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="eae9b-146">Brak</span><span class="sxs-lookup"><span data-stu-id="eae9b-146">None</span></span>  <br/> |<span data-ttu-id="eae9b-147">32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle</span><span class="sxs-lookup"><span data-stu-id="eae9b-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="eae9b-148">**(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu.</span><span class="sxs-lookup"><span data-stu-id="eae9b-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="eae9b-149">Poprawka jest w toku.</span><span class="sxs-lookup"><span data-stu-id="eae9b-149">A fix is in progress.</span></span> 
  
