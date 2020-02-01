---
title: Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Dowiedz się, jak automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i aktualizować je.
ms.openlocfilehash: fa5b2ce1852ebdb1e76c1fa844793fee56af3d68
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593624"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="47e23-103">Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="47e23-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="47e23-104">Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich</span><span class="sxs-lookup"><span data-stu-id="47e23-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="47e23-105">Za pomocą usługi Microsoft 365 Business można automatycznie instalować 32-bitowe aplikacje pakietu Office na komputerach z systemem Windows 10 i aktualizować je z aktualizacjami.</span><span class="sxs-lookup"><span data-stu-id="47e23-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="47e23-106">Instalacja automatyczna działa najlepiej, jeśli komputer użytkownika końcowego jest w systemie Windows 10 Business i:</span><span class="sxs-lookup"><span data-stu-id="47e23-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="47e23-107">nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).</span><span class="sxs-lookup"><span data-stu-id="47e23-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="47e23-108">lub</span><span class="sxs-lookup"><span data-stu-id="47e23-108">or</span></span>
    
- <span data-ttu-id="47e23-109">jest zainstalowana wersja Szybka instalacja pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="47e23-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="47e23-110">Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook).</span><span class="sxs-lookup"><span data-stu-id="47e23-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="47e23-111">Jeśli widzisz **aktualizacje pakietu Office,** jak pokazano na poniższym rysunku, instalacja została wykonana przy użyciu funkcji Szybka instalacja.</span><span class="sxs-lookup"><span data-stu-id="47e23-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="47e23-113">**Kto korzysta z tej funkcji**</span><span class="sxs-lookup"><span data-stu-id="47e23-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="47e23-114">Użytkownik końcowy, którego komputer spełnia następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="47e23-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="47e23-115">**Zawiera** licencję użytkownika systemu Windows 10 Business i aktywną licencję usług Microsoft 365 Business oraz aktualizację dla twórców systemu Windows 10, a także jest dołączony do usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="47e23-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="47e23-116">**Nie ma** 64-bitowych aplikacji pakietu Office (np. programów Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="47e23-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="47e23-117">Jeśli wymagane są 64-bitowe aplikacje pakietu Office, ta funkcja nie jest odpowiednia, ponieważ nie ma obsługi wyzwalania 64-bitowej wersji pakietu Office "Kliknij, aby uruchomić" z konsoli administracyjnej programu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="47e23-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="47e23-118">**Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project).</span><span class="sxs-lookup"><span data-stu-id="47e23-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="47e23-119">Usługa Microsoft 365 Business uaktualnia pakiet Office do wersji "Kliknij, aby uruchomić pakiet Office 2016" i nie działa z autonomicznymi aplikacjami usługi MSI pakietu Office 2016.</span><span class="sxs-lookup"><span data-stu-id="47e23-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="47e23-120">W poniższej tabeli przedstawiono, jaką akcję mogą podjąć użytkownicy końcowi/administratorzy, w zależności od stanu początkowego, aby mieć pomyślną 32-bitową wersję wdrożenia pakietu Office typu "Kliknij, aby uruchomić" z konsoli administracyjnej programu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="47e23-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="47e23-121">**Stan początkowy instalacji pakietu Office**</span><span class="sxs-lookup"><span data-stu-id="47e23-121">**Starting Office install status**</span></span>|<span data-ttu-id="47e23-122">**Działanie do wykonania przed rozpoczęciem instalacji pakietu Office przy użyciu usług Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="47e23-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="47e23-123">**Stan końcowy**</span><span class="sxs-lookup"><span data-stu-id="47e23-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="47e23-124">Brak zainstalowanego pakietu Office</span><span class="sxs-lookup"><span data-stu-id="47e23-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="47e23-125">Brak</span><span class="sxs-lookup"><span data-stu-id="47e23-125">None</span></span>  <br/> |<span data-ttu-id="47e23-126">32-bitowy pakiet Office 2016 jest instalowany przy użyciu funkcji Szybka instalacja</span><span class="sxs-lookup"><span data-stu-id="47e23-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="47e23-127">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych</span><span class="sxs-lookup"><span data-stu-id="47e23-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="47e23-128">Brak</span><span class="sxs-lookup"><span data-stu-id="47e23-128">None</span></span>  <br/> |<span data-ttu-id="47e23-129">Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\***</span><span class="sxs-lookup"><span data-stu-id="47e23-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="47e23-130">Istniejące 32-bitowa wersja pakietu Office i uruchamianych 32-bitowych lub 64-bitowych aplikacji pakietu Office typu "Kliknij, aby uruchomić" (na przykład program Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="47e23-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="47e23-131">Brak</span><span class="sxs-lookup"><span data-stu-id="47e23-131">None</span></span>  <br/> |<span data-ttu-id="47e23-132">Nie ma to wpływu na aplikacje autonomiczne.</span><span class="sxs-lookup"><span data-stu-id="47e23-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="47e23-133">Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="47e23-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="47e23-134">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)</span><span class="sxs-lookup"><span data-stu-id="47e23-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="47e23-135">Brak</span><span class="sxs-lookup"><span data-stu-id="47e23-135">None</span></span>  <br/> |<span data-ttu-id="47e23-136">Nie ma to wpływu na aplikacje autonomiczne.</span><span class="sxs-lookup"><span data-stu-id="47e23-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="47e23-137">Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="47e23-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="47e23-138">Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office</span><span class="sxs-lookup"><span data-stu-id="47e23-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="47e23-139">Odinstaluj 64-bitowe aplikacje pakietu Office, jeśli można zastąpić je 32-bitowymi aplikacjami pakietu Office</span><span class="sxs-lookup"><span data-stu-id="47e23-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="47e23-140">Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="47e23-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="47e23-141">Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich</span><span class="sxs-lookup"><span data-stu-id="47e23-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="47e23-142">Odinstalowanie pakietu Office 2016 w wersji MSI.</span><span class="sxs-lookup"><span data-stu-id="47e23-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="47e23-p106">Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych</span><span class="sxs-lookup"><span data-stu-id="47e23-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="47e23-145">Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office</span><span class="sxs-lookup"><span data-stu-id="47e23-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="47e23-146">Brak</span><span class="sxs-lookup"><span data-stu-id="47e23-146">None</span></span>  <br/> |<span data-ttu-id="47e23-147">32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle</span><span class="sxs-lookup"><span data-stu-id="47e23-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="47e23-148">**(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu.</span><span class="sxs-lookup"><span data-stu-id="47e23-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="47e23-149">Trwa poprawka.</span><span class="sxs-lookup"><span data-stu-id="47e23-149">A fix is in progress.</span></span> 
  