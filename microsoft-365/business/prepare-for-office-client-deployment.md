---
title: Przygotowywanie klienta pakietu Office do wdrożenia za pomocą platformy Microsoft 365 dla firm
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924232"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="35f01-103">Przygotowywanie klienta pakietu Office do wdrożenia za pomocą platformy Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="35f01-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="35f01-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="35f01-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="35f01-105">Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich</span><span class="sxs-lookup"><span data-stu-id="35f01-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="35f01-106">Za pomocą usługi Microsoft 365 Business Premium możesz automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i być na bieżąco z ich aktualizacjami.</span><span class="sxs-lookup"><span data-stu-id="35f01-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="35f01-107">Automatyczna instalacja działa najlepiej, jeśli komputer użytkownika końcowego znajduje się w systemie Windows 10 Business i:</span><span class="sxs-lookup"><span data-stu-id="35f01-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="35f01-108">nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).</span><span class="sxs-lookup"><span data-stu-id="35f01-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="35f01-109">lub</span><span class="sxs-lookup"><span data-stu-id="35f01-109">or</span></span>
    
- <span data-ttu-id="35f01-110">jest zainstalowana wersja Szybka instalacja pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="35f01-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="35f01-111">Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook).</span><span class="sxs-lookup"><span data-stu-id="35f01-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="35f01-112">Jeśli widzisz aktualizacje **pakietu Office,** jak pokazano na poniższej ilustracji, instalacja została wykonana przy użyciu technologii Click-to-Run.</span><span class="sxs-lookup"><span data-stu-id="35f01-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="35f01-114">**Kto korzysta z tej funkcji**</span><span class="sxs-lookup"><span data-stu-id="35f01-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="35f01-115">Użytkownik końcowy, którego komputer spełnia następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="35f01-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="35f01-116">**Ma**  licencję użytkownika systemu Windows 10 Business, aktywną licencję platformy Microsoft 365 dla firm i aktualizację systemu Windows 10 dla twórców oraz jest dołączany do usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="35f01-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="35f01-117">**Nie zawiera** 64-bitowych aplikacji pakietu Office (przykład: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="35f01-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="35f01-118">Jeśli 64-bitowe wersje aplikacji pakietu Office są wymagane, ta funkcja nie jest dobrym rozwiązaniem, ponieważ wyzwalanie 64-bitowej wersji 2016 pakietu Office w wersji Click-to-Run z konsoli administracyjnej platformy Microsoft 365 dla firm nie jest dostępne.</span><span class="sxs-lookup"><span data-stu-id="35f01-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="35f01-119">**Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project).</span><span class="sxs-lookup"><span data-stu-id="35f01-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="35f01-120">Usługa Microsoft 365 dla firm uaktualnia pakiet Office do wersji Click-to-Run pakietu Office 2016, która nie działa z aplikacjami autonomicznymi MSI pakietu Office 2016.</span><span class="sxs-lookup"><span data-stu-id="35f01-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="35f01-121">W poniższej tabeli przedstawiono działania, jakie mogą zostać podjąć użytkownicy końcowi/administratorzy w zależności od stanu ich rozpoczęcia, aby pomyślnie uruchomić 32-bitową wersję Technologii Kliknij, aby uruchomić wdrożenie pakietu Office z konsoli administracyjnej platformy Microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="35f01-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span><br/>


|<span data-ttu-id="35f01-122">Stan początkowy instalacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="35f01-122">Starting Office install status</span></span>|<span data-ttu-id="35f01-123">Akcja do podjęcia przed zainstalowaniem pakietu Office na platformie Microsoft 365 dla firm</span><span class="sxs-lookup"><span data-stu-id="35f01-123">Action to take before Microsoft 365 for business Office install</span></span>|<span data-ttu-id="35f01-124">Stan końcowy</span><span class="sxs-lookup"><span data-stu-id="35f01-124">End state</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="35f01-125">Brak zainstalowanego pakietu Office</span><span class="sxs-lookup"><span data-stu-id="35f01-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="35f01-126">Brak</span><span class="sxs-lookup"><span data-stu-id="35f01-126">None</span></span>  <br/> |<span data-ttu-id="35f01-127">32-bitowy pakiet Office 2016 jest instalowany przy użyciu technologii Click-to-Run</span><span class="sxs-lookup"><span data-stu-id="35f01-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="35f01-128">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych</span><span class="sxs-lookup"><span data-stu-id="35f01-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="35f01-129">Brak</span><span class="sxs-lookup"><span data-stu-id="35f01-129">None</span></span>  <br/> |<span data-ttu-id="35f01-130">Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\***</span><span class="sxs-lookup"><span data-stu-id="35f01-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="35f01-131">Istniejąca 32-bitowa wersja Click-to-Run pakietu Office i 32-bitowe lub 64-bitowe aplikacje autonomiczne pakietu Office w wersji Click-to-Run (na przykład Visio lub Project)</span><span class="sxs-lookup"><span data-stu-id="35f01-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="35f01-132">Brak</span><span class="sxs-lookup"><span data-stu-id="35f01-132">None</span></span>  <br/> |<span data-ttu-id="35f01-133">Nie wpływa to na aplikacje autonomiczne.</span><span class="sxs-lookup"><span data-stu-id="35f01-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="35f01-134">Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="35f01-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="35f01-135">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)</span><span class="sxs-lookup"><span data-stu-id="35f01-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="35f01-136">Brak</span><span class="sxs-lookup"><span data-stu-id="35f01-136">None</span></span>  <br/> |<span data-ttu-id="35f01-137">Nie wpływa to na aplikacje autonomiczne.</span><span class="sxs-lookup"><span data-stu-id="35f01-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="35f01-138">Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="35f01-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="35f01-139">Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office</span><span class="sxs-lookup"><span data-stu-id="35f01-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="35f01-140">Odinstaluj 64-bitowe aplikacje pakietu Office, jeśli można je zamienić na 32-bitowe aplikacje pakietu Office</span><span class="sxs-lookup"><span data-stu-id="35f01-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="35f01-141">Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="35f01-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="35f01-142">Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich</span><span class="sxs-lookup"><span data-stu-id="35f01-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="35f01-143">Odinstalowanie pakietu Office 2016 w wersji MSI.</span><span class="sxs-lookup"><span data-stu-id="35f01-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="35f01-p106">Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych</span><span class="sxs-lookup"><span data-stu-id="35f01-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="35f01-146">Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office</span><span class="sxs-lookup"><span data-stu-id="35f01-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="35f01-147">Brak</span><span class="sxs-lookup"><span data-stu-id="35f01-147">None</span></span>  <br/> |<span data-ttu-id="35f01-148">32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle</span><span class="sxs-lookup"><span data-stu-id="35f01-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="35f01-149">**(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu.</span><span class="sxs-lookup"><span data-stu-id="35f01-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="35f01-150">Trwa prace nad poprawą.</span><span class="sxs-lookup"><span data-stu-id="35f01-150">A fix is in progress.</span></span> 
  
