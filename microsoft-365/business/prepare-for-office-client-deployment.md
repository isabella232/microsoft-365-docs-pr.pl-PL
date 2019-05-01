---
title: Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Dowiedz się, jak automatycznie zainstalować 32-bitowe aplikacje pakietu Office na komputerach systemu Windows 10 i je aktualizować.
ms.openlocfilehash: c8e93746b89925d6b6a928a474fe5736e2834987
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286661"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="b3db7-103">Przygotowywanie klienta pakietu Office do wdrożenia za pomocą usługi Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="b3db7-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="b3db7-104">Przygotowywanie się do automatycznej instalacji aplikacji pakietu Office na komputerach klienckich</span><span class="sxs-lookup"><span data-stu-id="b3db7-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="b3db7-105">Usługi Microsoft 365 Business umożliwiają automatyczne instalowanie 32-bitowych aplikacji pakietu Office i aktualizacji dla tych aplikacji na komputerach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b3db7-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="b3db7-106">To rozwiązanie działa najlepiej, gdy na komputerze użytkownika końcowego jest zainstalowany system Windows 10 Business oraz:</span><span class="sxs-lookup"><span data-stu-id="b3db7-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="b3db7-107">nie ma na nim aplikacji klasycznych pakietu Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access i usługi OneDrive).</span><span class="sxs-lookup"><span data-stu-id="b3db7-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="b3db7-108">lub</span><span class="sxs-lookup"><span data-stu-id="b3db7-108">or</span></span>
    
- <span data-ttu-id="b3db7-109">jest zainstalowana wersja Szybka instalacja pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="b3db7-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="b3db7-p101">Aby sprawdzić, czy korzystasz z wersji Szybka instalacja pakietu Office, w dowolnej aplikacji pakietu Office przejdź do lokalizacji **Plik** \> **Konto** ( **Konto pakietu Office** w programie Outlook). Jeśli zostaną wyświetlone aktualizacje pakietu Office, jak pokazano na poniższej ilustracji, oznacza to, że instalację przeprowadzono za pomocą modułu Szybka instalacja.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="b3db7-113">**Kto będzie korzystać z tej funkcji**</span><span class="sxs-lookup"><span data-stu-id="b3db7-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="b3db7-114">Użytkownik końcowy, którego komputer spełnia następujące kryteria:</span><span class="sxs-lookup"><span data-stu-id="b3db7-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="b3db7-115">**Zawiera** licencję użytkownika systemu Windows 10 Business i aktywną licencję usług Microsoft 365 Business oraz aktualizację dla twórców systemu Windows 10, a także jest dołączony do usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b3db7-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="b3db7-p102">**Nie zawiera** 64-bitowych wersji aplikacji pakietu Office (przykład: Word, Excel, PowerPoint). Jeśli 64-bitowe wersje aplikacji pakietu Office są wymagane, ta funkcja nie jest dobrym rozwiązaniem, ponieważ wyzwalanie 64-bitowego modułu Szybka instalacja pakietu Office w wersji 2016 z poziomu konsoli administracyjnej usług Microsoft 365 Business nie jest obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="b3db7-p103">**Nie zawiera** żadnych aplikacji autonomicznych Instalatora Windows (MSI) w wersji 2016 (na przykład Visio lub Project). Usługi Microsoft 365 Business umożliwiają uaktualnienie pakietu Office do wersji Szybka instalacja pakietu Office 2016, która nie współdziała z aplikacjami autonomicznymi MSI pakietu Office 2016.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="b3db7-120">W poniższej tabeli wyszczególniono możliwe działania, które użytkownicy końcowi lub administratorzy muszą wykonać w zależności od stanu początkowego, aby pomyślnie zainstalować 32-bitową wersję Szybka instalacja wdrożenia pakietu Office z poziomu konsoli administracyjnej usług Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b3db7-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="b3db7-121">**Stan początkowy instalacji pakietu Office**</span><span class="sxs-lookup"><span data-stu-id="b3db7-121">**Starting Office install status**</span></span>|<span data-ttu-id="b3db7-122">**Działanie do wykonania przed rozpoczęciem instalacji pakietu Office przy użyciu usług Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="b3db7-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="b3db7-123">**Stan końcowy**</span><span class="sxs-lookup"><span data-stu-id="b3db7-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b3db7-124">Brak zainstalowanego pakietu Office</span><span class="sxs-lookup"><span data-stu-id="b3db7-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="b3db7-125">Brak</span><span class="sxs-lookup"><span data-stu-id="b3db7-125">None</span></span>  <br/> |<span data-ttu-id="b3db7-126">Pakiet Office 2016 w wersji 32-bitowej zainstalowany za pomocą modułu Szybka instalacja</span><span class="sxs-lookup"><span data-stu-id="b3db7-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="b3db7-127">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office (w wersji 2016 lub wcześniejszej) bez aplikacji autonomicznych</span><span class="sxs-lookup"><span data-stu-id="b3db7-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="b3db7-128">Brak</span><span class="sxs-lookup"><span data-stu-id="b3db7-128">None</span></span>  <br/> |<span data-ttu-id="b3db7-129">Uaktualnienie do najnowszej 32-bitowej wersji Szybka instalacja pakietu Office 2016 zgodnie z wymaganiami **\***</span><span class="sxs-lookup"><span data-stu-id="b3db7-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="b3db7-130">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i 32- lub 64-bitowe aplikacje autonomiczne pakietu Office w wersji Szybka instalacja (na przykład Visio lub Project)</span><span class="sxs-lookup"><span data-stu-id="b3db7-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="b3db7-131">Brak</span><span class="sxs-lookup"><span data-stu-id="b3db7-131">None</span></span>  <br/> |<span data-ttu-id="b3db7-p104">Aplikacje autonomiczne pozostają nienaruszone. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="b3db7-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="b3db7-134">Istniejąca 32-bitowa wersja Szybka instalacja pakietu Office i dowolne 32- lub 64-bitowe aplikacje autonomiczne MSI pakietu Office (z wyjątkiem wersji 2016)</span><span class="sxs-lookup"><span data-stu-id="b3db7-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="b3db7-135">Brak</span><span class="sxs-lookup"><span data-stu-id="b3db7-135">None</span></span>  <br/> |<span data-ttu-id="b3db7-p105">Aplikacje autonomiczne pozostają nienaruszone. Uaktualnienie pakietu do 32-bitowej wersji Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="b3db7-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="b3db7-138">Dowolna istniejąca 64-bitowa wersja Szybka instalacja pakietu Office</span><span class="sxs-lookup"><span data-stu-id="b3db7-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="b3db7-139">Odinstalowanie 64-bitowych wersji aplikacji pakietu Office, jeśli można je zamienić na 32-bitowe wersje aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="b3db7-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="b3db7-140">Jeśli 64-bitowe wersje aplikacji pakietu Office zostaną usunięte, zostanie zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016</span><span class="sxs-lookup"><span data-stu-id="b3db7-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="b3db7-141">Istniejąca instalacja MSI pakietu Office 2016 z aplikacjami autonomicznymi lub bez nich</span><span class="sxs-lookup"><span data-stu-id="b3db7-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="b3db7-142">Odinstalowanie pakietu Office 2016 w wersji MSI.</span><span class="sxs-lookup"><span data-stu-id="b3db7-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="b3db7-p106">Zainstalowana 32-bitowa wersja Szybka instalacja pakietu Office 2016. Brak zmian w aplikacjach autonomicznych</span><span class="sxs-lookup"><span data-stu-id="b3db7-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="b3db7-145">Istniejąca instalacja MSI pakietu Office 2013 (lub starszego) i/lub aplikacji autonomicznych pakietu Office</span><span class="sxs-lookup"><span data-stu-id="b3db7-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="b3db7-146">Brak</span><span class="sxs-lookup"><span data-stu-id="b3db7-146">None</span></span>  <br/> |<span data-ttu-id="b3db7-147">32-bitowa wersja Szybka instalacja pakietu Office 2016 i istniejąca wcześniej instalacja MSI pakietu Office (z aplikacjami autonomicznymi) istnieją równolegle</span><span class="sxs-lookup"><span data-stu-id="b3db7-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="b3db7-p107">**(\*) Uwaga:** Nie można przeprowadzić uaktualnienia do 32-bitowej wersji Szybka instalacja pakietu Office 2016 z powodu znanego błędu. Trwa opracowywanie rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  

