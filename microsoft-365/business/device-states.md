---
title: Stany urządzeń
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Dowiedz się więcej o różnych stanach urządzeń na liście Akcje urządzenia w domu administratora w usłudze Microsoft 365 dla firm.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471184"
---
# <a name="device-states"></a><span data-ttu-id="fb488-103">Stany urządzeń</span><span class="sxs-lookup"><span data-stu-id="fb488-103">Device states</span></span>

<span data-ttu-id="fb488-104">Ten artykuł dotyczy usługi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fb488-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="fb488-105">Urządzenia znajdujące się na liście **Akcje urządzenia** (Administrator  strona główna \> **Akcje urządzenia**) mogą mieć następujące stany.</span><span class="sxs-lookup"><span data-stu-id="fb488-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="fb488-107">**Stan**</span><span class="sxs-lookup"><span data-stu-id="fb488-107">**Status**</span></span>|<span data-ttu-id="fb488-108">**Opis**</span><span class="sxs-lookup"><span data-stu-id="fb488-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb488-109">Zarządzane przez usługę Intune</span><span class="sxs-lookup"><span data-stu-id="fb488-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="fb488-110">Zarządzane przez usługę Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fb488-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="fb488-111">Oczekiwanie na wycofanie</span><span class="sxs-lookup"><span data-stu-id="fb488-111">Retire pending</span></span>  <br/> |<span data-ttu-id="fb488-112">Usługa Microsoft 365 Business Premium przygotowuje się do usunięcia danych firmowych z urządzenia.</span><span class="sxs-lookup"><span data-stu-id="fb488-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fb488-113">Wycofywanie w toku</span><span class="sxs-lookup"><span data-stu-id="fb488-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="fb488-114">Usługa Microsoft 365 Business Premium obecnie usuwa dane firmowe z urządzenia.</span><span class="sxs-lookup"><span data-stu-id="fb488-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fb488-115">Wycofywanie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="fb488-115">Retire failed</span></span>  <br/> | <span data-ttu-id="fb488-116">Akcja usuwania danych firmy nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="fb488-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="fb488-117">Wycofaj anulowano</span><span class="sxs-lookup"><span data-stu-id="fb488-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="fb488-118">Działanie na emeryturę zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="fb488-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="fb488-119">Oczekiwanie na wyczyszczenie</span><span class="sxs-lookup"><span data-stu-id="fb488-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="fb488-120">Trwa oczekiwanie na rozpoczęcie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="fb488-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="fb488-121">Czyszczenie w toku</span><span class="sxs-lookup"><span data-stu-id="fb488-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="fb488-122">Wywołano polecenie przywracania ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="fb488-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="fb488-123">Czyszczenie nie powiodło się</span><span class="sxs-lookup"><span data-stu-id="fb488-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="fb488-124">Nie można przywrócić ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="fb488-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="fb488-125">Wyczyść anulowane</span><span class="sxs-lookup"><span data-stu-id="fb488-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="fb488-126">Czyszczenie fabryczne zostało anulowane.</span><span class="sxs-lookup"><span data-stu-id="fb488-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="fb488-127">Zła kondycja</span><span class="sxs-lookup"><span data-stu-id="fb488-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="fb488-128">Akcja jest w toku (lub w toku), ale urządzenie nie zostało zaewidencjonowane przez ponad 30 dni.</span><span class="sxs-lookup"><span data-stu-id="fb488-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="fb488-129">Oczekiwanie na usunięcie</span><span class="sxs-lookup"><span data-stu-id="fb488-129">Delete pending</span></span>  <br/> |<span data-ttu-id="fb488-130">Trwa oczekiwanie na akcję usuwania.</span><span class="sxs-lookup"><span data-stu-id="fb488-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="fb488-131">Odnaleziono</span><span class="sxs-lookup"><span data-stu-id="fb488-131">Discovered</span></span>  <br/> |<span data-ttu-id="fb488-132">Usługa Microsoft 365 Business Premium wykryła urządzenie.</span><span class="sxs-lookup"><span data-stu-id="fb488-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
